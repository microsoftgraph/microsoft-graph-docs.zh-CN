---
title: Microsoft Graph Toolkit
description: 开始在应用程序中Graph Toolkit Microsoft 应用。
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: 68260cf83f0e9bec34d2c3b23911d04c53143e76
ms.sourcegitcommit: 276a13a37c3772689dfc71f7cd47586c9581f27d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/24/2021
ms.locfileid: "52629152"
---
# <a name="getting-started-with-the-microsoft-graph-toolkit"></a><span data-ttu-id="8eb7d-103">Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="8eb7d-103">Getting started with the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="8eb7d-104">Microsoft Graph Toolkit组件可轻松添加到 Web 应用程序、SharePoint Web 部件或Microsoft Teams选项卡。</span><span class="sxs-lookup"><span data-stu-id="8eb7d-104">The Microsoft Graph Toolkit components can easily be added to your web application, SharePoint web part, or Microsoft Teams tabs.</span></span> <span data-ttu-id="8eb7d-105">这些组件基于 Web 标准，可用于纯 JavaScript 项目或热门 Web 框架（如 Reach、Angular、Vue.js 等）。</span><span class="sxs-lookup"><span data-stu-id="8eb7d-105">The components are based on web standards and can be used in both plain JavaScript projects or with popular web frameworks such as Reach, Angular, Vue.js, and more.</span></span>

<span data-ttu-id="8eb7d-106">你可以观看此简短视频，了解快速而轻松地开始使用 Toolkit。</span><span class="sxs-lookup"><span data-stu-id="8eb7d-106">You can watch this short video to see how quick and easy it is to get started with the Toolkit.</span></span>

> [!VIDEO https://www.youtube-nocookie.com/embed/oZCGb2MMxa0]

<span data-ttu-id="8eb7d-107">有关分步教程，请参阅 Microsoft Graph Toolkit[入门模块](/learn/modules/msgraph-toolkit-intro/)。</span><span class="sxs-lookup"><span data-stu-id="8eb7d-107">For a step-by-step tutorial, see the [Get started with Microsoft Graph Toolkit module](/learn/modules/msgraph-toolkit-intro/).</span></span> 

## <a name="set-up-your-microsoft-365-tenant"></a><span data-ttu-id="8eb7d-108">设置 Microsoft 365 租户</span><span class="sxs-lookup"><span data-stu-id="8eb7d-108">Set up your Microsoft 365 tenant</span></span>
<span data-ttu-id="8eb7d-109">为了使用租户进行Toolkit，你需要访问 Microsoft 365 租户。</span><span class="sxs-lookup"><span data-stu-id="8eb7d-109">In order to develop with the Toolkit, you need access to a Microsoft 365 tenant.</span></span> <span data-ttu-id="8eb7d-110">如果你没有，可以通过加入开发人员计划Microsoft 365免费订阅Microsoft 365[订阅](https://developer.microsoft.com/microsoft-365/dev-program)。</span><span class="sxs-lookup"><span data-stu-id="8eb7d-110">If you don't have one, you can get a free Microsoft 365 developer subscription by [joining the Microsoft 365 Developer Program](https://developer.microsoft.com/microsoft-365/dev-program).</span></span> <span data-ttu-id="8eb7d-111">若要详细了解如何配置订阅，请参阅设置Microsoft 365[开发人员订阅](/office/developer-program/microsoft-365-developer-program-get-started)。</span><span class="sxs-lookup"><span data-stu-id="8eb7d-111">For details about how to configure your subscription, see [Set up a Microsoft 365 developer subscription](/office/developer-program/microsoft-365-developer-program-get-started).</span></span>

## <a name="set-up-your-development-environment"></a><span data-ttu-id="8eb7d-112">设置开发环境</span><span class="sxs-lookup"><span data-stu-id="8eb7d-112">Set up your development environment</span></span>
<span data-ttu-id="8eb7d-113">若要使用 Toolkit 进行开发，您需要文本编辑器或 IDE。</span><span class="sxs-lookup"><span data-stu-id="8eb7d-113">To develop with the Toolkit, you will need a text editor or IDE.</span></span> <span data-ttu-id="8eb7d-114">可以使用自己选择的编辑器或 IDE，也可以免费[安装和Visual Studio Code](https://code.visualstudio.com/download) IDE。</span><span class="sxs-lookup"><span data-stu-id="8eb7d-114">You can use the editor or IDE of your choice or install and use [Visual Studio Code](https://code.visualstudio.com/download) for free.</span></span> <span data-ttu-id="8eb7d-115">你还需要新式 Web 浏览器，Microsoft Edge、Google Chrome 或 Firefox。</span><span class="sxs-lookup"><span data-stu-id="8eb7d-115">You will also need a modern web browser like Microsoft Edge, Google Chrome, or Firefox.</span></span> <span data-ttu-id="8eb7d-116">你还需要 LTS 版本的 Node.js，可以从 nodejs.org[安装。](https://nodejs.org)</span><span class="sxs-lookup"><span data-stu-id="8eb7d-116">You'll also need an LTS version of Node.js, which you can install from [nodejs.org](https://nodejs.org).</span></span>

## <a name="using-the-microsoft-graph-toolkit"></a><span data-ttu-id="8eb7d-117">使用 Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="8eb7d-117">Using the Microsoft Graph Toolkit</span></span>
<span data-ttu-id="8eb7d-118">可以在应用程序中使用 Microsoft Graph Toolkit，方法为通过 unpkg (直接引用加载程序) 安装 npm 包。</span><span class="sxs-lookup"><span data-stu-id="8eb7d-118">You can use the Microsoft Graph Toolkit in your application by referencing the loader directly (via unpkg) or by installing the npm package.</span></span>

# <a name="unpkg"></a>[<span data-ttu-id="8eb7d-119">unpkg</span><span class="sxs-lookup"><span data-stu-id="8eb7d-119">unpkg</span></span>](#tab/html)
<span data-ttu-id="8eb7d-120">若要通过 mgt-loader Toolkit脚本，请向代码添加脚本中的引用：</span><span class="sxs-lookup"><span data-stu-id="8eb7d-120">To use the Toolkit via mgt-loader, add the reference in a script to your code:</span></span>

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>

<mgt-msal2-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal2-provider>
<mgt-login></mgt-login>
```
# <a name="npm"></a>[<span data-ttu-id="8eb7d-121">npm</span><span class="sxs-lookup"><span data-stu-id="8eb7d-121">npm</span></span>](#tab/npm)
<span data-ttu-id="8eb7d-122">通过 ES6 模块使用 Toolkit 可以完全控制捆绑过程，并允许您仅捆绑应用程序所需的代码。</span><span class="sxs-lookup"><span data-stu-id="8eb7d-122">Using the Toolkit via ES6 modules will give you full control of the bundling process and allow you to bundle only the code you need for your application.</span></span> <span data-ttu-id="8eb7d-123">若要使用 ES6 模块，请向项目添加 npm 包：</span><span class="sxs-lookup"><span data-stu-id="8eb7d-123">To use the ES6 modules, add the npm package to your project:</span></span>

```cmd
npm install @microsoft/mgt
```
<span data-ttu-id="8eb7d-124">现在，你可以引用你正在使用的页面的所有组件：</span><span class="sxs-lookup"><span data-stu-id="8eb7d-124">Now you can reference all the components in the page you're using:</span></span>

```html
<script type="module" src="node_modules/@microsoft/mgt/dist/es6/index.js"></script>

<mgt-login></mgt-login>
<mgt-agenda></mgt-agenda>
```


---


## <a name="npm-packages"></a><span data-ttu-id="8eb7d-125">NPM 包</span><span class="sxs-lookup"><span data-stu-id="8eb7d-125">NPM packages</span></span>

<span data-ttu-id="8eb7d-126">Microsoft Graph Toolkit由多个 NPM 包决定，从而仅包含应用程序所需的代码。</span><span class="sxs-lookup"><span data-stu-id="8eb7d-126">The Microsoft Graph Toolkit is made up of several NPM packages, allowing you to only include the code you need for your applications.</span></span>

<span data-ttu-id="8eb7d-127"><b>@microsoft/mgt-element</b></span><span class="sxs-lookup"><span data-stu-id="8eb7d-127"><b>@microsoft/mgt-element</b></span></span>

<span data-ttu-id="8eb7d-128">是仅包含用于生成组件和提供程序的基类 `@microsoft/mgt-element` 的核心程序包。</span><span class="sxs-lookup"><span data-stu-id="8eb7d-128">The `@microsoft/mgt-element` is the core package that contains only the base classes used for building components and providers.</span></span> <span data-ttu-id="8eb7d-129">此包公开构建您自己的组件所需的所有必需类和接口，并导出用于生成自定义提供程序的 [IProvider 接口和 SimpleProvider](../providers/custom.md) 类。</span><span class="sxs-lookup"><span data-stu-id="8eb7d-129">This package exposes all  necessary classes and interfaces needed to build your own components and exports the [IProvider interface and SimpleProvider class](../providers/custom.md) for building custom providers.</span></span>

<span data-ttu-id="8eb7d-130"><b>@microsoft/mgt-components</b></span><span class="sxs-lookup"><span data-stu-id="8eb7d-130"><b>@microsoft/mgt-components</b></span></span>

<span data-ttu-id="8eb7d-131">程序包包含所有 Microsoft Graph连接的 Web 组件，如 、 `@microsoft/mgt-components` `Person` `PeoplePicker` 等。</span><span class="sxs-lookup"><span data-stu-id="8eb7d-131">The `@microsoft/mgt-components` package contains all Microsoft Graph connected web components, such as `Person`, `PeoplePicker`, and more.</span></span> 

<span data-ttu-id="8eb7d-132">**提供程序**</span><span class="sxs-lookup"><span data-stu-id="8eb7d-132">**Providers**</span></span>

<span data-ttu-id="8eb7d-133">提供程序可通过单个程序包提供，并可以根据需要进行安装。</span><span class="sxs-lookup"><span data-stu-id="8eb7d-133">Providers are available via a single package and can be installed as needed.</span></span> <span data-ttu-id="8eb7d-134">以下提供程序包可用：</span><span class="sxs-lookup"><span data-stu-id="8eb7d-134">The following provider packages are available:</span></span>

- <span data-ttu-id="8eb7d-135"><b>@micosoft/mgt-msal-provider</b></span><span class="sxs-lookup"><span data-stu-id="8eb7d-135"><b>@micosoft/mgt-msal-provider</b></span></span>

    <span data-ttu-id="8eb7d-136">[`@micosoft/mgt-msal-provider`](../providers/msal.md) 包含 `MsalProvider` 和 `mgt-msal-provider` 组件。</span><span class="sxs-lookup"><span data-stu-id="8eb7d-136">[`@micosoft/mgt-msal-provider`](../providers/msal.md) contains the `MsalProvider` and `mgt-msal-provider` component.</span></span> <span data-ttu-id="8eb7d-137">MSAL 提供程序使用 msal.js 在 Web 应用中进行身份验证，使用渐进式 Web 应用 (PA) 。</span><span class="sxs-lookup"><span data-stu-id="8eb7d-137">The MSAL provider uses msal.js for authenticating in web apps and Progressive Web Apps (PWAs).</span></span>

- <span data-ttu-id="8eb7d-138"><b>@micosoft/mgt-msal2-provider</b></span><span class="sxs-lookup"><span data-stu-id="8eb7d-138"><b>@micosoft/mgt-msal2-provider</b></span></span>

    <span data-ttu-id="8eb7d-139">[`@micosoft/mgt-msal2-provider`](../providers/msal2.md) 包含 `Msal2Provider` 和 `mgt-msal2-provider` 组件。</span><span class="sxs-lookup"><span data-stu-id="8eb7d-139">[`@micosoft/mgt-msal2-provider`](../providers/msal2.md) contains the `Msal2Provider` and `mgt-msal2-provider` component.</span></span> <span data-ttu-id="8eb7d-140">MSAL 提供程序使用 msal-browser 在 Web 应用和 PWA 中进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="8eb7d-140">The MSAL provider uses msal-browser for authenticating in web apps and PWAs.</span></span>

-  <span data-ttu-id="8eb7d-141"><b>@microsoft/mgt-teams-provider</b></span><span class="sxs-lookup"><span data-stu-id="8eb7d-141"><b>@microsoft/mgt-teams-provider</b></span></span>

    <span data-ttu-id="8eb7d-142">[`@microsoft/mgt-teams-provider`](../providers/teams.md) 包含 `TeamsProvider` 和 `mgt-teams-provider` 组件。</span><span class="sxs-lookup"><span data-stu-id="8eb7d-142">[`@microsoft/mgt-teams-provider`](../providers/teams.md) contains the `TeamsProvider` and `mgt-teams-provider` component.</span></span> <span data-ttu-id="8eb7d-143">该Microsoft Teams在选项卡应用程序中Microsoft Teams身份验证。</span><span class="sxs-lookup"><span data-stu-id="8eb7d-143">The Microsoft Teams provider enables authentication in Microsoft Teams tab application.</span></span>

- <span data-ttu-id="8eb7d-144"><b>@microsoft/mgt-sharepoint-provider</b></span><span class="sxs-lookup"><span data-stu-id="8eb7d-144"><b>@microsoft/mgt-sharepoint-provider</b></span></span>

    <span data-ttu-id="8eb7d-145">[`@microsoft/mgt-sharepoint-provider`](../providers/sharepoint.md)包含 `SharePointProvider` 用于在环境中进行身份验证SharePoint。</span><span class="sxs-lookup"><span data-stu-id="8eb7d-145">[`@microsoft/mgt-sharepoint-provider`](../providers/sharepoint.md) contains the `SharePointProvider` for authenticating in a SharePoint environment.</span></span> 

- <span data-ttu-id="8eb7d-146"><b>@microsoft/mgt-proxy-provider</b></span><span class="sxs-lookup"><span data-stu-id="8eb7d-146"><b>@microsoft/mgt-proxy-provider</b></span></span>

    <span data-ttu-id="8eb7d-147">[`@microsoft/mgt-proxy-provider`](../providers/proxy.md)包含 `ProxyProvider` 代理通过后端Graph调用的 for 应用程序。</span><span class="sxs-lookup"><span data-stu-id="8eb7d-147">[`@microsoft/mgt-proxy-provider`](../providers/proxy.md) contains the `ProxyProvider` for application that proxy Graph calls through a backend service.</span></span> 

<span data-ttu-id="8eb7d-148"><b>@microsoft/mgt</b></span><span class="sxs-lookup"><span data-stu-id="8eb7d-148"><b>@microsoft/mgt</b></span></span>

<span data-ttu-id="8eb7d-149">是包含上述所有程序包的主程序包，然后重新导出它们，以便可以通过你可以安装的单个程序包 `@microsoft/mgt` 获取它们。</span><span class="sxs-lookup"><span data-stu-id="8eb7d-149">The `@microsoft/mgt` is the main package that includes all above packages and re-exports them so they are available via a single package you can install.</span></span> 

<span data-ttu-id="8eb7d-150"><b>@microsoft/mgt-react</b></span><span class="sxs-lookup"><span data-stu-id="8eb7d-150"><b>@microsoft/mgt-react</b></span></span>

<span data-ttu-id="8eb7d-151">[`@microsoft/mgt-react`](./mgt-react.md)程序包包含所有自动生成的React组件，并依赖 `@microsoft/mgt` 该程序包。</span><span class="sxs-lookup"><span data-stu-id="8eb7d-151">The [`@microsoft/mgt-react`](./mgt-react.md) package contains all auto-generated React components and takes dependency on the `@microsoft/mgt` package.</span></span>

<span data-ttu-id="8eb7d-152"><b>@microsoft/mgt-spfx</b></span><span class="sxs-lookup"><span data-stu-id="8eb7d-152"><b>@microsoft/mgt-spfx</b></span></span>

<span data-ttu-id="8eb7d-153">[`@microsoft/mgt-spfx`](./mgt-spfx.md)该包包含SharePoint 框架解决方案中使用 Microsoft Graph Toolkit所需的SharePoint 框架库。</span><span class="sxs-lookup"><span data-stu-id="8eb7d-153">The [`@microsoft/mgt-spfx`](./mgt-spfx.md) package contains a SharePoint Framework library that's required to use Microsoft Graph Toolkit in SharePoint Framework solutions.</span></span>

## <a name="next-steps"></a><span data-ttu-id="8eb7d-154">后续步骤</span><span class="sxs-lookup"><span data-stu-id="8eb7d-154">Next Steps</span></span>
<span data-ttu-id="8eb7d-155">现在，你已准备好开始使用 Microsoft Graph Toolkit！</span><span class="sxs-lookup"><span data-stu-id="8eb7d-155">You're now ready to start developing with the Microsoft Graph Toolkit!</span></span> <span data-ttu-id="8eb7d-156">以下指南可帮助你入门：</span><span class="sxs-lookup"><span data-stu-id="8eb7d-156">The following guides are available to help you get started:</span></span>

- [<span data-ttu-id="8eb7d-157">注册 Azure Active Directory 应用</span><span class="sxs-lookup"><span data-stu-id="8eb7d-157">Register an Azure Active Directory app</span></span>](./add-aad-app-registration.md)
- <span data-ttu-id="8eb7d-158">[使用 JavaScript (生成 ](./build-a-web-app.md) Web)  (javaScript) </span><span class="sxs-lookup"><span data-stu-id="8eb7d-158">[Build a web app (JavaScript)](./build-a-web-app.md) (vanilla JavaScript)</span></span>
- [<span data-ttu-id="8eb7d-159">构建 web 应用程序 (React)</span><span class="sxs-lookup"><span data-stu-id="8eb7d-159">Build a web app (React)</span></span>](./use-toolkit-with-react.md)
- [<span data-ttu-id="8eb7d-160">构建 web 应用 (Angular)</span><span class="sxs-lookup"><span data-stu-id="8eb7d-160">Build a web app (Angular)</span></span>](./use-toolkit-with-angular.md)
- [<span data-ttu-id="8eb7d-161">构建 SharePoint Web 部件</span><span class="sxs-lookup"><span data-stu-id="8eb7d-161">Build a SharePoint web part</span></span>](./build-a-sharepoint-web-part.md)
- [<span data-ttu-id="8eb7d-162">构建 Microsoft Teams 选项卡</span><span class="sxs-lookup"><span data-stu-id="8eb7d-162">Build a Microsoft Teams tab</span></span>](./build-a-microsoft-teams-tab.md)
