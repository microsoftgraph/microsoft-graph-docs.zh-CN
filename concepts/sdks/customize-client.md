---
title: 自定义 Microsoft Graph SDK 服务客户端
description: 提供有关如何更改 Microsoft Graph SDK 服务客户端的默认行为的说明。
localization_priority: Normal
author: DarrelMiller
ms.openlocfilehash: a2750babd35f1e3fd5f361ae43009eaa25eefe87
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/12/2021
ms.locfileid: "52911653"
---
# <a name="customize-the-microsoft-graph-sdk-service-client"></a><span data-ttu-id="4d05b-103">自定义 Microsoft Graph SDK 服务客户端</span><span class="sxs-lookup"><span data-stu-id="4d05b-103">Customize the Microsoft Graph SDK service client</span></span>

<span data-ttu-id="4d05b-104">Microsoft Graph SDK 客户端配置了一组默认的中间件，允许 SDK 与 Microsoft Graph终结点通信。</span><span class="sxs-lookup"><span data-stu-id="4d05b-104">The Microsoft Graph SDK client configures a default set of middleware that allows the SDK to communicate with the Microsoft Graph endpoints.</span></span> <span data-ttu-id="4d05b-105">此默认集是可自定义的，允许您更改客户端的行为。</span><span class="sxs-lookup"><span data-stu-id="4d05b-105">This default set is customizable, allowing you to change the behavior of the client.</span></span> <span data-ttu-id="4d05b-106">例如，可以插入自定义日志记录，或添加测试处理程序以模拟特定方案。</span><span class="sxs-lookup"><span data-stu-id="4d05b-106">For example, you can insert customized logging, or add a test handler to simulate specific scenarios.</span></span> <span data-ttu-id="4d05b-107">可以添加和删除中间件组件。</span><span class="sxs-lookup"><span data-stu-id="4d05b-107">You can add and remove middleware components.</span></span> <span data-ttu-id="4d05b-108">需要注意的是，中间件组件的运行顺序非常重要。</span><span class="sxs-lookup"><span data-stu-id="4d05b-108">It is important to note that the order in which middleware components run is significant.</span></span>

## <a name="c"></a>[<span data-ttu-id="4d05b-109">C#</span><span class="sxs-lookup"><span data-stu-id="4d05b-109">C#</span></span>](#tab/csharp)

```csharp
var handlers = GraphClientFactory.CreateDefaultHandlers(authProvider);

// Remove a default handler
var compressionHandler =
    handlers.Where(h => h is CompressionHandler).FirstOrDefault();
handlers.Remove(compressionHandler);

// Add a new one
// ChaosHandler simulates random server failures
handlers.Add(new ChaosHandler());

var httpClient = GraphClientFactory.Create(handlers);

var customGraphClient = new GraphServiceClient(httpClient);

var messages = await customGraphClient.Me.Messages.Request()
    .Top(100)
    .Select(m => m.Subject)
    .GetAsync();
```

## <a name="typescript"></a>[<span data-ttu-id="4d05b-110">TypeScript</span><span class="sxs-lookup"><span data-stu-id="4d05b-110">TypeScript</span></span>](#tab/typeScript)

```typescript
// Create a custom auth provider
let authProvider = new SimpleAuthProvider(accessToken);
// Create an authentication handler that uses custom auth provider
let authHandler = new MicrosoftGraph.AuthenticationHandler(authProvider);

// Create a custom logging handler
let loggingHandler = new CustomLoggingHandler();

// Create a standard HTTP message handler
let httpHandler = new MicrosoftGraph.HTTPMessageHandler();

// Use setNext to chain handlers together
// auth -> logging -> http
authHandler.setNext(loggingHandler);
loggingHandler.setNext(httpHandler);

// Pass the first middleware in the chain in the middleWare property
const client = MicrosoftGraph.Client.initWithMiddleware({
  defaultVersion: 'v1.0',
  debugLogging: true,
  middleware: authHandler,
});

let response: PageCollection = await client
  .api('/me/messages?$top=10&$select=sender,subject')
  .get();
```

### <a name="simpleauthproviderts"></a><span data-ttu-id="4d05b-111">SimpleAuthProvider.ts</span><span class="sxs-lookup"><span data-stu-id="4d05b-111">SimpleAuthProvider.ts</span></span>

```typescript
import { AuthenticationProvider } from "@microsoft/microsoft-graph-client";

export default class SimpleAuthProvider implements AuthenticationProvider {
  private accessToken: string;

  constructor(accessToken: string) {
    this.accessToken = accessToken;
  }

  getAccessToken = async (): Promise<string> => {
    return this.accessToken;
  }
}
```

### <a name="customlogginghandlerts"></a><span data-ttu-id="4d05b-112">CustomLoggingHandler.ts</span><span class="sxs-lookup"><span data-stu-id="4d05b-112">CustomLoggingHandler.ts</span></span>

```typescript
import { Context, Middleware } from "@microsoft/microsoft-graph-client";

export default class CustomLoggingHandler implements Middleware {
  private nextMiddleware: any = null;

  execute = async (context: Context): Promise<void> => {
    console.log(`Logging request: ${context.request.toString()}`);
    return await this.nextMiddleware.execute(context);
  }
  setNext = (middleware: Middleware): void => {
    this.nextMiddleware = middleware;
  }
}
```

## <a name="java"></a>[<span data-ttu-id="4d05b-113">Java</span><span class="sxs-lookup"><span data-stu-id="4d05b-113">Java</span></span>](#tab/java)

```java
// you can configure any OkHttpClient option and add interceptors
// Note: com.microsoft.graph:microsoft-graph:3.0 or above is required
// for a complete description of available configuration options https://square.github.io/okhttp/4.x/okhttp/okhttp3/-ok-http-client/-builder/
final OkHttpClient httpClient = HttpClients.createDefault(authenticationProvider)
                                .newBuilder()
                                .followSslRedirects(false) // sample configuration to apply to client
                                .build();

final GraphServiceClient graphServiceClient = GraphServiceClient
                .builder()
                .httpClient(httpClient)
                .buildClient();
```

---

## <a name="configuring-the-http-proxy-for-the-client"></a><span data-ttu-id="4d05b-114">为客户端配置 HTTP 代理</span><span class="sxs-lookup"><span data-stu-id="4d05b-114">Configuring the HTTP proxy for the client</span></span>

<span data-ttu-id="4d05b-115">某些环境要求客户端应用程序在可以访问公共 Internet 之前使用 HTTP 代理。</span><span class="sxs-lookup"><span data-stu-id="4d05b-115">Some environments require client applications to use a HTTP proxy before they can access the public internet.</span></span> <span data-ttu-id="4d05b-116">本部分演示如何为 Microsoft SDK 配置Graph代理。</span><span class="sxs-lookup"><span data-stu-id="4d05b-116">This section shows how to configure the proxy for the Microsoft Graph SDKs.</span></span>

<!-- markdownlint-disable MD024 -->
## <a name="c"></a>[<span data-ttu-id="4d05b-117">C#</span><span class="sxs-lookup"><span data-stu-id="4d05b-117">C#</span></span>](#tab/csharp)

```csharp
// URI to proxy
var proxyAddress = "http://localhost:8888";

// Create a new System.Net.Http.HttpClientHandler with the proxy
var handler = new HttpClientHandler
{
    // Create a new System.Net.WebProxy
    // See WebProxy documentation for scenarios requiring
    // authentication to the proxy
    Proxy = new WebProxy(new Uri(proxyAddress))
};

// Create an options object for the credential being used
// For example, here we're using a ClientSecretCredential so
// we create a ClientSecretCredentialOptions object
var options = new ClientSecretCredentialOptions
{
    // Create a new Azure.Core.HttpClientTransport
    Transport = new HttpClientTransport(handler)
};

var credential = new ClientSecretCredential(
    "YOUR_TENANT_ID",
    "YOUR_CLIENT_ID",
    "YOUR_CLIENT_SECRET",
    options
);

// Create a new Microsoft.Graph.HttpProvider using the
// proxied HttpClientHandler
var httpProvider = new HttpProvider(handler, true);

var scopes = new[] { "https://graph.microsoft.com/.default" };
var graphClient = new GraphServiceClient(credential, scopes, httpProvider);
```

## <a name="typescript"></a>[<span data-ttu-id="4d05b-118">TypeScript</span><span class="sxs-lookup"><span data-stu-id="4d05b-118">TypeScript</span></span>](#tab/typeScript)

```typescript
// Create a credential from @azure/identity package
const credential = new ClientSecretCredential(
  'YOUR_TENANT_ID',
  'YOUR_CLIENT_ID',
  'YOUR_CLIENT_SECRET',
  {
    proxyOptions: {
      host: 'localhost',
      port: 8888,
      // If proxy requires authentication
      //username: '',
      //password: ''
    },
  }
);

// Create a Graph token credential provider
const tokenAuthProvider = new TokenCredentialAuthenticationProvider(
  credential,
  {
    scopes: [ 'https://graph.microsoft.com/.default' ]
  });

const client = MicrosoftGraph.Client.initWithMiddleware({
  authProvider: tokenAuthProvider,
  // Configure proxy in fetchOptions
  fetchOptions: {
    agent: new HttpsProxyAgent('http://localhost:8888')
  }
});
```

## <a name="java"></a>[<span data-ttu-id="4d05b-119">Java</span><span class="sxs-lookup"><span data-stu-id="4d05b-119">Java</span></span>](#tab/java)

```Java
final int proxyPort = 8080;
final InetSocketAddress proxyInetAddress = new InetSocketAddress("proxy.ip.or.hostname", proxyPort);

// The section below configures the proxy for the Azure Identity client
// and is only needed if you rely on Azure Identity for authentication
final ProxyOptions pOptions = new ProxyOptions(ProxyOptions.Type.HTTP, proxyInetAddress);
final HttpClientOptions clientOptions = new HttpClientOptions();
clientOptions.setProxyOptions(pOptions);
final HttpClient azHttpClient = HttpClient.createDefault(clientOptions);

// Or any other credential the application is using
final ClientSecretCredential clientSecretCredential =
    new ClientSecretCredentialBuilder()
        .clientId(CLIENT_ID)
        .clientSecret(CLIENT_SECRET)
        .tenantId(TENANT_GUID)
        // don't forget that addition to use the configured client
        .httpClient(azHttpClient)
        .build();
final TokenCredentialAuthProvider authenticationProvider =
    new TokenCredentialAuthProvider(Arrays.asList(SCOPES), clientSecretCredential);

// The section below configures the proxy for the Microsoft Graph SDK client
final Proxy proxy = new Proxy(Proxy.Type.HTTP, proxyInetAddress);

// This block is only needed if the proxy requires authentication
final Authenticator proxyAuthenticator = new Authenticator() {
  @Override
  public Request authenticate(Route route, Response response) throws IOException {
    String credential = Credentials.basic("username", "password");
    return response.request().newBuilder()
        .header("Proxy-Authorization", credential)
        .build();
  }
};

final OkHttpClient graphHttpClient =
    HttpClients.createDefault(authenticationProvider)
        .newBuilder()
        .proxy(proxy)
        .proxyAuthenticator(proxyAuthenticator)
        .build();

final GraphServiceClient graphServiceClient =
    GraphServiceClient
        .builder()
        .httpClient(graphHttpClient)
        .buildClient();

```

> [!NOTE]
> <span data-ttu-id="4d05b-120">有关 Azure Identity 代理配置详细信息，请参阅 [ProxyOptions](/java/api/com.azure.core.http.proxyoptions.proxyoptions)。</span><span class="sxs-lookup"><span data-stu-id="4d05b-120">For more information about Azure Identity proxy configuration, see [ProxyOptions](/java/api/com.azure.core.http.proxyoptions.proxyoptions).</span></span>

---
