---
title: MSAL 提供程序
description: MSAL 提供程序使用 MSAL 来登录用户并获取令牌以用于 Microsoft Graph
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 84962c0df0be9012f09ba8a87e17dcd3954d6e22
ms.sourcegitcommit: 195fa0d441a49662e144323d37518dbba0c76fc7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2020
ms.locfileid: "43806011"
---
# <a name="msal-provider"></a><span data-ttu-id="d026d-103">MSAL 提供程序</span><span class="sxs-lookup"><span data-stu-id="d026d-103">MSAL provider</span></span>

<span data-ttu-id="d026d-104">MSAL 提供程序使用[MSAL](https://github.com/AzureAD/microsoft-authentication-library-for-js)来登录用户并获取令牌以用于 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="d026d-104">The MSAL Provider uses [MSAL.js](https://github.com/AzureAD/microsoft-authentication-library-for-js) to sign in users and acquire tokens to use with the Microsoft Graph.</span></span>

<span data-ttu-id="d026d-105">若要了解详细信息，请参阅[提供程序](../providers.md)。</span><span class="sxs-lookup"><span data-stu-id="d026d-105">To learn more, see [providers](../providers.md).</span></span>

## <a name="get-started"></a><span data-ttu-id="d026d-106">入门</span><span class="sxs-lookup"><span data-stu-id="d026d-106">Get started</span></span>

<span data-ttu-id="d026d-107">您可以初始化 HTML 或 JavaScript 中的 MSAL 提供程序。</span><span class="sxs-lookup"><span data-stu-id="d026d-107">You can initialize the MSAL provider in HTML or JavaScript.</span></span>

### <a name="initialize-in-your-html-page"></a><span data-ttu-id="d026d-108">在 HTML 页面中初始化</span><span class="sxs-lookup"><span data-stu-id="d026d-108">Initialize in your HTML page</span></span>

<span data-ttu-id="d026d-109">若要在 HTML 中初始化 MSAL 提供程序，最简单的方法是创建新的提供程序。</span><span class="sxs-lookup"><span data-stu-id="d026d-109">Initializing the MSAL provider in HTML is the simplest way to create a new provider.</span></span> <span data-ttu-id="d026d-110">使用`mgt-msal-provider`组件设置**客户端 id**和其他属性。</span><span class="sxs-lookup"><span data-stu-id="d026d-110">Use the `mgt-msal-provider` component to set the **client-id** and other properties.</span></span> <span data-ttu-id="d026d-111">这将创建一个将`UserAgentApplication`用于所有身份验证和获取令牌的新实例。</span><span class="sxs-lookup"><span data-stu-id="d026d-111">This will create a new `UserAgentApplication` instance that will be used for all authentication and acquiring tokens.</span></span>

```html
<mgt-msal-provider client-id="<YOUR_CLIENT_ID>"
                   login-type="redirect/popup"
                   scopes="user.read,people.read"
                   authority=""></mgt-msal-provider>
```

| <span data-ttu-id="d026d-112">属性</span><span class="sxs-lookup"><span data-stu-id="d026d-112">Attribute</span></span> | <span data-ttu-id="d026d-113">说明</span><span class="sxs-lookup"><span data-stu-id="d026d-113">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="d026d-114">客户端 id</span><span class="sxs-lookup"><span data-stu-id="d026d-114">client-id</span></span>   | <span data-ttu-id="d026d-115">字符串客户端 ID （请参阅创建应用/客户端 ID）。</span><span class="sxs-lookup"><span data-stu-id="d026d-115">String client ID (see Creating an app/client ID).</span></span> <span data-ttu-id="d026d-116">必需。</span><span class="sxs-lookup"><span data-stu-id="d026d-116">Required.</span></span>|
| <span data-ttu-id="d026d-117">登录类型</span><span class="sxs-lookup"><span data-stu-id="d026d-117">login-type</span></span>  | <span data-ttu-id="d026d-118">和`redirect` `popup` -默认值之间的枚举`redirect`为。</span><span class="sxs-lookup"><span data-stu-id="d026d-118">Enumeration between `redirect` and `popup` - default value is `redirect`.</span></span> <span data-ttu-id="d026d-119">可选。</span><span class="sxs-lookup"><span data-stu-id="d026d-119">Optional.</span></span> |
| <span data-ttu-id="d026d-120">scopes</span><span class="sxs-lookup"><span data-stu-id="d026d-120">scopes</span></span>  | <span data-ttu-id="d026d-121">用户必须同意登录时的作用域的逗号分隔字符串。</span><span class="sxs-lookup"><span data-stu-id="d026d-121">Comma separated strings for scopes the user must consent to on sign in.</span></span> <span data-ttu-id="d026d-122">可选。</span><span class="sxs-lookup"><span data-stu-id="d026d-122">Optional.</span></span>|
| <span data-ttu-id="d026d-123">监管</span><span class="sxs-lookup"><span data-stu-id="d026d-123">authority</span></span>  | <span data-ttu-id="d026d-124">颁发机构字符串-默认为常用证书颁发机构。</span><span class="sxs-lookup"><span data-stu-id="d026d-124">Authority string - default is the common authority.</span></span> <span data-ttu-id="d026d-125">对于单租户应用，请使用租户 ID 或租户名称。</span><span class="sxs-lookup"><span data-stu-id="d026d-125">For single-tenant apps, use your tenant ID or tenant name.</span></span> <span data-ttu-id="d026d-126">例如， `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com`或`https://login.microsoftonline.com/[your-tenant-id]`。</span><span class="sxs-lookup"><span data-stu-id="d026d-126">For example, `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` or `https://login.microsoftonline.com/[your-tenant-id]`.</span></span> <span data-ttu-id="d026d-127">可选。</span><span class="sxs-lookup"><span data-stu-id="d026d-127">Optional.</span></span>|
| <span data-ttu-id="d026d-128">取决于</span><span class="sxs-lookup"><span data-stu-id="d026d-128">depends-on</span></span> | <span data-ttu-id="d026d-129">另一个较高优先级提供程序组件的元素选择器字符串。</span><span class="sxs-lookup"><span data-stu-id="d026d-129">Element selector string of another higher priority provider component.</span></span> <span data-ttu-id="d026d-130">可选。</span><span class="sxs-lookup"><span data-stu-id="d026d-130">Optional.</span></span> |

### <a name="initialize-in-javascript"></a><span data-ttu-id="d026d-131">在 JavaScript 中初始化</span><span class="sxs-lookup"><span data-stu-id="d026d-131">Initialize in JavaScript</span></span>

<span data-ttu-id="d026d-132">您可以通过在 JavaScript 中初始化提供程序来提供更多选项。</span><span class="sxs-lookup"><span data-stu-id="d026d-132">You can provide more options by initializing the provider in JavaScript.</span></span>

```ts
import {Providers, MsalProvider} from '@microsoft/mgt'
import {UserAgentApplication} from "msal";

Providers.globalProvider = new MsalProvider(config: MsalConfig);
```

<span data-ttu-id="d026d-133">其中 MsalConfig 是：</span><span class="sxs-lookup"><span data-stu-id="d026d-133">where MsalConfig is:</span></span>

```ts
interface MsalConfig {
  clientId: string;
  scopes?: string[];
  authority?: string;
  loginType?: LoginType;
  options?: Configuration; // msal js Configuration object
}
```

<span data-ttu-id="d026d-134">您必须提供`clientId` （以创建新`UserAgentApplication`的）。</span><span class="sxs-lookup"><span data-stu-id="d026d-134">You must provide a `clientId` (to create a new `UserAgentApplication`).</span></span>

<span data-ttu-id="d026d-135">若要了解有关 MSAL 的详细信息以及在初始化 MSAL 库时可以使用的其他选项，请参阅[MSAL 文档](https://docs.microsoft.com/azure/active-directory/develop/msal-js-initializing-client-applications)。</span><span class="sxs-lookup"><span data-stu-id="d026d-135">To learn more about MSAL.js and for additional options you can use when initializing the MSAL library, see the [MSAL documentation](https://docs.microsoft.com/azure/active-directory/develop/msal-js-initializing-client-applications).</span></span>

## <a name="creating-an-appclient-id"></a><span data-ttu-id="d026d-136">创建应用/客户端 ID</span><span class="sxs-lookup"><span data-stu-id="d026d-136">Creating an app/client ID</span></span>

<span data-ttu-id="d026d-137">有关如何注册应用并获取客户端 ID 的详细信息，请参阅[注册应用程序快速入门](/azure/active-directory/develop/quickstart-register-app)。</span><span class="sxs-lookup"><span data-stu-id="d026d-137">For details about how to register an app and get a client ID, see the [Register an app quick start](/azure/active-directory/develop/quickstart-register-app).</span></span>

><span data-ttu-id="d026d-138">**注意：** MSAL 仅支持 OAuth 的隐式流。</span><span class="sxs-lookup"><span data-stu-id="d026d-138">**Note:** MSAL only supports the Implicit Flow for OAuth.</span></span> <span data-ttu-id="d026d-139">请确保在 Azure 门户中的应用程序中启用隐式流（默认情况下不启用）。</span><span class="sxs-lookup"><span data-stu-id="d026d-139">Make sure to enable Implicit Flow in your application in the Azure Portal (it is not enabled by default).</span></span> <span data-ttu-id="d026d-140">在 "**身份验证**" 下，找到 "**隐式授予**" 部分，然后选择 "**访问令牌**" 和**ID 令牌**的复选框。</span><span class="sxs-lookup"><span data-stu-id="d026d-140">Under **Authentication**, find the **Implicit grant** section and select the checkboxes for **Access tokens** and **ID tokens**.</span></span> <span data-ttu-id="d026d-141">若要使用公共证书颁发机构，请**在任何组织目录中设置帐户**。</span><span class="sxs-lookup"><span data-stu-id="d026d-141">To use the common authority, set **Account in any organizational directory**.</span></span> <span data-ttu-id="d026d-142">若要使用特定租户，请在`authority`初始化过程中设置。</span><span class="sxs-lookup"><span data-stu-id="d026d-142">To use a specific tenant, set the `authority` during initialization.</span></span>
