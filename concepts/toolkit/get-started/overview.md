---
title: Microsoft Graph 工具包入门
description: 开始在应用程序中使用 Microsoft Graph 工具包。
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: e3739bb6180e19569ae40e873d3a018bbb541833
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48977133"
---
# <a name="getting-started-with-the-microsoft-graph-toolkit"></a><span data-ttu-id="5af1a-103">Microsoft Graph 工具包入门</span><span class="sxs-lookup"><span data-stu-id="5af1a-103">Getting started with the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="5af1a-104">可以轻松地将 Microsoft Graph 工具包组件添加到 web 应用程序、SharePoint web 部件或 Microsoft 团队选项卡。</span><span class="sxs-lookup"><span data-stu-id="5af1a-104">The Microsoft Graph Toolkit components can easily be added to your web application, SharePoint web part, or Microsoft Teams tabs.</span></span> <span data-ttu-id="5af1a-105">这些组件基于 web 标准，可在普通 JavaScript 项目中使用，也可用于常见的 web 框架，如 "接触"、"角度"、"Vue.js" 等。</span><span class="sxs-lookup"><span data-stu-id="5af1a-105">The components are based on web standards and can be used in both plain JavaScript projects or with popular web frameworks such as Reach, Angular, Vue.js, and more.</span></span>

<span data-ttu-id="5af1a-106">您可以观看这段短视频，了解如何快速轻松地开始使用工具包。</span><span class="sxs-lookup"><span data-stu-id="5af1a-106">You can watch this short video to see how quick and easy it is to get started with the Toolkit.</span></span>

> [!VIDEO https://www.youtube-nocookie.com/embed/oZCGb2MMxa0]

## <a name="set-up-your-microsoft-365-tenant"></a><span data-ttu-id="5af1a-107">设置你的 Microsoft 365 租户</span><span class="sxs-lookup"><span data-stu-id="5af1a-107">Set up your Microsoft 365 tenant</span></span>
<span data-ttu-id="5af1a-108">若要使用工具包进行开发，您需要访问 Microsoft 365 租户。</span><span class="sxs-lookup"><span data-stu-id="5af1a-108">In order to develop with the Toolkit, you need access to a Microsoft 365 tenant.</span></span> <span data-ttu-id="5af1a-109">如果没有，则可以通过 [加入 microsoft 365 开发人员计划](https://developer.microsoft.com/microsoft-365/dev-program)来获取免费的 microsoft 365 开发人员订阅。</span><span class="sxs-lookup"><span data-stu-id="5af1a-109">If you don't have one, you can get a free Microsoft 365 developer subscription by [joining the Microsoft 365 Developer Program](https://developer.microsoft.com/microsoft-365/dev-program).</span></span> <span data-ttu-id="5af1a-110">有关如何配置订阅的详细信息，请参阅 [Set up a Microsoft 365 developer 订阅](/office/developer-program/microsoft-365-developer-program-get-started)。</span><span class="sxs-lookup"><span data-stu-id="5af1a-110">For details about how to configure your subscription, see [Set up a Microsoft 365 developer subscription](/office/developer-program/microsoft-365-developer-program-get-started).</span></span>

## <a name="set-up-your-development-environment"></a><span data-ttu-id="5af1a-111">设置开发环境</span><span class="sxs-lookup"><span data-stu-id="5af1a-111">Set up your development environment</span></span>
<span data-ttu-id="5af1a-112">若要使用工具包进行开发，您将需要文本编辑器或 IDE。</span><span class="sxs-lookup"><span data-stu-id="5af1a-112">To develop with the Toolkit, you will need a text editor or IDE.</span></span> <span data-ttu-id="5af1a-113">您可以使用您选择的编辑器或 IDE，也可以免费安装和使用 [Visual Studio Code](https://code.visualstudio.com/download) 。</span><span class="sxs-lookup"><span data-stu-id="5af1a-113">You can use the editor or IDE of your choice or install and use [Visual Studio Code](https://code.visualstudio.com/download) for free.</span></span> <span data-ttu-id="5af1a-114">你还需要一个新式 web 浏览器，如 Microsoft Edge、Google Chrome 或 Firefox。</span><span class="sxs-lookup"><span data-stu-id="5af1a-114">You will also need a modern web browser like Microsoft Edge, Google Chrome, or Firefox.</span></span> <span data-ttu-id="5af1a-115">您还需要 Node.js 的 LTS 版本，可以从 [nodejs.org](https://nodejs.org)安装。</span><span class="sxs-lookup"><span data-stu-id="5af1a-115">You'll also need an LTS version of Node.js, which you can install from [nodejs.org](https://nodejs.org).</span></span>

## <a name="using-the-microsoft-graph-toolkit"></a><span data-ttu-id="5af1a-116">使用 Microsoft Graph 工具包</span><span class="sxs-lookup"><span data-stu-id="5af1a-116">Using the Microsoft Graph Toolkit</span></span>
<span data-ttu-id="5af1a-117">您可以在应用程序中使用 Microsoft Graph 工具包，方法是通过 unpkg) 或安装 npm 程序包直接 (引用加载程序。</span><span class="sxs-lookup"><span data-stu-id="5af1a-117">You can use the Microsoft Graph Toolkit in your application by referencing the loader directly (via unpkg) or by installing the npm package.</span></span>

### <a name="use-via-mgt-loader"></a><span data-ttu-id="5af1a-118">通过预加载加载程序使用</span><span class="sxs-lookup"><span data-stu-id="5af1a-118">Use via mgt-loader</span></span>
<span data-ttu-id="5af1a-119">若要通过预加载程序使用该工具包，请将脚本中的引用添加到代码中：</span><span class="sxs-lookup"><span data-stu-id="5af1a-119">To use the Toolkit via mgt-loader, add the reference in a script to your code:</span></span>

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
```

### <a name="use-via-npm-es6-modules"></a><span data-ttu-id="5af1a-120">通过 npm (ES6 模块使用) </span><span class="sxs-lookup"><span data-stu-id="5af1a-120">Use via npm (ES6 modules)</span></span>
<span data-ttu-id="5af1a-121">通过使用 ES6 模块中的工具包，可以完全控制捆绑过程，并允许您只捆绑应用程序所需的代码。</span><span class="sxs-lookup"><span data-stu-id="5af1a-121">Using the Toolkit via ES6 modules will give you full control of the bundling process and allow you to bundle only the code you need for your application.</span></span> <span data-ttu-id="5af1a-122">若要使用 ES6 模块，请将 npm 包添加到项目中：</span><span class="sxs-lookup"><span data-stu-id="5af1a-122">To use the ES6 modules, add the npm package to your project:</span></span>

```bash
npm install @microsoft/mgt
```
<span data-ttu-id="5af1a-123">现在，您可以引用要使用的页面中的所有组件：</span><span class="sxs-lookup"><span data-stu-id="5af1a-123">Now you can reference all the components in the page you're using:</span></span>

```html
<script src="node_modules/@microsoft/mgt/dist/es6/components.js"></script>
```

<span data-ttu-id="5af1a-124">或者，只引用所需的组件，避免加载其他所有内容：</span><span class="sxs-lookup"><span data-stu-id="5af1a-124">Or, just reference the component you need and avoid loading everything else:</span></span>
```html
<script src="node_modules/@microsoft/mgt/dist/es6/components/mgt-login/mgt-login.js"></script>
```

#### <a name="polyfills"></a><span data-ttu-id="5af1a-125">Polyfills.ts</span><span class="sxs-lookup"><span data-stu-id="5af1a-125">Polyfills</span></span>

<span data-ttu-id="5af1a-126">如果您使用 npm 程序包中的 ES6 模块，并且您针对的是不是本机支持 web 组件的 [浏览器（如 IE11](https://caniuse.com/#search=components) ），则需要在项目中包含 polyfills.ts，因为它们不会自动包含在内。</span><span class="sxs-lookup"><span data-stu-id="5af1a-126">If you're using the ES6 modules from the npm package and you're [targeting a browser such as IE11](https://caniuse.com/#search=components) that does not support web components natively, you will need to include polyfills in your project, as they are not automatically included.</span></span> <span data-ttu-id="5af1a-127">Polyfills.ts 帮助您在浏览器中填写缺少的浏览器功能，这些功能仍处于更新以支持 webcComponent 标准的过程中。</span><span class="sxs-lookup"><span data-stu-id="5af1a-127">Polyfills help to fill in missing browser capabilities in browsers that are still in the process of updating to support webcComponent standards.</span></span> <span data-ttu-id="5af1a-128">有关说明并了解详细信息，请参阅 [polyfills.ts 文档](https://www.webcomponents.org/polyfills)。</span><span class="sxs-lookup"><span data-stu-id="5af1a-128">For instructions and to learn more, see [polyfills documentation](https://www.webcomponents.org/polyfills).</span></span> 

<span data-ttu-id="5af1a-129">如果使用的是 "polyfills.ts"，则可通过 "预加载加载程序" 脚本使用该工具包。</span><span class="sxs-lookup"><span data-stu-id="5af1a-129">The polyfills are already included if you're using the Toolkit via the mgt-loader script.</span></span>

## <a name="next-steps"></a><span data-ttu-id="5af1a-130">后续步骤</span><span class="sxs-lookup"><span data-stu-id="5af1a-130">Next Steps</span></span>
<span data-ttu-id="5af1a-131">现在，你可以开始使用 Microsoft Graph 工具包进行开发了！</span><span class="sxs-lookup"><span data-stu-id="5af1a-131">You're now ready to start developing with the Microsoft Graph Toolkit!</span></span> <span data-ttu-id="5af1a-132">以下指南可帮助您入门：</span><span class="sxs-lookup"><span data-stu-id="5af1a-132">The following guides are available to help you get started:</span></span>

- [<span data-ttu-id="5af1a-133">创建 Azure Active Directory 应用程序</span><span class="sxs-lookup"><span data-stu-id="5af1a-133">Create an Azure Active Directory app</span></span>](./add-aad-app-registration.md)
- <span data-ttu-id="5af1a-134">[构建 web 应用程序](./build-a-web-app.md) (vanilla JavaScript) </span><span class="sxs-lookup"><span data-stu-id="5af1a-134">[Build a web application](./build-a-web-app.md) (vanilla JavaScript)</span></span>
- [<span data-ttu-id="5af1a-135">构建 SharePoint Web 部件</span><span class="sxs-lookup"><span data-stu-id="5af1a-135">Build a SharePoint web part</span></span>](./build-a-sharepoint-web-part.md)
- [<span data-ttu-id="5af1a-136">构建 Microsoft Teams 选项卡</span><span class="sxs-lookup"><span data-stu-id="5af1a-136">Build a Microsoft Teams tab</span></span>](./build-a-microsoft-teams-tab.md)
- [<span data-ttu-id="5af1a-137">将此工具包与响应结合使用</span><span class="sxs-lookup"><span data-stu-id="5af1a-137">Use the Toolkit with React</span></span>](./use-toolkit-with-react.md)
- [<span data-ttu-id="5af1a-138">使用具有角度的工具包</span><span class="sxs-lookup"><span data-stu-id="5af1a-138">Use the Toolkit with Angular</span></span>](./use-toolkit-with-angular.md)
