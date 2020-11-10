---
title: 创建 Azure Active Directory 应用程序
description: 创建用于与 Microsoft 365 通信的 Azure Active Directory 应用程序注册
localization_priority: Normal
author: waldekmastykarz
ms.openlocfilehash: 13b3a876e80e5c2437eba3d264053cdbbcbb5909
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48982321"
---
# <a name="create-an-azure-active-directory-app-to-use-with-the-microsoft-graph-toolkit"></a>创建 Azure Active Directory 应用程序以用于 Microsoft Graph 工具包

Microsoft Graph 是用于连接到 Microsoft 365 的 API，通过 OAuth 2.0 进行保护。 若要将应用程序连接到 Microsoft 365，您需要在 Azure Active Directory 中创建一个应用程序 (Azure AD) 并授予此应用程序权限代表使用您的应用程序的用户访问特定资源。 本主题介绍如何注册和配置要与 Microsoft Graph 工具包一起使用的 web 应用程序。

## <a name="add-new-application-registration-in-azure-active-directory"></a>在 Azure Active Directory 中添加新的应用程序注册

若要在 Azure Active Directory 中创建应用程序，您需要添加新的应用程序注册，然后配置应用程序名称和 URL 位置。

若要在 Azure Active Directory 中创建应用程序，请执行以下操作：

1. 转到 Azure 门户处 https://portal.azure.com 。
1. 从菜单中选择 " **Azure Active Directory** "。
1. 从 "Azure Active Directory" 菜单中，选择 " **应用注册** "。
1. 从顶部菜单中，选择 " **新注册** " 按钮。
1. 输入您的应用程序的名称;对于 exampe，为 `My M365 app` 。
1. 对于 [受支持的帐户类型](/azure/active-directory/develop/single-and-multi-tenant-apps#who-can-sign-in-to-your-app)的类型，请选择 "任何 **(任何 Azure AD 目录-多租户") 和个人 Microsoft 帐户 (例如 Skype、Xbox) 的任何组织目录中的 "帐户"** 。
1. 在 " **重定向 URI** " 字段的下拉列表中，选择 " **Web** "，并在 "URL" 字段中输入 `https://localhost:3000` 。
1. 通过选择 " **注册** " 按钮确认更改。

## <a name="enable-oauth-implicit-flow"></a>启用 OAuth 隐式流

在大多数情况下，将在仅包含客户端代码的客户端应用程序中使用 Microsoft Graph 工具包。 由于客户端应用程序无法安全地存储机密信息，因此您需要使用 [OAuth 隐式流](/azure/active-directory/develop/v2-oauth2-implicit-grant-flow?WT.mc_id=m365-10340-wmastyka)，它假定应用程序的 ID 和 URL 基于其标识。

1. 在 Azure 门户中，打开新创建的应用注册。
1. 从菜单中选择 " **身份验证** "。
1. 在 " **隐式授予** " 部分，启用 " **访问令牌** " 和 " **ID 令牌** " 选项。
1. 通过选择 " **保存** " 按钮确认更改。

## <a name="next-steps"></a>后续步骤

- [构建 web 应用程序](./build-a-web-app.md) (vanilla JavaScript) 
- [构建 Microsoft Teams 选项卡](./build-a-microsoft-teams-tab.md)
- [将此工具包与响应结合使用](./use-toolkit-with-react.md)
- [使用具有角度的工具包](./use-toolkit-with-angular.md)
