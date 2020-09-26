---
title: MSAL 提供商
description: MSAL 提供程序使用 MSAL.js 登录用户并获取令牌以用于 Microsoft Graph
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: c3c921cfa473e2001d2a150096741d2bddf39f10
ms.sourcegitcommit: 3fbc2249b307e8d3a9de18f22ef6911094ca272c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2020
ms.locfileid: "48288159"
---
# <a name="msal-provider"></a><span data-ttu-id="c76fe-103">MSAL 提供商</span><span class="sxs-lookup"><span data-stu-id="c76fe-103">MSAL provider</span></span>

<span data-ttu-id="c76fe-104">MSAL 提供程序使用 [MSAL.js](https://github.com/AzureAD/microsoft-authentication-library-for-js) 登录用户并获取令牌以用于 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="c76fe-104">The MSAL provider uses [MSAL.js](https://github.com/AzureAD/microsoft-authentication-library-for-js) to sign in users and acquire tokens to use with Microsoft Graph.</span></span>

<span data-ttu-id="c76fe-105">若要了解详细信息，请参阅 [提供程序](../providers.md)。</span><span class="sxs-lookup"><span data-stu-id="c76fe-105">To learn more, see [providers](../providers.md).</span></span>

## <a name="get-started"></a><span data-ttu-id="c76fe-106">入门</span><span class="sxs-lookup"><span data-stu-id="c76fe-106">Get started</span></span>

<span data-ttu-id="c76fe-107">您可以初始化 HTML 或 JavaScript 中的 MSAL 提供程序。</span><span class="sxs-lookup"><span data-stu-id="c76fe-107">You can initialize the MSAL provider in HTML or JavaScript.</span></span>

### <a name="initialize-in-your-html-page"></a><span data-ttu-id="c76fe-108">在 HTML 页面中初始化</span><span class="sxs-lookup"><span data-stu-id="c76fe-108">Initialize in your HTML page</span></span>

<span data-ttu-id="c76fe-109">若要在 HTML 中初始化 MSAL 提供程序，最简单的方法是创建新的提供程序。</span><span class="sxs-lookup"><span data-stu-id="c76fe-109">Initializing the MSAL provider in HTML is the simplest way to create a new provider.</span></span> <span data-ttu-id="c76fe-110">使用 `mgt-msal-provider` 组件设置 **客户端 id** 和其他属性。</span><span class="sxs-lookup"><span data-stu-id="c76fe-110">Use the `mgt-msal-provider` component to set the **client-id** and other properties.</span></span> <span data-ttu-id="c76fe-111">这将创建一个 `UserAgentApplication` 将用于所有身份验证和获取令牌的新实例。</span><span class="sxs-lookup"><span data-stu-id="c76fe-111">This will create a new `UserAgentApplication` instance that will be used for all authentication and acquiring tokens.</span></span>

```html
<mgt-msal-provider client-id="<YOUR_CLIENT_ID>"
                   login-type="redirect/popup"
                   scopes="user.read,people.read"
                   redirect-uri="https://my.redirect/uri"
                   authority=""></mgt-msal-provider>
```

| <span data-ttu-id="c76fe-112">属性</span><span class="sxs-lookup"><span data-stu-id="c76fe-112">Attribute</span></span>    | <span data-ttu-id="c76fe-113">说明</span><span class="sxs-lookup"><span data-stu-id="c76fe-113">Description</span></span>                                                                                                                                                                                                                                                           |
|--------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="c76fe-114">客户端 id</span><span class="sxs-lookup"><span data-stu-id="c76fe-114">client-id</span></span>    | <span data-ttu-id="c76fe-115">字符串客户端 ID (请参阅创建应用/客户端 ID) 。</span><span class="sxs-lookup"><span data-stu-id="c76fe-115">String client ID (see Creating an app/client ID).</span></span> <span data-ttu-id="c76fe-116">必需。</span><span class="sxs-lookup"><span data-stu-id="c76fe-116">Required.</span></span>                                                                                                                                                                                                           |
| <span data-ttu-id="c76fe-117">登录类型</span><span class="sxs-lookup"><span data-stu-id="c76fe-117">login-type</span></span>   | <span data-ttu-id="c76fe-118">`redirect`和 `popup` -默认值之间的枚举为 `redirect` 。</span><span class="sxs-lookup"><span data-stu-id="c76fe-118">Enumeration between `redirect` and `popup` - default value is `redirect`.</span></span> <span data-ttu-id="c76fe-119">可选。</span><span class="sxs-lookup"><span data-stu-id="c76fe-119">Optional.</span></span>                                                                                                                                                                                   |
| <span data-ttu-id="c76fe-120">scopes</span><span class="sxs-lookup"><span data-stu-id="c76fe-120">scopes</span></span>       | <span data-ttu-id="c76fe-121">用户必须同意登录时的作用域的逗号分隔字符串。</span><span class="sxs-lookup"><span data-stu-id="c76fe-121">Comma separated strings for scopes the user must consent to on sign in.</span></span> <span data-ttu-id="c76fe-122">可选。</span><span class="sxs-lookup"><span data-stu-id="c76fe-122">Optional.</span></span>                                                                                                                                                                                     |
| <span data-ttu-id="c76fe-123">监管</span><span class="sxs-lookup"><span data-stu-id="c76fe-123">authority</span></span>    | <span data-ttu-id="c76fe-124">颁发机构字符串-默认为常用证书颁发机构。</span><span class="sxs-lookup"><span data-stu-id="c76fe-124">Authority string - default is the common authority.</span></span> <span data-ttu-id="c76fe-125">对于单租户应用，请使用租户 ID 或租户名称。</span><span class="sxs-lookup"><span data-stu-id="c76fe-125">For single-tenant apps, use your tenant ID or tenant name.</span></span> <span data-ttu-id="c76fe-126">例如， `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` 或 `https://login.microsoftonline.com/[your-tenant-id]` 。</span><span class="sxs-lookup"><span data-stu-id="c76fe-126">For example, `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` or `https://login.microsoftonline.com/[your-tenant-id]`.</span></span> <span data-ttu-id="c76fe-127">可选。</span><span class="sxs-lookup"><span data-stu-id="c76fe-127">Optional.</span></span> |
| <span data-ttu-id="c76fe-128">重定向-uri</span><span class="sxs-lookup"><span data-stu-id="c76fe-128">redirect-uri</span></span> | <span data-ttu-id="c76fe-129">重定向 URI 字符串-默认情况下，使用当前窗口 URI。</span><span class="sxs-lookup"><span data-stu-id="c76fe-129">Redirect URI string - by default the current window URI is used.</span></span> <span data-ttu-id="c76fe-130">可选。</span><span class="sxs-lookup"><span data-stu-id="c76fe-130">Optional.</span></span>                                                                                                                                                                                            |
| <span data-ttu-id="c76fe-131">取决于</span><span class="sxs-lookup"><span data-stu-id="c76fe-131">depends-on</span></span>   | <span data-ttu-id="c76fe-132">另一个较高优先级提供程序组件的元素选择器字符串。</span><span class="sxs-lookup"><span data-stu-id="c76fe-132">Element selector string of another higher priority provider component.</span></span> <span data-ttu-id="c76fe-133">可选。</span><span class="sxs-lookup"><span data-stu-id="c76fe-133">Optional.</span></span>                                                                                                                                                                                      |

### <a name="initialize-in-javascript"></a><span data-ttu-id="c76fe-134">在 JavaScript 中初始化</span><span class="sxs-lookup"><span data-stu-id="c76fe-134">Initialize in JavaScript</span></span>

<span data-ttu-id="c76fe-135">您可以通过在 JavaScript 中初始化提供程序来提供更多选项。</span><span class="sxs-lookup"><span data-stu-id="c76fe-135">You can provide more options by initializing the provider in JavaScript.</span></span>

```ts
import {Providers, MsalProvider} from '@microsoft/mgt'
import {UserAgentApplication} from "msal";

Providers.globalProvider = new MsalProvider(config: MsalConfig);
```

<span data-ttu-id="c76fe-136">其中 MsalConfig 是：</span><span class="sxs-lookup"><span data-stu-id="c76fe-136">where MsalConfig is:</span></span>

```ts
interface MsalConfig {
  clientId: string;
  scopes?: string[];
  authority?: string;
  redirectUri?: string;
  loginType?: LoginType; // LoginType.Popup or LoginType.Redirect (redirect is default)
  loginHint?: string
  options?: Configuration; // msal js Configuration object
}
```

<span data-ttu-id="c76fe-137">您必须提供 `clientId` (才能创建新 `UserAgentApplication`) 。</span><span class="sxs-lookup"><span data-stu-id="c76fe-137">You must provide a `clientId` (to create a new `UserAgentApplication`).</span></span>

<span data-ttu-id="c76fe-138">若要详细了解 MSAL.js 以及在初始化 MSAL 库时可使用的其他选项，请参阅 [MSAL 文档](/azure/active-directory/develop/msal-js-initializing-client-applications)。</span><span class="sxs-lookup"><span data-stu-id="c76fe-138">To learn more about MSAL.js and for additional options you can use when initializing the MSAL library, see the [MSAL documentation](/azure/active-directory/develop/msal-js-initializing-client-applications).</span></span>

## <a name="creating-an-appclient-id"></a><span data-ttu-id="c76fe-139">创建应用/客户端 ID</span><span class="sxs-lookup"><span data-stu-id="c76fe-139">Creating an app/client ID</span></span>

<span data-ttu-id="c76fe-140">有关如何注册应用并获取客户端 ID 的详细信息，请参阅 [注册应用程序快速入门](/azure/active-directory/develop/quickstart-register-app)。</span><span class="sxs-lookup"><span data-stu-id="c76fe-140">For details about how to register an app and get a client ID, see the [Register an app quick start](/azure/active-directory/develop/quickstart-register-app).</span></span>

><span data-ttu-id="c76fe-141">**注意：** MSAL 仅支持 OAuth 的隐式流。</span><span class="sxs-lookup"><span data-stu-id="c76fe-141">**Note:** MSAL only supports the Implicit Flow for OAuth.</span></span> <span data-ttu-id="c76fe-142">请务必在 Azure 门户中的应用程序中启用隐式流， (默认情况下不启用它) 。</span><span class="sxs-lookup"><span data-stu-id="c76fe-142">Make sure to enable Implicit Flow in your application in the Azure Portal (it is not enabled by default).</span></span> <span data-ttu-id="c76fe-143">在 " **身份验证**" 下，找到 " **隐式授予** " 部分，然后选择 " **访问令牌** " 和 **ID 令牌**的复选框。</span><span class="sxs-lookup"><span data-stu-id="c76fe-143">Under **Authentication**, find the **Implicit grant** section and select the checkboxes for **Access tokens** and **ID tokens**.</span></span> <span data-ttu-id="c76fe-144">若要使用公共证书颁发机构，请 **在任何组织目录中设置帐户**。</span><span class="sxs-lookup"><span data-stu-id="c76fe-144">To use the common authority, set **Account in any organizational directory**.</span></span> <span data-ttu-id="c76fe-145">若要使用特定租户，请在 `authority` 初始化过程中设置。</span><span class="sxs-lookup"><span data-stu-id="c76fe-145">To use a specific tenant, set the `authority` during initialization.</span></span>