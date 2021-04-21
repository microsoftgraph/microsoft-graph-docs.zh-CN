---
title: 选择 Microsoft Graph 身份验证提供程序
description: 了解如何为应用程序选择特定于方案的身份验证提供程序。
localization_priority: Normal
author: MichaelMainer
ms.openlocfilehash: 726fbf1334a99ab6a854bd4627052d154187105c
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921124"
---
# <a name="choose-a-microsoft-graph-authentication-provider-based-on-scenario"></a><span data-ttu-id="9d3eb-103">根据方案选择 Microsoft Graph 身份验证提供程序</span><span class="sxs-lookup"><span data-stu-id="9d3eb-103">Choose a Microsoft Graph authentication provider based on scenario</span></span>

<span data-ttu-id="9d3eb-104">身份验证提供程序使用 MICROSOFT 身份验证库和 MSAL 身份验证库实现获取 (所需的) ;处理增量同意、密码过期和条件访问等情况下的一些潜在错误;，然后设置 HTTP 请求授权标头。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-104">Authentication providers implement the code required to acquire a token using the Microsoft Authentication Library (MSAL); handle a number of potential errors for cases like incremental consent, expired passwords, and conditional access; and then set the HTTP request authorization header.</span></span> <span data-ttu-id="9d3eb-105">下表列出了一组与不同应用程序类型的方案匹配的 [提供程序](/azure/active-directory/develop/v2-app-types)。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-105">The following table lists the set of providers that match the scenarios for different [application types](/azure/active-directory/develop/v2-app-types).</span></span>

|<span data-ttu-id="9d3eb-106">方案</span><span class="sxs-lookup"><span data-stu-id="9d3eb-106">Scenario</span></span> | <span data-ttu-id="9d3eb-107">Flow/Grant</span><span class="sxs-lookup"><span data-stu-id="9d3eb-107">Flow/Grant</span></span> | <span data-ttu-id="9d3eb-108">受众</span><span class="sxs-lookup"><span data-stu-id="9d3eb-108">Audience</span></span> | <span data-ttu-id="9d3eb-109">提供程序</span><span class="sxs-lookup"><span data-stu-id="9d3eb-109">Provider</span></span>|
|--|--|--|--|
| [<span data-ttu-id="9d3eb-110">单页应用</span><span class="sxs-lookup"><span data-stu-id="9d3eb-110">Single Page App</span></span>](/azure/active-directory/develop/scenario-spa-acquire-token)| | | |
| | <span data-ttu-id="9d3eb-111">隐式</span><span class="sxs-lookup"><span data-stu-id="9d3eb-111">Implicit</span></span> | <span data-ttu-id="9d3eb-112">委派使用者/组织</span><span class="sxs-lookup"><span data-stu-id="9d3eb-112">Delegated Consumer/Org</span></span> |[<span data-ttu-id="9d3eb-113">隐式提供程序</span><span class="sxs-lookup"><span data-stu-id="9d3eb-113">Implicit Provider</span></span>](#ImplicitProvider) |
| [<span data-ttu-id="9d3eb-114">调用 Web API 的 Web 应用</span><span class="sxs-lookup"><span data-stu-id="9d3eb-114">Web App that calls web APIs</span></span>](/azure/active-directory/develop/scenario-web-app-call-api-acquire-token) | | | |
| | <span data-ttu-id="9d3eb-115">授权代码</span><span class="sxs-lookup"><span data-stu-id="9d3eb-115">Authorization Code</span></span> | <span data-ttu-id="9d3eb-116">委派使用者/组织</span><span class="sxs-lookup"><span data-stu-id="9d3eb-116">Delegated Consumer/Org</span></span> | [<span data-ttu-id="9d3eb-117">授权代码提供程序</span><span class="sxs-lookup"><span data-stu-id="9d3eb-117">Authorization Code Provider</span></span>](#AuthCodeProvider) |
| | <span data-ttu-id="9d3eb-118">客户端凭据</span><span class="sxs-lookup"><span data-stu-id="9d3eb-118">Client Credentials</span></span>  | <span data-ttu-id="9d3eb-119">仅限应用</span><span class="sxs-lookup"><span data-stu-id="9d3eb-119">App Only</span></span> | [<span data-ttu-id="9d3eb-120">客户端凭据提供程序</span><span class="sxs-lookup"><span data-stu-id="9d3eb-120">Client Credentials Provider</span></span>](#ClientCredentialsProvider) |
| [<span data-ttu-id="9d3eb-121">调用 Web API 的 Web API</span><span class="sxs-lookup"><span data-stu-id="9d3eb-121">Web API that calls web APIs</span></span>](/azure/active-directory/develop/scenario-web-api-call-api-acquire-token) | | | |
| | <span data-ttu-id="9d3eb-122">代表</span><span class="sxs-lookup"><span data-stu-id="9d3eb-122">On Behalf Of</span></span> | <span data-ttu-id="9d3eb-123">委派使用者/组织</span><span class="sxs-lookup"><span data-stu-id="9d3eb-123">Delegated Consumer/Org</span></span> | [<span data-ttu-id="9d3eb-124">代表提供商</span><span class="sxs-lookup"><span data-stu-id="9d3eb-124">On Behalf Of Provider</span></span>](#OnBehalfOfProvider) |
| | <span data-ttu-id="9d3eb-125">客户端凭据</span><span class="sxs-lookup"><span data-stu-id="9d3eb-125">Client Credentials</span></span>  | <span data-ttu-id="9d3eb-126">仅限应用</span><span class="sxs-lookup"><span data-stu-id="9d3eb-126">App Only</span></span> | [<span data-ttu-id="9d3eb-127">客户端凭据提供程序</span><span class="sxs-lookup"><span data-stu-id="9d3eb-127">Client Credentials Provider</span></span>](#ClientCredentialsProvider) |
| [<span data-ttu-id="9d3eb-128">调用 Web API 的桌面应用</span><span class="sxs-lookup"><span data-stu-id="9d3eb-128">Desktop app that calls web APIs</span></span>](/azure/active-directory/develop/scenario-desktop-acquire-token) | | | |
| | <span data-ttu-id="9d3eb-129">Interactive</span><span class="sxs-lookup"><span data-stu-id="9d3eb-129">Interactive</span></span> | <span data-ttu-id="9d3eb-130">委派使用者/组织</span><span class="sxs-lookup"><span data-stu-id="9d3eb-130">Delegated Consumer/Org</span></span> | [<span data-ttu-id="9d3eb-131">交互式提供程序</span><span class="sxs-lookup"><span data-stu-id="9d3eb-131">Interactive Provider</span></span>](#InteractiveProvider) |
| | <span data-ttu-id="9d3eb-132">集成 Windows</span><span class="sxs-lookup"><span data-stu-id="9d3eb-132">Integrated Windows</span></span> | <span data-ttu-id="9d3eb-133">委派组织</span><span class="sxs-lookup"><span data-stu-id="9d3eb-133">Delegated Org</span></span> | [<span data-ttu-id="9d3eb-134">集成 Windows 提供程序</span><span class="sxs-lookup"><span data-stu-id="9d3eb-134">Integrated Windows Provider</span></span>](#IntegratedWindowsProvider) |
| | <span data-ttu-id="9d3eb-135">资源所有者</span><span class="sxs-lookup"><span data-stu-id="9d3eb-135">Resource Owner</span></span>  | <span data-ttu-id="9d3eb-136">委派组织</span><span class="sxs-lookup"><span data-stu-id="9d3eb-136">Delegated Org</span></span> | [<span data-ttu-id="9d3eb-137">用户名/密码提供程序</span><span class="sxs-lookup"><span data-stu-id="9d3eb-137">Username / Password Provider</span></span>](#UsernamePasswordProvider) |
| | <span data-ttu-id="9d3eb-138">设备代码</span><span class="sxs-lookup"><span data-stu-id="9d3eb-138">Device Code</span></span>  | <span data-ttu-id="9d3eb-139">委派组织</span><span class="sxs-lookup"><span data-stu-id="9d3eb-139">Delegated Org</span></span> | [<span data-ttu-id="9d3eb-140">设备代码提供程序</span><span class="sxs-lookup"><span data-stu-id="9d3eb-140">Device Code Provider</span></span>](#DeviceCodeProvider) |
| [<span data-ttu-id="9d3eb-141">守护程序应用</span><span class="sxs-lookup"><span data-stu-id="9d3eb-141">Daemon app</span></span>](/azure/active-directory/develop/scenario-daemon-acquire-token) | | | |
| | <span data-ttu-id="9d3eb-142">客户端凭据</span><span class="sxs-lookup"><span data-stu-id="9d3eb-142">Client Credentials</span></span>  | <span data-ttu-id="9d3eb-143">仅限应用</span><span class="sxs-lookup"><span data-stu-id="9d3eb-143">App Only</span></span> | [<span data-ttu-id="9d3eb-144">客户端凭据提供程序</span><span class="sxs-lookup"><span data-stu-id="9d3eb-144">Client Credentials Provider</span></span>](#ClientCredentialsProvider) |
| [<span data-ttu-id="9d3eb-145">调用 Web API 的移动应用</span><span class="sxs-lookup"><span data-stu-id="9d3eb-145">Mobile app that calls web APIs</span></span>](/azure/active-directory/develop/scenario-mobile-acquire-token) | | | |
| | <span data-ttu-id="9d3eb-146">Interactive</span><span class="sxs-lookup"><span data-stu-id="9d3eb-146">Interactive</span></span> | <span data-ttu-id="9d3eb-147">委派使用者/组织</span><span class="sxs-lookup"><span data-stu-id="9d3eb-147">Delegated Consumer/Org</span></span> | [<span data-ttu-id="9d3eb-148">交互式提供程序</span><span class="sxs-lookup"><span data-stu-id="9d3eb-148">Interactive Provider</span></span>](#InteractiveProvider) |

> <span data-ttu-id="9d3eb-149">注意Java和 android 开发人员需要添加 [azure-identity](/java/api/overview/azure/identity-readme?view=azure-java-stable) 库才能访问不同的凭据类型。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-149">Note: Java and android developers need to add the [azure-identity](/java/api/overview/azure/identity-readme?view=azure-java-stable) library in order to get access to the different credentials types.</span></span>

## <a name="authorization-code-provider"></a><a name="AuthCodeProvider" ></a><span data-ttu-id="9d3eb-150">授权代码提供程序</span><span class="sxs-lookup"><span data-stu-id="9d3eb-150">Authorization code provider</span></span>

<span data-ttu-id="9d3eb-151">授权代码流使本机和 Web 应用能够安全地获取用户名称中的令牌。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-151">The authorization code flow enables native and web apps to securely obtain tokens in the name of the user.</span></span> <span data-ttu-id="9d3eb-152">若要了解更多信息，请参阅 [Microsoft 标识平台和 OAuth 2.0 授权代码流](/azure/active-directory/develop/v2-oauth2-auth-code-flow)。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-152">To learn more, see [Microsoft identity platform and OAuth 2.0 authorization code flow](/azure/active-directory/develop/v2-oauth2-auth-code-flow).</span></span>

# <a name="c"></a>[<span data-ttu-id="9d3eb-153">C#</span><span class="sxs-lookup"><span data-stu-id="9d3eb-153">C#</span></span>](#tab/CS)

```csharp
IConfidentialClientApplication confidentialClientApplication = ConfidentialClientApplicationBuilder
    .Create(clientId)
    .WithRedirectUri(redirectUri)
    .WithClientSecret(clientSecret) // or .WithCertificate(certificate)
    .Build();

AuthorizationCodeProvider authProvider = new AuthorizationCodeProvider(confidentialClientApplication, scopes);
```

# <a name="javascript"></a>[<span data-ttu-id="9d3eb-154">Javascript</span><span class="sxs-lookup"><span data-stu-id="9d3eb-154">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="9d3eb-155">授权代码、客户端凭据和代表 OAuth 流目前要求您实现自定义身份验证提供程序。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-155">Authorization code, client credential, and on-behalf-of OAuth flows require that you implement a custom authentication provider at this time.</span></span> <span data-ttu-id="9d3eb-156">有关详细信息，请参阅 [使用自定义身份验证提供程序](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md)。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-156">For more information, see [Using a custom authentication provider](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md).</span></span>

# <a name="java"></a>[<span data-ttu-id="9d3eb-157">Java</span><span class="sxs-lookup"><span data-stu-id="9d3eb-157">Java</span></span>](#tab/Java)

```java
final AuthorizationCodeCredential authCodeCredential = new AuthorizationCodeCredentialBuilder()
        .clientId(clientId)
        .clientSecret(clientSecret) //required for web apps, do not set for native apps
        .authorizationCode(authorizationCode)
        .redirectUrl(redirectUri)
        .build();

final TokenCredentialAuthProvider tokenCredentialAuthProvider = new TokenCredentialAuthProvider(scopes, authCodeCredential);

final GraphServiceClient graphClient =
  GraphServiceClient
    .builder()
    .authenticationProvider(tokenCredentialAuthProvider)
    .buildClient();

final User me = graphClient.me().buildRequest().get();
```

# <a name="android"></a>[<span data-ttu-id="9d3eb-158">Android</span><span class="sxs-lookup"><span data-stu-id="9d3eb-158">Android</span></span>](#tab/Android)

<span data-ttu-id="9d3eb-159">不适用。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-159">Not applicable.</span></span>

# <a name="objective-c"></a>[<span data-ttu-id="9d3eb-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9d3eb-160">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="9d3eb-161">不适用。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-161">Not applicable.</span></span>

# <a name="php"></a>[<span data-ttu-id="9d3eb-162">PHP</span><span class="sxs-lookup"><span data-stu-id="9d3eb-162">PHP</span></span>](#tab/PHP)

<span data-ttu-id="9d3eb-163">尚不可用。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-163">Not yet available.</span></span> <span data-ttu-id="9d3eb-164">如果这对你很重要，请支持或打开 [Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) 功能请求。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-164">Please support or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="ruby"></a>[<span data-ttu-id="9d3eb-165">Ruby</span><span class="sxs-lookup"><span data-stu-id="9d3eb-165">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="9d3eb-166">尚不可用。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-166">Not available, yet.</span></span> <span data-ttu-id="9d3eb-167">如果这对你很重要，请投票支持或打开 [Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) 功能请求。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-167">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

##  <a name="client-credentials-provider"></a><a name="ClientCredentialsProvider"></a><span data-ttu-id="9d3eb-168">客户端凭据提供程序</span><span class="sxs-lookup"><span data-stu-id="9d3eb-168">Client credentials provider</span></span>

<span data-ttu-id="9d3eb-169">客户端凭据流使服务应用程序无需用户交互即可运行。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-169">The client credential flow enables service applications to run without user interaction.</span></span> <span data-ttu-id="9d3eb-170">访问基于应用程序的标识。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-170">Access is based on the identity of the application.</span></span> <span data-ttu-id="9d3eb-171">有关详细信息，请参阅 [Microsoft 标识平台和 OAuth 2.0 客户端凭据流](/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-171">For more information, see [Microsoft identity platform and the OAuth 2.0 client credentials flow](/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow).</span></span>

# <a name="c"></a>[<span data-ttu-id="9d3eb-172">C#</span><span class="sxs-lookup"><span data-stu-id="9d3eb-172">C#</span></span>](#tab/CS)

```csharp
IConfidentialClientApplication confidentialClientApplication = ConfidentialClientApplicationBuilder
    .Create(clientId)
    .WithTenantId(tenantID)
    .WithClientSecret(clientSecret)
    .Build();

ClientCredentialProvider authProvider = new ClientCredentialProvider(confidentialClientApplication);
```

# <a name="javascript"></a>[<span data-ttu-id="9d3eb-173">Javascript</span><span class="sxs-lookup"><span data-stu-id="9d3eb-173">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="9d3eb-174">授权代码、客户端凭据和代表 OAuth 流目前要求您实现自定义身份验证提供程序。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-174">Authorization code, client credential, and on-behalf-of OAuth flows require that you implement a custom authentication provider at this time.</span></span> <span data-ttu-id="9d3eb-175">有关详细信息，请参阅 [使用自定义身份验证提供程序](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md)。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-175">For more information, see [Using a custom authentication provider](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md).</span></span>

# <a name="java"></a>[<span data-ttu-id="9d3eb-176">Java</span><span class="sxs-lookup"><span data-stu-id="9d3eb-176">Java</span></span>](#tab/Java)

```java
final ClientSecretCredential clientSecretCredential = new ClientSecretCredentialBuilder()
        .clientId(clientId)
        .clientSecret(clientSecret)
        .tenantId(tenant)
        .build();

final TokenCredentialAuthProvider tokenCredentialAuthProvider = new TokenCredentialAuthProvider(scopes, clientSecretCredential);

final GraphServiceClient graphClient =
  GraphServiceClient
    .builder()
    .authenticationProvider(tokenCredentialAuthProvider)
    .buildClient();

final User me = graphClient.me().buildRequest().get();
```

# <a name="android"></a>[<span data-ttu-id="9d3eb-177">Android</span><span class="sxs-lookup"><span data-stu-id="9d3eb-177">Android</span></span>](#tab/Android)

<span data-ttu-id="9d3eb-178">不适用。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-178">Not applicable.</span></span>

# <a name="objective-c"></a>[<span data-ttu-id="9d3eb-179">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9d3eb-179">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="9d3eb-180">不适用。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-180">Not applicable.</span></span>

# <a name="php"></a>[<span data-ttu-id="9d3eb-181">PHP</span><span class="sxs-lookup"><span data-stu-id="9d3eb-181">PHP</span></span>](#tab/PHP)

<span data-ttu-id="9d3eb-182">尚不可用。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-182">Not available, yet.</span></span> <span data-ttu-id="9d3eb-183">如果这对你很重要，请支持或打开 [Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) 功能请求。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-183">Please support or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="ruby"></a>[<span data-ttu-id="9d3eb-184">Ruby</span><span class="sxs-lookup"><span data-stu-id="9d3eb-184">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="9d3eb-185">尚不可用。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-185">Not available, yet.</span></span> <span data-ttu-id="9d3eb-186">如果这对你很重要，请支持或打开 [Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) 功能请求。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-186">Please support or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

##  <a name="on-behalf-of-provider"></a><a name="OnBehalfOfProvider"></a><span data-ttu-id="9d3eb-187">代表提供程序</span><span class="sxs-lookup"><span data-stu-id="9d3eb-187">On-behalf-of provider</span></span>

<span data-ttu-id="9d3eb-188">当应用程序调用服务/Web API 时，代表流适用，而服务/Web API 则调用 Microsoft Graph API。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-188">The on-behalf-of flow is applicable when your application calls a service/web API which in turns calls the Microsoft Graph API.</span></span> <span data-ttu-id="9d3eb-189">通过阅读 [Microsoft 标识平台和 OAuth 2.0 代表流了解更多信息](/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow)</span><span class="sxs-lookup"><span data-stu-id="9d3eb-189">Learn more by reading [Microsoft identity platform and OAuth 2.0 On-Behalf-Of flow](/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow)</span></span>

# <a name="c"></a>[<span data-ttu-id="9d3eb-190">C#</span><span class="sxs-lookup"><span data-stu-id="9d3eb-190">C#</span></span>](#tab/CS)

```csharp
IConfidentialClientApplication confidentialClientApplication = ConfidentialClientApplicationBuilder
    .Create(clientId)
    .WithRedirectUri(redirectUri)
    .WithClientSecret(clientSecret)
    .Build();

OnBehalfOfProvider authProvider = new OnBehalfOfProvider(confidentialClientApplication, scopes);
```

# <a name="javascript"></a>[<span data-ttu-id="9d3eb-191">Javascript</span><span class="sxs-lookup"><span data-stu-id="9d3eb-191">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="9d3eb-192">授权代码、客户端凭据和代表 OAuth 流目前要求您实现自定义身份验证提供程序。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-192">Authorization code, client credential, and on-behalf-of OAuth flows require that you implement a custom authentication provider at this time.</span></span> <span data-ttu-id="9d3eb-193">有关详细信息 [，请参阅](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md) 使用自定义验证提供程序。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-193">Read [Using Custom Authentication Provider](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md) for more information.</span></span>

# <a name="java"></a>[<span data-ttu-id="9d3eb-194">Java</span><span class="sxs-lookup"><span data-stu-id="9d3eb-194">Java</span></span>](#tab/Java)

<span data-ttu-id="9d3eb-195">尚不可用。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-195">Not yet available.</span></span> <span data-ttu-id="9d3eb-196">如果这对你很重要，请投票支持或打开 [Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) 功能请求。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-196">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="android"></a>[<span data-ttu-id="9d3eb-197">Android</span><span class="sxs-lookup"><span data-stu-id="9d3eb-197">Android</span></span>](#tab/Android)

<span data-ttu-id="9d3eb-198">不适用。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-198">Not applicable.</span></span>

# <a name="objective-c"></a>[<span data-ttu-id="9d3eb-199">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9d3eb-199">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="9d3eb-200">不适用。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-200">Not applicable.</span></span>

# <a name="php"></a>[<span data-ttu-id="9d3eb-201">PHP</span><span class="sxs-lookup"><span data-stu-id="9d3eb-201">PHP</span></span>](#tab/PHP)

<span data-ttu-id="9d3eb-202">尚不可用。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-202">Not yet available.</span></span> <span data-ttu-id="9d3eb-203">如果这对你很重要，请投票支持或打开 [Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) 功能请求。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-203">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="ruby"></a>[<span data-ttu-id="9d3eb-204">Ruby</span><span class="sxs-lookup"><span data-stu-id="9d3eb-204">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="9d3eb-205">尚不可用。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-205">Not yet available.</span></span> <span data-ttu-id="9d3eb-206">如果这对你很重要，请投票支持或打开 [Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) 功能请求。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-206">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

## <a name="implicit-provider"></a><a name="ImplicitProvider"></a><span data-ttu-id="9d3eb-207">隐式提供程序</span><span class="sxs-lookup"><span data-stu-id="9d3eb-207">Implicit provider</span></span>

<span data-ttu-id="9d3eb-208">隐式授予流用于基于浏览器的应用程序。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-208">The implicit grant flow is used in browser-based applications.</span></span> <span data-ttu-id="9d3eb-209">有关详细信息，请参阅 [Microsoft 标识平台和隐式授权流](/azure/active-directory/develop/v2-oauth2-implicit-grant-flow)。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-209">For more information, see [Microsoft identity platform and Implicit grant flow](/azure/active-directory/develop/v2-oauth2-implicit-grant-flow).</span></span>

# <a name="c"></a>[<span data-ttu-id="9d3eb-210">C#</span><span class="sxs-lookup"><span data-stu-id="9d3eb-210">C#</span></span>](#tab/CS)

<span data-ttu-id="9d3eb-211">不适用。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-211">Not applicable.</span></span>

# <a name="javascript"></a>[<span data-ttu-id="9d3eb-212">Javascript</span><span class="sxs-lookup"><span data-stu-id="9d3eb-212">Javascript</span></span>](#tab/Javascript)

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

# <a name="java"></a>[<span data-ttu-id="9d3eb-213">Java</span><span class="sxs-lookup"><span data-stu-id="9d3eb-213">Java</span></span>](#tab/Java)

<span data-ttu-id="9d3eb-214">不适用。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-214">Not applicable.</span></span>

# <a name="android"></a>[<span data-ttu-id="9d3eb-215">Android</span><span class="sxs-lookup"><span data-stu-id="9d3eb-215">Android</span></span>](#tab/Android)

<span data-ttu-id="9d3eb-216">不适用。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-216">Not applicable.</span></span>

# <a name="objective-c"></a>[<span data-ttu-id="9d3eb-217">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9d3eb-217">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="9d3eb-218">不适用。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-218">Not applicable.</span></span>

# <a name="php"></a>[<span data-ttu-id="9d3eb-219">PHP</span><span class="sxs-lookup"><span data-stu-id="9d3eb-219">PHP</span></span>](#tab/PHP)

<span data-ttu-id="9d3eb-220">不适用。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-220">Not applicable.</span></span>

# <a name="ruby"></a>[<span data-ttu-id="9d3eb-221">Ruby</span><span class="sxs-lookup"><span data-stu-id="9d3eb-221">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="9d3eb-222">不适用。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-222">Not applicable.</span></span>

---

##  <a name="device-code-provider"></a><a name="DeviceCodeProvider"></a><span data-ttu-id="9d3eb-223">设备代码提供程序</span><span class="sxs-lookup"><span data-stu-id="9d3eb-223">Device code provider</span></span>

<span data-ttu-id="9d3eb-224">设备代码流允许通过另一台设备登录到设备。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-224">The device code flow enables sign in to devices by way of another device.</span></span> <span data-ttu-id="9d3eb-225">有关详细信息，请参阅 [Microsoft 标识平台和 OAuth 2.0 设备代码流](/azure/active-directory/develop/v2-oauth2-device-code)。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-225">For details, see [Microsoft identity platform and the OAuth 2.0 device code flow](/azure/active-directory/develop/v2-oauth2-device-code).</span></span>

# <a name="c"></a>[<span data-ttu-id="9d3eb-226">C#</span><span class="sxs-lookup"><span data-stu-id="9d3eb-226">C#</span></span>](#tab/CS)

```csharp
IPublicClientApplication publicClientApplication = PublicClientApplicationBuilder
            .Create(clientId)
            .Build();

Func<DeviceCodeResult, Task> deviceCodeReadyCallback = async dcr => await Console.Out.WriteLineAsync(dcr.Message);

DeviceCodeProvider authProvider = new DeviceCodeProvider(publicClientApplication, scopes, deviceCodeReadyCallback);
```

# <a name="javascript"></a>[<span data-ttu-id="9d3eb-227">Javascript</span><span class="sxs-lookup"><span data-stu-id="9d3eb-227">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="9d3eb-228">尚不可用。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-228">Not yet available.</span></span> <span data-ttu-id="9d3eb-229">如果这对你很重要，请投票支持或打开 [Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) 功能请求。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-229">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="java"></a>[<span data-ttu-id="9d3eb-230">Java</span><span class="sxs-lookup"><span data-stu-id="9d3eb-230">Java</span></span>](#tab/Java)

```java
final DeviceCodeCredential deviceCodeCredential = new DeviceCodeCredentialBuilder()
                    .clientId(clientId)
                    .challengeConsumer(challenge -> {
                        // lets user know of the challenge
                        System.out.println(challenge.getMessage());
                    })
                    .build();
final TokenCredentialAuthProvider tokenCredentialAuthProvider = new TokenCredentialAuthProvider(scopes, deviceCodeCredential);

final GraphServiceClient graphClient =
  GraphServiceClient
    .builder()
    .authenticationProvider(tokenCredentialAuthProvider)
    .buildClient();

final User me = graphClient.me().buildRequest().get();
```

# <a name="android"></a>[<span data-ttu-id="9d3eb-231">Android</span><span class="sxs-lookup"><span data-stu-id="9d3eb-231">Android</span></span>](#tab/Android)

<span data-ttu-id="9d3eb-232">不适用。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-232">Not applicable.</span></span>

# <a name="objective-c"></a>[<span data-ttu-id="9d3eb-233">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9d3eb-233">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="9d3eb-234">不适用。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-234">Not applicable.</span></span>

# <a name="php"></a>[<span data-ttu-id="9d3eb-235">PHP</span><span class="sxs-lookup"><span data-stu-id="9d3eb-235">PHP</span></span>](#tab/PHP)

<span data-ttu-id="9d3eb-236">尚不可用。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-236">Not yet available.</span></span> <span data-ttu-id="9d3eb-237">如果这对你很重要，请投票支持或打开 [Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) 功能请求。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-237">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="ruby"></a>[<span data-ttu-id="9d3eb-238">Ruby</span><span class="sxs-lookup"><span data-stu-id="9d3eb-238">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="9d3eb-239">尚不可用。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-239">Not yet available.</span></span> <span data-ttu-id="9d3eb-240">如果这对你很重要，请投票支持或打开 [Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) 功能请求。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-240">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

##  <a name="integrated-windows-provider"></a><a name="IntegratedWindowsProvider"></a><span data-ttu-id="9d3eb-241">集成 Windows 提供程序</span><span class="sxs-lookup"><span data-stu-id="9d3eb-241">Integrated Windows provider</span></span>

<span data-ttu-id="9d3eb-242">集成 Windows 流为 Windows 计算机提供了一种在加入域时以静默方式获取访问令牌的方法。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-242">The integrated Windows flow provides a way for Windows computers to silently acquire an access token when they are domain joined.</span></span> <span data-ttu-id="9d3eb-243">有关详细信息，请参阅集成 [Windows 身份验证](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Integrated-Windows-Authentication)。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-243">For details, see [Integrated Windows authentication](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Integrated-Windows-Authentication).</span></span>

# <a name="c"></a>[<span data-ttu-id="9d3eb-244">C#</span><span class="sxs-lookup"><span data-stu-id="9d3eb-244">C#</span></span>](#tab/CS)

```csharp
IPublicClientApplication publicClientApplication = PublicClientApplicationBuilder
            .Create(clientId)
            .WithTenantId(tenantID)
            .Build();

IntegratedWindowsAuthenticationProvider authProvider = new IntegratedWindowsAuthenticationProvider(publicClientApplication, scopes);
```

# <a name="javascript"></a>[<span data-ttu-id="9d3eb-245">Javascript</span><span class="sxs-lookup"><span data-stu-id="9d3eb-245">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="9d3eb-246">不适用。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-246">Not applicable.</span></span>

# <a name="java"></a>[<span data-ttu-id="9d3eb-247">Java</span><span class="sxs-lookup"><span data-stu-id="9d3eb-247">Java</span></span>](#tab/Java)

<span data-ttu-id="9d3eb-248">不适用。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-248">Not applicable.</span></span>

# <a name="android"></a>[<span data-ttu-id="9d3eb-249">Android</span><span class="sxs-lookup"><span data-stu-id="9d3eb-249">Android</span></span>](#tab/Android)

<span data-ttu-id="9d3eb-250">不适用。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-250">Not applicable.</span></span>

# <a name="objective-c"></a>[<span data-ttu-id="9d3eb-251">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9d3eb-251">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="9d3eb-252">不适用。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-252">Not applicable.</span></span>

# <a name="php"></a>[<span data-ttu-id="9d3eb-253">PHP</span><span class="sxs-lookup"><span data-stu-id="9d3eb-253">PHP</span></span>](#tab/PHP)

<span data-ttu-id="9d3eb-254">不适用。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-254">Not applicable.</span></span>

# <a name="ruby"></a>[<span data-ttu-id="9d3eb-255">Ruby</span><span class="sxs-lookup"><span data-stu-id="9d3eb-255">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="9d3eb-256">不适用。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-256">Not applicable.</span></span>

---

##  <a name="interactive-provider"></a><a name="InteractiveProvider"></a><span data-ttu-id="9d3eb-257">交互式提供程序</span><span class="sxs-lookup"><span data-stu-id="9d3eb-257">Interactive provider</span></span>

<span data-ttu-id="9d3eb-258">交互流由 Xamarin (UWP) 桌面应用程序使用，以用户名称调用 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-258">The interactive flow is used by mobile applications (Xamarin and UWP) and desktops applications to call Microsoft Graph in the name of a user.</span></span> <span data-ttu-id="9d3eb-259">有关详细信息，请参阅 [以交互方式获取令牌](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Acquiring-tokens-interactively)。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-259">For details, see [Acquiring tokens interactively](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Acquiring-tokens-interactively).</span></span>

# <a name="c"></a>[<span data-ttu-id="9d3eb-260">C#</span><span class="sxs-lookup"><span data-stu-id="9d3eb-260">C#</span></span>](#tab/CS)

```csharp
IPublicClientApplication publicClientApplication = PublicClientApplicationBuilder
            .Create(clientId)
            .Build();

InteractiveAuthenticationProvider authProvider = new InteractiveAuthenticationProvider(publicClientApplication, scopes);
```

# <a name="javascript"></a>[<span data-ttu-id="9d3eb-261">Javascript</span><span class="sxs-lookup"><span data-stu-id="9d3eb-261">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="9d3eb-262">尚不可用。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-262">Not yet available.</span></span> <span data-ttu-id="9d3eb-263">如果这对你很重要，请投票支持或打开 [Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) 功能请求。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-263">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="java"></a>[<span data-ttu-id="9d3eb-264">Java</span><span class="sxs-lookup"><span data-stu-id="9d3eb-264">Java</span></span>](#tab/Java)

```java
final InteractiveBrowserCredential interactiveBrowserCredential = new InteractiveBrowserCredentialBuilder()
                .clientId(clientId)
                .redirectUrl("http://localhost:8765")
                .build();
final TokenCredentialAuthProvider tokenCredentialAuthProvider = new TokenCredentialAuthProvider(scopes, interactiveBrowserCredential);

final GraphServiceClient graphClient =
  GraphServiceClient
    .builder()
    .authenticationProvider(tokenCredentialAuthProvider)
    .buildClient();

final User me = graphClient.me().buildRequest().get();
```

# <a name="android"></a>[<span data-ttu-id="9d3eb-265">Android</span><span class="sxs-lookup"><span data-stu-id="9d3eb-265">Android</span></span>](#tab/Android)

```java
final InteractiveBrowserCredential interactiveBrowserCredential = new InteractiveBrowserCredentialBuilder()
                .clientId(clientId)
                .redirectUrl("http://localhost:8765")
                .build();
final TokenCredentialAuthProvider tokenCredentialAuthProvider = new TokenCredentialAuthProvider(scopes, interactiveBrowserCredential);

final GraphServiceClient graphClient =
  GraphServiceClient
    .builder()
    .authenticationProvider(tokenCredentialAuthProvider)
    .buildClient();

final User me = graphClient.me().buildRequest().get();
```

# <a name="objective-c"></a>[<span data-ttu-id="9d3eb-266">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9d3eb-266">Objective-C</span></span>](#tab/Objective-C)

```objc
NSError *error = nil;
MSALPublicClientApplication *publicClientApplication = [[MSALPublicClientApplication alloc] initWithClientId:@"INSERT-CLIENT-APP-ID"
error:&error];

MSALAuthenticationProviderOptions *authProviderOptions= [[MSALAuthenticationProviderOptions alloc] initWithScopes:<array-of-scopes-for-which-you-need-access-token>];

 MSALAuthenticationProvider *authenticationProvider = [[MSALAuthenticationProvider alloc] initWithPublicClientApplication:publicClientApplication
 andOptions:authProviderOptions];
```

# <a name="php"></a>[<span data-ttu-id="9d3eb-267">PHP</span><span class="sxs-lookup"><span data-stu-id="9d3eb-267">PHP</span></span>](#tab/PHP)

<span data-ttu-id="9d3eb-268">不适用。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-268">Not applicable.</span></span>

# <a name="ruby"></a>[<span data-ttu-id="9d3eb-269">Ruby</span><span class="sxs-lookup"><span data-stu-id="9d3eb-269">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="9d3eb-270">不适用。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-270">Not applicable.</span></span>

---

##  <a name="usernamepassword-provider"></a><a name="UsernamePasswordProvider"></a><span data-ttu-id="9d3eb-271">用户名/密码提供程序</span><span class="sxs-lookup"><span data-stu-id="9d3eb-271">Username/password provider</span></span>

<span data-ttu-id="9d3eb-272">用户名/密码提供程序允许应用程序使用用户的用户名和密码登录。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-272">The username/password provider allows an application to sign in a user by using their username and password.</span></span> <span data-ttu-id="9d3eb-273">只有在不能使用任何其他 OAuth 流时，才使用此流。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-273">Use this flow only when you cannot use any of the other OAuth flows.</span></span> <span data-ttu-id="9d3eb-274">有关详细信息，请参阅 [Microsoft 标识平台和 OAuth 2.0 资源所有者密码凭据](/azure/active-directory/develop/v2-oauth-ropc)</span><span class="sxs-lookup"><span data-stu-id="9d3eb-274">For more information, see [Microsoft identity platform and the OAuth 2.0 resource owner password credential](/azure/active-directory/develop/v2-oauth-ropc)</span></span>



# <a name="c"></a>[<span data-ttu-id="9d3eb-275">C#</span><span class="sxs-lookup"><span data-stu-id="9d3eb-275">C#</span></span>](#tab/CS)

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

# <a name="javascript"></a>[<span data-ttu-id="9d3eb-276">Javascript</span><span class="sxs-lookup"><span data-stu-id="9d3eb-276">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="9d3eb-277">尚不可用。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-277">Not yet available.</span></span> <span data-ttu-id="9d3eb-278">如果这对你很重要，请投票支持或打开 [Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) 功能请求。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-278">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="java"></a>[<span data-ttu-id="9d3eb-279">Java</span><span class="sxs-lookup"><span data-stu-id="9d3eb-279">Java</span></span>](#tab/Java)

```java
final UsernamePasswordCredential usernamePasswordCredential = new UsernamePasswordCredentialBuilder()
        .clientId(clientId)
        .username(username)
        .password(password)
        .build();

final TokenCredentialAuthProvider tokenCredentialAuthProvider = new TokenCredentialAuthProvider(scopes, usernamePasswordCredential);

final GraphServiceClient graphClient =
  GraphServiceClient
    .builder()
    .authenticationProvider(tokenCredentialAuthProvider)
    .buildClient();

final User me = graphClient.me().buildRequest().get();
```

# <a name="android"></a>[<span data-ttu-id="9d3eb-280">Android</span><span class="sxs-lookup"><span data-stu-id="9d3eb-280">Android</span></span>](#tab/Android)

<span data-ttu-id="9d3eb-281">不适用。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-281">Not applicable.</span></span>

# <a name="objective-c"></a>[<span data-ttu-id="9d3eb-282">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9d3eb-282">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="9d3eb-283">不适用。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-283">Not applicable.</span></span>

# <a name="php"></a>[<span data-ttu-id="9d3eb-284">PHP</span><span class="sxs-lookup"><span data-stu-id="9d3eb-284">PHP</span></span>](#tab/PHP)

<span data-ttu-id="9d3eb-285">尚不可用。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-285">Not yet available.</span></span> <span data-ttu-id="9d3eb-286">如果这对你很重要，请投票支持或打开 [Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) 功能请求。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-286">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="ruby"></a>[<span data-ttu-id="9d3eb-287">Ruby</span><span class="sxs-lookup"><span data-stu-id="9d3eb-287">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="9d3eb-288">尚不可用。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-288">Not yet available.</span></span> <span data-ttu-id="9d3eb-289">如果这对你很重要，请投票支持或打开 [Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) 功能请求。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-289">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

## <a name="next-steps"></a><span data-ttu-id="9d3eb-290">后续步骤</span><span class="sxs-lookup"><span data-stu-id="9d3eb-290">Next steps</span></span>

* <span data-ttu-id="9d3eb-291">身份验证提供程序需要客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-291">Authentication providers require an client ID.</span></span> <span data-ttu-id="9d3eb-292">设置身份验证 [提供程序后](https://portal.azure.com/) ，需要注册应用程序。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-292">You'll want to [register your application](https://portal.azure.com/) after you set up your authentication provider.</span></span>
* <span data-ttu-id="9d3eb-293">通过投票或打开 Microsoft Graph 功能请求，告诉我们当前是否不支持所需的 [OAuth 流](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)。</span><span class="sxs-lookup"><span data-stu-id="9d3eb-293">Let us know if a required OAuth flow isn't currently supported by voting for or opening a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests).</span></span>