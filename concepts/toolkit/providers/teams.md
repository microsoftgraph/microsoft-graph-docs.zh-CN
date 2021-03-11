---
title: Microsoft Teams 提供程序
description: 使用 Microsoft Teams 选项卡内的 Teams 提供程序促进身份验证和 Microsoft Graph 访问所有组件。
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 2d4bff6363cc87256f7ec3f9456fbd11f011b48e
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50719751"
---
# <a name="microsoft-teams-provider"></a><span data-ttu-id="96221-103">Microsoft Teams 提供程序</span><span class="sxs-lookup"><span data-stu-id="96221-103">Microsoft Teams provider</span></span>

<span data-ttu-id="96221-104">使用 Microsoft Teams 选项卡内的 Teams 提供程序促进身份验证和 Microsoft Graph 访问所有组件。</span><span class="sxs-lookup"><span data-stu-id="96221-104">Use the Teams provider inside your Microsoft Teams tab to facilitate authentication and Microsoft Graph access to all components.</span></span>

<span data-ttu-id="96221-105">若要了解有关身份验证提供程序的信息，请参阅 [提供程序](./providers.md)。</span><span class="sxs-lookup"><span data-stu-id="96221-105">To learn more about authentication providers, see [providers](./providers.md).</span></span>

><span data-ttu-id="96221-106">**提示：** 有关如何使用 Teams 提供商创建 Microsoft Teams 应用程序的详细信息，请参阅"生成 [Microsoft Teams"选项卡](../get-started/build-a-microsoft-teams-tab.md) 入门指南。</span><span class="sxs-lookup"><span data-stu-id="96221-106">**Tip:** For details about how to get started with creating a Microsoft Teams application with the Teams Provider, see the [Build a Microsoft Teams tab](../get-started/build-a-microsoft-teams-tab.md) getting started guide.</span></span>

## <a name="get-started"></a><span data-ttu-id="96221-107">入门</span><span class="sxs-lookup"><span data-stu-id="96221-107">Get started</span></span>

<span data-ttu-id="96221-108">在使用 Teams 提供程序之前，你将需要确保你已在你的页面中引用了[Microsoft Teams SDK。](/javascript/api/overview/msteams-client?view=msteams-client-js-latest&preserve-view=true#using-the-sdk)</span><span class="sxs-lookup"><span data-stu-id="96221-108">Before using the Teams provider, you will need to make sure you have referenced the [Microsoft Teams SDK](/javascript/api/overview/msteams-client?view=msteams-client-js-latest&preserve-view=true#using-the-sdk) in your page.</span></span>

# <a name="npm"></a>[<span data-ttu-id="96221-109">npm</span><span class="sxs-lookup"><span data-stu-id="96221-109">npm</span></span>](#tab/ts)

<span data-ttu-id="96221-110">请确保同时安装工具包和 Microsoft Teams SDK。</span><span class="sxs-lookup"><span data-stu-id="96221-110">Make sure to install both the toolkit and the Microsoft Teams SDK.</span></span>

```cmd
npm install @microsoft/mgt @microsoft/teams-js
```

<span data-ttu-id="96221-111">接下来，导入和使用提供程序。</span><span class="sxs-lookup"><span data-stu-id="96221-111">Next, import and use the provider.</span></span>

```ts
import * as microsoftTeams from "@microsoft/teams-js";
import {Providers, TeamsProvider} from '@microsoft/mgt';

TeamsProvider.microsoftTeamsLib = microsoftTeams;
Providers.globalProvider = new TeamsProvider(config);
```

<span data-ttu-id="96221-112">where `config` is</span><span class="sxs-lookup"><span data-stu-id="96221-112">where `config` is</span></span>

```ts
export interface TeamsConfig {
  clientId: string;
  authPopupUrl: string; // see below for creating the popup page
  scopes?: string[];
  msalOptions?: Configuration;
}
```

# <a name="unpkg"></a>[<span data-ttu-id="96221-113">unpkg</span><span class="sxs-lookup"><span data-stu-id="96221-113">unpkg</span></span>](#tab/html)

```html
<!-- Microsoft Teams sdk must be referenced before the toolkit -->
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>

<mgt-teams-provider
  client-id="<YOUR_CLIENT_ID>"
  auth-popup-url="/AUTH-PATH"
  scopes="User.Read,People.Read..."
  authority=""
></mgt-teams-provider>
```

### <a name="mgt-teams-provider-attributes"></a><span data-ttu-id="96221-114">mgt-teams-provider 属性</span><span class="sxs-lookup"><span data-stu-id="96221-114">mgt-teams-provider attributes</span></span>
| <span data-ttu-id="96221-115">属性</span><span class="sxs-lookup"><span data-stu-id="96221-115">Attribute</span></span> | <span data-ttu-id="96221-116">说明</span><span class="sxs-lookup"><span data-stu-id="96221-116">Description</span></span> |
| --- | --- |
| <span data-ttu-id="96221-117">client-id</span><span class="sxs-lookup"><span data-stu-id="96221-117">client-id</span></span>   | <span data-ttu-id="96221-118">字符串客户端 ID ([请参阅"配置 Teams"应用](#configure-your-teams-app)。</span><span class="sxs-lookup"><span data-stu-id="96221-118">String client ID (see [Configure your Teams app](#configure-your-teams-app).</span></span> <span data-ttu-id="96221-119">必需。</span><span class="sxs-lookup"><span data-stu-id="96221-119">Required.</span></span> |
| <span data-ttu-id="96221-120">auth-popup-url</span><span class="sxs-lookup"><span data-stu-id="96221-120">auth-popup-url</span></span>  | <span data-ttu-id="96221-121">将在弹出窗口中处理身份验证的页面的绝对路径或相对路径 (创建弹出窗口[页面) 。](#create-the-popup-page)</span><span class="sxs-lookup"><span data-stu-id="96221-121">Absolute or relative path to the page that will handle auth in the popup (see [Create the popup page](#create-the-popup-page)).</span></span> <span data-ttu-id="96221-122">必需。</span><span class="sxs-lookup"><span data-stu-id="96221-122">Required.</span></span> |
| <span data-ttu-id="96221-123">scopes</span><span class="sxs-lookup"><span data-stu-id="96221-123">scopes</span></span>  | <span data-ttu-id="96221-124">用户必须同意登录的范围的逗号分隔字符串。</span><span class="sxs-lookup"><span data-stu-id="96221-124">Comma separated strings for scopes the user must consent to on sign in.</span></span> <span data-ttu-id="96221-125">可选。</span><span class="sxs-lookup"><span data-stu-id="96221-125">Optional.</span></span> |
| <span data-ttu-id="96221-126">depends-on</span><span class="sxs-lookup"><span data-stu-id="96221-126">depends-on</span></span> | <span data-ttu-id="96221-127">另一个优先级较高的提供程序组件的元素选择器字符串。</span><span class="sxs-lookup"><span data-stu-id="96221-127">Element selector string of another higher-priority provider component.</span></span> <span data-ttu-id="96221-128">可选。</span><span class="sxs-lookup"><span data-stu-id="96221-128">Optional.</span></span> |
| <span data-ttu-id="96221-129">authority</span><span class="sxs-lookup"><span data-stu-id="96221-129">authority</span></span>    | <span data-ttu-id="96221-130">颁发机构字符串。</span><span class="sxs-lookup"><span data-stu-id="96221-130">Authority string.</span></span> <span data-ttu-id="96221-131">默认为公共颁发机构。</span><span class="sxs-lookup"><span data-stu-id="96221-131">The default is the common authority.</span></span> <span data-ttu-id="96221-132">对于单租户应用，请使用租户 ID 或租户名称。</span><span class="sxs-lookup"><span data-stu-id="96221-132">For single-tenant apps, use your tenant ID or tenant name.</span></span> <span data-ttu-id="96221-133">例如， `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` 或 `https://login.microsoftonline.com/[your-tenant-id]` 。</span><span class="sxs-lookup"><span data-stu-id="96221-133">For example, `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` or `https://login.microsoftonline.com/[your-tenant-id]`.</span></span> <span data-ttu-id="96221-134">可选。</span><span class="sxs-lookup"><span data-stu-id="96221-134">Optional.</span></span> |

---

### <a name="create-the-popup-page"></a><span data-ttu-id="96221-135">创建弹出窗口</span><span class="sxs-lookup"><span data-stu-id="96221-135">Create the popup page</span></span>

<span data-ttu-id="96221-136">若要使用 Teams 凭据登录，你需要提供 Teams 应用将在弹出窗口中打开的 URL，这将遵循身份验证流程。</span><span class="sxs-lookup"><span data-stu-id="96221-136">In order to sign in with your Teams credentials, you need to provide a URL that the Teams app will open in a popup, which will follow the authentication flow.</span></span> <span data-ttu-id="96221-137">此 URL 需要在你的域中，并且需要调用 `TeamsProvider.handleAuth();` 该方法。</span><span class="sxs-lookup"><span data-stu-id="96221-137">This URL needs to be in your domain, and it needs to call the `TeamsProvider.handleAuth();` method.</span></span> <span data-ttu-id="96221-138">这是此页面需要执行的唯一工作。</span><span class="sxs-lookup"><span data-stu-id="96221-138">That's the only thing that this page needs to do.</span></span> <span data-ttu-id="96221-139">例如：</span><span class="sxs-lookup"><span data-stu-id="96221-139">For example:</span></span>

# <a name="npm"></a>[<span data-ttu-id="96221-140">npm</span><span class="sxs-lookup"><span data-stu-id="96221-140">npm</span></span>](#tab/ts)

```ts
import * as microsoftTeams from "@microsoft/teams-js";
import {Providers, TeamsProvider} from '@microsoft/mgt';

TeamsProvider.microsoftTeamsLib = microsoftTeams;
TeamsProvider.handleAuth();
```

# <a name="unpkg"></a>[<span data-ttu-id="96221-141">unpkg</span><span class="sxs-lookup"><span data-stu-id="96221-141">unpkg</span></span>](#tab/html)

```html
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>

<script>
  mgt.TeamsProvider.handleAuth();
</script>
```
---

### <a name="configure-redirect-uris"></a><span data-ttu-id="96221-142">配置重定向 URI</span><span class="sxs-lookup"><span data-stu-id="96221-142">Configure redirect URIs</span></span>

<span data-ttu-id="96221-143">在网站上发布弹出窗口后，您需要使用属性中的 `auth-popup-url/authPopupUrl` URL。</span><span class="sxs-lookup"><span data-stu-id="96221-143">After you publish the popup page on your website, you need to use the URL in the `auth-popup-url/authPopupUrl` property.</span></span> <span data-ttu-id="96221-144">此 URL 还需要在 Azure AD 门户的应用配置中配置为有效的重定向 URI。</span><span class="sxs-lookup"><span data-stu-id="96221-144">This URL also needs to be configured as a valid redirect URI in your app configuration in the Azure AD portal.</span></span>

## <a name="configure-your-teams-app"></a><span data-ttu-id="96221-145">配置 Teams 应用</span><span class="sxs-lookup"><span data-stu-id="96221-145">Configure your Teams app</span></span>

<span data-ttu-id="96221-146">如果你刚开始使用 Teams 应用，请参阅"将[选项卡添加到 Microsoft Teams 应用"。](/microsoftteams/platform/concepts/tabs/tabs-overview)</span><span class="sxs-lookup"><span data-stu-id="96221-146">If you're just getting started with Teams apps, see [Add tabs to Microsoft Teams apps](/microsoftteams/platform/concepts/tabs/tabs-overview).</span></span> <span data-ttu-id="96221-147">您还可以使用 [App Studio](/microsoftteams/platform/get-started/get-started-app-studio) 快速开发应用清单。</span><span class="sxs-lookup"><span data-stu-id="96221-147">You can also use [App Studio](/microsoftteams/platform/get-started/get-started-app-studio) to quickly develop your app manifest.</span></span>
### <a name="creating-an-appclient-id"></a><span data-ttu-id="96221-148">创建应用/客户端 ID</span><span class="sxs-lookup"><span data-stu-id="96221-148">Creating an app/client ID</span></span>
<span data-ttu-id="96221-149">若要获取客户端 ID，需要在 Azure AD [中注册应用程序](../get-started/add-aad-app-registration.md) 。</span><span class="sxs-lookup"><span data-stu-id="96221-149">In order to get a client ID, you need to [register your application](../get-started/add-aad-app-registration.md) in Azure AD.</span></span> 
><span data-ttu-id="96221-150">**注意**：MSAL 仅支持 OAuth 的隐式流。</span><span class="sxs-lookup"><span data-stu-id="96221-150">**Note**: MSAL only supports the Implicit Flow for OAuth.</span></span> <span data-ttu-id="96221-151">请确保在 Azure 门户中启用应用程序中的隐式流 (默认情况下不会启用它) 。</span><span class="sxs-lookup"><span data-stu-id="96221-151">Make sure to enable Implicit Flow in your application in the Azure Portal (it is not enabled by default).</span></span> <span data-ttu-id="96221-152">在 **"身份验证**"下，找到 **隐式授予** 部分，并选中 **访问** 令牌和 **ID 令牌的复选框**。</span><span class="sxs-lookup"><span data-stu-id="96221-152">Under **Authentication**, find the **Implicit grant** section and select the checkboxes for **Access tokens** and **ID tokens**.</span></span> 

## <a name="see-also"></a><span data-ttu-id="96221-153">另请参阅</span><span class="sxs-lookup"><span data-stu-id="96221-153">See also</span></span>
* [<span data-ttu-id="96221-154">Microsoft Teams 选项卡示例</span><span class="sxs-lookup"><span data-stu-id="96221-154">Microsoft Teams tab sample</span></span>](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/teams-tab)
* [<span data-ttu-id="96221-155">构建 Microsoft Teams 选项卡</span><span class="sxs-lookup"><span data-stu-id="96221-155">Build a Microsoft Teams tab</span></span>](../get-started/build-a-microsoft-teams-tab.md)