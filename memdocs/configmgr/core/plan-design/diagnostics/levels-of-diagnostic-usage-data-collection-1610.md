---
title: 1610 の診断データ
titleSuffix: Configuration Manager
description: Configuration Manager バージョン 1610 で収集される診断結果および使用状況データの各種レベルについて説明します。
ms.date: 12/29/2016
ms.prod: configuration-manager
ms.technology: configmgr-core
ms.topic: conceptual
ms.assetid: eb20eb90-bcc0-41de-bfea-638ea470c0dd
author: aczechowski
ms.author: aaroncz
manager: dougeby
ROBOTS: NOINDEX
ms.openlocfilehash: 87049bb9799ba5764a3cdd5a14fbf622e7056f3c
ms.sourcegitcommit: bbf820c35414bf2cba356f30fe047c1a34c5384d
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/21/2020
ms.locfileid: "81698140"
---
# <a name="levels-of-diagnostic-usage-data-collection-for-version-1610-of-configuration-manager"></a>Configuration Manager バージョン 1610 で収集される診断結果および使用状況データのレベル

*適用対象:Configuration Manager (Current Branch)*

Configuration Manager バージョン 1610 では、**基本**、**エンハンス**、**フル**の 3 つのレベルの診断結果と使用状況データが収集されます。 既定では、この機能は、エンハンス レベルに設定されます。 以降のセクションでは、各レベルで収集されるデータについて詳しく説明します。

以前のバージョンからの変更は、***[新規]***、***[更新]***、***[削除]***、または ***[移動]*** で示されます。


> [!IMPORTANT]
>  Configuration Manager は、基本レベルとエンハンス レベルでは、サイト コードまたはサイト名、IP アドレス、ユーザー名またはコンピューター名、物理アドレス、電子メール アドレスを収集しません。 フル レベルで収集したこの情報 (ログ ファイルやメモリのスナップショットなどの詳細な診断情報に含まれる可能性があります) に特別な目的はありません。 Microsoft が個人の特定、連絡、広告作成の目的でこの情報を使用することはありません。

##  <a name="how-to-change-the-level"></a><a name="bkmk_change"></a> レベルを変更する方法
 管理者に指定された役割に基づいた管理スコープに、**サイト** オブジェクト クラスにおける**変更**アクセス許可が含まれる場合、その管理者は、Configuration Manager コンソールの診断結果と使用状況データの設定で収集されるデータ レベルを変更できます。

バージョン 1610 以降では、データ収集レベルの変更は、コンソールで **[管理]**  >  **[概要]**  >  **[サイトの構成]**  >  **[サイト]** に移動して行います。 **[階層設定]** を開き、使用するデータのレベルを選択します。  

##  <a name="level-1---basic"></a><a name="bkmk_level1"></a> レベル 1 - 基本
 基本レベルには階層に関するデータが含まれています。これには、インストールまたはアップグレードのエクスペリエンスを向上させるために必要なデータや、階層に適用できる Configuration Manager 更新プログラムを判断するために役立つデータが含まれます。

 Configuration Manager バージョン 1610 では、このレベルには次のデータが含まれます。


- セットアップ情報:
  - ビルド、インストールの種類、言語パック、有効にされた機能  

  - 更新プログラム パックの展開の状態とエラー、ダウンロードの進行状況、前提条件エラー    

  - アップグレード後のスクリプトのバージョン

  - 更新プログラムの高速リングの使用

  - ***[新規]*** リリース前の使用、セットアップ メディアの種類、ブランチの種類

  - ***[新規]*** ソフトウェア アシュアランスの有効期限

- データベースのパフォーマンス指標 (レプリケーション処理情報、プロセッサおよびディスク使用率が上位の SQL Server ストアド プロシージャ)

- 基本的なデータベース構成 (プロセッサ、クラスターの構成、分散ビューの構成)

- Configuration Manager データベース スキーマ (すべてのオブジェクト定義のハッシュ)

- Configuration Manager クライアント バージョンとオペレーティング システム バージョンの数

- マネージド デバイスのオペレーティング システムおよび Exchange Connector によって設定されたポリシーの数

- クライアントの言語とロケールの数

- Windows 10 デバイスの数 (ブランチおよびビルド別)

- Configuration Manager サイト階層の基本データ (サイトの一覧、種類、バージョン、状態、クライアントの数、およびタイム ゾーン)

- サイト システム サーバーの基本情報 (使用されるサイト システムの役割、インターネットと SSL ステータス、オペレーティング システム、プロセッサ、物理または仮想マシン)

- ユーザー探索に関する基本統計情報 (ユーザー探索の数、グループ サイズの最小/最大/平均値)

- エンドポイント保護の基本情報 (マルウェア対策クライアントのバージョン)

- アプリケーションと展開の種類の数に関する基本情報 (アプリの合計、複数の展開の種類を持つアプリの合計、依存関係を持つアプリの合計、置き換えられたアプリの合計、使用中の展開テクノロジの数)

- 基本的なオペレーティング システム展開 (OSD) 数 (イメージ)

- 配布ポイントと管理ポイントの種類、構成の基本情報 (保護済み、事前設定済み、PXE、マルチキャスト、SSL の状態、プル/ピア配布ポイント、MDM 対応、SSL 対応など)

- 製品利用統計情報 (実行時、ランタイム、エラー)

- 構成された製品利用統計情報のレベル、モード (オンラインまたはオフライン)、更新プログラムの高速構成

- ネットワーク探索の使用 (有効または無効)
- 管理コンソール:

  - コンソール接続に関する統計情報 (オペレーティング システムのバージョン、言語、SKU、アーキテクチャに加えて、システム メモリ、論理プロセッサの数、接続サイト ID、インストールされてた .NET のバージョン、コンソールの言語パック)    

- SQL のバージョン、Service Pack レベル、エディション、照合順序 ID、文字セット


##  <a name="level-2---enhanced"></a><a name="bkmk_level2"></a> レベル 2 - エンハンス
エンハンス レベルはセットアップ終了後の既定値です。 このレベルには、基本レベルで収集されたデータと機能固有のデータ (頻度と使用期間)、Configuration Manager クライアントの設定 (コンポーネント名、状態、ポーリング間隔などの特定の設定)、およびソフトウェアの更新に関する基本情報が含まれます。

これが推奨レベルです。このレベルでは、製品やサービスを今後適切に改善するために最小限必要なデータを Microsoft に提供します。 このレベルでは、オブジェクト名 (サイト、ユーザー、コンピューター、またはオブジェクト)、セキュリティ関連のオブジェクトの詳細、またはソフトウェア更新プログラムを必要とするシステムの数などの脆弱性が収集されます。

Configuration Manager バージョン 1610 では、このレベルには次のデータが含まれます。

-   **アプリケーション管理:**  

    -    組織内で使用される展開の種類の使用状況/ターゲットに関する基本情報 (対象となるユーザー/デバイス、必須/使用可能、ユニバーサル アプリ)  

    -   アプリケーションの展開情報 (インストール/アンインストール、承認が必要、ユーザーの介入が有効/無効、依存関係、置き換え)  

    -   使用可能なアプリケーション要求の統計  

    -   パッケージの数 (種類別)  

    -   アプリケーションへの適用の数 (オペレーティング システム別)  

    -   パッケージ/プログラムの展開の数  

    -   App-V 環境と展開のプロパティの数  

    -   Windows 10 ライセンスが供与されたアプリケーションのライセンスの数  

    -   時間帯あたりのユーザーまたはデバイスあたりのアプリケーション展開数の最小/最大/平均値

    -   メンテナンス期間の種類と期間  

    -  アプリケーション ポリシーのサイズと複雑さの統計情報

    - ***[更新]*** ビジネス向け Windows ストア アプリの数と同期の統計情報 (集計されたアプリの種類、ライセンスされたアプリの状態、オンラインおよびオフラインのライセンスされたアプリ数を含みます)  

    - 境界グループの統計情報 (高速の数、低速の数、グループあたりの数)

    - MSI 構成オプションとカウント

    - アプリの要件 (組み込み条件の数を参照する展開テクノロジ)

    - アプリの置き換え、チェーンの最大深度

    - Universal Data Access (UDA) の使用状況、作成方法

    - ***[新規]*** アプリケーション承認の統計情報と使用頻度



-   **クライアント:**  

    -   有効なクライアント エージェントの一覧/数  

    -   クライアント インストールの数 (ソースの場所の種類別)  

    -   クライアント インストール エラーの数  

    -  ***[更新]*** クライアントの自動アップグレード: クライアントのパイロット運用、除外使用状況を含む展開の構成 (拡張相互運用性クライアント)

    -  クライアントの正常性の統計情報と主要な問題のまとめ

    - BIOS の動作時間 (年単位)

    - オペレーティング システムの動作時間 (月単位)

    - ソフトウェア センターのアクションの数

    - Active Management Technology (AMT) クライアント バージョン

    - クライアント展開のダウンロード エラー

    - クライアント通知操作の動作状態 (各々の実行回数、対象となるクライアントの最大数、平均の成功率)

    - クライアントで使用される展開方法、展開方法ごとのクライアントの数

    - クライアントのキャッシュ サイズ構成

    - ***[新規]*** ハードウェア インベントリ クラス、ソフトウェア インベントリ ルール、およびファイル収集規則の数




- **Cloud Services:**

  - Operations Management Suite に同期されているコレクションの数

  -  Operations Management Suite クラウド コネクタが有効になっているかどうか

  - ***[新規]*** クラウド管理ゲートウェイの構成と使用状況の統計情報

  - ***[新規]*** アップグレード分析コネクタの数




- **コレクション:**

    -  コレクションの評価統計情報 (クエリ時間、割り当て数/未割り当て数、種類別のカウント、ID のロール オーバー、規則の使用状況)

    - 展開なしのコレクション

    - コレクション ID の使用状況 (ID が不足していない)



-   **コンプライアンス設定:**  

    -   構成アイテムの数 (種類別)  

    -   構成基準の基本情報 (数、展開数、参照数)  

    -   組み込み設定を参照する展開の数 (修復設定をキャプチャするようになりました)  

    -   カスタム設定に対して作成された規則および展開の数 (修復設定をキャプチャするようになりました)  
    -   展開された Simple Certificate Enrollment Protocol (SCEP)、VPN、Wi-Fi、証明書 (.pfx)、コンプライアンス ポリシー テンプレートの数

    -  SCEP 証明書、VPN、Wi-Fi、証明書 (.pfx)、プラットフォーム別のコンプライアンス ポリシー展開の数

    - Passport for Work のポリシー (作成済み、展開済み)



-   **コンテンツ:**  

    -   境界の数 (種類別)  

    -   境界グループの情報 (各境界グループに割り当てられた境界とサイト システムの数)  

    - ***[新規]*** 境界グループの関係とフォールバックの構成

    -   配布ポイント グループの情報 (配布ポイント グループに割り当てられたパッケージと配布ポイントの数)  

    -   配布ポイントの構成情報 (ブランチ キャッシュの使用、配布ポイントの監視)  

    -   配布マネージャーの構成情報 (スレッド、再試行の待ち時間、再試行回数、プル配布ポイントの設定)  

    - ***[新規]*** ピア キャッシュ クライアントの数、使用状況の統計

    - ***[新規]*** クライアント コンテンツのダウンロードの統計


-   **エンドポイント保護:**  

    -   Endpoint Protection のマルウェア対策および Windows ファイアウォール ポリシーの使用状況 (グループに割り当てられている固有のポリシーの数)<br /><br /> これには、ポリシーに含まれている設定に関する情報は含まれません。  

    -   エンドポイント保護の展開エラー (エンドポイント保護ポリシーの展開エラー コードの数)  

    -   エンドポイント保護ダッシュボードに表示するように選択されたコレクションの数  

    -   エンドポイント保護機能用に構成されたアラートの数  

    -   Advanced Threat Protection (ATP) ポリシー (ポリシーの数、ポリシーが展開されているかどうか)


- **移行:**

  -   移行されたオブジェクト (移行ウィザードを使用) の数



-   **モバイル デバイス管理 (MDM):**  

    -   ***[更新]*** 発行されたモバイル デバイス アクションの数: 各種コマンド (ロック、ピン留め、ワイプ、インベントリからの削除、今すぐ同期)  

    -   Configuration Manager および Microsoft Intune によって管理されるモバイル デバイスの数と、そのデバイスの登録方法 (一括、ユーザー ベース)  

    -   モバイル デバイスのポーリング スケジュールと統計情報、モバイル デバイスのチェックイン期間  

    -   モバイル デバイス ポリシーの数  

    -   複数の登録済みモバイル デバイスを持つユーザーの数  

-   **Microsoft Intune のトラブルシューティング:**

    -   状態、ステータス、インベントリ、RDR、DDR、UDX、テナントの状態、POL、LOG、証明書、CRP、再同期、CFD、RDO、BEX、ISM、および Microsoft Intune からダウンロードされたコンプライアンス メッセージの数とサイズ

    -   Microsoft Intune にレプリケートされたデバイス アクション (ワイプ、インベントリからの削除、ロック)、製品利用統計情報、およびデータ メッセージの数とサイズ

    -   Microsoft Intune のユーザー同期に関する完全な統計とデルタ統計


-   **オンプレミス モバイル デバイス管理 (MDM):**  

    -   オンプレミス MDM アプリケーション展開に関する展開成功/失敗の統計情報  

    -   Windows 10 一括登録パッケージおよびプロファイルの数  



-   **オペレーティング システムの展開:**  

    -   ブート イメージ、ドライバー、ドライバー パッケージ、マルチキャスト対応の配布ポイント、PXE 対応の配布ポイント、およびタスク シーケンスの数  

    -   タスク シーケンス ステップの使用数

    - ***[新規]*** エディション アップグレード ポリシーの数



-   **サイトの更新プログラム:**

    - インストールされた Configuration Manager 修正プログラムのバージョン




-   **ソフトウェア更新プログラム:**  

    -   ソフトウェア更新プログラムの展開が含まれるコレクション数の合計/平均値、および展開された更新プログラム数の最大/平均値  

    -   同期に関連付けられた自動展開規則の数  

    -   新しく作成する、または更新プログラムを既存のグループに追加する自動展開規則の数  

    -   自動展開規則で使用される使用可能なデルタと期限デルタ  

    -   更新プログラムあたりの割り当て数の平均/最大値  

    -   System Center Update Publisher で作成および展開された更新プログラムの数  

    -   更新プログラムのグループと割り当ての数  

    -   更新プログラム パッケージの数と、パッケージの対象配布ポイント数の最大/最小/平均値  

    -   更新プログラム グループの数と、グループあたりの更新プログラム数の最小/最大/平均値  

    -   更新プログラムの数と、展開済み、期限切れ、置き換え済み、ダウンロード済み、および EULA を含む更新プログラムの割合  

    -   更新スキャン エラー コードとマシンの数  

    -   クライアント更新の評価とスキャンのスケジュール  

    -   ソフトウェアの更新ポイントの同期スケジュール  

    -   複数の展開を含む自動展開規則の数  

    -   アクティブな Windows 10 サービス プランに使用される構成  

    -   Windows 10 ダッシュボードのコンテンツ バージョン  

    -   Windows Update for Business を使用している Windows 10 クライアントの数  

    -   クラスターの修正プログラム適用の統計情報  

    -   展開された Office 365 更新プログラムの数  

    -   ソフトウェアの更新ポイントで同期される分類

    -   ソフトウェア更新ポイントの負荷分散の統計情報

    -  ***[新規]*** Windows 10 高速更新プログラムの構成




-   **SQL/パフォーマンス データ:**  

    -   最大データベース テーブルの数  

    -   ***[更新]*** SQL AlwaysOn レプリカ情報、使用状況、正常性の状態

    -  SQL の変更の追跡の保有期間

    - 探索の種類、有効化、スケジュール (完全、増分)

    - 探索の運用統計 (見つかったオブジェクトの数)

    - SQL 変更の追跡のパフォーマンスの問題、保有期間、自動クリーンアップの状態



- **その他**

    - Wake On Lan (WOL) サイトの数

    - ***[新規]*** 使用状況とパフォーマンスの統計情報のレポート  



##  <a name="level-3---full"></a><a name="bkmk_level3"></a> レベル 3 - フル
フル レベルには、基本レベルとエンハンス レベルのすべてのデータが含まれます。 また、Endpoint Protection の詳細情報、更新プログラムの対応率、およびソフトウェア更新プログラム情報も含まれています。  このレベルには、キャプチャ時にメモリやログ ファイルに存在していた、個人情報が含まれる可能性があるシステム ファイルやメモリ スナップショットなどの詳細な診断情報を含めることもできます。

Configuration Manager バージョン 1610 では、このレベルには次のデータが含まれます。

-   コレクションの評価および更新の統計情報

-   Endpoint Protection の正常性の概要 (保護済み、危険、不明、未サポート クライアントの数を含む)

-   Endpoint Protection ポリシーの構成

-   ソフトウェア更新プログラムの展開情報 (クライアントとUTC 時刻の対象となっている展開の割合、必須/オプション/サイレント、再起動抑制)

-   ソフトウェア更新プログラムの展開の全体的なコンプライアンス対応状況

-   自動展開規則の評価スケジュールの情報

-   ソフトウェア更新プログラムの展開のエラー コードと数

-   ソフトウェア更新プログラムの展開コレクションの非アクティブなクライアント数の最小/最大/平均値

-   期限切れのソフトウェア更新プログラムが含まれるグループの数

-   パッケージあたりのソフトウェア更新プログラム数の最小/最大/平均値

-   ソフトウェア更新プログラムのスキャン成功の割合

-   最後のソフトウェア更新プログラムのスキャンが実行されてからの経過時間の最小/最大/平均値

-    ソフトウェアの更新ポイントで同期されるソフトウェア更新プログラムの製品
-    コンプライアンス設定: SCEP、VPN、Wi-Fi、コンプライアンス ポリシー テンプレートの構成の詳細

-    Intune で管理されるデバイス向けの EAS 条件付きアクセス ポリシーの種類 (ブロックまたは検疫)

-   環境内の上位 50 の CPU

-   Configuration Manager の DCM 構成パックの使用状況

-   MSI 製品コード (顧客が展開する一般的なアプリ)

-   ATP の正常性の概要

-   クライアント展開のインストール エラーの詳細

- ***[新規]*** ビジネス向け Windows ストアの詳細 (AppID、オンラインまたはオフラインの状態、合計購入ライセンス数を含む、同期したアプリケーションの非集計リスト)
