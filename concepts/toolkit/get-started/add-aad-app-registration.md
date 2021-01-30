---
title: 创建 Azure Active Directory 应用
description: 创建 Azure Active Directory 应用程序注册以与 Microsoft 365 通信
localization_priority: Normal
author: waldekmastykarz
ms.openlocfilehash: 821cd6981ddb24e3917a4c0720f1c8c524081f54
ms.sourcegitcommit: 1138d6e84f64f3727e180da10f89b89021855c3e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2021
ms.locfileid: "50059565"
---
# <a name="create-an-azure-active-directory-app-to-use-with-the-microsoft-graph-toolkit"></a><span data-ttu-id="2995d-103">创建 Azure Active Directory 应用以与 Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="2995d-103">Create an Azure Active Directory app to use with the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="2995d-104">Microsoft Graph 是一种用于连接到 Microsoft 365 的 API，它使用 OAuth 2.0 进行保护。</span><span class="sxs-lookup"><span data-stu-id="2995d-104">Microsoft Graph, the API that you use to connect to Microsoft 365, is secured with OAuth 2.0.</span></span> <span data-ttu-id="2995d-105">若要将应用连接到 Microsoft 365，你需要在 Azure Active Directory (Azure AD) 中创建应用，并授予此应用权限以代表使用你的应用的用户访问特定资源。</span><span class="sxs-lookup"><span data-stu-id="2995d-105">In order to connect your app to Microsoft 365, you will need to create an app in Azure Active Directory (Azure AD) and grant this app permissions to access specific resources on behalf of the person using your app.</span></span> <span data-ttu-id="2995d-106">本主题介绍如何注册和配置 Web 应用程序以与 Microsoft Graph Toolkit。</span><span class="sxs-lookup"><span data-stu-id="2995d-106">This topic describes how to register and configure a web application to use with Microsoft Graph Toolkit.</span></span>

## <a name="add-new-application-registration-in-azure-active-directory"></a><span data-ttu-id="2995d-107">在 Azure Active Directory 中添加新的应用程序注册</span><span class="sxs-lookup"><span data-stu-id="2995d-107">Add new application registration in Azure Active Directory</span></span>

<span data-ttu-id="2995d-108">若要在 Azure Active Directory 中创建应用程序，需要添加新的应用程序注册，然后配置应用名称和 URL 位置。</span><span class="sxs-lookup"><span data-stu-id="2995d-108">To create an application in Azure Active Directory, you need to add a new application registration, and then configure an app name and URL location.</span></span>

<span data-ttu-id="2995d-109">若要在 Azure Active Directory 中创建应用，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="2995d-109">To create the app in Azure Active Directory:</span></span>

1. <span data-ttu-id="2995d-110">转到 Azure 门户 https://portal.azure.com 。</span><span class="sxs-lookup"><span data-stu-id="2995d-110">Go to the Azure portal at https://portal.azure.com.</span></span>
1. <span data-ttu-id="2995d-111">从菜单中，选择 **Azure Active Directory。**</span><span class="sxs-lookup"><span data-stu-id="2995d-111">From the menu, select **Azure Active Directory**.</span></span>
1. <span data-ttu-id="2995d-112">从 Azure Active Directory 菜单中，选择 **应用注册**。</span><span class="sxs-lookup"><span data-stu-id="2995d-112">From the Azure Active Directory menu, select **App registrations**.</span></span>
1. <span data-ttu-id="2995d-113">从顶部菜单中，选择" **新建注册"** 按钮。</span><span class="sxs-lookup"><span data-stu-id="2995d-113">From the top menu, select the **New registration** button.</span></span>
1. <span data-ttu-id="2995d-114">输入应用的名称;例如 `My M365 app` ，。</span><span class="sxs-lookup"><span data-stu-id="2995d-114">Enter the name for your app; for example, `My M365 app`.</span></span>
1. <span data-ttu-id="2995d-115">对于支持的帐户类型 [](/azure/active-directory/develop/single-and-multi-tenant-apps#who-can-sign-in-to-your-app)类型，请选择任何组织目录中的帐户 (任何 Azure AD 目录 - 多租户) 和个人 Microsoft 帐户 (例如 **Skype、Xbox) 。**</span><span class="sxs-lookup"><span data-stu-id="2995d-115">For the type of [supported account types](/azure/active-directory/develop/single-and-multi-tenant-apps#who-can-sign-in-to-your-app), select **Accounts in any organizational directory (Any Azure AD directory - Multitenant) and personal Microsoft accounts (e.g. Skype, Xbox)**.</span></span>
1. <span data-ttu-id="2995d-116">在" **重定向 URI"** 字段中的下拉列表中，选择 **"Web"，** 在"URL"字段中输入 `http://localhost:3000` 。</span><span class="sxs-lookup"><span data-stu-id="2995d-116">In the **Redirect URI** field, in the dropdown, select **Web**, and in the URL field, enter `http://localhost:3000`.</span></span>
1. <span data-ttu-id="2995d-117">通过选择"注册"按钮 **确认** 更改。</span><span class="sxs-lookup"><span data-stu-id="2995d-117">Confirm changes by selecting the **Register** button.</span></span>

## <a name="enable-oauth-implicit-flow"></a><span data-ttu-id="2995d-118">启用 OAuth 隐式流</span><span class="sxs-lookup"><span data-stu-id="2995d-118">Enable OAuth implicit flow</span></span>

<span data-ttu-id="2995d-119">在大多数情况下，你将在仅Toolkit代码的客户端应用程序中使用 Microsoft Graph 应用程序。</span><span class="sxs-lookup"><span data-stu-id="2995d-119">In most cases, you will use Microsoft Graph Toolkit in client-side applications that consist only of client-side code.</span></span> <span data-ttu-id="2995d-120">由于客户端应用无法安全地存储密钥，因此你需要使用 [OAuth](/azure/active-directory/develop/v2-oauth2-implicit-grant-flow?WT.mc_id=m365-10340-wmastyka)隐式流，该流假定应用基于其 ID 和 URL 的标识。</span><span class="sxs-lookup"><span data-stu-id="2995d-120">Because client-side apps can't store secrets securely, you need to use [OAuth implicit flow](/azure/active-directory/develop/v2-oauth2-implicit-grant-flow?WT.mc_id=m365-10340-wmastyka), which assumes an app's identity based on its ID and URL.</span></span>

1. <span data-ttu-id="2995d-121">在 Azure 门户中，打开新创建的应用注册。</span><span class="sxs-lookup"><span data-stu-id="2995d-121">In the Azure Portal, open your newly created app registration.</span></span>
1. <span data-ttu-id="2995d-122">从菜单中，选择"**身份验证"。**</span><span class="sxs-lookup"><span data-stu-id="2995d-122">From the menu, choose **Authentication**.</span></span>
1. <span data-ttu-id="2995d-123">在 **隐式授予** 部分中，同时启用 **访问令牌\*\*\*\*和 ID 令牌** 选项。</span><span class="sxs-lookup"><span data-stu-id="2995d-123">In the **Implicit grant** section, enable both **Access tokens** and **ID tokens** options.</span></span>
1. <span data-ttu-id="2995d-124">通过选择"保存"按钮 **确认** 更改。</span><span class="sxs-lookup"><span data-stu-id="2995d-124">Confirm your changes by choosing the **Save** button.</span></span>

## <a name="next-steps"></a><span data-ttu-id="2995d-125">后续步骤</span><span class="sxs-lookup"><span data-stu-id="2995d-125">Next steps</span></span>

- <span data-ttu-id="2995d-126">[使用 javaScript (](./build-a-web-app.md) 生成 Web) </span><span class="sxs-lookup"><span data-stu-id="2995d-126">[Build a web application](./build-a-web-app.md) (vanilla JavaScript)</span></span>
- [<span data-ttu-id="2995d-127">构建 Microsoft Teams 选项卡</span><span class="sxs-lookup"><span data-stu-id="2995d-127">Build a Microsoft Teams tab</span></span>](./build-a-microsoft-teams-tab.md)
- [<span data-ttu-id="2995d-128">将 Toolkit与 React 一同使用</span><span class="sxs-lookup"><span data-stu-id="2995d-128">Use the Toolkit with React</span></span>](./use-toolkit-with-react.md)
- [<span data-ttu-id="2995d-129">将 Toolkit与 Angular 一同使用</span><span class="sxs-lookup"><span data-stu-id="2995d-129">Use the Toolkit with Angular</span></span>](./use-toolkit-with-angular.md)
