---
title: 使用 Microsoft 网站生成 web Graph Toolkit
description: 开始使用 Microsoft Graph Toolkit 构建 Web Graph Toolkit。
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: 5eed45974428a2c6daf47d02144741d937e12c91
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579898"
---
# <a name="build-a-web-application-with-the-microsoft-graph-toolkit"></a><span data-ttu-id="8a5b8-103">使用 Microsoft 网站生成 web Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="8a5b8-103">Build a web application with the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="8a5b8-104">本主题介绍如何在用 vanilla JavaScript 编写的 Web Graph Toolkit Microsoft 应用程序入门。</span><span class="sxs-lookup"><span data-stu-id="8a5b8-104">This topic describes how to get started with the Microsoft Graph Toolkit in a web application written in vanilla JavaScript.</span></span> <span data-ttu-id="8a5b8-105">有关分步教程，请尝试 Microsoft Graph Toolkit[入门。](/learn/modules/msgraph-toolkit-intro/)</span><span class="sxs-lookup"><span data-stu-id="8a5b8-105">For a step-by-step tutorial, try the [Get started with Microsoft Graph Toolkit module](/learn/modules/msgraph-toolkit-intro/).</span></span> <span data-ttu-id="8a5b8-106">如果你想要了解如何将 web 应用程序与 web 框架Toolkit，[请参阅生成](./use-toolkit-with-react.md)Web (React) 或 生成[Web ](./use-toolkit-with-angular.md) (Angular) 。</span><span class="sxs-lookup"><span data-stu-id="8a5b8-106">If you would like to learn how to use the Toolkit with a web framework, see [Build a web app (React)](./use-toolkit-with-react.md) or [Build a web app (Angular)](./use-toolkit-with-angular.md).</span></span>

<span data-ttu-id="8a5b8-107">Microsoft Graph Toolkit入门包括以下步骤：</span><span class="sxs-lookup"><span data-stu-id="8a5b8-107">Getting started with the Microsoft Graph Toolkit involves the following steps:</span></span>
1. <span data-ttu-id="8a5b8-108">将 Microsoft Graph Toolkit添加到你的项目中。</span><span class="sxs-lookup"><span data-stu-id="8a5b8-108">Add Microsoft Graph Toolkit to your project.</span></span>
2. <span data-ttu-id="8a5b8-109">初始化 MSAL 2.0 提供程序。</span><span class="sxs-lookup"><span data-stu-id="8a5b8-109">Initialize the MSAL 2.0 Provider.</span></span>
3. <span data-ttu-id="8a5b8-110">添加组件。</span><span class="sxs-lookup"><span data-stu-id="8a5b8-110">Add components.</span></span>
4. <span data-ttu-id="8a5b8-111">测试应用程序。</span><span class="sxs-lookup"><span data-stu-id="8a5b8-111">Test your application.</span></span>

## <a name="add-the-microsoft-graph-toolkit-to-your-project"></a><span data-ttu-id="8a5b8-112">将 Microsoft Graph Toolkit添加到你的项目</span><span class="sxs-lookup"><span data-stu-id="8a5b8-112">Add the Microsoft Graph Toolkit to your project</span></span>
<span data-ttu-id="8a5b8-113">可以在应用程序中使用 Microsoft Graph Toolkit，方法为通过 unpkg (直接引用加载程序) 安装 npm 包。</span><span class="sxs-lookup"><span data-stu-id="8a5b8-113">You can use the Microsoft Graph Toolkit in your application by referencing the loader directly (via unpkg) or by installing the npm package.</span></span>

# <a name="unpkg"></a>[<span data-ttu-id="8a5b8-114">unpkg</span><span class="sxs-lookup"><span data-stu-id="8a5b8-114">unpkg</span></span>](#tab/html)
<span data-ttu-id="8a5b8-115">若要通过 mgt-loader Toolkit脚本，请向代码添加脚本中的引用：</span><span class="sxs-lookup"><span data-stu-id="8a5b8-115">To use the Toolkit via mgt-loader, add the reference in a script to your code:</span></span>

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
```
# <a name="npm"></a>[<span data-ttu-id="8a5b8-116">npm</span><span class="sxs-lookup"><span data-stu-id="8a5b8-116">npm</span></span>](#tab/npm)
<span data-ttu-id="8a5b8-117">通过 ES6 模块使用 Toolkit 可以完全控制捆绑过程，并允许您仅捆绑应用程序所需的代码。</span><span class="sxs-lookup"><span data-stu-id="8a5b8-117">Using the Toolkit via ES6 modules will give you full control of the bundling process and allow you to bundle only the code you need for your application.</span></span> <span data-ttu-id="8a5b8-118">若要使用 ES6 模块，请向项目添加 npm 包：</span><span class="sxs-lookup"><span data-stu-id="8a5b8-118">To use the ES6 modules, add the npm package to your project:</span></span>

```cmd
npm install @microsoft/mgt
```

---


> <span data-ttu-id="8a5b8-119">**注意**：如果你面向的浏览器（如 IE11）在本机不支持 Web 组件，可能需要包含 [填充](./overview.md#polyfills)。</span><span class="sxs-lookup"><span data-stu-id="8a5b8-119">**Note**: If you're targeting a browser such as IE11 that does not support web components natively, you might need to [include polyfills](./overview.md#polyfills).</span></span>

## <a name="initialize-the-msal-20-provider"></a><span data-ttu-id="8a5b8-120">初始化 MSAL 2.0 提供程序</span><span class="sxs-lookup"><span data-stu-id="8a5b8-120">Initialize the MSAL 2.0 Provider</span></span>
<span data-ttu-id="8a5b8-121">Microsoft Graph Toolkit提供程序支持对组件的 Microsoft Graph进行身份验证和访问。</span><span class="sxs-lookup"><span data-stu-id="8a5b8-121">The Microsoft Graph Toolkit providers enable authentication and access to Microsoft Graph for the components.</span></span> <span data-ttu-id="8a5b8-122">若要了解更多信息，请参阅 [使用提供程序](../providers/providers.md)。</span><span class="sxs-lookup"><span data-stu-id="8a5b8-122">To learn more, see [Using the providers](../providers/providers.md).</span></span> <span data-ttu-id="8a5b8-123">[MSAL 2.0 提供程序](../providers/msal2.md)使用 msal-browser 登录用户并获取令牌。</span><span class="sxs-lookup"><span data-stu-id="8a5b8-123">The [MSAL 2.0 Provider](../providers/msal2.md) uses msal-browser to sign in users and acquire tokens.</span></span> <span data-ttu-id="8a5b8-124">可以在 HTML 或 JavaScript 中初始化此提供程序。</span><span class="sxs-lookup"><span data-stu-id="8a5b8-124">You can initialize this provider in your HTML or JavaScript.</span></span>

> <span data-ttu-id="8a5b8-125">**注意**：如果你当前正在使用 MSAL 提供程序，并且要更新到 MSAL 2.0 提供程序，请按照此处列出的 [步骤操作](../providers/msal2.md#migrating-from-msal-provider-to-msal-2-provider)。</span><span class="sxs-lookup"><span data-stu-id="8a5b8-125">**Note**: If you are currently using MSAL Provider and would like to update to MSAL 2.0 Provider, follow the steps listed [here](../providers/msal2.md#migrating-from-msal-provider-to-msal-2-provider).</span></span>
<span data-ttu-id="8a5b8-126">如果要使用自己的后端身份验证，请使用代理 [提供程序](../providers/proxy.md) 替代 MSAL 2.0 提供程序。</span><span class="sxs-lookup"><span data-stu-id="8a5b8-126">If you would like to use your own backend authentication, use the [Proxy Provider](../providers/proxy.md) in place of the MSAL 2.0 provider.</span></span>

<span data-ttu-id="8a5b8-127">可以选择在 HTML 或 JavaScript 代码中初始化提供程序。</span><span class="sxs-lookup"><span data-stu-id="8a5b8-127">You can choose to initialize the provider in either your HTML or your JavaScript code.</span></span> 

# <a name="html"></a>[<span data-ttu-id="8a5b8-128">html</span><span class="sxs-lookup"><span data-stu-id="8a5b8-128">html</span></span>](#tab/HTML)
<span data-ttu-id="8a5b8-129">将 `mgt-msal2-provider` 组件添加到 HTML 页面，将 设置为 `client-id` 应用程序 client-id。</span><span class="sxs-lookup"><span data-stu-id="8a5b8-129">Add the `mgt-msal2-provider` component to your HTML page and set the `client-id` to your application client-id.</span></span>

```html
<mgt-msal2-provider client-id="<YOUR_CLIENT_ID"></mgt-msal2-provider>
```
# <a name="js"></a>[<span data-ttu-id="8a5b8-130">js</span><span class="sxs-lookup"><span data-stu-id="8a5b8-130">js</span></span>](#tab/JavaScript)
<span data-ttu-id="8a5b8-131">若要在 JavaScript 中初始化 MSAL 提供程序，请向应用程序添加以下代码：</span><span class="sxs-lookup"><span data-stu-id="8a5b8-131">To initialize the MSAL provider in your JavaScript, add the following code to your application:</span></span>

```js
import {Providers, Msal2Provider} from '@microsoft/mgt'

Providers.globalProvider = new Msal2Provider({
    clientId: "<YOUR_CLIENT_ID>"
})
```

---


<span data-ttu-id="8a5b8-132">客户端 ID 是初始化提供程序所需的唯一属性，但您可以设置其他选项。</span><span class="sxs-lookup"><span data-stu-id="8a5b8-132">The client ID is the only property required to initialize the provider, but you can set additional options.</span></span> <span data-ttu-id="8a5b8-133">有关完整列表，请参阅[Msal 2.0 Provider。](../providers/msal2.md)</span><span class="sxs-lookup"><span data-stu-id="8a5b8-133">For the full list, see [Msal 2.0 Provider](../providers/msal2.md).</span></span>

### <a name="creating-an-appclient-id"></a><span data-ttu-id="8a5b8-134">创建应用/客户端 ID</span><span class="sxs-lookup"><span data-stu-id="8a5b8-134">Creating an app/client ID</span></span>
<span data-ttu-id="8a5b8-135">若要获取客户端 ID，需要在 Azure AD 中 [注册](./add-aad-app-registration.md) 应用程序。</span><span class="sxs-lookup"><span data-stu-id="8a5b8-135">In order to get a client ID, you need to [register your application](./add-aad-app-registration.md) in Azure AD.</span></span> 

## <a name="add-components"></a><span data-ttu-id="8a5b8-136">添加组件</span><span class="sxs-lookup"><span data-stu-id="8a5b8-136">Add components</span></span>
<span data-ttu-id="8a5b8-137">初始化 MSAL 2.0 提供程序后，就可以开始使用任何Toolkit组件。</span><span class="sxs-lookup"><span data-stu-id="8a5b8-137">After you initialize the MSAL 2.0 provider, you can start using any of the Toolkit components.</span></span>

# <a name="html"></a>[<span data-ttu-id="8a5b8-138">html</span><span class="sxs-lookup"><span data-stu-id="8a5b8-138">html</span></span>](#tab/HTML)
<span data-ttu-id="8a5b8-139">下面是使用 mgt-loader 的完整工作示例、HTML 中初始化的 MSAL 提供程序和登录组件：</span><span class="sxs-lookup"><span data-stu-id="8a5b8-139">The following is a full working example using mgt-loader, the MSAL Provider initialized in HTML, and the Login component:</span></span>

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal2-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal2-provider>
<mgt-login></mgt-login>
```

<span data-ttu-id="8a5b8-140">这是使用 ES6 模块、HTML 中初始化的 MSAL 2.0 提供程序和登录组件的示例：</span><span class="sxs-lookup"><span data-stu-id="8a5b8-140">This is an example using the ES6 modules, the MSAL 2.0 Provider initialized in HTML, and the Login component:</span></span>

```html
<script type="module" src="node_modules/@microsoft/mgt/dist/es6/index.js"></script>

<mgt-msal2-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal2-provider>

<mgt-login></mgt-login>
```
# <a name="js"></a>[<span data-ttu-id="8a5b8-141">js</span><span class="sxs-lookup"><span data-stu-id="8a5b8-141">js</span></span>](#tab/JavaScript)
<span data-ttu-id="8a5b8-142">这是使用 ES6 模块、在 JavaScript 中初始化的 MSAL 2.0 提供程序和登录组件的示例：</span><span class="sxs-lookup"><span data-stu-id="8a5b8-142">This is an example using the ES6 modules, the MSAL 2.0 Provider initialized in JavaScript, and the Login component:</span></span>

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


## <a name="test-your-app"></a><span data-ttu-id="8a5b8-143">测试应用</span><span class="sxs-lookup"><span data-stu-id="8a5b8-143">Test your app</span></span>

<span data-ttu-id="8a5b8-144">为了测试你的应用，MSAL 要求将页面托管在 Web 服务器中，以便进行身份验证重定向。</span><span class="sxs-lookup"><span data-stu-id="8a5b8-144">In order to test your app, MSAL requires the page to be hosted in a web server for the authentication redirects.</span></span> 

<span data-ttu-id="8a5b8-145">如果你刚开始工作并且想要玩游戏，可以在 Visual Studio Code或任何类似的轻型开发服务器中使用[Live](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) Server。</span><span class="sxs-lookup"><span data-stu-id="8a5b8-145">If you're just getting started and want to play around, you can use [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) in Visual Studio Code or any similar lightweight development server.</span></span> <span data-ttu-id="8a5b8-146">下载扩展名，然后使用实时服务器打开 HTML 文件。</span><span class="sxs-lookup"><span data-stu-id="8a5b8-146">Download the extension and open your HTML file using live server.</span></span> 
> <span data-ttu-id="8a5b8-147">**注意：** 确保应用 **注册中的重定向 URI** 设置为托管应用程序的 localhost 端口。</span><span class="sxs-lookup"><span data-stu-id="8a5b8-147">**Note:** Make sure the **redirect URI** in your app registration is set to the localhost port your application is hosted on.</span></span> <span data-ttu-id="8a5b8-148">转到 Azure 门户中的应用注册 [，](https://portal.azure.com)单击"管理"下的"身份验证"，然后添加正确的 **重定向 URI。**</span><span class="sxs-lookup"><span data-stu-id="8a5b8-148">Go to your app registration in the [Azure portal](https://portal.azure.com), click **Authentication** under manage, and add the correct **redirect URI**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="8a5b8-149">后续步骤</span><span class="sxs-lookup"><span data-stu-id="8a5b8-149">Next Steps</span></span>
- <span data-ttu-id="8a5b8-150">请查看 Microsoft [Graph Toolkit](/learn/modules/msgraph-toolkit-intro/)入门教程。</span><span class="sxs-lookup"><span data-stu-id="8a5b8-150">Check out the [Get started with Microsoft Graph Toolkit](/learn/modules/msgraph-toolkit-intro/) step-by-step tutorial.</span></span>
- <span data-ttu-id="8a5b8-151">尝试在运动场中的 [组件](https://mgt.dev)。</span><span class="sxs-lookup"><span data-stu-id="8a5b8-151">Try out the components in the [playground](https://mgt.dev).</span></span>
- <span data-ttu-id="8a5b8-152">在 Stack [Overflow 上提问](https://aka.ms/mgt-question)。</span><span class="sxs-lookup"><span data-stu-id="8a5b8-152">Ask a question on [Stack Overflow](https://aka.ms/mgt-question).</span></span>
- <span data-ttu-id="8a5b8-153">报告 Bug 或将功能请求[保留GitHub。](https://aka.ms/mgt)</span><span class="sxs-lookup"><span data-stu-id="8a5b8-153">Report bugs or leave a feature request on [GitHub](https://aka.ms/mgt).</span></span>
