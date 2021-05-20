---
title: MSAL 2 提供程序
description: MSAL 2 提供程序使用 msal-browser 登录用户并获取令牌以用于 Microsoft Graph
localization_priority: Normal
author: amrutha95
ms.openlocfilehash: f583845f5c1929669242323501d08fa4a861197e
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579799"
---
# <a name="msal-2--provider"></a><span data-ttu-id="d5e72-103">MSAL 2 提供程序</span><span class="sxs-lookup"><span data-stu-id="d5e72-103">MSAL 2  provider</span></span>

<span data-ttu-id="d5e72-104">MSAL 2 提供程序使用[msal-browser](https://github.com/AzureAD/microsoft-authentication-library-for-js/tree/dev/lib/msal-browser)登录用户并获取与 Microsoft Graph 一Graph。</span><span class="sxs-lookup"><span data-stu-id="d5e72-104">The MSAL 2 provider uses [msal-browser](https://github.com/AzureAD/microsoft-authentication-library-for-js/tree/dev/lib/msal-browser) to sign in users and acquire tokens to use with Microsoft Graph.</span></span>
<span data-ttu-id="d5e72-105">若要了解更多信息，请参阅 [提供程序](./providers.md)。</span><span class="sxs-lookup"><span data-stu-id="d5e72-105">To learn more, see [providers](./providers.md).</span></span>

## <a name="get-started"></a><span data-ttu-id="d5e72-106">入门</span><span class="sxs-lookup"><span data-stu-id="d5e72-106">Get started</span></span>

<span data-ttu-id="d5e72-107">可以使用 HTML 或 JavaScript 初始化 MSAL 2.0 提供程序。</span><span class="sxs-lookup"><span data-stu-id="d5e72-107">You can initialize the MSAL 2.0 provider in HTML or JavaScript.</span></span>

### <a name="initialize-in-your-html-page"></a><span data-ttu-id="d5e72-108">在 HTML 页中初始化</span><span class="sxs-lookup"><span data-stu-id="d5e72-108">Initialize in your HTML page</span></span>

<span data-ttu-id="d5e72-109">使用 HTML 初始化 MSAL 2 提供程序是创建新提供程序的最简单方法。</span><span class="sxs-lookup"><span data-stu-id="d5e72-109">Initializing the MSAL 2 provider in HTML is the simplest way to create a new provider.</span></span> <span data-ttu-id="d5e72-110">使用该 `mgt-msal2-provider` 组件设置 **client-id** 和其他属性。</span><span class="sxs-lookup"><span data-stu-id="d5e72-110">Use the `mgt-msal2-provider` component to set the **client-id** and other properties.</span></span> <span data-ttu-id="d5e72-111">这将创建一 `PublicClientApplication` 个将用于所有身份验证和获取令牌的新实例。</span><span class="sxs-lookup"><span data-stu-id="d5e72-111">This will create a new `PublicClientApplication` instance that will be used for all authentication and acquiring tokens.</span></span>

```html
    <mgt-msal2-provider client-id="<YOUR_CLIENT_ID>"
                        login-type="redirect/popup" 
                        scopes="user.read,people.read" 
                        redirect-uri="https://my.redirect/uri" 
                        authority=""> 
    </mgt-msal2-provider> 
```

| <span data-ttu-id="d5e72-112">属性</span><span class="sxs-lookup"><span data-stu-id="d5e72-112">Attribute</span></span>    | <span data-ttu-id="d5e72-113">说明</span><span class="sxs-lookup"><span data-stu-id="d5e72-113">Description</span></span>                                                                                                                                                                                                                                                           |
|--------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="d5e72-114">client-id</span><span class="sxs-lookup"><span data-stu-id="d5e72-114">client-id</span></span>    | <span data-ttu-id="d5e72-115">字符串客户端 ID (创建应用/客户端 ID) 。</span><span class="sxs-lookup"><span data-stu-id="d5e72-115">String client ID (see Creating an app/client ID).</span></span> <span data-ttu-id="d5e72-116">必填。</span><span class="sxs-lookup"><span data-stu-id="d5e72-116">Required.</span></span>                                                                                                                                                                                                           |
| <span data-ttu-id="d5e72-117">login-type</span><span class="sxs-lookup"><span data-stu-id="d5e72-117">login-type</span></span>   | <span data-ttu-id="d5e72-118">和 之间的 `redirect` `popup` 枚举 - 默认值为 `redirect` 。</span><span class="sxs-lookup"><span data-stu-id="d5e72-118">Enumeration between `redirect` and `popup` - default value is `redirect`.</span></span> <span data-ttu-id="d5e72-119">可选。</span><span class="sxs-lookup"><span data-stu-id="d5e72-119">Optional.</span></span>                                                                                                                                                                                   |
| <span data-ttu-id="d5e72-120">scopes</span><span class="sxs-lookup"><span data-stu-id="d5e72-120">scopes</span></span>       | <span data-ttu-id="d5e72-121">用户登录时必须同意的范围的逗号分隔字符串。</span><span class="sxs-lookup"><span data-stu-id="d5e72-121">Comma separated strings for scopes the user must consent to on sign in.</span></span> <span data-ttu-id="d5e72-122">可选。</span><span class="sxs-lookup"><span data-stu-id="d5e72-122">Optional.</span></span>                                                                                                                                                                                     |
| <span data-ttu-id="d5e72-123">authority</span><span class="sxs-lookup"><span data-stu-id="d5e72-123">authority</span></span>    | <span data-ttu-id="d5e72-124">颁发机构字符串 - 默认为公共颁发机构。</span><span class="sxs-lookup"><span data-stu-id="d5e72-124">Authority string - default is the common authority.</span></span> <span data-ttu-id="d5e72-125">对于单租户应用，请使用租户 ID 或租户名称。</span><span class="sxs-lookup"><span data-stu-id="d5e72-125">For single-tenant apps, use your tenant ID or tenant name.</span></span> <span data-ttu-id="d5e72-126">例如， `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` `https://login.microsoftonline.com/[your-tenant-id]` 或 。</span><span class="sxs-lookup"><span data-stu-id="d5e72-126">For example, `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` or `https://login.microsoftonline.com/[your-tenant-id]`.</span></span> <span data-ttu-id="d5e72-127">可选。</span><span class="sxs-lookup"><span data-stu-id="d5e72-127">Optional.</span></span> |
| <span data-ttu-id="d5e72-128">redirect-uri</span><span class="sxs-lookup"><span data-stu-id="d5e72-128">redirect-uri</span></span> | <span data-ttu-id="d5e72-129">重定向 URI 字符串 - 默认情况下，使用当前窗口 URI。</span><span class="sxs-lookup"><span data-stu-id="d5e72-129">Redirect URI string - by default the current window URI is used.</span></span> <span data-ttu-id="d5e72-130">可选。</span><span class="sxs-lookup"><span data-stu-id="d5e72-130">Optional.</span></span>                                                                                                                                                                                            |
| <span data-ttu-id="d5e72-131">提示</span><span class="sxs-lookup"><span data-stu-id="d5e72-131">prompt</span></span>       | <span data-ttu-id="d5e72-132">用于登录的提示类型，介于 ```SELECT_ACCOUNT``` 和 ```CONSENT``` 之间 ```LOGIN``` 。</span><span class="sxs-lookup"><span data-stu-id="d5e72-132">Type of prompt to use for login, between ```SELECT_ACCOUNT```, ```CONSENT``` and ```LOGIN```.</span></span> <span data-ttu-id="d5e72-133">默认值为“```SELECT_ACCOUNT```”。</span><span class="sxs-lookup"><span data-stu-id="d5e72-133">Default is ```SELECT_ACCOUNT```.</span></span> <span data-ttu-id="d5e72-134">可选。</span><span class="sxs-lookup"><span data-stu-id="d5e72-134">Optional.</span></span>

### <a name="initialize-in-javascript"></a><span data-ttu-id="d5e72-135">在 JavaScript 中初始化</span><span class="sxs-lookup"><span data-stu-id="d5e72-135">Initialize in JavaScript</span></span>

<span data-ttu-id="d5e72-136">可以通过在 JavaScript 中初始化提供程序来提供更多选项。</span><span class="sxs-lookup"><span data-stu-id="d5e72-136">You can provide more options by initializing the provider in JavaScript.</span></span>

```ts
    import {Providers, LoginType} from '@microsoft/mgt-element';
    import {Msal2Provider, PromptType} from '@microsoft/mgt-msal2-provider';

    // initialize the auth provider globally
    Providers.globalProvider = new Msal2Provider({
      clientId: 'REPLACE_WITH_CLIENTID',
      scopes?: string[],
      authority?: string,
      redirectUri?: string,
      loginType?: LoginType, // LoginType.Popup or LoginType.Redirect (redirect is default)
      prompt?: PromptType, // PromptType.CONSENT, PromptType.LOGIN or PromptType.SELECT_ACCOUNT
      sid?: string, // Session ID
      loginHint?: string,
      domainHint?: string,
      options?: Configuration // msal js Configuration object
    });
```

## <a name="creating-an-appclient-id"></a><span data-ttu-id="d5e72-137">创建应用/客户端 ID</span><span class="sxs-lookup"><span data-stu-id="d5e72-137">Creating an app/client ID</span></span>

<span data-ttu-id="d5e72-138">若要详细了解如何注册应用和获取客户端 ID，请参阅创建Azure Active Directory[应用](../get-started/add-aad-app-registration.md)。</span><span class="sxs-lookup"><span data-stu-id="d5e72-138">For details about how to register an app and get a client ID, see [Create an Azure Active Directory app](../get-started/add-aad-app-registration.md).</span></span>

## <a name="difference-between-msal2provider-and-msalprovider"></a><span data-ttu-id="d5e72-139">Msal2Provider 和 MsalProvider 的区别</span><span class="sxs-lookup"><span data-stu-id="d5e72-139">Difference between Msal2Provider and MsalProvider</span></span>
<span data-ttu-id="d5e72-140">尽管用法非常相似，但 MsalProvider 和 Msal2Provider 是在不同的 OAuth 流上构建的。</span><span class="sxs-lookup"><span data-stu-id="d5e72-140">Although the usage is very similar, MsalProvider and Msal2Provider are built on top of different OAuth flows.</span></span> <span data-ttu-id="d5e72-141">MsalProvider 基于实现 OAuth2.0 [](/azure/active-directory/develop/v2-oauth2-implicit-grant-flow)隐式MSAL.js构建于 Flow。</span><span class="sxs-lookup"><span data-stu-id="d5e72-141">MsalProvider is built on top of MSAL.js, which implements the OAuth2.0 [Implicit Grant Flow](/azure/active-directory/develop/v2-oauth2-implicit-grant-flow).</span></span> <span data-ttu-id="d5e72-142">Msal2Provider 基于[msal-browser](https://github.com/AzureAD/microsoft-authentication-library-for-js/tree/dev/lib/msal-browser)构建，它使用 PKCE 实现 OAuth 2.0 授权[Flow](/azure/active-directory/develop/v2-oauth2-auth-code-flow)代码。</span><span class="sxs-lookup"><span data-stu-id="d5e72-142">Msal2Provider is built on top of [msal-browser](https://github.com/AzureAD/microsoft-authentication-library-for-js/tree/dev/lib/msal-browser), which implements the OAuth 2.0 [Authorization Code Flow](/azure/active-directory/develop/v2-oauth2-auth-code-flow) with PKCE.</span></span>
<span data-ttu-id="d5e72-143">授权代码Flow Web 应用程序的隐式授权Flow，因此我们建议使用 MSAL2Provider 而不是 MSALProvider。</span><span class="sxs-lookup"><span data-stu-id="d5e72-143">Authorization Code Flow is deemed more secure than Implicit Grant Flow for web applications, so we recommend usage of MSAL2Provider over MSALProvider.</span></span> <span data-ttu-id="d5e72-144">有关与隐式授予流相关的安全问题的详细信息，请参阅 [隐式流的缺点](https://tools.ietf.org/html/draft-ietf-oauth-browser-based-apps-04#section-9.8.6)。</span><span class="sxs-lookup"><span data-stu-id="d5e72-144">For details about security issues related to implicit grant flow, see [Disadvantages of the implicit flow](https://tools.ietf.org/html/draft-ietf-oauth-browser-based-apps-04#section-9.8.6).</span></span>

## <a name="migrating-from-msal-provider-to-msal-2-provider"></a><span data-ttu-id="d5e72-145">从 MSAL 提供程序迁移到 MSAL 2 提供程序</span><span class="sxs-lookup"><span data-stu-id="d5e72-145">Migrating from MSAL Provider to MSAL 2 Provider</span></span>
<span data-ttu-id="d5e72-146">若要将使用 MSAL 提供程序的应用程序迁移到 MSAL 2 提供程序：</span><span class="sxs-lookup"><span data-stu-id="d5e72-146">To migrate an application that's using MSAL provider to the MSAL 2 Provider:</span></span>
1. <span data-ttu-id="d5e72-147">转到 Azure 门户，位于 https://portal.azure.com 。</span><span class="sxs-lookup"><span data-stu-id="d5e72-147">Go to the Azure portal at https://portal.azure.com.</span></span>
1. <span data-ttu-id="d5e72-148">从菜单中，选择 **"Azure Active Directory"。**</span><span class="sxs-lookup"><span data-stu-id="d5e72-148">From the menu, select **Azure Active Directory**.</span></span>
1. <span data-ttu-id="d5e72-149">从"Azure Active Directory"菜单中，选择 **"应用注册"。**</span><span class="sxs-lookup"><span data-stu-id="d5e72-149">From the Azure Active Directory menu, select **App registrations**.</span></span>
1. <span data-ttu-id="d5e72-150">选择当前使用的应用的应用注册。</span><span class="sxs-lookup"><span data-stu-id="d5e72-150">Select the app registration of the app that you're currently using.</span></span> 
1. <span data-ttu-id="d5e72-151">转到左侧 **菜单** 上的"身份验证"。</span><span class="sxs-lookup"><span data-stu-id="d5e72-151">Go to **Authentication** on the left menu.</span></span>
1. <span data-ttu-id="d5e72-152">在 **"平台配置"** 下，单击 **"添加平台"，** 然后选择 **"单页应用程序"。**</span><span class="sxs-lookup"><span data-stu-id="d5e72-152">Under **Platform configurations**, click on **Add a platform** and select **Single-page Application**.</span></span>
1. <span data-ttu-id="d5e72-153">删除当前在 **Web** 下注册的所有重定向 URI，并改为将它们添加到 **单页应用程序 下**。</span><span class="sxs-lookup"><span data-stu-id="d5e72-153">Remove all the redirect URIs that you have currently registered under **Web**, and instead add them under **Single-page application**.</span></span>
1. <span data-ttu-id="d5e72-154">在你的代码中，将 MSALProvider 替换为 MSAL2Provider。</span><span class="sxs-lookup"><span data-stu-id="d5e72-154">In your code, replace MSALProvider with MSAL2Provider.</span></span>

    <span data-ttu-id="d5e72-155">如果要在 JS/TS 代码中初始化提供程序，请按照以下步骤操作：</span><span class="sxs-lookup"><span data-stu-id="d5e72-155">If you are initializing your provider in the JS/TS code, follow these steps:</span></span>
    
    <span data-ttu-id="d5e72-156">将 的 import 语句 ```mgt-msal-provider``` 替换为</span><span class="sxs-lookup"><span data-stu-id="d5e72-156">Replace the import statement for ```mgt-msal-provider``` with</span></span> 
    ```ts 
    import {Msal2Provider, PromptType} from '@microsoft/mgt-msal2-provider';
    ```

    <span data-ttu-id="d5e72-157">将 MsalProvider 的初始化替换为</span><span class="sxs-lookup"><span data-stu-id="d5e72-157">Replace the initialization of MsalProvider with</span></span>
    ```ts
    Providers.globalProvider = new Msal2Provider({ 
      clientId: 'REPLACE_WITH_CLIENTID'
      ...
    })
    ```
    <span data-ttu-id="d5e72-158">如果以 HTML 格式初始化提供程序，请替换</span><span class="sxs-lookup"><span data-stu-id="d5e72-158">If you are initializing the provider in HTML, replace</span></span> 
    ```html
    <mgt-msal-provider client-id="" ... ></mgt-msal-provider>
    ``` 
    <span data-ttu-id="d5e72-159">with</span><span class="sxs-lookup"><span data-stu-id="d5e72-159">with</span></span> 
    ```html
    <mgt-msal2-provider  client-id="" ... ></mgt-msal2-provider>
     ```
    <span data-ttu-id="d5e72-160">有关详细信息，请参阅[HTML 页面中的 Initialize。](#initialize-in-your-html-page)</span><span class="sxs-lookup"><span data-stu-id="d5e72-160">For details, see [Initialize in your HTML page](#initialize-in-your-html-page).</span></span>
