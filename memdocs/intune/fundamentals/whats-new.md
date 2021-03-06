---
title: Microsoft Intune の新機能 - Azure | Microsoft Docs
titleSuffix: ''
description: Intune Azure Portal の新機能を確認する
keywords: ''
author: ErikjeMS
ms.author: erikje
manager: dougeby
ms.date: 05/04/2020
ms.topic: conceptual
ms.service: microsoft-intune
ms.subservice: fundamentals
ms.localizationpriority: high
ms.technology: ''
ms.assetid: 791ed23f-bd13-4ef0-a3dd-cd2d7332c5cc
ms.reviewer: dougeby
ms.suite: ems
search.appverid: MET150
ms.custom: intune-azure; get-started
ms.collection: M365-identity-device-management
ms.openlocfilehash: 5b3c8287d9b5ca2d46094d04ee2179128bead4a8
ms.sourcegitcommit: 0dafd513a59afe592b5cfe2a80b6288020dc5bf0
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/08/2020
ms.locfileid: "82991740"
---
# <a name="whats-new-in-microsoft-intune"></a>Microsoft Intune の新機能

[Microsoft Endpoint Manager admin center](https://go.microsoft.com/fwlink/?linkid=2109431) で Microsoft Intune の週ごとの新機能について説明します。 また、[重要なお知らせ](#notices)、[過去のリリース](whats-new-archive.md)、および [Intune サービスの更新プログラムのリリース方法](https://techcommunity.microsoft.com/t5/Intune-Customer-Success/Microsoft-Intune-Service-Updates/ba-p/358728)に関する情報もあります。 

> [!Note]
> 個々の[マンスリー更新プログラム](https://techcommunity.microsoft.com/t5/Intune-Customer-Success/Microsoft-Intune-Service-Updates/ba-p/358728)は、展開に最大 3 日かかることがあります。順序は次のとおりです。
>
> - 1 日目:アジア太平洋 (APAC)
> - 2 日目:ヨーロッパ、中東、アフリカ (EMEA)
> - 3 日目:北米
> - 4 日目以降:政府機関向け Intune
>
> 一部の機能は数週間にわたってロールアウトされ、一部のお客様は最初の週にご利用になれない可能性があります。
>
> リリースの今後の機能の一覧については、[開発中のページ](in-development.md)を参照してください。

**RSS フィード**:ご自身のフィード リーダーに次の URL をコピーして貼り付けることで、このページの更新時に通知を受け取ることができます。`https://docs.microsoft.com/api/search/rss?search=%22What%27s+new+in+microsoft+intune%3F+-+Azure%22&locale=en-us`

<!-- Common categories:  
### App management
### Device configuration
### Device enrollment
### Device management
### Device security
### Intune apps
### Monitor and troubleshoot

<!-- ########################## -->
## <a name="week-of-may-4-2020"></a>2020 年 5 月 4 日の週  

<!-- vvvvvvvvvvvvvvvvvvvvvv -->  

### <a name="company-portal-for-android-guides-users-to-get-apps-after-work-profile-enrollment----6103999---"></a>Android 用ポータル サイトで仕事用プロファイルの登録後にアプリを取得する方法がユーザーに示される <!-- 6103999 -->
ユーザーがアプリをより簡単に見つけてインストールできるように、ポータル サイトのアプリ内ガイダンスが改善されました。 仕事用プロファイルの管理に登録した後、バッジ付きバージョンの Google Play でおすすめのアプリを見つける方法を説明するメッセージがユーザーに表示されます。 [Android のプロファイルでデバイスを登録する方法](../user-help/enroll-device-android-work-profile.md)に関する記事の最後の手順は、新しいメッセージを示すように更新されています。 また、ユーザーには、左側のポータル サイト ドロアーで新しい **[アプリの取得]** リンクが表示されます。 これらの新規および改善されたエクスペリエンスの場所を空けるために、 **[アプリ]** タブは削除されました。 更新された画面を確認するには、「[Intune エンド ユーザー アプリの UI 更新](./whats-new-app-ui.md)」を参照してください。 

<!-- ########################## -->
## <a name="week-of-april-20-2020"></a>2020 年 4 月 20 日の週

<!-- vvvvvvvvvvvvvvvvvvvvvv -->

### <a name="device-management"></a>デバイス管理

#### <a name="microsoft-endpoint-manager-tenant-attach-device-sync-and-device-actions---6317104-cm3555758-idready---"></a>Microsoft Endpoint Manager テナントのアタッチ:デバイスの同期とデバイスのアクション<!-- 6317104, CM3555758 idready -->
Microsoft Endpoint Manager によって、Configuration Manager と Intune が 1 つのコンソールに統合されます。 Configuration Manager バージョン 2002 以降、ご利用の Configuration Manager デバイスをクラウド サービスにアップロードし、管理センターからそれらに対するアクションを実行できます。 詳細については、「[Microsoft Endpoint Manager テナントのアタッチ: デバイスの同期とデバイスのアクション](../../configmgr/tenant-attach/device-sync-actions.md)」を参照してください。 

### <a name="app-management"></a>アプリ管理

#### <a name="microsoft-office-365-proplus-rename---6368143---"></a>Microsoft Office 365 ProPlus 名前変更<!-- 6368143 -->
Microsoft Office 365 ProPlus は **Microsoft 365 Apps for enterprise** に名前変更されています。 詳細については、「[Office 365 ProPlus の名前の変更](https://docs.microsoft.com/deployoffice/name-change)」を参照してください。 このドキュメントでは、これを通例 Microsoft 365 アプリと呼びます。 [Microsoft Endpoint Manager admin center](https://go.microsoft.com/fwlink/?linkid=2109431) で、 **[アプリ]** 、 **[Windows]** 、 **[追加]** の順に選択して、このアプリを見つけることができます。 アプリを追加する方法の詳細については、「[Microsoft Intune にアプリを追加する](../apps/apps-add.md)」を参照してください。

<!-- ########################## -->
## <a name="week-of-april-13-2020-2004-service-release"></a>2020 年 4 月 13 日の週 (2004 サービス リリース)

<!-- vvvvvvvvvvvvvvvvvvvvvv -->
### <a name="app-management"></a>アプリ管理

#### <a name="manage-smime-settings-for-outlook-on-android-enterprise-devices---6517085-----"></a>Android Enterprise デバイスで Outlook の S/MIME 設定を管理する<!-- 6517085   -->
アプリ構成ポリシーを使用して、Android Enterprise を実行するデバイス上で Outlook の S/MIME 設定を管理できます。 また、デバイスのユーザーが Outlook の設定で S/MIME を有効または無効にすることを許可するかどうかも選択できます。 Android 用のアプリ構成ポリシーを使用するには、[Microsoft Endpoint Manager admin center](https://go.microsoft.com/fwlink/?linkid=2109431) で、 **[アプリ]**  >  **[アプリ構成ポリシー]**  >  **[追加]**  >  **[マネージド デバイス]** の順に移動します。 Outlook の設定を構成する方法の詳細については、「[Microsoft Outlook の構成設定](../apps/app-configuration-policies-outlook.md)」を参照してください。

#### <a name="pre-release-testing-for-managed-google-play-apps---2681933----"></a>マネージド Google Play アプリのプレリリース テスト<!-- 2681933  -->
[アプリのプレリリース テストに Google Play のクローズド テスト トラック](https://support.google.com/googleplay/android-developer/answer/3131213)を使用している組織は、Intune でこれらのトラックを管理できます。 テストを実行するために、Google Play の実稼働前のトラックに発行されたアプリをパイロット グループに選択的に割り当てることができます。 Intune では、アプリに実稼働前のビルド テスト トラックが発行されているかどうかや、そのトラックを AAD ユーザーまたはデバイス グループに割り当てることができるかどうかを確認できます。 この機能は、現在サポートされているすべての Android Enterprise シナリオ (仕事用プロファイル、フル マネージド、および専用) で利用できます。 [Microsoft Endpoint Manager admin center](https://go.microsoft.com/fwlink/?linkid=2109431) で、 **[アプリ]**  >  **[Android]**  >  **[追加]** を選択して、マネージド Google Play アプリを追加できます。 詳細については、「[マネージド Google Play のクローズド テスト トラックの操作](../apps/apps-add-android-for-work.md#working-with-managed-google-play-closed-testing-tracks)」を参照してください。

#### <a name="microsoft-teams-is-now-included-in-the-office-365-suite-for-macos---5903936----"></a>Microsoft Teams が Office 365 Suite for macOS に含まれるようになりました<!-- 5903936  -->
Microsoft エンドポイント マネージャーで Microsoft Office for macOS が割り当てられているユーザーは、既存の Microsoft Office アプリ (Word、Excel、PowerPoint、Outlook、OneNote) に加えて、Microsoft Teams を受け取るようになります。 Intune は、他の Office for macOS アプリがインストールされている既存の Mac デバイスを認識し、次回デバイスが Intune にチェックインするときに Microsoft Teams のインストールを試行します。 [Microsoft Endpoint Manager admin center](https://go.microsoft.com/fwlink/?linkid=2109431) で、 **[アプリ]**  >  **[macOS]**  >  **[追加]** の順に選択して、**Office 365 Suite** for macOS を見つけることができます。 詳しくは、「[Microsoft Intune を使用して macOS デバイスに Office 365 を割り当てる](../apps/apps-add-office365-macos.md)」をご覧ください。

#### <a name="update-to-android-app-configuration-policies---6113334----"></a>Android アプリ構成ポリシーの更新<!-- 6113334  -->
Android アプリ構成ポリシーは、アプリ構成プロファイルを作成する前に、管理者がデバイス登録の種類を選択できるように更新されています。 この機能は、登録の種類 (仕事用プロファイルまたはデバイス所有者) に基づく証明書プロファイルのために追加されます。  この更新の内容は次のとおりです。

1. 新しいプロファイルが作成され、デバイス登録の種類として [仕事用プロファイルとデバイス所有者プロファイル] が選択されている場合は、証明書プロファイルをアプリ構成ポリシーに関連付けることはできません。
2. 新しいプロファイルが作成され、[仕事用プロファイルのみ] が選択されている場合は、[デバイスの構成] で作成された仕事用プロファイルの証明書ポリシーを利用できます。
3. 新しいプロファイルが作成され、[デバイスの所有者のみ] が選択されている場合は、[デバイスの構成] で作成されたデバイスの所有者の証明書ポリシーを利用できます。 

> [!IMPORTANT]
> この機能がリリースされる前 (2020 年 4 月リリース- 2004 年) に作成され、ポリシーに関連付けられている証明書プロファイルがない既存のポリシーは、デバイス登録の種類の既定値が [仕事用プロファイルとデバイス所有者プロファイル] になります。 また、この機能がリリースされる前に作成され、関連付けられている証明書プロファイルがある既存のポリシーは、既定値が [仕事用プロファイルのみ] になります。

さらに、仕事用プロファイルとデバイス所有者の両方の登録タイプに対して機能する、Gmail および Nine の電子メール構成プロファイルを追加しています。これには、両方の電子メール構成の種類での証明書プロファイルの使用が含まれます。  仕事用プロファイル用に [デバイスの構成] で作成した Gmail または Nine のポリシーはすべて、デバイスに引き続き適用されるため、アプリ構成ポリシーに移動する必要はありません。

[Microsoft Endpoint Manager admin center](https://go.microsoft.com/fwlink/?linkid=2109431) で、 **[アプリ]**  >  **[アプリ構成ポリシー]** を選択して、アプリ構成ポリシーを検索できます。 アプリ構成ポリシーの詳細については、「[Microsoft Intune 用アプリ構成ポリシー](../apps/app-configuration-policies-overview.md)」を参照してください。

#### <a name="push-notification-when-device-ownership-type-is-changed---5575875---"></a>デバイスの所有権の種類が変更されたときのプッシュ通知<!-- 5575875 -->
Android と iOS の両方のポータル サイト ユーザーに、自身のデバイスの所有権の種類が個人用から企業に変更されている場合に、プライバシーを尊重するため、プッシュ通知を送信するように構成できます。 既定では、このプッシュ通知はオフに設定されています。 この設定は、Microsoft エンドポイント マネージャーで **[テナント管理]**  >  **[カスタマイズ]** を選択すると見つかります。 デバイスの所有権がエンドユーザーに与える影響の詳細については、「[デバイス所有権を変更する](../enrollment/corporate-identifiers-add.md#change-device-ownership)」を参照してください。

#### <a name="group-targeting-support-for-customization-pane---4722837----"></a>[カスタマイズ] ペインのグループのターゲット サポート<!-- 4722837  -->
**[カスタマイズ]** ペインの設定をユーザー グループをターゲットにすることができます。 Intune でこれらの設定を見つけるには、[Microsoft Endpoint Manager admin center](https://go.microsoft.com/fwlink/?linkid=2109431) に移動し、 **[テナント管理]**  >  **[カスタマイズ]** の順に選択します。 カスタマイズに関する詳細については、「[Intune ポータル サイト アプリ、ポータル サイト Web サイト、および Intune アプリをカスタマイズする方法](../apps/company-portal-app.md)」を参照してください。


<!-- vvvvvvvvvvvvvvvvvvvvvv -->
### <a name="device-configuration"></a>デバイスの構成

#### <a name="multiple-evaluate-each-connection-attempt-on-demand-vpn-rules-supported-on-ios-ipados-and-macos---6424615----"></a>iOS、iPadOS、macOS でサポートされている、複数の "接続が試みられるたびに評価する" オンデマンド VPN 規則<!-- 6424615  -->
Intune ユーザー エクスペリエンスでは、**接続が試みられるたびに評価する**アクションによって、同じ VPN プロファイル内で複数のオンデマンド VPN 規則を使用できます。( **[デバイス]**  >  **[構成プロファイル]**  >  **[プロファイルの作成]**  >  プラットフォームが **[iOS/iPadOS]** または **[macOS]** > プロファイルが **[VPN]** > **[自動 VPN]**  >  **[オンデマンド]** )。

リスト内の最初の規則のみが受け入れられます。 この動作は固定で、Intune によってリスト内のすべての規則が評価されます。 各規則は、オンデマンド規則リストに表示されている順序で評価されます。

> [!NOTE]
> これらのオンデマンド VPN 規則を使用する既存の VPN プロファイルがある場合、次回 VPN プロファイルを変更したときに修正が適用されます。 たとえば、接続の名前を変更してから、プロファイルを保存するなど、小さな変更を行います。
>
> 認証に SCEP 証明書を使用している場合、この変更により、この VPN プロファイルの証明書が再発行されます。

適用対象:
- iOS/iPadOS
- macOS

VPN プロファイルの詳細については、「[VPN プロファイルの作成](../configuration/vpn-settings-configure.md)」を参照してください。

#### <a name="additional-options-in-sso-and-sso-app-extension-profiles-on-iosipados-devices---6504155-----"></a>iOS/iPadOS デバイスでの SSO および SSO アプリ拡張機能プロファイルの追加オプション<!-- 6504155   -->

iOS/iPadOS デバイスでは、次のことができます。
- SSO プロファイル ( **[デバイス]**  >  **[構成プロファイル]**  >  **[プロファイルの作成]**  > プラットフォームに **[iOS/iPadOS]** > プロファイルに **[デバイスの機能]** > **[シングル サインオン]** ) で、Kerberos プリンシパル名が SSO プロファイルのセキュリティ アカウント マネージャー (SAM) アカウント名になるように設定します。 
- SSO アプリ拡張機能プロファイル ( **[デバイス]**  >  **[構成プロファイル]**  >  **[プロファイルの作成]**  > プラットフォームに **[iOS/iPadOS]** > プロファイルに **[デバイスの機能]** > **[シングル サインオン アプリの拡張機能]** ) で、新しい SSO アプリ拡張機能の種類を使用して、より少ないクリック回数で iOS/iPadOS Microsoft Azure AD 拡張機能を構成します。 共有デバイス モードでデバイスの Azure AD 拡張機能を有効にし、拡張機能固有データを拡張機能に送信できます。

適用対象:
- iOS/iPadOS 13.0 以降

iOS/iPadOS デバイスでのシングル サインオンの使用に関する詳細については、[シングル サインオン アプリの拡張機能の概要](../configuration/device-features-configure.md#single-sign-on-app-extension)と[シングル サインオンの設定リスト](../configuration/ios-device-features-settings.md#single-sign-on-app-extension)を参照してください。

<!-- vvvvvvvvvvvvvvvvvvvvvv -->
### <a name="device-enrollment"></a>デバイスの登録

#### <a name="delete-apple-automated-device-enrollment-token-when-default-profile-is-present--6393220---"></a>既定のプロファイルが存在する場合に、Apple 自動デバイス登録トークンを削除する<!--6393220 -->
以前は、既定のプロファイルを削除できませんでした。これは、関連付けられている自動デバイス登録トークンを削除できなかったことを意味します。 次の場合にトークンを削除できるようになりました。
- トークンに割り当てられているデバイスがない
- 既定のプロファイルが存在する。それを行うには、既定のプロファイルを削除してから、関連付けられているトークンを削除します。
詳細については、「[Intune から ADE トークンを削除する](../enrollment/device-enrollment-program-enroll-ios.md#delete-an-ade-token-from-intune)」を参照してください。

#### <a name="scaled-up-support-for-apple-automated-device-enrollment-and-apple-configurator-2-devices-profiles-and-tokens--3542402---"></a>Apple 自動デバイス登録と Apple Configurator 2 デバイス、プロファイル、トークンの拡張されたサポート<!--3542402 -->
分散した IT 部門と組織を支援するために、Intune では、トークンあたり最大 1000 の登録プロファイル、Intune アカウントあたり 2000 の自動デバイス登録 (旧称 DEP) トークン、およびトークンあたり 75000 のデバイスがサポートされるようになりました。 登録プロファイルあたりのデバイス数に特定の制限はなく、トークンあたりのデバイスの最大数未満です。

Intune では、最大 1000 の Apple Configurator 2 プロファイルがサポートされるようになりました。

詳細については、「[サポートされるボリューム](../enrollment/device-enrollment-program-enroll-ios.md#supported-volume)」を参照してください。

#### <a name="all-devices-page-column-entry-changes--6967616---"></a>[すべてのデバイス] ページの列エントリの変更<!--6967616 -->
**すべてのデバイス** ページで、**管理者** 列のエントリが変更されました。
- *MDM* ではなく、*Intune* が 表示されるようになりました
- *MDM/ConfigMgr エージェント*ではなく、* 共同管理*が表示されるようになりました

エクスポート値は変更されていません。

<!-- vvvvvvvvvvvvvvvvvvvvvv -->
### <a name="device-management"></a>デバイス管理

#### <a name="trusted-platform-manager-tpm-version-information-now-on-device-hardware-page--6224914-idmiss---"></a>トラステッド プラットフォーム マネージャー (TPM) のバージョン情報がデバイス ハードウェア ページに表示される<!--6224914 idmiss -->
デバイスのハードウェア ページに TPM バージョン番号が表示されるようになりました ([Microsoft Endpoint Manager admin center](https://go.microsoft.com/fwlink/?linkid=2109431) >  **[デバイス]** > デバイスの選択 > **[ハードウェア]** > **[システム格納装置]** の下を参照)。

<!-- vvvvvvvvvvvvvvvvvvvvvv -->
### <a name="monitor-and-troubleshoot"></a>監視とトラブルシューティング

#### <a name="collect-logs-to-better-troubleshoot-scripts-assigned-to-macos-devices---6359853----"></a>ログを収集して macOS デバイスに割り当てられているスクリプトのトラブルシューティングを改善する<!-- 6359853  -->
macOS デバイスに割り当てられているスクリプトのトラブルシューティングを改善するために、ログを収集できるようになりました。 ログは、60 MB (圧縮) または 25 個のファイルのどちらか先に発生するまで収集できます。 詳細については、「[ログ収集を使用した macOS シェル スクリプト ポリシーのトラブルシューティング](../apps/macos-shell-scripts.md#troubleshoot-macos-shell-script-policies-using-log-collection)」を参照してください。
 

<!-- vvvvvvvvvvvvvvvvvvvvvv -->
### <a name="security"></a>セキュリティ

#### <a name="derived-credentials-to-provision-android-enterprise-fully-managed-devices-with-certificates--4839592------"></a>証明書によって Android Enterprise のフル マネージド デバイスをプロビジョニングするための派生資格情報<!--4839592    -->
Intune では、Android デバイスの認証方法として、[派生資格情報](../protect/derived-credentials.md)の使用がサポートされるようになりました。 派生資格情報は、証明書をデバイスに展開するためのアメリカ国立標準技術研究所 (NIST) 800-157 標準を実装したものです。 Android のサポートは、iOS/iPadOS を実行するデバイスのサポートを拡張したものです。

派生資格情報は、スマート カードのように、Personal Identity Verification (PIV) または Common Access Card (CAC) カードの使用に依存します。 モバイル デバイスのために派生資格情報を得るには、ユーザーは Microsoft Intune アプリから開始し、使用しているプロバイダーに固有の登録ワークフローに従います。 すべてのプロバイダーに共通することは、コンピューターのスマート カードを使用し、派生資格情報プロバイダーに対して認証するという要件です。 そのプロバイダーはその後、ユーザーのスマート カードから誘導されたデバイスに証明書を発行します。

VPN および Wi-Fi のデバイス構成プロファイル用の認証方法として派生資格情報を使用できます。 それらは、アプリ認証や、それをサポートするアプリケーションの S/MIME 署名と暗号化にも使用できます。

Intune では、Android で次の派生資格情報プロバイダーをサポートするようになりました。
- Entrust Datacard
- Intercede

サードパーティ プロバイダーの DISA Purebred は、今後のリリースで Android で使用できるようになります。

#### <a name="microsoft-edge-security-baseline-is-now-generally-available--6586139---"></a>Microsoft Edge のセキュリティ ベースラインの一般提供が開始<!--6586139 -->

*この新しいベースラインはこれから数週間かけてテナントにロールアウトされます。5 月の早い段階でこの新しいベースラインがすべてのテナントに与えられるものと予想しています。*

[Microsoft Edge のセキュリティ ベースライン](../protect/security-baselines.md#available-security-baselines)の新しいバージョンの提供が開始され、一般公開 (GA) としてリリースされました。 以前の Edge のベースラインはプレビュー段階でした。  新しいベースライン バージョンは 2020 年 4 月 (Edge バージョン 80 以降) に含まれます。 

この新しいベースラインのリリースによって、以前のベースライン バージョンに基づいてプロファイルを作成できなくなりますが、それらのバージョンで作成したプロファイルは引き続き使用できます。 また、[最新のベースライン バージョンを使用するように、既存のプロファイルを更新する](../protect/security-baselines.md#change-the-baseline-version-for-a-profile)こともできます。 

<!-- ########################## -->
## <a name="week-of-april-6-2020"></a>2020 年 4 月 6 日の週

#### <a name="new-shell-script-settings-for-macos-devices---6884363---"></a>macOS デバイス向けの新しいシェル スクリプト設定<!-- 6884363 -->
macOS デバイス向けのシェル スクリプトを構成するときに、次の新しい設定を構成できるようになりました。 
- デバイスでスクリプトの通知を非表示にする
- スクリプトの頻度
- スクリプトが失敗した場合の再試行回数の最大値

詳細については、「[Intune で macOS デバイスに対してシェル スクリプトを使用する](../apps/macos-shell-scripts.md)」を参照してください。

<!-- ########################## -->
## <a name="week-of-march-30-2020"></a>2020 年 3 月 30 日の週

### <a name="new-url-for-the-microsoft-endpoint-manager-admin-center---3704810---"></a>Microsoft Endpoint Manager admin center の新しい URL<!-- 3704810 -->
昨年の Ignite での Microsoft エンドポイント マネージャーの発表に合わせて、Microsoft Endpoint Manager admin center (旧称 Microsoft 365 デバイス管理) の URL を [https://endpoint.microsoft.com](https://endpoint.microsoft.com) に変更しました。 古い管理センターの URL ([https://devicemanagement.microsoft.com](https://devicemanagement.microsoft.com)) は引き続き機能しますが、新しい URL を使用して Microsoft Endpoint Manager admin center へのアクセスを開始することをお勧めします。

詳細については、「[Microsoft Endpoint Manager admin center を使用して IT タスクを簡略化する](what-is-device-management.md#simplify-it-tasks-using-the-device-management-admin-center)」を参照してください。  


### <a name="app-management"></a>アプリ管理  

#### <a name="company-portal-for-ios-supports-landscape-mode--6048329----"></a>iOS 用ポータル サイトでの横向きモードのサポート<!--6048329  -->   
ユーザーは、好みの画面の向きを使用して、デバイスを登録したり、アプリを検索したり、IT サポートを受けたりできるようになりました。 ユーザーが縦向きモードで画面をロックしない限り、アプリでは画面を縦向きまたは横向きモードに合わせて自動的に検出して調整します。  

#### <a name="script-support-for-macos-devices-public-preview---4280361----"></a>macOS デバイスのスクリプト サポート (パブリック プレビュー)<!-- 4280361  -->
macOS デバイスにスクリプトを追加して展開できます。 このサポートにより、macOS デバイスを構成する機能が拡張され、macOS デバイスでネイティブの MDM 機能を使用してできること以上のことが可能になります。 詳細については、「[Intune で macOS デバイスに対してシェル スクリプトを使用する](../apps/macos-shell-scripts.md)」を参照してください。

<!-- ########################## -->
## <a name="week-of-march-24-2020"></a>2020 年 3 月 24 日の週

### <a name="improved-user-interface-experience-when-creating-device-restrictions-profiles-on-android-and-android-enterprise-devices---5841361---"></a>Android および Android Enterprise デバイスでデバイス制限プロファイルを作成するときのユーザー インターフェイス エクスペリエンスの向上<!-- 5841361 -->
Android または Android Enterprise デバイス用のプロファイルを作成するときの、Endpoint Management 管理センターのエクスペリエンスが更新されます。 この変更は、次のデバイス構成プロファイルに影響します ( **[デバイス]**  >  **[構成プロファイル]**  >  **[プロファイルの作成]**  > **プラットフォームの [Android デバイス管理者]** または **[Android Enterprise]** )。

- デバイスの制限:Android デバイス管理者
- デバイスの制限:Android Enterprise デバイス所有者
- デバイスの制限:Android Enterprise 仕事用プロファイル

構成できるデバイスの制限の詳細については、[Android デバイス管理者](../configuration/device-restrictions-android.md)と [Android Enterprise](../configuration/device-restrictions-android-for-work.md) に関するページを参照してください。

### <a name="improved-user-interface-experience-when-creating-configuration-profiles-on-iosipados-and-macos-devices---5569002-5568997---"></a>iOS/iPadOS および macOS デバイスで構成プロファイルを作成するときのユーザー インターフェイス エクスペリエンスの向上<!-- 5569002 5568997 -->
iOS または macOS デバイス用のプロファイルを作成するときの、エンドポイント管理センターのエクスペリエンスが更新されます。 この変更は、次のデバイス構成プロファイルに影響します ( **[デバイス]**  >  **[構成プロファイル]**  >  **[プロファイルの作成]**  >  プラットフォームの **[iOS/iPadOS]** または **[macOS]** ):

- カスタム: iOS/iPadOS、macOS
- デバイスの機能: iOS/iPadOS、macOS
- デバイスの制限: iOS/iPadOS、macOS
- エンドポイント保護: macOS
- 拡張機能: macOS
- 設定ファイル: macOS

### <a name="hide-from-user-configuration-setting-in-device-features-on-macos-devices---6524869---"></a>macOS デバイスのデバイス機能でユーザー構成設定を非表示にする<!-- 6524869 -->

macOS デバイスでデバイス機能の構成プロファイルを作成するときに、新しい設定 **[ユーザーの構成を非表示にします]** があります ( **[デバイス]**  >  **[構成プロファイル]**  >  **[プロファイルの作成]**  >  プラットフォームに **[macOS]** > プロファイルに **[デバイスの機能]** > **[ログイン項目]** )。

この機能では、macOS デバイスの **[ユーザーとグループ]** ログイン項目アプリのリストに、アプリの非表示のチェックマークが設定されます。 既存のプロファイルでは、この設定が未構成としてリスト内に表示されます。 この設定を構成するために、管理者は既存のプロファイルを更新できます。

**[非表示]** に設定すると、アプリの [非表示] チェックボックスがオンになり、ユーザーは変更することはできません。 また、ユーザーが自分のデバイスにサインインした後に、ユーザーに対してアプリを非表示にします。

> [!div class="mx-imgBorder"]
> ![Microsoft Intune とエンドポイント マネージャーでユーザーがデバイスにサインインした後に macOS デバイスでアプリを非表示にする](./media/whats-new/macos-hide-checkmark-users-groups-login-items-apps-list.png)

構成できる設定の詳細については、[macOS デバイスの機能設定](../configuration/macos-device-features-settings.md)に関する記事を参照してください。

この機能は、以下に適用されます。

- macOS

## <a name="week-of-march-16-2020-2003-service-release"></a>2020 年 3 月 16 日の週 (2003 サービス リリース)

<!-- vvvvvvvvvvvvvvvvvvvvvv -->
### <a name="app-management"></a>アプリ管理

#### <a name="macos-and-ios-company-portal-updates---5779439-5780234----"></a>macOS および iOS ポータル サイトの更新<!-- 5779439, 5780234  -->
macOS および iOS ポータル サイトの [プロファイル] ウィンドウが更新され、サインアウト ボタンが追加されました。 さらに、macOS ポータル サイトの [プロファイル] ウィンドウは UI が改善されました。 ポータル サイトの詳細については、「[Microsoft Intune ポータル サイト アプリを構成する方法](../apps/company-portal-app.md)」をご覧ください。

#### <a name="retarget-web-clips-to-microsoft-edge-on-ios-devices---5455276-----"></a>iOS デバイス上の Microsoft Edge に Web クリップを再ターゲットする<!-- 5455276   -->
保護されたブラウザーで開く必要がある、iOS デバイス上の新たに展開された Web クリップ (ピン留めされた Web アプリ) は、Intune Managed Browser ではなく Microsoft Edge で開かれます。 既存の Web クリップを再ターゲットして、Managed Browser ではなく Microsoft Edge で開くようにする必要があります。 詳細については、「[Microsoft Edge と Microsoft Intune を使用して Web アクセスを管理する](../apps/manage-microsoft-edge.md)」および「[Web アプリを Microsoft Intune に追加する](../apps/web-app.md)」をご覧ください。

#### <a name="use-the-intune-diagnostic-tool-with-microsoft-edge-for-android---4735244----"></a>Android 用 Microsoft Edge で Intune 診断ツールを使用する<!-- 4735244  -->
Android 用 Microsoft Edge が Intune 診断ツールと統合されました。 iOS 用 Microsoft Edge のエクスペリエンスと同様に、デバイス上の Microsoft Edge の URL バー (アドレス ボックス) に「about:intunehelp」と入力すると、Intune 診断ツールが開始されます。 このツールでは、詳細なログが提供されます。 ユーザーは、ガイドを利用しながら、これらのログを収集して IT 部門に送信したり、特定のアプリの MAM ログを表示したりできます。

#### <a name="updates-to-intune-branding-and-customization---5236032----"></a>Intune のブランド化とカスタマイズの更新<!-- 5236032  -->
"ブランド化とカスタマイズ" という名前だった Intune ウィンドウが更新され、次のような改善が加えられました。

- ペインの名前を**カスタマイズ**に変更。
- 設定の編成と設計の改善。
- 設定のテキストとヒントの改善。

Intune でこれらの設定を見つけるには、[Microsoft Endpoint Manager admin center](https://go.microsoft.com/fwlink/?linkid=2109431) に移動し、 **[テナント管理]**  >  **[カスタマイズ]** の順に選択します。 既存のカスタマイズについては、「[Microsoft Intune ポータル サイト アプリを構成する方法](../apps/company-portal-app.md)」を参照してください。

#### <a name="users-personal-encrypted-recovery-key---6273943----"></a>ユーザーの個人用の暗号化された回復キー<!-- 6273943  -->
ユーザーが Android ポータル サイト アプリケーションまたは Android Intune アプリケーションを介して、Mac デバイスの個人用の暗号化された **FileVault** 回復キーを取得できるようにする、新しい Intune 機能を使用できます。 ポータル サイト アプリケーションと Intune アプリケーションの両方にリンクが表示されます。これを使用すると、Chrome ブラウザーで Web ポータル サイトが開き、そこでユーザーは Mac デバイスにアクセスするために必要な **FileVault** 回復キーを確認できます。 暗号化の詳細については、「[Intune でデバイスの暗号化を使用する](../protect/encrypt-devices.md)」を参照してください。

#### <a name="optimized-dedicated-device-enrollment----6114580----"></a>専用デバイスの登録の最適化 <!-- 6114580  -->
Android エンタープライズ専用デバイスの登録を最適化し、Wi-Fi に関連付けられた SCEP 証明書を 2019 年 11 月 22 日より前に登録した専用デバイスに適用しやすくしています。 新しい登録の場合、Intune アプリは引き続きインストールされますが、エンド ユーザーは登録中に **Intune エージェントを有効にする**手順を実行する必要がなくなります。 インストールはバックグラウンドで自動的に行われ、Wi-Fi に関連付けられた SCEP 証明書はエンド ユーザーの介入なしで展開および設定できます。  

これらの変更は、Intune サービス バックエンドの展開として 3 月中に段階的にロールアウトされます。 3 月の終わりまでに、すべてのテナントでこの新しい動作が実現されます。 関連情報については、「[Android エンタープライズ専用デバイスでの SCEP 証明書のサポート](https://techcommunity.microsoft.com/t5/intune-customer-success/support-for-scep-certificates-in-android-enterprise-dedicated/ba-p/928147)」をご覧ください。

<!-- vvvvvvvvvvvvvvvvvvvvvv -->
### <a name="device-configuration"></a>デバイスの構成

#### <a name="new-user-experience-when-creating-administrative-templates-on-windows-devices--5096036---"></a>Windows デバイスに対する管理用テンプレートを作成するときの新しいユーザー エクスペリエンス<!--5096036 -->
お客様からのフィードバックに基づき、新しい Azure の全画面表示エクスペリエンスへの移行に伴って、管理用テンプレート プロファイルのエクスペリエンスをフォルダー ビューを使用して再構築しました。 設定や既存のプロファイルに対する変更は加えられていません。 そのため、お使いの既存のプロファイルは変更されず、そのまま新しいビューで使用できます。 **[すべての設定]** を選択し、検索を使用することで、引き続きすべての設定オプションを参照できます。 ツリー ビューは、コンピューターの構成とユーザーの構成によって分割されます。 Windows、Office、および Edge の設定は、その関連するフォルダーに配置されます。  

適用対象:
- Windows 10 以降

#### <a name="vpn-profiles-with-ikev2-vpn-connections-can-use-always-on-with-iosipados-devices---1947932-----"></a>IKEv2 VPN 接続を使用する VPN プロファイルでは iOS/iPadOS デバイスで常時接続を使用できる<!-- 1947932   -->
iOS/iPadOS デバイスでは、IKEv2 接続を使用する VPN プロファイルを作成することができます ( **[デバイス]**  >  **[構成プロファイル]**  >  **[プロファイルの作成]**  >  プラットフォームの **[iOS/iPadOS]** > プロファイル タイプの **[VPN]** )。 現在、IKEv2 を使用して常時接続を構成できます。 構成すると、IKEv2 VPN プロファイルは自動的に接続され、VPN に接続されたままになります (またはすぐに再接続されます)。 ネットワーク間を移動したり、デバイスを再起動したりしても、接続されたままになります。

iOS/iPadOS では、常時接続 VPN は IKEv2 プロファイルに限定されます。

構成できる IKEv2 設定については、[Microsoft Intune で iOS デバイス向けの VPN 設定を追加する方法](../configuration/vpn-settings-ios.md#ikev2-settings)に関する記事をご覧ください。

適用対象:
- iOS/iPadOS

#### <a name="delete-bundles-and-bundle-arrays-in-oemconfig-device-configuration-profiles-on-android-enterprise-devices---5550355-----"></a>Android Enterprise デバイスで OEMConfig デバイス構成プロファイルのバンドルとバンドル配列を削除する<!-- 5550355   -->
Android エンタープライズ デバイスでは、OEMConfig プロファイルを作成して構成します ( **[デバイス]**  >  **[構成プロファイル]**  >  **[プロファイルの作成]**  >  プラットフォームの **[Android Enterprise]** > プロファイルの種類の **[OEMConfig]** )。 現在、ユーザーは、Intune の**構成デザイナー**を使用して、バンドルとバンドル配列を削除できます。

OEMConfig プロファイルの詳細については、「[Microsoft Intune で、OEMConfig を使って Android Enterprise デバイスを使用および管理する](../configuration/android-oem-configuration-overview.md)」を参照してください。

適用対象:
- Android エンタープライズ

#### <a name="configure-the-iosipados-microsoft-azure-ad-sso-app-extension---5672534-----"></a>iOS/iPadOS の Microsoft Azure AD SSO アプリ拡張機能を構成する<!-- 5672534   -->
Microsoft Azure AD チームは、iOS/iPadOS 13.0 以降のユーザーが、1 回のサインオンで Microsoft アプリと Web サイトにアクセスできるようにするために、リダイレクト シングル サインオン (SSO) アプリ拡張機能を開発しました。 以前に Microsoft Authenticator アプリで仲介型認証を使用していたすべてのアプリは、新しい SSO 拡張機能で引き続き SSO を取得します。 Azure AD SSO アプリ拡張機能のリリースに伴い、リダイレクト SSO アプリ拡張機能の種類を使用して SSO 拡張機能を構成できます ( **[デバイス]**  >  **[構成プロファイル]**  >  **[プロファイルの作成]**  >  プラットフォームの **[iOS/iPadOS]** > プロファイルの種類の **[デバイスの機能]** > **[シングル サインオン アプリ拡張機能]** )。

適用対象:
- iOS 13.0 以降
- iPadOS 13.0 以降

iOS SSO アプリ拡張機能について詳しくは、「[シングル サインオン アプリ拡張機能](../configuration/device-features-configure.md#single-sign-on-app-extension)」をご覧ください。

#### <a name="enterprise-app-trust-settings-modification-setting-is-removed-from-iosipados-device-restriction-profiles---6225131-----"></a>[エンタープライズ アプリの信頼設定の変更] 設定が iOS/iPadOS デバイスの制限プロファイルから削除される<!-- 6225131   -->
iOS/iPadOS デバイス上に、デバイスの制限プロファイルを作成します ( **[デバイス]**  >  **[構成プロファイル]**  >  **[プロファイルの作成]**  > プラットフォームとして **[iOS/iPadOS]** > プロファイルの種類として **[デバイスの制限]** )。 **[エンタープライズ アプリの信頼設定の変更]** 設定は、Apple によって削除され、Intune から削除されます。 プロファイルで現在この設定を使用している場合、それは影響を及ぼさず、既存のプロファイルから削除されます。 この設定は、Intune のレポートからも削除されます。

適用対象:
- iOS/iPadOS

制限できる設定を確認するには、[機能を許可または制限するための iOS および iPadOS デバイスの設定](../configuration/device-restrictions-ios.md)に関するページに移動します。

#### <a name="troubleshooting-pending-mam-policy-notification-changed-to-informational-icon--6348954---"></a>トラブルシューティング:保留中の MAM ポリシーの通知が情報アイコンに変更されました<!--6348954 -->
トラブルシューティング ブレードでの保留中の MAM ポリシーの通知アイコンが、情報アイコンに変更されました。

####  <a name="ui-update-when-configuring-compliance-policy---3961639------"></a>コンプライアンス ポリシーを構成するときの UI の更新<!-- 3961639    -->

Microsoft Endpoint Manager で[コンプライアンス ポリシーを作成する](../protect/create-compliance-policy.md#create-the-policy)ための UI が更新されました ( **[デバイス]**  >  **[コンプライアンス ポリシー]**  >  **[ポリシー]**  >  **[ポリシーの作成]** )。 以前に使用していたのと同じ設定と詳細情報を含む新しいユーザー エクスペリエンスが提供されます。 新しいエクスペリエンスでは、ウィザードのようなプロセスに従ってコンプライアンス ポリシーを作成することができ、ポリシーの *[割り当て]* を追加できるページと、ポリシーを作成する前に構成を確認できる *[確認および作成]* ページが含まれます。

#### <a name="retire-noncompliant-devices---1827291---------"></a>非準拠デバイスをインベントリから削除する<!-- 1827291       -->
任意のポリシーに追加できる、準拠していないデバイスに対する新しいアクション、[準拠していないデバイスをインベントリから削除](../protect/actions-for-noncompliance.md#add-actions-for-noncompliance)が追加されました。  この新しいアクション **[準拠していないデバイスを削除します]** を使用すると、そのデバイスから会社のデータがすべて削除され、また、そのデバイスが Intune による管理対象から削除されます。  このアクションは、構成した日数の値に達し、その時点でデバイスがインベントリから削除可能になったときに実行されます。 最小値は 30 日間です。  デバイスをインベントリから削除するには、IT 管理者の明示的な承認が必要になります。その場合、 *[準拠していないデバイスを削除します]* セクションを使用し、そこで管理者は対象となるすべてのデバイスをインベントリから削除できます。

#### <a name="support-for-wpa-and-wpa2-in-ios-enterprise-wi-fi-profiles--6215273-----"></a>iOS エンタープライズ Wi-Fi プロファイルでの WPA と WPA2 のサポート<!--6215273   -->
[iOS 用エンタープライズ Wi-Fi プロファイル](../configuration/wi-fi-settings-ios.md#enterprise-profiles)で、 *[セキュリティの種類]* フィールドがサポートされるようになりました。 *[セキュリティの種類]* には、**WPA エンタープライズ**または **WPA/WPA2 エンタープライズ**のいずれかを選択した後、 *[EAP の種類]* の選択を指定できます。  ( **[デバイス]**  >  **[構成プロファイル]**  >  **[プロファイルの作成]** で、 *[プラットフォーム]* に **[iOS/iPadOS]** を選択し、 *[プロファイル]* に **[Wi-Fi]** を選択します)。 

新しいエンタープライズ オプションは、iOS 用の基本的な Wi-Fi プロファイルに対して使用できたオプションと似ています。

#### <a name="new-user-experience-for-certificate-email-vpn-and-wi-fi-vpn-profiles---5615208-----"></a>証明書、電子メール、VPN、および Wi-Fi、VPN プロファイルの新しいユーザー エクスペリエンス<!-- 5615208   -->
Endpoint Management 管理センターで次のプロファイルの種類の作成および変更を行うための[ユーザー エクスペリエンス](../configuration/device-profile-create.md)が更新されました ( **[デバイス]**  >  **[構成プロファイル]**  >  **[プロファイルの作成]** )。 新しいエクスペリエンスでは、以前と同じ設定が表示されますが、あまり水平スクロールを必要としないウィザードのようなエクスペリエンスが使用されます。 新しいエクスペリエンスで既存の構成を変更する必要はありません。

- 派生資格情報
- 電子メール
- PKCS 証明書
- PKCS のインポートされた証明書
- SCEP 証明書
- 信頼された証明書
- VPN
- Wi-Fi

<!-- vvvvvvvvvvvvvvvvvvvvvv -->
### <a name="device-enrollment"></a>デバイスの登録

#### <a name="configure-if-enrollment-is-available-in-company-portal-for-android-and-ios---4260128----"></a>Android と iOS 用のポータル サイトで登録を使用できるようにするかどうかを構成する<!-- 4260128  -->
Android および iOS デバイス上のポータル サイトでのデバイス登録を、プロンプトを表示して使用できるようにするか、プロンプトを表示せずに使用できるようにするか、またはユーザーが使用できないようにするかを構成できます。 Intune でこれらの設定を見つけるには、[Microsoft Endpoint Manager admin center](https://go.microsoft.com/fwlink/?linkid=2109431) に移動し、 **[テナント管理]**  >  **[カスタマイズ]**  >  **[編集]**  >  **[デバイスの登録]** の順に選択します。  

デバイス登録設定をサポートするには、エンド ユーザーに次のバージョンのポータル サイトが必要です。
-    iOS 上のポータル サイト: バージョン 4.4 以降
-    Android 上のポータル サイト: バージョン 5.0.4715.0 以降

既存のポータル サイトのカスタマイズについては、「[Microsoft Intune ポータル サイト アプリを構成する方法](../apps/company-portal-app.md)」を参照してください。

<!-- vvvvvvvvvvvvvvvvvvvvvv -->
### <a name="device-management"></a>デバイス管理

#### <a name="new-android-report-on-android-devices-overview-page---5435435-----"></a>Android デバイスの概要ページの新しい Android レポート<!-- 5435435   -->
Microsoft Endpoint Manager 管理コンソールの Android デバイスの概要ページに、各デバイス管理ソリューションに登録されている Android デバイスの数を表示するレポートが追加されました。 このグラフ (Azure コンソールに既にあるのと同じような) には、仕事用プロファイル、フル マネージド、専用、およびデバイス管理者が登録したデバイスの数が表示されます。 レポートを表示するには、 **[デバイス]**  >  **[Android]**  >  **[概要]** の順に選択します。

#### <a name="guide-users-from-android-device-administrator-management-to-work-profile-management--5857738---wnstaged--"></a>Android デバイス管理者の管理から仕事用プロファイルの管理にユーザーをガイドする<!--5857738   wnstaged-->
Android デバイス管理者プラットフォーム用の新しいコンプライアンス設定をリリースしています。 この設定を使用すると、デバイス管理者によって管理される場合にデバイスを非準拠にすることができます。

これらの非準拠デバイスでは、 **[デバイス設定の更新]** ページに、ユーザーに対して **[新しいデバイス管理セットアップに移動する]** メッセージが表示されます。 **[解決]** ボタンをタップすると、次のようにガイドされます。

1. デバイス管理者の管理からの登録解除
2. 仕事用プロファイルの管理への登録
3. コンプライアンスに関する問題の解決 
 
Google では、Android Enterprise を使用した最新のより豊富で安全なデバイス管理に移行するための取り組みの一環として、新しい Android リリースでのデバイス管理者サポートを縮小しています。  Intune では、Android 10 以降を実行している、デバイス管理者が管理する Android デバイスのフル サポートを 2020 年第 2 四半期までのみ提供できます。 これを過ぎると、Android 10 以降を実行している、デバイス管理者が管理するデバイス (Samsung を除く) は、完全には管理できなくなります。 具体的には、影響を受けるデバイスが新しいパスワード要件を受け取ることはありません。

この設定の詳細については、「[Android デバイスをデバイス管理者から仕事用プロファイル管理に移動する](../enrollment/android-move-device-admin-work-profile.md)」をご覧ください。 

<!-- vvvvvvvvvvvvvvvvvvvvvv -->
### <a name="monitor-and-troubleshoot"></a>監視とトラブルシューティング

#### <a name="the-data-warehouse-now-provides-the-mac-address---6123680----"></a>データ ウェアハウスでの MAC アドレスの提供開始<!-- 6123680  -->
Intune データ ウェアハウスでは、`device` エンティティ内の新しいプロパティ (`EthernetMacAddress`) として MAC アドレスが提供され、管理者がユーザーとホスト間の MAC アドレスを関連付けることができるようになります。 このプロパティは、特定のユーザーに接続し、そのネットワーク上で発生しているインシデントをトラブルシューティングするのに役立ちます。 また、管理者は、[Power BI レポート](../developer/reports-proc-get-a-link-powerbi.md)内でこのプロパティを使用し、より豊富な機能を備えたレポートを作成することもできます。 詳細については、Intune データ ウェアハウスの [device](../developer/intune-data-warehouse-collections.md#devices) エンティティを参照してください。

#### <a name="additional-data-warehouse-device-inventory-properties---6125732----"></a>追加のデータ ウェアハウス デバイス インベントリ プロパティ<!-- 6125732  -->
Intune データ ウェアハウスを使用して、追加のデバイス インベントリ プロパティを使用できます。 次のプロパティが、[device](../developer/intune-data-warehouse-collections.md#devices) コレクションを介して公開されるようになりました。
- 'Model' - デバイスのモデル。
- 'Office365Version' - デバイスにインストールされている Office 365 のバージョン。
- 'PhysicalMemoryInBytes' - 物理メモリ (バイト単位)。
- `TotalStorageSpaceInBytes` - 記憶域の合計容量 (バイト単位)。

詳細については、「[Microsoft Intune データ ウェアハウス API](../developer/reports-nav-intune-data-warehouse.md)」と、Intune データ ウェアハウスの [device](../developer/intune-data-warehouse-collections.md#devices) エンティティを参照してください。

#### <a name="help-and-support-workflow-update-to-support-additional-services---5654170-----"></a>追加サービスをサポートするためのヘルプとサポート ワークフローの更新<!-- 5654170   -->
Microsoft Endpoint Manager admin center の [ヘルプとサポート] ページが更新され、[使用する管理の種類を選択](../fundamentals/get-support.md#options-to-access-help-and-support)できるようになりました。 この変更により、次の管理の種類から選択できるようになります。

- Configuration Manager (Desktop Analytics を含む)
- Intune
- 共同管理

<!-- vvvvvvvvvvvvvvvvvvvvvv -->
### <a name="security"></a>セキュリティ

#### <a name="use-a-preview-of-security-administrator-focused-policies-as-part-of-endpoint-security--6131401----"></a>エンドポイント セキュリティの一部としてセキュリティ管理者に焦点を当てたポリシーのプレビューを使用する<!--6131401  -->
パブリック プレビューとして、Microsoft Endpoint Management 管理センターのエンドポイント セキュリティ ノードに、いくつかの新しいポリシー グループが追加されました。 セキュリティ管理者は、これらの新しいポリシーを使用してデバイス セキュリティに関する特定の側面に焦点を当て、より大きなデバイス構成ポリシー本文によるオーバーヘッドを発生させることなく、関連する設定の個別のグループを管理できます。

"*Microsoft Defender ウイルス対策のウイルス対策ポリシー*" を除き (下記参照)、これらの新しいプレビューの各ポリシーおよびプロファイルの設定は、現在既に[デバイス構成プロファイル](../configuration/device-profile-create.md)を使用して構成している可能性がある設定と同じものです。

すべてプレビューである新しいポリシーの種類と、その使用可能なプロファイルの種類を次に示します。

- **[ウイルス対策 (プレビュー)]** :
  - macOS:
    - **[ウイルス対策]** - macOS 用の[ウイルス対策ポリシーの設定](../protect/antivirus-microsoft-defender-settings-macos.md)を管理して、[Microsoft Defender ATP for Mac](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac) を管理します。

  - Windows 10 以降:
    - **[Microsoft Defender ウイルス対策]** - クラウド保護、ウイルス対策の除外、修復、スキャン オプションなどのための[ウイルス対策ポリシーの設定](../protect/antivirus-microsoft-defender-settings-windows.md)を管理します。

      *[Microsoft Defender ウイルス対策]* のウイルス対策プロファイルは、デバイス制限プロファイルの一部として検出される、設定の新しいインスタンスを導入する例外です。 これらの新しいウイルス対策の設定は:

        - デバイス制限で使用されるのと同じ設定ですが、デバイス制限として構成する場合は使用できない、構成の 3 番目のオプションがサポートされています。
        - Endpoint Protection の[共同管理ワークロードのスライダー](https://docs.microsoft.com/configmgr/comanage/how-to-switch-workloads)が Intune に設定されている場合に、Configuration Manager で共同管理されているデバイスに適用されます。

     デバイス制限プロファイルを使用して構成する代わりに、新しい *[ウイルス対策]*  >  *[Microsoft Defender ウイルス対策]* プロファイルを使用することを計画してください。

  - **[Windows セキュリティ エクスペリエンス]** - エンド ユーザーが Microsoft Defender セキュリティ センターで表示できる Windows セキュリティ設定と、エンド ユーザーが受信する通知を管理します。 これらの設定は、デバイス構成 Endpoint Protection プロファイルとして使用できる設定から変更されていません。

- **[ディスク暗号化 (プレビュー)]** :
  - macOS:
    - **FileVault**
  - Windows 10 以降:
    - **BitLocker**
- **[ファイアウォール (プレビュー)]** :
  - macOS:
    - **[macOS ファイアウォール]**
  - Windows 10 以降:
    - **Microsoft Defender ファイアウォール**
- **[エンドポイントの検出と応答 (プレビュー)]** :
  - Windows 10 以降:-**Windows 10 Intune**
- **[攻撃面の減少 (プレビュー)]** :
  - Windows 10 以降:
    - **[アプリとブラウザーの分離]**
    - **[Web 保護]**
    - **[アプリケーションの制御]**
    - **[攻撃の回避規則]**
    - **[デバイス制御]**
    - **[悪用に対する保護]**
- **[アカウント保護 (プレビュー)]** :
  - Windows 10 以降:
    - **[アカウント保護]**

<!-- ########################## -->
## <a name="week-of-march-9-2020"></a>2020 年 3 月 9 日の週

<!-- vvvvvvvvvvvvvvvvvvvvvv -->
### <a name="app-management"></a>アプリ管理

#### <a name="configure-delivery-optimization-agent-when-downloading-win32-app-content---5410945---"></a>Win32 アプリ コンテンツをダウンロードするときに配信の最適化エージェントを構成する<!-- 5410945 -->

配信の最適化エージェントを、割り当てに基づいてバックグラウンドまたはフォアグラウンド モードで Win32 アプリ コンテンツをダウンロードするように構成できます。 既存の Win32 アプリでは、コンテンツは引き続きバックグラウンド モードでダウンロードされます。 [Microsoft Endpoint Manager admin center](https://go.microsoft.com/fwlink/?linkid=2109431) で、 **[アプリ]**  >  **[すべてのアプリ]**  > "*Win32 アプリを選択*" >  **[プロパティ]** の順に選択します。 **[割り当て]** の横にある **[編集]** を選択します。  **[必須]** セクションの **[モード]** の下で **[含める]** を選択して、割り当てを編集します。  **[アプリの設定]** セクションに新しい設定が表示されます。 配信の最適化の詳細については、[「Win32 アプリ管理」の「配信の最適化」](../apps/apps-win32-app-management.md#delivery-optimization)を参照してください。

<!-- vvvvvvvvvvvvvvvvvvvvvv -->
### <a name="device-management"></a>デバイス管理

#### <a name="change-primary-user-for-windows-devices---3794742-----"></a>Windows デバイスのプライマリ ユーザーを変更する<!-- 3794742   -->
Windows ハイブリッド デバイスと Azure AD 参加済みデバイスのプライマリ ユーザーを変更できます。 これを行うには、 **[Intune]**  >  **[デバイス]**  >  **[すべてのデバイス]** > デバイスを選択 > **[プロパティ]**  >  **[プライマリ ユーザー]** を選択します。 詳細については、「[デバイスのプライマリ ユーザーを変更する](../remote-actions/find-primary-user.md#change-a-devices-primary-user)」をご覧ください。

このタスクに対して、新しい RBAC アクセス許可 (マネージド デバイス/プライマリ ユーザーの設定) も作成されています。 このアクセス許可は、ヘルプデスク オペレーター、学校管理者、エンドポイント セキュリティ マネージャーなどの組み込みロールに追加されています。

この機能は、プレビューとしてグローバルにお客様にロールアウトされています。 この機能は、今後数週間以内に表示されるはずです。


<!-- ########################## -->
## <a name="week-of-march-2-2020"></a>2020 年 3 月 2 日の週

<!-- vvvvvvvvvvvvvvvvvvvvvv -->
### <a name="device-management"></a>デバイス管理

#### <a name="microsoft-endpoint-manager-tenant-attach-device-sync-and-device-actions---6317104-cm3555758--"></a>Microsoft Endpoint Manager テナントのアタッチ:デバイスの同期とデバイスのアクション<!-- 6317104, CM3555758-->
Microsoft Endpoint Manager によって、Configuration Manager と Intune が 1 つのコンソールに統合されます。 Configuration Manager Technical Preview バージョン 2002.2 以降、ご利用の Configuration Manager デバイスをクラウド サービスにアップロードし、管理センターからそれらに対するアクションを実行できます。 詳細については、[Configuration Manager Technical Preview バージョン 2002.2 の機能](https://docs.microsoft.com/configmgr/core/get-started/2020/technical-preview-2002-2#bkmk_attach)に関する記事をご覧ください。

この更新プログラムをインストールする前に、[Configuration Manager Technical Preview に関する記事](https://docs.microsoft.com/configmgr/core/get-started/technical-preview)をご確認ください。 この記事により、Technical Preview の使用に関する一般的な要件と制限事項、バージョン間の更新方法、フィードバックを提供する方法についての理解を深めることができます。

#### <a name="bulk-remote-actions--4576882--"></a>一括リモート操作<!--4576882-->
次のリモート操作に対して、一括コマンドを発行できるようになりました: 再起動、名前変更、Autopilot リセット、ワイプ、削除。 新しい一括操作を表示するには、[Microsoft Endpoint Manager admin center](https://go.microsoft.com/fwlink/?linkid=2109431) >  **[デバイス]**  >  **[すべてのデバイス]**  >  **[Bulk actions]\(一括操作\)** の順に移動します。

#### <a name="all-devices-list-improved-search-sort-and-filter--6179023--"></a>すべてのデバイス リストで検索、並べ替え、フィルターが改善<!--6179023-->
[すべてのデバイス] リストが改善され、パフォーマンスが上がり、検索、並べ替え、フィルター処理の各種機能が強化されました。 詳細については、[こちらのサポート ヒント](https://techcommunity.microsoft.com/t5/intune-customer-success/support-tip-changes-in-all-devices-list-and-reporting-in-intune/ba-p/1220946)に関する記事をご覧ください。  

### <a name="app-management"></a>アプリ管理  
####  <a name="improved-sign-in-experience-in-company-portal-for-android"></a>Android 用ポータル サイトでのサインイン エクスペリエンスの向上    
エクスペリエンスをユーザーにとってより新しく、シンプルでクリーンなものにするために、Android 用ポータル サイト アプリのいくつかのサインイン画面のレイアウトを更新しました。 機能強化の詳細については、「[アプリの UI の新機能](https://docs.microsoft.com/mem/intune/fundamentals/whats-new-app-ui)」を参照してください。

<!-- ########################## -->
## <a name="week-of-february-24-2020"></a>2020 年 2 月 24 日の週

<!-- vvvvvvvvvvvvvvvvvvvvvv -->
### <a name="app-management"></a>アプリ管理

#### <a name="macos-company-portal-user-experience-improvements---5568987---"></a>macOS ポータル サイトのユーザー エクスペリエンスの向上<!-- 5568987 -->
macOS デバイスを登録しやすくし、Mac 用ポータル サイト アプリを改善しました。 次の点が改善されています。
- 登録時の Microsoft **AutoUpdate** エクスペリエンスが向上し、ユーザーが最新バージョンのポータル サイトを確実に使用できるようになります。
- 登録時のコンプライアンス チェック手順が強化されます。
- インシデント ID のコピーがサポートされるため、ユーザーは自分のデバイスから会社のサポート チームにエラーを迅速に送信することができます。

Mac の登録とポータルサイトアプリの詳細については、「[ポータル サイト アプリを使用して macOS デバイスを登録する](../user-help/enroll-your-device-in-intune-macos-cp.md)」を参照してください。

#### <a name="app-protection-policies-for-better-mobile-now-supports-ios-and-ipados---6224512----"></a>Better Mobile のアプリ保護ポリシーで iOS と iPadOS がサポートされるようになりました<!-- 6224512  -->

2019 年 10 月に、Intune アプリ保護ポリシーに、Microsoft の脅威防御パートナーのデータを使用する機能が追加されました。 この更新により、アプリ保護ポリシーを使用して、iOS と iPadOS で Better Mobile を使用するデバイスの正常性に基づいてユーザーの企業データをブロックしたり選択的にワイプしたりできるようになりました。  詳細については、「[Intune で Mobile Threat Defense アプリ保護ポリシーを作成する](../protect/mtd-app-protection-policy.md)」をご覧ください。

<!-- vvvvvvvvvvvvvvvvvvvvvv -->
### <a name="device-management"></a>デバイス管理

#### <a name="exports-from-the-all-devices-list--now-in-zipped-csv-format--6343117--"></a>すべてのデバイスのリストのエクスポートが CSV 形式で圧縮されるようになりました<!--6343117-->
**[デバイス]**  >  **[すべてのデバイス]** ページからのエクスポートが CSV 形式で圧縮されるようになりました。


<!-- ########################## -->
## <a name="week-of-february-17-2020-2002-service-release"></a>2020 年 2 月 17 日の週 (2002 サービス リリース)

<!-- vvvvvvvvvvvvvvvvvvvvvv -->
### <a name="app-management"></a>アプリ管理

#### <a name="microsoft-defender-advanced-threat-protection-atp-app-for-macos---5424618---"></a>macOS 用 Microsoft Defender Advanced Threat Protection (ATP) アプリ<!-- 5424618 -->
Intune を使用すると、macOS 用 Microsoft Defender Advanced Threat Protection (ATP) アプリを管理対象 Mac デバイスに簡単に展開できます。 詳細については、「[Microsoft Intune を使用して Microsoft Defender ATP を macOS に追加する](../apps/apps-advanced-threat-protection-macos.md)」と「[Microsoft Defender Advanced Threat Protection for Mac](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac)」を参照してください。  

<!-- vvvvvvvvvvvvvvvvvvvvvv -->
### <a name="device-configuration"></a>デバイスの構成

#### <a name="enable-network-access-control-nac-with-cisco-anyconnect-vpn-on-ios-devices---4860111----"></a>iOS デバイスで Cisco AnyConnect VPN を利用し、ネットワーク アクセス制御 (NAC) を有効にする<!-- 4860111  -->
iOS デバイスで、VPN プロファイルを作成し、Cisco AnyConnect など ( **[デバイス構成]**  >  **[プロファイル]**  >  **[プロファイルの作成]** の順に選択し > プラットフォームに **[iOS]** を選択し、プロファイルの種類に **[VPN]** を選択し、接続の種類に **[Cisco AnyConnect]** を選択する)、さまざまな種類の接続を使用できます。

Cisco AnyConnect を利用し、ネットワーク アクセス制御 (NAC) を有効にできます。 この機能を使用するには、以下を行います。

1. 「[Cisco Identity Services Engine 管理者ガイド](https://www.cisco.com/c/en/us/td/docs/security/ise/2-1/admin_guide/b_ise_admin_guide_21/b_ise_admin_guide_20_chapter_01000.html)」の「**Configuring Microsoft Intune as an MDM Server**」(Microsoft Intune の MDM サーバーとしての構成) に記載されている手順を利用し、Azure で Cisco Identity Services Engine (ISE) を構成します。
2. Intune デバイス構成プロファイルで、 **[ネットワーク アクセス制御 (NAC) を有効にする]** 設定を選択します。

利用できる VPN 設定については、[iOS デバイスへの VPN 設定の構成](../configuration/vpn-settings-ios.md)に関する記事を参照してください。

<!-- vvvvvvvvvvvvvvvvvvvvvv -->
### <a name="device-enrollment"></a>デバイスの登録

#### <a name="serial-number-on-the-apple-mdm-push-certificate-page--5947765----"></a>[Apple MDM プッシュ通知証明書] ページのシリアル番号<!--5947765  -->
[Apple MDM プッシュ通知証明書] ページにシリアル番号が表示されるようになりました。 証明書を作成した Apple ID へのアクセスが失われた場合に、Apple MDM プッシュ通知証明書へのアクセスを回復するには、シリアル番号が必要です。 シリアル番号を表示するには、 **[デバイス]**  >  **[iOS]**  >  **[iOS enrollment]\(iOS の登録\)**  >  **[Apple MDM プッシュ通知証明書]** に移動します。

<!-- vvvvvvvvvvvvvvvvvvvvvv -->
### <a name="device-management"></a>デバイス管理

#### <a name="new-update-schedule-options-for-pushing-os-updates-to-enrolled-iosipados-devices--5879689----"></a>登録された iOS デバイスまたは iPadOS デバイスに OS 更新プログラムをプッシュするための新しい更新スケジュール オプション<!--5879689  -->
iOS/iPadOS デバイスのオペレーティング システムの更新をスケジュールするとき、次のオプションから選択できます。 これらのオプションは、Apple Business Manager または Apple School Manager の登録タイプを使用したデバイスに適用されます。
- 次回のチェックイン時に更新する
- スケジュールされた時刻に更新する
- スケジュールされた時刻以外に更新する

後者の 2 つのオプションでは、複数の時間帯を作成できます。

新しいオプションを確認するには、MEM > **[デバイス]**  >  **[iOS]**  >  **[Update policies for iOS/iPadOS]\(iOS または iPadOS のポリシーを更新する\)**  >  **[プロファイルの作成]** に移動します。

#### <a name="choose-which-iosipados-updates-to-push-to-enrolled-devices--5879689----"></a>登録されたデバイスにプッシュする iOS または iPadOS の更新プログラムを選択する<!--5879689  -->
Apple Business Manager または Apple School Manager を使用すると、登録されたデバイスにプッシュする特定の iOS/iPadOS の更新プログラムを選択できます (最新の更新プログラムを除く)。 これらのデバイスでは、ソフトウェア更新プログラムの可視性を一定の日数だけ遅らせるようにデバイス構成ポリシーを設定する必要があります。 この機能を確認するには、MEM > **[デバイス]**  >  **[iOS]**  >  **[Update policies for iOS/iPadOS]\(iOS または iPadOS のポリシーを更新する\)**  >  **[プロファイルの作成]** に移動します。



<!-- vvvvvvvvvvvvvvvvvvvvvv -->
### <a name="device-security"></a>デバイス セキュリティ

#### <a name="improved-intune-reporting-experience---3791418-----"></a>Intune レポート エクスペリエンスの向上<!-- 3791418   -->
Intune では、新しいレポートの種類、より優れたレポート編成、より対象を絞ったビュー、より優れたレポート機能、より一貫性のあるタイムリーなデータを含め、レポート エクスペリエンスが向上しています。 レポート エクスペリエンスは、パブリック プレビューから GA (一般公開) に移行します。 また、GA リリースでは、[Microsoft Endpoint Manager 管理センター](https://go.microsoft.com/fwlink/?linkid=2109431)のタイルで、ローカライズ サポート、バグ修正、設計の改善、デバイス コンプライアンス データの集計を行うことができます。

新しいレポートの種類では、次の情報に重点が置かれています。

- **運用** - 正常性への悪影響に焦点を置いた最新のレコードが表示されます。 
- **組織** - 全体的な状態の概要が表示されます。
- **履歴** - 一定期間におけるパターンと傾向が表示されます。
- **スペシャリスト** - 生データを使用して独自のカスタム レポートを作成できます。

新しいレポートの最初のセットでは、デバイスのコンプライアンスに重点が置かれています。 詳細については、[ブログ - Microsoft Intune レポート フレームワーク](https://techcommunity.microsoft.com/t5/Intune-Customer-Success/New-Reporting-Framework-Coming-to-Intune/ba-p/1009553)および[Intune レポート](reports.md)に関するページを参照してください。

#### <a name="consolidated-the-location-of-security-baselines-in-the-ui---6177074-----"></a>UI でセキュリティ ベースラインの場所を統合<!-- 6177074   -->
いくつかの UI の場所から*セキュリティ ベースライン*を削除し、パスを統合して、Microsoft Endpoint Manager admin center で[セキュリティ ベースライン](../protect/security-baselines.md)を見つけられるようにしました。 セキュリティ ベースラインを見つける場合、今後は次のパスを使用します。**エンドポイント セキュリティ** > **セキュリティ ベースライン**。

#### <a name="expanded-support-for-imported-pkcs-certificates---6044197----"></a>インポートした PKCS 証明書のサポート拡張<!-- 6044197  -->
[インポートされた PKCS 証明書](../protect/certificates-imported-pfx-configure.md#supported-platforms)を使用するためのサポートが拡張され、"*Android Enterprise フル マネージド デバイス*" がサポートされるようになりました。 一般的に、PFX 証明書のインポートは S/MIME 暗号化シナリオで利用されます。ここでは、電子メールを復号化できるよう、ユーザーのすべてのデバイスでユーザーの暗号化証明書が必須となります。

次のプラットフォームでは、PFX 証明書のインポートがサポートされています。

- Android - デバイス管理者
- Android Enterprise - フル マネージド
- Android Enterprise - 仕事用プロファイル
- iOS
- Mac
- Windows 10

#### <a name="view-the-endpoint-security-configuration-for-devices---6206460----"></a>デバイスのエンドポイント セキュリティ構成を表示する<!-- 6206460  -->
[特定のデバイスに適用されるエンドポイント セキュリティ構成](../protect/security-baselines-monitor.md#view-endpoint-security-configurations-per-device)を表示する目的で、Microsoft Endpoint Manager admin center のオプションの名前を更新しました。 このオプションの名前は**エンドポイント セキュリティ構成**に変更されました。該当するセキュリティ ベースラインと、セキュリティ ベースラインの外部で作成された追加ポリシーを示すためです。 このオプションの以前の名前は "*セキュリティ ベースライン*" でした。

<!-- vvvvvvvvvvvvvvvvvvvvvv -->
### <a name="role-based-access-control"></a>ロール ベースのアクセス制御

#### <a name="intune-roles-user-interface-changes-coming--5801612-----"></a>Intune ロールのユーザー インターフェイスが変更予定<!--5801612   -->
[Microsoft Endpoint Manager admin center](https://go.microsoft.com/fwlink/?linkid=2109431) >  **[テナント管理]**  >  **[ロール]** のユーザー インターフェイスが改善され、ユーザーにとって使いやすく、直観的なデザインになりました。 このエクスペリエンスでは、現在使用しているのと同じ設定と詳細が提供されます。ただし、新しいエクスペリエンスでは、ウィザードに似たプロセスが採用されています。

<!-- ########################## -->
## <a name="week-of-february-17-2020"></a>2020 年 2 月 17 日の週

<!-- vvvvvvvvvvvvvvvvvvvvvv -->
### <a name="app-management"></a>アプリ管理

#### <a name="microsofts-new-office-app---5859926---"></a>Microsoft の新しい Office アプリ<!-- 5859926 -->
Microsoft の新しい Office アプリが一般公開され、ダウンロードして使用できるようになりました。 Office アプリは統合環境であり、ユーザーは 1 つのアプリ内で Word、Excel、PowerPoint をまたいで作業できます。 アクセスするデータが保護されるよう、アプリをアプリ保護ポリシーの対象にできます。

詳細については、「[Office モバイル プレビュー アプリで Intune アプリ保護ポリシーを有効にする方法](https://techcommunity.microsoft.com/t5/intune-customer-success/support-tip-how-to-enable-intune-app-protection-policies-with/ba-p/1045493)」を参照してください。

<!-- ########################## -->

## <a name="week-of-february-10-2020"></a>2020 年 2 月 10 日の週

### <a name="windows-7-ends-extended-support--3042987---"></a>Windows 7 の延長サポートの終了<!--3042987 -->
Windows 7 の延長サポートは、2020 年 1 月 14 日に終了しました。 同時に、Intune では Windows 7 を稼働しているデバイスのサポートが非推奨になりました。 PC の保護に役立つ技術的なサポートや自動更新が利用できなくなりました。 Windows 10 にアップグレードする必要があります。 詳細については、[変更の計画に関するブログ記事](https://aka.ms/Windows7_Intune)を参照してください。

<!-- vvvvvvvvvvvvvvvvvvvvvv -->
### <a name="app-management"></a>アプリ管理

#### <a name="microsoft-edge-version-77-and-later-on-windows-10-devices---5843584---"></a>Windows 10 デバイスの Microsoft Edge バージョン 77 以降<!-- 5843584 -->
Intune で、Windows 10 デバイスでの Microsoft Edge バージョン 77 以降のアンインストールがサポートされるようになりました。 詳細については、「[Microsoft Edge for Windows 10 を Microsoft Intune に追加する](../apps/apps-windows-edge.md)」を参照してください。

#### <a name="screen-removed-from-company-portal-android-work-profile-enrollment--6103987---"></a>ポータル サイトの Android 仕事用プロファイルの登録から削除される画面<!--6103987 -->
ユーザー エクスペリエンスを効率化するために、ポータル サイトの Android 仕事用プロファイルの登録フローから **[次の手順]** 画面が削除されました。 更新後の Android 仕事用プロファイルの登録フローを確認するには、[Android 仕事用プロファイルへの登録](../user-help/enroll-device-android-work-profile.md)に関する記事を参照してください。  

#### <a name="company-portal-app-improved-performance---6178652---"></a>ポータル サイト アプリのパフォーマンスの向上<!-- 6178652 -->
ポータル サイト アプリが更新され、Surface Pro X などの ARM64 プロセッサを使用したデバイス向けのパフォーマンスの向上がサポートされました。これまでは、ポータル サイトはエミュレートされた ARM32 モードで動作していました。 現在、バージョン 10.4.7080.0 以降では、ポータル サイト アプリは ARM64 用にネイティブ コンパイルされています。 ポータル サイト アプリの詳細については、「[Microsoft Intune ポータル サイト アプリを構成する方法](../apps/company-portal-app.md)」をご覧ください。

<!-- ########################## -->
## <a name="week-of-january-27-2020"></a>2020 年 1 月 27 日の週

<!-- vvvvvvvvvvvvvvvvvvvvvv -->
### <a name="app-management"></a>アプリ管理

#### <a name="intune-support-for-additional-microsoft-edge-version-77-deployment-channel-for-macos---5983950----"></a>macOS 用の追加の Microsoft Edge バージョン 77 展開チャネルの Intune サポート<!-- 5983950  -->
Microsoft Intune で、macOS 用 Microsoft Edge アプリの追加の **[安定]** 展開チャネルがサポートされるようになりました。 **[安定]** チャネルは、Microsoft Edge をエンタープライズ環境で幅広く展開する場合に推奨されるチャネルです。 これは 6 週間ごとに更新され、各リリースには **[Beta]** チャネルからの機能強化が組み込まれています。 **[安定]** および **[Beta]** チャネルに加えて、Intune では **[Dev]** チャネルもサポートされています。 パブリック プレビューでは、macOS 用の Microsoft Edge バージョン 77 以降の [安定] および [Dev] チャネルが提供されます。 ブラウザーの自動更新は、既定で有効になっています。 詳細については、[Microsoft Intune を使用した macOS デバイスへの Microsoft Edge の追加](../apps/apps-edge-macos.md)に関する記事をご覧ください。

#### <a name="retirement-of-intune-managed-browser--5728447---"></a>Intune Managed Browser の提供終了<!--5728447 -->
Intune Managed Browser の提供は終了します。 保護された Intune ブラウザー エクスペリエンスには Microsoft Edge を使用してください。 

<!-- ########################## -->
## <a name="week-of-january-20-2020-2001-service-release"></a>2020 年 1 月 20 日の週 (2001 サービス リリース)

<!-- vvvvvvvvvvvvvvvvvvvvvv -->
### <a name="app-management"></a>アプリ管理

#### <a name="user-experience-change-when-adding-apps-to-intune---4705829-----"></a>Intune にアプリを追加するときのユーザー エクスペリエンスの変更<!-- 4705829   -->
Intune を使用してにアプリを追加するときに、新しいユーザー エクスペリエンスを確認できます。 このエクスペリエンスでは、以前使用していたのと同じ設定と詳細が提供されます。ただし、新しいエクスペリエンスでは、Intune にアプリを追加する前に、ウィザードに似たプロセスが実行されます。 この新しいエクスペリエンスでは、アプリを追加する前にレビュー ページも提供されます。 [Microsoft Endpoint Manager 管理センター](https://go.microsoft.com/fwlink/?linkid=2109431)から、 **[アプリ]**  >  **[すべてのアプリ]**  >  **[追加]** の順に選択します。 詳しくは、「[Microsoft Intune にアプリを追加する](../apps/apps-add.md)」をご覧ください。

#### <a name="require-win32-apps-to-restart----5622282-----"></a>Win32 アプリの再起動を要求する <!-- 5622282   -->
正常にインストールされた後、Win32 アプリの再起動を要求することができます。 また、再起動が発生するまでの時間 (猶予期間) を選択することもできます。

#### <a name="user-experience-change-when-configuring-apps-in-intune---4207990-----"></a>Intune でアプリを構成するときのユーザー エクスペリエンスの変更<!-- 4207990   -->
Intune でアプリ構成ポリシーを作成するときに、新しいユーザー エクスペリエンスを確認できます。 このエクスペリエンスでは、以前使用していたのと同じ設定と詳細が提供されます。ただし、新しいエクスペリエンスでは、Intune にポリシーを追加する前に、ウィザードに似たプロセスが実行されます。 [Microsoft Endpoint Manager admin center](https://go.microsoft.com/fwlink/?linkid=2109431) から、 **[アプリ]**  >  **[アプリ構成ポリシー]**  >  **[追加]** の順に選択します。 詳細については、「[Microsoft Intune 用アプリ構成ポリシー](../apps/app-configuration-policies-overview.md)」を参照してください。 

#### <a name="intune-support-for-additional-microsoft-edge-for-windows-10-deployment-channel---5861774---"></a>追加の Windows 10 用 Microsoft Edge 展開チャネルの Intune サポート<!-- 5861774 -->
Microsoft Intune で、Windows 10 用 Microsoft Edge (バージョン 77 以降) アプリの追加の **[安定]** 展開チャネルがサポートされるようになりました。 **[安定]** チャネルは、Windows 10 用 Microsoft Edge をエンタープライズ環境で幅広く展開する場合に推奨されるチャネルです。 このチャネルは 6 週間ごとに更新され、各リリースには **[Beta]** チャネルからの機能強化が組み込まれています。 **[安定]** および **[Beta]** チャネルに加えて、Intune では **[Dev]** チャネルもサポートされています。 詳細については、[Windows 10 用 Microsoft Edge - アプリ設定の構成](../apps/apps-windows-edge.md#configure-app-settings)に関する記事をご覧ください。

<!-- vvvvvvvvvvvvvvvvvvvvvv -->
### <a name="device-configuration"></a>デバイスの構成

#### <a name="improved-user-interface-experience-when-configuring-exchange-activesync-on-premises-connector-ui---5695492-----"></a>Exchange ActiveSync のオンプレミス コネクタ UI を構成するときのユーザー インターフェイス エクスペリエンスの向上<!-- 5695492   -->
[Exchange ActiveSync のオンプレミス コネクタを構成する](../protect/exchange-connector-install.md)ためのエクスペリエンスが更新されました。 更新されたエクスペリエンスでは、1 つのペインを使用して、オンプレミス コネクタの詳細を構成、編集、および要約することができます。

#### <a name="add-automatic-proxy-settings-to-wi-fi-profiles-for-android-enterprise-work-profiles---4490822-----"></a>Android エンタープライズ仕事用プロファイルの Wi-Fi プロファイルに自動プロキシ設定を追加する<!-- 4490822   -->
Android Enterprise 仕事用プロファイル デバイスで、Wi-Fi プロファイルを作成できます。 Wi-Fi Enterprise の種類を選択した場合は、Wi-Fi ネットワークで使用される拡張認証プロトコル (EAP) の種類を入力することもできます。

今回、Enterprise の種類を選択したときに、プロキシ サーバーの URL (例: `proxy.contoso.com`) などの自動プロキシ設定も入力できるようになりました。

現在構成できる Wi-Fi の設定については、[Microsoft Intune で Android エンタープライズおよび Android キオスクを稼働しているデバイス用の Wi-Fi 設定を追加する方法](../configuration/wi-fi-settings-android-enterprise.md#work-profile-only)に関する記事を参照してください。

適用対象:
- Android Enterprise 仕事用プロファイル

<!-- vvvvvvvvvvvvvvvvvvvvvv -->
### <a name="device-enrollment"></a>デバイスの登録

#### <a name="block-android-enrollments-by-device-manufacturer--5197392----"></a>デバイスの製造元で Android の登録をブロックする<!--5197392  -->
デバイスの製造元に基づいてデバイスの登録をブロックすることができます。 この機能は、Android デバイス管理者と Android Enterprise 仕事用プロファイル デバイスに適用されます。 登録制限を確認するには、[Microsoft Endpoint Manager admin center](https://go.microsoft.com/fwlink/?linkid=2109431) >  **[デバイス]**  >  **[登録制限]** の順に移動します。

#### <a name="improvements-to-the-iosipados-create-enrollment-type-profile-ui---6055005---"></a>iOS、iPadOS の [登録の種類のプロファイルの作成] UI の機能強化<!-- 6055005 -->
iOS、iPadOS のユーザー登録に関して、 **[登録の種類のプロファイルの作成]** の **[設定]** ページが合理化され、 **[登録の種類]** の選択プロセスが強化されました (機能は同じです)。 新しい UI を確認するには、[Microsoft Endpoint Manager admin center](https://go.microsoft.com/fwlink/?linkid=2109431) >  **[デバイス]**  >  **[iOS]**  >  **[iOS の登録]**  >  **[登録の種類]**  >  **[プロファイルの作成]**  >  **[設定]** の順に移動します。 詳細については、「[Intune でユーザー登録プロファイルを作成する](../enrollment/ios-user-enrollment.md#create-a-user-enrollment-profile-in-intune)」を参照してください。

<!-- vvvvvvvvvvvvvvvvvvvvvv -->
### <a name="device-management"></a>デバイス管理

#### <a name="new-information-in-device-details---4471759-5604099----"></a>デバイスの詳細の新しい情報<!-- 4471759 5604099  -->
デバイスの **[概要]** ページに、次の情報が追加されました。
- メモリ容量 (デバイスの物理メモリの容量)
- ストレージ容量 (デバイスの物理ストレージの容量) 
- CPU アーキテクチャ

#### <a name="ios-bypass-activation-lock-remote-action-renamed-to-disable-activation-lock---5904591----"></a>iOS の [アクティベーション ロックのバイパス] リモート操作の [アクティベーション ロックの無効化] への名前変更 <!--5904591  -->
リモート操作 **[アクティベーション ロックのバイパス]** の名前が、 **[アクティベーション ロックの無効化]** に変更されています。 詳細については、[Intuneで iOS のアクティベーション ロックを無効にする方法](../remote-actions/device-activation-lock-disable.md)に関する記事をご覧ください。

#### <a name="windows-10-feature-update-deployment-support-for-autopilot-devices---5948137-----"></a>Autopilot デバイスに対する Windows 10 機能更新プログラムの展開のサポート<!-- 5948137   -->
Intune では、[Windows 10 機能更新プログラムの展開](../protect/windows-update-for-business-configure.md#windows-10-feature-updates)を使用して Autopilot に登録されたデバイスを対象にすることができるようになりました。

Windows 10 の機能更新ポリシーは、Autopilot の Out-of-Box Experience (OOBE) 中には適用できず、デバイスのプロビジョニングの完了後 (通常は 1 日)、最初の Windows Update のスキャン時にのみ適用されます。

<!-- vvvvvvvvvvvvvvvvvvvvvv -->
### <a name="monitor-and-troubleshoot"></a>監視とトラブルシューティング

#### <a name="windows-autopilot-deployment-reports-preview----3856172-----"></a>Windows Autopilot の展開レポート (プレビュー) <!-- 3856172   -->
新しいレポートでは、Windows Autopilot によって展開された各デバイスについて詳しく報告されます。 詳しくは、[Autopilot の展開レポート](../enrollment/enrollment-autopilot.md#autopilot-deployments-report)に関するページをご覧ください。

<!-- vvvvvvvvvvvvvvvvvvvvvv -->
### <a name="role-based-access-control"></a>ロール ベースのアクセス制御

#### <a name="new-intune-built-in-role-endpoint-security-manager--4253397-----"></a>新しい Intune 組み込みロールであるエンドポイント セキュリティ マネージャー<!--4253397   -->
新しい Intune 組み込みロール: エンドポイント セキュリティ マネージャーを利用できます。 この新しいロールにより、管理者には、Intune の Endpoint Manager ノードへのフル アクセス権、およびその他の領域への読み取り専用アクセス権が付与されます。 このロールは、Azure AD の "セキュリティ管理者" ロールを拡張したものです。 現在、ロールとしてグローバル管理者のみを使用している場合、変更は必要ありません。 複数のロールを使用し、エンドポイント セキュリティ マネージャーで提供される粒度が必要な場合は、使用可能であればこのロールを割り当ててください。 組み込みロールの詳細については、[ロールベースのアクセス制御](role-based-access-control.md)に関するページを参照してください。

<!-- ########################## -->
## <a name="week-of-january-6-2020"></a>2020 年 1 月 6 日の週

<!-- vvvvvvvvvvvvvvvvvvvvvv -->
### <a name="app-management"></a>アプリ管理

#### <a name="smime-support-for-microsoft-outlook-for-ios---2669398---"></a>Microsoft Outlook for iOS での S/MIME のサポート<!-- 2669398 -->
Intune では、iOS デバイス上の Outlook for iOS で使用できる S/MIME 署名証明書と暗号化証明書の配信がサポートされています。 詳細については、「[iOS 向けおよび Android 向け Outlook の秘密度ラベルと保護](https://aka.ms/omsmime)」を参照してください。

#### <a name="cache-win32-app-content-using-microsoft-connected-cache-server---6030314---"></a>Microsoft 接続キャッシュ サーバーを使用して Win32 アプリのコンテンツをキャッシュする<!-- 6030314 -->
Configuration Manager の配布ポイントに Microsoft 接続キャッシュ サーバーをインストールして、Intune Win32 アプリのコンテンツをキャッシュできます。 詳細については、「Configuration Manager における Microsoft 接続済みキャッシュ」の「[Intune Win32 アプリのサポート](https://docs.microsoft.com/configmgr/core/plan-design/hierarchy/microsoft-connected-cache#bkmk_intune)」を参照してください。

<!-- vvvvvvvvvvvvvvvvvvvvvv -->
### <a name="role-based-access-control"></a>ロール ベースのアクセス制御

#### <a name="windows-10-administrative-templates-admx-profiles-now-support-scope-tags---5137390---"></a>Windows 10 管理用テンプレート (ADMX) プロファイルでのスコープ タグのサポートの開始 <!--5137390 -->
スコープ タグを管理用テンプレート プロファイル (ADMX) に割り当てることができるようになりました。 これを行うには、 **[Intune]**  >  **[デバイス]**  >  **[構成プロファイル]** に移動し、一覧から管理用テンプレート プロファイルを選択して、 **[プロパティ]**  >  **[スコープ タグ]** を選択します。 スコープ タグの詳細については、「[スコープ タグを他のオブジェクトに割り当てる](../fundamentals/scope-tags.md#assign-scope-tags-to-other-objects)」をご覧ください。

<!-- ########################## -->
## <a name="week-of-december-30-2019"></a>2019 年 12 月 30 日の週

<!-- vvvvvvvvvvvvvvvvvvvvvv -->
### <a name="app-management"></a>アプリ管理

#### <a name="retrieve-personal-recovery-key-from-mem-encrypted-macos-devices---4851745---"></a>MEM 暗号化 macOS デバイスから個人用回復キーを取得する<!-- 4851745 -->
エンド ユーザーは、iOS ポータル サイト アプリを使用して個人用回復キー (FileVault キー) を取得できます。 個人用回復キーを持つデバイスは、Intune に登録され、Intune により FileVault を使用して暗号化されている必要があります。 iOS ポータル サイト アプリを使うと、エンド ユーザーは、 **[回復キーを取得する]** をクリックして、暗号化された macOS デバイス上の個人用回復キーを取得できます。 また、 **[デバイス]**  > "*暗号化されて登録された macOS デバイス*" >  **[回復キーの取得]** を選択することで、Intune から回復キーを取得することもできます。 FileVault の詳細については、「[macOS 用 FileVault 暗号化](../protect/encrypt-devices.md#filevault-encryption-for-macos)」を参照してください。

#### <a name="ios-and-ipados-user-licensed-vpp-apps---5619268---"></a>iOS と iPadOS のユーザー ライセンス VPP アプリ<!-- 5619268 -->
ユーザーが登録した iOS および iPadOS デバイスの場合、エンド ユーザーには、利用可能として展開された、新しく作成されたデバイス ライセンス VPP アプリケーションが表示されなくなります。 ただし、エンド ユーザーには、Intune ポータル サイト内のすべてのユーザー ライセンス VPP アプリが引き続き表示されます。 VPP アプリの詳細については、「[Apple Volume Purchase Program で購入した iOS アプリと macOS アプリを Microsoft Intune で管理する方法](../apps/vpp-apps-ios.md)」をご覧ください。

<!-- ########################## -->
## <a name="week-of-december-23-2019"></a>2019 年 12 月 23 日の週

<!-- vvvvvvvvvvvvvvvvvvvvvv -->
### <a name="app-management"></a>アプリ管理

#### <a name="notice---windows-10-1703-rs2-will-be-moving-out-of-support----5026679---"></a>注意 - Windows 10 1703 (RS2) がサポート対象外になる <!-- 5026679 -->
2018 年 10 月 9 日以降、Windows 10 1703 (RS2) は、Home、Pro、および Pro for Workstations の各エディションに対する Microsoft プラットフォーム サポートの対象外になりました。 Windows 10 Enterprise および Education エディションについては、Windows 10 1703 (RS2) は 2019 年 10 月 8 日にプラットフォーム サポートの対象外になりました。 2019 年 12 月 26 日以降、Windows ポータル サイト アプリケーションの最小バージョンは Windows 10 1709 (RS3) に更新されます。 1709 より前のバージョンが実行されているコンピューターでは、アプリケーションの更新されたバージョンを Microsoft Store から受け取ることができなくなります。 古いバージョンの Windows 10 を管理しているお客様には、メッセージ センター経由でこの変更を既にお知らせしてあります。 詳細については、「[Windows ライフサイクルのファクト シート](https://support.microsoft.com/help/13853/windows-lifecycle-fact-sheet)」を参照してください。

<!-- ########################## -->

## <a name="week-of-december-16-2019"></a>2019 年 12 月 16 日の週

### <a name="device-configuration"></a>デバイスの構成

#### <a name="updates-to-administrative-templates-for-windows-10-devices----5941568---"></a>Windows 10 デバイス用の管理用テンプレートの更新 <!-- 5941568 -->

Microsoft Intune の ADMX テンプレートを使用して、Microsoft Edge、Office、Windows の設定を制御および管理できます。 Intune の管理用テンプレートでは、次のポリシー設定が更新されました。

- Microsoft Edge バージョン 78 および 79 のサポートが追加されました。
- [Office 365 ProPlus、Office 2019、Office 2016 のための管理用テンプレート ファイル (ADMX/ADML) および Office カスタマイズ ツール](https://www.microsoft.com/download/details.aspx?id=49030)には、2019 年 11 月 11 日の ADMX ファイルが含まれています。

Intune での ADMX テンプレートの詳細については、「[Windows 10 テンプレートを使用し、Microsoft Intune でグループ ポリシー設定を構成する](../configuration/administrative-templates-windows.md)」を参照してください。

適用対象:

- Windows 10 以降

## <a name="week-of-december-9-2019-1912-service-release"></a>2019 年 12 月 9 日の週 (1912 サービス リリース)

<!-- vvvvvvvvvvvvvvvvvvvvvv -->
### <a name="app-management"></a>アプリ管理

#### <a name="migrating-to-microsoft-edge-for-managed-browsing-scenarios---5173762---"></a>マネージド ブラウジング シナリオのための Microsoft Edge への移行<!-- 5173762 -->
Intune Managed Browser の提供終了が近づいているため、アプリ保護ポリシーを変更して、ユーザーを Edge に移動するために必要な手順を簡略化しました。 アプリ保護ポリシー設定 **[その他のアプリでの Web コンテンツの転送を制限する]** のオプションを、次のいずれかになるように更新しました。

- すべてのアプリ
- Intune Managed Browser
- Microsoft Edge
- アンマネージド ブラウザー 

**[Microsoft Edge]** を選択すると、マネージド ブラウジング シナリオには Microsoft Edge が必要であることを通知する、条件付きアクセス メッセージングがエンド ユーザーに表示されます。 自身の AAD アカウントを使用して Microsoft Edge をダウンロードし、サインインするように求められます (まだ行っていない場合)。  これは、アプリの構成設定 `com.microsoft.intune.useEdge` が **True** に設定されている MAM 対応アプリをターゲットにすることと同じです。 **ポリシーで管理されているブラウザー**設定を使用していた既存のアプリ保護ポリシーでは、 **[Intune Managed Browser]** が選択されるようになります。動作が変更されることはありません。 これは、**useEdge** アプリの構成設定を **True** に設定している場合は、ユーザーに Microsoft Edge を使用するようにメッセージングが表示されることを意味します。 アプリ保護ポリシーを更新するためにマネージド ブラウジング シナリオを利用しているすべてのお客様に、 **[その他のアプリでの Web コンテンツの転送を制限する]** を使用して、ユーザーがどのアプリからリンクを起動しているかに関係なく、Microsoft Edge に移行するための適切なガイダンスがユーザーに表示されるようにすることをお勧めします。 

#### <a name="configure-app-notification-content-for-organization-accounts---2576686----"></a>組織アカウント向けのアプリ通知の内容を構成する<!-- 2576686  -->
Android および iOS デバイスで Intune アプリ保護ポリシー (APP) を使用すると、組織アカウントに対するアプリ通知の内容を制御できます。 オプション ([許可]、[組織データをブロック]、[ブロック済み]) を選択して、組織アカウントに対する通知の内容が選択したアプリでどのように表示されるかを指定できます。 この機能は、アプリケーションからのサポートを必要とし、APP 対応のすべてのアプリケーションで使用できるとは限りません。 Outlook for iOS バージョン 4.15.0 (以降) および Outlook for Android 4.83.0 (以降) では、この設定がサポートされます。 コンソールでは設定を使用できますが、機能が有効になるのは 2019 年 12 月 16 日以降です。 アプリの詳細については、「[アプリ保護ポリシーとは](../apps/app-protection-policy.md)」を参照してください。

#### <a name="microsoft-app-icons-update--4677605----"></a>Microsoft アプリ アイコンの更新<!--4677605  -->
アプリ保護ポリシーとアプリ構成ポリシーのアプリ ターゲット設定ウィンドウで Microsoft アプリに対して使用されるアイコンが更新されました。

#### <a name="require-use-of-approved-keyboards-on-android--4761794----"></a>Android で承認済みキーボードの使用を要求する<!--4761794  -->
アプリ保護ポリシーの一部として、[**承認済みキーボード**](../apps/app-protection-policy-settings-android.md#data-protection)の設定を指定し、マネージド Android アプリで使用できる Android キーボードを管理できます。 ユーザーがマネージド アプリを開いたとき、そのアプリに対する承認済みキーボードが使われていない場合は、デバイスに既にインストールされている承認済みキーボードのいずれかに切り替えるように求められます。 必要に応じて、承認済みキーボードを Google Play ストアからダウンロードするためのリンクが表示されます。このリンクを使用して、インストールとセットアップを行うことができます。 アクティブなキーボードが承認済みキーボードでない場合、ユーザーがマネージド アプリで編集できるのはテキスト フィールドだけです。

<!-- vvvvvvvvvvvvvvvvvvvvvv -->
### <a name="device-configuration"></a>デバイスの構成

#### <a name="updated-single-sign-on-experience-for-apps-and-websites-on-your-ios-ipados-and-macos-devices---4999578----"></a>iOS、iPadOS、macOS デバイスでのアプリと Web サイトに対するシングル サインオン エクスペリエンスが更新された<!-- 4999578  -->
Intune では、iOS、iPadOS、macOS デバイス向けのシングル サインオン (SSO) の設定が追加されました。 組織または ID プロバイダーによって作成されたリダイレクト SSO アプリ拡張機能を構成できるようになりました。 これらの設定は、OAuth や SAML2 などの最新の認証方法を使用するアプリと Web サイトに対してシームレスなシングル サインオン エクスペリエンスを構成するために使用します。 

これらの新しい設定では、SSO アプリ拡張機能および Apple の組み込み Kerberos 拡張機能に対する以前の設定が拡張されます ( **[デバイス]**  >  **[デバイスの構成]**  >  **[プロファイル]**  >  **[プロファイルの作成]**  >  **[iOS/iPadOS]** または **[macOS]** (プラットフォームの種類) > **[デバイス機能]** (プロファイルの種類))。 

構成できるすべての SSO アプリ拡張機能の設定については、[iOS での SSO](../configuration/ios-device-features-settings.md#single-sign-on-app-extension) および [macOS での SSO](../configuration/macos-device-features-settings.md#single-sign-on-app-extension) に関する記事を参照してください。

適用対象:

- iOS/iPadOS
- macOS

#### <a name="we-have-updated-two-device-restriction-settings-for-ios-and-ipados-devices-to-correct-their-behavior---5701352------"></a>動作を修正するため、iOS および iPadOS デバイスに対する 2 つのデバイス制限設定を更新した<!-- 5701352    -->
iOS デバイスの場合、 **[無線による PKI の更新を許可する]** および **[USB 制限モードをブロックする]** が有効なデバイス制限プロファイルを作成できま ( **[デバイス]**  >  **[デバイスの構成]**  >  **[プロファイル]**  >  **[プロファイルの作成]**  >  **[iOS/iPadOS]** (プラットフォーム) > **[デバイスの制限]** (プロファイルの種類))。 このリリースより前では、次の設定の UI 設定と説明は正しくありませんでしたが、現在は修正されています。 このリリース以降では、設定の動作は次のようになります。

**[無線による PKI の更新をブロックする]** : **[Block]\(ブロックする\)** に設定すると、デバイスがコンピューターに接続されていない場合、ユーザーはソフトウェア更新プログラムを受信できません。 **[未構成]** (既定値): コンピューターに接続されていなくても、デバイスはソフトウェア更新プログラムを受信できます。
- 以前のこの設定では、次のように構成できます: **[許可]** を選択すると、ユーザーはデバイスをコンピューターに接続せずにソフトウェア更新プログラムを受信できるようになります。
**[デバイスのロック中に USB アクセサリの使用を許可する]** : **[許可]** を選択すると、USB アクセサリは 1 時間以上ロックされているデバイスとデータを交換できます。 **[未構成]** (既定値) では、デバイスでの USB 制限モードは更新されず、USB アクセサリは、1 時間以上ロックされている場合、デバイスからのデータの転送をブロックされます。
- 以前のこの設定では、次のように構成できます: **[ブロック]** を選択すると、監視対象のデバイスで USB 制限モードが無効になります。

構成できる設定の詳細については、「[Intune を使用した機能を許可または制限するための iOS および iPadOS デバイスの設定](../configuration/device-restrictions-ios.md)」を参照してください。

この機能は、以下に適用されます。

- iOS/iPadOS

#### <a name="wired-network-device-configuration-profiles-for-macos-devices---3508686----"></a>macOS デバイス用の有線ネットワーク デバイス構成プロファイル<!-- 3508686  -->
   > [!NOTE]
   > この機能は遅れていますが、間もなくリリースされる予定です。

#### <a name="block-users-from-configuring-certificate-credentials-in-the-managed-keystore-on-android-enterprise-device-owner-devices---3311998---"></a>Android Enterprise デバイス所有者デバイスでマネージド キーストア内の証明書資格情報をユーザーが構成できないようにする<!-- 3311998 -->
Android Enterprise デバイス所有者デバイスでは、マネージド キーストア内の証明書資格情報をユーザーが構成できないようにする新しい設定を構成できます ( **[デバイスの構成]**  >  **[プロファイル]**  >  **[プロファイルの作成]**  >  **[Android Enterprise]** (プラットフォーム) > **[デバイスの所有者のみ] > [デバイスの制限]** (プロファイルの種類) > **[ユーザーとアカウント]** )。

<!-- vvvvvvvvvvvvvvvvvvvvvv -->
### <a name="device-management"></a>デバイス管理

#### <a name="protected-wipe-action-now-available--51150000---"></a>保護されたワイプ アクションを使用できるようになった<!--51150000 -->
デバイスのワイプ アクションを使用して、デバイスの保護されたワイプを実行できるようになりました。 保護されたワイプは標準のワイプと同じですが、デバイスの電源をオフにしても回避できない点が異なります。 保護されたワイプは、成功するまでデバイスをリセットしようとします。 一部の構成では、このアクションによってデバイスを再起動できなくなる場合があります。 詳細については、[デバイスのインベントリからの削除またはワイプ](../remote-actions/devices-wipe.md)に関する記事を参照してください。

#### <a name="device-ethernet-mac-address-added-to-devices-overview-page--5562275---"></a>デバイスの [概要] ページにデバイスのイーサネット MAC アドレスが追加された<!--5562275 -->
デバイスの詳細ページで、デバイスのイーサネット MAC アドレスを確認できるようになりました ( **[デバイス]**  >  **[すべてのデバイス]** > デバイスを選択 > **[概要]** )。

<!-- vvvvvvvvvvvvvvvvvvvvvv -->
### <a name="device-security"></a>デバイス セキュリティ

#### <a name="improved-experience-on-a-shared-device-when-device-based-conditional-access-policies-are-enabled---1734096----"></a>デバイス ベースの条件付きアクセス ポリシーが有効になっているときの、共有デバイスでのエクスペリエンスが向上した<!-- 1734096  -->
ポリシーの適用時にユーザーの最新のコンプライアンス評価をチェックすることで、デバイス ベースの条件付きアクセス ポリシーの対象となっている複数のユーザーが使用する共有デバイスでのエクスペリエンスが向上しました。 詳細については、以下の概要記事を参照してください。
- [Azure での条件付きアクセスの概要](https://docs.microsoft.com/azure/active-directory/conditional-access/overview)
- [Intune でのデバイス コンプライアンスの概要](../protect/device-compliance-get-started.md)

#### <a name="use-pkcs-certificate-profiles-to-provision-devices-with-certificates---2317124-2317130-2317139-2340517-2340528-2340529----"></a>PKCS 証明書プロファイルを使用し、証明書でデバイスをプロビジョニングする<!-- 2317124, 2317130, 2317139, 2340517, 2340528, 2340529  -->
Wi-Fi や VPN のようなプロファイルに関連付けられている場合に、PKCS 証明書プロファイルを使用して、Android for Work、iOS/iPadOS、Windows を実行する*デバイス*に証明書を発行できるようになりました。 以前は、それら 3 つのプラットフォームではユーザー ベースの証明書のみがサポートされており、デバイス ベースのサポートは macOS に限定されていました。

> [!NOTE]
> PKCS 証明書プロファイルは、Wi-Fi プロファイルではサポートされていません。 代わりに、[EAP の種類](../configuration/wi-fi-settings-windows.md#enterprise-profile)を使用する場合は SCEP 証明書プロファイルを使用します。

デバイス ベースの証明書を使用するには、サポートされるプラットフォーム用の [PKCS 証明書プロファイルを作成する](../protect/certficates-pfx-configure.md#create-a-pkcs-certificate-profile)ときに、 **[設定]** を選択します。 **[証明書の種類]** の設定が表示されるようになり、そこでは [デバイス] または [ユーザー] のオプションがサポートされています。


<!-- vvvvvvvvvvvvvvvvvvvvvv -->
### <a name="monitor-and-troubleshoot"></a>監視とトラブルシューティング

#### <a name="centralized-audit-logs--5603185-5697164---"></a>一元化された監査ログ<!--5603185, 5697164 -->
新しい一元化された監査ログ エクスペリエンスでは、すべてのカテゴリの監査ログが 1 ページに収集されるようになりました。 ログをフィルター処理して、探しているデータを取得できます。 監査ログを表示するには、 **[テナント管理]**  >  **[監査ログ]** に移動します。 

#### <a name="scope-tag-information-included-in-audit-log-activity-details--5763534---"></a>監査ログ アクティビティの詳細に組み込まれたスコープ タグ情報<!--5763534 -->
監査ログ アクティビティの詳細に、スコープ タグ情報が含まれるようになりました (スコープ タグをサポートする Intune オブジェクトの場合)。 監査ログの詳細については、[監査ログを使用したイベントの追跡と監視](monitor-audit-logs.md)に関する記事を参照してください。

<!-- ########################## -->
## <a name="week-of-december-2-2019"></a>2019 年 12 月 2 日の週

#### <a name="new-microsoft-endpoint-configuration-manager-co-management-licensing--5027281--"></a>新しい Microsoft Endpoint Configuration Manager の共同管理ライセンス<!--5027281-->
ソフトウェア アシュアランスをお持ちの Configuration Manager のお客様は、Windows 10 PC 向けの Intune 共同管理を利用できるようになりました。共同管理のために追加の Intune ライセンスを購入する必要はありません。 Windows 10 を共同管理するために個別の Intune または EMS ライセンスをエンド ユーザーに割り当てる必要はなくなりました。
- Configuration Manager によって管理され、共同管理に登録されているデバイスは、Intune スタンドアロン MDM によって管理されている PC とほぼ同じ権限を持ちます。 ただし、これらをリセットすると、オートパイロットを使用して再プロビジョニングすることはできません。
- 他の方法を使用して Intune に登録された Windows 10 デバイスには、Intune のフル ライセンスが必要です。
- その他のプラットフォームのデバイスには、引き続き Intune のフル ライセンスが必要です。

詳細については、[ライセンス条項](https://www.microsoft.com/en-us/Licensing/product-licensing/products)を参照してください。

<!-- ########################## -->
## <a name="week-of-november-18-2019-1911-service-release"></a>2019 年 11 月 18 日の週 (1911 サービス リリース)

<!-- vvvvvvvvvvvvvvvvvvvvvv -->
### <a name="app-management"></a>アプリ管理

#### <a name="ui-update-when-selectively-wiping-app-data---4102028---"></a>アプリ データを選択的にワイプするときの UI の更新<!-- 4102028 -->
Intune でアプリ データを選択的にワイプするための UI が更新されました。 UI に対する次のような変更があります。
- ウィザード方式による簡単操作が 1 つのウィンドウ内に凝縮されました。
- 作成フローを更新し、割り当てを含めました。
- プロパティを表示するときに、新しいポリシーを作成する前に、プロパティを編集するときに、まとめページに全部設定されます。 また、プロパティを編集するとき、編集されるプロパティのカテゴリから項目の一覧のみがまとめに表示されます。

詳細については、「[Intune で管理されているアプリから会社のデータをワイプする方法](../apps/apps-selective-wipe.md)」を参照してください。

#### <a name="ios-and-ipados-third-party-keyboard-support---4922950---"></a>iOS と iPadOS のサード パーティ キーボードのサポート<!-- 4922950 -->
2019 年 3 月に、iOS アプリ保護ポリシー設定の "サードパーティのキーボード" のサポートが削除されたことが発表されました。 この機能は、iOS と iPadOS の両方のサポートと共に Intune に再び備わります。 この設定を有効にするには、新規または既存の iOS および iPadOS アプリ保護ポリシーの **[データ保護]** タブを開いて、 **[データ転送]** で **[サードパーティのキーボード]** 設定を見つけます。

このポリシー設定の動作は、以前の実装と若干異なります。 SDK バージョン 12.0.16 以降を使用するマルチ ID アプリでは、この設定が **[ブロック]** に構成されているアプリ保護ポリシーにより、エンド ユーザーは組織と個人の両方のアカウントでサード パーティのキーボードを選択できなくなります。 SDK バージョン 12.0.12 以前を使用しているアプリでは、引き続き[既知の問題: 個人用アカウントの iOS でサードパーティのキーボードがブロックされない](https://aka.ms/3rdparty_iOS_Intune)という問題に関するブログ投稿に記載された動作が発生します。

<!-- vvvvvvvvvvvvvvvvvvvvvv -->
### <a name="device-configuration"></a>デバイスの構成

#### <a name="target-macos-user-groups-to-require-jamf-management---4061739----"></a>Jamf による管理を必要とする macOS ユーザー グループをターゲットにする<!-- 4061739  --> 
[Jamf による macOS デバイスの管理](../protect/conditional-access-integrate-jamf.md)を利用する特定のユーザー グループをターゲットにすることができます。 このターゲット設定により、macOS デバイスのサブセットに Jamf コンプライアンス統合を適用しながら、その他のデバイスを Intune によって管理することができます。 Jamf 統合を既に使用している場合は、すべてのユーザーが既定で統合のターゲットとなります。

#### <a name="new-exchange-activesync-settings-when-creating-an-email-device-configuration-profile-on-ios-devices---4892824-----"></a>iOS デバイスでメール デバイス構成プロファイルを作成するときの新しい Exchange ActiveSync 設定<!-- 4892824   --> 
iOS および iPadOS デバイスにおいて、デバイス構成プロファイルでメール接続を構成できます ( **[デバイス構成]**  >  **[プロファイル]**  >  **[プロファイルの作成]**  >  **[iOS および iPadOS]** (プラットフォーム) > **[メール]** (プロファイルの種類))。 

次のような新しい Exchange ActiveSync 設定を使用できます。
- **[同期する Exchange データ]** :予定表、連絡先、アラーム、メモ、メールに対して同期する (または同期をブロックする) Exchange サービスを選択します。
- **[同期の設定の変更をユーザーに許可する]** :デバイスでこれらのサービスの同期設定を変更することをユーザーに許可 (またはブロック) します。  

これらの設定の詳細については、[Intune での iOS デバイスのメール プロファイル設定](../configuration/email-settings-ios.md)に関するページを参照してください。 

適用対象:

- iOS 13.0 以降
- iPadOS 13.0 以降

#### <a name="prevent-users-from-adding-personal-google-accounts-to-android-enterprise-fully-managed-and-dedicated-devices---5353228-----"></a>Android Enterprise のフル マネージド専用デバイスにユーザーが個人用 Google アカウントを追加できないようにする<!-- 5353228   -->
Android Enterprise のフル マネージド デバイスおよび専用デバイスには、ユーザーが個人用 Google アカウントを作成できないようにする新しい設定があります ( **[デバイスの構成]**  >  **[プロファイル]**  >  **[プロファイルの作成]**  >  **[Android Enterprise]** (プラットフォーム) > **[デバイスの所有者のみ] > [デバイスの制限]** (プロファイルの種類) > **[ユーザーとアカウント] 設定** >  **[個人用 Google アカウント]** )。

構成できる設定を確認するには、「[Intune を使用して機能を許可または制限するように Android エンタープライズ デバイスを設定する](../configuration/device-restrictions-android-for-work.md)」をご覧ください。

適用対象:

- Android エンタープライズのフル マネージド デバイス
- Android Enterprise 専用デバイス

#### <a name="server-side-logging-for-siri-commands-setting-is-removed-in-iosipados-device-restrictions-profile----5468501-----"></a>iOS および iPadOS デバイス制限プロファイルから Siri コマンド設定のサーバー側のログ記録が削除されます <!-- 5468501   -->
iOS および iPadOS デバイスでは、Microsoft Endpoint Manager 管理コンソールから **Siri コマンド**設定のサーバー側のログ記録が削除されます ( **[デバイスの構成]**  >  **[プロファイル]**  >  **[プロファイルの作成]**  >  **[iOS および iPadOS]** (プラットフォーム) > **[デバイスの制限]** (プロファイルの種類) > **[組み込みアプリ]** )。 

この設定は、デバイスには影響を与えません。 既存のプロファイルから設定を削除するには、プロファイルを開いて変更を加え、プロファイルを保存します。 プロファイルが更新され、デバイスから設定が削除されます。

構成できるすべての設定を確認するには、[Intune を使用した機能を許可または制限するための iOS および iPadOS デバイスの設定](../configuration/device-restrictions-ios.md)に関するページを参照してください。

適用対象:

- iOS/iPadOS

#### <a name="windows-10-feature-updates-public-preview---2384877---"></a>Windows 10 機能更新プログラム (パブリック プレビュー)<!-- 2384877 -->
[Windows 10 機能更新プログラム](../protect/windows-update-for-business-configure.md#windows-10-feature-updates)を Windows 10 デバイスに展開できるようになりました。 Windows 10 機能更新プログラムは、デバイスにインストールして維持する必要がある Windows 10 のバージョンを設定できる、新しいソフトウェア更新プログラムのポリシーです。 この新しいポリシーの種類は、既存の Windows 10 更新プログラムのリングと共に使用できます。

Windows 10 機能更新ポリシーを受け取ったデバイスでは、指定されたバージョンの Windows がインストールされ、そのポリシーが編集または削除されるまでそのバージョンにとどまります。 より新しいバージョンの Windows を稼働しているデバイスは、その現在のバージョンにとどまります。 Windows の特定のバージョンで固定されているデバイスでも、Windows 10 更新プログラムのリングから、そのバージョンの品質更新プログラムおよびセキュリティ更新プログラムをインストールできます。

この新しい種類のポリシーは、今週テナントへのロールアウトが開始されます。 ご自分のテナントでまだこのポリシーを使用できない場合は、間もなく使用できるようになります。

#### <a name="add-and-change-key-information-in-plist-files-for-macos-applications---4736278---"></a>macOS アプリケーションの plist ファイルのキー情報を追加および変更する<!-- 4736278 -->
macOS デバイスでは、アプリまたはデバイスに関連付けられているプロパティ リスト ファイル (.plist) をアップロードするデバイス構成プロファイルを作成できるようになりました ( **[デバイス]**  >  **[構成プロファイル]**  >  **[プロファイルの作成]**  >  **[macOS]** (プラットフォーム) > **[設定ファイル]** (プロファイルの種類))。

マネージド基本設定は一部のアプリでのみサポートされており、これらのアプリではすべての設定を管理できるとは限りません。 ユーザー チャネルの設定ではなく、デバイス チャネルの設定を構成するプロパティ リスト ファイルを必ずアップロードします。

この機能の詳細については、[Microsoft Intune を使用した macOS デバイスへのプロパティ リスト ファイルの追加](../configuration/preference-file-settings-macos.md)に関するページを参照してください。

適用対象:

- 10.7 以降を実行している macOS デバイス

<!-- vvvvvvvvvvvvvvvvvvvvvv -->
### <a name="device-management"></a>デバイス管理

#### <a name="edit-device-name-value-for-autopilot-devices---2640074---"></a>Autopilot デバイスの [デバイス名] 値を編集する<!-- 2640074 -->
Azure AD 参加済み Autopilot デバイスの [デバイス名] 値を編集できます。  詳細については、[Autopilot デバイスの属性の編集](../enrollment/enrollment-autopilot.md#edit-autopilot-device-attributes)に関するページを参照してください。

#### <a name="edit-group-tag-value-for-autopilot-devices---4816775-----"></a>Autopilot デバイスの [グループ タグ] 値を編集する<!-- 4816775   -->
Autopilot デバイスの [グループ タグ] 値を編集できます。 詳細については、[Autopilot デバイスの属性の編集](../enrollment/enrollment-autopilot.md#edit-autopilot-device-attributes)に関するページを参照してください。

<!-- vvvvvvvvvvvvvvvvvvvvvv -->
### <a name="monitor-and-troubleshoot"></a>監視とトラブルシューティング

#### <a name="updated-support-experience---5012398---"></a>更新されたサポート エクスペリエンス<!-- 5012398 -->

本日から、[Intune のヘルプとサポートの取得](get-support.md)に関する、更新および合理化されたコンソール内のエクスペリエンスがテナントにロールアウトされます。 お客様がまだこの新しいエクスペリエンスを利用できない場合は、間もなく利用できるようになります。

コンソール内でのよくあるイシューの検索とフィードバック、およびサポートへの問い合わせに使用するワークフローが改善されました。 サポート イシューを作成するときに、コールバックまたはメールの返信をいつ受け取ることができるのかについての推定が、リアルタイムで表示されます。また、Premier および統合サポートのお客様は、より迅速なサポートを受けるために、それぞれのイシューについて、簡単に重大度を指定できます。

#### <a name="improved-intune-reporting-experience-public-preview----3791418---"></a>Intune レポート エクスペリエンスの向上 (パブリック プレビュー) <!-- 3791418 -->
Intune では、新しいレポートの種類、より優れたレポート編成、より対象を絞ったビュー、より優れたレポート機能、より一貫性のあるタイムリーなデータを含め、レポート エクスペリエンスが向上しています。 新しいレポートの種類では、次のことに重点が置かれています。

- **運用** - 正常性への悪影響に焦点を置いた最新のレコードが表示されます。 
- **組織** - 全体的な状態の概要が表示されます。
- **履歴** - 一定期間におけるパターンと傾向が表示されます。
- **スペシャリスト** - 生データを使用して独自のカスタム レポートを作成できます。

新しいレポートの最初のセットでは、デバイスのコンプライアンスに重点が置かれています。 詳細については、[ブログ - Microsoft Intune レポート フレームワーク](https://techcommunity.microsoft.com/t5/Intune-Customer-Success/New-Reporting-Framework-Coming-to-Intune/ba-p/1009553)および[Intune レポート](reports.md)に関するページを参照してください。

<!-- vvvvvvvvvvvvvvvvvvvvvv -->
### <a name="role-based-access-control"></a>ロール ベースのアクセス制御

#### <a name="duplicate-custom-or-built-in-roles----1081938-----"></a>カスタム ロールまたは組み込みロールを複製する <!-- 1081938   -->
組み込みロールとカスタム ロールをコピーできるようになりました。 詳細については、[ロールのコピー](../fundamentals/create-custom-role.md#copy-a-role)に関するページを参照してください。

#### <a name="new-permissions-for-school-administrator-role----5621805----"></a>学校管理者ロールの新しいアクセス許可 <!-- 5621805  -->  
学校管理者ロール > **[アクセス許可]**  >  **[登録プログラム]** に、2 つの新しいアクセス許可である **[プロファイルの割り当て]** と **[デバイスの同期]** が追加されました。 [デバイスの同期] アクセス許可を使用すると、グループ管理者は Windows Autopilot デバイスを同期できます。 [プロファイルの割り当て] アクセス許可を使用すると、これらの管理者はユーザーが開始した Apple 登録プロファイルを削除できます。 また、Autopilot デバイスの割り当てと Autopilot 展開プロファイルの割り当てを管理するためのアクセス許可も付与されます。 すべての学校管理者またはグループ管理者のアクセス許可の一覧については、[グループ管理者の割り当て](https://docs.microsoft.com/intune-education/group-admin-delegate)に関するページを参照してください。

<!-- vvvvvvvvvvvvvvvvvvvvvv -->
### <a name="security"></a>セキュリティ

#### <a name="bitlocker-key-rotation---2564951----"></a>BitLocker キーの交換<!-- 2564951  -->
Intune デバイス アクションを使用することで、Windows バージョン 1909 以降を実行するマネージド デバイスの [BitLocker 回復キーをリモートで交換](../protect/encrypt-devices.md#rotate-bitlocker-recovery-keys)できます。 回復キーが交換されるようにするには、回復キーの交換をサポートするようにデバイスを構成する必要があります。  

#### <a name="updates-to-dedicated-device-enrollment-to-support-scep-device-certificate-deployment----5198878----"></a>SCEP デバイス証明書の展開をサポートするための専用デバイス登録の更新 <!-- 5198878  -->
Intune では、Wi-Fi プロファイルに証明書ベースでアクセスできるよう、Android Enterprise 専用デバイスへの SCEP デバイス証明書の展開がサポートされるようになりました。 展開が機能するには、Microsoft Intune アプリがデバイス上に存在する必要があります。 そのため、Android Enterprise 専用デバイスの登録エクスペリエンスが更新されました。 新しい登録は、今までと同様に (QR、NFC、ゼロタッチ、またはデバイス識別子を使用して) 開始されますが、ユーザーが Intune アプリをインストールすることが必要になりました。 既存のデバイスでは、アプリのインストールがローリング方式で自動的に開始されます。

#### <a name="intune-audit-logs-for-business-to-business-collaboration--5670211---"></a>企業間コラボレーションのための Intune 監査ログ<!--5670211 -->
企業間 (B2B) コラボレーションにより、会社のアプリケーションやサービスを他の組織のゲスト ユーザーと安全に共有しながら、自社データの管理を維持することができます。 Intune では、B2B ゲスト ユーザーの監査ログがサポートされるようになりました。 たとえば、ゲスト ユーザーが変更を行うと、Intune では監査ログを使用してこのデータをキャプチャできます。 詳細については、[Azure Active Directory B2B でのゲスト ユーザー アクセス](https://docs.microsoft.com/azure/active-directory/b2b/what-is-b2b)に関するページを参照してください。

<!-- ########################## -->
## <a name="week-of-november-11-2019"></a>2019 年 11 月 11 日の週  

<!-- vvvvvvvvvvvvvvvvvvvvvv -->
### <a name="app-management"></a>アプリ管理  

#### <a name="improved-macos-enrollment-experience-in-company-portal----5074349----"></a>ポータル サイトにおける macOS の登録エクスペリエンスの改善 <!-- 5074349  -->  
macOS の登録エクスペリエンス用のポータル サイトには、よりシンプルな登録プロセスが備わっています。これにより、iOS の登録エクスペリエンス用のポータル サイトと、より厳密な一致がとれます。 デバイス ユーザーに次が表示されるようになりました。  

- より洗練されたユーザー インターフェイス。  
- 強化された登録チェックリスト。  
- デバイスの登録方法に関するより明確な説明。  
- 強化されたトラブルシューティング オプション。  

#### <a name="web-apps-launched-from-the-windows-company-portal-app---5030972---"></a>Windows ポータル サイト アプリから起動する Web アプリ<!-- 5030972 -->
エンド ユーザーは、Windows ポータル サイト アプリから直接 Web アプリを起動できるようになりました。 エンド ユーザーは、Web アプリを選択してから、 **[ブラウザーで開く]** オプションを選択できます。 発行された Web URL は、Web ブラウザー内で直接開かれます。 この機能は、次の週にわたってロールアウトされます。 Web アプリの詳細については、「[Web アプリを Microsoft Intune に追加する](../apps/web-app.md)」をご覧ください。  

#### <a name="new-assignment-type-column-in-company-portal-for-windows-10----5459950----"></a>Windows 10 のポータル サイトにおける新しい割り当ての種類の列 <!-- 5459950  -->
ポータル サイト > **[インストール済みアプリ]**  >  **[割り当ての種類]** 列の名前が、 **[組織で必要]** に変更されました。  その列の下に、アプリが組織によって必須、省略可能のいずれに設定されているかを示す **[はい]** または **[いいえ]** の値がユーザーに表示されます。 デバイス ユーザーが利用可能なアプリの概念について混乱していたため、このような変更が行われました。 ユーザーは、「[デバイスにアプリをインストールして共有する](../user-help/install-apps-cpapp-windows.md)」で、ポータル サイトからのアプリのインストールに関する詳細情報を参照できます。 ユーザーに対するポータル サイト アプリの構成方法の詳細については、「[Microsoft Intune ポータル サイト アプリを構成する方法](../apps/company-portal-app.md)」をご覧ください。  

<!-- ########################## -->
## <a name="week-of-november-4-2019"></a>2019 年 11 月 4 日の週

<!-- vvvvvvvvvvvvvvvvvvvvvv -->
### <a name="device-security"></a>デバイス セキュリティ

#### <a name="security-baselines-are-supported-on-microsoft-azure-government---4062552---"></a>セキュリティ ベースラインが Microsoft Azure Government でサポートされる<!-- 4062552 -->

*Microsoft Azure Government* でホストされている Intune のインスタンスで、[セキュリティ ベースライン](../protect/security-baselines.md)を使用して、ユーザーとデバイスのセキュリティ保護と保護を行えるようになりました。

## <a name="whats-new-archive"></a>新機能の公開履歴
以前の月については、[新機能の公開履歴](whats-new-archive.md)を参照してください。

## <a name="notices"></a>通知

[!INCLUDE [Intune notices](../includes/intune-notices.md)]


