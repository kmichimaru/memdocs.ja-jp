---
title: Wake On LAN の構成
titleSuffix: Configuration Manager
description: Configuration Manager で Wake On LAN 設定を選択します。
ms.date: 04/01/2020
ms.prod: configuration-manager
ms.technology: configmgr-client
ms.topic: conceptual
ms.assetid: b475a0c8-85d6-4cc4-b11f-32c0cc98239e
author: mestew
ms.author: mstewart
manager: dougeby
ms.openlocfilehash: 512d942d79d11178f010c4f0adb41a25ee432743
ms.sourcegitcommit: bbf820c35414bf2cba356f30fe047c1a34c5384d
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/21/2020
ms.locfileid: "81694120"
---
# <a name="how-to-configure-wake-on-lan-in-configuration-manager"></a>Configuration Manager で Wake On LAN を構成する方法

*適用対象:Configuration Manager (Current Branch)*

スリープ状態からコンピューターを復帰させるための Wake On LAN 設定を Configuration Manager に指定します。

## <a name="wake-on-lan-starting-in-version-1810"></a><a name="bkmk_wol-1810"></a> バージョン 1810 以降の Wake on LAN
<!--3607710-->
Configuration Manager 1810 以降、新しい方法でスリープ状態のコンピューターを復帰させることができます。 クライアントとサイト サーバーのサブネットが異なる場合でも、Configuration Manager コンソールからクライアントを復帰させることができます。 メンテナンスを実行したり、デバイスにクエリを実行したりする必要がある場合、スリープ状態にあるリモート クライアントで制限されることがありません。 サイト サーバーでは、クライアント通知チャネルを利用し、同じリモート サブネット上で起動状態にある他のクライアントが識別されます。次に、そのクライアントを利用し、Wake On LAN 要求 (マジック パケット) が送信されます。 クライアント通知チャネルを利用することで MAC フラップが回避されます。MAC フラップは、ポートがルーターによってシャットダウンされる原因になることがあります。 新しいバージョンの Wake on LAN は[以前のバージョン](#bkmk_wol-previous)と同じ時刻で有効にできます。

### <a name="limitations"></a>制限事項

- ターゲット サブネットの少なくとも 1 つのクライアントが起動状態にある必要があります。
- この機能では、次のネットワーク テクノロジがサポートされていません。
   - IPv6
   - 802.1x ネットワーク認証
    >[!NOTE]
    > 802.1x ネットワーク認証は、ハードウェアとその構成によっては、追加の構成で動作する場合があります。
- コンピューターは、**Wake Up** クライアント通知経由で通知されたときにのみ復帰します。
    - 期限に到達したときに復帰させるには、以前のバージョンの Wake On LAN が使用されます。
    -  以前のバージョンが有効になっていない場合、 **[展開が必要なときに Wake-on-LAN を使用してクライアントを起動する]** または **[ウェイクアップ パケットを送信する]** という設定で作成された展開ではクライアントが復帰しません。  

> [!IMPORTANT]
> Wake On LAN 機能の同時使用は、限られた量のデバイス (100 台) だけを対象にすることが推奨されます。
>
> Wake On LAN 機能を使用して Configuration Manager 管理コンソールからマシンをウェイクアップすると、その他のリアルタイム アクション機能と共有している内部キューに、ウェイクアップ要求が格納されます。 それら以外の機能の例として、スクリプトの実行、CMPivot、およびその他の高速チャネル クライアント通知があります。 サイト システムのパフォーマンスによっては、ウェイクアップ アクションの所要時間が長くなり、他のリアルタイム アクションで遅延が発生することがあります。 一度に 100 台を超えるマシンをウェイクアップしないことが推奨されます。 この領域に遅延を引き起こす可能性のあるバックログができつつあるかどうかを知るには、\inboxes\objmgr.box ディレクトリで、拡張子が .OPA のファイルが多数あるかどうかを確認します。


### <a name="security-role-permissions"></a>セキュリティ ロールのアクセス許可

- [コレクション] カテゴリの **[リソースの通知]**

### <a name="configure-the-clients-to-use-wake-on-lan-starting-in-version-1810"></a>バージョン 1810 以降で Wake on LAN を使用するようにクライアントを構成する

以前は、ネットワーク アダプターのプロパティを使用してクライアントの Wake On LAN を手動で有効にする必要がありました。 Configuration Manager 1810 には、 **[ネットワークのウェイクアップを許可する]** という新しいクライアント設定があります。 ネットワーク アダプターのプロパティを変更せず、この設定を構成し、展開します。

1. **[管理]** の下で **[クライアント設定]** に移動します。
1. 編集するクライアント設定を選択するか、展開する新しいカスタム クライアント設定を作成します。 詳しくは、「[クライアント設定を構成する方法](configure-client-settings.md)」をご覧ください。
1. **[電源管理]** クライアント設定で **[ネットワークのウェイクアップを許可する]** 設定に **[有効にする]** を選択します。 この設定の詳細については、「[クライアント設定について](about-client-settings.md#power-management)」を参照してください。

4. Configuration Manager 1902 以降では、新しいバージョンの Wake On LAN で、 **[Wake On LAN ポート番号 (UDP)]** [クライアント設定](about-client-settings.md#power-management)に指定されたカスタム UDP ポートが使用されます。 この設定は新旧バージョンの Wake on LAN で共有されます。
 
<!--3605925-->

### <a name="wake-up-a-client-using-client-notification-starting-in-1810"></a>1810 以降でクライアント通知を利用してクライアントを復帰させる
 
1 台のクライアントを復帰させることも、1 つのコレクションに含まれるすべてのスリープ状態クライアントを復帰させることもできます。 コレクション内ですでに復帰しているデバイスについては、何のアクションも行われません。 スリープ状態のクライアントにのみ Wake on LAN 要求が送信されます。 クライアントに復帰を通知する方法については、「[クライアント通知](../manage/client-notification.md)」を参照してください。

- **1 台のクライアントを復帰させるには:** クライアントを右クリックし、 **[クライアント通知]** に移動し、 **[ウェイク アップ]** を選択します。

   ![コンソールの [ウェイク アップ] クライアント通知](media/wol-wake-up-client-notification.png)

- **1 つのコレクションに含まれるすべてのスリープ状態クライアントを復帰させるには:** デバイス コレクションを右クリックし、 **[クライアント通知]** に移動し、 **[ウェイク アップ]** を選択します。
   - このアクションは組み込みコレクションでは実行できません。
   - 1 つのコレクション内にスリープ状態のクライアントとすでに復帰しているデバイスが混在している場合、スリープ状態のクライアントにのみ Wake on LAN 要求が送信されます。
   - Configuration Manager 2002 以降、このアクションは、中央管理サイト、スタンドアロン サイト、または子プライマリ サイトに接続されているコンソールから実行できます。
   - バージョン 1910 以前では、このアクションは、Configuration Manager コンソールがスタンドアロン サイトまたは子プライマリ サイトに接続されている場合にのみアクティブになります。 中央管理サイトに接続されている場合、このアクションは使用できません。

### <a name="what-to-expect-when-only-the-new-version-of-wake-on-lan-is-enabled"></a>新しいバージョンの Wake on LAN のみが有効になっているときの動作

新しいバージョンの Wake on LAN のみを有効にしているとき、 **[ウェイク アップ]** クライアント通知のみが有効になります。 タスク シーケンス、ソフトウェアの配布、ソフトウェア更新プログラムのインストールなどの展開で期限になったとき、クライアントには通知が送信されません。 スリープ状態のクライアントがオンラインに戻ると、管理ポイントでチェックインしたとき、オンラインに戻ったことがコンソールに反映されます。

Configuration Manager バージョン 1902 以降では、Wake on LAN ポートを指定できます。 この設定は新旧バージョンの Wake on LAN で共有されます。

### <a name="what-to-expect-when-both-versions-of-wake-on-lan-are-enabled"></a>両方のバージョンの Wake on LAN が有効になっているときの動作

両方のバージョンの Wake on LAN を有効にしているとき、 **[ウェイク アップ]** クライアント通知と期限での復帰を利用できます。 クライアント通知は、従来の Wake on LAN と機能が少し異なります。 クライアント通知のしくみは「[バージョン 1810 以降の Wake on LAN](#bkmk_wol-1810)」セクションで簡単に説明されているのでご覧ください。 新しいクライアント設定の **[ネットワークのウェイクアップを許可する]** によって、Wake On LAN を許可するように NIC プロパティが変更されます。 環境に追加されている新しいコンピューターに対して NIC プロパティを手動で変更する必要がなくなりました。 Wake on LAN の他の機能はどれも変更されていません。

バージョン 1902 以降、 **[ウェイク アップ]** クライアント通知では既存 **[Wake On LAN ポート番号 (UDP)]** 設定が使用されます。


## <a name="wake-on-lan-for-version-1806-and-earlier"></a><a name="bkmk_wol-previous"></a> バージョン 1806 以前の Wake on LAN

コンピューターをスリープ状態から復帰させて、必須のソフトウェア (ソフトウェア更新プログラム、アプリケーション、タスク シーケンス、プログラムなど) をインストールする場合は、Configuration Manager の Wake On LAN 設定を指定します。

ウェイクアップ プロキシ クライアント設定を使用して、Wake on LAN を補うことができます。 ただし、ウェイクアップ プロキシを使用する場合は、まずそのサイト用に Wake on LAN を有効にし、Wake on LAN 送信方法で **[ウェイクアップ パケットのみを使用する]** および **[ユニキャスト]** オプションを指定する必要があります。 このウェイクアップ ソリューションは、リモート デスクトップ接続などのアドホック接続もサポートします。

最初の手順を Wake on LAN 用にプライマリ サイトを構成します。 次に、2 番目の手順を使用してウェイクアップ プロキシ クライアント設定を構成します。 この 2 番目の手順では、ウェイクアップ プロキシ設定用に既定のクライアント設定を構成し、階層内のすべてのコンピューターに適用します。 一部のコンピューターにのみこれらの設定を適用するには、カスタムのデバイス設定を作成し、ウェイクアップ プロキシ用に構成するコンピューターが含まれるコレクションに割り当てます。 カスタムのクライアント設定を作成する方法について詳しくは、[クライアント設定を構成する方法](../../../core/clients/deploy/configure-client-settings.md)に関するページをご覧ください。

ウェイクアップ プロキシ クライアント設定を受け取ったコンピューターでは、多くの場合、そのネットワーク接続が 1 ～ 3 秒間一時停止されます。 これは、クライアントのウェイクアップ プロキシ ドライバーを有効にするために、クライアントでネットワーク インターフェイスをリセットする必要があるために発生します。

> [!WARNING]
> ネットワーク サービスの予期しない中断を防ぐために、まず分離した代表的なネットワーク インフラストラクチャを使用してウェイクアップ プロキシを評価します。 次に、カスタム クライアント設定を使用して、いくつかのサブネット上にある一部のコンピューター グループにテスト範囲を広げます。 ウェイクアップ プロキシのしくみの詳細については、[クライアントをウェイク アップする方法の計画](../../../core/clients/deploy/plan/plan-wake-up-clients.md)に関するページを参照してください。


### <a name="to-configure-wake-on-lan-for-a-site-for-version-1806-and-earlier"></a>バージョン 1806 以前でサイトに Wake on LAN を構成するには

 Wake on LAN を使用するには、階層内の各サイトに対してそれを有効にする必要があります。

1. Configuration Manager コンソールで、 **[管理]、[サイトの構成]、[サイト]** の順に移動します。
2. 構成するプライマリ サイトをクリックし、 **[プロパティ]** をクリックします。
3. **[Wake on LAN]** タブをクリックし、このサイトに必要なオプションを構成します。 ウェイクアップ プロキシをサポートするには、 **[ウェイクアップ パケットのみを使用する]** と **[ユニキャスト]** を選択する必要があります。 詳細については、「[クライアントをウェイクアップする方法の計画](../../../core/clients/deploy/plan/plan-wake-up-clients.md)」をご覧ください。
4. **[OK]** をクリックし、階層内のすべてのプライマリ サイトでこの手順を繰り返します。

![サイトのプロパティで Wake On LAN を有効にする](media/wol-site-properties.png)

### <a name="to-configure-wake-up-proxy-client-settings"></a>ウェイク アップ プロキシ クライアント設定を構成するには

1. Configuration Manager コンソールで、 **[管理]、[クライアント設定]** に移動します。
2. **[既定のクライアント設定]** をクリックし、 **[プロパティ]** をクリックします。
3. **[電力管理]** を選択し、 **[ウェイクアップ プロキシを有効にする]** に対して **[はい]** を選択します。
4. 設定を確認し、必要に応じてウェイクアップ プロキシ設定を変更します。 これらの設定の詳細については、「[電力管理設定](../../../core/clients/deploy/about-client-settings.md#power-management)」を参照してください。
5. **[OK]** をクリックしてダイアログ ボックスを閉じ、 **[OK]** をクリックして [既定のクライアント設定] ダイアログ ボックスを閉じます。

次の Wake on LAN レポートを使用して、ウェイクアップ プロキシのインストールと構成を監視します。

- ウェイクアップ プロキシの展開状態の概要
- ウェイクアップ プロキシの展開状態の詳細

> [!TIP]
> ウェイクアップ プロキシが機能しているかどうかをテストするには、休止中のコンピューターに対する接続をテストします。 たとえば、休止中のコンピューターにある共有フォルダーに接続したり、リモート デスクトップを使用して休止中のコンピューターへの接続を試行したりします。 Direct Access を使用している場合、現在インターネット上にある休止中のコンピューターに対して同じテストを実行して、IPv6 プレフィックスが機能することを確認します。
