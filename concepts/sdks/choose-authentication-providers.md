---
title: 选择 Microsoft Graph 身份验证提供程序
description: 了解如何为您的应用程序选择特定于方案的身份验证提供程序。
localization_priority: Normal
author: MichaelMainer
ms.openlocfilehash: 5061b38249f31a6eea959ecec94899337bf57326
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33630193"
---
# <a name="choose-a-microsoft-graph-authentication-provider-based-on-oauth-flow"></a><span data-ttu-id="6df6c-103">根据 OAuth 流选择 Microsoft Graph 身份验证提供程序</span><span class="sxs-lookup"><span data-stu-id="6df6c-103">Choose a Microsoft Graph authentication provider based on OAuth flow</span></span>

<span data-ttu-id="6df6c-104">身份验证提供程序通过抽象身份验证客户端库所需的参数简化了获取访问令牌的方法。</span><span class="sxs-lookup"><span data-stu-id="6df6c-104">Authentication providers simplify getting an access token by abstracting the parameters required by the authentication client libraries.</span></span> <span data-ttu-id="6df6c-105">Microsoft Graph 身份验证提供程序通过为每个平台提供适配器简化了 Microsoft 身份验证库 (MSAL) 的使用。</span><span class="sxs-lookup"><span data-stu-id="6df6c-105">The Microsoft Graph authentication providers simplify the use of the Microsoft Authentication Library (MSAL) by providing adapters for each platform.</span></span> <span data-ttu-id="6df6c-106">这些适配器处理应用程序的令牌获取。</span><span class="sxs-lookup"><span data-stu-id="6df6c-106">These adapters handle token acquisition for your application.</span></span> <span data-ttu-id="6df6c-107">Microsoft Graph 身份验证提供程序映射到 OAuth 授予流。</span><span class="sxs-lookup"><span data-stu-id="6df6c-107">The Microsoft Graph authentication providers map to an OAuth grant flow.</span></span> <span data-ttu-id="6df6c-108">您需要知道要用于应用程序的 OAuth 授予流, 以便为您的应用程序选择适当的身份验证提供程序。</span><span class="sxs-lookup"><span data-stu-id="6df6c-108">You'll need to know which OAuth grant flow to use for your application in order to select the appropriate authentication provider for your application.</span></span>

## <a name="authorization-code-oauth-flow"></a><span data-ttu-id="6df6c-109">授权代码 OAuth 流</span><span class="sxs-lookup"><span data-stu-id="6df6c-109">Authorization code OAuth flow</span></span>

<span data-ttu-id="6df6c-110">授权代码流使本机应用程序和 web 应用能够安全地获取用户名称中的令牌。</span><span class="sxs-lookup"><span data-stu-id="6df6c-110">The authorization code flow enables native and web apps to securely obtain tokens in the name of the user.</span></span> <span data-ttu-id="6df6c-111">若要了解详细信息, 请参阅[Microsoft identity platform 和 OAuth 2.0 授权代码流](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-auth-code-flow)。</span><span class="sxs-lookup"><span data-stu-id="6df6c-111">To learn more, see [Microsoft identity platform and OAuth 2.0 authorization code flow](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-auth-code-flow).</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="6df6c-112">语言</span><span class="sxs-lookup"><span data-stu-id="6df6c-112">C#</span></span>](#tab/CS)

```csharp
IConfidentialClientApplication clientApplication = AuthorizationCodeProvider.CreateClientApplication(clientId, redirectUri, clientCredential);
AuthorizationCodeProvider authProvider = new AuthorizationCodeProvider(clientApplication, scopes);
```

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6df6c-113">Javascript</span><span class="sxs-lookup"><span data-stu-id="6df6c-113">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="6df6c-114">授权代码、客户端凭据和代表的 OAuth 流都要求您在此时实现自定义身份验证提供程序。</span><span class="sxs-lookup"><span data-stu-id="6df6c-114">Authorization code, client credential, and on-behalf-of OAuth flows require that you implement a custom authentication provider at this time.</span></span> <span data-ttu-id="6df6c-115">有关详细信息, 请参阅[使用自定义身份验证提供程序](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md)。</span><span class="sxs-lookup"><span data-stu-id="6df6c-115">For more information, see [Using a custom authentication provider](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md).</span></span>

# <a name="javatabjava"></a>[<span data-ttu-id="6df6c-116">Java</span><span class="sxs-lookup"><span data-stu-id="6df6c-116">Java</span></span>](#tab/Java)

```java
AuthorizationCodeProvider authProvider = new AuthorizationCodeProvider(
                                                    clientId,
                                                    scopes,
                                                    authorizationCode,
                                                    redirectUri,
                                                    clientSecret);
```

# <a name="androidtabandroid"></a>[<span data-ttu-id="6df6c-117">Android</span><span class="sxs-lookup"><span data-stu-id="6df6c-117">Android</span></span>](#tab/Android)

<span data-ttu-id="6df6c-118">不适用。</span><span class="sxs-lookup"><span data-stu-id="6df6c-118">Not applicable.</span></span>

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="6df6c-119">目标-C</span><span class="sxs-lookup"><span data-stu-id="6df6c-119">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="6df6c-120">不适用。</span><span class="sxs-lookup"><span data-stu-id="6df6c-120">Not applicable.</span></span>

# <a name="phptabphp"></a>[<span data-ttu-id="6df6c-121">PHP</span><span class="sxs-lookup"><span data-stu-id="6df6c-121">PHP</span></span>](#tab/PHP)

<span data-ttu-id="6df6c-122">尚不可用。</span><span class="sxs-lookup"><span data-stu-id="6df6c-122">Not yet available.</span></span> <span data-ttu-id="6df6c-123">如果这对你非常重要, 请支持或打开[Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)。</span><span class="sxs-lookup"><span data-stu-id="6df6c-123">Please support or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="6df6c-124">Ruby</span><span class="sxs-lookup"><span data-stu-id="6df6c-124">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="6df6c-125">尚不可用。</span><span class="sxs-lookup"><span data-stu-id="6df6c-125">Not available, yet.</span></span> <span data-ttu-id="6df6c-126">如果这对你非常重要, 请投票或打开[Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)。</span><span class="sxs-lookup"><span data-stu-id="6df6c-126">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

## <a name="client-credential-oauth-flow"></a><span data-ttu-id="6df6c-127">客户端凭据 OAuth 流</span><span class="sxs-lookup"><span data-stu-id="6df6c-127">Client credential OAuth flow</span></span>

<span data-ttu-id="6df6c-128">客户端凭据流使服务应用程序可以在没有用户交互的情况下运行。</span><span class="sxs-lookup"><span data-stu-id="6df6c-128">The client credential flow enables service applications to run without user interaction.</span></span> <span data-ttu-id="6df6c-129">访问基于应用程序的标识。</span><span class="sxs-lookup"><span data-stu-id="6df6c-129">Access is based on the identity of the application.</span></span> <span data-ttu-id="6df6c-130">有关详细信息, 请参阅[Microsoft identity platform 和 OAuth 2.0 客户端凭据流](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)。</span><span class="sxs-lookup"><span data-stu-id="6df6c-130">For more information, see [Microsoft identity platform and the OAuth 2.0 client credentials flow](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow).</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="6df6c-131">语言</span><span class="sxs-lookup"><span data-stu-id="6df6c-131">C#</span></span>](#tab/CS)

```csharp
IConfidentialClientApplication clientApplication = ClientCredentialProvider.CreateClientApplication(clientId, clientCredential);
ClientCredentialProvider authProvider = new ClientCredentialProvider(clientApplication);
```

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6df6c-132">Javascript</span><span class="sxs-lookup"><span data-stu-id="6df6c-132">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="6df6c-133">授权代码、客户端凭据和代表的 OAuth 流都要求您在此时实现自定义身份验证提供程序。</span><span class="sxs-lookup"><span data-stu-id="6df6c-133">Authorization code, client credential, and on-behalf-of OAuth flows require that you implement a custom authentication provider at this time.</span></span> <span data-ttu-id="6df6c-134">有关详细信息, 请参阅[使用自定义身份验证提供程序](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md)。</span><span class="sxs-lookup"><span data-stu-id="6df6c-134">For more information, see [Using a custom authentication provider](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md).</span></span>

# <a name="javatabjava"></a>[<span data-ttu-id="6df6c-135">Java</span><span class="sxs-lookup"><span data-stu-id="6df6c-135">Java</span></span>](#tab/Java)

```java
ClientCredentialProvider authProvider = new ClientCredentialProvider(
                                                    clientId,
                                                    scopes,
                                                    clientSecret,
                                                    tenant,
                                                    endpoint);
```

# <a name="androidtabandroid"></a>[<span data-ttu-id="6df6c-136">Android</span><span class="sxs-lookup"><span data-stu-id="6df6c-136">Android</span></span>](#tab/Android)

<span data-ttu-id="6df6c-137">不适用。</span><span class="sxs-lookup"><span data-stu-id="6df6c-137">Not applicable.</span></span>

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="6df6c-138">目标-C</span><span class="sxs-lookup"><span data-stu-id="6df6c-138">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="6df6c-139">不适用。</span><span class="sxs-lookup"><span data-stu-id="6df6c-139">Not applicable.</span></span>

# <a name="phptabphp"></a>[<span data-ttu-id="6df6c-140">PHP</span><span class="sxs-lookup"><span data-stu-id="6df6c-140">PHP</span></span>](#tab/PHP)

<span data-ttu-id="6df6c-141">尚不可用。</span><span class="sxs-lookup"><span data-stu-id="6df6c-141">Not available, yet.</span></span> <span data-ttu-id="6df6c-142">如果这对你非常重要, 请支持或打开[Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)。</span><span class="sxs-lookup"><span data-stu-id="6df6c-142">Please support or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="6df6c-143">Ruby</span><span class="sxs-lookup"><span data-stu-id="6df6c-143">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="6df6c-144">尚不可用。</span><span class="sxs-lookup"><span data-stu-id="6df6c-144">Not available, yet.</span></span> <span data-ttu-id="6df6c-145">如果这对你非常重要, 请支持或打开[Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)。</span><span class="sxs-lookup"><span data-stu-id="6df6c-145">Please support or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

## <a name="on-behalf-of-oauth-flow"></a><span data-ttu-id="6df6c-146">代表 OAuth 流</span><span class="sxs-lookup"><span data-stu-id="6df6c-146">On-behalf-of OAuth flow</span></span>

<span data-ttu-id="6df6c-147">当应用程序调用在其中打开 Microsoft Graph API 的服务/web API 时, 代表流是适用的。</span><span class="sxs-lookup"><span data-stu-id="6df6c-147">The on-behalf-of flow is applicable when your application calls a service/web API which in turns calls the Microsoft Graph API.</span></span> <span data-ttu-id="6df6c-148">若要了解详细信息, 请阅读[Microsoft identity platform 和 OAuth 2.0 代表流](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow)</span><span class="sxs-lookup"><span data-stu-id="6df6c-148">Learn more by reading [Microsoft identity platform and OAuth 2.0 On-Behalf-Of flow](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow)</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="6df6c-149">语言</span><span class="sxs-lookup"><span data-stu-id="6df6c-149">C#</span></span>](#tab/CS)

```csharp
IConfidentialClientApplication clientApplication = OnBehalfOfProvider.CreateClientApplication(clientId, redirectUri, clientCredential);
OnBehalfOfProvider authProvider = new OnBehalfOfProvider(clientApplication, scopes);
```

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6df6c-150">Javascript</span><span class="sxs-lookup"><span data-stu-id="6df6c-150">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="6df6c-151">授权代码、客户端凭据和代表的 OAuth 流都要求您在此时实现自定义身份验证提供程序。</span><span class="sxs-lookup"><span data-stu-id="6df6c-151">Authorization code, client credential, and on-behalf-of OAuth flows require that you implement a custom authentication provider at this time.</span></span> <span data-ttu-id="6df6c-152">有关详细信息, 请参阅[使用自定义身份验证提供程序](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md)。</span><span class="sxs-lookup"><span data-stu-id="6df6c-152">Read [Using Custom Authentication Provider](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md) for more information.</span></span>

# <a name="javatabjava"></a>[<span data-ttu-id="6df6c-153">Java</span><span class="sxs-lookup"><span data-stu-id="6df6c-153">Java</span></span>](#tab/Java)

<span data-ttu-id="6df6c-154">尚不可用。</span><span class="sxs-lookup"><span data-stu-id="6df6c-154">Not yet available.</span></span> <span data-ttu-id="6df6c-155">如果这对你非常重要, 请投票或打开[Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)。</span><span class="sxs-lookup"><span data-stu-id="6df6c-155">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="androidtabandroid"></a>[<span data-ttu-id="6df6c-156">Android</span><span class="sxs-lookup"><span data-stu-id="6df6c-156">Android</span></span>](#tab/Android)

<span data-ttu-id="6df6c-157">不适用。</span><span class="sxs-lookup"><span data-stu-id="6df6c-157">Not applicable.</span></span>

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="6df6c-158">目标-C</span><span class="sxs-lookup"><span data-stu-id="6df6c-158">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="6df6c-159">不适用。</span><span class="sxs-lookup"><span data-stu-id="6df6c-159">Not applicable.</span></span>

# <a name="phptabphp"></a>[<span data-ttu-id="6df6c-160">PHP</span><span class="sxs-lookup"><span data-stu-id="6df6c-160">PHP</span></span>](#tab/PHP)

<span data-ttu-id="6df6c-161">尚不可用。</span><span class="sxs-lookup"><span data-stu-id="6df6c-161">Not yet available.</span></span> <span data-ttu-id="6df6c-162">如果这对你非常重要, 请投票或打开[Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)。</span><span class="sxs-lookup"><span data-stu-id="6df6c-162">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="6df6c-163">Ruby</span><span class="sxs-lookup"><span data-stu-id="6df6c-163">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="6df6c-164">尚不可用。</span><span class="sxs-lookup"><span data-stu-id="6df6c-164">Not yet available.</span></span> <span data-ttu-id="6df6c-165">如果这对你非常重要, 请投票或打开[Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)。</span><span class="sxs-lookup"><span data-stu-id="6df6c-165">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

## <a name="implicit-grant-oauth-flow"></a><span data-ttu-id="6df6c-166">隐式授予 OAuth 流</span><span class="sxs-lookup"><span data-stu-id="6df6c-166">Implicit grant OAuth flow</span></span>

<span data-ttu-id="6df6c-167">隐式授予流在基于浏览器的应用程序中使用。</span><span class="sxs-lookup"><span data-stu-id="6df6c-167">The implicit grant flow is used in browser-based applications.</span></span> <span data-ttu-id="6df6c-168">有关详细信息, 请参阅[Microsoft identity platform 和隐式授予流](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-implicit-grant-flow)。</span><span class="sxs-lookup"><span data-stu-id="6df6c-168">For more information, see [Microsoft identity platform and Implicit grant flow](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-implicit-grant-flow).</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="6df6c-169">语言</span><span class="sxs-lookup"><span data-stu-id="6df6c-169">C#</span></span>](#tab/CS)

<span data-ttu-id="6df6c-170">不适用。</span><span class="sxs-lookup"><span data-stu-id="6df6c-170">Not applicable.</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6df6c-171">Javascript</span><span class="sxs-lookup"><span data-stu-id="6df6c-171">Javascript</span></span>](#tab/Javascript)

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

# <a name="javatabjava"></a>[<span data-ttu-id="6df6c-172">Java</span><span class="sxs-lookup"><span data-stu-id="6df6c-172">Java</span></span>](#tab/Java)

<span data-ttu-id="6df6c-173">不适用。</span><span class="sxs-lookup"><span data-stu-id="6df6c-173">Not applicable.</span></span>

# <a name="androidtabandroid"></a>[<span data-ttu-id="6df6c-174">Android</span><span class="sxs-lookup"><span data-stu-id="6df6c-174">Android</span></span>](#tab/Android)

<span data-ttu-id="6df6c-175">不适用。</span><span class="sxs-lookup"><span data-stu-id="6df6c-175">Not applicable.</span></span>

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="6df6c-176">目标-C</span><span class="sxs-lookup"><span data-stu-id="6df6c-176">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="6df6c-177">不适用。</span><span class="sxs-lookup"><span data-stu-id="6df6c-177">Not applicable.</span></span>

# <a name="phptabphp"></a>[<span data-ttu-id="6df6c-178">PHP</span><span class="sxs-lookup"><span data-stu-id="6df6c-178">PHP</span></span>](#tab/PHP)

<span data-ttu-id="6df6c-179">不适用。</span><span class="sxs-lookup"><span data-stu-id="6df6c-179">Not applicable.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="6df6c-180">Ruby</span><span class="sxs-lookup"><span data-stu-id="6df6c-180">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="6df6c-181">不适用。</span><span class="sxs-lookup"><span data-stu-id="6df6c-181">Not applicable.</span></span>

---

## <a name="device-code-oauth-flow"></a><span data-ttu-id="6df6c-182">设备代码 OAuth 流</span><span class="sxs-lookup"><span data-stu-id="6df6c-182">Device code OAuth flow</span></span>

<span data-ttu-id="6df6c-183">设备代码流允许通过其他设备登录设备。</span><span class="sxs-lookup"><span data-stu-id="6df6c-183">The device code flow enables sign in to devices by way of another device.</span></span> <span data-ttu-id="6df6c-184">有关详细信息, 请参阅[Microsoft identity platform 和 OAuth 2.0 设备代码流](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-device-code)。</span><span class="sxs-lookup"><span data-stu-id="6df6c-184">For details, see [Microsoft identity platform and the OAuth 2.0 device code flow](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-device-code).</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="6df6c-185">语言</span><span class="sxs-lookup"><span data-stu-id="6df6c-185">C#</span></span>](#tab/CS)

```csharp
IPublicClientApplication clientApplication = DeviceCodeProvider.CreateClientApplication(clientId);
DeviceCodeProvider authProvider = new DeviceCodeProvider(clientApplication, scopes);
```

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6df6c-186">Javascript</span><span class="sxs-lookup"><span data-stu-id="6df6c-186">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="6df6c-187">尚不可用。</span><span class="sxs-lookup"><span data-stu-id="6df6c-187">Not yet available.</span></span> <span data-ttu-id="6df6c-188">如果这对你非常重要, 请投票或打开[Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)。</span><span class="sxs-lookup"><span data-stu-id="6df6c-188">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="javatabjava"></a>[<span data-ttu-id="6df6c-189">Java</span><span class="sxs-lookup"><span data-stu-id="6df6c-189">Java</span></span>](#tab/Java)

<span data-ttu-id="6df6c-190">尚不可用。</span><span class="sxs-lookup"><span data-stu-id="6df6c-190">Not available, yet.</span></span> <span data-ttu-id="6df6c-191">如果这对你非常重要, 请支持或打开[Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)。</span><span class="sxs-lookup"><span data-stu-id="6df6c-191">Please support or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="androidtabandroid"></a>[<span data-ttu-id="6df6c-192">Android</span><span class="sxs-lookup"><span data-stu-id="6df6c-192">Android</span></span>](#tab/Android)

<span data-ttu-id="6df6c-193">不适用。</span><span class="sxs-lookup"><span data-stu-id="6df6c-193">Not applicable.</span></span>

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="6df6c-194">目标-C</span><span class="sxs-lookup"><span data-stu-id="6df6c-194">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="6df6c-195">不适用。</span><span class="sxs-lookup"><span data-stu-id="6df6c-195">Not applicable.</span></span>

# <a name="phptabphp"></a>[<span data-ttu-id="6df6c-196">PHP</span><span class="sxs-lookup"><span data-stu-id="6df6c-196">PHP</span></span>](#tab/PHP)

<span data-ttu-id="6df6c-197">尚不可用。</span><span class="sxs-lookup"><span data-stu-id="6df6c-197">Not yet available.</span></span> <span data-ttu-id="6df6c-198">如果这对你非常重要, 请投票或打开[Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)。</span><span class="sxs-lookup"><span data-stu-id="6df6c-198">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="6df6c-199">Ruby</span><span class="sxs-lookup"><span data-stu-id="6df6c-199">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="6df6c-200">尚不可用。</span><span class="sxs-lookup"><span data-stu-id="6df6c-200">Not yet available.</span></span> <span data-ttu-id="6df6c-201">如果这对你非常重要, 请投票或打开[Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)。</span><span class="sxs-lookup"><span data-stu-id="6df6c-201">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

## <a name="integrated-windows-flow"></a><span data-ttu-id="6df6c-202">集成的 Windows 流</span><span class="sxs-lookup"><span data-stu-id="6df6c-202">Integrated Windows flow</span></span>

<span data-ttu-id="6df6c-203">集成的 Windows 流为 Windows 计算机提供了一种在加入域时无提示地获取访问令牌的方法。</span><span class="sxs-lookup"><span data-stu-id="6df6c-203">The integrated Windows flow provides a way for Windows computers to silently acquire an access token when they are domain joined.</span></span> <span data-ttu-id="6df6c-204">有关详细信息, 请参阅[集成 Windows 身份验证](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Integrated-Windows-Authentication)。</span><span class="sxs-lookup"><span data-stu-id="6df6c-204">For details, see [Integrated Windows authentication](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Integrated-Windows-Authentication).</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="6df6c-205">语言</span><span class="sxs-lookup"><span data-stu-id="6df6c-205">C#</span></span>](#tab/CS)

```csharp
IPublicClientApplication clientApplication = IntegratedWindowsAuthenticationProvider.CreateClientApplication(clientId);
IntegratedWindowsAuthenticationProvider authProvider = new IntegratedWindowsAuthenticationProvider(clientApplication, scopes);
```

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6df6c-206">Javascript</span><span class="sxs-lookup"><span data-stu-id="6df6c-206">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="6df6c-207">不适用。</span><span class="sxs-lookup"><span data-stu-id="6df6c-207">Not applicable.</span></span>

# <a name="javatabjava"></a>[<span data-ttu-id="6df6c-208">Java</span><span class="sxs-lookup"><span data-stu-id="6df6c-208">Java</span></span>](#tab/Java)

<span data-ttu-id="6df6c-209">不适用。</span><span class="sxs-lookup"><span data-stu-id="6df6c-209">Not applicable.</span></span>

# <a name="androidtabandroid"></a>[<span data-ttu-id="6df6c-210">Android</span><span class="sxs-lookup"><span data-stu-id="6df6c-210">Android</span></span>](#tab/Android)

<span data-ttu-id="6df6c-211">不适用。</span><span class="sxs-lookup"><span data-stu-id="6df6c-211">Not applicable.</span></span>

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="6df6c-212">目标-C</span><span class="sxs-lookup"><span data-stu-id="6df6c-212">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="6df6c-213">不适用。</span><span class="sxs-lookup"><span data-stu-id="6df6c-213">Not applicable.</span></span>

# <a name="phptabphp"></a>[<span data-ttu-id="6df6c-214">PHP</span><span class="sxs-lookup"><span data-stu-id="6df6c-214">PHP</span></span>](#tab/PHP)

<span data-ttu-id="6df6c-215">不适用。</span><span class="sxs-lookup"><span data-stu-id="6df6c-215">Not applicable.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="6df6c-216">Ruby</span><span class="sxs-lookup"><span data-stu-id="6df6c-216">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="6df6c-217">不适用。</span><span class="sxs-lookup"><span data-stu-id="6df6c-217">Not applicable.</span></span>

---

## <a name="interactive-flow"></a><span data-ttu-id="6df6c-218">交互流</span><span class="sxs-lookup"><span data-stu-id="6df6c-218">Interactive flow</span></span>

<span data-ttu-id="6df6c-219">移动应用程序 (Xamarin 和 UWP) 和桌面应用程序使用交互流, 以在用户的名称中调用 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="6df6c-219">The interactive flow is used by mobile applications (Xamarin and UWP) and desktops applications to call Microsoft Graph in the name of a user.</span></span> <span data-ttu-id="6df6c-220">有关详细信息, 请参阅[以交互方式获取令牌](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Acquiring-tokens-interactively)。</span><span class="sxs-lookup"><span data-stu-id="6df6c-220">For details, see [Acquiring tokens interactively](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Acquiring-tokens-interactively).</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="6df6c-221">语言</span><span class="sxs-lookup"><span data-stu-id="6df6c-221">C#</span></span>](#tab/CS)

```csharp
IPublicClientApplication clientApplication = InteractiveAuthenticationProvider.CreateClientApplication(clientId);
InteractiveAuthenticationProvider authProvider = new InteractiveAuthenticationProvider(clientApplication, scopes);
```

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6df6c-222">Javascript</span><span class="sxs-lookup"><span data-stu-id="6df6c-222">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="6df6c-223">尚不可用。</span><span class="sxs-lookup"><span data-stu-id="6df6c-223">Not yet available.</span></span> <span data-ttu-id="6df6c-224">如果这对你非常重要, 请投票或打开[Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)。</span><span class="sxs-lookup"><span data-stu-id="6df6c-224">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="javatabjava"></a>[<span data-ttu-id="6df6c-225">Java</span><span class="sxs-lookup"><span data-stu-id="6df6c-225">Java</span></span>](#tab/Java)

<span data-ttu-id="6df6c-226">尚不可用。</span><span class="sxs-lookup"><span data-stu-id="6df6c-226">Not yet available.</span></span> <span data-ttu-id="6df6c-227">如果这对你非常重要, 请投票或打开[Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)。</span><span class="sxs-lookup"><span data-stu-id="6df6c-227">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="androidtabandroid"></a>[<span data-ttu-id="6df6c-228">Android</span><span class="sxs-lookup"><span data-stu-id="6df6c-228">Android</span></span>](#tab/Android)

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

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="6df6c-229">目标-C</span><span class="sxs-lookup"><span data-stu-id="6df6c-229">Objective-C</span></span>](#tab/Objective-C)

```objc
NSError *error = nil;
MSALPublicClientApplication *publicClientApplication = [[MSALPublicClientApplication alloc] initWithClientId:@"INSERT-CLIENT-APP-ID" 
error:&error];

MSALAuthenticationProviderOptions *authProviderOptions= [[MSALAuthenticationProviderOptions alloc] initWithScopes:<array-of-scopes-for-which-you-need-access-token>];

 MSALAuthenticationProvider *authenticationProvider = [[MSALAuthenticationProvider alloc] initWithPublicClientApplication:publicClientApplication 
 andOptions:authProviderOptions];
```

# <a name="phptabphp"></a>[<span data-ttu-id="6df6c-230">PHP</span><span class="sxs-lookup"><span data-stu-id="6df6c-230">PHP</span></span>](#tab/PHP)

<span data-ttu-id="6df6c-231">不适用。</span><span class="sxs-lookup"><span data-stu-id="6df6c-231">Not applicable.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="6df6c-232">Ruby</span><span class="sxs-lookup"><span data-stu-id="6df6c-232">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="6df6c-233">不适用。</span><span class="sxs-lookup"><span data-stu-id="6df6c-233">Not applicable.</span></span>

---

## <a name="resource-owner-password-credential-grant-oauth-flow"></a><span data-ttu-id="6df6c-234">资源所有者密码凭据授予 OAuth 流</span><span class="sxs-lookup"><span data-stu-id="6df6c-234">Resource owner password credential grant OAuth flow</span></span>

<span data-ttu-id="6df6c-235">资源所有者密码凭据流允许应用程序使用用户名和密码登录用户。</span><span class="sxs-lookup"><span data-stu-id="6df6c-235">The resource owner password credential flow allows an application to sign in a user by using their username and password.</span></span> <span data-ttu-id="6df6c-236">仅当您不能使用任何其他 OAuth 流时, 才使用此流。</span><span class="sxs-lookup"><span data-stu-id="6df6c-236">Use this flow only when you cannot use any of the other OAuth flows.</span></span> <span data-ttu-id="6df6c-237">有关详细信息, 请参阅[Microsoft identity platform 和 OAuth 2.0 资源所有者密码凭据](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth-ropc)</span><span class="sxs-lookup"><span data-stu-id="6df6c-237">For more information, see [Microsoft identity platform and the OAuth 2.0 resource owner password credential](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth-ropc)</span></span>



# <a name="ctabcs"></a>[<span data-ttu-id="6df6c-238">语言</span><span class="sxs-lookup"><span data-stu-id="6df6c-238">C#</span></span>](#tab/CS)

```csharp
IPublicClientApplication clientApplication = UsernamePasswordProvider.CreateClientApplication(clientId);
UsernamePasswordProvider authProvider = new UsernamePasswordProvider(clientApplication, scopes);
```

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6df6c-239">Javascript</span><span class="sxs-lookup"><span data-stu-id="6df6c-239">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="6df6c-240">尚不可用。</span><span class="sxs-lookup"><span data-stu-id="6df6c-240">Not yet available.</span></span> <span data-ttu-id="6df6c-241">如果这对你非常重要, 请投票或打开[Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)。</span><span class="sxs-lookup"><span data-stu-id="6df6c-241">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="javatabjava"></a>[<span data-ttu-id="6df6c-242">Java</span><span class="sxs-lookup"><span data-stu-id="6df6c-242">Java</span></span>](#tab/Java)

```java
UsernamePasswordProvider authProvider = new UsernamePasswordProvider(
                                                    clientId,
                                                    scopes,
                                                    username,
                                                    password);
```

# <a name="androidtabandroid"></a>[<span data-ttu-id="6df6c-243">Android</span><span class="sxs-lookup"><span data-stu-id="6df6c-243">Android</span></span>](#tab/Android)

<span data-ttu-id="6df6c-244">不适用。</span><span class="sxs-lookup"><span data-stu-id="6df6c-244">Not applicable.</span></span>

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="6df6c-245">目标-C</span><span class="sxs-lookup"><span data-stu-id="6df6c-245">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="6df6c-246">不适用。</span><span class="sxs-lookup"><span data-stu-id="6df6c-246">Not applicable.</span></span>

# <a name="phptabphp"></a>[<span data-ttu-id="6df6c-247">PHP</span><span class="sxs-lookup"><span data-stu-id="6df6c-247">PHP</span></span>](#tab/PHP)

<span data-ttu-id="6df6c-248">尚不可用。</span><span class="sxs-lookup"><span data-stu-id="6df6c-248">Not yet available.</span></span> <span data-ttu-id="6df6c-249">如果这对你非常重要, 请投票或打开[Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)。</span><span class="sxs-lookup"><span data-stu-id="6df6c-249">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="6df6c-250">Ruby</span><span class="sxs-lookup"><span data-stu-id="6df6c-250">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="6df6c-251">尚不可用。</span><span class="sxs-lookup"><span data-stu-id="6df6c-251">Not yet available.</span></span> <span data-ttu-id="6df6c-252">如果这对你非常重要, 请投票或打开[Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)。</span><span class="sxs-lookup"><span data-stu-id="6df6c-252">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

## <a name="next-steps"></a><span data-ttu-id="6df6c-253">后续步骤</span><span class="sxs-lookup"><span data-stu-id="6df6c-253">Next steps</span></span>

* <span data-ttu-id="6df6c-254">身份验证提供程序需要客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="6df6c-254">Authentication providers require an client ID.</span></span> <span data-ttu-id="6df6c-255">设置身份验证提供程序后, 需要[注册应用程序](https://portal.azure.com/)。</span><span class="sxs-lookup"><span data-stu-id="6df6c-255">You'll want to [register your application](https://portal.azure.com/) after you set up your authentication provider.</span></span>
* <span data-ttu-id="6df6c-256">如果[Microsoft Graph 功能请求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)目前不支持所需的 OAuth 流, 请告知我们。</span><span class="sxs-lookup"><span data-stu-id="6df6c-256">Let us know if a required OAuth flow isn't currently supported by voting for or opening a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests).</span></span>