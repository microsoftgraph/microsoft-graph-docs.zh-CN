---
title: 使用 Microsoft Graph 应用程序生成Toolkit
description: 开始使用 Microsoft Graph Toolkit。
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: 73e61e9d2c1c453ec67e61dce1f088b5119d1e8d
ms.sourcegitcommit: 7902607a1e5a030d46e907d08e16644a47a47006
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/12/2020
ms.locfileid: "49664014"
---
# <a name="build-a-web-application-with-the-microsoft-graph-toolkit"></a><span data-ttu-id="3a0f9-103">使用 Microsoft Graph 应用程序生成Toolkit</span><span class="sxs-lookup"><span data-stu-id="3a0f9-103">Build a web application with the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="3a0f9-104">本主题介绍如何在用 javaScript 编写的 Web 应用程序中Toolkit Microsoft Graph 应用程序入门。</span><span class="sxs-lookup"><span data-stu-id="3a0f9-104">This topic describes how to get started with the Microsoft Graph Toolkit in a web application written in vanilla JavaScript.</span></span> <span data-ttu-id="3a0f9-105">如果你想要了解如何将 Toolkit 与 Web 框架一起使用，请参阅"生成 Web 应用[ (React) "](./use-toolkit-with-react.md)或"使用 Angular (生成 web [) "。 ](./use-toolkit-with-angular.md)</span><span class="sxs-lookup"><span data-stu-id="3a0f9-105">If you would like to learn how to use the Toolkit with a web framework, see [Build a web app (React)](./use-toolkit-with-react.md) or [Build a web app (Angular)](./use-toolkit-with-angular.md).</span></span>

<span data-ttu-id="3a0f9-106">Microsoft Graph Toolkit入门包括以下步骤：</span><span class="sxs-lookup"><span data-stu-id="3a0f9-106">Getting started with the Microsoft Graph Toolkit involves the following steps:</span></span>
1. <span data-ttu-id="3a0f9-107">将 Microsoft Graph Toolkit添加到你的项目中。</span><span class="sxs-lookup"><span data-stu-id="3a0f9-107">Add Microsoft Graph Toolkit to your project.</span></span>
2. <span data-ttu-id="3a0f9-108">初始化 MSAL 提供程序。</span><span class="sxs-lookup"><span data-stu-id="3a0f9-108">Initialize the MSAL Provider.</span></span>
3. <span data-ttu-id="3a0f9-109">添加组件。</span><span class="sxs-lookup"><span data-stu-id="3a0f9-109">Add components.</span></span>
4. <span data-ttu-id="3a0f9-110">测试应用程序。</span><span class="sxs-lookup"><span data-stu-id="3a0f9-110">Test your application.</span></span>

## <a name="add-the-microsoft-graph-toolkit-to-your-project"></a><span data-ttu-id="3a0f9-111">将 Microsoft Graph Toolkit添加到项目</span><span class="sxs-lookup"><span data-stu-id="3a0f9-111">Add the Microsoft Graph Toolkit to your project</span></span>
<span data-ttu-id="3a0f9-112">可以在应用程序中使用 Microsoft Graph Toolkit，方法为直接通过取消 (加载程序) 安装 npm 包。</span><span class="sxs-lookup"><span data-stu-id="3a0f9-112">You can use the Microsoft Graph Toolkit in your application by referencing the loader directly (via unpkg) or by installing the npm package.</span></span>

# <a name="unpkg"></a>[<span data-ttu-id="3a0f9-113">unpkg</span><span class="sxs-lookup"><span data-stu-id="3a0f9-113">unpkg</span></span>](#tab/html)
<span data-ttu-id="3a0f9-114">若要通过 mgt Toolkit使用脚本，请向代码添加脚本中的引用：</span><span class="sxs-lookup"><span data-stu-id="3a0f9-114">To use the Toolkit via mgt-loader, add the reference in a script to your code:</span></span>

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
```
# <a name="npm"></a>[<span data-ttu-id="3a0f9-115">npm</span><span class="sxs-lookup"><span data-stu-id="3a0f9-115">npm</span></span>](#tab/npm)
<span data-ttu-id="3a0f9-116">通过 ES6 模块使用 Toolkit 可完全控制捆绑过程，并允许您仅捆绑应用程序所需的代码。</span><span class="sxs-lookup"><span data-stu-id="3a0f9-116">Using the Toolkit via ES6 modules will give you full control of the bundling process and allow you to bundle only the code you need for your application.</span></span> <span data-ttu-id="3a0f9-117">若要使用 ES6 模块，请向项目添加 npm 包：</span><span class="sxs-lookup"><span data-stu-id="3a0f9-117">To use the ES6 modules, add the npm package to your project:</span></span>

```cmd
npm install @microsoft/mgt
```

---


> <span data-ttu-id="3a0f9-118">**注意**：如果你面向的浏览器（如 IE11）在本机不支持 Web 组件，可能需要包括 [填充](./overview.md#polyfills)。</span><span class="sxs-lookup"><span data-stu-id="3a0f9-118">**Note**: If you're targeting a browser such as IE11 that does not support web components natively, you might need to [include polyfills](./overview.md#polyfills).</span></span>

## <a name="initialize-the-msal-provider"></a><span data-ttu-id="3a0f9-119">初始化 MSAL 提供程序</span><span class="sxs-lookup"><span data-stu-id="3a0f9-119">Initialize the MSAL Provider</span></span>
<span data-ttu-id="3a0f9-120">Microsoft Graph Toolkit提供程序为组件启用身份验证并访问 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="3a0f9-120">The Microsoft Graph Toolkit providers enable authentication and access to Microsoft Graph for the components.</span></span> <span data-ttu-id="3a0f9-121">若要了解更多信息，请参阅["使用提供程序"。](../providers/providers.md)</span><span class="sxs-lookup"><span data-stu-id="3a0f9-121">To learn more, see [Using the providers](../providers/providers.md).</span></span> <span data-ttu-id="3a0f9-122">[MSAL 提供程序](../providers/msal.md)使用MSAL.js登录用户和获取令牌。</span><span class="sxs-lookup"><span data-stu-id="3a0f9-122">The [MSAL Provider](../providers/msal.md) uses MSAL.js to sign in users and acquire tokens.</span></span> <span data-ttu-id="3a0f9-123">可以在 HTML 或 JavaScript 中初始化 MSAL 提供程序。</span><span class="sxs-lookup"><span data-stu-id="3a0f9-123">You can initialize the MSAL provider in your HTML or JavaScript.</span></span>

<span data-ttu-id="3a0f9-124">如果要使用自己的后端身份验证，请使用代理 [提供程序](../providers/proxy.md) 替代 MSAL 提供程序。</span><span class="sxs-lookup"><span data-stu-id="3a0f9-124">If you would like to use your own backend authentication, use the [Proxy Provider](../providers/proxy.md) in place of the MSAL provider.</span></span>

<span data-ttu-id="3a0f9-125">可以选择在 HTML 或 JavaScript 代码中初始化提供程序。</span><span class="sxs-lookup"><span data-stu-id="3a0f9-125">You can choose to initialize the provider in either your HTML or your JavaScript code.</span></span> 

# <a name="html"></a>[<span data-ttu-id="3a0f9-126">html</span><span class="sxs-lookup"><span data-stu-id="3a0f9-126">html</span></span>](#tab/HTML)
<span data-ttu-id="3a0f9-127">将 `mgt-msal-provider` 组件添加到 HTML 页面，并设置为 `client-id` 应用程序客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="3a0f9-127">Add the `mgt-msal-provider` component to your HTML page and set the `client-id` to your application client-id.</span></span>

```html
<mgt-msal-provider client-id="<YOUR_CLIENT_ID"></mgt-msal-provider>
```
# <a name="js"></a>[<span data-ttu-id="3a0f9-128">js</span><span class="sxs-lookup"><span data-stu-id="3a0f9-128">js</span></span>](#tab/JavaScript)
<span data-ttu-id="3a0f9-129">若要在 JavaScript 中初始化 MSAL 提供程序，请向应用程序添加以下代码：</span><span class="sxs-lookup"><span data-stu-id="3a0f9-129">To initialize the MSAL provider in your JavaScript, add the following code to your application:</span></span>

```js
import {Providers, MsalProvider} from '@microsoft/mgt'

Providers.globalProvider = new MsalProvider({
    clientId: "<YOUR_CLIENT_ID>"
})
```

---


<span data-ttu-id="3a0f9-130">客户端 ID 是初始化提供程序所需的唯一属性，但您可以设置其他选项。</span><span class="sxs-lookup"><span data-stu-id="3a0f9-130">The client ID is the only property required to initialize the provider, but you can set additional options.</span></span> <span data-ttu-id="3a0f9-131">有关完整列表，请参阅[Msal Provider。](../providers/msal.md)</span><span class="sxs-lookup"><span data-stu-id="3a0f9-131">For the full list, see [Msal Provider](../providers/msal.md).</span></span>

### <a name="creating-an-appclient-id"></a><span data-ttu-id="3a0f9-132">创建应用/客户端 ID</span><span class="sxs-lookup"><span data-stu-id="3a0f9-132">Creating an app/client ID</span></span>
<span data-ttu-id="3a0f9-133">若要获取客户端 ID，需要在 Azure AD 中 [注册](./add-aad-app-registration.md) 应用程序。</span><span class="sxs-lookup"><span data-stu-id="3a0f9-133">In order to get a client ID, you need to [register your application](./add-aad-app-registration.md) in Azure AD.</span></span> 
><span data-ttu-id="3a0f9-134">**注意**：MSAL 仅支持 OAuth 的隐式流。</span><span class="sxs-lookup"><span data-stu-id="3a0f9-134">**Note**: MSAL only supports the Implicit Flow for OAuth.</span></span> <span data-ttu-id="3a0f9-135">请确保在 Azure 门户中启用应用程序中的隐式流 (默认情况下未启用它) 。</span><span class="sxs-lookup"><span data-stu-id="3a0f9-135">Make sure to enable Implicit Flow in your application in the Azure Portal (it is not enabled by default).</span></span> <span data-ttu-id="3a0f9-136">在 **"身份验证**"下，找到 **隐式授予** 部分并选择 **访问** 令牌和 ID 令牌 **的复选框**。</span><span class="sxs-lookup"><span data-stu-id="3a0f9-136">Under **Authentication**, find the **Implicit grant** section and select the checkboxes for **Access tokens** and **ID tokens**.</span></span> 

## <a name="add-components"></a><span data-ttu-id="3a0f9-137">添加组件</span><span class="sxs-lookup"><span data-stu-id="3a0f9-137">Add components</span></span>
<span data-ttu-id="3a0f9-138">初始化 MSAL 提供程序后，就可以开始使用任何Toolkit组件。</span><span class="sxs-lookup"><span data-stu-id="3a0f9-138">After you initialize the MSAL provider, you can start using any of the Toolkit components.</span></span>

# <a name="html"></a>[<span data-ttu-id="3a0f9-139">html</span><span class="sxs-lookup"><span data-stu-id="3a0f9-139">html</span></span>](#tab/HTML)
<span data-ttu-id="3a0f9-140">下面是使用 mgt 加载程序、HTML 中初始化的 MSAL 提供程序和登录组件的完整工作示例：</span><span class="sxs-lookup"><span data-stu-id="3a0f9-140">The following is a full working example using mgt-loader, the MSAL Provider initialized in HTML, and the Login component:</span></span>

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal-provider>
<mgt-login></mgt-login>
```

<span data-ttu-id="3a0f9-141">这是使用 ES6 模块、HTML 中初始化的 MSAL 提供程序和登录组件的示例：</span><span class="sxs-lookup"><span data-stu-id="3a0f9-141">This is an example using the ES6 modules, the MSAL Provider initialized in HTML, and the Login component:</span></span>

```html
<script type="module" src="node_modules/@microsoft/mgt/dist/es6/index.js"></script>

<mgt-msal-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal-provider>

<mgt-login></mgt-login>
```
# <a name="js"></a>[<span data-ttu-id="3a0f9-142">js</span><span class="sxs-lookup"><span data-stu-id="3a0f9-142">js</span></span>](#tab/JavaScript)
<span data-ttu-id="3a0f9-143">这是使用 ES6 模块、在 JavaScript 中初始化的 MSAL 提供程序和登录组件的示例：</span><span class="sxs-lookup"><span data-stu-id="3a0f9-143">This is an example using the ES6 modules, the MSAL Provider initialized in JavaScript, and the Login component:</span></span>

```js
import {Providers, MsalProvider} from '@microsoft/mgt'

Providers.globalProvider = new MsalProvider({
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


## <a name="test-your-app"></a><span data-ttu-id="3a0f9-144">测试应用</span><span class="sxs-lookup"><span data-stu-id="3a0f9-144">Test your app</span></span>

<span data-ttu-id="3a0f9-145">为了测试你的应用，MSAL 要求页面承载在 Web 服务器中，以便进行身份验证重定向。</span><span class="sxs-lookup"><span data-stu-id="3a0f9-145">In order to test your app, MSAL requires the page to be hosted in a web server for the authentication redirects.</span></span> 

<span data-ttu-id="3a0f9-146">如果刚开始操作并且想要玩游戏，可以在 Visual Studio 代码或任何类似的轻型开发服务器中使用 [Live](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) Server。</span><span class="sxs-lookup"><span data-stu-id="3a0f9-146">If you're just getting started and want to play around, you can use [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) in Visual Studio Code or any similar lightweight development server.</span></span> <span data-ttu-id="3a0f9-147">下载扩展名，然后使用实时服务器打开 HTML 文件。</span><span class="sxs-lookup"><span data-stu-id="3a0f9-147">Download the extension and open your HTML file using live server.</span></span> 
> <span data-ttu-id="3a0f9-148">**注意：** 确保应用 **注册中的重定向 URI** 设置为托管应用程序的本地主机端口。</span><span class="sxs-lookup"><span data-stu-id="3a0f9-148">**Note:** Make sure the **redirect URI** in your app registration is set to the localhost port your application is hosted on.</span></span> <span data-ttu-id="3a0f9-149">转到 Azure 门户中的应用注册 [，](https://portal.azure.com)**单击"** 管理下的身份验证"，然后添加正确的 **重定向 URI。**</span><span class="sxs-lookup"><span data-stu-id="3a0f9-149">Go to your app registration in the [Azure portal](https://portal.azure.com), click **Authentication** under manage, and add the correct **redirect URI**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="3a0f9-150">后续步骤</span><span class="sxs-lookup"><span data-stu-id="3a0f9-150">Next Steps</span></span>
- <span data-ttu-id="3a0f9-151">请查看此有关生成简单 Web 应用的 [分步教程](https://developer.microsoft.com/microsoft-365/blogs/a-lap-around-microsoft-graph-toolkit-day-2-zero-to-hero/)。</span><span class="sxs-lookup"><span data-stu-id="3a0f9-151">Check out this step-by-step tutorial on [building a simple web app](https://developer.microsoft.com/microsoft-365/blogs/a-lap-around-microsoft-graph-toolkit-day-2-zero-to-hero/).</span></span>
- <span data-ttu-id="3a0f9-152">尝试在运动场 [中的组件](https://mgt.dev)。</span><span class="sxs-lookup"><span data-stu-id="3a0f9-152">Try out the components in the [playground](https://mgt.dev).</span></span>
- <span data-ttu-id="3a0f9-153">在 Stack [Overflow](https://aka.ms/mgt-question)上提问。</span><span class="sxs-lookup"><span data-stu-id="3a0f9-153">Ask a question on [Stack Overflow](https://aka.ms/mgt-question).</span></span>
- <span data-ttu-id="3a0f9-154">在 GitHub 上报告 Bug 或保留 [功能请求](https://aka.ms/mgt)。</span><span class="sxs-lookup"><span data-stu-id="3a0f9-154">Report bugs or leave a feature request on [GitHub](https://aka.ms/mgt).</span></span>