---
title: 选择 Microsoft Graph 身份验证提供程序
description: 了解如何为您的应用程序选择特定于方案的身份验证提供程序。
localization_priority: Normal
author: MichaelMainer
ms.openlocfilehash: 29f7ea60080ed1f1a2ed6ea02256e03f5b91e6cd
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/05/2020
ms.locfileid: "49580968"
---
# <a name="choose-a-microsoft-graph-authentication-provider-based-on-scenario"></a><span data-ttu-id="11e9d-103">根据应用场景选择 Microsoft Graph 身份验证提供程序</span><span class="sxs-lookup"><span data-stu-id="11e9d-103">Choose a Microsoft Graph authentication provider based on scenario</span></span>

<span data-ttu-id="11e9d-104">身份验证提供程序实现使用 Microsoft 身份验证库 (MSAL) 获取令牌所需的代码。处理一些可能的错误，如增量许可、过期密码和有条件访问等情况。，然后设置 HTTP 请求授权标头。</span><span class="sxs-lookup"><span data-stu-id="11e9d-104">Authentication providers implement the code required to acquire a token using the Microsoft Authentication Library (MSAL); handle a number of potential errors for cases like incremental consent, expired passwords, and conditional access; and then set the HTTP request authorization header.</span></span> <span data-ttu-id="11e9d-105">下表列出了与不同 [应用程序类型](/azure/active-directory/develop/v2-app-types)的方案相匹配的提供程序集。</span><span class="sxs-lookup"><span data-stu-id="11e9d-105">The following table lists the set of providers that match the scenarios for different [application types](/azure/active-directory/develop/v2-app-types).</span></span>

|<span data-ttu-id="11e9d-106">方案</span><span class="sxs-lookup"><span data-stu-id="11e9d-106">Scenario</span></span> | <span data-ttu-id="11e9d-107">流/授予</span><span class="sxs-lookup"><span data-stu-id="11e9d-107">Flow/Grant</span></span> | <span data-ttu-id="11e9d-108">受众</span><span class="sxs-lookup"><span data-stu-id="11e9d-108">Audience</span></span> | <span data-ttu-id="11e9d-109">提供程序</span><span class="sxs-lookup"><span data-stu-id="11e9d-109">Provider</span></span>|
|--|--|--|--|
| [<span data-ttu-id="11e9d-110">单页面应用程序</span><span class="sxs-lookup"><span data-stu-id="11e9d-110">Single Page App</span></span>](/azure/active-directory/develop/scenario-spa-acquire-token)| | | |
| | <span data-ttu-id="11e9d-111">隐式</span><span class="sxs-lookup"><span data-stu-id="11e9d-111">Implicit</span></span> | <span data-ttu-id="11e9d-112">委派的消费者/组织</span><span class="sxs-lookup"><span data-stu-id="11e9d-112">Delegated Consumer/Org</span></span> |[<span data-ttu-id="11e9d-113">隐式提供程序</span><span class="sxs-lookup"><span data-stu-id="11e9d-113">Implicit Provider</span></span>](#ImplicitProvider) |
| [<span data-ttu-id="11e9d-114">调用 web Api 的 web 应用程序</span><span class="sxs-lookup"><span data-stu-id="11e9d-114">Web App that calls web APIs</span></span>](/azure/active-directory/develop/scenario-web-app-call-api-acquire-token) | | | |
| | <span data-ttu-id="11e9d-115">授权代码</span><span class="sxs-lookup"><span data-stu-id="11e9d-115">Authorization Code</span></span> | <span data-ttu-id="11e9d-116">委派的消费者/组织</span><span class="sxs-lookup"><span data-stu-id="11e9d-116">Delegated Consumer/Org</span></span> | [<span data-ttu-id="11e9d-117">授权代码提供程序</span><span class="sxs-lookup"><span data-stu-id="11e9d-117">Authorization Code Provider</span></span>](#AuthCodeProvider) |
| | <span data-ttu-id="11e9d-118">客户端凭据</span><span class="sxs-lookup"><span data-stu-id="11e9d-118">Client Credentials</span></span>  | <span data-ttu-id="11e9d-119">仅限应用</span><span class="sxs-lookup"><span data-stu-id="11e9d-119">App Only</span></span> | [<span data-ttu-id="11e9d-120">客户端凭据提供程序</span><span class="sxs-lookup"><span data-stu-id="11e9d-120">Client Credentials Provider</span></span>](#ClientCredentialsProvider) |
| [<span data-ttu-id="11e9d-121">调用 web Api 的 Web API</span><span class="sxs-lookup"><span data-stu-id="11e9d-121">Web API that calls web APIs</span></span>](/azure/active-directory/develop/scenario-web-api-call-api-acquire-token) | | | |
| | <span data-ttu-id="11e9d-122">代表</span><span class="sxs-lookup"><span data-stu-id="11e9d-122">On Behalf Of</span></span> | <span data-ttu-id="11e9d-123">委派的消费者/组织</span><span class="sxs-lookup"><span data-stu-id="11e9d-123">Delegated Consumer/Org</span></span> | [<span data-ttu-id="11e9d-124">代表提供程序</span><span class="sxs-lookup"><span data-stu-id="11e9d-124">On Behalf Of Provider</span></span>](#OnBehalfOfProvider) |
| | <span data-ttu-id="11e9d-125">客户端凭据</span><span class="sxs-lookup"><span data-stu-id="11e9d-125">Client Credentials</span></span>  | <span data-ttu-id="11e9d-126">仅限应用</span><span class="sxs-lookup"><span data-stu-id="11e9d-126">App Only</span></span> | [<span data-ttu-id="11e9d-127">客户端凭据提供程序</span><span class="sxs-lookup"><span data-stu-id="11e9d-127">Client Credentials Provider</span></span>](#ClientCredentialsProvider) |
| [<span data-ttu-id="11e9d-128">调用 web Api 的桌面应用程序</span><span class="sxs-lookup"><span data-stu-id="11e9d-128">Desktop app that calls web APIs</span></span>](/azure/active-directory/develop/scenario-desktop-acquire-token) | | | |
| | <span data-ttu-id="11e9d-129">Interactive</span><span class="sxs-lookup"><span data-stu-id="11e9d-129">Interactive</span></span> | <span data-ttu-id="11e9d-130">委派的消费者/组织</span><span class="sxs-lookup"><span data-stu-id="11e9d-130">Delegated Consumer/Org</span></span> | [<span data-ttu-id="11e9d-131">交互式提供程序</span><span class="sxs-lookup"><span data-stu-id="11e9d-131">Interactive Provider</span></span>](#InteractiveProvider) |
| | <span data-ttu-id="11e9d-132">集成的 Windows</span><span class="sxs-lookup"><span data-stu-id="11e9d-132">Integrated Windows</span></span> | <span data-ttu-id="11e9d-133">委派的组织</span><span class="sxs-lookup"><span data-stu-id="11e9d-133">Delegated Org</span></span> | [<span data-ttu-id="11e9d-134">集成 Windows 提供程序</span><span class="sxs-lookup"><span data-stu-id="11e9d-134">Integrated Windows Provider</span></span>](#IntegratedWindowsProvider) |
| | <span data-ttu-id="11e9d-135">资源所有者</span><span class="sxs-lookup"><span data-stu-id="11e9d-135">Resource Owner</span></span>  | <span data-ttu-id="11e9d-136">委派的组织</span><span class="sxs-lookup"><span data-stu-id="11e9d-136">Delegated Org</span></span> | [<span data-ttu-id="11e9d-137">用户名/密码提供程序</span><span class="sxs-lookup"><span data-stu-id="11e9d-137">Username / Password Provider</span></span>](#UsernamePasswordProvider) |
| | <span data-ttu-id="11e9d-138">设备代码</span><span class="sxs-lookup"><span data-stu-id="11e9d-138">Device Code</span></span>  | <span data-ttu-id="11e9d-139">委派的组织</span><span class="sxs-lookup"><span data-stu-id="11e9d-139">Delegated Org</span></span> | [<span data-ttu-id="11e9d-140">设备代码提供程序</span><span class="sxs-lookup"><span data-stu-id="11e9d-140">Device Code Provider</span></span>](#DeviceCodeProvider) |
| [<span data-ttu-id="11e9d-141">守护程序应用</span><span class="sxs-lookup"><span data-stu-id="11e9d-141">Daemon app</span></span>](/azure/active-directory/develop/scenario-daemon-acquire-token) | | | |
| | <span data-ttu-id="11e9d-142">客户端凭据</span><span class="sxs-lookup"><span data-stu-id="11e9d-142">Client Credentials</span></span>  | <span data-ttu-id="11e9d-143">仅限应用</span><span class="sxs-lookup"><span data-stu-id="11e9d-143">App Only</span></span> | [<span data-ttu-id="11e9d-144">客户端凭据提供程序</span><span class="sxs-lookup"><span data-stu-id="11e9d-144">Client Credentials Provider</span></span>](#ClientCredentialsProvider) |
| [<span data-ttu-id="11e9d-145">调用 web Api 的移动应用程序</span><span class="sxs-lookup"><span data-stu-id="11e9d-145">Mobile app that calls web APIs</span></span>](/azure/active-directory/develop/scenario-mobile-acquire-token) | | | |
| | <span data-ttu-id="11e9d-146">Interactive</span><span class="sxs-lookup"><span data-stu-id="11e9d-146">Interactive</span></span> | <span data-ttu-id="11e9d-147">委派的消费者/组织</span><span class="sxs-lookup"><span data-stu-id="11e9d-147">Delegated Consumer/Org</span></span> | [<span data-ttu-id="11e9d-148">交互式提供程序</span><span class="sxs-lookup"><span data-stu-id="11e9d-148">Interactive Provider</span></span>](#InteractiveProvider) |


## <a name="authorization-code-provider"></a><a name="AuthCodeProvider" ></a><span data-ttu-id="11e9d-149">授权代码提供程序</span><span class="sxs-lookup"><span data-stu-id="11e9d-149">Authorization code provider</span></span>

<span data-ttu-id="11e9d-150">授权代码流使本机应用程序和 web 应用能够安全地获取用户名称中的令牌。</span><span class="sxs-lookup"><span data-stu-id="11e9d-150">The authorization code flow enables native and web apps to securely obtain tokens in the name of the user.</span></span> <span data-ttu-id="11e9d-151">若要了解详细信息，请参阅 [Microsoft identity platform 和 OAuth 2.0 授权代码流](/azure/active-directory/develop/v2-oauth2-auth-code-flow)。</span><span class="sxs-lookup"><span data-stu-id="11e9d-151">To learn more, see [Microsoft identity platform and OAuth 2.0 authorization code flow](/azure/active-directory/develop/v2-oauth2-auth-code-flow).</span></span>

# <a name="c"></a>[<span data-ttu-id="11e9d-152">C#</span><span class="sxs-lookup"><span data-stu-id="11e9d-152">C#</span></span>](#tab/CS)

```csharp
IConfidentialClientApplication confidentialClientApplication = ConfidentialClientApplicationBuilder
    .Create(clientId)
    .WithRedirectUri(redirectUri)
    .WithClientSecret(clientSecret) // or .WithCertificate(certificate)
    .Build();

AuthorizationCodeProvider authProvider = new AuthorizationCodeProvider(confidentialClientApplication, scopes);
```

# <a name="javascript"></a>[<span data-ttu-id="11e9d-153">Javascript</span><span class="sxs-lookup"><span data-stu-id="11e9d-153">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="11e9d-154">授权代码、客户端凭据和代表的 OAuth 流都要求您在此时实现自定义身份验证提供程序。</span><span class="sxs-lookup"><span data-stu-id="11e9d-154">Authorization code, client credential, and on-behalf-of OAuth flows require that you implement a custom authentication provider at this time.</span></span> <span data-ttu-id="11e9d-155">有关详细信息，请参阅 [使用自定义身份验证提供程序](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md)。</span><span class="sxs-lookup"><span data-stu-id="11e9d-155">For more information, see [Using a custom authentication provider](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md).</span></span>

# <a name="java"></a>[<span data-ttu-id="11e9d-156">Java</span><span class="sxs-lookup"><span data-stu-id="11e9d-156">Java</span></span>](#tab/Java)

```java
AuthorizationCodeProvider authProvider = new AuthorizationCodeProvider(
                                                    clientId,
                                                    scopes,
                                                    authorizationCode,
                                                    redirectUri,
                                                    clientSecret);
```

# <a name="android"></a>[<span data-ttu-id="11e9d-157">Android</span><span class="sxs-lookup"><span data-stu-id="11e9d-157">Android</span></span>](#tab/Android)

<span data-ttu-id="11e9d-158">不适用。</span><span class="sxs-lookup"><span data-stu-id="11e9d-158">Not applicable.</span></span>

# <a name="objective-c"></a>[<span data-ttu-id="11e9d-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="11e9d-159">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="11e9d-160">不适用。</span><span class="sxs-lookup"><span data-stu-id="11e9d-160">Not applicable.</span></span>

# <a name="php"></a>[<span data-ttu-id="11e9d-161">PHP</span><span class="sxs-lookup"><span data-stu-id="11e9d-161">PHP</span></span>](#tab/PHP)

<span data-ttu-id="11e9d-162">尚不可用。</span><span class="sxs-lookup"><span data-stu-id="11e9d-162">Not yet available.</span></span> <span data-ttu-id="11e9d-163">如果这对你非常重要，请支持或打开 [Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) 。</span><span class="sxs-lookup"><span data-stu-id="11e9d-163">Please support or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="ruby"></a>[<span data-ttu-id="11e9d-164">Ruby</span><span class="sxs-lookup"><span data-stu-id="11e9d-164">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="11e9d-165">尚不可用。</span><span class="sxs-lookup"><span data-stu-id="11e9d-165">Not available, yet.</span></span> <span data-ttu-id="11e9d-166">如果这对你非常重要，请投票或打开 [Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) 。</span><span class="sxs-lookup"><span data-stu-id="11e9d-166">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

##  <a name="client-credentials-provider"></a><a name="ClientCredentialsProvider"></a><span data-ttu-id="11e9d-167">客户端凭据提供程序</span><span class="sxs-lookup"><span data-stu-id="11e9d-167">Client credentials provider</span></span>

<span data-ttu-id="11e9d-168">客户端凭据流使服务应用程序可以在没有用户交互的情况下运行。</span><span class="sxs-lookup"><span data-stu-id="11e9d-168">The client credential flow enables service applications to run without user interaction.</span></span> <span data-ttu-id="11e9d-169">访问基于应用程序的标识。</span><span class="sxs-lookup"><span data-stu-id="11e9d-169">Access is based on the identity of the application.</span></span> <span data-ttu-id="11e9d-170">有关详细信息，请参阅 [Microsoft identity platform 和 OAuth 2.0 客户端凭据流](/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)。</span><span class="sxs-lookup"><span data-stu-id="11e9d-170">For more information, see [Microsoft identity platform and the OAuth 2.0 client credentials flow](/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow).</span></span>

# <a name="c"></a>[<span data-ttu-id="11e9d-171">C#</span><span class="sxs-lookup"><span data-stu-id="11e9d-171">C#</span></span>](#tab/CS)

```csharp
IConfidentialClientApplication confidentialClientApplication = ConfidentialClientApplicationBuilder
    .Create(clientId)
    .WithTenantId(tenantID)
    .WithClientSecret(clientSecret)
    .Build();

ClientCredentialProvider authProvider = new ClientCredentialProvider(confidentialClientApplication);
```

# <a name="javascript"></a>[<span data-ttu-id="11e9d-172">Javascript</span><span class="sxs-lookup"><span data-stu-id="11e9d-172">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="11e9d-173">授权代码、客户端凭据和代表的 OAuth 流都要求您在此时实现自定义身份验证提供程序。</span><span class="sxs-lookup"><span data-stu-id="11e9d-173">Authorization code, client credential, and on-behalf-of OAuth flows require that you implement a custom authentication provider at this time.</span></span> <span data-ttu-id="11e9d-174">有关详细信息，请参阅 [使用自定义身份验证提供程序](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md)。</span><span class="sxs-lookup"><span data-stu-id="11e9d-174">For more information, see [Using a custom authentication provider](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md).</span></span>

# <a name="java"></a>[<span data-ttu-id="11e9d-175">Java</span><span class="sxs-lookup"><span data-stu-id="11e9d-175">Java</span></span>](#tab/Java)

```java
ClientCredentialProvider authProvider = new ClientCredentialProvider(
                                                    clientId,
                                                    scopes,
                                                    clientSecret,
                                                    tenant,
                                                    NationalCloud.Global);
```

# <a name="android"></a>[<span data-ttu-id="11e9d-176">Android</span><span class="sxs-lookup"><span data-stu-id="11e9d-176">Android</span></span>](#tab/Android)

<span data-ttu-id="11e9d-177">不适用。</span><span class="sxs-lookup"><span data-stu-id="11e9d-177">Not applicable.</span></span>

# <a name="objective-c"></a>[<span data-ttu-id="11e9d-178">Objective-C</span><span class="sxs-lookup"><span data-stu-id="11e9d-178">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="11e9d-179">不适用。</span><span class="sxs-lookup"><span data-stu-id="11e9d-179">Not applicable.</span></span>

# <a name="php"></a>[<span data-ttu-id="11e9d-180">PHP</span><span class="sxs-lookup"><span data-stu-id="11e9d-180">PHP</span></span>](#tab/PHP)

<span data-ttu-id="11e9d-181">尚不可用。</span><span class="sxs-lookup"><span data-stu-id="11e9d-181">Not available, yet.</span></span> <span data-ttu-id="11e9d-182">如果这对你非常重要，请支持或打开 [Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) 。</span><span class="sxs-lookup"><span data-stu-id="11e9d-182">Please support or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="ruby"></a>[<span data-ttu-id="11e9d-183">Ruby</span><span class="sxs-lookup"><span data-stu-id="11e9d-183">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="11e9d-184">尚不可用。</span><span class="sxs-lookup"><span data-stu-id="11e9d-184">Not available, yet.</span></span> <span data-ttu-id="11e9d-185">如果这对你非常重要，请支持或打开 [Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) 。</span><span class="sxs-lookup"><span data-stu-id="11e9d-185">Please support or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

##  <a name="on-behalf-of-provider"></a><a name="OnBehalfOfProvider"></a><span data-ttu-id="11e9d-186">代表提供程序</span><span class="sxs-lookup"><span data-stu-id="11e9d-186">On-behalf-of provider</span></span>

<span data-ttu-id="11e9d-187">当应用程序调用在其中打开 Microsoft Graph API 的服务/web API 时，代表流是适用的。</span><span class="sxs-lookup"><span data-stu-id="11e9d-187">The on-behalf-of flow is applicable when your application calls a service/web API which in turns calls the Microsoft Graph API.</span></span> <span data-ttu-id="11e9d-188">若要了解详细信息，请阅读 [Microsoft identity platform 和 OAuth 2.0 代表流](/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow)</span><span class="sxs-lookup"><span data-stu-id="11e9d-188">Learn more by reading [Microsoft identity platform and OAuth 2.0 On-Behalf-Of flow](/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow)</span></span>

# <a name="c"></a>[<span data-ttu-id="11e9d-189">C#</span><span class="sxs-lookup"><span data-stu-id="11e9d-189">C#</span></span>](#tab/CS)

```csharp
IConfidentialClientApplication confidentialClientApplication = ConfidentialClientApplicationBuilder
    .Create(clientId)
    .WithRedirectUri(redirectUri)
    .WithClientSecret(clientSecret)
    .Build();

OnBehalfOfProvider authProvider = new OnBehalfOfProvider(confidentialClientApplication, scopes);
```

# <a name="javascript"></a>[<span data-ttu-id="11e9d-190">Javascript</span><span class="sxs-lookup"><span data-stu-id="11e9d-190">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="11e9d-191">授权代码、客户端凭据和代表的 OAuth 流都要求您在此时实现自定义身份验证提供程序。</span><span class="sxs-lookup"><span data-stu-id="11e9d-191">Authorization code, client credential, and on-behalf-of OAuth flows require that you implement a custom authentication provider at this time.</span></span> <span data-ttu-id="11e9d-192">有关详细信息，请参阅 [使用自定义身份验证提供程序](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md) 。</span><span class="sxs-lookup"><span data-stu-id="11e9d-192">Read [Using Custom Authentication Provider](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md) for more information.</span></span>

# <a name="java"></a>[<span data-ttu-id="11e9d-193">Java</span><span class="sxs-lookup"><span data-stu-id="11e9d-193">Java</span></span>](#tab/Java)

<span data-ttu-id="11e9d-194">尚不可用。</span><span class="sxs-lookup"><span data-stu-id="11e9d-194">Not yet available.</span></span> <span data-ttu-id="11e9d-195">如果这对你非常重要，请投票或打开 [Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) 。</span><span class="sxs-lookup"><span data-stu-id="11e9d-195">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="android"></a>[<span data-ttu-id="11e9d-196">Android</span><span class="sxs-lookup"><span data-stu-id="11e9d-196">Android</span></span>](#tab/Android)

<span data-ttu-id="11e9d-197">不适用。</span><span class="sxs-lookup"><span data-stu-id="11e9d-197">Not applicable.</span></span>

# <a name="objective-c"></a>[<span data-ttu-id="11e9d-198">Objective-C</span><span class="sxs-lookup"><span data-stu-id="11e9d-198">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="11e9d-199">不适用。</span><span class="sxs-lookup"><span data-stu-id="11e9d-199">Not applicable.</span></span>

# <a name="php"></a>[<span data-ttu-id="11e9d-200">PHP</span><span class="sxs-lookup"><span data-stu-id="11e9d-200">PHP</span></span>](#tab/PHP)

<span data-ttu-id="11e9d-201">尚不可用。</span><span class="sxs-lookup"><span data-stu-id="11e9d-201">Not yet available.</span></span> <span data-ttu-id="11e9d-202">如果这对你非常重要，请投票或打开 [Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) 。</span><span class="sxs-lookup"><span data-stu-id="11e9d-202">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="ruby"></a>[<span data-ttu-id="11e9d-203">Ruby</span><span class="sxs-lookup"><span data-stu-id="11e9d-203">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="11e9d-204">尚不可用。</span><span class="sxs-lookup"><span data-stu-id="11e9d-204">Not yet available.</span></span> <span data-ttu-id="11e9d-205">如果这对你非常重要，请投票或打开 [Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) 。</span><span class="sxs-lookup"><span data-stu-id="11e9d-205">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

## <a name="implicit-provider"></a><a name="ImplicitProvider"></a><span data-ttu-id="11e9d-206">隐式提供程序</span><span class="sxs-lookup"><span data-stu-id="11e9d-206">Implicit provider</span></span>

<span data-ttu-id="11e9d-207">隐式授予流在基于浏览器的应用程序中使用。</span><span class="sxs-lookup"><span data-stu-id="11e9d-207">The implicit grant flow is used in browser-based applications.</span></span> <span data-ttu-id="11e9d-208">有关详细信息，请参阅 [Microsoft identity platform 和隐式授予流](/azure/active-directory/develop/v2-oauth2-implicit-grant-flow)。</span><span class="sxs-lookup"><span data-stu-id="11e9d-208">For more information, see [Microsoft identity platform and Implicit grant flow](/azure/active-directory/develop/v2-oauth2-implicit-grant-flow).</span></span>

# <a name="c"></a>[<span data-ttu-id="11e9d-209">C#</span><span class="sxs-lookup"><span data-stu-id="11e9d-209">C#</span></span>](#tab/CS)

<span data-ttu-id="11e9d-210">不适用。</span><span class="sxs-lookup"><span data-stu-id="11e9d-210">Not applicable.</span></span>

# <a name="javascript"></a>[<span data-ttu-id="11e9d-211">Javascript</span><span class="sxs-lookup"><span data-stu-id="11e9d-211">Javascript</span></span>](#tab/Javascript)

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

# <a name="java"></a>[<span data-ttu-id="11e9d-212">Java</span><span class="sxs-lookup"><span data-stu-id="11e9d-212">Java</span></span>](#tab/Java)

<span data-ttu-id="11e9d-213">不适用。</span><span class="sxs-lookup"><span data-stu-id="11e9d-213">Not applicable.</span></span>

# <a name="android"></a>[<span data-ttu-id="11e9d-214">Android</span><span class="sxs-lookup"><span data-stu-id="11e9d-214">Android</span></span>](#tab/Android)

<span data-ttu-id="11e9d-215">不适用。</span><span class="sxs-lookup"><span data-stu-id="11e9d-215">Not applicable.</span></span>

# <a name="objective-c"></a>[<span data-ttu-id="11e9d-216">Objective-C</span><span class="sxs-lookup"><span data-stu-id="11e9d-216">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="11e9d-217">不适用。</span><span class="sxs-lookup"><span data-stu-id="11e9d-217">Not applicable.</span></span>

# <a name="php"></a>[<span data-ttu-id="11e9d-218">PHP</span><span class="sxs-lookup"><span data-stu-id="11e9d-218">PHP</span></span>](#tab/PHP)

<span data-ttu-id="11e9d-219">不适用。</span><span class="sxs-lookup"><span data-stu-id="11e9d-219">Not applicable.</span></span>

# <a name="ruby"></a>[<span data-ttu-id="11e9d-220">Ruby</span><span class="sxs-lookup"><span data-stu-id="11e9d-220">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="11e9d-221">不适用。</span><span class="sxs-lookup"><span data-stu-id="11e9d-221">Not applicable.</span></span>

---

##  <a name="device-code-provider"></a><a name="DeviceCodeProvider"></a><span data-ttu-id="11e9d-222">设备代码提供程序</span><span class="sxs-lookup"><span data-stu-id="11e9d-222">Device code provider</span></span>

<span data-ttu-id="11e9d-223">设备代码流允许通过其他设备登录设备。</span><span class="sxs-lookup"><span data-stu-id="11e9d-223">The device code flow enables sign in to devices by way of another device.</span></span> <span data-ttu-id="11e9d-224">有关详细信息，请参阅 [Microsoft identity platform 和 OAuth 2.0 设备代码流](/azure/active-directory/develop/v2-oauth2-device-code)。</span><span class="sxs-lookup"><span data-stu-id="11e9d-224">For details, see [Microsoft identity platform and the OAuth 2.0 device code flow](/azure/active-directory/develop/v2-oauth2-device-code).</span></span>

# <a name="c"></a>[<span data-ttu-id="11e9d-225">C#</span><span class="sxs-lookup"><span data-stu-id="11e9d-225">C#</span></span>](#tab/CS)

```csharp
IPublicClientApplication publicClientApplication = PublicClientApplicationBuilder
            .Create(clientId)
            .Build();

Func<DeviceCodeResult, Task> deviceCodeReadyCallback = async dcr => await Console.Out.WriteLineAsync(dcr.Message);

DeviceCodeProvider authProvider = new DeviceCodeProvider(publicClientApplication, scopes, deviceCodeReadyCallback);
```

# <a name="javascript"></a>[<span data-ttu-id="11e9d-226">Javascript</span><span class="sxs-lookup"><span data-stu-id="11e9d-226">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="11e9d-227">尚不可用。</span><span class="sxs-lookup"><span data-stu-id="11e9d-227">Not yet available.</span></span> <span data-ttu-id="11e9d-228">如果这对你非常重要，请投票或打开 [Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) 。</span><span class="sxs-lookup"><span data-stu-id="11e9d-228">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="java"></a>[<span data-ttu-id="11e9d-229">Java</span><span class="sxs-lookup"><span data-stu-id="11e9d-229">Java</span></span>](#tab/Java)

<span data-ttu-id="11e9d-230">尚不可用。</span><span class="sxs-lookup"><span data-stu-id="11e9d-230">Not available, yet.</span></span> <span data-ttu-id="11e9d-231">如果这对你非常重要，请支持或打开 [Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) 。</span><span class="sxs-lookup"><span data-stu-id="11e9d-231">Please support or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="android"></a>[<span data-ttu-id="11e9d-232">Android</span><span class="sxs-lookup"><span data-stu-id="11e9d-232">Android</span></span>](#tab/Android)

<span data-ttu-id="11e9d-233">不适用。</span><span class="sxs-lookup"><span data-stu-id="11e9d-233">Not applicable.</span></span>

# <a name="objective-c"></a>[<span data-ttu-id="11e9d-234">Objective-C</span><span class="sxs-lookup"><span data-stu-id="11e9d-234">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="11e9d-235">不适用。</span><span class="sxs-lookup"><span data-stu-id="11e9d-235">Not applicable.</span></span>

# <a name="php"></a>[<span data-ttu-id="11e9d-236">PHP</span><span class="sxs-lookup"><span data-stu-id="11e9d-236">PHP</span></span>](#tab/PHP)

<span data-ttu-id="11e9d-237">尚不可用。</span><span class="sxs-lookup"><span data-stu-id="11e9d-237">Not yet available.</span></span> <span data-ttu-id="11e9d-238">如果这对你非常重要，请投票或打开 [Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) 。</span><span class="sxs-lookup"><span data-stu-id="11e9d-238">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="ruby"></a>[<span data-ttu-id="11e9d-239">Ruby</span><span class="sxs-lookup"><span data-stu-id="11e9d-239">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="11e9d-240">尚不可用。</span><span class="sxs-lookup"><span data-stu-id="11e9d-240">Not yet available.</span></span> <span data-ttu-id="11e9d-241">如果这对你非常重要，请投票或打开 [Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) 。</span><span class="sxs-lookup"><span data-stu-id="11e9d-241">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

##  <a name="integrated-windows-provider"></a><a name="IntegratedWindowsProvider"></a><span data-ttu-id="11e9d-242">集成 Windows 提供程序</span><span class="sxs-lookup"><span data-stu-id="11e9d-242">Integrated Windows provider</span></span>

<span data-ttu-id="11e9d-243">集成的 Windows 流为 Windows 计算机提供了一种在加入域时无提示地获取访问令牌的方法。</span><span class="sxs-lookup"><span data-stu-id="11e9d-243">The integrated Windows flow provides a way for Windows computers to silently acquire an access token when they are domain joined.</span></span> <span data-ttu-id="11e9d-244">有关详细信息，请参阅 [集成 Windows 身份验证](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Integrated-Windows-Authentication)。</span><span class="sxs-lookup"><span data-stu-id="11e9d-244">For details, see [Integrated Windows authentication](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Integrated-Windows-Authentication).</span></span>

# <a name="c"></a>[<span data-ttu-id="11e9d-245">C#</span><span class="sxs-lookup"><span data-stu-id="11e9d-245">C#</span></span>](#tab/CS)

```csharp
IPublicClientApplication publicClientApplication = PublicClientApplicationBuilder
            .Create(clientId)
            .WithTenantId(tenantID)
            .Build();

IntegratedWindowsAuthenticationProvider authProvider = new IntegratedWindowsAuthenticationProvider(publicClientApplication, scopes);
```

# <a name="javascript"></a>[<span data-ttu-id="11e9d-246">Javascript</span><span class="sxs-lookup"><span data-stu-id="11e9d-246">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="11e9d-247">不适用。</span><span class="sxs-lookup"><span data-stu-id="11e9d-247">Not applicable.</span></span>

# <a name="java"></a>[<span data-ttu-id="11e9d-248">Java</span><span class="sxs-lookup"><span data-stu-id="11e9d-248">Java</span></span>](#tab/Java)

<span data-ttu-id="11e9d-249">不适用。</span><span class="sxs-lookup"><span data-stu-id="11e9d-249">Not applicable.</span></span>

# <a name="android"></a>[<span data-ttu-id="11e9d-250">Android</span><span class="sxs-lookup"><span data-stu-id="11e9d-250">Android</span></span>](#tab/Android)

<span data-ttu-id="11e9d-251">不适用。</span><span class="sxs-lookup"><span data-stu-id="11e9d-251">Not applicable.</span></span>

# <a name="objective-c"></a>[<span data-ttu-id="11e9d-252">Objective-C</span><span class="sxs-lookup"><span data-stu-id="11e9d-252">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="11e9d-253">不适用。</span><span class="sxs-lookup"><span data-stu-id="11e9d-253">Not applicable.</span></span>

# <a name="php"></a>[<span data-ttu-id="11e9d-254">PHP</span><span class="sxs-lookup"><span data-stu-id="11e9d-254">PHP</span></span>](#tab/PHP)

<span data-ttu-id="11e9d-255">不适用。</span><span class="sxs-lookup"><span data-stu-id="11e9d-255">Not applicable.</span></span>

# <a name="ruby"></a>[<span data-ttu-id="11e9d-256">Ruby</span><span class="sxs-lookup"><span data-stu-id="11e9d-256">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="11e9d-257">不适用。</span><span class="sxs-lookup"><span data-stu-id="11e9d-257">Not applicable.</span></span>

---

##  <a name="interactive-provider"></a><a name="InteractiveProvider"></a><span data-ttu-id="11e9d-258">交互式提供程序</span><span class="sxs-lookup"><span data-stu-id="11e9d-258">Interactive provider</span></span>

<span data-ttu-id="11e9d-259">移动应用程序 (Xamarin 和 UWP) 和桌面应用程序使用交互流，以在用户的名称中调用 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="11e9d-259">The interactive flow is used by mobile applications (Xamarin and UWP) and desktops applications to call Microsoft Graph in the name of a user.</span></span> <span data-ttu-id="11e9d-260">有关详细信息，请参阅 [以交互方式获取令牌](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Acquiring-tokens-interactively)。</span><span class="sxs-lookup"><span data-stu-id="11e9d-260">For details, see [Acquiring tokens interactively](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Acquiring-tokens-interactively).</span></span>

# <a name="c"></a>[<span data-ttu-id="11e9d-261">C#</span><span class="sxs-lookup"><span data-stu-id="11e9d-261">C#</span></span>](#tab/CS)

```csharp
IPublicClientApplication publicClientApplication = PublicClientApplicationBuilder
            .Create(clientId)
            .Build();

InteractiveAuthenticationProvider authProvider = new InteractiveAuthenticationProvider(publicClientApplication, scopes);
```

# <a name="javascript"></a>[<span data-ttu-id="11e9d-262">Javascript</span><span class="sxs-lookup"><span data-stu-id="11e9d-262">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="11e9d-263">尚不可用。</span><span class="sxs-lookup"><span data-stu-id="11e9d-263">Not yet available.</span></span> <span data-ttu-id="11e9d-264">如果这对你非常重要，请投票或打开 [Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) 。</span><span class="sxs-lookup"><span data-stu-id="11e9d-264">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="java"></a>[<span data-ttu-id="11e9d-265">Java</span><span class="sxs-lookup"><span data-stu-id="11e9d-265">Java</span></span>](#tab/Java)

<span data-ttu-id="11e9d-266">尚不可用。</span><span class="sxs-lookup"><span data-stu-id="11e9d-266">Not yet available.</span></span> <span data-ttu-id="11e9d-267">如果这对你非常重要，请投票或打开 [Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) 。</span><span class="sxs-lookup"><span data-stu-id="11e9d-267">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="android"></a>[<span data-ttu-id="11e9d-268">Android</span><span class="sxs-lookup"><span data-stu-id="11e9d-268">Android</span></span>](#tab/Android)

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

# <a name="objective-c"></a>[<span data-ttu-id="11e9d-269">Objective-C</span><span class="sxs-lookup"><span data-stu-id="11e9d-269">Objective-C</span></span>](#tab/Objective-C)

```objc
NSError *error = nil;
MSALPublicClientApplication *publicClientApplication = [[MSALPublicClientApplication alloc] initWithClientId:@"INSERT-CLIENT-APP-ID"
error:&error];

MSALAuthenticationProviderOptions *authProviderOptions= [[MSALAuthenticationProviderOptions alloc] initWithScopes:<array-of-scopes-for-which-you-need-access-token>];

 MSALAuthenticationProvider *authenticationProvider = [[MSALAuthenticationProvider alloc] initWithPublicClientApplication:publicClientApplication
 andOptions:authProviderOptions];
```

# <a name="php"></a>[<span data-ttu-id="11e9d-270">PHP</span><span class="sxs-lookup"><span data-stu-id="11e9d-270">PHP</span></span>](#tab/PHP)

<span data-ttu-id="11e9d-271">不适用。</span><span class="sxs-lookup"><span data-stu-id="11e9d-271">Not applicable.</span></span>

# <a name="ruby"></a>[<span data-ttu-id="11e9d-272">Ruby</span><span class="sxs-lookup"><span data-stu-id="11e9d-272">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="11e9d-273">不适用。</span><span class="sxs-lookup"><span data-stu-id="11e9d-273">Not applicable.</span></span>

---

##  <a name="usernamepassword-provider"></a><a name="UsernamePasswordProvider"></a><span data-ttu-id="11e9d-274">用户名/密码提供程序</span><span class="sxs-lookup"><span data-stu-id="11e9d-274">Username/password provider</span></span>

<span data-ttu-id="11e9d-275">用户名/密码提供程序允许应用程序使用用户名和密码登录用户。</span><span class="sxs-lookup"><span data-stu-id="11e9d-275">The username/password provider allows an application to sign in a user by using their username and password.</span></span> <span data-ttu-id="11e9d-276">仅当您不能使用任何其他 OAuth 流时，才使用此流。</span><span class="sxs-lookup"><span data-stu-id="11e9d-276">Use this flow only when you cannot use any of the other OAuth flows.</span></span> <span data-ttu-id="11e9d-277">有关详细信息，请参阅 [Microsoft identity platform 和 OAuth 2.0 资源所有者密码凭据](/azure/active-directory/develop/v2-oauth-ropc)</span><span class="sxs-lookup"><span data-stu-id="11e9d-277">For more information, see [Microsoft identity platform and the OAuth 2.0 resource owner password credential](/azure/active-directory/develop/v2-oauth-ropc)</span></span>



# <a name="c"></a>[<span data-ttu-id="11e9d-278">C#</span><span class="sxs-lookup"><span data-stu-id="11e9d-278">C#</span></span>](#tab/CS)

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

# <a name="javascript"></a>[<span data-ttu-id="11e9d-279">Javascript</span><span class="sxs-lookup"><span data-stu-id="11e9d-279">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="11e9d-280">尚不可用。</span><span class="sxs-lookup"><span data-stu-id="11e9d-280">Not yet available.</span></span> <span data-ttu-id="11e9d-281">如果这对你非常重要，请投票或打开 [Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) 。</span><span class="sxs-lookup"><span data-stu-id="11e9d-281">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="java"></a>[<span data-ttu-id="11e9d-282">Java</span><span class="sxs-lookup"><span data-stu-id="11e9d-282">Java</span></span>](#tab/Java)

```java
UsernamePasswordProvider authProvider = new UsernamePasswordProvider(
                                                    clientId,
                                                    scopes,
                                                    username,
                                                    password);
```

# <a name="android"></a>[<span data-ttu-id="11e9d-283">Android</span><span class="sxs-lookup"><span data-stu-id="11e9d-283">Android</span></span>](#tab/Android)

<span data-ttu-id="11e9d-284">不适用。</span><span class="sxs-lookup"><span data-stu-id="11e9d-284">Not applicable.</span></span>

# <a name="objective-c"></a>[<span data-ttu-id="11e9d-285">Objective-C</span><span class="sxs-lookup"><span data-stu-id="11e9d-285">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="11e9d-286">不适用。</span><span class="sxs-lookup"><span data-stu-id="11e9d-286">Not applicable.</span></span>

# <a name="php"></a>[<span data-ttu-id="11e9d-287">PHP</span><span class="sxs-lookup"><span data-stu-id="11e9d-287">PHP</span></span>](#tab/PHP)

<span data-ttu-id="11e9d-288">尚不可用。</span><span class="sxs-lookup"><span data-stu-id="11e9d-288">Not yet available.</span></span> <span data-ttu-id="11e9d-289">如果这对你非常重要，请投票或打开 [Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) 。</span><span class="sxs-lookup"><span data-stu-id="11e9d-289">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="ruby"></a>[<span data-ttu-id="11e9d-290">Ruby</span><span class="sxs-lookup"><span data-stu-id="11e9d-290">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="11e9d-291">尚不可用。</span><span class="sxs-lookup"><span data-stu-id="11e9d-291">Not yet available.</span></span> <span data-ttu-id="11e9d-292">如果这对你非常重要，请投票或打开 [Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) 。</span><span class="sxs-lookup"><span data-stu-id="11e9d-292">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

## <a name="next-steps"></a><span data-ttu-id="11e9d-293">后续步骤</span><span class="sxs-lookup"><span data-stu-id="11e9d-293">Next steps</span></span>

* <span data-ttu-id="11e9d-294">身份验证提供程序需要客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="11e9d-294">Authentication providers require an client ID.</span></span> <span data-ttu-id="11e9d-295">设置身份验证提供程序后，需要 [注册应用程序](https://portal.azure.com/) 。</span><span class="sxs-lookup"><span data-stu-id="11e9d-295">You'll want to [register your application](https://portal.azure.com/) after you set up your authentication provider.</span></span>
* <span data-ttu-id="11e9d-296">如果 [Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)目前不支持所需的 OAuth 流，请告知我们。</span><span class="sxs-lookup"><span data-stu-id="11e9d-296">Let us know if a required OAuth flow isn't currently supported by voting for or opening a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests).</span></span>
