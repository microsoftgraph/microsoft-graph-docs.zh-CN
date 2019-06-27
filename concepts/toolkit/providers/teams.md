---
title: Microsoft 团队提供商
description: 使用 Microsoft "团队" 选项卡中的团队提供程序来促进对所有组件的身份验证和 Microsoft Graph 访问。
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 348980225f04adfac4ded6f79a72654fbeec81e7
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2019
ms.locfileid: "35242961"
---
# <a name="microsoft-teams-provider"></a><span data-ttu-id="6ad3d-103">Microsoft 团队提供商</span><span class="sxs-lookup"><span data-stu-id="6ad3d-103">Microsoft Teams provider</span></span>

<span data-ttu-id="6ad3d-104">使用 Microsoft "团队" 选项卡中的团队提供程序来促进对所有组件的身份验证和 Microsoft Graph 访问。</span><span class="sxs-lookup"><span data-stu-id="6ad3d-104">Use the Teams provider inside your Microsoft Teams tab to facilitate authentication and Microsoft Graph access to all components.</span></span>

<span data-ttu-id="6ad3d-105">若要了解详细信息, 请参阅[提供程序](../providers.md)。</span><span class="sxs-lookup"><span data-stu-id="6ad3d-105">To learn more, see [providers](../providers.md).</span></span>

## <a name="get-started"></a><span data-ttu-id="6ad3d-106">入门</span><span class="sxs-lookup"><span data-stu-id="6ad3d-106">Get started</span></span>

<span data-ttu-id="6ad3d-107">在使用团队提供程序之前, 您需要确保您已在页面中引用[Microsoft 团队 SDK](https://docs.microsoft.com/en-us/javascript/api/overview/msteams-client?view=msteams-client-js-latest#using-the-sdk) 。</span><span class="sxs-lookup"><span data-stu-id="6ad3d-107">Before using the Teams provider, you will need to make sure you have referenced the [Microsoft Teams SDK](https://docs.microsoft.com/en-us/javascript/api/overview/msteams-client?view=msteams-client-js-latest#using-the-sdk) in your page.</span></span>

<span data-ttu-id="6ad3d-108">下面的示例使用 HTML (通过 CDN) 中的提供程序。</span><span class="sxs-lookup"><span data-stu-id="6ad3d-108">The following example uses the provider in HTML (via CDN).</span></span>

```html
<!-- Microsoft Teams sdk must be referenced before the toolkit -->
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>

<mgt-teams-provider
  client-id="<YOUR_CLIENT_ID>"
  auth-popup-url="https://<YOUR-DOMAIN>.com/AUTH-PATH"
></mgt-teams-provider>
```

<span data-ttu-id="6ad3d-109">下面的示例使用 JS 模块 (通过 NPM) 中的提供程序。</span><span class="sxs-lookup"><span data-stu-id="6ad3d-109">The following example uses the provider in JS modules (via NPM).</span></span>

<span data-ttu-id="6ad3d-110">请务必同时安装工具包和 Microsoft 团队 SDK。</span><span class="sxs-lookup"><span data-stu-id="6ad3d-110">Make sure to install both the toolkit and the Microsoft Teams SDK.</span></span>

```bash
npm install @microsoft/mgt @microsoft/teams-js
```

<span data-ttu-id="6ad3d-111">接下来, 导入并使用提供程序。</span><span class="sxs-lookup"><span data-stu-id="6ad3d-111">Next, import and use the provider.</span></span>

```ts
import '@microsoft/teams-js';
import {Providers, TeamsProvider} from '@microsoft/mgt'; 
Providers.globalProvider = new TeamsProvider(config);
```

<span data-ttu-id="6ad3d-112">其中`config`是</span><span class="sxs-lookup"><span data-stu-id="6ad3d-112">where `config` is</span></span>

```ts
export interface TeamsConfig {
  clientId: string;
  authPopupUrl: string;
  scopes?: string[];
  msalOptions?: Configuration;
}
```

<span data-ttu-id="6ad3d-113">有关完整示例, 请参阅[Microsoft 团队选项卡示例](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/teams-tab)。</span><span class="sxs-lookup"><span data-stu-id="6ad3d-113">For a complete example, see [Microsoft Teams tab sample](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/teams-tab).</span></span>

## <a name="configure-your-teams-app"></a><span data-ttu-id="6ad3d-114">配置团队应用程序</span><span class="sxs-lookup"><span data-stu-id="6ad3d-114">Configure your Teams app</span></span>

<span data-ttu-id="6ad3d-115">如果只是开始使用团队应用程序, 请参阅[将选项卡添加到 Microsoft 团队应用](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/tabs/tabs-overview)。</span><span class="sxs-lookup"><span data-stu-id="6ad3d-115">If you're just getting started with Teams apps, see [Add tabs to Microsoft Teams apps](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/tabs/tabs-overview).</span></span> <span data-ttu-id="6ad3d-116">您还可以使用[应用程序 Studio](https://docs.microsoft.com/en-us/microsoftteams/platform/get-started/get-started-app-studio)快速开发您的应用程序清单。</span><span class="sxs-lookup"><span data-stu-id="6ad3d-116">You can also use [App Studio](https://docs.microsoft.com/en-us/microsoftteams/platform/get-started/get-started-app-studio) to quickly develop your app manifest.</span></span>

<span data-ttu-id="6ad3d-117">使用选项卡安装您的应用程序并准备好使用组件时, 需要确保您的应用程序具有访问 Microsoft Graph 的适当权限。</span><span class="sxs-lookup"><span data-stu-id="6ad3d-117">After you install your app with a tab, and you're ready to use the components, you need to make sure that your app has the right permissions to access Microsoft Graph.</span></span> <span data-ttu-id="6ad3d-118">若要使用所需的权限配置应用程序, 请执行以下操作:</span><span class="sxs-lookup"><span data-stu-id="6ad3d-118">To configure your app with the necessary permissions:</span></span>

1. [<span data-ttu-id="6ad3d-119">检索你的域名</span><span class="sxs-lookup"><span data-stu-id="6ad3d-119">Retrieve your domain name</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/identity-protection/graph-get-started#retrieve-your-domain-name)
2. [<span data-ttu-id="6ad3d-120">创建新的应用注册</span><span class="sxs-lookup"><span data-stu-id="6ad3d-120">Create a new app registration</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/identity-protection/graph-get-started#create-a-new-app-registration)
3. [<span data-ttu-id="6ad3d-121">授予应用程序权限</span><span class="sxs-lookup"><span data-stu-id="6ad3d-121">Grant your application permission</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/identity-protection/graph-get-started#grant-your-application-permission-to-use-the-api)

<span data-ttu-id="6ad3d-122">在 "**添加 API 访问" 页**上添加正确的权限非常重要。</span><span class="sxs-lookup"><span data-stu-id="6ad3d-122">It's important to add the right permission on the **Add API access page**.</span></span> <span data-ttu-id="6ad3d-123">你将需要管理员添加和批准权限, 具体取决于所需的组件。</span><span class="sxs-lookup"><span data-stu-id="6ad3d-123">You will need an administrator to add and approve the permissions, depending on which component you need.</span></span>

><span data-ttu-id="6ad3d-124">**提示:** 如果你不确定要添加哪些权限, 请参阅每个组件的文档。</span><span class="sxs-lookup"><span data-stu-id="6ad3d-124">**Tip:** If you're not sure what permissions to add, see the documentation for each component.</span></span>

### <a name="enable-implicit-grant-flow"></a><span data-ttu-id="6ad3d-125">启用隐式授予流</span><span class="sxs-lookup"><span data-stu-id="6ad3d-125">Enable implicit grant Flow</span></span>

<span data-ttu-id="6ad3d-126">请确保启用隐式授予流;这对于从客户端请求令牌的 web 应用程序是必需的。</span><span class="sxs-lookup"><span data-stu-id="6ad3d-126">Make sure to enable implicit grant flow; this is a requirement for web apps that request tokens from the client side.</span></span> <span data-ttu-id="6ad3d-127">在 Azure 门户中, 在管理应用注册时, 请编辑清单并更改`oauth2AllowImplicitFlow`为`true`。</span><span class="sxs-lookup"><span data-stu-id="6ad3d-127">In the Azure Portal, when managing your app registration, edit the manifest and change `oauth2AllowImplicitFlow` to `true`.</span></span>

### <a name="create-the-popup-page"></a><span data-ttu-id="6ad3d-128">创建弹出页</span><span class="sxs-lookup"><span data-stu-id="6ad3d-128">Create the popup page</span></span>

<span data-ttu-id="6ad3d-129">若要使用你的团队凭据登录, 你需要提供团队应用将在弹出项中打开的 URL, 这将遵循身份验证流。</span><span class="sxs-lookup"><span data-stu-id="6ad3d-129">In order to sign in with your Teams credentials, you need to provide a URL that the Teams app will open in a popup, which will follow the authentication flow.</span></span> <span data-ttu-id="6ad3d-130">此 URL 必须在您的域中, 并且需要调用该`TeamsProvider.handleAuth();`方法。</span><span class="sxs-lookup"><span data-stu-id="6ad3d-130">This URL needs to be in your domain, and it needs to call the `TeamsProvider.handleAuth();` method.</span></span> <span data-ttu-id="6ad3d-131">这是此页面唯一需要执行的操作。</span><span class="sxs-lookup"><span data-stu-id="6ad3d-131">That's the only thing that this page needs to do.</span></span> <span data-ttu-id="6ad3d-132">例如：</span><span class="sxs-lookup"><span data-stu-id="6ad3d-132">For example:</span></span>

```html
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js">

<script>        
  mgt.TeamsProvider.handleAuth();
</script>
```

### <a name="configure-redirect-uris"></a><span data-ttu-id="6ad3d-133">配置重定向 Uri</span><span class="sxs-lookup"><span data-stu-id="6ad3d-133">Configure redirect URIs</span></span>

<span data-ttu-id="6ad3d-134">在您的网站上发布此页面后, 您需要使用`auth-popup-url/authPopupUrl`属性中的 URL。</span><span class="sxs-lookup"><span data-stu-id="6ad3d-134">After you publish this page on your website, you need to use the URL in the `auth-popup-url/authPopupUrl` property.</span></span> <span data-ttu-id="6ad3d-135">此外, 还需要在 Azure AD 门户的应用配置中将此 URL 配置为有效的重定向 URI。</span><span class="sxs-lookup"><span data-stu-id="6ad3d-135">This URL also needs to be configured as a valid redirect URI in your app configuration in the Azure AD portal.</span></span>
