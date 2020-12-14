---
title: Getting started with the Microsoft Graph Toolkit
description: 开始在应用程序中Toolkit Microsoft Graph 应用。
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: f1451213822e2489f04bb454c355125ed95b1aed
ms.sourcegitcommit: 7902607a1e5a030d46e907d08e16644a47a47006
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/12/2020
ms.locfileid: "49664126"
---
# <a name="getting-started-with-the-microsoft-graph-toolkit"></a><span data-ttu-id="07f7d-103">Getting started with the Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="07f7d-103">Getting started with the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="07f7d-104">Microsoft Graph Toolkit组件可轻松添加到 Web 应用程序、SharePoint Web 部件或 Microsoft Teams 选项卡。</span><span class="sxs-lookup"><span data-stu-id="07f7d-104">The Microsoft Graph Toolkit components can easily be added to your web application, SharePoint web part, or Microsoft Teams tabs.</span></span> <span data-ttu-id="07f7d-105">这些组件基于 Web 标准，可用于纯 JavaScript 项目或热门 Web 框架（如 Reach、Angular、Vue.js等）。</span><span class="sxs-lookup"><span data-stu-id="07f7d-105">The components are based on web standards and can be used in both plain JavaScript projects or with popular web frameworks such as Reach, Angular, Vue.js, and more.</span></span>

<span data-ttu-id="07f7d-106">你可以观看此简短视频，了解快速而轻松地开始使用 Toolkit。</span><span class="sxs-lookup"><span data-stu-id="07f7d-106">You can watch this short video to see how quick and easy it is to get started with the Toolkit.</span></span>

> [!VIDEO https://www.youtube-nocookie.com/embed/oZCGb2MMxa0]

## <a name="set-up-your-microsoft-365-tenant"></a><span data-ttu-id="07f7d-107">设置 Microsoft 365 租户</span><span class="sxs-lookup"><span data-stu-id="07f7d-107">Set up your Microsoft 365 tenant</span></span>
<span data-ttu-id="07f7d-108">为了使用应用程序进行Toolkit，你需要访问 Microsoft 365 租户。</span><span class="sxs-lookup"><span data-stu-id="07f7d-108">In order to develop with the Toolkit, you need access to a Microsoft 365 tenant.</span></span> <span data-ttu-id="07f7d-109">如果你没有，可以通过加入 Microsoft 365 开发人员计划获取 [免费的 Microsoft 365 开发人员订阅](https://developer.microsoft.com/microsoft-365/dev-program)。</span><span class="sxs-lookup"><span data-stu-id="07f7d-109">If you don't have one, you can get a free Microsoft 365 developer subscription by [joining the Microsoft 365 Developer Program](https://developer.microsoft.com/microsoft-365/dev-program).</span></span> <span data-ttu-id="07f7d-110">若要详细了解如何配置订阅，请参阅 [设置 Microsoft 365 开发人员订阅](/office/developer-program/microsoft-365-developer-program-get-started)。</span><span class="sxs-lookup"><span data-stu-id="07f7d-110">For details about how to configure your subscription, see [Set up a Microsoft 365 developer subscription](/office/developer-program/microsoft-365-developer-program-get-started).</span></span>

## <a name="set-up-your-development-environment"></a><span data-ttu-id="07f7d-111">设置开发环境</span><span class="sxs-lookup"><span data-stu-id="07f7d-111">Set up your development environment</span></span>
<span data-ttu-id="07f7d-112">若要使用 Toolkit 进行开发，您需要文本编辑器或 IDE。</span><span class="sxs-lookup"><span data-stu-id="07f7d-112">To develop with the Toolkit, you will need a text editor or IDE.</span></span> <span data-ttu-id="07f7d-113">可以使用你选择的编辑器或 IDE，也可以免费安装和Visual Studio [代码](https://code.visualstudio.com/download) 。</span><span class="sxs-lookup"><span data-stu-id="07f7d-113">You can use the editor or IDE of your choice or install and use [Visual Studio Code](https://code.visualstudio.com/download) for free.</span></span> <span data-ttu-id="07f7d-114">你还需要一个新式 Web 浏览器，如 Microsoft Edge、Google Chrome 或 Firefox。</span><span class="sxs-lookup"><span data-stu-id="07f7d-114">You will also need a modern web browser like Microsoft Edge, Google Chrome, or Firefox.</span></span> <span data-ttu-id="07f7d-115">你还需要 LTS 版本的 Node.js，可以从[nodejs.org。](https://nodejs.org)</span><span class="sxs-lookup"><span data-stu-id="07f7d-115">You'll also need an LTS version of Node.js, which you can install from [nodejs.org](https://nodejs.org).</span></span>

## <a name="using-the-microsoft-graph-toolkit"></a><span data-ttu-id="07f7d-116">使用 Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="07f7d-116">Using the Microsoft Graph Toolkit</span></span>
<span data-ttu-id="07f7d-117">可以在应用程序中使用 Microsoft Graph Toolkit，方法为直接通过取消 (加载程序) 安装 npm 包。</span><span class="sxs-lookup"><span data-stu-id="07f7d-117">You can use the Microsoft Graph Toolkit in your application by referencing the loader directly (via unpkg) or by installing the npm package.</span></span>

# <a name="unpkg"></a>[<span data-ttu-id="07f7d-118">unpkg</span><span class="sxs-lookup"><span data-stu-id="07f7d-118">unpkg</span></span>](#tab/html)
<span data-ttu-id="07f7d-119">若要通过 mgt Toolkit使用脚本，请向代码添加脚本中的引用：</span><span class="sxs-lookup"><span data-stu-id="07f7d-119">To use the Toolkit via mgt-loader, add the reference in a script to your code:</span></span>

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>

<mgt-msal-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal-provider>
<mgt-login></mgt-login>
```
# <a name="npm"></a>[<span data-ttu-id="07f7d-120">npm</span><span class="sxs-lookup"><span data-stu-id="07f7d-120">npm</span></span>](#tab/npm)
<span data-ttu-id="07f7d-121">通过 ES6 模块使用 Toolkit 可完全控制捆绑过程，并允许您仅捆绑应用程序所需的代码。</span><span class="sxs-lookup"><span data-stu-id="07f7d-121">Using the Toolkit via ES6 modules will give you full control of the bundling process and allow you to bundle only the code you need for your application.</span></span> <span data-ttu-id="07f7d-122">若要使用 ES6 模块，请向项目添加 npm 包：</span><span class="sxs-lookup"><span data-stu-id="07f7d-122">To use the ES6 modules, add the npm package to your project:</span></span>

```cmd
npm install @microsoft/mgt
```
<span data-ttu-id="07f7d-123">现在，你可以引用你使用的页面的所有组件：</span><span class="sxs-lookup"><span data-stu-id="07f7d-123">Now you can reference all the components in the page you're using:</span></span>

```html
<script type="module" src="node_modules/@microsoft/mgt/dist/es6/index.js"></script>

<mgt-login></mgt-login>
<mgt-agenda></mgt-agenda>
```


---


## <a name="npm-packages"></a><span data-ttu-id="07f7d-124">NPM 包</span><span class="sxs-lookup"><span data-stu-id="07f7d-124">NPM packages</span></span>

<span data-ttu-id="07f7d-125">Microsoft Graph Toolkit由多个 NPM 包决定，因此只需包含应用程序所需的代码。</span><span class="sxs-lookup"><span data-stu-id="07f7d-125">The Microsoft Graph Toolkit is made up of several NPM packages, allowing you to only include the code you need for your applications.</span></span>

<span data-ttu-id="07f7d-126"><b>@microsoft/mgt-element</b></span><span class="sxs-lookup"><span data-stu-id="07f7d-126"><b>@microsoft/mgt-element</b></span></span>

<span data-ttu-id="07f7d-127">它是仅包含用于生成组件和提供程序的基 `@microsoft/mgt-element` 类的核心包。</span><span class="sxs-lookup"><span data-stu-id="07f7d-127">The `@microsoft/mgt-element` is the core package that contains only the base classes used for building components and providers.</span></span> <span data-ttu-id="07f7d-128">此包公开构建您自己的组件所需的所有必需类和接口，并导出用于生成自定义提供程序的 [IProvider 接口和 SimpleProvider](../providers/custom.md) 类。</span><span class="sxs-lookup"><span data-stu-id="07f7d-128">This package exposes all  necessary classes and interfaces needed to build your own components and exports the [IProvider interface and SimpleProvider class](../providers/custom.md) for building custom providers.</span></span>

<span data-ttu-id="07f7d-129"><b>@microsoft/mgt 组件</b></span><span class="sxs-lookup"><span data-stu-id="07f7d-129"><b>@microsoft/mgt-components</b></span></span>

<span data-ttu-id="07f7d-130">该 `@microsoft/mgt-components` 包包含所有 Microsoft Graph 连接的 Web 组件，如 `Person` ， `PeoplePicker` 等。</span><span class="sxs-lookup"><span data-stu-id="07f7d-130">The `@microsoft/mgt-components` package contains all Microsoft Graph connected web components, such as `Person`, `PeoplePicker`, and more.</span></span> 

<span data-ttu-id="07f7d-131">**提供程序**</span><span class="sxs-lookup"><span data-stu-id="07f7d-131">**Providers**</span></span>

<span data-ttu-id="07f7d-132">提供程序可通过单个程序包提供，并可以根据需要进行安装。</span><span class="sxs-lookup"><span data-stu-id="07f7d-132">Providers are available via a single package and can be installed as needed.</span></span> <span data-ttu-id="07f7d-133">以下提供程序包可用：</span><span class="sxs-lookup"><span data-stu-id="07f7d-133">The following provider packages are available:</span></span>

- <span data-ttu-id="07f7d-134"><b>@micosoft/mgt-msal-provider</b></span><span class="sxs-lookup"><span data-stu-id="07f7d-134"><b>@micosoft/mgt-msal-provider</b></span></span>

    <span data-ttu-id="07f7d-135">[`@micosoft/mgt-msal-provider`](../providers/msal.md) 包含 `MsalProvider` 和 `mgt-msal-provider` 组件。</span><span class="sxs-lookup"><span data-stu-id="07f7d-135">[`@micosoft/mgt-msal-provider`](../providers/msal.md) contains the `MsalProvider` and `mgt-msal-provider` component.</span></span> <span data-ttu-id="07f7d-136">msal 提供程序利用msal.js Web 应用和 PWA 进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="07f7d-136">The msal provider leverages msal.js for authenticating in web apps and PWAs.</span></span>

-  <span data-ttu-id="07f7d-137"><b>@microsoft/mgt-teams-provider</b></span><span class="sxs-lookup"><span data-stu-id="07f7d-137"><b>@microsoft/mgt-teams-provider</b></span></span>

    <span data-ttu-id="07f7d-138">[`@microsoft/mgt-teams-provider`](../providers/teams.md) 包含 `TeamsProvider` 和 `mgt-teams-provider` 组件。</span><span class="sxs-lookup"><span data-stu-id="07f7d-138">[`@microsoft/mgt-teams-provider`](../providers/teams.md) contains the `TeamsProvider` and `mgt-teams-provider` component.</span></span> <span data-ttu-id="07f7d-139">Microsoft Teams 提供程序在 Microsoft Teams 选项卡应用程序中启用身份验证。</span><span class="sxs-lookup"><span data-stu-id="07f7d-139">The Microsoft Teams provider enables authentication in Microsoft Teams tab application.</span></span>

- <span data-ttu-id="07f7d-140"><b>@microsoft/mgt-sharepoint-provider</b></span><span class="sxs-lookup"><span data-stu-id="07f7d-140"><b>@microsoft/mgt-sharepoint-provider</b></span></span>

    <span data-ttu-id="07f7d-141">[`@microsoft/mgt-sharepoint-provider`](../providers/sharepoint.md) 包含在 `SharePointProvider` SharePoint 环境中进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="07f7d-141">[`@microsoft/mgt-sharepoint-provider`](../providers/sharepoint.md) contains the `SharePointProvider` for authenticating in a SharePoint environment.</span></span> 

- <span data-ttu-id="07f7d-142"><b>@microsoft/mgt-proxy-provider</b></span><span class="sxs-lookup"><span data-stu-id="07f7d-142"><b>@microsoft/mgt-proxy-provider</b></span></span>

    <span data-ttu-id="07f7d-143">[`@microsoft/mgt-proxy-provider`](../providers/proxy.md) 包含 `ProxyProvider` 通过后端服务代理 Graph 调用的 for 应用程序。</span><span class="sxs-lookup"><span data-stu-id="07f7d-143">[`@microsoft/mgt-proxy-provider`](../providers/proxy.md) contains the `ProxyProvider` for application that proxy Graph calls through a backend service.</span></span> 

<span data-ttu-id="07f7d-144"><b>@microsoft/mgt</b></span><span class="sxs-lookup"><span data-stu-id="07f7d-144"><b>@microsoft/mgt</b></span></span>

<span data-ttu-id="07f7d-145">它是包含上述所有程序包的主程序包，并重新导出它们，以便它们可通过可安装的单个 `@microsoft/mgt` 程序包提供。</span><span class="sxs-lookup"><span data-stu-id="07f7d-145">The `@microsoft/mgt` is the main package that includes all above packages and re-exports them so they are available via a single package you can install.</span></span> 

<span data-ttu-id="07f7d-146"><b>@microsoft/mgt-react</b></span><span class="sxs-lookup"><span data-stu-id="07f7d-146"><b>@microsoft/mgt-react</b></span></span>

<span data-ttu-id="07f7d-147">该 [`@microsoft/mgt-react`](./mgt-react.md) 包包含所有自动生成的 React 组件，并依赖 `@microsoft/mgt` 该包。</span><span class="sxs-lookup"><span data-stu-id="07f7d-147">The [`@microsoft/mgt-react`](./mgt-react.md) package contains all auto-generated React components and takes dependency on the `@microsoft/mgt` package.</span></span>

## <a name="polyfills"></a><span data-ttu-id="07f7d-148">填充</span><span class="sxs-lookup"><span data-stu-id="07f7d-148">Polyfills</span></span>

<span data-ttu-id="07f7d-149">如果使用的是 npm 包中的 ES6 模块，并且面向的浏览器（如 [IE11）](https://caniuse.com/#search=components) 本机不支持 Web 组件，则需要在项目中包含填充，因为它们不会自动包含在项目中。</span><span class="sxs-lookup"><span data-stu-id="07f7d-149">If you're using the ES6 modules from the npm package and you're [targeting a browser such as IE11](https://caniuse.com/#search=components) that does not support web components natively, you will need to include polyfills in your project, as they are not automatically included.</span></span> <span data-ttu-id="07f7d-150">填充有助于填充仍在更新以支持 Web 组件标准的浏览器中缺少的浏览器功能。</span><span class="sxs-lookup"><span data-stu-id="07f7d-150">Polyfills help to fill in missing browser capabilities in browsers that are still in the process of updating to support Web Component standards.</span></span> <span data-ttu-id="07f7d-151">有关说明和了解更多信息，请参阅 [填充文档](https://www.webcomponents.org/polyfills)。</span><span class="sxs-lookup"><span data-stu-id="07f7d-151">For instructions and to learn more, see [polyfills documentation](https://www.webcomponents.org/polyfills).</span></span> 

<span data-ttu-id="07f7d-152">如果通过 mgt-loader 脚本使用 Toolkit，则已包含填充。</span><span class="sxs-lookup"><span data-stu-id="07f7d-152">The polyfills are already included if you're using the Toolkit via the mgt-loader script.</span></span>

## <a name="next-steps"></a><span data-ttu-id="07f7d-153">后续步骤</span><span class="sxs-lookup"><span data-stu-id="07f7d-153">Next Steps</span></span>
<span data-ttu-id="07f7d-154">现在，你已准备好开始使用 Microsoft Graph Toolkit！</span><span class="sxs-lookup"><span data-stu-id="07f7d-154">You're now ready to start developing with the Microsoft Graph Toolkit!</span></span> <span data-ttu-id="07f7d-155">以下指南可帮助你入门：</span><span class="sxs-lookup"><span data-stu-id="07f7d-155">The following guides are available to help you get started:</span></span>

- [<span data-ttu-id="07f7d-156">注册 Azure Active Directory 应用</span><span class="sxs-lookup"><span data-stu-id="07f7d-156">Register an Azure Active Directory app</span></span>](./add-aad-app-registration.md)
- <span data-ttu-id="07f7d-157">[使用 javaScript (javaScript)  (](./build-a-web-app.md) JavaScript) </span><span class="sxs-lookup"><span data-stu-id="07f7d-157">[Build a web app (JavaScript)](./build-a-web-app.md) (vanilla JavaScript)</span></span>
- [<span data-ttu-id="07f7d-158">构建 web 应用程序 (React)</span><span class="sxs-lookup"><span data-stu-id="07f7d-158">Build a web app (React)</span></span>](./use-toolkit-with-react.md)
- [<span data-ttu-id="07f7d-159">构建 web 应用 (Angular)</span><span class="sxs-lookup"><span data-stu-id="07f7d-159">Build a web app (Angular)</span></span>](./use-toolkit-with-angular.md)
- [<span data-ttu-id="07f7d-160">构建 SharePoint Web 部件</span><span class="sxs-lookup"><span data-stu-id="07f7d-160">Build a SharePoint web part</span></span>](./build-a-sharepoint-web-part.md)
- [<span data-ttu-id="07f7d-161">构建 Microsoft Teams 选项卡</span><span class="sxs-lookup"><span data-stu-id="07f7d-161">Build a Microsoft Teams tab</span></span>](./build-a-microsoft-teams-tab.md)
