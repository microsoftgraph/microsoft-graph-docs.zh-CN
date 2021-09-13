---
title: 创建 Azure Active Directory 应用
description: 创建Azure Active Directory应用程序注册以与用户Microsoft 365
ms.localizationpriority: medium
author: waldekmastykarz
ms.openlocfilehash: 21a298874beb7cc3c67bc807b4c51fce42a39564
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59078523"
---
# <a name="create-an-azure-active-directory-app-to-use-with-the-microsoft-graph-toolkit"></a>创建Azure Active Directory Microsoft Graph Toolkit

Microsoft Graph是一种用于连接到 Microsoft 365 的 API，它使用 OAuth 2.0 进行保护。 若要将应用连接到 Microsoft 365，你需要在 Azure Active Directory (Azure AD) 创建一个应用，并授权此应用程序代表使用你的应用的用户访问特定资源。 本主题介绍如何注册和配置 Web 应用程序以与 Microsoft Graph Toolkit。

## <a name="add-new-application-registration-in-azure-active-directory"></a>在应用程序中添加新的Azure Active Directory

若要在应用程序Azure Active Directory，需要添加新的应用程序注册，然后配置应用名称和 URL 位置。

若要在应用程序中创建Azure Active Directory：

1. 转到 Azure 门户，位于 https://portal.azure.com 。
1. 从菜单中，选择 **"Azure Active Directory"。**
1. 从"Azure Active Directory"菜单中，选择 **"应用注册"。**
1. 从顶部菜单中，选择"新建 **注册"** 按钮。
1. 输入应用的名称;例如， `My M365 app` 。
1. 对于受支持的帐户类型 [](/azure/active-directory/develop/single-and-multi-tenant-apps#who-can-sign-in-to-your-app)类型，请选择任何组织目录中的帐户 (任何 Azure AD 目录 - 多租户) 和个人 Microsoft 帐户 (例如 **Skype、Xbox) 。**
1. 对于 **"重定向 URI"** 字段：
    - 如果使用 或 ，请选择"SPA (应用程序) "，在"URL"字段中输入重定向 URL (`Msal2Provider` `TeamsMsal2Provider` 和/或在本地测试 `http://localhost`) 。 
    - 如果使用 或 `MsalProvider` `TeamsProvider` ，请选择 **"Web"，** 在"URL"字段中，输入重定向 URL (和/或在本地测试 `http://localhost`) 。 
1. 通过选择"注册" **按钮确认** 更改。

## <a name="enable-oauth-implicit-flow-only-for-msalprovider-and-teamsprovider"></a>仅对 MsalProvider (TeamsProvider 启用 OAuth 隐式流) 

在大多数情况下，你将在仅Graph Toolkit代码的客户端应用程序中使用 Microsoft 应用程序。 由于客户端应用无法安全存储密钥，因此你需要使用 [OAuth](/azure/active-directory/develop/v2-oauth2-implicit-grant-flow?WT.mc_id=m365-10340-wmastyka)隐式流，它假定应用的标识基于其 ID 和 URL。

1. 在 Azure 门户中，打开新创建的应用注册。
1. 从菜单中， **选择身份验证**。
1. 在 **隐式授予** 部分中，同时启用 **访问令牌** 和 **ID 令牌** 选项。
1. 通过选择"保存"按钮 **确认** 更改。

## <a name="next-steps"></a>后续步骤

- [使用 vanilla](./build-a-web-app.md) JavaScript (生成 Web) 
- [构建 Microsoft Teams 选项卡](./build-a-microsoft-teams-tab.md)
- [将 Toolkit与 React](./use-toolkit-with-react.md)
- [将Toolkit与Angular](./use-toolkit-with-angular.md)
