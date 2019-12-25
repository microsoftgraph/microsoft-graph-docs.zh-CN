---
title: 选择 Microsoft Graph 身份验证提供程序
description: 了解如何为您的应用程序选择特定于方案的身份验证提供程序。
localization_priority: Normal
author: MichaelMainer
ms.openlocfilehash: 678468abae61fa0f9830c0dd1b1578d9aafa177a
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40868532"
---
# <a name="choose-a-microsoft-graph-authentication-provider-based-on-scenario"></a><span data-ttu-id="7ebb7-103">根据应用场景选择 Microsoft Graph 身份验证提供程序</span><span class="sxs-lookup"><span data-stu-id="7ebb7-103">Choose a Microsoft Graph authentication provider based on scenario</span></span>

<span data-ttu-id="7ebb7-104">身份验证提供程序实现使用 Microsoft 身份验证库（MSAL）获取令牌所需的代码;处理一些可能的错误，如增量许可、过期密码和有条件访问等情况。，然后设置 HTTP 请求授权标头。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-104">Authentication providers implement the code required to acquire a token using the Microsoft Authentication Library (MSAL); handle a number of potential errors for cases like incremental consent, expired passwords, and conditional access; and then set the HTTP request authorization header.</span></span> <span data-ttu-id="7ebb7-105">下表列出了与不同[应用程序类型](/azure/active-directory/develop/v2-app-types)的方案相匹配的提供程序集。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-105">The following table lists the set of providers that match the scenarios for different [application types](/azure/active-directory/develop/v2-app-types).</span></span>

|<span data-ttu-id="7ebb7-106">方案</span><span class="sxs-lookup"><span data-stu-id="7ebb7-106">Scenario</span></span> | <span data-ttu-id="7ebb7-107">流/授予</span><span class="sxs-lookup"><span data-stu-id="7ebb7-107">Flow/Grant</span></span> | <span data-ttu-id="7ebb7-108">受众</span><span class="sxs-lookup"><span data-stu-id="7ebb7-108">Audience</span></span> | <span data-ttu-id="7ebb7-109">提供程序</span><span class="sxs-lookup"><span data-stu-id="7ebb7-109">Provider</span></span>|
|--|--|--|--|
| [<span data-ttu-id="7ebb7-110">单页面应用程序</span><span class="sxs-lookup"><span data-stu-id="7ebb7-110">Single Page App</span></span>](/azure/active-directory/develop/scenario-spa-acquire-token)| | | |
| | <span data-ttu-id="7ebb7-111">隐式</span><span class="sxs-lookup"><span data-stu-id="7ebb7-111">Implicit</span></span> | <span data-ttu-id="7ebb7-112">委派的消费者/组织</span><span class="sxs-lookup"><span data-stu-id="7ebb7-112">Delegated Consumer/Org</span></span> |[<span data-ttu-id="7ebb7-113">隐式提供程序</span><span class="sxs-lookup"><span data-stu-id="7ebb7-113">Implicit Provider</span></span>](#ImplicitProvider) |
| [<span data-ttu-id="7ebb7-114">调用 web Api 的 web 应用程序</span><span class="sxs-lookup"><span data-stu-id="7ebb7-114">Web App that calls web APIs</span></span>](/azure/active-directory/develop/scenario-web-app-call-api-acquire-token) | | | |
| | <span data-ttu-id="7ebb7-115">授权代码</span><span class="sxs-lookup"><span data-stu-id="7ebb7-115">Authorization Code</span></span> | <span data-ttu-id="7ebb7-116">委派的消费者/组织</span><span class="sxs-lookup"><span data-stu-id="7ebb7-116">Delegated Consumer/Org</span></span> | [<span data-ttu-id="7ebb7-117">授权代码提供程序</span><span class="sxs-lookup"><span data-stu-id="7ebb7-117">Authorization Code Provider</span></span>](#AuthCodeProvider) |
| | <span data-ttu-id="7ebb7-118">客户端凭据</span><span class="sxs-lookup"><span data-stu-id="7ebb7-118">Client Credentials</span></span>  | <span data-ttu-id="7ebb7-119">仅限应用</span><span class="sxs-lookup"><span data-stu-id="7ebb7-119">App Only</span></span> | [<span data-ttu-id="7ebb7-120">客户端凭据提供程序</span><span class="sxs-lookup"><span data-stu-id="7ebb7-120">Client Credentials Provider</span></span>](#ClientCredentialsProvider) |
| [<span data-ttu-id="7ebb7-121">调用 web Api 的 Web API</span><span class="sxs-lookup"><span data-stu-id="7ebb7-121">Web API that calls web APIs</span></span>](/azure/active-directory/develop/scenario-web-api-call-api-acquire-token) | | | |
| | <span data-ttu-id="7ebb7-122">代表</span><span class="sxs-lookup"><span data-stu-id="7ebb7-122">On Behalf Of</span></span> | <span data-ttu-id="7ebb7-123">委派的消费者/组织</span><span class="sxs-lookup"><span data-stu-id="7ebb7-123">Delegated Consumer/Org</span></span> | [<span data-ttu-id="7ebb7-124">代表提供程序</span><span class="sxs-lookup"><span data-stu-id="7ebb7-124">On Behalf Of Provider</span></span>](#OnBehalfOfProvider) |
| | <span data-ttu-id="7ebb7-125">客户端凭据</span><span class="sxs-lookup"><span data-stu-id="7ebb7-125">Client Credentials</span></span>  | <span data-ttu-id="7ebb7-126">仅限应用</span><span class="sxs-lookup"><span data-stu-id="7ebb7-126">App Only</span></span> | [<span data-ttu-id="7ebb7-127">客户端凭据提供程序</span><span class="sxs-lookup"><span data-stu-id="7ebb7-127">Client Credentials Provider</span></span>](#ClientCredentialsProvider) |
| [<span data-ttu-id="7ebb7-128">调用 web Api 的桌面应用程序</span><span class="sxs-lookup"><span data-stu-id="7ebb7-128">Desktop app that calls web APIs</span></span>](/azure/active-directory/develop/scenario-desktop-acquire-token) | | | |
| | <span data-ttu-id="7ebb7-129">Interactive</span><span class="sxs-lookup"><span data-stu-id="7ebb7-129">Interactive</span></span> | <span data-ttu-id="7ebb7-130">委派的消费者/组织</span><span class="sxs-lookup"><span data-stu-id="7ebb7-130">Delegated Consumer/Org</span></span> | [<span data-ttu-id="7ebb7-131">交互式提供程序</span><span class="sxs-lookup"><span data-stu-id="7ebb7-131">Interactive Provider</span></span>](#InteractiveProvider) |
| | <span data-ttu-id="7ebb7-132">集成的 Windows</span><span class="sxs-lookup"><span data-stu-id="7ebb7-132">Integrated Windows</span></span> | <span data-ttu-id="7ebb7-133">委派的组织</span><span class="sxs-lookup"><span data-stu-id="7ebb7-133">Delegated Org</span></span> | [<span data-ttu-id="7ebb7-134">集成 Windows 提供程序</span><span class="sxs-lookup"><span data-stu-id="7ebb7-134">Integrated Windows Provider</span></span>](#IntegratedWindowsProvider) |
| | <span data-ttu-id="7ebb7-135">资源所有者</span><span class="sxs-lookup"><span data-stu-id="7ebb7-135">Resource Owner</span></span>  | <span data-ttu-id="7ebb7-136">委派的组织</span><span class="sxs-lookup"><span data-stu-id="7ebb7-136">Delegated Org</span></span> | [<span data-ttu-id="7ebb7-137">用户名/密码提供程序</span><span class="sxs-lookup"><span data-stu-id="7ebb7-137">Username / Password Provider</span></span>](#UsernamePasswordProvider) |
| | <span data-ttu-id="7ebb7-138">设备代码</span><span class="sxs-lookup"><span data-stu-id="7ebb7-138">Device Code</span></span>  | <span data-ttu-id="7ebb7-139">委派的组织</span><span class="sxs-lookup"><span data-stu-id="7ebb7-139">Delegated Org</span></span> | [<span data-ttu-id="7ebb7-140">设备代码提供程序</span><span class="sxs-lookup"><span data-stu-id="7ebb7-140">Device Code Provider</span></span>](#DeviceCodeProvider) |
| [<span data-ttu-id="7ebb7-141">守护程序应用</span><span class="sxs-lookup"><span data-stu-id="7ebb7-141">Daemon app</span></span>](/azure/active-directory/develop/scenario-daemon-acquire-token) | | | |
| | <span data-ttu-id="7ebb7-142">客户端凭据</span><span class="sxs-lookup"><span data-stu-id="7ebb7-142">Client Credentials</span></span>  | <span data-ttu-id="7ebb7-143">仅限应用</span><span class="sxs-lookup"><span data-stu-id="7ebb7-143">App Only</span></span> | [<span data-ttu-id="7ebb7-144">客户端凭据提供程序</span><span class="sxs-lookup"><span data-stu-id="7ebb7-144">Client Credentials Provider</span></span>](#ClientCredentialsProvider) |
| [<span data-ttu-id="7ebb7-145">调用 web Api 的移动应用程序</span><span class="sxs-lookup"><span data-stu-id="7ebb7-145">Mobile app that calls web APIs</span></span>](/azure/active-directory/develop/scenario-mobile-acquire-token) | | | |
| | <span data-ttu-id="7ebb7-146">Interactive</span><span class="sxs-lookup"><span data-stu-id="7ebb7-146">Interactive</span></span> | <span data-ttu-id="7ebb7-147">委派的消费者/组织</span><span class="sxs-lookup"><span data-stu-id="7ebb7-147">Delegated Consumer/Org</span></span> | [<span data-ttu-id="7ebb7-148">交互式提供程序</span><span class="sxs-lookup"><span data-stu-id="7ebb7-148">Interactive Provider</span></span>](#InteractiveProvider) |


## <a name="a-nameauthcodeproviderauthorization-code-provider"></a><span data-ttu-id="7ebb7-149"><a name="AuthCodeProvider"/>授权代码提供程序</span><span class="sxs-lookup"><span data-stu-id="7ebb7-149"><a name="AuthCodeProvider"/>Authorization code provider</span></span>

<span data-ttu-id="7ebb7-150">授权代码流使本机应用程序和 web 应用能够安全地获取用户名称中的令牌。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-150">The authorization code flow enables native and web apps to securely obtain tokens in the name of the user.</span></span> <span data-ttu-id="7ebb7-151">若要了解详细信息，请参阅[Microsoft identity platform 和 OAuth 2.0 授权代码流](/azure/active-directory/develop/v2-oauth2-auth-code-flow)。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-151">To learn more, see [Microsoft identity platform and OAuth 2.0 authorization code flow](/azure/active-directory/develop/v2-oauth2-auth-code-flow).</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="7ebb7-152">C#</span><span class="sxs-lookup"><span data-stu-id="7ebb7-152">C#</span></span>](#tab/CS)

```csharp
IConfidentialClientApplication confidentialClientApplication = ConfidentialClientApplicationBuilder
    .Create(clientId)
    .WithRedirectUri(redirectUri)
    .WithClientSecret(clientSecret) // or .WithCertificate(certificate)
    .Build();

AuthorizationCodeProvider authProvider = new AuthorizationCodeProvider(confidentialClientApplication, scopes);
```

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7ebb7-153">Javascript</span><span class="sxs-lookup"><span data-stu-id="7ebb7-153">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="7ebb7-154">授权代码、客户端凭据和代表的 OAuth 流都要求您在此时实现自定义身份验证提供程序。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-154">Authorization code, client credential, and on-behalf-of OAuth flows require that you implement a custom authentication provider at this time.</span></span> <span data-ttu-id="7ebb7-155">有关详细信息，请参阅[使用自定义身份验证提供程序](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md)。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-155">For more information, see [Using a custom authentication provider](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md).</span></span>

# <a name="javatabjava"></a>[<span data-ttu-id="7ebb7-156">Java</span><span class="sxs-lookup"><span data-stu-id="7ebb7-156">Java</span></span>](#tab/Java)

```java
AuthorizationCodeProvider authProvider = new AuthorizationCodeProvider(
                                                    clientId,
                                                    scopes,
                                                    authorizationCode,
                                                    redirectUri,
                                                    clientSecret);
```

# <a name="androidtabandroid"></a>[<span data-ttu-id="7ebb7-157">Android</span><span class="sxs-lookup"><span data-stu-id="7ebb7-157">Android</span></span>](#tab/Android)

<span data-ttu-id="7ebb7-158">不适用。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-158">Not applicable.</span></span>

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="7ebb7-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7ebb7-159">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="7ebb7-160">不适用。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-160">Not applicable.</span></span>

# <a name="phptabphp"></a>[<span data-ttu-id="7ebb7-161">PHP</span><span class="sxs-lookup"><span data-stu-id="7ebb7-161">PHP</span></span>](#tab/PHP)

<span data-ttu-id="7ebb7-162">尚不可用。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-162">Not yet available.</span></span> <span data-ttu-id="7ebb7-163">如果这对你非常重要，请支持或打开[Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-163">Please support or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="7ebb7-164">Ruby</span><span class="sxs-lookup"><span data-stu-id="7ebb7-164">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="7ebb7-165">尚不可用。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-165">Not available, yet.</span></span> <span data-ttu-id="7ebb7-166">如果这对你非常重要，请投票或打开[Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-166">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

##  <a name="a-nameclientcredentialsproviderclient-credentials-provider"></a><span data-ttu-id="7ebb7-167"><a name="ClientCredentialsProvider"/>客户端凭据提供程序</span><span class="sxs-lookup"><span data-stu-id="7ebb7-167"><a name="ClientCredentialsProvider"/>Client credentials provider</span></span>

<span data-ttu-id="7ebb7-168">客户端凭据流使服务应用程序可以在没有用户交互的情况下运行。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-168">The client credential flow enables service applications to run without user interaction.</span></span> <span data-ttu-id="7ebb7-169">访问基于应用程序的标识。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-169">Access is based on the identity of the application.</span></span> <span data-ttu-id="7ebb7-170">有关详细信息，请参阅[Microsoft identity platform 和 OAuth 2.0 客户端凭据流](/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-170">For more information, see [Microsoft identity platform and the OAuth 2.0 client credentials flow](/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow).</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="7ebb7-171">C#</span><span class="sxs-lookup"><span data-stu-id="7ebb7-171">C#</span></span>](#tab/CS)

```csharp
IConfidentialClientApplication confidentialClientApplication = ConfidentialClientApplicationBuilder
    .Create(clientId)
    .WithTenantId(tenantID)
    .WithClientSecret(clientSecret)
    .Build();

ClientCredentialProvider authProvider = new ClientCredentialProvider(confidentialClientApplication);
```

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7ebb7-172">Javascript</span><span class="sxs-lookup"><span data-stu-id="7ebb7-172">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="7ebb7-173">授权代码、客户端凭据和代表的 OAuth 流都要求您在此时实现自定义身份验证提供程序。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-173">Authorization code, client credential, and on-behalf-of OAuth flows require that you implement a custom authentication provider at this time.</span></span> <span data-ttu-id="7ebb7-174">有关详细信息，请参阅[使用自定义身份验证提供程序](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md)。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-174">For more information, see [Using a custom authentication provider](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md).</span></span>

# <a name="javatabjava"></a>[<span data-ttu-id="7ebb7-175">Java</span><span class="sxs-lookup"><span data-stu-id="7ebb7-175">Java</span></span>](#tab/Java)

```java
ClientCredentialProvider authProvider = new ClientCredentialProvider(
                                                    clientId,
                                                    scopes,
                                                    clientSecret,
                                                    tenant,
                                                    endpoint);
```

# <a name="androidtabandroid"></a>[<span data-ttu-id="7ebb7-176">Android</span><span class="sxs-lookup"><span data-stu-id="7ebb7-176">Android</span></span>](#tab/Android)

<span data-ttu-id="7ebb7-177">不适用。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-177">Not applicable.</span></span>

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="7ebb7-178">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7ebb7-178">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="7ebb7-179">不适用。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-179">Not applicable.</span></span>

# <a name="phptabphp"></a>[<span data-ttu-id="7ebb7-180">PHP</span><span class="sxs-lookup"><span data-stu-id="7ebb7-180">PHP</span></span>](#tab/PHP)

<span data-ttu-id="7ebb7-181">尚不可用。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-181">Not available, yet.</span></span> <span data-ttu-id="7ebb7-182">如果这对你非常重要，请支持或打开[Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-182">Please support or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="7ebb7-183">Ruby</span><span class="sxs-lookup"><span data-stu-id="7ebb7-183">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="7ebb7-184">尚不可用。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-184">Not available, yet.</span></span> <span data-ttu-id="7ebb7-185">如果这对你非常重要，请支持或打开[Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-185">Please support or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

##  <a name="a-nameonbehalfofprovideron-behalf-of-provider"></a><span data-ttu-id="7ebb7-186"><a name="OnBehalfOfProvider"/>代表提供程序</span><span class="sxs-lookup"><span data-stu-id="7ebb7-186"><a name="OnBehalfOfProvider"/>On-behalf-of provider</span></span>

<span data-ttu-id="7ebb7-187">当应用程序调用在其中打开 Microsoft Graph API 的服务/web API 时，代表流是适用的。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-187">The on-behalf-of flow is applicable when your application calls a service/web API which in turns calls the Microsoft Graph API.</span></span> <span data-ttu-id="7ebb7-188">若要了解详细信息，请阅读[Microsoft identity platform 和 OAuth 2.0 代表流](/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow)</span><span class="sxs-lookup"><span data-stu-id="7ebb7-188">Learn more by reading [Microsoft identity platform and OAuth 2.0 On-Behalf-Of flow](/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow)</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="7ebb7-189">C#</span><span class="sxs-lookup"><span data-stu-id="7ebb7-189">C#</span></span>](#tab/CS)

```csharp
IConfidentialClientApplication confidentialClientApplication = ConfidentialClientApplicationBuilder
    .Create(clientId)
    .WithRedirectUri(redirectUri)
    .WithClientSecret(clientSecret)
    .Build();

OnBehalfOfProvider authProvider = new OnBehalfOfProvider(confidentialClientApplication, scopes);
```

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7ebb7-190">Javascript</span><span class="sxs-lookup"><span data-stu-id="7ebb7-190">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="7ebb7-191">授权代码、客户端凭据和代表的 OAuth 流都要求您在此时实现自定义身份验证提供程序。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-191">Authorization code, client credential, and on-behalf-of OAuth flows require that you implement a custom authentication provider at this time.</span></span> <span data-ttu-id="7ebb7-192">有关详细信息，请参阅[使用自定义身份验证提供程序](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md)。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-192">Read [Using Custom Authentication Provider](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md) for more information.</span></span>

# <a name="javatabjava"></a>[<span data-ttu-id="7ebb7-193">Java</span><span class="sxs-lookup"><span data-stu-id="7ebb7-193">Java</span></span>](#tab/Java)

<span data-ttu-id="7ebb7-194">尚不可用。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-194">Not yet available.</span></span> <span data-ttu-id="7ebb7-195">如果这对你非常重要，请投票或打开[Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-195">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="androidtabandroid"></a>[<span data-ttu-id="7ebb7-196">Android</span><span class="sxs-lookup"><span data-stu-id="7ebb7-196">Android</span></span>](#tab/Android)

<span data-ttu-id="7ebb7-197">不适用。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-197">Not applicable.</span></span>

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="7ebb7-198">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7ebb7-198">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="7ebb7-199">不适用。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-199">Not applicable.</span></span>

# <a name="phptabphp"></a>[<span data-ttu-id="7ebb7-200">PHP</span><span class="sxs-lookup"><span data-stu-id="7ebb7-200">PHP</span></span>](#tab/PHP)

<span data-ttu-id="7ebb7-201">尚不可用。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-201">Not yet available.</span></span> <span data-ttu-id="7ebb7-202">如果这对你非常重要，请投票或打开[Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-202">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="7ebb7-203">Ruby</span><span class="sxs-lookup"><span data-stu-id="7ebb7-203">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="7ebb7-204">尚不可用。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-204">Not yet available.</span></span> <span data-ttu-id="7ebb7-205">如果这对你非常重要，请投票或打开[Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-205">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

## <a name="a-nameimplicitproviderimplicit-provider"></a><span data-ttu-id="7ebb7-206"><a name="ImplicitProvider"/>隐式提供程序</span><span class="sxs-lookup"><span data-stu-id="7ebb7-206"><a name="ImplicitProvider"/>Implicit provider</span></span>

<span data-ttu-id="7ebb7-207">隐式授予流在基于浏览器的应用程序中使用。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-207">The implicit grant flow is used in browser-based applications.</span></span> <span data-ttu-id="7ebb7-208">有关详细信息，请参阅[Microsoft identity platform 和隐式授予流](/azure/active-directory/develop/v2-oauth2-implicit-grant-flow)。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-208">For more information, see [Microsoft identity platform and Implicit grant flow](/azure/active-directory/develop/v2-oauth2-implicit-grant-flow).</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="7ebb7-209">C#</span><span class="sxs-lookup"><span data-stu-id="7ebb7-209">C#</span></span>](#tab/CS)

<span data-ttu-id="7ebb7-210">不适用。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-210">Not applicable.</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7ebb7-211">Javascript</span><span class="sxs-lookup"><span data-stu-id="7ebb7-211">Javascript</span></span>](#tab/Javascript)

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
const authProvider = new MicrosoftGraph.ImplicitMSALAuthenticationProvider(userAgentApplication, graphScopes);

const options = {
    authProvider, // An instance created from previous step
};
const Client = MicrosoftGraph.Client;
const client = Client.initWithMiddleware(options);
```

# <a name="javatabjava"></a>[<span data-ttu-id="7ebb7-212">Java</span><span class="sxs-lookup"><span data-stu-id="7ebb7-212">Java</span></span>](#tab/Java)

<span data-ttu-id="7ebb7-213">不适用。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-213">Not applicable.</span></span>

# <a name="androidtabandroid"></a>[<span data-ttu-id="7ebb7-214">Android</span><span class="sxs-lookup"><span data-stu-id="7ebb7-214">Android</span></span>](#tab/Android)

<span data-ttu-id="7ebb7-215">不适用。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-215">Not applicable.</span></span>

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="7ebb7-216">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7ebb7-216">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="7ebb7-217">不适用。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-217">Not applicable.</span></span>

# <a name="phptabphp"></a>[<span data-ttu-id="7ebb7-218">PHP</span><span class="sxs-lookup"><span data-stu-id="7ebb7-218">PHP</span></span>](#tab/PHP)

<span data-ttu-id="7ebb7-219">不适用。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-219">Not applicable.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="7ebb7-220">Ruby</span><span class="sxs-lookup"><span data-stu-id="7ebb7-220">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="7ebb7-221">不适用。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-221">Not applicable.</span></span>

---

##  <a name="a-namedevicecodeproviderdevice-code-provider"></a><span data-ttu-id="7ebb7-222"><a name="DeviceCodeProvider"/>设备代码提供程序</span><span class="sxs-lookup"><span data-stu-id="7ebb7-222"><a name="DeviceCodeProvider"/>Device code provider</span></span>

<span data-ttu-id="7ebb7-223">设备代码流允许通过其他设备登录设备。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-223">The device code flow enables sign in to devices by way of another device.</span></span> <span data-ttu-id="7ebb7-224">有关详细信息，请参阅[Microsoft identity platform 和 OAuth 2.0 设备代码流](/azure/active-directory/develop/v2-oauth2-device-code)。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-224">For details, see [Microsoft identity platform and the OAuth 2.0 device code flow](/azure/active-directory/develop/v2-oauth2-device-code).</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="7ebb7-225">C#</span><span class="sxs-lookup"><span data-stu-id="7ebb7-225">C#</span></span>](#tab/CS)

```csharp
IPublicClientApplication publicClientApplication = PublicClientApplicationBuilder
            .Create(clientId)
            .Build();

Func<DeviceCodeResult, Task> deviceCodeReadyCallback = async dcr => await Console.Out.WriteLineAsync(dcr.Message);

DeviceCodeProvider authProvider = new DeviceCodeProvider(publicClientApplication, scopes, deviceCodeReadyCallback);
```

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7ebb7-226">Javascript</span><span class="sxs-lookup"><span data-stu-id="7ebb7-226">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="7ebb7-227">尚不可用。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-227">Not yet available.</span></span> <span data-ttu-id="7ebb7-228">如果这对你非常重要，请投票或打开[Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-228">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="javatabjava"></a>[<span data-ttu-id="7ebb7-229">Java</span><span class="sxs-lookup"><span data-stu-id="7ebb7-229">Java</span></span>](#tab/Java)

<span data-ttu-id="7ebb7-230">尚不可用。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-230">Not available, yet.</span></span> <span data-ttu-id="7ebb7-231">如果这对你非常重要，请支持或打开[Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-231">Please support or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="androidtabandroid"></a>[<span data-ttu-id="7ebb7-232">Android</span><span class="sxs-lookup"><span data-stu-id="7ebb7-232">Android</span></span>](#tab/Android)

<span data-ttu-id="7ebb7-233">不适用。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-233">Not applicable.</span></span>

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="7ebb7-234">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7ebb7-234">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="7ebb7-235">不适用。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-235">Not applicable.</span></span>

# <a name="phptabphp"></a>[<span data-ttu-id="7ebb7-236">PHP</span><span class="sxs-lookup"><span data-stu-id="7ebb7-236">PHP</span></span>](#tab/PHP)

<span data-ttu-id="7ebb7-237">尚不可用。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-237">Not yet available.</span></span> <span data-ttu-id="7ebb7-238">如果这对你非常重要，请投票或打开[Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-238">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="7ebb7-239">Ruby</span><span class="sxs-lookup"><span data-stu-id="7ebb7-239">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="7ebb7-240">尚不可用。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-240">Not yet available.</span></span> <span data-ttu-id="7ebb7-241">如果这对你非常重要，请投票或打开[Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-241">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

##  <a name="a-nameintegratedwindowsproviderintegrated-windows-provider"></a><span data-ttu-id="7ebb7-242"><a name="IntegratedWindowsProvider"/>集成 Windows 提供程序</span><span class="sxs-lookup"><span data-stu-id="7ebb7-242"><a name="IntegratedWindowsProvider"/>Integrated Windows provider</span></span>

<span data-ttu-id="7ebb7-243">集成的 Windows 流为 Windows 计算机提供了一种在加入域时无提示地获取访问令牌的方法。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-243">The integrated Windows flow provides a way for Windows computers to silently acquire an access token when they are domain joined.</span></span> <span data-ttu-id="7ebb7-244">有关详细信息，请参阅[集成 Windows 身份验证](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Integrated-Windows-Authentication)。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-244">For details, see [Integrated Windows authentication](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Integrated-Windows-Authentication).</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="7ebb7-245">C#</span><span class="sxs-lookup"><span data-stu-id="7ebb7-245">C#</span></span>](#tab/CS)

```csharp
IPublicClientApplication publicClientApplication = PublicClientApplicationBuilder
            .Create(clientId)
            .WithTenantId(tenantID)
            .Build();

IntegratedWindowsAuthenticationProvider authProvider = new IntegratedWindowsAuthenticationProvider(publicClientApplication, scopes);
```

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7ebb7-246">Javascript</span><span class="sxs-lookup"><span data-stu-id="7ebb7-246">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="7ebb7-247">不适用。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-247">Not applicable.</span></span>

# <a name="javatabjava"></a>[<span data-ttu-id="7ebb7-248">Java</span><span class="sxs-lookup"><span data-stu-id="7ebb7-248">Java</span></span>](#tab/Java)

<span data-ttu-id="7ebb7-249">不适用。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-249">Not applicable.</span></span>

# <a name="androidtabandroid"></a>[<span data-ttu-id="7ebb7-250">Android</span><span class="sxs-lookup"><span data-stu-id="7ebb7-250">Android</span></span>](#tab/Android)

<span data-ttu-id="7ebb7-251">不适用。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-251">Not applicable.</span></span>

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="7ebb7-252">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7ebb7-252">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="7ebb7-253">不适用。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-253">Not applicable.</span></span>

# <a name="phptabphp"></a>[<span data-ttu-id="7ebb7-254">PHP</span><span class="sxs-lookup"><span data-stu-id="7ebb7-254">PHP</span></span>](#tab/PHP)

<span data-ttu-id="7ebb7-255">不适用。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-255">Not applicable.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="7ebb7-256">Ruby</span><span class="sxs-lookup"><span data-stu-id="7ebb7-256">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="7ebb7-257">不适用。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-257">Not applicable.</span></span>

---

##  <a name="a-nameinteractiveproviderinteractive-provider"></a><span data-ttu-id="7ebb7-258"><a name="InteractiveProvider"/>交互式提供程序</span><span class="sxs-lookup"><span data-stu-id="7ebb7-258"><a name="InteractiveProvider"/>Interactive provider</span></span>

<span data-ttu-id="7ebb7-259">移动应用程序（Xamarin 和 UWP）和桌面应用程序使用交互流，以在用户的名称中调用 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-259">The interactive flow is used by mobile applications (Xamarin and UWP) and desktops applications to call Microsoft Graph in the name of a user.</span></span> <span data-ttu-id="7ebb7-260">有关详细信息，请参阅[以交互方式获取令牌](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Acquiring-tokens-interactively)。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-260">For details, see [Acquiring tokens interactively](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Acquiring-tokens-interactively).</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="7ebb7-261">C#</span><span class="sxs-lookup"><span data-stu-id="7ebb7-261">C#</span></span>](#tab/CS)

```csharp
IPublicClientApplication publicClientApplication = PublicClientApplicationBuilder
            .Create(clientId)
            .Build();

InteractiveAuthenticationProvider authProvider = new InteractiveAuthenticationProvider(publicClientApplication, scopes);
```

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7ebb7-262">Javascript</span><span class="sxs-lookup"><span data-stu-id="7ebb7-262">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="7ebb7-263">尚不可用。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-263">Not yet available.</span></span> <span data-ttu-id="7ebb7-264">如果这对你非常重要，请投票或打开[Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-264">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="javatabjava"></a>[<span data-ttu-id="7ebb7-265">Java</span><span class="sxs-lookup"><span data-stu-id="7ebb7-265">Java</span></span>](#tab/Java)

<span data-ttu-id="7ebb7-266">尚不可用。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-266">Not yet available.</span></span> <span data-ttu-id="7ebb7-267">如果这对你非常重要，请投票或打开[Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-267">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="androidtabandroid"></a>[<span data-ttu-id="7ebb7-268">Android</span><span class="sxs-lookup"><span data-stu-id="7ebb7-268">Android</span></span>](#tab/Android)

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

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="7ebb7-269">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7ebb7-269">Objective-C</span></span>](#tab/Objective-C)

```objc
NSError *error = nil;
MSALPublicClientApplication *publicClientApplication = [[MSALPublicClientApplication alloc] initWithClientId:@"INSERT-CLIENT-APP-ID"
error:&error];

MSALAuthenticationProviderOptions *authProviderOptions= [[MSALAuthenticationProviderOptions alloc] initWithScopes:<array-of-scopes-for-which-you-need-access-token>];

 MSALAuthenticationProvider *authenticationProvider = [[MSALAuthenticationProvider alloc] initWithPublicClientApplication:publicClientApplication
 andOptions:authProviderOptions];
```

# <a name="phptabphp"></a>[<span data-ttu-id="7ebb7-270">PHP</span><span class="sxs-lookup"><span data-stu-id="7ebb7-270">PHP</span></span>](#tab/PHP)

<span data-ttu-id="7ebb7-271">不适用。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-271">Not applicable.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="7ebb7-272">Ruby</span><span class="sxs-lookup"><span data-stu-id="7ebb7-272">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="7ebb7-273">不适用。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-273">Not applicable.</span></span>

---

##  <a name="a-nameusernamepasswordproviderusernamepassword-provider"></a><span data-ttu-id="7ebb7-274"><a name="UsernamePasswordProvider"/>用户名/密码提供程序</span><span class="sxs-lookup"><span data-stu-id="7ebb7-274"><a name="UsernamePasswordProvider"/>Username/password provider</span></span>

<span data-ttu-id="7ebb7-275">用户名/密码提供程序允许应用程序使用用户名和密码登录用户。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-275">The username/password provider allows an application to sign in a user by using their username and password.</span></span> <span data-ttu-id="7ebb7-276">仅当您不能使用任何其他 OAuth 流时，才使用此流。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-276">Use this flow only when you cannot use any of the other OAuth flows.</span></span> <span data-ttu-id="7ebb7-277">有关详细信息，请参阅[Microsoft identity platform 和 OAuth 2.0 资源所有者密码凭据](/azure/active-directory/develop/v2-oauth-ropc)</span><span class="sxs-lookup"><span data-stu-id="7ebb7-277">For more information, see [Microsoft identity platform and the OAuth 2.0 resource owner password credential](/azure/active-directory/develop/v2-oauth-ropc)</span></span>



# <a name="ctabcs"></a>[<span data-ttu-id="7ebb7-278">C#</span><span class="sxs-lookup"><span data-stu-id="7ebb7-278">C#</span></span>](#tab/CS)

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

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7ebb7-279">Javascript</span><span class="sxs-lookup"><span data-stu-id="7ebb7-279">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="7ebb7-280">尚不可用。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-280">Not yet available.</span></span> <span data-ttu-id="7ebb7-281">如果这对你非常重要，请投票或打开[Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-281">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="javatabjava"></a>[<span data-ttu-id="7ebb7-282">Java</span><span class="sxs-lookup"><span data-stu-id="7ebb7-282">Java</span></span>](#tab/Java)

```java
UsernamePasswordProvider authProvider = new UsernamePasswordProvider(
                                                    clientId,
                                                    scopes,
                                                    username,
                                                    password);
```

# <a name="androidtabandroid"></a>[<span data-ttu-id="7ebb7-283">Android</span><span class="sxs-lookup"><span data-stu-id="7ebb7-283">Android</span></span>](#tab/Android)

<span data-ttu-id="7ebb7-284">不适用。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-284">Not applicable.</span></span>

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="7ebb7-285">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7ebb7-285">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="7ebb7-286">不适用。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-286">Not applicable.</span></span>

# <a name="phptabphp"></a>[<span data-ttu-id="7ebb7-287">PHP</span><span class="sxs-lookup"><span data-stu-id="7ebb7-287">PHP</span></span>](#tab/PHP)

<span data-ttu-id="7ebb7-288">尚不可用。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-288">Not yet available.</span></span> <span data-ttu-id="7ebb7-289">如果这对你非常重要，请投票或打开[Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-289">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="7ebb7-290">Ruby</span><span class="sxs-lookup"><span data-stu-id="7ebb7-290">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="7ebb7-291">尚不可用。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-291">Not yet available.</span></span> <span data-ttu-id="7ebb7-292">如果这对你非常重要，请投票或打开[Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-292">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

## <a name="next-steps"></a><span data-ttu-id="7ebb7-293">后续步骤</span><span class="sxs-lookup"><span data-stu-id="7ebb7-293">Next steps</span></span>

* <span data-ttu-id="7ebb7-294">身份验证提供程序需要客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-294">Authentication providers require an client ID.</span></span> <span data-ttu-id="7ebb7-295">设置身份验证提供程序后，需要[注册应用程序](https://portal.azure.com/)。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-295">You'll want to [register your application](https://portal.azure.com/) after you set up your authentication provider.</span></span>
* <span data-ttu-id="7ebb7-296">如果[Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)目前不支持所需的 OAuth 流，请告知我们。</span><span class="sxs-lookup"><span data-stu-id="7ebb7-296">Let us know if a required OAuth flow isn't currently supported by voting for or opening a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests).</span></span>
