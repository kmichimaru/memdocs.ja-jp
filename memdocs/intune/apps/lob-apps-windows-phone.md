---
title: Windows Phone の基幹業務アプリを Microsoft Intune に追加する
titleSuffix: ''
description: Microsoft Intune を使って Windows Phone の基幹業務 (LOB) アプリを追加する方法について説明します。
keywords: ''
author: Erikre
ms.author: erikre
manager: dougeby
ms.date: 01/23/2020
ms.topic: conceptual
ms.service: microsoft-intune
ms.subservice: apps
ms.localizationpriority: high
ms.technology: ''
ms.assetid: a097b7b2-d01d-454b-954c-da4f3cd0ae86
ms.reviewer: mghadial
ms.suite: ems
search.appverid: MET150
ms.custom: intune-azure
ms.collection: M365-identity-device-management
ms.openlocfilehash: c64d6dab674b75fd4e62638ac6a221cd2aca4a85
ms.sourcegitcommit: 7f17d6eb9dd41b031a6af4148863d2ffc4f49551
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/21/2020
ms.locfileid: "80323984"
---
# <a name="add-a-windows-phone-line-of-business-app-to-microsoft-intune"></a>Windows Phone の基幹業務アプリを Microsoft Intune に追加する

[!INCLUDE [azure_portal](../includes/azure_portal.md)]

この記事の情報を使用して、Microsoft Intune に Windows Phone の基幹業務 (LOB) アプリを追加できます。 LOB アプリとは、アプリのインストール ファイルから Intune に追加するアプリのことです。 通常、この種類のアプリは社内で作成されます。 Intune によって、ユーザーのデバイス上に LOB アプリがインストールされます。 

## <a name="select-the-app-type"></a>アプリの種類を選択する

1. [Microsoft Endpoint Manager 管理センター](https://go.microsoft.com/fwlink/?linkid=2109431)にサインインします。
2. **[アプリ]**  >  **[すべてのアプリ]**  >  **[追加]** の順に選択します。
3. **[アプリの種類の選択]** ペインの **[その他]** のアプリの種類で、 **[基幹業務アプリ]** を選択します。
4. **[選択]** をクリックします。 **[アプリの追加]** 手順が表示されます。

## <a name="step-1---app-information"></a>ステップ 1 - アプリ情報

### <a name="select-the-app-package-file"></a>アプリ パッケージ ファイルを選択する

1. **[アプリの追加]** ウィンドウで、 **[アプリ パッケージ ファイルの選択]** をクリックします。 
2. **[アプリのパッケージ ファイル]** ウィンドウで、参照ボタンを選択します。 次に、拡張子が **.xap** の Windows Phone インストール ファイルを選択します。
   アプリの詳細が表示されます。
3. 操作を完了したら、 **[アプリ パッケージ ファイル]** ペインの **[OK]** を選択してアプリを追加します。

### <a name="set-app-information"></a>アプリ情報を設定する

1. **[アプリ情報]** ページで、アプリの詳細を追加します。 選択したアプリによっては、このウィンドウ内の一部の値が自動的に入力されている場合があります。
    - **名前**:アプリの名前を入力します。これは会社のポータルに表示されます。 使用するアプリ名はすべて一意にします。 同じアプリ名が 2 つ存在する場合、いずれか 1 つのアプリのみが会社のポータルに表示されます。
    - **説明**:アプリの説明を入力します。 説明はポータル サイトに表示されます。
    - **[発行元]** : アプリの発行元の名前を入力します。
    - **[最低限のオペレーティング システム]** :アプリをインストールできる最小限のオペレーティング システム バージョンを一覧から選択します。 これよりも前のオペレーティング システムがアプリの割り当て先デバイスにインストールされている場合、そのアプリはインストールされません。
    - **[カテゴリ]** :1 つまたは複数の組み込みアプリ カテゴリを選択するか、ご自身で作成したカテゴリを選択します。 カテゴリを使用すれば、ユーザーはポータル サイトを参照する際にアプリを見つけやすくなります。
    - **[会社のポータルでおすすめアプリとして表示します]** : ユーザーがアプリを参照するとき、会社のポータルのメイン ページにアプリが目立つように表示されます。
    - **[情報 URL]** : このアプリに関する情報が含まれる Web サイトの URL を入力することもできます。 この URL はポータル サイトに表示されます。
    - **[プライバシー URL]** : このアプリのプライバシー情報が含まれる Web サイトの URL を入力することもできます。 この URL はポータル サイトに表示されます。
    - **[開発者]** : (省略可能) アプリ開発者の名前を入力します。
    - **[所有者]** : (省略可能) このアプリの所有者の名前を入力します。 たとえば、「**人事部**」と入力します。
    - **[メモ]** : このアプリに関連付けるメモを入力します。
    - **[ロゴ]** : アプリに関連付けるアイコンをアップロードします。 ユーザーが会社のポータルを参照するとき、アプリにアイコンが表示されます。
2. **[次 へ]** をクリックして **[スコープ タグ]** ページを表示します。

## <a name="step-2---select-scope-tags-optional"></a>ステップ 2 - スコープのタグを選択する (省略可能)
スコープのタグを使って、Intune のクライアント アプリの情報を表示できるユーザーを決定することができます。 スコープのタグの詳細については、[分散 IT のためのロールベースのアクセス制御とスコープのタグの使用](../fundamentals/scope-tags.md)に関するページをご覧ください。

1. **[スコープ タグを選択]** をクリックして、必要に応じてアプリのスコープ タグを追加します。 
2. **[次へ]** をクリックして、 **[割り当て]** ページを表示します。

## <a name="step-3---assignments"></a>ステップ 3 - 割り当て

1. アプリのグループ割り当てについて、 **[必須]** 、 **[登録済みデバイスで使用可能]** 、または **[アンインストール]** を選択します。 詳細については、「[ユーザーとデバイスを整理するためのグループを追加する](../fundamentals/groups-add.md)」と「[Microsoft Intune を使用してアプリをグループに割り当てる](apps-deploy.md)」を参照してください。
2. **[次へ]** をクリックして、 **[確認と作成]** ページを表示します。

## <a name="step-4---review--create"></a>ステップ 4 - 確認と作成

1. アプリに入力した値と設定を確認します。
2. 完了したら、 **[作成]** をクリックしてアプリを Intune に追加します。

    基幹業務アプリの **[概要]** ブレードが表示されます。

作成したアプリがアプリ一覧に表示されます。 一覧から、選択したグループにアプリを割り当てることができます。 詳細については、[アプリをグループに割り当てる方法](apps-deploy.md)に関するページを参照してください。

## <a name="next-steps"></a>次のステップ

- 作成したアプリはアプリの一覧に表示されます。 選択したグループにアプリを割り当てることができます。 詳細については、[アプリをグループに割り当てる方法](apps-deploy.md)に関するページを参照してください。

- アプリのプロパティと割り当てを監視する方法について説明します。 「[アプリ情報と割り当てを監視する方法](apps-monitor.md)」を参照してください。

- Intune におけるアプリのコンテキストについて説明します。 「[デバイスとアプリのライフサイクルの概要](../fundamentals/device-lifecycle.md)」を参照してください。
