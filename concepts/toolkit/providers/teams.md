---
title: Microsoft Teams 提供程序
description: 使用 Microsoft "团队" 选项卡中的团队提供程序来促进对所有组件的身份验证和 Microsoft Graph 访问。
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 62dba210d4fbf7d3540df7fd58d33e275f0065c3
ms.sourcegitcommit: 05645bc582d14781a9ca6b78ed598a4e7dc26869
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/01/2020
ms.locfileid: "44990253"
---
# <a name="microsoft-teams-provider"></a><span data-ttu-id="feba5-103">Microsoft Teams 提供程序</span><span class="sxs-lookup"><span data-stu-id="feba5-103">Microsoft Teams provider</span></span>

<span data-ttu-id="feba5-104">使用 Microsoft "团队" 选项卡中的团队提供程序来促进对所有组件的身份验证和 Microsoft Graph 访问。</span><span class="sxs-lookup"><span data-stu-id="feba5-104">Use the Teams provider inside your Microsoft Teams tab to facilitate authentication and Microsoft Graph access to all components.</span></span>

<span data-ttu-id="feba5-105">若要了解详细信息，请参阅[提供程序](../providers.md)。</span><span class="sxs-lookup"><span data-stu-id="feba5-105">To learn more, see [providers](../providers.md).</span></span>

## <a name="get-started"></a><span data-ttu-id="feba5-106">入门</span><span class="sxs-lookup"><span data-stu-id="feba5-106">Get started</span></span>

<span data-ttu-id="feba5-107">在使用团队提供程序之前，您需要确保您已在页面中引用[Microsoft 团队 SDK](/javascript/api/overview/msteams-client?view=msteams-client-js-latest#using-the-sdk) 。</span><span class="sxs-lookup"><span data-stu-id="feba5-107">Before using the Teams provider, you will need to make sure you have referenced the [Microsoft Teams SDK](/javascript/api/overview/msteams-client?view=msteams-client-js-latest#using-the-sdk) in your page.</span></span>

### <a name="via-script-tag"></a><span data-ttu-id="feba5-108">via script 标记</span><span class="sxs-lookup"><span data-stu-id="feba5-108">via script tag</span></span>
<span data-ttu-id="feba5-109">下面的示例使用 HTML （通过 CDN）中的提供程序。</span><span class="sxs-lookup"><span data-stu-id="feba5-109">The following example uses the provider in HTML (via CDN).</span></span>

```html
<!-- Microsoft Teams sdk must be referenced before the toolkit -->
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>

<mgt-teams-provider
  client-id="<YOUR_CLIENT_ID>"
  auth-popup-url="https://<YOUR-DOMAIN>.com/AUTH-PATH"
  authority=""
></mgt-teams-provider>
```

| <span data-ttu-id="feba5-110">属性</span><span class="sxs-lookup"><span data-stu-id="feba5-110">Attribute</span></span> | <span data-ttu-id="feba5-111">说明</span><span class="sxs-lookup"><span data-stu-id="feba5-111">Description</span></span> |
| --- | --- |
| <span data-ttu-id="feba5-112">客户端 id</span><span class="sxs-lookup"><span data-stu-id="feba5-112">client-id</span></span>   | <span data-ttu-id="feba5-113">字符串客户端 ID （请参阅[配置团队应用](#configure-your-teams-app)。</span><span class="sxs-lookup"><span data-stu-id="feba5-113">String client ID (see [Configure your Teams app](#configure-your-teams-app).</span></span> <span data-ttu-id="feba5-114">必需。</span><span class="sxs-lookup"><span data-stu-id="feba5-114">Required.</span></span> |
| <span data-ttu-id="feba5-115">auth-popup-url</span><span class="sxs-lookup"><span data-stu-id="feba5-115">auth-popup-url</span></span>  | <span data-ttu-id="feba5-116">将在弹出窗口中处理 auth 的页面的绝对或相对路径（请参阅[Create the popup page](#create-the-popup-page)）。</span><span class="sxs-lookup"><span data-stu-id="feba5-116">Absolute or relative path to the page that will handle auth in the popup (see [Create the popup page](#create-the-popup-page)).</span></span> <span data-ttu-id="feba5-117">必需。</span><span class="sxs-lookup"><span data-stu-id="feba5-117">Required.</span></span> |
| <span data-ttu-id="feba5-118">scopes</span><span class="sxs-lookup"><span data-stu-id="feba5-118">scopes</span></span>  | <span data-ttu-id="feba5-119">用户必须同意登录时的作用域的逗号分隔字符串。</span><span class="sxs-lookup"><span data-stu-id="feba5-119">Comma separated strings for scopes the user must consent to on sign in.</span></span> <span data-ttu-id="feba5-120">可选。</span><span class="sxs-lookup"><span data-stu-id="feba5-120">Optional.</span></span> |
| <span data-ttu-id="feba5-121">取决于</span><span class="sxs-lookup"><span data-stu-id="feba5-121">depends-on</span></span> | <span data-ttu-id="feba5-122">另一个较高优先级提供程序组件的元素选择器字符串。</span><span class="sxs-lookup"><span data-stu-id="feba5-122">Element selector string of another higher-priority provider component.</span></span> <span data-ttu-id="feba5-123">可选。</span><span class="sxs-lookup"><span data-stu-id="feba5-123">Optional.</span></span> |
| <span data-ttu-id="feba5-124">监管</span><span class="sxs-lookup"><span data-stu-id="feba5-124">authority</span></span>    | <span data-ttu-id="feba5-125">颁发机构字符串。</span><span class="sxs-lookup"><span data-stu-id="feba5-125">Authority string.</span></span> <span data-ttu-id="feba5-126">默认值是公共颁发机构。</span><span class="sxs-lookup"><span data-stu-id="feba5-126">The default is the common authority.</span></span> <span data-ttu-id="feba5-127">对于单租户应用，请使用租户 ID 或租户名称。</span><span class="sxs-lookup"><span data-stu-id="feba5-127">For single-tenant apps, use your tenant ID or tenant name.</span></span> <span data-ttu-id="feba5-128">例如， `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` 或 `https://login.microsoftonline.com/[your-tenant-id]` 。</span><span class="sxs-lookup"><span data-stu-id="feba5-128">For example, `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` or `https://login.microsoftonline.com/[your-tenant-id]`.</span></span> <span data-ttu-id="feba5-129">可选。</span><span class="sxs-lookup"><span data-stu-id="feba5-129">Optional.</span></span> |


### <a name="via-npm"></a><span data-ttu-id="feba5-130">via NPM</span><span class="sxs-lookup"><span data-stu-id="feba5-130">via NPM</span></span>
<span data-ttu-id="feba5-131">下面的示例使用 JS 模块（通过 NPM）中的提供程序。</span><span class="sxs-lookup"><span data-stu-id="feba5-131">The following example uses the provider in JS modules (via NPM).</span></span>

<span data-ttu-id="feba5-132">请务必同时安装工具包和 Microsoft 团队 SDK。</span><span class="sxs-lookup"><span data-stu-id="feba5-132">Make sure to install both the toolkit and the Microsoft Teams SDK.</span></span>

```bash
npm install @microsoft/mgt @microsoft/teams-js
```

<span data-ttu-id="feba5-133">接下来，导入并使用提供程序。</span><span class="sxs-lookup"><span data-stu-id="feba5-133">Next, import and use the provider.</span></span>

```ts
import '@microsoft/teams-js';
import {Providers, TeamsProvider} from '@microsoft/mgt';
Providers.globalProvider = new TeamsProvider(config);
```

<span data-ttu-id="feba5-134">其中 `config` 是</span><span class="sxs-lookup"><span data-stu-id="feba5-134">where `config` is</span></span>

```ts
export interface TeamsConfig {
  clientId: string;
  authPopupUrl: string;
  scopes?: string[];
  msalOptions?: Configuration;
}
```

<span data-ttu-id="feba5-135">或者，您可能需要设置对 Microsoft 团队库的引用。</span><span class="sxs-lookup"><span data-stu-id="feba5-135">Alternatively, you might need to set the reference to the Microsoft Teams Library.</span></span> <span data-ttu-id="feba5-136">如以下示例所示：</span><span class="sxs-lookup"><span data-stu-id="feba5-136">Here is an example:</span></span>

```ts
import * as MicrosoftTeams from "@microsoft/teams-js/dist/MicrosoftTeams";
import {Providers, TeamsProvider} from '@microsoft/mgt';

TeamsProvider.microsoftTeamsLib = MicrosoftTeams;
Providers.globalProvider = new TeamsProvider(config);
```

<span data-ttu-id="feba5-137">有关完整示例，请参阅[Microsoft 团队选项卡示例](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/teams-tab)。</span><span class="sxs-lookup"><span data-stu-id="feba5-137">For a complete example, see [Microsoft Teams tab sample](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/teams-tab).</span></span>

## <a name="configure-your-teams-app"></a><span data-ttu-id="feba5-138">配置团队应用程序</span><span class="sxs-lookup"><span data-stu-id="feba5-138">Configure your Teams app</span></span>

<span data-ttu-id="feba5-139">如果只是开始使用团队应用程序，请参阅[将选项卡添加到 Microsoft 团队应用](/microsoftteams/platform/concepts/tabs/tabs-overview)。</span><span class="sxs-lookup"><span data-stu-id="feba5-139">If you're just getting started with Teams apps, see [Add tabs to Microsoft Teams apps](/microsoftteams/platform/concepts/tabs/tabs-overview).</span></span> <span data-ttu-id="feba5-140">您还可以使用[应用程序 Studio](/microsoftteams/platform/get-started/get-started-app-studio)快速开发您的应用程序清单。</span><span class="sxs-lookup"><span data-stu-id="feba5-140">You can also use [App Studio](/microsoftteams/platform/get-started/get-started-app-studio) to quickly develop your app manifest.</span></span>

<span data-ttu-id="feba5-141">使用选项卡安装您的应用程序并准备好使用组件时，需要确保您的应用程序具有访问 Microsoft Graph 的适当权限。</span><span class="sxs-lookup"><span data-stu-id="feba5-141">After you install your app with a tab, and you're ready to use the components, you need to make sure that your app has the right permissions to access Microsoft Graph.</span></span> <span data-ttu-id="feba5-142">若要使用所需的权限配置应用程序，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="feba5-142">To configure your app with the necessary permissions:</span></span>

1. [<span data-ttu-id="feba5-143">检索你的域名</span><span class="sxs-lookup"><span data-stu-id="feba5-143">Retrieve your domain name</span></span>](/azure/active-directory/identity-protection/graph-get-started#retrieve-your-domain-name)
2. [<span data-ttu-id="feba5-144">创建新的应用注册</span><span class="sxs-lookup"><span data-stu-id="feba5-144">Create a new app registration</span></span>](/azure/active-directory/identity-protection/graph-get-started#create-a-new-app-registration)
3. [<span data-ttu-id="feba5-145">授予应用程序权限</span><span class="sxs-lookup"><span data-stu-id="feba5-145">Grant your application permission</span></span>](/azure/active-directory/identity-protection/graph-get-started#grant-your-application-permission-to-use-the-api)

<span data-ttu-id="feba5-146">在 "**添加 API 访问" 页**上添加正确的权限非常重要。</span><span class="sxs-lookup"><span data-stu-id="feba5-146">It's important to add the right permission on the **Add API access page**.</span></span> <span data-ttu-id="feba5-147">你将需要管理员添加和批准权限，具体取决于所需的组件。</span><span class="sxs-lookup"><span data-stu-id="feba5-147">You will need an administrator to add and approve the permissions, depending on which component you need.</span></span>

><span data-ttu-id="feba5-148">**提示：** 如果你不确定要添加哪些权限，请参阅每个组件的文档。</span><span class="sxs-lookup"><span data-stu-id="feba5-148">**Tip:** If you're not sure what permissions to add, see the documentation for each component.</span></span>

### <a name="enable-implicit-grant-flow"></a><span data-ttu-id="feba5-149">启用隐式授予流</span><span class="sxs-lookup"><span data-stu-id="feba5-149">Enable implicit grant Flow</span></span>

<span data-ttu-id="feba5-150">请确保启用隐式授予流;这对于从客户端请求令牌的 web 应用程序是必需的。</span><span class="sxs-lookup"><span data-stu-id="feba5-150">Make sure to enable implicit grant flow; this is a requirement for web apps that request tokens from the client side.</span></span> <span data-ttu-id="feba5-151">在 Azure 门户中，在管理应用注册时，请编辑清单并更改 `oauth2AllowImplicitFlow` 为 `true` 。</span><span class="sxs-lookup"><span data-stu-id="feba5-151">In the Azure Portal, when managing your app registration, edit the manifest and change `oauth2AllowImplicitFlow` to `true`.</span></span>

### <a name="create-the-popup-page"></a><span data-ttu-id="feba5-152">创建弹出页</span><span class="sxs-lookup"><span data-stu-id="feba5-152">Create the popup page</span></span>

<span data-ttu-id="feba5-153">若要使用你的团队凭据登录，你需要提供团队应用将在弹出项中打开的 URL，这将遵循身份验证流。</span><span class="sxs-lookup"><span data-stu-id="feba5-153">In order to sign in with your Teams credentials, you need to provide a URL that the Teams app will open in a popup, which will follow the authentication flow.</span></span> <span data-ttu-id="feba5-154">此 URL 必须在您的域中，并且需要调用该 `TeamsProvider.handleAuth();` 方法。</span><span class="sxs-lookup"><span data-stu-id="feba5-154">This URL needs to be in your domain, and it needs to call the `TeamsProvider.handleAuth();` method.</span></span> <span data-ttu-id="feba5-155">这是此页面唯一需要执行的操作。</span><span class="sxs-lookup"><span data-stu-id="feba5-155">That's the only thing that this page needs to do.</span></span> <span data-ttu-id="feba5-156">例如：</span><span class="sxs-lookup"><span data-stu-id="feba5-156">For example:</span></span>

```html
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js">

<script>
  mgt.TeamsProvider.handleAuth();
</script>
```

<span data-ttu-id="feba5-157">或通过身份验证弹出页面中引用的模块：</span><span class="sxs-lookup"><span data-stu-id="feba5-157">or via a module referenced in your auth popup page:</span></span>

```ts
import * as MicrosoftTeams from "@microsoft/teams-js/dist/MicrosoftTeams";
import {Providers, TeamsProvider} from '@microsoft/mgt';

TeamsProvider.microsoftTeamsLib = MicrosoftTeams;
TeamsProvider.handleAuth();
```

### <a name="configure-redirect-uris"></a><span data-ttu-id="feba5-158">配置重定向 Uri</span><span class="sxs-lookup"><span data-stu-id="feba5-158">Configure redirect URIs</span></span>

<span data-ttu-id="feba5-159">在您的网站上发布此页面后，您需要使用属性中的 URL `auth-popup-url/authPopupUrl` 。</span><span class="sxs-lookup"><span data-stu-id="feba5-159">After you publish this page on your website, you need to use the URL in the `auth-popup-url/authPopupUrl` property.</span></span> <span data-ttu-id="feba5-160">此外，还需要在 Azure AD 门户的应用配置中将此 URL 配置为有效的重定向 URI。</span><span class="sxs-lookup"><span data-stu-id="feba5-160">This URL also needs to be configured as a valid redirect URI in your app configuration in the Azure AD portal.</span></span>
