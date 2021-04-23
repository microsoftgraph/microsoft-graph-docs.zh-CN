---
title: Getting started with the Microsoft Graph Toolkit
description: 开始在应用程序中Toolkit Microsoft Graph 应用。
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: 3197542066d92978bf151d61a378e7f392633016
ms.sourcegitcommit: 2006bf01c60793ac6ab1e25fa0526ec5d33c6334
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/23/2021
ms.locfileid: "51961420"
---
# <a name="getting-started-with-the-microsoft-graph-toolkit"></a><span data-ttu-id="2eefb-103">Getting started with the Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="2eefb-103">Getting started with the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="2eefb-104">Microsoft Graph Toolkit组件可轻松添加到 Web 应用程序、SharePoint Web 部件或 Microsoft Teams 选项卡。</span><span class="sxs-lookup"><span data-stu-id="2eefb-104">The Microsoft Graph Toolkit components can easily be added to your web application, SharePoint web part, or Microsoft Teams tabs.</span></span> <span data-ttu-id="2eefb-105">这些组件基于 Web 标准，可用于纯 JavaScript 项目或热门 Web 框架（如 Reach、Angular、Vue.js 等）。</span><span class="sxs-lookup"><span data-stu-id="2eefb-105">The components are based on web standards and can be used in both plain JavaScript projects or with popular web frameworks such as Reach, Angular, Vue.js, and more.</span></span>

<span data-ttu-id="2eefb-106">你可以观看此简短视频，了解快速而轻松地开始使用 Toolkit。</span><span class="sxs-lookup"><span data-stu-id="2eefb-106">You can watch this short video to see how quick and easy it is to get started with the Toolkit.</span></span>

> [!VIDEO https://www.youtube-nocookie.com/embed/oZCGb2MMxa0]

<span data-ttu-id="2eefb-107">有关分步教程，请参阅 [Microsot Graph Toolkit入门模块](/learn/modules/msgraph-toolkit-intro/)。</span><span class="sxs-lookup"><span data-stu-id="2eefb-107">For a step-by-step tutorial, see the [Get started with Microsot Graph Toolkit module](/learn/modules/msgraph-toolkit-intro/).</span></span> 

## <a name="set-up-your-microsoft-365-tenant"></a><span data-ttu-id="2eefb-108">设置 Microsoft 365 租户</span><span class="sxs-lookup"><span data-stu-id="2eefb-108">Set up your Microsoft 365 tenant</span></span>
<span data-ttu-id="2eefb-109">为了使用 Microsoft 365 Toolkit，你需要访问 Microsoft 365 租户。</span><span class="sxs-lookup"><span data-stu-id="2eefb-109">In order to develop with the Toolkit, you need access to a Microsoft 365 tenant.</span></span> <span data-ttu-id="2eefb-110">如果没有，可以通过加入 Microsoft 365 开发人员计划获取免费的 [Microsoft 365 开发人员订阅](https://developer.microsoft.com/microsoft-365/dev-program)。</span><span class="sxs-lookup"><span data-stu-id="2eefb-110">If you don't have one, you can get a free Microsoft 365 developer subscription by [joining the Microsoft 365 Developer Program](https://developer.microsoft.com/microsoft-365/dev-program).</span></span> <span data-ttu-id="2eefb-111">若要详细了解如何配置订阅，请参阅 [设置 Microsoft 365 开发人员订阅](/office/developer-program/microsoft-365-developer-program-get-started)。</span><span class="sxs-lookup"><span data-stu-id="2eefb-111">For details about how to configure your subscription, see [Set up a Microsoft 365 developer subscription](/office/developer-program/microsoft-365-developer-program-get-started).</span></span>

## <a name="set-up-your-development-environment"></a><span data-ttu-id="2eefb-112">设置开发环境</span><span class="sxs-lookup"><span data-stu-id="2eefb-112">Set up your development environment</span></span>
<span data-ttu-id="2eefb-113">若要使用 Toolkit 进行开发，您需要文本编辑器或 IDE。</span><span class="sxs-lookup"><span data-stu-id="2eefb-113">To develop with the Toolkit, you will need a text editor or IDE.</span></span> <span data-ttu-id="2eefb-114">可以使用自己选择的编辑器或 IDE，也可以免费 [安装和Visual Studio代码](https://code.visualstudio.com/download) 。</span><span class="sxs-lookup"><span data-stu-id="2eefb-114">You can use the editor or IDE of your choice or install and use [Visual Studio Code](https://code.visualstudio.com/download) for free.</span></span> <span data-ttu-id="2eefb-115">你还需要 Microsoft Edge、Google Chrome 或 Firefox 等新式 Web 浏览器。</span><span class="sxs-lookup"><span data-stu-id="2eefb-115">You will also need a modern web browser like Microsoft Edge, Google Chrome, or Firefox.</span></span> <span data-ttu-id="2eefb-116">你还需要 LTS 版本的 Node.js，可以从 nodejs.org[安装。](https://nodejs.org)</span><span class="sxs-lookup"><span data-stu-id="2eefb-116">You'll also need an LTS version of Node.js, which you can install from [nodejs.org](https://nodejs.org).</span></span>

## <a name="using-the-microsoft-graph-toolkit"></a><span data-ttu-id="2eefb-117">使用 Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="2eefb-117">Using the Microsoft Graph Toolkit</span></span>
<span data-ttu-id="2eefb-118">可以在应用程序中使用 Microsoft Graph Toolkit，方法为通过 unpkg (直接引用加载程序) 安装 npm 包。</span><span class="sxs-lookup"><span data-stu-id="2eefb-118">You can use the Microsoft Graph Toolkit in your application by referencing the loader directly (via unpkg) or by installing the npm package.</span></span>

# <a name="unpkg"></a>[<span data-ttu-id="2eefb-119">unpkg</span><span class="sxs-lookup"><span data-stu-id="2eefb-119">unpkg</span></span>](#tab/html)
<span data-ttu-id="2eefb-120">若要通过 mgt-loader Toolkit脚本，请向代码添加脚本中的引用：</span><span class="sxs-lookup"><span data-stu-id="2eefb-120">To use the Toolkit via mgt-loader, add the reference in a script to your code:</span></span>

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>

<mgt-msal-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal-provider>
<mgt-login></mgt-login>
```
# <a name="npm"></a>[<span data-ttu-id="2eefb-121">npm</span><span class="sxs-lookup"><span data-stu-id="2eefb-121">npm</span></span>](#tab/npm)
<span data-ttu-id="2eefb-122">通过 ES6 模块Toolkit可完全控制捆绑过程，并允许您仅捆绑应用程序所需的代码。</span><span class="sxs-lookup"><span data-stu-id="2eefb-122">Using the Toolkit via ES6 modules will give you full control of the bundling process and allow you to bundle only the code you need for your application.</span></span> <span data-ttu-id="2eefb-123">若要使用 ES6 模块，请向项目添加 npm 包：</span><span class="sxs-lookup"><span data-stu-id="2eefb-123">To use the ES6 modules, add the npm package to your project:</span></span>

```cmd
npm install @microsoft/mgt
```
<span data-ttu-id="2eefb-124">现在，你可以引用你正在使用的页面的所有组件：</span><span class="sxs-lookup"><span data-stu-id="2eefb-124">Now you can reference all the components in the page you're using:</span></span>

```html
<script type="module" src="node_modules/@microsoft/mgt/dist/es6/index.js"></script>

<mgt-login></mgt-login>
<mgt-agenda></mgt-agenda>
```


---


## <a name="npm-packages"></a><span data-ttu-id="2eefb-125">NPM 包</span><span class="sxs-lookup"><span data-stu-id="2eefb-125">NPM packages</span></span>

<span data-ttu-id="2eefb-126">Microsoft Graph Toolkit由多个 NPM 包决定，从而仅包含应用程序所需的代码。</span><span class="sxs-lookup"><span data-stu-id="2eefb-126">The Microsoft Graph Toolkit is made up of several NPM packages, allowing you to only include the code you need for your applications.</span></span>

<span data-ttu-id="2eefb-127"><b>@microsoft/mgt-element</b></span><span class="sxs-lookup"><span data-stu-id="2eefb-127"><b>@microsoft/mgt-element</b></span></span>

<span data-ttu-id="2eefb-128">是仅包含用于生成组件和提供程序的基类 `@microsoft/mgt-element` 的核心程序包。</span><span class="sxs-lookup"><span data-stu-id="2eefb-128">The `@microsoft/mgt-element` is the core package that contains only the base classes used for building components and providers.</span></span> <span data-ttu-id="2eefb-129">此包公开构建您自己的组件所需的所有必需类和接口，并导出用于生成自定义提供程序的 [IProvider 接口和 SimpleProvider](../providers/custom.md) 类。</span><span class="sxs-lookup"><span data-stu-id="2eefb-129">This package exposes all  necessary classes and interfaces needed to build your own components and exports the [IProvider interface and SimpleProvider class](../providers/custom.md) for building custom providers.</span></span>

<span data-ttu-id="2eefb-130"><b>@microsoft/mgt-components</b></span><span class="sxs-lookup"><span data-stu-id="2eefb-130"><b>@microsoft/mgt-components</b></span></span>

<span data-ttu-id="2eefb-131">该 `@microsoft/mgt-components` 程序包包含所有连接的 Microsoft Graph Web 组件，如 、 `Person` `PeoplePicker` 等。</span><span class="sxs-lookup"><span data-stu-id="2eefb-131">The `@microsoft/mgt-components` package contains all Microsoft Graph connected web components, such as `Person`, `PeoplePicker`, and more.</span></span> 

<span data-ttu-id="2eefb-132">**提供程序**</span><span class="sxs-lookup"><span data-stu-id="2eefb-132">**Providers**</span></span>

<span data-ttu-id="2eefb-133">提供程序可通过单个程序包提供，并可以根据需要进行安装。</span><span class="sxs-lookup"><span data-stu-id="2eefb-133">Providers are available via a single package and can be installed as needed.</span></span> <span data-ttu-id="2eefb-134">以下提供程序包可用：</span><span class="sxs-lookup"><span data-stu-id="2eefb-134">The following provider packages are available:</span></span>

- <span data-ttu-id="2eefb-135"><b>@micosoft/mgt-msal-provider</b></span><span class="sxs-lookup"><span data-stu-id="2eefb-135"><b>@micosoft/mgt-msal-provider</b></span></span>

    <span data-ttu-id="2eefb-136">[`@micosoft/mgt-msal-provider`](../providers/msal.md) 包含 `MsalProvider` 和 `mgt-msal-provider` 组件。</span><span class="sxs-lookup"><span data-stu-id="2eefb-136">[`@micosoft/mgt-msal-provider`](../providers/msal.md) contains the `MsalProvider` and `mgt-msal-provider` component.</span></span> <span data-ttu-id="2eefb-137">msal 提供程序利用 msal.js Web 应用和 PWA 进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="2eefb-137">The msal provider leverages msal.js for authenticating in web apps and PWAs.</span></span>

-  <span data-ttu-id="2eefb-138"><b>@microsoft/mgt-teams-provider</b></span><span class="sxs-lookup"><span data-stu-id="2eefb-138"><b>@microsoft/mgt-teams-provider</b></span></span>

    <span data-ttu-id="2eefb-139">[`@microsoft/mgt-teams-provider`](../providers/teams.md) 包含 `TeamsProvider` 和 `mgt-teams-provider` 组件。</span><span class="sxs-lookup"><span data-stu-id="2eefb-139">[`@microsoft/mgt-teams-provider`](../providers/teams.md) contains the `TeamsProvider` and `mgt-teams-provider` component.</span></span> <span data-ttu-id="2eefb-140">Microsoft Teams 提供程序在 Microsoft Teams 选项卡应用程序中启用身份验证。</span><span class="sxs-lookup"><span data-stu-id="2eefb-140">The Microsoft Teams provider enables authentication in Microsoft Teams tab application.</span></span>

- <span data-ttu-id="2eefb-141"><b>@microsoft/mgt-sharepoint-provider</b></span><span class="sxs-lookup"><span data-stu-id="2eefb-141"><b>@microsoft/mgt-sharepoint-provider</b></span></span>

    <span data-ttu-id="2eefb-142">[`@microsoft/mgt-sharepoint-provider`](../providers/sharepoint.md) 包含 `SharePointProvider` 用于 SharePoint 环境中进行身份验证的 。</span><span class="sxs-lookup"><span data-stu-id="2eefb-142">[`@microsoft/mgt-sharepoint-provider`](../providers/sharepoint.md) contains the `SharePointProvider` for authenticating in a SharePoint environment.</span></span> 

- <span data-ttu-id="2eefb-143"><b>@microsoft/mgt-proxy-provider</b></span><span class="sxs-lookup"><span data-stu-id="2eefb-143"><b>@microsoft/mgt-proxy-provider</b></span></span>

    <span data-ttu-id="2eefb-144">[`@microsoft/mgt-proxy-provider`](../providers/proxy.md) 包含 `ProxyProvider` 通过后端服务代理 Graph 调用的 for 应用程序。</span><span class="sxs-lookup"><span data-stu-id="2eefb-144">[`@microsoft/mgt-proxy-provider`](../providers/proxy.md) contains the `ProxyProvider` for application that proxy Graph calls through a backend service.</span></span> 

<span data-ttu-id="2eefb-145"><b>@microsoft/mgt</b></span><span class="sxs-lookup"><span data-stu-id="2eefb-145"><b>@microsoft/mgt</b></span></span>

<span data-ttu-id="2eefb-146">是包含上述所有程序包的主程序包，然后重新导出它们，以便可以通过你可以安装的单个程序包 `@microsoft/mgt` 获取它们。</span><span class="sxs-lookup"><span data-stu-id="2eefb-146">The `@microsoft/mgt` is the main package that includes all above packages and re-exports them so they are available via a single package you can install.</span></span> 

<span data-ttu-id="2eefb-147"><b>@microsoft/mgt-react</b></span><span class="sxs-lookup"><span data-stu-id="2eefb-147"><b>@microsoft/mgt-react</b></span></span>

<span data-ttu-id="2eefb-148">该 [`@microsoft/mgt-react`](./mgt-react.md) 包包含所有自动生成的 React 组件，并且依赖 `@microsoft/mgt` 该程序包。</span><span class="sxs-lookup"><span data-stu-id="2eefb-148">The [`@microsoft/mgt-react`](./mgt-react.md) package contains all auto-generated React components and takes dependency on the `@microsoft/mgt` package.</span></span>

## <a name="polyfills"></a><span data-ttu-id="2eefb-149">Polyfills</span><span class="sxs-lookup"><span data-stu-id="2eefb-149">Polyfills</span></span>

<span data-ttu-id="2eefb-150">如果使用的是 npm 包中的 ES6 模块，并且面向的浏览器（如 [IE11）](https://caniuse.com/#search=components) 在本机不支持 Web 组件，则需要在项目中包含填充，因为它们不会自动包含。</span><span class="sxs-lookup"><span data-stu-id="2eefb-150">If you're using the ES6 modules from the npm package and you're [targeting a browser such as IE11](https://caniuse.com/#search=components) that does not support web components natively, you will need to include polyfills in your project, as they are not automatically included.</span></span> <span data-ttu-id="2eefb-151">填充有助于填充仍在更新以支持 Web 组件标准的浏览器中缺少的浏览器功能。</span><span class="sxs-lookup"><span data-stu-id="2eefb-151">Polyfills help to fill in missing browser capabilities in browsers that are still in the process of updating to support Web Component standards.</span></span> <span data-ttu-id="2eefb-152">有关说明和了解更多信息，请参阅 [填充文档](https://www.webcomponents.org/polyfills)。</span><span class="sxs-lookup"><span data-stu-id="2eefb-152">For instructions and to learn more, see [polyfills documentation](https://www.webcomponents.org/polyfills).</span></span> 

<span data-ttu-id="2eefb-153">如果你通过 mgt-loader 脚本使用 Toolkit填充已包含在内。</span><span class="sxs-lookup"><span data-stu-id="2eefb-153">The polyfills are already included if you're using the Toolkit via the mgt-loader script.</span></span>

## <a name="next-steps"></a><span data-ttu-id="2eefb-154">后续步骤</span><span class="sxs-lookup"><span data-stu-id="2eefb-154">Next Steps</span></span>
<span data-ttu-id="2eefb-155">现在可以开始使用 Microsoft Graph Toolkit！</span><span class="sxs-lookup"><span data-stu-id="2eefb-155">You're now ready to start developing with the Microsoft Graph Toolkit!</span></span> <span data-ttu-id="2eefb-156">以下指南可帮助你入门：</span><span class="sxs-lookup"><span data-stu-id="2eefb-156">The following guides are available to help you get started:</span></span>

- [<span data-ttu-id="2eefb-157">注册 Azure Active Directory 应用</span><span class="sxs-lookup"><span data-stu-id="2eefb-157">Register an Azure Active Directory app</span></span>](./add-aad-app-registration.md)
- <span data-ttu-id="2eefb-158">[使用 JavaScript (生成 ](./build-a-web-app.md) Web)  (javaScript) </span><span class="sxs-lookup"><span data-stu-id="2eefb-158">[Build a web app (JavaScript)](./build-a-web-app.md) (vanilla JavaScript)</span></span>
- [<span data-ttu-id="2eefb-159">构建 web 应用程序 (React)</span><span class="sxs-lookup"><span data-stu-id="2eefb-159">Build a web app (React)</span></span>](./use-toolkit-with-react.md)
- [<span data-ttu-id="2eefb-160">构建 web 应用 (Angular)</span><span class="sxs-lookup"><span data-stu-id="2eefb-160">Build a web app (Angular)</span></span>](./use-toolkit-with-angular.md)
- [<span data-ttu-id="2eefb-161">构建 SharePoint Web 部件</span><span class="sxs-lookup"><span data-stu-id="2eefb-161">Build a SharePoint web part</span></span>](./build-a-sharepoint-web-part.md)
- [<span data-ttu-id="2eefb-162">构建 Microsoft Teams 选项卡</span><span class="sxs-lookup"><span data-stu-id="2eefb-162">Build a Microsoft Teams tab</span></span>](./build-a-microsoft-teams-tab.md)
