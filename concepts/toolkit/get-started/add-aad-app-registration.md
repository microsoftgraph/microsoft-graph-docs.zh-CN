---
title: 创建 Azure Active Directory 应用
description: 创建Azure Active Directory应用程序注册以与用户Microsoft 365
localization_priority: Normal
author: waldekmastykarz
ms.openlocfilehash: b68281473d884309c23a72979ae07a8a9c752d2f
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579919"
---
# <a name="create-an-azure-active-directory-app-to-use-with-the-microsoft-graph-toolkit"></a><span data-ttu-id="e4db4-103">创建Azure Active Directory Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="e4db4-103">Create an Azure Active Directory app to use with the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="e4db4-104">Microsoft Graph是一种用于连接到 Microsoft 365 的 API，它使用 OAuth 2.0 进行保护。</span><span class="sxs-lookup"><span data-stu-id="e4db4-104">Microsoft Graph, the API that you use to connect to Microsoft 365, is secured with OAuth 2.0.</span></span> <span data-ttu-id="e4db4-105">若要将应用连接到 Microsoft 365，你需要在 Azure Active Directory (Azure AD) 创建一个应用，并授权此应用程序代表使用你的应用的用户访问特定资源。</span><span class="sxs-lookup"><span data-stu-id="e4db4-105">In order to connect your app to Microsoft 365, you will need to create an app in Azure Active Directory (Azure AD) and grant this app permissions to access specific resources on behalf of the person using your app.</span></span> <span data-ttu-id="e4db4-106">本主题介绍如何注册和配置 Web 应用程序以用于 Microsoft Graph Toolkit。</span><span class="sxs-lookup"><span data-stu-id="e4db4-106">This topic describes how to register and configure a web application to use with Microsoft Graph Toolkit.</span></span>

## <a name="add-new-application-registration-in-azure-active-directory"></a><span data-ttu-id="e4db4-107">在应用程序中添加新的Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="e4db4-107">Add new application registration in Azure Active Directory</span></span>

<span data-ttu-id="e4db4-108">若要在应用程序Azure Active Directory，需要添加新的应用程序注册，然后配置应用名称和 URL 位置。</span><span class="sxs-lookup"><span data-stu-id="e4db4-108">To create an application in Azure Active Directory, you need to add a new application registration, and then configure an app name and URL location.</span></span>

<span data-ttu-id="e4db4-109">若要在应用程序中创建Azure Active Directory：</span><span class="sxs-lookup"><span data-stu-id="e4db4-109">To create the app in Azure Active Directory:</span></span>

1. <span data-ttu-id="e4db4-110">转到 Azure 门户，位于 https://portal.azure.com 。</span><span class="sxs-lookup"><span data-stu-id="e4db4-110">Go to the Azure portal at https://portal.azure.com.</span></span>
1. <span data-ttu-id="e4db4-111">从菜单中，选择 **"Azure Active Directory"。**</span><span class="sxs-lookup"><span data-stu-id="e4db4-111">From the menu, select **Azure Active Directory**.</span></span>
1. <span data-ttu-id="e4db4-112">从"Azure Active Directory"菜单中，选择 **"应用注册"。**</span><span class="sxs-lookup"><span data-stu-id="e4db4-112">From the Azure Active Directory menu, select **App registrations**.</span></span>
1. <span data-ttu-id="e4db4-113">从顶部菜单中，选择"新建 **注册"** 按钮。</span><span class="sxs-lookup"><span data-stu-id="e4db4-113">From the top menu, select the **New registration** button.</span></span>
1. <span data-ttu-id="e4db4-114">输入应用的名称;例如， `My M365 app` 。</span><span class="sxs-lookup"><span data-stu-id="e4db4-114">Enter the name for your app; for example, `My M365 app`.</span></span>
1. <span data-ttu-id="e4db4-115">对于受支持的帐户类型 [](/azure/active-directory/develop/single-and-multi-tenant-apps#who-can-sign-in-to-your-app)类型，请选择任何组织目录中的帐户 (任何 Azure AD 目录 - 多租户) 和个人 Microsoft 帐户 (例如 **Skype、Xbox) 。**</span><span class="sxs-lookup"><span data-stu-id="e4db4-115">For the type of [supported account types](/azure/active-directory/develop/single-and-multi-tenant-apps#who-can-sign-in-to-your-app), select **Accounts in any organizational directory (Any Azure AD directory - Multitenant) and personal Microsoft accounts (e.g. Skype, Xbox)**.</span></span>
1. <span data-ttu-id="e4db4-116">在" **重定向 URI"** 字段中的下拉列表中，选择"SPA (") "， **在**"URL"字段中输入 `http://localhost:3000` 。</span><span class="sxs-lookup"><span data-stu-id="e4db4-116">In the **Redirect URI** field, in the dropdown, select **Single Page Application (SPA)**, and in the URL field, enter `http://localhost:3000`.</span></span> <span data-ttu-id="e4db4-117">注意：如果使用的是 MSAL 提供程序，而不是 MSAL 2.0 提供程序，则需要选择 **"Web"，** 而不是 **"SPA"。**</span><span class="sxs-lookup"><span data-stu-id="e4db4-117">Note: if you are using MSAL Provider and not MSAL 2.0 Provider, you will need to select **Web** instead of **SPA**.</span></span>
1. <span data-ttu-id="e4db4-118">通过选择"注册" **按钮确认** 更改。</span><span class="sxs-lookup"><span data-stu-id="e4db4-118">Confirm changes by selecting the **Register** button.</span></span>

## <a name="enable-oauth-implicit-flow-only-for-msal-10-provider"></a><span data-ttu-id="e4db4-119">仅对 MSAL 1.0 () 启用 OAuth 隐式流) </span><span class="sxs-lookup"><span data-stu-id="e4db4-119">Enable OAuth implicit flow (only for MSAL 1.0 provider)</span></span>

<span data-ttu-id="e4db4-120">在大多数情况下，你将在仅Graph Toolkit代码的客户端应用程序中使用 Microsoft 代码。</span><span class="sxs-lookup"><span data-stu-id="e4db4-120">In most cases, you will use Microsoft Graph Toolkit in client-side applications that consist only of client-side code.</span></span> <span data-ttu-id="e4db4-121">由于客户端应用无法安全存储密钥，因此你需要使用 [OAuth](/azure/active-directory/develop/v2-oauth2-implicit-grant-flow?WT.mc_id=m365-10340-wmastyka)隐式流，该流假定应用基于其 ID 和 URL 的标识。</span><span class="sxs-lookup"><span data-stu-id="e4db4-121">Because client-side apps can't store secrets securely, you need to use [OAuth implicit flow](/azure/active-directory/develop/v2-oauth2-implicit-grant-flow?WT.mc_id=m365-10340-wmastyka), which assumes an app's identity based on its ID and URL.</span></span>

1. <span data-ttu-id="e4db4-122">在 Azure 门户中，打开新创建的应用注册。</span><span class="sxs-lookup"><span data-stu-id="e4db4-122">In the Azure Portal, open your newly created app registration.</span></span>
1. <span data-ttu-id="e4db4-123">从菜单中， **选择身份验证**。</span><span class="sxs-lookup"><span data-stu-id="e4db4-123">From the menu, choose **Authentication**.</span></span>
1. <span data-ttu-id="e4db4-124">在 **隐式授予** 部分中，同时启用 **访问令牌** 和 **ID 令牌** 选项。</span><span class="sxs-lookup"><span data-stu-id="e4db4-124">In the **Implicit grant** section, enable both **Access tokens** and **ID tokens** options.</span></span>
1. <span data-ttu-id="e4db4-125">通过选择"保存"按钮 **确认** 更改。</span><span class="sxs-lookup"><span data-stu-id="e4db4-125">Confirm your changes by choosing the **Save** button.</span></span>

## <a name="next-steps"></a><span data-ttu-id="e4db4-126">后续步骤</span><span class="sxs-lookup"><span data-stu-id="e4db4-126">Next steps</span></span>

- <span data-ttu-id="e4db4-127">[使用 vanilla](./build-a-web-app.md) JavaScript (生成 Web) </span><span class="sxs-lookup"><span data-stu-id="e4db4-127">[Build a web application](./build-a-web-app.md) (vanilla JavaScript)</span></span>
- [<span data-ttu-id="e4db4-128">构建 Microsoft Teams 选项卡</span><span class="sxs-lookup"><span data-stu-id="e4db4-128">Build a Microsoft Teams tab</span></span>](./build-a-microsoft-teams-tab.md)
- [<span data-ttu-id="e4db4-129">将 Toolkit与 React</span><span class="sxs-lookup"><span data-stu-id="e4db4-129">Use the Toolkit with React</span></span>](./use-toolkit-with-react.md)
- [<span data-ttu-id="e4db4-130">将Toolkit与Angular</span><span class="sxs-lookup"><span data-stu-id="e4db4-130">Use the Toolkit with Angular</span></span>](./use-toolkit-with-angular.md)
