---
title: コンテンツのネットワーク帯域幅の管理
titleSuffix: Configuration Manager
description: Configuration Manager のスケジューリング、帯域幅調整、および事前設定されたコンテンツを構成します。
ms.date: 02/6/2017
ms.prod: configuration-manager
ms.technology: configmgr-core
ms.topic: conceptual
ms.assetid: e80d1151-91db-4a27-8411-a957297b67d0
author: aczechowski
ms.author: aaroncz
manager: dougeby
ms.openlocfilehash: b8ee7d00f3b5c98528d9999b83b07aa393b72e36
ms.sourcegitcommit: bbf820c35414bf2cba356f30fe047c1a34c5384d
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/21/2020
ms.locfileid: "81704160"
---
# <a name="manage-network-bandwidth-for-content"></a>コンテンツのネットワーク帯域幅の管理
Configuration Manager のコンテンツ管理プロセスに使用されるネットワーク帯域幅を効率よく利用するには、スケジューリング用および帯域幅調整用の組み込みの制御機構を使用することができます。 事前設定されたコンテンツを使用することもできます。 以降のセクションでは、これらの方法について詳しく説明します。

##  <a name="scheduling-and-throttling"></a><a name="BKMK_PlanningForThrottling"></a>スケジュールと調整  

 パッケージの作成、コンテンツのソース パスの変更、または配布ポイントのコンテンツの更新を行うと、ファイルがソース パスからサイト サーバー上のコンテンツ ライブラリにコピーされます。 その後、コンテンツはサイト サーバー上のコンテンツ ライブラリから配布ポイント上のコンテンツ ライブラリにコピーされます。 コンテンツのソース ファイルが更新され、ソース ファイルが既に配布されている場合、Configuration Manager は新しいファイルまたは更新されたファイルのみを取得して、配布ポイントに送信します。

 サイト間の通信、およびサイト サーバーとリモート配布ポイント間の通信に対しては、スケジュールおよび調整の制御を使用できます。 スケジュールと帯域幅調整の制御機構をセットアップしたにもかかわらずネットワーク帯域幅が足りないと感じる場合は、配布ポイントにコンテンツを事前設定することを検討してください。  

 リモート配布ポイントに対して Configuration Manager からスケジュールを設定したり帯域幅調整を指定したりすることによって、いつどのようにコンテンツの配布を実行するかを設定することができます。 各リモート配布ポイントは、サイト サーバーとリモート配布ポイントの間のネットワーク帯域幅の制限に対応するために個別の構成にすることができます。 リモート配布ポイントに対するスケジューリングと帯域幅調整の制御は、標準センダー アドレスの設定に似ています。 この場合、設定は、Package Transfer Manager と呼ばれる新しいコンポーネントによって使用されます。

 Package Transfer Manager は、サイト サーバー (プライマリ サイトまたはセカンダリ サイト) からサイト システムにインストールされている配布ポイントにコンテンツを配布します。 サイト サーバー上にない配布ポイントに対しては、 **[転送率の制限]** タブで帯域幅調整設定を指定し、 **[スケジュール]** タブでスケジュール設定を指定します。 時刻の設定は、配布ポイントではなく、送信元のサイトのタイム ゾーンに基づきます。  

> [!IMPORTANT]  
>  **[転送率の制限]** タブおよび **[スケジュール]** タブは、サイト サーバーにインストールされていない配布ポイントのプロパティにのみ表示されます。  

詳細については、「[Configuration Manager の配布ポイントのインストールと構成](../../servers/deploy/configure/install-and-configure-distribution-points.md)」を参照してください。  

##  <a name="prestaged-content"></a><a name="BKMK_PrestagingContent"></a>事前設定されたコンテンツ  
 コンテンツを配布する前に、サイト サーバーのコンテンツ ライブラリまたは配布ポイントにコンテンツ ファイルを追加するための事前設定をすることができます。 コンテンツ ファイルは既にコンテンツ ライブラリに格納されているため、コンテンツを配布するときにネットワークを介してファイルが転送されることはありません。 アプリケーションおよびパッケージ用にコンテンツ ファイルを事前設定することができます。  

Configuration Manager コンソールで、事前設定するコンテンツを選択し、**事前設定コンテンツ ファイルの作成ウィザード**を使用します。 そのコンテンツのファイルや関連するメタデータが格納された、圧縮された事前設定コンテンツ ファイルがこのウィザードによって作成されます。 次に、サイト サーバーまたは配布ポイントで、コンテンツを手動でインポートすることができます。 次の点に注意してください。  

-   事前設定コンテンツ ファイルをサイト サーバーにインポートする場合、コンテンツ ファイルはサイト サーバーのコンテンツ ライブラリに追加され、サイト サーバー データベースに登録されます。  

-   事前設定されたコンテンツ ファイルを配布ポイントでインポートすると、配布ポイント上のコンテンツ ライブラリにそのコンテンツ ファイルが追加されます。 サイト サーバーにステータス メッセージが送信され、配布ポイント上にあってコンテンツが置かれているサイトが通知されます。  

必要に応じて、配布ポイントをコンテンツ配布を管理するために **事前設定済み** に構成することもできます。 次に、コンテンツを配布するときの操作を次の中から選択できます。  

-   配布ポイントのコンテンツを常に事前設定する。  

-   パッケージの初期コンテンツを事前設定し、コンテンツの更新があるときは標準のコンテンツ配布プロセスを使用する。  

-   パッケージのコンテンツに対して、常に標準のコンテンツ配布プロセスを使用する。  

###  <a name="determine-whether-to-prestage-content"></a><a name="BKMK_DetermineToPrestageContent"></a>コンテンツを事前設定するかどうかの判断  
 次のような場合は、アプリケーションおよびパッケージのコンテンツを事前設定することを検討してください。  

-   **サイト サーバーから配布ポイントへのネットワーク帯域幅不足の問題を解決する。** スケジューリングと帯域幅調整だけでは帯域幅の問題が解消されないおそれがある場合は、配布ポイントにコンテンツを事前設定することを検討してください。 各配布ポイントには、配布ポイントのプロパティで選択できる **[事前設定されたコンテンツ用にこの配布ポイントを有効にする]** 設定があります。 このオプションを有効にすると、配布ポイントは事前設定された配布ポイントとして識別され、パッケージごとにコンテンツを管理する方法を選択できます。  

    アプリケーション、パッケージ、ドライバー パッケージ、ブート イメージ、オペレーティング システム インストーラー、イメージのプロパティでは、以下の設定にアクセスできます。 これらの設定を通じて、事前設定された配布ポイントとして識別されたリモート配布ポイントにおけるコンテンツの配布方法を選択できます。  

    -   **[パッケージが配布ポイントに割り当てられたときにコンテンツを自動的にダウンロードする]** : このオプションは、スケジュール設定および調整設定でコンテンツの配布を十分に制御できる小さいパッケージの場合に使用します。  

    -   **[配布ポイントにコンテンツの変更箇所のみダウンロードする]** : このオプションは、将来そのパッケージ内のコンテンツに対して行われる更新が、当初のパッケージよりも概して小さいことが予想される場合に使用します。 たとえば、Microsoft Office のようなアプリケーションは、最初のパッケージ サイズが 700 MB 以上あり、ネットワークで送信するには大きすぎるため事前設定するようにします。 一方、このパッケージのコンテンツの更新ファイルは通常 10 MB 未満であるため、ネットワーク経由で配布できると考えられます。 別の例としてはドライバー パッケージがあります。最初のパッケージのサイズは大きくても、パッケージに追加される付加的なドライバーは小さい可能性があります。  

    -   **[このパッケージのコンテンツを配布ポイントに手動でコピーする]** : このオプションは、オペレーティング システムなどのコンテンツが含まれている大きなパッケージがあり、コンテンツを配布ポイントに配布するためにネットワークを使用しない場合に選択します。 このオプションを選択したら、コンテンツを配布ポイントに事前設定する必要があります。  

    > [!IMPORTANT]  
    >  上記のオプションは、パッケージごとに適用でき、配布ポイントにコンテンツが事前設定されている場合だけ使用されます。 事前設定されていない配布ポイントでは、上記の設定が無視されます。 この場合は、コンテンツがサイト サーバーから配布ポイントにネットワーク経由で配付されます。  

-   **サイト サーバーのコンテンツ ライブラリを復元する。** サイト サーバーで障害が発生した場合に、コンテンツ ライブラリに含まれているパッケージとアプリケーションに関する情報は復元処理の一部でサイト データベースに復元されますが、コンテンツ ライブラリ ファイルは復元されません。 コンテンツ ライブラリを復元するためのファイル システム バックアップがない場合は、必要なパッケージおよびアプリケーションが含まれている別のサイトから、事前設定のコンテンツ ファイルを作成します。 その後、回復したサイト サーバーに事前設定のコンテンツ ファイルを展開します。 サイト サーバーのバックアップおよび回復の詳細については、[Configuration Manager のバックアップと回復](../../servers/manage/backup-and-recovery.md)に関するページを参照してください。  