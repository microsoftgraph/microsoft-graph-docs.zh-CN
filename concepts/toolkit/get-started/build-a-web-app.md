---
title: 使用 Microsoft 网站生成 web Graph Toolkit
description: 开始使用 Microsoft Graph Toolkit 构建 Web Graph Toolkit。
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: eef2bb9644fdd7da95ccce5da2b6802f4e893573
ms.sourcegitcommit: 276a13a37c3772689dfc71f7cd47586c9581f27d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/24/2021
ms.locfileid: "52629495"
---
# <a name="build-a-web-application-with-the-microsoft-graph-toolkit"></a><span data-ttu-id="f8a0b-103">使用 Microsoft 网站生成 web Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="f8a0b-103">Build a web application with the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="f8a0b-104">本主题介绍如何在用 vanilla JavaScript 编写的 Web Graph Toolkit Microsoft 应用程序入门。</span><span class="sxs-lookup"><span data-stu-id="f8a0b-104">This topic describes how to get started with the Microsoft Graph Toolkit in a web application written in vanilla JavaScript.</span></span> <span data-ttu-id="f8a0b-105">有关分步教程，请尝试 Microsoft Graph Toolkit[入门。](/learn/modules/msgraph-toolkit-intro/)</span><span class="sxs-lookup"><span data-stu-id="f8a0b-105">For a step-by-step tutorial, try the [Get started with Microsoft Graph Toolkit module](/learn/modules/msgraph-toolkit-intro/).</span></span> <span data-ttu-id="f8a0b-106">如果你想要了解如何将 web 应用程序与 web 框架Toolkit，[请参阅生成](./use-toolkit-with-react.md)Web (React) 或 生成[Web ](./use-toolkit-with-angular.md) (Angular) 。</span><span class="sxs-lookup"><span data-stu-id="f8a0b-106">If you would like to learn how to use the Toolkit with a web framework, see [Build a web app (React)](./use-toolkit-with-react.md) or [Build a web app (Angular)](./use-toolkit-with-angular.md).</span></span>

<span data-ttu-id="f8a0b-107">Microsoft Graph Toolkit入门包括以下步骤：</span><span class="sxs-lookup"><span data-stu-id="f8a0b-107">Getting started with the Microsoft Graph Toolkit involves the following steps:</span></span>
1. <span data-ttu-id="f8a0b-108">将 Microsoft Graph Toolkit添加到你的项目中。</span><span class="sxs-lookup"><span data-stu-id="f8a0b-108">Add Microsoft Graph Toolkit to your project.</span></span>
2. <span data-ttu-id="f8a0b-109">初始化 MSAL 2.0 提供程序。</span><span class="sxs-lookup"><span data-stu-id="f8a0b-109">Initialize the MSAL 2.0 Provider.</span></span>
3. <span data-ttu-id="f8a0b-110">添加组件。</span><span class="sxs-lookup"><span data-stu-id="f8a0b-110">Add components.</span></span>
4. <span data-ttu-id="f8a0b-111">测试应用程序。</span><span class="sxs-lookup"><span data-stu-id="f8a0b-111">Test your application.</span></span>

## <a name="add-the-microsoft-graph-toolkit-to-your-project"></a><span data-ttu-id="f8a0b-112">将 Microsoft Graph Toolkit添加到你的项目</span><span class="sxs-lookup"><span data-stu-id="f8a0b-112">Add the Microsoft Graph Toolkit to your project</span></span>
<span data-ttu-id="f8a0b-113">可以在应用程序中使用 Microsoft Graph Toolkit，方法为通过 unpkg (直接引用加载程序) 安装 npm 包。</span><span class="sxs-lookup"><span data-stu-id="f8a0b-113">You can use the Microsoft Graph Toolkit in your application by referencing the loader directly (via unpkg) or by installing the npm package.</span></span>

# <a name="unpkg"></a>[<span data-ttu-id="f8a0b-114">unpkg</span><span class="sxs-lookup"><span data-stu-id="f8a0b-114">unpkg</span></span>](#tab/html)
<span data-ttu-id="f8a0b-115">若要通过 mgt-loader Toolkit脚本，请向代码添加脚本中的引用：</span><span class="sxs-lookup"><span data-stu-id="f8a0b-115">To use the Toolkit via mgt-loader, add the reference in a script to your code:</span></span>

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
```
# <a name="npm"></a>[<span data-ttu-id="f8a0b-116">npm</span><span class="sxs-lookup"><span data-stu-id="f8a0b-116">npm</span></span>](#tab/npm)
<span data-ttu-id="f8a0b-117">通过 ES6 模块使用 Toolkit 可以完全控制捆绑过程，并允许您仅捆绑应用程序所需的代码。</span><span class="sxs-lookup"><span data-stu-id="f8a0b-117">Using the Toolkit via ES6 modules will give you full control of the bundling process and allow you to bundle only the code you need for your application.</span></span> <span data-ttu-id="f8a0b-118">若要使用 ES6 模块，请向项目添加 npm 包：</span><span class="sxs-lookup"><span data-stu-id="f8a0b-118">To use the ES6 modules, add the npm package to your project:</span></span>

```cmd
npm install @microsoft/mgt
```

---

## <a name="initialize-the-msal-20-provider"></a><span data-ttu-id="f8a0b-119">初始化 MSAL 2.0 提供程序</span><span class="sxs-lookup"><span data-stu-id="f8a0b-119">Initialize the MSAL 2.0 Provider</span></span>
<span data-ttu-id="f8a0b-120">Microsoft Graph Toolkit提供程序支持对组件的 Microsoft Graph进行身份验证和访问。</span><span class="sxs-lookup"><span data-stu-id="f8a0b-120">The Microsoft Graph Toolkit providers enable authentication and access to Microsoft Graph for the components.</span></span> <span data-ttu-id="f8a0b-121">若要了解更多信息，请参阅 [使用提供程序](../providers/providers.md)。</span><span class="sxs-lookup"><span data-stu-id="f8a0b-121">To learn more, see [Using the providers](../providers/providers.md).</span></span> <span data-ttu-id="f8a0b-122">[MSAL 2.0 提供程序](../providers/msal2.md)使用 msal-browser 登录用户并获取令牌。</span><span class="sxs-lookup"><span data-stu-id="f8a0b-122">The [MSAL 2.0 Provider](../providers/msal2.md) uses msal-browser to sign in users and acquire tokens.</span></span> <span data-ttu-id="f8a0b-123">可以在 HTML 或 JavaScript 中初始化此提供程序。</span><span class="sxs-lookup"><span data-stu-id="f8a0b-123">You can initialize this provider in your HTML or JavaScript.</span></span>

> <span data-ttu-id="f8a0b-124">**注意**：如果你当前正在使用 MSAL 提供程序，并且要更新到 MSAL 2.0 提供程序，请按照此处列出的 [步骤操作](../providers/msal2.md#migrating-from-msal-provider-to-msal-2-provider)。</span><span class="sxs-lookup"><span data-stu-id="f8a0b-124">**Note**: If you are currently using MSAL Provider and would like to update to MSAL 2.0 Provider, follow the steps listed [here](../providers/msal2.md#migrating-from-msal-provider-to-msal-2-provider).</span></span>
<span data-ttu-id="f8a0b-125">如果要使用自己的后端身份验证，请使用代理 [提供程序](../providers/proxy.md) 替代 MSAL 2.0 提供程序。</span><span class="sxs-lookup"><span data-stu-id="f8a0b-125">If you would like to use your own backend authentication, use the [Proxy Provider](../providers/proxy.md) in place of the MSAL 2.0 provider.</span></span>

<span data-ttu-id="f8a0b-126">可以选择在 HTML 或 JavaScript 代码中初始化提供程序。</span><span class="sxs-lookup"><span data-stu-id="f8a0b-126">You can choose to initialize the provider in either your HTML or your JavaScript code.</span></span> 

# <a name="html"></a>[<span data-ttu-id="f8a0b-127">html</span><span class="sxs-lookup"><span data-stu-id="f8a0b-127">html</span></span>](#tab/HTML)
<span data-ttu-id="f8a0b-128">将 `mgt-msal2-provider` 组件添加到 HTML 页面，将 设置为 `client-id` 应用程序 client-id。</span><span class="sxs-lookup"><span data-stu-id="f8a0b-128">Add the `mgt-msal2-provider` component to your HTML page and set the `client-id` to your application client-id.</span></span>

```html
<mgt-msal2-provider client-id="<YOUR_CLIENT_ID"></mgt-msal2-provider>
```
# <a name="js"></a>[<span data-ttu-id="f8a0b-129">js</span><span class="sxs-lookup"><span data-stu-id="f8a0b-129">js</span></span>](#tab/JavaScript)
<span data-ttu-id="f8a0b-130">若要在 JavaScript 中初始化 MSAL 提供程序，请向应用程序添加以下代码：</span><span class="sxs-lookup"><span data-stu-id="f8a0b-130">To initialize the MSAL provider in your JavaScript, add the following code to your application:</span></span>

```js
import {Providers, Msal2Provider} from '@microsoft/mgt'

Providers.globalProvider = new Msal2Provider({
    clientId: "<YOUR_CLIENT_ID>"
})
```

---


<span data-ttu-id="f8a0b-131">客户端 ID 是初始化提供程序所需的唯一属性，但您可以设置其他选项。</span><span class="sxs-lookup"><span data-stu-id="f8a0b-131">The client ID is the only property required to initialize the provider, but you can set additional options.</span></span> <span data-ttu-id="f8a0b-132">有关完整列表，请参阅[Msal 2.0 Provider。](../providers/msal2.md)</span><span class="sxs-lookup"><span data-stu-id="f8a0b-132">For the full list, see [Msal 2.0 Provider](../providers/msal2.md).</span></span>

### <a name="creating-an-appclient-id"></a><span data-ttu-id="f8a0b-133">创建应用/客户端 ID</span><span class="sxs-lookup"><span data-stu-id="f8a0b-133">Creating an app/client ID</span></span>
<span data-ttu-id="f8a0b-134">若要获取客户端 ID，需要在 Azure AD 中 [注册](./add-aad-app-registration.md) 应用程序。</span><span class="sxs-lookup"><span data-stu-id="f8a0b-134">In order to get a client ID, you need to [register your application](./add-aad-app-registration.md) in Azure AD.</span></span> 

## <a name="add-components"></a><span data-ttu-id="f8a0b-135">添加组件</span><span class="sxs-lookup"><span data-stu-id="f8a0b-135">Add components</span></span>
<span data-ttu-id="f8a0b-136">初始化 MSAL 2.0 提供程序后，就可以开始使用任何Toolkit组件。</span><span class="sxs-lookup"><span data-stu-id="f8a0b-136">After you initialize the MSAL 2.0 provider, you can start using any of the Toolkit components.</span></span>

# <a name="html"></a>[<span data-ttu-id="f8a0b-137">html</span><span class="sxs-lookup"><span data-stu-id="f8a0b-137">html</span></span>](#tab/HTML)
<span data-ttu-id="f8a0b-138">下面是使用 mgt-loader 的完整工作示例、HTML 中初始化的 MSAL 提供程序和登录组件：</span><span class="sxs-lookup"><span data-stu-id="f8a0b-138">The following is a full working example using mgt-loader, the MSAL Provider initialized in HTML, and the Login component:</span></span>

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal2-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal2-provider>
<mgt-login></mgt-login>
```

<span data-ttu-id="f8a0b-139">这是使用 ES6 模块、HTML 中初始化的 MSAL 2.0 提供程序和登录组件的示例：</span><span class="sxs-lookup"><span data-stu-id="f8a0b-139">This is an example using the ES6 modules, the MSAL 2.0 Provider initialized in HTML, and the Login component:</span></span>

```html
<script type="module" src="node_modules/@microsoft/mgt/dist/es6/index.js"></script>

<mgt-msal2-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal2-provider>

<mgt-login></mgt-login>
```
# <a name="js"></a>[<span data-ttu-id="f8a0b-140">js</span><span class="sxs-lookup"><span data-stu-id="f8a0b-140">js</span></span>](#tab/JavaScript)
<span data-ttu-id="f8a0b-141">这是使用 ES6 模块、在 JavaScript 中初始化的 MSAL 2.0 提供程序和登录组件的示例：</span><span class="sxs-lookup"><span data-stu-id="f8a0b-141">This is an example using the ES6 modules, the MSAL 2.0 Provider initialized in JavaScript, and the Login component:</span></span>

```js
import {Providers, Msal2Provider} from '@microsoft/mgt'

Providers.globalProvider = new Msal2Provider({
    clientId: "<YOUR_CLIENT_ID>"
})

function component() {
    const element = document.createElement('div');
    element.innerHTML = '<mgt-login></mgt-login>'
    return element;
}

document.body.appendChild((component()));
```

---


## <a name="test-your-app"></a><span data-ttu-id="f8a0b-142">测试应用</span><span class="sxs-lookup"><span data-stu-id="f8a0b-142">Test your app</span></span>

<span data-ttu-id="f8a0b-143">为了测试你的应用，MSAL 要求将页面托管在 Web 服务器中，以便进行身份验证重定向。</span><span class="sxs-lookup"><span data-stu-id="f8a0b-143">In order to test your app, MSAL requires the page to be hosted in a web server for the authentication redirects.</span></span> 

<span data-ttu-id="f8a0b-144">如果你刚开始工作并且想要玩游戏，可以在 Visual Studio Code或任何类似的轻型开发服务器中使用[Live](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) Server。</span><span class="sxs-lookup"><span data-stu-id="f8a0b-144">If you're just getting started and want to play around, you can use [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) in Visual Studio Code or any similar lightweight development server.</span></span> <span data-ttu-id="f8a0b-145">下载扩展名，然后使用实时服务器打开 HTML 文件。</span><span class="sxs-lookup"><span data-stu-id="f8a0b-145">Download the extension and open your HTML file using live server.</span></span> 
> <span data-ttu-id="f8a0b-146">**注意：** 确保应用 **注册中的重定向 URI** 设置为托管应用程序的 localhost 端口。</span><span class="sxs-lookup"><span data-stu-id="f8a0b-146">**Note:** Make sure the **redirect URI** in your app registration is set to the localhost port your application is hosted on.</span></span> <span data-ttu-id="f8a0b-147">转到 Azure 门户中的应用注册 [，](https://portal.azure.com)单击"管理"下的"身份验证"，然后添加正确的 **重定向 URI。**</span><span class="sxs-lookup"><span data-stu-id="f8a0b-147">Go to your app registration in the [Azure portal](https://portal.azure.com), click **Authentication** under manage, and add the correct **redirect URI**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="f8a0b-148">后续步骤</span><span class="sxs-lookup"><span data-stu-id="f8a0b-148">Next Steps</span></span>
- <span data-ttu-id="f8a0b-149">请查看 Microsoft [Graph Toolkit](/learn/modules/msgraph-toolkit-intro/)入门教程。</span><span class="sxs-lookup"><span data-stu-id="f8a0b-149">Check out the [Get started with Microsoft Graph Toolkit](/learn/modules/msgraph-toolkit-intro/) step-by-step tutorial.</span></span>
- <span data-ttu-id="f8a0b-150">尝试在运动场中的 [组件](https://mgt.dev)。</span><span class="sxs-lookup"><span data-stu-id="f8a0b-150">Try out the components in the [playground](https://mgt.dev).</span></span>
- <span data-ttu-id="f8a0b-151">在 Stack [Overflow 上提问](https://aka.ms/mgt-question)。</span><span class="sxs-lookup"><span data-stu-id="f8a0b-151">Ask a question on [Stack Overflow](https://aka.ms/mgt-question).</span></span>
- <span data-ttu-id="f8a0b-152">报告 Bug 或将功能请求[保留GitHub。](https://aka.ms/mgt)</span><span class="sxs-lookup"><span data-stu-id="f8a0b-152">Report bugs or leave a feature request on [GitHub](https://aka.ms/mgt).</span></span>
