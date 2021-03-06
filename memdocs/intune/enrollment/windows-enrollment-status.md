---
title: 登録ステータス ページを設定する
titleSuffix: Microsoft Intune
description: Windows 10 デバイスを登録するユーザー向けの案内ページを設定します。
keywords: ''
author: ErikjeMS
ms.author: erikje
manager: dougeby
ms.date: 11/26/2019
ms.topic: conceptual
ms.service: microsoft-intune
ms.subservice: enrollment
ms.localizationpriority: high
ms.technology: ''
ms.assetid: 8518d8fa-a0de-449d-89b6-8a33fad7b3eb
ms.reviewer: ericor
ms.suite: ems
search.appverid: MET150
ms.custom: intune-azure;seodec18
ms.collection: M365-identity-device-management
ms.openlocfilehash: 8ba3563a243b13b874608ad7a3ec918130e5bb80
ms.sourcegitcommit: fb84a87e46f9fa126c1c24ddea26974984bc9ccc
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/22/2020
ms.locfileid: "82022706"
---
# <a name="set-up-an-enrollment-status-page"></a>登録ステータス ページを設定する
 
[!INCLUDE [azure_portal](../includes/azure_portal.md)]
 
登録ステータス ページ (ESP) には、デバイスの初期登録時に Windows 10 デバイス (バージョン 1803 以降) に関するインストール情報が表示されます。 次に例を示します。
- [Windows Autopilot](https://docs.microsoft.com/windows/deployment/windows-autopilot/) を使用しているとき 
- 登録ステータス ページ ポリシーの適用後、マネージド デバイスが初めて起動されたとき。 

登録ステータス ページは、ユーザーがデバイスの設定中に自分のデバイスの状態を把握するのに役立ちます。 登録ステータス ページのプロファイルを複数作成し、ユーザーが含まれるさまざまなグループに適用することができます。 プロファイルを設定すると、次のことが行えます。
- インストールの進行状況を表示する。
- インストールが完了するまで使用をブロックする。
- デバイスの設定が失敗した場合にユーザーが行えることを指定する。

同じユーザーに対して競合するプロファイルの割り当てを考慮して、プロファイルごとに優先順位を設定することもできます。

> [!NOTE]
> 登録ステータス ページは割り当てられたグループに属しているユーザーだけを対象にすることができ、ポリシーはそのデバイスを使用するすべてのユーザーに対して登録時にデバイスに設定されます。  登録ステータス ページのプロファイルを対象とするデバイスは、現在サポートされていません。

## <a name="available-settings"></a>利用可能な設定

 登録ステータス ページの動作をカスタマイズするには、次の設定を構成できます。

<table>
<th align="left">設定<th align="left">はい<th align="left">いいえ
<tr><td>アプリとプロファイルのインストールの進行状況を表示する<td>登録ステータス ページは表示されます。<td>登録ステータス ページは表示されません。
<tr><td>すべてのアプリとプロファイルがインストールされるまでデバイスの使用をブロックする<td>このテーブルの設定を使用して、ユーザーがインストールに関する潜在的な問題に対処できるように、登録ステータス ページの動作をカスタマイズできます。
<td>登録のステータス ページには、インストールの失敗を解決するための追加オプションは表示されません。
<tr><td>インストール エラーが発生した場合にデバイスのリセットをユーザーに許可する<td>インストール エラーが発生した場合、<b>[デバイスのリセット]</b> ボタンが表示されます。<td>インストール エラーが発生した場合、<b>[デバイスのリセット]</b> ボタンは表示されません。
<tr><td>インストール エラーが発生した場合にデバイスの使用をユーザーに許可する<td>インストール エラーが発生した場合、<b>[続行]</b> ボタンが表示されます。<td>インストール エラーが発生した場合、<b>[続行]</b> ボタンは表示されません。
<tr><td>Show timeout error when installation takes longer than specified number of minutes (インストールに要する時間が指定された分数を超えたらタイムアウト エラーを表示する)<td colspan="2">インストールが完了するまでの待機時間を分単位で指定します。 既定値の 60 分が入力されます。
<tr><td>エラー発生時にカスタム メッセージを表示する<td>テキスト ボックスで、インストール エラー発生時に表示するカスタム メッセージを指定できます。<td>既定のメッセージが表示されます。 <br><b>インストールが組織によって設定された時間制限を超えました。 やり直すか、IT サポート担当者にお問い合わせください。<b>
<tr><td>インストール エラーに関するログ収集をユーザーに許可する<td>インストール エラーが発生した場合、<b>[ログの収集]</b> ボタンが表示されます。 <br>ユーザーがこのボタンをクリックすると、ログ ファイル <b>MDMDiagReport.cab</b> を保存する場所の選択を求められます<td>インストール エラーが発生した場合、<b>[ログの収集]</b> ボタンは表示されません。
<tr><td>これらの必要なアプリがユーザーまたはデバイスに割り当てられている場合、それらがインストールされるまでデバイスの使用をブロックします<td colspan="2"><b>[すべて]</b> または <b>[選択済み]</b> を選択します。 <br><br><b>[選択済み]</b> を選択すると、<b>[アプリを選択]</b> ボタンが表示され、デバイスを有効にする前にインストールする必要があるアプリを選択できます。
</table>

## <a name="turn-on-default-enrollment-status-page-for-all-users"></a>すべてのユーザーに対して既定の登録ステータス ページを有効にする

登録ステータス ページを有効にするには、以下の手順のようにします。
 
1. [Microsoft Endpoint Manager admin center](https://go.microsoft.com/fwlink/?linkid=2109431) で、 **[デバイス]**  >  **[Windows]**  >  **[Windows の登録]**  >  **[登録ステータス ページ]** を選択します。
2. **[登録ステータス ページ]** ブレードで、 **[既定]**  >  **[設定]** の順に選択します。
3. **[Show app and profile installation progress]\(アプリとプロファイルのインストールの進行状況を表示する\)** で、 **[はい]** を選択します。
4. 有効にするその他の設定を選択してから、 **[保存]** を選びます。

## <a name="create-enrollment-status-page-profile-and-assign-to-a-group"></a>登録ステータス ページのプロファイルを作成してグループに割り当てる

1. [Microsoft Endpoint Manager admin center](https://go.microsoft.com/fwlink/?linkid=2109431) で、 **[デバイス]**  >  **[Windows]**  >  **[Windows の登録]**  >  **[登録ステータス ページ]**  >  **[プロファイルの作成]** を選択します。
2. **名前**と**説明**を入力します。
3. **[作成]** を選択します。
4. **[登録ステータス ページ]** リストで新しいプロファイルを選択します。
5. **[割り当て]**  >  **[グループの選択]** の順に選択します。次に、このプロファイルを採用するグループを選び、 **[選択]**  >  **[保存]** の順に選択します。
6. **[設定]** を選択し、このプロファイルに適用する設定を選びます。次に **[保存]** を選択します。

## <a name="set-the-enrollment-status-page-priority"></a>登録ステータス ページの優先順位を設定する

1 人のユーザーが、複数のグループに属し、多くの登録ステータス ページ プロファイルを使用することができます。 そのような競合に対処するため、プロファイルごとに優先順位を設定することができます。 登録時に、ユーザーが複数の登録ステータス ページ プロファイルを持っている場合は、優先順位の最も高いプロファイルのみがデバイスの登録に適用されます。

1. [Microsoft Endpoint Manager admin center](https://go.microsoft.com/fwlink/?linkid=2109431) で、 **[デバイス]**  >  **[Windows]**  >  **[Windows の登録]**  >  **[登録ステータス ページ]** を選択します。
2. 一覧内のプロファイルにカーソルを合わせます。
3. 3 つの縦向きドットを使用して、そのプロファイルを一覧上の目的の位置にドラッグします。

## <a name="block-access-to-a-device-until-a-specific-application-is-installed"></a>特定のアプリケーションがインストールされるまでデバイスへのアクセスをブロックする

ユーザーがデスクトップにアクセスするためにインストールしておく必要があるアプリを指定できます。

1. [Microsoft Endpoint Manager admin center](https://go.microsoft.com/fwlink/?linkid=2109431) で、 **[デバイス]**  >  **[Windows]**  >  **[Windows の登録]**  >  **[登録ステータス ページ]** を選択します。
2. プロファイルを選択して、 **[設定]** を選択します。
3. **[アプリとプロファイルのインストールの進行状況を表示する]** で、 **[はい]** を選択します。
4. **[すべてのアプリとプロファイルがインストールされるまでデバイスの使用をブロックする]** で **[はい]** を選択します。
5. **[これらの必要なアプリがユーザーまたはデバイスに割り当てられている場合、それらがインストールされるまでデバイスの使用をブロックします]** で **[選択済み]** を選択します。
6. **[アプリを選択]** を選択し、アプリを選択してから、 **[選択]**  >  **[保存]** を選択します。

この一覧に含まれているアプリは、Intune によって、ブロックされていると見なされる必要がある一覧をフィルター処理するために使用されます。  インストールする必要があるアプリを指定していません。  たとえば、"App 1"、"App 2"、および "App 3" を含めるようにこの一覧を構成し、"App 3" と "App 4" がデバイスまたはユーザーの対象とされる場合、[登録ステータス ページ] では "App 3" のみが追跡されます。  "App 4" はインストールされますが、[登録ステータス ページ] ではそれが完了するまで待機しません。

最大 25 個のアプリを指定できます。

## <a name="enrollment-status-page-tracking-information"></a>登録ステータス ページの追跡情報

登録ステータス ページの情報追跡フェーズには、デバイスの準備、デバイスのセットアップ、アカウントのセットアップの 3 つがあります。

### <a name="device-preparation"></a>デバイスの準備

デバイスの準備では、次の情報が登録ステータス ページで追跡されます。
- トラステッド プラットフォーム モジュール (TPM) キー構成証明 (該当する場合)
- Azure Active Directory への参加の進行状況
- Intune への登録
- Intune 管理拡張機能のインストール

### <a name="device-setup"></a>デバイスのセットアップ

登録ステータス ページでは、次のデバイス セットアップ項目が追跡されます (項目が、すべてのデバイス、または登録デバイスがメンバーとなっているデバイス グループに割り当てられている場合)。
- セキュリティ ポリシー
  - すべての登録に対する 1 つの構成サービス プロバイダー (CSP)。
  - Intune で構成されている実際の CSP は、ここでは追跡されません。
- アプリケーション
  - コンピューター単位の基幹業務 (LoB) MSI アプリ。
  - インストール コンテキストがデバイスの LoB ストア アプリ。
  - インストール コンテキストがデバイスのオフライン ストアおよび LoB ストア アプリ。
  - Win32 アプリケーション (Windows 10 バージョン 1903 以降のみ) 
- 接続プロファイル
  - **[すべてのデバイス]** または、登録中のデバイスが属しているデバイス グループに割り当てられる VPN または Wi-Fi プロファイル。ただし、Autopilot デバイスの場合に限られる
- **[すべてのデバイス]** または、登録中のデバイスが属しているデバイス グループに割り当てられる証明書プロファイル。ただし、Autopilot デバイスの場合に限られる

### <a name="account-setup"></a>アカウントのセットアップ
アカウントのセットアップの場合、登録ステータス ページでは、次の項目が現在のログイン ユーザーに割り当てられている場合、これらの項目が追跡されます。
- セキュリティ ポリシー
  - すべての登録に対する 1 つの CSP。
  - Intune で構成されている実際の CSP は、ここでは追跡されません。
- アプリケーション
  - すべてのデバイス、すべてのユーザー、またはデバイスを登録しているユーザーがメンバーであるユーザー グループに割り当てられている、ユーザー単位の LoB MSI アプリ。
  - すべてのユーザー、またはデバイスを登録しているユーザーがメンバーであるユーザー グループに割り当てられている、コンピューター単位の LoB MSI アプリ。
  - 次のいずれかのオブジェクトに割り当てられている、LoB ストア アプリ、オンライン ストア アプリ、およびオフライン ストア アプリ。
    - すべてのデバイス
    - すべてのユーザー
    - デバイスを登録するユーザーが、インストール コンテキストがユーザーに設定されているメンバーである、ユーザー グループ。
  - Win32 アプリケーション (Windows 10 バージョン 1903 以降のみ) 
- 接続プロファイル
  - すべてのユーザー、またはデバイスを登録しているユーザーがメンバーであるユーザー グループに割り当てられている、VPN または Wi-Fi プロファイル。
- 証明書
  - すべてのユーザー、またはデバイスを登録しているユーザーがメンバーであるユーザー グループに割り当てられている、証明書プロファイル。

### <a name="troubleshooting"></a>トラブルシューティング
トラブルシューティングに関してよくある質問。

- 登録ステータス ページを見ても、アプリケーションがインストールされておらず、追跡記録されていません。なぜですか。
  - アプリケーションを確実にインストールして追跡記録するよう、登録ステータス ページを利用するには、次のように手配します。
      - "必須" 割り当てを利用することで、デバイス (デバイス対象アプリの場合) またはユーザー (ユーザー対象アプリの場合) が含まれる Azure AD グループにアプリを割り当てます。  (デバイス対象アプリは ESP のデバイス段階中に追跡記録され、ユーザー対象アプリは ESP のユーザー段階中に追跡記録されます)
      - **[すべてのアプリとプロファイルがインストールされるまでデバイスの使用をブロックする]** を指定するか、 **[Block device use until these required apps are installed]\(これらの必要なアプリがインストールされるまでデバイスの使用をブロックする\)** にアプリを含めます。
      - アプリはデバイス関連でインストールされ、ユーザー関連で適用される規則は与えられません。

- たとえば、ユーザーが Configuration Manager で共同管理に登録されているデバイスに初めてログインする場合など、Autopilot ではない展開で登録ステータス ページが表示されるのはなぜですか?  
  - 登録ステータス ページには、次のようなすべての登録方法に対するインストール状態が表示されます
      - Autopilot
      - Configuration Manager の共同管理
      - 登録ステータス ページ ポリシーが初めて適用されたデバイスに新しいユーザーがログインしたとき
      - **[out-of-box experience (OOBE) でプロビジョニングされたデバイスにのみページを表示する]** の設定がオンになっていて、ポリシーが設定されている場合は、デバイスに最初にサインインしたユーザーに対してのみ [登録ステータス ページ] が表示されます

- 登録ステータス ページがデバイスで構成されている場合、それを無効にする方法はありますか?
  - 登録ステータス ページ ポリシーは、登録時にデバイスに設定されます。 登録ステータス ページを無効にするには、ユーザーとデバイスの登録ステータス ページのセクションを無効にする必要があります。 セクションを無効にするには、次の構成で OMA-URI のカスタム設定を作成します。

      ユーザーの登録ステータス ページを無効にする:

      ```
      Name:  Disable User ESP (choose a name you desire)
      Description:  (enter a description)
      OMA-URI:  ./Vendor/MSFT/DMClient/Provider/MS DM Server/FirstSyncStatus/SkipUserStatusPage
      Data type:  Boolean
      Value:  True 
      ```
      デバイスの登録ステータス ページを無効にする:

      ```
      Name:  Disable Device ESP (choose a name you desire)
      Description:  (enter a description)
      OMA-URI:  ./Vendor/MSFT/DMClient/Provider/MS DM Server/FirstSyncStatus/SkipDeviceStatusPage
      Data type:  Boolean
      Value:  True 
      ```
- ログ ファイルを収集するにはどうすればよいですか?
  - 登録ステータス ページのログ ファイルを収集するには、次の 2 つの方法があります。
      - ユーザーが ESP ポリシーでログを収集できるようにします。 登録ステータス ページでタイムアウトが発生した場合、エンド ユーザーは **[ログの収集]** のオプションを選択できます。 USB ドライブを挿入することにより、ログ ファイルをドライブにコピーできます
      - Shift + F10 キー シーケンスを入力してコマンド プロンプトを開いた後、次のコマンド ラインを入力してログ ファイルを生成します。 

      ```
      mdmdiagnosticstool.exe -area Autopilot -cab <pathToOutputCabFile>.cab 
      ```

### <a name="known-issues"></a>既知の問題
既知の問題を以下に示します。 
- ESP プロファイルを無効にしてもデバイスから ESP ポリシーは削除されず、ユーザーが初めてデバイスにログインするときに ESP が引き続き使用されます。 ESP プロファイルを無効にしても、ポリシーは削除されません。 ESP を無効にするには、OMA-URI を展開する必要があります。 OMA-URI を使用して ESP を無効にする方法については、上記を参照してください。 
- デバイス セットアップの間に再起動すると、アカウント セットアップ フェーズに移行する前に、ユーザーは資格情報の入力を強制されます。 再起動時に、ユーザーの資格情報は保持されません。 ユーザーが資格情報を入力すると、登録ステータス ページは続行できます。 
- 1903 より前の Windows 10 バージョンでは、職場または学校アカウントの登録の追加の間に、登録ステータス ページが常にタイムアウトします。 登録ステータス ページは Azure AD の登録が完了するのを待機しています。 この問題は、Windows 10 バージョン 1903 以降で修正されています。  
- ESP を使用する Hybrid Azure AD の Autopilot 展開には、ESP プロファイルで定義されているタイムアウト時間より長い時間がかかります。 Hybrid Azure AD の Autopilot 展開の ESP には、ESP プロファイルで設定された値より 40 分長くかかります。 この遅延により、オンプレミス AD コネクタは Azure AD に新しいデバイス レコードを作成できます。 
- Autopilot のユーザー主導モードでは、Windows ログオン ページにユーザー名が事前設定されません。 ESP のデバイス セットアップ フェーズ中に再起動が行われた場合、次のようになります。
    - ユーザーの資格情報は保持されません
    - ユーザーは、デバイス セットアップ フェーズからアカウント セットアップ フェーズに進む前に、資格情報をもう一度入力する必要があります
- ESP の "識別" フェーズが、長時間かかるか、完了しません。 Intune では、識別フェーズの間に ESP ポリシーが計算されます。 現在のユーザーに Intune ライセンスが割り当てられていない場合、ESP ポリシーの計算が完了しないことがあります。  
- Microsoft Defender アプリケーション制御を構成すると、Autopilot の間に再起動を求められます。 Microsoft Defender アプリケーション (AppLocker CSP) を構成するには、再起動が必要です。 このポリシーが構成されていると、Autopilot の間にデバイスが再起動される可能性があります。 現時点では、再起動を抑制または延期する方法はありません。
- ESP プロファイルの一部として DeviceLock ポリシー (https://docs.microsoft.com/windows/client-management/mdm/policy-csp-devicelock) が有効になっている場合、OOBE またはユーザー デスクトップの自動ログオンは、次の 2 つの理由で予期せず失敗する可能性があります。
  - ESP デバイス セットアップ フェーズ終了前にデバイスが再起動しなかった場合、ユーザーは Azure AD 資格情報の入力を求められることがあります。 自動ログオンが成功して Windows 初回ログイン アニメーションがユーザーに表示される代わりに、この要求が発生します。
  - ユーザーが Azure AD 資格情報を入力した後、ESP デバイス セットアップ フェーズが終了する前に、デバイスが再起動された場合、自動ログオンは失敗します。 この失敗は、ESP デバイス セットアップ フェーズが完了していないために発生します。 それを回避するには、デバイスをリセットします。

## <a name="next-steps"></a>次のステップ
Windows 登録ページを設定したら、Windows デバイスの管理方法を学習します。 詳細については、「[Microsoft Intune デバイスの管理とは](../remote-actions/device-management.md)」をご覧ください。
