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
# <a name="create-an-azure-active-directory-app-to-use-with-the-microsoft-graph-toolkit"></a><span data-ttu-id="a01ca-103">创建 Azure Active Directory 应用程序以用于 Microsoft Graph 工具包</span><span class="sxs-lookup"><span data-stu-id="a01ca-103">Create an Azure Active Directory app to use with the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="a01ca-104">Microsoft Graph 是用于连接到 Microsoft 365 的 API，通过 OAuth 2.0 进行保护。</span><span class="sxs-lookup"><span data-stu-id="a01ca-104">Microsoft Graph, the API that you use to connect to Microsoft 365, is secured with OAuth 2.0.</span></span> <span data-ttu-id="a01ca-105">若要将应用程序连接到 Microsoft 365，您需要在 Azure Active Directory 中创建一个应用程序 (Azure AD) 并授予此应用程序权限代表使用您的应用程序的用户访问特定资源。</span><span class="sxs-lookup"><span data-stu-id="a01ca-105">In order to connect your app to Microsoft 365, you will need to create an app in Azure Active Directory (Azure AD) and grant this app permissions to access specific resources on behalf of the person using your app.</span></span> <span data-ttu-id="a01ca-106">本主题介绍如何注册和配置要与 Microsoft Graph 工具包一起使用的 web 应用程序。</span><span class="sxs-lookup"><span data-stu-id="a01ca-106">This topic describes how to register and configure a web application to use with Microsoft Graph Toolkit.</span></span>

## <a name="add-new-application-registration-in-azure-active-directory"></a><span data-ttu-id="a01ca-107">在 Azure Active Directory 中添加新的应用程序注册</span><span class="sxs-lookup"><span data-stu-id="a01ca-107">Add new application registration in Azure Active Directory</span></span>

<span data-ttu-id="a01ca-108">若要在 Azure Active Directory 中创建应用程序，您需要添加新的应用程序注册，然后配置应用程序名称和 URL 位置。</span><span class="sxs-lookup"><span data-stu-id="a01ca-108">To create an application in Azure Active Directory, you need to add a new application registration, and then configure an app name and URL location.</span></span>

<span data-ttu-id="a01ca-109">若要在 Azure Active Directory 中创建应用程序，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="a01ca-109">To create the app in Azure Active Directory:</span></span>

1. <span data-ttu-id="a01ca-110">转到 Azure 门户处 https://portal.azure.com 。</span><span class="sxs-lookup"><span data-stu-id="a01ca-110">Go to the Azure portal at https://portal.azure.com.</span></span>
1. <span data-ttu-id="a01ca-111">从菜单中选择 " **Azure Active Directory** "。</span><span class="sxs-lookup"><span data-stu-id="a01ca-111">From the menu, select **Azure Active Directory**.</span></span>
1. <span data-ttu-id="a01ca-112">从 "Azure Active Directory" 菜单中，选择 " **应用注册** "。</span><span class="sxs-lookup"><span data-stu-id="a01ca-112">From the Azure Active Directory menu, select **App registrations**.</span></span>
1. <span data-ttu-id="a01ca-113">从顶部菜单中，选择 " **新注册** " 按钮。</span><span class="sxs-lookup"><span data-stu-id="a01ca-113">From the top menu, select the **New registration** button.</span></span>
1. <span data-ttu-id="a01ca-114">输入您的应用程序的名称;对于 exampe，为 `My M365 app` 。</span><span class="sxs-lookup"><span data-stu-id="a01ca-114">Enter the name for your app; for exampe, `My M365 app`.</span></span>
1. <span data-ttu-id="a01ca-115">对于 [受支持的帐户类型](/azure/active-directory/develop/single-and-multi-tenant-apps#who-can-sign-in-to-your-app)的类型，请选择 "任何 **(任何 Azure AD 目录-多租户") 和个人 Microsoft 帐户 (例如 Skype、Xbox) 的任何组织目录中的 "帐户"** 。</span><span class="sxs-lookup"><span data-stu-id="a01ca-115">For the type of [supported account types](/azure/active-directory/develop/single-and-multi-tenant-apps#who-can-sign-in-to-your-app), select **Accounts in any organizational directory (Any Azure AD directory - Multitenant) and personal Microsoft accounts (e.g. Skype, Xbox)**.</span></span>
1. <span data-ttu-id="a01ca-116">在 " **重定向 URI** " 字段的下拉列表中，选择 " **Web** "，并在 "URL" 字段中输入 `https://localhost:3000` 。</span><span class="sxs-lookup"><span data-stu-id="a01ca-116">In the **Redirect URI** field, in the dropdown, select **Web** , and in the URL field, enter `https://localhost:3000`.</span></span>
1. <span data-ttu-id="a01ca-117">通过选择 " **注册** " 按钮确认更改。</span><span class="sxs-lookup"><span data-stu-id="a01ca-117">Confirm changes by selecting the **Register** button.</span></span>

## <a name="enable-oauth-implicit-flow"></a><span data-ttu-id="a01ca-118">启用 OAuth 隐式流</span><span class="sxs-lookup"><span data-stu-id="a01ca-118">Enable OAuth implicit flow</span></span>

<span data-ttu-id="a01ca-119">在大多数情况下，将在仅包含客户端代码的客户端应用程序中使用 Microsoft Graph 工具包。</span><span class="sxs-lookup"><span data-stu-id="a01ca-119">In most cases, you will use Microsoft Graph Toolkit in client-side applications that consist only of client-side code.</span></span> <span data-ttu-id="a01ca-120">由于客户端应用程序无法安全地存储机密信息，因此您需要使用 [OAuth 隐式流](/azure/active-directory/develop/v2-oauth2-implicit-grant-flow?WT.mc_id=m365-10340-wmastyka)，它假定应用程序的 ID 和 URL 基于其标识。</span><span class="sxs-lookup"><span data-stu-id="a01ca-120">Because client-side apps can't store secrets securely, you need to use [OAuth implicit flow](/azure/active-directory/develop/v2-oauth2-implicit-grant-flow?WT.mc_id=m365-10340-wmastyka), which assumes an app's identity based on its ID and URL.</span></span>

1. <span data-ttu-id="a01ca-121">在 Azure 门户中，打开新创建的应用注册。</span><span class="sxs-lookup"><span data-stu-id="a01ca-121">In the Azure Portal, open your newly created app registration.</span></span>
1. <span data-ttu-id="a01ca-122">从菜单中选择 " **身份验证** "。</span><span class="sxs-lookup"><span data-stu-id="a01ca-122">From the menu, choose **Authentication**.</span></span>
1. <span data-ttu-id="a01ca-123">在 " **隐式授予** " 部分，启用 " **访问令牌** " 和 " **ID 令牌** " 选项。</span><span class="sxs-lookup"><span data-stu-id="a01ca-123">In the **Implicit grant** section, enable both **Access tokens** and **ID tokens** options.</span></span>
1. <span data-ttu-id="a01ca-124">通过选择 " **保存** " 按钮确认更改。</span><span class="sxs-lookup"><span data-stu-id="a01ca-124">Confirm your changes by choosing the **Save** button.</span></span>

## <a name="next-steps"></a><span data-ttu-id="a01ca-125">后续步骤</span><span class="sxs-lookup"><span data-stu-id="a01ca-125">Next steps</span></span>

- <span data-ttu-id="a01ca-126">[构建 web 应用程序](./build-a-web-app.md) (vanilla JavaScript) </span><span class="sxs-lookup"><span data-stu-id="a01ca-126">[Build a web application](./build-a-web-app.md) (vanilla JavaScript)</span></span>
- [<span data-ttu-id="a01ca-127">构建 Microsoft Teams 选项卡</span><span class="sxs-lookup"><span data-stu-id="a01ca-127">Build a Microsoft Teams tab</span></span>](./build-a-microsoft-teams-tab.md)
- [<span data-ttu-id="a01ca-128">将此工具包与响应结合使用</span><span class="sxs-lookup"><span data-stu-id="a01ca-128">Use the Toolkit with React</span></span>](./use-toolkit-with-react.md)
- [<span data-ttu-id="a01ca-129">使用具有角度的工具包</span><span class="sxs-lookup"><span data-stu-id="a01ca-129">Use the Toolkit with Angular</span></span>](./use-toolkit-with-angular.md)
