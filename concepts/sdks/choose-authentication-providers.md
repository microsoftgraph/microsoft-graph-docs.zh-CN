---
title: 选择 Microsoft Graph 身份验证提供程序
description: 了解如何为您的应用程序选择特定于方案的身份验证提供程序。
localization_priority: Normal
author: MichaelMainer
ms.openlocfilehash: 7975a2049ee16d89cfc9668babde091db7dd140e
ms.sourcegitcommit: 9cee9d8229fc84dd7ef97670ff27c145e1a78408
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/18/2019
ms.locfileid: "35778297"
---
# <a name="choose-a-microsoft-graph-authentication-provider-based-on-scenario"></a><span data-ttu-id="55e56-103">根据应用场景选择 Microsoft Graph 身份验证提供程序</span><span class="sxs-lookup"><span data-stu-id="55e56-103">Choose a Microsoft Graph authentication provider based on scenario</span></span>

<span data-ttu-id="55e56-104">身份验证提供程序实现使用 Microsoft 身份验证库 (MSAL) 获取令牌所需的代码;处理一些可能的错误, 如增量许可、过期密码和有条件访问等情况。, 然后设置 HTTP 请求授权标头。</span><span class="sxs-lookup"><span data-stu-id="55e56-104">Authentication providers implement the code required to acquire a token using the Microsoft Authentication Library (MSAL); handle a number of potential errors for cases like incremental consent, expired passwords, and conditional access; and then set the HTTP request authorization header.</span></span> <span data-ttu-id="55e56-105">下表列出了与不同[应用程序类型](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-app-types)的方案相匹配的提供程序集。</span><span class="sxs-lookup"><span data-stu-id="55e56-105">The following table lists the set of providers that match the scenarios for different [application types](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-app-types).</span></span>

|<span data-ttu-id="55e56-106">应用场景</span><span class="sxs-lookup"><span data-stu-id="55e56-106">Scenario</span></span> | <span data-ttu-id="55e56-107">流/授予</span><span class="sxs-lookup"><span data-stu-id="55e56-107">Flow/Grant</span></span> | <span data-ttu-id="55e56-108">受众</span><span class="sxs-lookup"><span data-stu-id="55e56-108">Audience</span></span> | <span data-ttu-id="55e56-109">提供程序</span><span class="sxs-lookup"><span data-stu-id="55e56-109">Provider</span></span>|
|--|--|--|--|
| [<span data-ttu-id="55e56-110">单页面应用程序</span><span class="sxs-lookup"><span data-stu-id="55e56-110">Single Page App</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/develop/scenario-spa-acquire-token)| | | |
| | <span data-ttu-id="55e56-111">隐式</span><span class="sxs-lookup"><span data-stu-id="55e56-111">Implicit</span></span> | <span data-ttu-id="55e56-112">委派的消费者/组织</span><span class="sxs-lookup"><span data-stu-id="55e56-112">Delegated Consumer/Org</span></span> |[<span data-ttu-id="55e56-113">隐式提供程序</span><span class="sxs-lookup"><span data-stu-id="55e56-113">Implicit Provider</span></span>](#ImplicitProvider) |
| [<span data-ttu-id="55e56-114">调用 web Api 的 web 应用程序</span><span class="sxs-lookup"><span data-stu-id="55e56-114">Web App that calls web APIs</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/develop/scenario-web-app-call-api-acquire-token) | | | |
| | <span data-ttu-id="55e56-115">授权代码</span><span class="sxs-lookup"><span data-stu-id="55e56-115">Authorization Code</span></span> | <span data-ttu-id="55e56-116">委派的消费者/组织</span><span class="sxs-lookup"><span data-stu-id="55e56-116">Delegated Consumer/Org</span></span> | [<span data-ttu-id="55e56-117">授权代码提供程序</span><span class="sxs-lookup"><span data-stu-id="55e56-117">Authorization Code Provider</span></span>](#AuthCodeProvider) |
| | <span data-ttu-id="55e56-118">客户端凭据</span><span class="sxs-lookup"><span data-stu-id="55e56-118">Client Credentials</span></span>  | <span data-ttu-id="55e56-119">仅限应用</span><span class="sxs-lookup"><span data-stu-id="55e56-119">App Only</span></span> | [<span data-ttu-id="55e56-120">客户端凭据提供程序</span><span class="sxs-lookup"><span data-stu-id="55e56-120">Client Credentials Provider</span></span>](#ClientCredentialsProvider) |
| [<span data-ttu-id="55e56-121">调用 web Api 的 Web API</span><span class="sxs-lookup"><span data-stu-id="55e56-121">Web API that calls web APIs</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/develop/scenario-web-api-call-api-acquire-token) | | | |
| | <span data-ttu-id="55e56-122">代表</span><span class="sxs-lookup"><span data-stu-id="55e56-122">On Behalf Of</span></span> | <span data-ttu-id="55e56-123">委派的消费者/组织</span><span class="sxs-lookup"><span data-stu-id="55e56-123">Delegated Consumer/Org</span></span> | [<span data-ttu-id="55e56-124">代表提供程序</span><span class="sxs-lookup"><span data-stu-id="55e56-124">On Behalf Of Provider</span></span>](#OnBehalfOfProvider) |
| | <span data-ttu-id="55e56-125">客户端凭据</span><span class="sxs-lookup"><span data-stu-id="55e56-125">Client Credentials</span></span>  | <span data-ttu-id="55e56-126">仅限应用</span><span class="sxs-lookup"><span data-stu-id="55e56-126">App Only</span></span> | [<span data-ttu-id="55e56-127">客户端凭据提供程序</span><span class="sxs-lookup"><span data-stu-id="55e56-127">Client Credentials Provider</span></span>](#ClientCredentialsProvider) |
| [<span data-ttu-id="55e56-128">调用 web Api 的桌面应用程序</span><span class="sxs-lookup"><span data-stu-id="55e56-128">Desktop app that calls web APIs</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/develop/scenario-desktop-acquire-token) | | | |
| | <span data-ttu-id="55e56-129">Interactive</span><span class="sxs-lookup"><span data-stu-id="55e56-129">Interactive</span></span> | <span data-ttu-id="55e56-130">委派的消费者/组织</span><span class="sxs-lookup"><span data-stu-id="55e56-130">Delegated Consumer/Org</span></span> | [<span data-ttu-id="55e56-131">交互式提供程序</span><span class="sxs-lookup"><span data-stu-id="55e56-131">Interactive Provider</span></span>](#InteractiveProvider) |
| | <span data-ttu-id="55e56-132">集成的 Windows</span><span class="sxs-lookup"><span data-stu-id="55e56-132">Integrated Windows</span></span> | <span data-ttu-id="55e56-133">委派的组织</span><span class="sxs-lookup"><span data-stu-id="55e56-133">Delegated Org</span></span> | [<span data-ttu-id="55e56-134">集成 Windows 提供程序</span><span class="sxs-lookup"><span data-stu-id="55e56-134">Integrated Windows Provider</span></span>](#IntegratedWindowsProvider) |
| | <span data-ttu-id="55e56-135">资源所有者</span><span class="sxs-lookup"><span data-stu-id="55e56-135">Resource Owner</span></span>  | <span data-ttu-id="55e56-136">委派的组织</span><span class="sxs-lookup"><span data-stu-id="55e56-136">Delegated Org</span></span> | [<span data-ttu-id="55e56-137">用户名/密码提供程序</span><span class="sxs-lookup"><span data-stu-id="55e56-137">Username / Password Provider</span></span>](#UsernamePasswordProvider) |
| | <span data-ttu-id="55e56-138">设备代码</span><span class="sxs-lookup"><span data-stu-id="55e56-138">Device Code</span></span>  | <span data-ttu-id="55e56-139">委派的组织</span><span class="sxs-lookup"><span data-stu-id="55e56-139">Delegated Org</span></span> | [<span data-ttu-id="55e56-140">设备代码提供程序</span><span class="sxs-lookup"><span data-stu-id="55e56-140">Device Code Provider</span></span>](#DeviceCodeProvider) |
| [<span data-ttu-id="55e56-141">守护程序应用</span><span class="sxs-lookup"><span data-stu-id="55e56-141">Daemon app</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/develop/scenario-daemon-acquire-token) | | | |
| | <span data-ttu-id="55e56-142">客户端凭据</span><span class="sxs-lookup"><span data-stu-id="55e56-142">Client Credentials</span></span>  | <span data-ttu-id="55e56-143">仅限应用</span><span class="sxs-lookup"><span data-stu-id="55e56-143">App Only</span></span> | [<span data-ttu-id="55e56-144">客户端凭据提供程序</span><span class="sxs-lookup"><span data-stu-id="55e56-144">Client Credentials Provider</span></span>](#ClientCredentialsProvider) |
| [<span data-ttu-id="55e56-145">调用 web Api 的移动应用程序</span><span class="sxs-lookup"><span data-stu-id="55e56-145">Mobile app that calls web APIs</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/develop/scenario-mobile-acquire-token) | | | |
| | <span data-ttu-id="55e56-146">Interactive</span><span class="sxs-lookup"><span data-stu-id="55e56-146">Interactive</span></span> | <span data-ttu-id="55e56-147">委派的消费者/组织</span><span class="sxs-lookup"><span data-stu-id="55e56-147">Delegated Consumer/Org</span></span> | [<span data-ttu-id="55e56-148">交互式提供程序</span><span class="sxs-lookup"><span data-stu-id="55e56-148">Interactive Provider</span></span>](#InteractiveProvider) |


## <a name="a-nameauthcodeproviderauthorization-code-provider"></a><span data-ttu-id="55e56-149"><a name="AuthCodeProvider"/>授权代码提供程序</span><span class="sxs-lookup"><span data-stu-id="55e56-149"><a name="AuthCodeProvider"/>Authorization code provider</span></span>

<span data-ttu-id="55e56-150">授权代码流使本机应用程序和 web 应用能够安全地获取用户名称中的令牌。</span><span class="sxs-lookup"><span data-stu-id="55e56-150">The authorization code flow enables native and web apps to securely obtain tokens in the name of the user.</span></span> <span data-ttu-id="55e56-151">若要了解详细信息, 请参阅[Microsoft identity platform 和 OAuth 2.0 授权代码流](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-auth-code-flow)。</span><span class="sxs-lookup"><span data-stu-id="55e56-151">To learn more, see [Microsoft identity platform and OAuth 2.0 authorization code flow](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-auth-code-flow).</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="55e56-152">C#</span><span class="sxs-lookup"><span data-stu-id="55e56-152">C#</span></span>](#tab/CS)

```csharp
IConfidentialClientApplication confidentialClientApplication = ConfidentialClientApplicationBuilder
    .Create(clientId)
    .WithRedirectUri(redirectUri)
    .WithClientSecret(clientSecret) // or .WithCertificate(certificate)
    .Build();

AuthorizationCodeProvider authProvider = new AuthorizationCodeProvider(confidentialClientApplication, scopes);  
```

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="55e56-153">Javascript</span><span class="sxs-lookup"><span data-stu-id="55e56-153">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="55e56-154">授权代码、客户端凭据和代表的 OAuth 流都要求您在此时实现自定义身份验证提供程序。</span><span class="sxs-lookup"><span data-stu-id="55e56-154">Authorization code, client credential, and on-behalf-of OAuth flows require that you implement a custom authentication provider at this time.</span></span> <span data-ttu-id="55e56-155">有关详细信息, 请参阅[使用自定义身份验证提供程序](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md)。</span><span class="sxs-lookup"><span data-stu-id="55e56-155">For more information, see [Using a custom authentication provider](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md).</span></span>

# <a name="javatabjava"></a>[<span data-ttu-id="55e56-156">Java</span><span class="sxs-lookup"><span data-stu-id="55e56-156">Java</span></span>](#tab/Java)

```java
AuthorizationCodeProvider authProvider = new AuthorizationCodeProvider(
                                                    clientId,
                                                    scopes,
                                                    authorizationCode,
                                                    redirectUri,
                                                    clientSecret);
```

# <a name="androidtabandroid"></a>[<span data-ttu-id="55e56-157">Android</span><span class="sxs-lookup"><span data-stu-id="55e56-157">Android</span></span>](#tab/Android)

<span data-ttu-id="55e56-158">不适用。</span><span class="sxs-lookup"><span data-stu-id="55e56-158">Not applicable.</span></span>

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="55e56-159">目标-C</span><span class="sxs-lookup"><span data-stu-id="55e56-159">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="55e56-160">不适用。</span><span class="sxs-lookup"><span data-stu-id="55e56-160">Not applicable.</span></span>

# <a name="phptabphp"></a>[<span data-ttu-id="55e56-161">PHP</span><span class="sxs-lookup"><span data-stu-id="55e56-161">PHP</span></span>](#tab/PHP)

<span data-ttu-id="55e56-162">尚不可用。</span><span class="sxs-lookup"><span data-stu-id="55e56-162">Not yet available.</span></span> <span data-ttu-id="55e56-163">如果这对你非常重要, 请支持或打开[Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)。</span><span class="sxs-lookup"><span data-stu-id="55e56-163">Please support or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="55e56-164">Ruby</span><span class="sxs-lookup"><span data-stu-id="55e56-164">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="55e56-165">尚不可用。</span><span class="sxs-lookup"><span data-stu-id="55e56-165">Not available, yet.</span></span> <span data-ttu-id="55e56-166">如果这对你非常重要, 请投票或打开[Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)。</span><span class="sxs-lookup"><span data-stu-id="55e56-166">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

##  <a name="a-nameclientcredentialsproviderclient-credentials-provider"></a><span data-ttu-id="55e56-167"><a name="ClientCredentialsProvider"/>客户端凭据提供程序</span><span class="sxs-lookup"><span data-stu-id="55e56-167"><a name="ClientCredentialsProvider"/>Client credentials provider</span></span>

<span data-ttu-id="55e56-168">客户端凭据流使服务应用程序可以在没有用户交互的情况下运行。</span><span class="sxs-lookup"><span data-stu-id="55e56-168">The client credential flow enables service applications to run without user interaction.</span></span> <span data-ttu-id="55e56-169">访问基于应用程序的标识。</span><span class="sxs-lookup"><span data-stu-id="55e56-169">Access is based on the identity of the application.</span></span> <span data-ttu-id="55e56-170">有关详细信息, 请参阅[Microsoft identity platform 和 OAuth 2.0 客户端凭据流](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)。</span><span class="sxs-lookup"><span data-stu-id="55e56-170">For more information, see [Microsoft identity platform and the OAuth 2.0 client credentials flow](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow).</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="55e56-171">C#</span><span class="sxs-lookup"><span data-stu-id="55e56-171">C#</span></span>](#tab/CS)

```csharp
IConfidentialClientApplication confidentialClientApplication = ConfidentialClientApplicationBuilder
    .Create(clientId)
    .WithTenantId(tenantID)
    .WithClientSecret(clientSecret)
    .Build();

ClientCredentialProvider authProvider = new ClientCredentialProvider(confidentialClientApplication);
```

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="55e56-172">Javascript</span><span class="sxs-lookup"><span data-stu-id="55e56-172">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="55e56-173">授权代码、客户端凭据和代表的 OAuth 流都要求您在此时实现自定义身份验证提供程序。</span><span class="sxs-lookup"><span data-stu-id="55e56-173">Authorization code, client credential, and on-behalf-of OAuth flows require that you implement a custom authentication provider at this time.</span></span> <span data-ttu-id="55e56-174">有关详细信息, 请参阅[使用自定义身份验证提供程序](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md)。</span><span class="sxs-lookup"><span data-stu-id="55e56-174">For more information, see [Using a custom authentication provider](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md).</span></span>

# <a name="javatabjava"></a>[<span data-ttu-id="55e56-175">Java</span><span class="sxs-lookup"><span data-stu-id="55e56-175">Java</span></span>](#tab/Java)

```java
ClientCredentialProvider authProvider = new ClientCredentialProvider(
                                                    clientId,
                                                    scopes,
                                                    clientSecret,
                                                    tenant,
                                                    endpoint);
```

# <a name="androidtabandroid"></a>[<span data-ttu-id="55e56-176">Android</span><span class="sxs-lookup"><span data-stu-id="55e56-176">Android</span></span>](#tab/Android)

<span data-ttu-id="55e56-177">不适用。</span><span class="sxs-lookup"><span data-stu-id="55e56-177">Not applicable.</span></span>

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="55e56-178">目标-C</span><span class="sxs-lookup"><span data-stu-id="55e56-178">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="55e56-179">不适用。</span><span class="sxs-lookup"><span data-stu-id="55e56-179">Not applicable.</span></span>

# <a name="phptabphp"></a>[<span data-ttu-id="55e56-180">PHP</span><span class="sxs-lookup"><span data-stu-id="55e56-180">PHP</span></span>](#tab/PHP)

<span data-ttu-id="55e56-181">尚不可用。</span><span class="sxs-lookup"><span data-stu-id="55e56-181">Not available, yet.</span></span> <span data-ttu-id="55e56-182">如果这对你非常重要, 请支持或打开[Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)。</span><span class="sxs-lookup"><span data-stu-id="55e56-182">Please support or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="55e56-183">Ruby</span><span class="sxs-lookup"><span data-stu-id="55e56-183">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="55e56-184">尚不可用。</span><span class="sxs-lookup"><span data-stu-id="55e56-184">Not available, yet.</span></span> <span data-ttu-id="55e56-185">如果这对你非常重要, 请支持或打开[Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)。</span><span class="sxs-lookup"><span data-stu-id="55e56-185">Please support or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

##  <a name="a-nameonbehalfofprovideron-behalf-of-provider"></a><span data-ttu-id="55e56-186"><a name="OnBehalfOfProvider"/>代表提供程序</span><span class="sxs-lookup"><span data-stu-id="55e56-186"><a name="OnBehalfOfProvider"/>On-behalf-of provider</span></span>

<span data-ttu-id="55e56-187">当应用程序调用在其中打开 Microsoft Graph API 的服务/web API 时, 代表流是适用的。</span><span class="sxs-lookup"><span data-stu-id="55e56-187">The on-behalf-of flow is applicable when your application calls a service/web API which in turns calls the Microsoft Graph API.</span></span> <span data-ttu-id="55e56-188">若要了解详细信息, 请阅读[Microsoft identity platform 和 OAuth 2.0 代表流](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow)</span><span class="sxs-lookup"><span data-stu-id="55e56-188">Learn more by reading [Microsoft identity platform and OAuth 2.0 On-Behalf-Of flow](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow)</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="55e56-189">C#</span><span class="sxs-lookup"><span data-stu-id="55e56-189">C#</span></span>](#tab/CS)

```csharp
IConfidentialClientApplication confidentialClientApplication = ConfidentialClientApplicationBuilder
    .Create(clientId)
    .WithRedirectUri(redirectUri)
    .WithClientSecret(clientSecret)
    .Build();

OnBehalfOfProvider authProvider = new OnBehalfOfProvider(confidentialClientApplication, scopes);
```

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="55e56-190">Javascript</span><span class="sxs-lookup"><span data-stu-id="55e56-190">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="55e56-191">授权代码、客户端凭据和代表的 OAuth 流都要求您在此时实现自定义身份验证提供程序。</span><span class="sxs-lookup"><span data-stu-id="55e56-191">Authorization code, client credential, and on-behalf-of OAuth flows require that you implement a custom authentication provider at this time.</span></span> <span data-ttu-id="55e56-192">有关详细信息, 请参阅[使用自定义身份验证提供程序](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md)。</span><span class="sxs-lookup"><span data-stu-id="55e56-192">Read [Using Custom Authentication Provider](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md) for more information.</span></span>

# <a name="javatabjava"></a>[<span data-ttu-id="55e56-193">Java</span><span class="sxs-lookup"><span data-stu-id="55e56-193">Java</span></span>](#tab/Java)

<span data-ttu-id="55e56-194">尚不可用。</span><span class="sxs-lookup"><span data-stu-id="55e56-194">Not yet available.</span></span> <span data-ttu-id="55e56-195">如果这对你非常重要, 请投票或打开[Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)。</span><span class="sxs-lookup"><span data-stu-id="55e56-195">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="androidtabandroid"></a>[<span data-ttu-id="55e56-196">Android</span><span class="sxs-lookup"><span data-stu-id="55e56-196">Android</span></span>](#tab/Android)

<span data-ttu-id="55e56-197">不适用。</span><span class="sxs-lookup"><span data-stu-id="55e56-197">Not applicable.</span></span>

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="55e56-198">目标-C</span><span class="sxs-lookup"><span data-stu-id="55e56-198">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="55e56-199">不适用。</span><span class="sxs-lookup"><span data-stu-id="55e56-199">Not applicable.</span></span>

# <a name="phptabphp"></a>[<span data-ttu-id="55e56-200">PHP</span><span class="sxs-lookup"><span data-stu-id="55e56-200">PHP</span></span>](#tab/PHP)

<span data-ttu-id="55e56-201">尚不可用。</span><span class="sxs-lookup"><span data-stu-id="55e56-201">Not yet available.</span></span> <span data-ttu-id="55e56-202">如果这对你非常重要, 请投票或打开[Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)。</span><span class="sxs-lookup"><span data-stu-id="55e56-202">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="55e56-203">Ruby</span><span class="sxs-lookup"><span data-stu-id="55e56-203">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="55e56-204">尚不可用。</span><span class="sxs-lookup"><span data-stu-id="55e56-204">Not yet available.</span></span> <span data-ttu-id="55e56-205">如果这对你非常重要, 请投票或打开[Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)。</span><span class="sxs-lookup"><span data-stu-id="55e56-205">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

## <a name="a-nameimplicitproviderimplicit-provider"></a><span data-ttu-id="55e56-206"><a name="ImplicitProvider"/>隐式提供程序</span><span class="sxs-lookup"><span data-stu-id="55e56-206"><a name="ImplicitProvider"/>Implicit provider</span></span>

<span data-ttu-id="55e56-207">隐式授予流在基于浏览器的应用程序中使用。</span><span class="sxs-lookup"><span data-stu-id="55e56-207">The implicit grant flow is used in browser-based applications.</span></span> <span data-ttu-id="55e56-208">有关详细信息, 请参阅[Microsoft identity platform 和隐式授予流](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-implicit-grant-flow)。</span><span class="sxs-lookup"><span data-stu-id="55e56-208">For more information, see [Microsoft identity platform and Implicit grant flow](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-implicit-grant-flow).</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="55e56-209">C#</span><span class="sxs-lookup"><span data-stu-id="55e56-209">C#</span></span>](#tab/CS)

<span data-ttu-id="55e56-210">不适用。</span><span class="sxs-lookup"><span data-stu-id="55e56-210">Not applicable.</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="55e56-211">Javascript</span><span class="sxs-lookup"><span data-stu-id="55e56-211">Javascript</span></span>](#tab/Javascript)

```javascript
const clientId = "your_client_id"; // Client Id of the registered application
const callback = (errorDesc, token, error, tokenType) => {};
// An Optional options for initializing the MSAL @see https://github.com/AzureAD/microsoft-authentication-library-for-js/wiki/MSAL-basics#configuration-options
const options = {
    redirectUri: "Your redirect URI",
};
const graphScopes = ["user.read", "mail.send"]; // An array of graph scopes

// Initialize the MSAL @see https://github.com/AzureAD/microsoft-authentication-library-for-js/wiki/MSAL-basics#initialization-of-msal
const userAgentApplication = new Msal.UserAgentApplication(clientId, undefined, callback, options);
const authProvider = new MicrosoftGraph.MSALAuthenticationProvider(userAgentApplication, graphScopes);

const options = {
    authProvider, // An instance created from previous step
};
const Client = MicrosoftGraph.Client;
const client = Client.initWithMiddleware(options);
```

# <a name="javatabjava"></a>[<span data-ttu-id="55e56-212">Java</span><span class="sxs-lookup"><span data-stu-id="55e56-212">Java</span></span>](#tab/Java)

<span data-ttu-id="55e56-213">不适用。</span><span class="sxs-lookup"><span data-stu-id="55e56-213">Not applicable.</span></span>

# <a name="androidtabandroid"></a>[<span data-ttu-id="55e56-214">Android</span><span class="sxs-lookup"><span data-stu-id="55e56-214">Android</span></span>](#tab/Android)

<span data-ttu-id="55e56-215">不适用。</span><span class="sxs-lookup"><span data-stu-id="55e56-215">Not applicable.</span></span>

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="55e56-216">目标-C</span><span class="sxs-lookup"><span data-stu-id="55e56-216">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="55e56-217">不适用。</span><span class="sxs-lookup"><span data-stu-id="55e56-217">Not applicable.</span></span>

# <a name="phptabphp"></a>[<span data-ttu-id="55e56-218">PHP</span><span class="sxs-lookup"><span data-stu-id="55e56-218">PHP</span></span>](#tab/PHP)

<span data-ttu-id="55e56-219">不适用。</span><span class="sxs-lookup"><span data-stu-id="55e56-219">Not applicable.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="55e56-220">Ruby</span><span class="sxs-lookup"><span data-stu-id="55e56-220">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="55e56-221">不适用。</span><span class="sxs-lookup"><span data-stu-id="55e56-221">Not applicable.</span></span>

---

##  <a name="a-namedevicecodeproviderdevice-code-provider"></a><span data-ttu-id="55e56-222"><a name="DeviceCodeProvider"/>设备代码提供程序</span><span class="sxs-lookup"><span data-stu-id="55e56-222"><a name="DeviceCodeProvider"/>Device code provider</span></span>

<span data-ttu-id="55e56-223">设备代码流允许通过其他设备登录设备。</span><span class="sxs-lookup"><span data-stu-id="55e56-223">The device code flow enables sign in to devices by way of another device.</span></span> <span data-ttu-id="55e56-224">有关详细信息, 请参阅[Microsoft identity platform 和 OAuth 2.0 设备代码流](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-device-code)。</span><span class="sxs-lookup"><span data-stu-id="55e56-224">For details, see [Microsoft identity platform and the OAuth 2.0 device code flow](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-device-code).</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="55e56-225">C#</span><span class="sxs-lookup"><span data-stu-id="55e56-225">C#</span></span>](#tab/CS)

```csharp
IPublicClientApplication publicClientApplication = PublicClientApplicationBuilder
            .Create(clientId)
            .Build();

Func<DeviceCodeResult, Task> deviceCodeReadyCallback = async dcr => await Console.Out.WriteLineAsync(dcr.Message);

DeviceCodeProvider authProvider = new DeviceCodeProvider(publicClientApplication, scopes, deviceCodeReadyCallback);
```

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="55e56-226">Javascript</span><span class="sxs-lookup"><span data-stu-id="55e56-226">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="55e56-227">尚不可用。</span><span class="sxs-lookup"><span data-stu-id="55e56-227">Not yet available.</span></span> <span data-ttu-id="55e56-228">如果这对你非常重要, 请投票或打开[Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)。</span><span class="sxs-lookup"><span data-stu-id="55e56-228">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="javatabjava"></a>[<span data-ttu-id="55e56-229">Java</span><span class="sxs-lookup"><span data-stu-id="55e56-229">Java</span></span>](#tab/Java)

<span data-ttu-id="55e56-230">尚不可用。</span><span class="sxs-lookup"><span data-stu-id="55e56-230">Not available, yet.</span></span> <span data-ttu-id="55e56-231">如果这对你非常重要, 请支持或打开[Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)。</span><span class="sxs-lookup"><span data-stu-id="55e56-231">Please support or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="androidtabandroid"></a>[<span data-ttu-id="55e56-232">Android</span><span class="sxs-lookup"><span data-stu-id="55e56-232">Android</span></span>](#tab/Android)

<span data-ttu-id="55e56-233">不适用。</span><span class="sxs-lookup"><span data-stu-id="55e56-233">Not applicable.</span></span>

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="55e56-234">目标-C</span><span class="sxs-lookup"><span data-stu-id="55e56-234">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="55e56-235">不适用。</span><span class="sxs-lookup"><span data-stu-id="55e56-235">Not applicable.</span></span>

# <a name="phptabphp"></a>[<span data-ttu-id="55e56-236">PHP</span><span class="sxs-lookup"><span data-stu-id="55e56-236">PHP</span></span>](#tab/PHP)

<span data-ttu-id="55e56-237">尚不可用。</span><span class="sxs-lookup"><span data-stu-id="55e56-237">Not yet available.</span></span> <span data-ttu-id="55e56-238">如果这对你非常重要, 请投票或打开[Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)。</span><span class="sxs-lookup"><span data-stu-id="55e56-238">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="55e56-239">Ruby</span><span class="sxs-lookup"><span data-stu-id="55e56-239">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="55e56-240">尚不可用。</span><span class="sxs-lookup"><span data-stu-id="55e56-240">Not yet available.</span></span> <span data-ttu-id="55e56-241">如果这对你非常重要, 请投票或打开[Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)。</span><span class="sxs-lookup"><span data-stu-id="55e56-241">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

##  <a name="a-nameintegratedwindowsproviderintegrated-windows-provider"></a><span data-ttu-id="55e56-242"><a name="IntegratedWindowsProvider"/>集成 Windows 提供程序</span><span class="sxs-lookup"><span data-stu-id="55e56-242"><a name="IntegratedWindowsProvider"/>Integrated Windows provider</span></span>

<span data-ttu-id="55e56-243">集成的 Windows 流为 Windows 计算机提供了一种在加入域时无提示地获取访问令牌的方法。</span><span class="sxs-lookup"><span data-stu-id="55e56-243">The integrated Windows flow provides a way for Windows computers to silently acquire an access token when they are domain joined.</span></span> <span data-ttu-id="55e56-244">有关详细信息, 请参阅[集成 Windows 身份验证](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Integrated-Windows-Authentication)。</span><span class="sxs-lookup"><span data-stu-id="55e56-244">For details, see [Integrated Windows authentication](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Integrated-Windows-Authentication).</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="55e56-245">C#</span><span class="sxs-lookup"><span data-stu-id="55e56-245">C#</span></span>](#tab/CS)

```csharp
IPublicClientApplication publicClientApplication = PublicClientApplicationBuilder
            .Create(clientId)
            .WithTenantId(tenantID)
            .Build();

IntegratedWindowsAuthenticationProvider authProvider = new IntegratedWindowsAuthenticationProvider(publicClientApplication, scopes);
```

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="55e56-246">Javascript</span><span class="sxs-lookup"><span data-stu-id="55e56-246">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="55e56-247">不适用。</span><span class="sxs-lookup"><span data-stu-id="55e56-247">Not applicable.</span></span>

# <a name="javatabjava"></a>[<span data-ttu-id="55e56-248">Java</span><span class="sxs-lookup"><span data-stu-id="55e56-248">Java</span></span>](#tab/Java)

<span data-ttu-id="55e56-249">不适用。</span><span class="sxs-lookup"><span data-stu-id="55e56-249">Not applicable.</span></span>

# <a name="androidtabandroid"></a>[<span data-ttu-id="55e56-250">Android</span><span class="sxs-lookup"><span data-stu-id="55e56-250">Android</span></span>](#tab/Android)

<span data-ttu-id="55e56-251">不适用。</span><span class="sxs-lookup"><span data-stu-id="55e56-251">Not applicable.</span></span>

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="55e56-252">目标-C</span><span class="sxs-lookup"><span data-stu-id="55e56-252">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="55e56-253">不适用。</span><span class="sxs-lookup"><span data-stu-id="55e56-253">Not applicable.</span></span>

# <a name="phptabphp"></a>[<span data-ttu-id="55e56-254">PHP</span><span class="sxs-lookup"><span data-stu-id="55e56-254">PHP</span></span>](#tab/PHP)

<span data-ttu-id="55e56-255">不适用。</span><span class="sxs-lookup"><span data-stu-id="55e56-255">Not applicable.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="55e56-256">Ruby</span><span class="sxs-lookup"><span data-stu-id="55e56-256">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="55e56-257">不适用。</span><span class="sxs-lookup"><span data-stu-id="55e56-257">Not applicable.</span></span>

---

##  <a name="a-nameinteractiveproviderinteractive-provider"></a><span data-ttu-id="55e56-258"><a name="InteractiveProvider"/>交互式提供程序</span><span class="sxs-lookup"><span data-stu-id="55e56-258"><a name="InteractiveProvider"/>Interactive provider</span></span>

<span data-ttu-id="55e56-259">移动应用程序 (Xamarin 和 UWP) 和桌面应用程序使用交互流, 以在用户的名称中调用 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="55e56-259">The interactive flow is used by mobile applications (Xamarin and UWP) and desktops applications to call Microsoft Graph in the name of a user.</span></span> <span data-ttu-id="55e56-260">有关详细信息, 请参阅[以交互方式获取令牌](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Acquiring-tokens-interactively)。</span><span class="sxs-lookup"><span data-stu-id="55e56-260">For details, see [Acquiring tokens interactively](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Acquiring-tokens-interactively).</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="55e56-261">C#</span><span class="sxs-lookup"><span data-stu-id="55e56-261">C#</span></span>](#tab/CS)

```csharp
IPublicClientApplication publicClientApplication = PublicClientApplicationBuilder
            .Create(clientId)
            .Build();

InteractiveAuthenticationProvider authProvider = new InteractiveAuthenticationProvider(publicClientApplication, scopes);
```

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="55e56-262">Javascript</span><span class="sxs-lookup"><span data-stu-id="55e56-262">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="55e56-263">尚不可用。</span><span class="sxs-lookup"><span data-stu-id="55e56-263">Not yet available.</span></span> <span data-ttu-id="55e56-264">如果这对你非常重要, 请投票或打开[Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)。</span><span class="sxs-lookup"><span data-stu-id="55e56-264">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="javatabjava"></a>[<span data-ttu-id="55e56-265">Java</span><span class="sxs-lookup"><span data-stu-id="55e56-265">Java</span></span>](#tab/Java)

<span data-ttu-id="55e56-266">尚不可用。</span><span class="sxs-lookup"><span data-stu-id="55e56-266">Not yet available.</span></span> <span data-ttu-id="55e56-267">如果这对你非常重要, 请投票或打开[Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)。</span><span class="sxs-lookup"><span data-stu-id="55e56-267">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="androidtabandroid"></a>[<span data-ttu-id="55e56-268">Android</span><span class="sxs-lookup"><span data-stu-id="55e56-268">Android</span></span>](#tab/Android)

```java
PublicClientApplication publicClientApplication = new PublicClientApplication(getApplicationContext(), "CLIENT_ID_OF_YOUR_APPLICATION");
MSALAuthenticationProvider msalAuthenticationProvider = new MSALAuthenticationProvider(
    getActivity(),
    getApplication(),
    publicClientApplication,
    scopes);

IGraphServiceClient graphClient =
  GraphServiceClient
    .builder()
    .authenticationProvider(msalAuthenticationProvider)
    .buildClient();
```

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="55e56-269">目标-C</span><span class="sxs-lookup"><span data-stu-id="55e56-269">Objective-C</span></span>](#tab/Objective-C)

```objc
NSError *error = nil;
MSALPublicClientApplication *publicClientApplication = [[MSALPublicClientApplication alloc] initWithClientId:@"INSERT-CLIENT-APP-ID" 
error:&error];

MSALAuthenticationProviderOptions *authProviderOptions= [[MSALAuthenticationProviderOptions alloc] initWithScopes:<array-of-scopes-for-which-you-need-access-token>];

 MSALAuthenticationProvider *authenticationProvider = [[MSALAuthenticationProvider alloc] initWithPublicClientApplication:publicClientApplication 
 andOptions:authProviderOptions];
```

# <a name="phptabphp"></a>[<span data-ttu-id="55e56-270">PHP</span><span class="sxs-lookup"><span data-stu-id="55e56-270">PHP</span></span>](#tab/PHP)

<span data-ttu-id="55e56-271">不适用。</span><span class="sxs-lookup"><span data-stu-id="55e56-271">Not applicable.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="55e56-272">Ruby</span><span class="sxs-lookup"><span data-stu-id="55e56-272">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="55e56-273">不适用。</span><span class="sxs-lookup"><span data-stu-id="55e56-273">Not applicable.</span></span>

---

##  <a name="a-nameusernamepasswordproviderusernamepassword-provider"></a><span data-ttu-id="55e56-274"><a name="UsernamePasswordProvider"/>用户名/密码提供程序</span><span class="sxs-lookup"><span data-stu-id="55e56-274"><a name="UsernamePasswordProvider"/>Username/password provider</span></span>

<span data-ttu-id="55e56-275">用户名/密码提供程序允许应用程序使用用户名和密码登录用户。</span><span class="sxs-lookup"><span data-stu-id="55e56-275">The username/password provider allows an application to sign in a user by using their username and password.</span></span> <span data-ttu-id="55e56-276">仅当您不能使用任何其他 OAuth 流时, 才使用此流。</span><span class="sxs-lookup"><span data-stu-id="55e56-276">Use this flow only when you cannot use any of the other OAuth flows.</span></span> <span data-ttu-id="55e56-277">有关详细信息, 请参阅[Microsoft identity platform 和 OAuth 2.0 资源所有者密码凭据](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth-ropc)</span><span class="sxs-lookup"><span data-stu-id="55e56-277">For more information, see [Microsoft identity platform and the OAuth 2.0 resource owner password credential](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth-ropc)</span></span>



# <a name="ctabcs"></a>[<span data-ttu-id="55e56-278">C#</span><span class="sxs-lookup"><span data-stu-id="55e56-278">C#</span></span>](#tab/CS)

```csharp
IPublicClientApplication publicClientApplication = PublicClientApplicationBuilder
            .Create(clientId)
            .WithTenantId(tenantID)
            .Build();

UsernamePasswordProvider authProvider = new UsernamePasswordProvider(publicClientApplication, scopes);

GraphServiceClient graphClient = new GraphServiceClient(authProvider);

User me = await graphClient.Me.Request()
                .WithUsernamePassword(email, password)
                .GetAsync();
```

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="55e56-279">Javascript</span><span class="sxs-lookup"><span data-stu-id="55e56-279">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="55e56-280">尚不可用。</span><span class="sxs-lookup"><span data-stu-id="55e56-280">Not yet available.</span></span> <span data-ttu-id="55e56-281">如果这对你非常重要, 请投票或打开[Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)。</span><span class="sxs-lookup"><span data-stu-id="55e56-281">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="javatabjava"></a>[<span data-ttu-id="55e56-282">Java</span><span class="sxs-lookup"><span data-stu-id="55e56-282">Java</span></span>](#tab/Java)

```java
UsernamePasswordProvider authProvider = new UsernamePasswordProvider(
                                                    clientId,
                                                    scopes,
                                                    username,
                                                    password);
```

# <a name="androidtabandroid"></a>[<span data-ttu-id="55e56-283">Android</span><span class="sxs-lookup"><span data-stu-id="55e56-283">Android</span></span>](#tab/Android)

<span data-ttu-id="55e56-284">不适用。</span><span class="sxs-lookup"><span data-stu-id="55e56-284">Not applicable.</span></span>

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="55e56-285">目标-C</span><span class="sxs-lookup"><span data-stu-id="55e56-285">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="55e56-286">不适用。</span><span class="sxs-lookup"><span data-stu-id="55e56-286">Not applicable.</span></span>

# <a name="phptabphp"></a>[<span data-ttu-id="55e56-287">PHP</span><span class="sxs-lookup"><span data-stu-id="55e56-287">PHP</span></span>](#tab/PHP)

<span data-ttu-id="55e56-288">尚不可用。</span><span class="sxs-lookup"><span data-stu-id="55e56-288">Not yet available.</span></span> <span data-ttu-id="55e56-289">如果这对你非常重要, 请投票或打开[Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)。</span><span class="sxs-lookup"><span data-stu-id="55e56-289">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="55e56-290">Ruby</span><span class="sxs-lookup"><span data-stu-id="55e56-290">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="55e56-291">尚不可用。</span><span class="sxs-lookup"><span data-stu-id="55e56-291">Not yet available.</span></span> <span data-ttu-id="55e56-292">如果这对你非常重要, 请投票或打开[Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)。</span><span class="sxs-lookup"><span data-stu-id="55e56-292">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

## <a name="next-steps"></a><span data-ttu-id="55e56-293">后续步骤</span><span class="sxs-lookup"><span data-stu-id="55e56-293">Next steps</span></span>

* <span data-ttu-id="55e56-294">身份验证提供程序需要客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="55e56-294">Authentication providers require an client ID.</span></span> <span data-ttu-id="55e56-295">设置身份验证提供程序后, 需要[注册应用程序](https://portal.azure.com/)。</span><span class="sxs-lookup"><span data-stu-id="55e56-295">You'll want to [register your application](https://portal.azure.com/) after you set up your authentication provider.</span></span>
* <span data-ttu-id="55e56-296">如果[Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)目前不支持所需的 OAuth 流, 请告知我们。</span><span class="sxs-lookup"><span data-stu-id="55e56-296">Let us know if a required OAuth flow isn't currently supported by voting for or opening a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests).</span></span>
