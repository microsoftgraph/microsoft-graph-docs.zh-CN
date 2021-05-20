---
title: MSAL 提供商
description: MSAL 提供程序MSAL.js登录用户并获取令牌以与 Microsoft Graph
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: e612e11e7b1a26765175ba10097c8e54317e9e1d
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579758"
---
# <a name="msal-provider"></a><span data-ttu-id="3810f-103">MSAL 提供商</span><span class="sxs-lookup"><span data-stu-id="3810f-103">MSAL provider</span></span>

<span data-ttu-id="3810f-104">MSAL 提供程序[使用MSAL.js](https://github.com/AzureAD/microsoft-authentication-library-for-js)登录用户并获取与 Microsoft Graph 一Graph。</span><span class="sxs-lookup"><span data-stu-id="3810f-104">The MSAL provider uses [MSAL.js](https://github.com/AzureAD/microsoft-authentication-library-for-js) to sign in users and acquire tokens to use with Microsoft Graph.</span></span>

<span data-ttu-id="3810f-105">若要了解更多信息，请参阅 [提供程序](./providers.md)。</span><span class="sxs-lookup"><span data-stu-id="3810f-105">To learn more, see [providers](./providers.md).</span></span>

## <a name="get-started"></a><span data-ttu-id="3810f-106">入门</span><span class="sxs-lookup"><span data-stu-id="3810f-106">Get started</span></span>

<span data-ttu-id="3810f-107">可以使用 HTML 或 JavaScript 初始化 MSAL 提供程序。</span><span class="sxs-lookup"><span data-stu-id="3810f-107">You can initialize the MSAL provider in HTML or JavaScript.</span></span>

### <a name="initialize-in-your-html-page"></a><span data-ttu-id="3810f-108">在 HTML 页中初始化</span><span class="sxs-lookup"><span data-stu-id="3810f-108">Initialize in your HTML page</span></span>

<span data-ttu-id="3810f-109">使用 HTML 初始化 MSAL 提供程序是创建新提供程序的最简单方法。</span><span class="sxs-lookup"><span data-stu-id="3810f-109">Initializing the MSAL provider in HTML is the simplest way to create a new provider.</span></span> <span data-ttu-id="3810f-110">使用该 `mgt-msal-provider` 组件设置 **client-id** 和其他属性。</span><span class="sxs-lookup"><span data-stu-id="3810f-110">Use the `mgt-msal-provider` component to set the **client-id** and other properties.</span></span> <span data-ttu-id="3810f-111">这将创建一 `UserAgentApplication` 个将用于所有身份验证和获取令牌的新实例。</span><span class="sxs-lookup"><span data-stu-id="3810f-111">This will create a new `UserAgentApplication` instance that will be used for all authentication and acquiring tokens.</span></span>

```html
<mgt-msal-provider client-id="<YOUR_CLIENT_ID>"
                   login-type="redirect/popup"
                   scopes="user.read,people.read"
                   redirect-uri="https://my.redirect/uri"
                   authority=""
                   domainHint="mydomain.com"
                   prompt="consent"></mgt-msal-provider>
```

| <span data-ttu-id="3810f-112">属性</span><span class="sxs-lookup"><span data-stu-id="3810f-112">Attribute</span></span>    | <span data-ttu-id="3810f-113">说明</span><span class="sxs-lookup"><span data-stu-id="3810f-113">Description</span></span>                                                                                                                                                                                                                                                           |
|--------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="3810f-114">client-id</span><span class="sxs-lookup"><span data-stu-id="3810f-114">client-id</span></span>    | <span data-ttu-id="3810f-115">字符串客户端 ID (创建应用/客户端 ID) 。</span><span class="sxs-lookup"><span data-stu-id="3810f-115">String client ID (see Creating an app/client ID).</span></span> <span data-ttu-id="3810f-116">必填。</span><span class="sxs-lookup"><span data-stu-id="3810f-116">Required.</span></span>                                                                                                                                                                                                           |
| <span data-ttu-id="3810f-117">login-type</span><span class="sxs-lookup"><span data-stu-id="3810f-117">login-type</span></span>   | <span data-ttu-id="3810f-118">和 之间的 `redirect` `popup` 枚举 - 默认值为 `redirect` 。</span><span class="sxs-lookup"><span data-stu-id="3810f-118">Enumeration between `redirect` and `popup` - default value is `redirect`.</span></span> <span data-ttu-id="3810f-119">可选。</span><span class="sxs-lookup"><span data-stu-id="3810f-119">Optional.</span></span>                                                                                                                                                                                   |
| <span data-ttu-id="3810f-120">scopes</span><span class="sxs-lookup"><span data-stu-id="3810f-120">scopes</span></span>       | <span data-ttu-id="3810f-121">用户登录时必须同意的范围的逗号分隔字符串。</span><span class="sxs-lookup"><span data-stu-id="3810f-121">Comma separated strings for scopes the user must consent to on sign in.</span></span> <span data-ttu-id="3810f-122">可选。</span><span class="sxs-lookup"><span data-stu-id="3810f-122">Optional.</span></span>                                                                                                                                                                                     |
| <span data-ttu-id="3810f-123">authority</span><span class="sxs-lookup"><span data-stu-id="3810f-123">authority</span></span>    | <span data-ttu-id="3810f-124">颁发机构字符串 - 默认为公共颁发机构。</span><span class="sxs-lookup"><span data-stu-id="3810f-124">Authority string - default is the common authority.</span></span> <span data-ttu-id="3810f-125">对于单租户应用，请使用租户 ID 或租户名称。</span><span class="sxs-lookup"><span data-stu-id="3810f-125">For single-tenant apps, use your tenant ID or tenant name.</span></span> <span data-ttu-id="3810f-126">例如， `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` `https://login.microsoftonline.com/[your-tenant-id]` 或 。</span><span class="sxs-lookup"><span data-stu-id="3810f-126">For example, `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` or `https://login.microsoftonline.com/[your-tenant-id]`.</span></span> <span data-ttu-id="3810f-127">可选。</span><span class="sxs-lookup"><span data-stu-id="3810f-127">Optional.</span></span> |
| <span data-ttu-id="3810f-128">redirect-uri</span><span class="sxs-lookup"><span data-stu-id="3810f-128">redirect-uri</span></span> | <span data-ttu-id="3810f-129">重定向 URI 字符串 - 默认情况下，使用当前窗口 URI。</span><span class="sxs-lookup"><span data-stu-id="3810f-129">Redirect URI string - by default the current window URI is used.</span></span> <span data-ttu-id="3810f-130">可选。</span><span class="sxs-lookup"><span data-stu-id="3810f-130">Optional.</span></span>                                                                                                                                                                                            |
| <span data-ttu-id="3810f-131">depends-on</span><span class="sxs-lookup"><span data-stu-id="3810f-131">depends-on</span></span>   | <span data-ttu-id="3810f-132">另一个优先级较高的提供程序组件的元素选择器字符串。</span><span class="sxs-lookup"><span data-stu-id="3810f-132">Element selector string of another higher priority provider component.</span></span> <span data-ttu-id="3810f-133">可选。</span><span class="sxs-lookup"><span data-stu-id="3810f-133">Optional.</span></span> 
| <span data-ttu-id="3810f-134">域提示</span><span class="sxs-lookup"><span data-stu-id="3810f-134">domain-hint</span></span>  | <span data-ttu-id="3810f-135">用于转发登录体验的域位置的查询字符串。</span><span class="sxs-lookup"><span data-stu-id="3810f-135">Query string of domain location for forwarding sign in experience.</span></span> <span data-ttu-id="3810f-136">可选。</span><span class="sxs-lookup"><span data-stu-id="3810f-136">Optional.</span></span>              
| <span data-ttu-id="3810f-137">提示</span><span class="sxs-lookup"><span data-stu-id="3810f-137">prompt</span></span> | <span data-ttu-id="3810f-138">选择登录所需的用户交互类型。</span><span class="sxs-lookup"><span data-stu-id="3810f-138">Selection for type of user interaction required to login.</span></span> <span data-ttu-id="3810f-139">有效选项包括：</span><span class="sxs-lookup"><span data-stu-id="3810f-139">Valid options include:</span></span> <ul><li><span data-ttu-id="3810f-140">`login` 强制用户在请求时输入凭据</span><span class="sxs-lookup"><span data-stu-id="3810f-140">`login` forces the user to enter credentials on request</span></span> </li><li><span data-ttu-id="3810f-141">`none` 无交互提示</span><span class="sxs-lookup"><span data-stu-id="3810f-141">`none` for no interactive prompt</span></span></li> <li><span data-ttu-id="3810f-142">`select_account` 将用户发送到帐户选取器</span><span class="sxs-lookup"><span data-stu-id="3810f-142">`select_account` to send the user to an account picker</span></span></li><li><span data-ttu-id="3810f-143">`consent` 将用户发送到 OAuth 同意对话框</span><span class="sxs-lookup"><span data-stu-id="3810f-143">`consent` to send the user to a OAuth consent dialog</span></span></li></ul> <span data-ttu-id="3810f-144">有关更多提示信息，请参阅本文 [中的MSAL.js](/azure/active-directory/develop/msal-js-prompt-behavior) 行为。</span><span class="sxs-lookup"><span data-stu-id="3810f-144">For more prompt information, see the [prompt behavior in MSAL.js](/azure/active-directory/develop/msal-js-prompt-behavior) article.</span></span> <span data-ttu-id="3810f-145">可选。</span><span class="sxs-lookup"><span data-stu-id="3810f-145">Optional.</span></span>                                                                                                                                                                            |


### <a name="initialize-in-javascript"></a><span data-ttu-id="3810f-146">在 JavaScript 中初始化</span><span class="sxs-lookup"><span data-stu-id="3810f-146">Initialize in JavaScript</span></span>

<span data-ttu-id="3810f-147">可以通过在 JavaScript 中初始化提供程序来提供更多选项。</span><span class="sxs-lookup"><span data-stu-id="3810f-147">You can provide more options by initializing the provider in JavaScript.</span></span>

```ts
import {Providers, MsalProvider} from '@microsoft/mgt'
import {UserAgentApplication} from "msal";

Providers.globalProvider = new MsalProvider(config: MsalConfig);
```

<span data-ttu-id="3810f-148">您可以通过两 `MsalProvider` 种方式配置构造函数参数，如以下各节所述。</span><span class="sxs-lookup"><span data-stu-id="3810f-148">You can configure the `MsalProvider` constructor parameter in two ways, as described in the following sections.</span></span>

#### <a name="provide-a-clientid-to-create-a-new-useragentapplication"></a><span data-ttu-id="3810f-149">提供 `clientId` 以创建新 `UserAgentApplication`</span><span class="sxs-lookup"><span data-stu-id="3810f-149">Provide a `clientId` to create a new `UserAgentApplication`</span></span>

<span data-ttu-id="3810f-150">此选项在用户负责Graph Toolkit身份验证时有意义。</span><span class="sxs-lookup"><span data-stu-id="3810f-150">This option makes sense when Graph Toolkit is responsible for all authentication in your application.</span></span>

```ts
interface MsalConfig {
  clientId: string;
  scopes?: string[];
  authority?: string;
  redirectUri?: string;
  loginType?: LoginType; // LoginType.Popup or LoginType.Redirect (redirect is default)
  loginHint?: string
  options?: Configuration; // msal js Configuration object
  domainHint?: string;
  prompt?: string; // "login", "none", "select_account", "consent"
}
```

#### <a name="pass-an-existing-useragentapplication-in-the-useragentapplication-property"></a><span data-ttu-id="3810f-151">在 属性 `UserAgentApplication` 中传递 `userAgentApplication` 现有的 。</span><span class="sxs-lookup"><span data-stu-id="3810f-151">Pass an existing `UserAgentApplication` in the `userAgentApplication` property.</span></span>

<span data-ttu-id="3810f-152">当你的应用使用 MSAL 功能（除了由 Microsoft 和其他 Microsoft 应用公开的功能Graph Toolkit `MsalProvider` 此功能。</span><span class="sxs-lookup"><span data-stu-id="3810f-152">Use this when your app uses MSAL functionality beyond what's exposed by the `MsalProvider` and other Microsoft Graph Toolkit features.</span></span> <span data-ttu-id="3810f-153">当框架自动实例化 并公开 时，这尤其适用;例如， `UserAgentApplication` 使用 [msal-angular 时](/azure/active-directory/develop/tutorial-v2-angular)。</span><span class="sxs-lookup"><span data-stu-id="3810f-153">This is particularly appropriate if a framework automatically instantiates and exposes a `UserAgentApplication` for you; for example, when using [msal-angular](/azure/active-directory/develop/tutorial-v2-angular).</span></span>

<span data-ttu-id="3810f-154">请务必了解使用此选项时发生冲突的机会。</span><span class="sxs-lookup"><span data-stu-id="3810f-154">Be sure to understand opportunities for collisions when using this option.</span></span> <span data-ttu-id="3810f-155">从本质上说，存在可以更改会话状态的风险，例如，让用户登录或同意其他 `MsalProvider` 范围。</span><span class="sxs-lookup"><span data-stu-id="3810f-155">By its very nature, there is a risk that the `MsalProvider` can change the state of a session, for example by having the user sign in or consent to additional scopes.</span></span> <span data-ttu-id="3810f-156">请确保应用和其他框架在状态中流畅地响应这些更改，或考虑改为使用 [自定义提供程序](./custom.md) 。</span><span class="sxs-lookup"><span data-stu-id="3810f-156">Make sure that your app and other frameworks respond gracefully to these changes in state, or consider using a [custom provider](./custom.md) instead.</span></span>

```ts
interface MsalConfig {
  userAgentApplication: UserAgentApplication;
  scopes?: string[];
  loginType?: LoginType; // LoginType.Popup or LoginType.Redirect (redirect is default)
  loginHint?: string;
}
```

<span data-ttu-id="3810f-157">若要详细了解MSAL.js以及初始化 MSAL 库时可以使用的其他选项，请参阅 [MSAL 文档](/azure/active-directory/develop/msal-js-initializing-client-applications)。</span><span class="sxs-lookup"><span data-stu-id="3810f-157">To learn more about MSAL.js and for additional options you can use when initializing the MSAL library, see the [MSAL documentation](/azure/active-directory/develop/msal-js-initializing-client-applications).</span></span>

## <a name="creating-an-appclient-id"></a><span data-ttu-id="3810f-158">创建应用/客户端 ID</span><span class="sxs-lookup"><span data-stu-id="3810f-158">Creating an app/client ID</span></span>

<span data-ttu-id="3810f-159">若要详细了解如何注册应用和获取客户端 ID，请参阅创建Azure Active Directory[应用](../get-started/add-aad-app-registration.md)。</span><span class="sxs-lookup"><span data-stu-id="3810f-159">For details about how to register an app and get a client ID, see [Create an Azure Active Directory app](../get-started/add-aad-app-registration.md).</span></span>
