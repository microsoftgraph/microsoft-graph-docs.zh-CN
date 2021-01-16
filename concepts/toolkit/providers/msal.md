---
title: MSAL 提供商
description: MSAL 提供程序MSAL.js登录用户并获取与 Microsoft Graph 一同使用的令牌
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 738e8ebcd24b3e7e528bdf0a1676dd54103ee2ea
ms.sourcegitcommit: 1d2adc4062c8e83d23768682cf66a731bccd313c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/16/2021
ms.locfileid: "49883023"
---
# <a name="msal-provider"></a><span data-ttu-id="69835-103">MSAL 提供商</span><span class="sxs-lookup"><span data-stu-id="69835-103">MSAL provider</span></span>

<span data-ttu-id="69835-104">MSAL [ 提供程序MSAL.js登录 ](https://github.com/AzureAD/microsoft-authentication-library-for-js) 用户并获取与 Microsoft Graph 一同使用的令牌。</span><span class="sxs-lookup"><span data-stu-id="69835-104">The MSAL provider uses [MSAL.js](https://github.com/AzureAD/microsoft-authentication-library-for-js) to sign in users and acquire tokens to use with Microsoft Graph.</span></span>

<span data-ttu-id="69835-105">若要了解更多信息，请参阅 [提供程序](./providers.md)。</span><span class="sxs-lookup"><span data-stu-id="69835-105">To learn more, see [providers](./providers.md).</span></span>

## <a name="get-started"></a><span data-ttu-id="69835-106">入门</span><span class="sxs-lookup"><span data-stu-id="69835-106">Get started</span></span>

<span data-ttu-id="69835-107">可以使用 HTML 或 JavaScript 初始化 MSAL 提供程序。</span><span class="sxs-lookup"><span data-stu-id="69835-107">You can initialize the MSAL provider in HTML or JavaScript.</span></span>

### <a name="initialize-in-your-html-page"></a><span data-ttu-id="69835-108">在 HTML 页中初始化</span><span class="sxs-lookup"><span data-stu-id="69835-108">Initialize in your HTML page</span></span>

<span data-ttu-id="69835-109">以 HTML 格式初始化 MSAL 提供程序是创建新提供程序的最简单方法。</span><span class="sxs-lookup"><span data-stu-id="69835-109">Initializing the MSAL provider in HTML is the simplest way to create a new provider.</span></span> <span data-ttu-id="69835-110">使用该 `mgt-msal-provider` 组件设置 **客户端 ID** 和其他属性。</span><span class="sxs-lookup"><span data-stu-id="69835-110">Use the `mgt-msal-provider` component to set the **client-id** and other properties.</span></span> <span data-ttu-id="69835-111">这将创建一 `UserAgentApplication` 个新实例，该实例将用于所有身份验证和获取令牌。</span><span class="sxs-lookup"><span data-stu-id="69835-111">This will create a new `UserAgentApplication` instance that will be used for all authentication and acquiring tokens.</span></span>

```html
<mgt-msal-provider client-id="<YOUR_CLIENT_ID>"
                   login-type="redirect/popup"
                   scopes="user.read,people.read"
                   redirect-uri="https://my.redirect/uri"
                   authority=""></mgt-msal-provider>
```

| <span data-ttu-id="69835-112">属性</span><span class="sxs-lookup"><span data-stu-id="69835-112">Attribute</span></span>    | <span data-ttu-id="69835-113">说明</span><span class="sxs-lookup"><span data-stu-id="69835-113">Description</span></span>                                                                                                                                                                                                                                                           |
|--------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="69835-114">client-id</span><span class="sxs-lookup"><span data-stu-id="69835-114">client-id</span></span>    | <span data-ttu-id="69835-115">字符串客户端 ID (请参阅创建应用/客户端 ID) 。</span><span class="sxs-lookup"><span data-stu-id="69835-115">String client ID (see Creating an app/client ID).</span></span> <span data-ttu-id="69835-116">必需。</span><span class="sxs-lookup"><span data-stu-id="69835-116">Required.</span></span>                                                                                                                                                                                                           |
| <span data-ttu-id="69835-117">login-type</span><span class="sxs-lookup"><span data-stu-id="69835-117">login-type</span></span>   | <span data-ttu-id="69835-118">与 - `redirect` `popup` 默认值之间的枚举为 `redirect` 。</span><span class="sxs-lookup"><span data-stu-id="69835-118">Enumeration between `redirect` and `popup` - default value is `redirect`.</span></span> <span data-ttu-id="69835-119">可选。</span><span class="sxs-lookup"><span data-stu-id="69835-119">Optional.</span></span>                                                                                                                                                                                   |
| <span data-ttu-id="69835-120">scopes</span><span class="sxs-lookup"><span data-stu-id="69835-120">scopes</span></span>       | <span data-ttu-id="69835-121">用户登录时必须同意的范围的逗号分隔字符串。</span><span class="sxs-lookup"><span data-stu-id="69835-121">Comma separated strings for scopes the user must consent to on sign in.</span></span> <span data-ttu-id="69835-122">可选。</span><span class="sxs-lookup"><span data-stu-id="69835-122">Optional.</span></span>                                                                                                                                                                                     |
| <span data-ttu-id="69835-123">authority</span><span class="sxs-lookup"><span data-stu-id="69835-123">authority</span></span>    | <span data-ttu-id="69835-124">颁发机构字符串 - 默认为公用颁发机构。</span><span class="sxs-lookup"><span data-stu-id="69835-124">Authority string - default is the common authority.</span></span> <span data-ttu-id="69835-125">对于单租户应用，请使用租户 ID 或租户名称。</span><span class="sxs-lookup"><span data-stu-id="69835-125">For single-tenant apps, use your tenant ID or tenant name.</span></span> <span data-ttu-id="69835-126">例如， `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` 或 `https://login.microsoftonline.com/[your-tenant-id]` 。</span><span class="sxs-lookup"><span data-stu-id="69835-126">For example, `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` or `https://login.microsoftonline.com/[your-tenant-id]`.</span></span> <span data-ttu-id="69835-127">可选。</span><span class="sxs-lookup"><span data-stu-id="69835-127">Optional.</span></span> |
| <span data-ttu-id="69835-128">redirect-uri</span><span class="sxs-lookup"><span data-stu-id="69835-128">redirect-uri</span></span> | <span data-ttu-id="69835-129">重定向 URI 字符串 - 默认情况下，使用当前窗口 URI。</span><span class="sxs-lookup"><span data-stu-id="69835-129">Redirect URI string - by default the current window URI is used.</span></span> <span data-ttu-id="69835-130">可选。</span><span class="sxs-lookup"><span data-stu-id="69835-130">Optional.</span></span>                                                                                                                                                                                            |
| <span data-ttu-id="69835-131">depends-on</span><span class="sxs-lookup"><span data-stu-id="69835-131">depends-on</span></span>   | <span data-ttu-id="69835-132">另一个优先级较高的提供程序组件的元素选择器字符串。</span><span class="sxs-lookup"><span data-stu-id="69835-132">Element selector string of another higher priority provider component.</span></span> <span data-ttu-id="69835-133">可选。</span><span class="sxs-lookup"><span data-stu-id="69835-133">Optional.</span></span>                                                                                                                                                                                      |

### <a name="initialize-in-javascript"></a><span data-ttu-id="69835-134">在 JavaScript 中初始化</span><span class="sxs-lookup"><span data-stu-id="69835-134">Initialize in JavaScript</span></span>

<span data-ttu-id="69835-135">可以通过在 JavaScript 中初始化提供程序提供更多选项。</span><span class="sxs-lookup"><span data-stu-id="69835-135">You can provide more options by initializing the provider in JavaScript.</span></span>

```ts
import {Providers, MsalProvider} from '@microsoft/mgt'
import {UserAgentApplication} from "msal";

Providers.globalProvider = new MsalProvider(config: MsalConfig);
```

<span data-ttu-id="69835-136">可以通过两 `MsalProvider` 种方式配置构造函数参数，如以下各节所述。</span><span class="sxs-lookup"><span data-stu-id="69835-136">You can configure the `MsalProvider` constructor parameter in two ways, as described in the following sections.</span></span>

#### <a name="provide-a-clientid-to-create-a-new-useragentapplication"></a><span data-ttu-id="69835-137">提供 `clientId` 用于创建新 `UserAgentApplication`</span><span class="sxs-lookup"><span data-stu-id="69835-137">Provide a `clientId` to create a new `UserAgentApplication`</span></span>

<span data-ttu-id="69835-138">当 Graph Toolkit负责应用程序中的所有身份验证时，此选项有意义。</span><span class="sxs-lookup"><span data-stu-id="69835-138">This option makes sense when Graph Toolkit is responsible for all authentication in your application.</span></span>

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

#### <a name="pass-an-existing-useragentapplication-in-the-useragentapplication-property"></a><span data-ttu-id="69835-139">传递属性 `UserAgentApplication` 中的 `userAgentApplication` 现有属性。</span><span class="sxs-lookup"><span data-stu-id="69835-139">Pass an existing `UserAgentApplication` in the `userAgentApplication` property.</span></span>

<span data-ttu-id="69835-140">当你的应用使用 MSAL 功能超过由 Microsoft Graph 和其他 Microsoft Graph 功能公开的功能 `MsalProvider` 时，Toolkit此功能。</span><span class="sxs-lookup"><span data-stu-id="69835-140">Use this when your app uses MSAL functionality beyond what's exposed by the `MsalProvider` and other Microsoft Graph Toolkit features.</span></span> <span data-ttu-id="69835-141">当框架自动实例化并公开 a 时，这尤其适用;例如，使用 `UserAgentApplication` [msal-angular 时](/azure/active-directory/develop/tutorial-v2-angular)。</span><span class="sxs-lookup"><span data-stu-id="69835-141">This is particularly appropriate if a framework automatically instantiates and exposes a `UserAgentApplication` for you; for example, when using [msal-angular](/azure/active-directory/develop/tutorial-v2-angular).</span></span>

<span data-ttu-id="69835-142">请务必了解使用此选项时发生冲突的机会。</span><span class="sxs-lookup"><span data-stu-id="69835-142">Be sure to understand opportunities for collisions when using this option.</span></span> <span data-ttu-id="69835-143">从本质上说，存在更改会话状态的风险，例如，让用户登录或同意其他 `MsalProvider` 范围。</span><span class="sxs-lookup"><span data-stu-id="69835-143">By its very nature, there is a risk that the `MsalProvider` can change the state of a session, for example by having the user sign in or consent to additional scopes.</span></span> <span data-ttu-id="69835-144">请确保你的应用和其他框架在状态中流畅地响应这些更改，或考虑改为使用 [自定义提供程序](./custom.md) 。</span><span class="sxs-lookup"><span data-stu-id="69835-144">Make sure that your app and other frameworks respond gracefully to these changes in state, or consider using a [custom provider](./custom.md) instead.</span></span>

```ts
interface MsalConfig {
  userAgentApplication: UserAgentApplication;
  scopes?: string[];
  loginType?: LoginType; // LoginType.Popup or LoginType.Redirect (redirect is default)
  loginHint?: string;
}
```

<span data-ttu-id="69835-145">若要详细了解MSAL.js以及初始化 MSAL 库时可以使用的其他选项，请参阅 [MSAL 文档](/azure/active-directory/develop/msal-js-initializing-client-applications)。</span><span class="sxs-lookup"><span data-stu-id="69835-145">To learn more about MSAL.js and for additional options you can use when initializing the MSAL library, see the [MSAL documentation](/azure/active-directory/develop/msal-js-initializing-client-applications).</span></span>

## <a name="creating-an-appclient-id"></a><span data-ttu-id="69835-146">创建应用/客户端 ID</span><span class="sxs-lookup"><span data-stu-id="69835-146">Creating an app/client ID</span></span>

<span data-ttu-id="69835-147">若要详细了解如何注册应用和获取客户端 ID，请参阅"创建[Azure Active Directory 应用"。](../get-started/add-aad-app-registration.md)</span><span class="sxs-lookup"><span data-stu-id="69835-147">For details about how to register an app and get a client ID, see [Create an Azure Active Directory app](../get-started/add-aad-app-registration.md).</span></span>