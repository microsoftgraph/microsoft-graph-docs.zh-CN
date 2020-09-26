---
title: 使用 Microsoft Graph 工具包生成 web 应用程序
description: 使用 Microsoft Graph 工具包开始构建 web 应用程序。
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: 6852351e39aa3754ba7458bfe6fe5cd45f5cf635
ms.sourcegitcommit: 3fbc2249b307e8d3a9de18f22ef6911094ca272c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2020
ms.locfileid: "48288526"
---
# <a name="build-a-web-application-with-the-microsoft-graph-toolkit"></a><span data-ttu-id="c3982-103">使用 Microsoft Graph 工具包生成 web 应用程序</span><span class="sxs-lookup"><span data-stu-id="c3982-103">Build a web application with the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="c3982-104">本主题介绍如何在使用 vanilla JavaScript 编写的 web 应用程序中开始使用 Microsoft Graph 工具包。</span><span class="sxs-lookup"><span data-stu-id="c3982-104">This topic describes how to get started with the Microsoft Graph Toolkit in a web application written in vanilla JavaScript.</span></span> <span data-ttu-id="c3982-105">如果您想了解如何将此工具包与 web 框架结合使用，请参阅 [将此工具包与 "使用](./use-toolkit-with-react.md) " 进行响应或 [使用具有角度的工具包](./use-toolkit-with-angular.md)。</span><span class="sxs-lookup"><span data-stu-id="c3982-105">If you would like to learn how to use the Toolkit with a web framework, see [Use the Toolkit with React](./use-toolkit-with-react.md) or [Use the Toolkit with Angular](./use-toolkit-with-angular.md).</span></span>

<span data-ttu-id="c3982-106">Microsoft Graph 工具包入门包括以下步骤：</span><span class="sxs-lookup"><span data-stu-id="c3982-106">Getting started with the Microsoft Graph Toolkit involves the following steps:</span></span>
1. <span data-ttu-id="c3982-107">将 Microsoft Graph 工具包添加到项目中。</span><span class="sxs-lookup"><span data-stu-id="c3982-107">Add Microsoft Graph Toolkit to your project.</span></span>
2. <span data-ttu-id="c3982-108">初始化 MSAL 提供程序。</span><span class="sxs-lookup"><span data-stu-id="c3982-108">Initialize the MSAL Provider.</span></span>
3. <span data-ttu-id="c3982-109">添加组件。</span><span class="sxs-lookup"><span data-stu-id="c3982-109">Add components.</span></span>
4. <span data-ttu-id="c3982-110">测试应用程序。</span><span class="sxs-lookup"><span data-stu-id="c3982-110">Test your application.</span></span>

## <a name="add-the-microsoft-graph-toolkit-to-your-project"></a><span data-ttu-id="c3982-111">将 Microsoft Graph 工具包添加到项目中</span><span class="sxs-lookup"><span data-stu-id="c3982-111">Add the Microsoft Graph Toolkit to your project</span></span>
<span data-ttu-id="c3982-112">您可以在应用程序中使用 Microsoft Graph 工具包，方法是通过 unpkg) 或安装 npm 程序包直接 (引用加载程序。</span><span class="sxs-lookup"><span data-stu-id="c3982-112">You can use the Microsoft Graph Toolkit in your application by referencing the loader directly (via unpkg) or by installing the npm package.</span></span>

### <a name="use-via-mgt-loader"></a><span data-ttu-id="c3982-113">通过预加载加载程序使用</span><span class="sxs-lookup"><span data-stu-id="c3982-113">Use via mgt-loader</span></span>
<span data-ttu-id="c3982-114">若要通过预加载程序使用该工具包，请将脚本中的引用添加到代码中：</span><span class="sxs-lookup"><span data-stu-id="c3982-114">To use the Toolkit via mgt-loader, add the reference in a script to your code:</span></span>

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
```

### <a name="use-via-npm-es6-modules"></a><span data-ttu-id="c3982-115">通过 npm (ES6 模块使用) </span><span class="sxs-lookup"><span data-stu-id="c3982-115">Use via npm (ES6 modules)</span></span>
<span data-ttu-id="c3982-116">通过使用 ES6 模块中的工具包，可以完全控制捆绑过程，并允许您只捆绑应用程序所需的代码。</span><span class="sxs-lookup"><span data-stu-id="c3982-116">Using the Toolkit via ES6 modules will give you full control of the bundling process and allow you to bundle only the code you need for your application.</span></span> <span data-ttu-id="c3982-117">若要使用 ES6 模块，请将 npm 包添加到项目中：</span><span class="sxs-lookup"><span data-stu-id="c3982-117">To use the ES6 modules, add the npm package to your project:</span></span>

```bash
npm install @microsoft/mgt
```
> <span data-ttu-id="c3982-118">**注意**：如果您针对的是不是本机支持 web 组件的浏览器（如 IE11），则可能需要 [包含 polyfills.ts](./overview.md#polyfills)。</span><span class="sxs-lookup"><span data-stu-id="c3982-118">**Note**: If you're targeting a browser such as IE11 that does not support web components natively, you might need to [include polyfills](./overview.md#polyfills).</span></span>

<span data-ttu-id="c3982-119">现在，您可以通过以下方式引用应用程序中的所有工具包组件：</span><span class="sxs-lookup"><span data-stu-id="c3982-119">Now, you can reference the all the Toolkit components in your application with:</span></span>

```html
<script src="node_modules/@microsoft/mgt/dist/es6/components.js"></script>
```
<span data-ttu-id="c3982-120">或者，只引用所需的组件，避免加载其他内容。</span><span class="sxs-lookup"><span data-stu-id="c3982-120">Or, reference only the components you need and avoid loading everything else.</span></span> <span data-ttu-id="c3982-121">例如，若要添加 MSAL 提供程序：</span><span class="sxs-lookup"><span data-stu-id="c3982-121">For example, to add the MSAL Provider:</span></span>

```html
<script src="node_modules/@microsoft/mgt/dist/es6/components/providers/mgt-msal-provider.js"></script>
```

## <a name="initialize-the-msal-provider"></a><span data-ttu-id="c3982-122">初始化 MSAL 提供程序</span><span class="sxs-lookup"><span data-stu-id="c3982-122">Initialize the MSAL Provider</span></span>
<span data-ttu-id="c3982-123">Microsoft Graph 工具包提供程序启用对组件的 Microsoft Graph 的身份验证和访问。</span><span class="sxs-lookup"><span data-stu-id="c3982-123">The Microsoft Graph Toolkit providers enable authentication and access to Microsoft Graph for the components.</span></span> <span data-ttu-id="c3982-124">若要了解详细信息，请参阅 [使用提供程序](../providers.md)。</span><span class="sxs-lookup"><span data-stu-id="c3982-124">To learn more, see [Using the providers](../providers.md).</span></span> <span data-ttu-id="c3982-125">[MSAL 提供程序](../providers/msal.md)使用 MSAL.js 登录用户和获取令牌。</span><span class="sxs-lookup"><span data-stu-id="c3982-125">The [MSAL Provider](../providers/msal.md) uses MSAL.js to sign in users and acquire tokens.</span></span> <span data-ttu-id="c3982-126">您可以在 HTML 或 JavaScript 中初始化 MSAL 提供程序。</span><span class="sxs-lookup"><span data-stu-id="c3982-126">You can initialize the MSAL provider in your HTML or JavaScript.</span></span>

<span data-ttu-id="c3982-127">如果要使用自己的后端身份验证，请使用 [代理提供程序](../providers/proxy.md) 替换 MSAL 提供程序。</span><span class="sxs-lookup"><span data-stu-id="c3982-127">If you would like to use your own backend authentication, use the [Proxy Provider](../providers/proxy.md) in place of the MSAL provider.</span></span>

<span data-ttu-id="c3982-128">您可以选择在 HTML 或 JavaScript 代码中初始化提供程序。</span><span class="sxs-lookup"><span data-stu-id="c3982-128">You can choose to initialize the provider in either your HTML or your JavaScript code.</span></span> 

### <a name="initialize-in-your-html-page"></a><span data-ttu-id="c3982-129">在 HTML 页面中初始化</span><span class="sxs-lookup"><span data-stu-id="c3982-129">Initialize in your HTML page</span></span>
<span data-ttu-id="c3982-130">将 `mgt-msal-provider` 组件添加到 HTML 页面，并将设置 `client-id` 为应用程序客户端 id。</span><span class="sxs-lookup"><span data-stu-id="c3982-130">Add the `mgt-msal-provider` component to your HTML page and set the `client-id` to your application client-id.</span></span>

```html
<mgt-msal-provider client-id="<YOUR_CLIENT_ID"></mgt-msal-provider>
```
### <a name="initialize-in-javascript"></a><span data-ttu-id="c3982-131">在 JavaScript 中初始化</span><span class="sxs-lookup"><span data-stu-id="c3982-131">Initialize in JavaScript</span></span>
<span data-ttu-id="c3982-132">若要在 JavaScript 中初始化 MSAL 提供程序，请将以下代码添加到应用程序：</span><span class="sxs-lookup"><span data-stu-id="c3982-132">To initialize the MSAL provider in your JavaScript, add the following code to your application:</span></span>

```js
import {Providers, MsalProvider} from '@microsoft/mgt'

Providers.globalProvider = new MsalProvider({
    clientId: "<YOUR_CLIENT_ID>"
})
```
<span data-ttu-id="c3982-133">客户端 ID 是初始化提供程序所需的唯一属性，但您可以设置其他选项。</span><span class="sxs-lookup"><span data-stu-id="c3982-133">The client ID is the only property required to initialize the provider, but you can set additional options.</span></span> <span data-ttu-id="c3982-134">有关完整列表，请参阅 [Msal Provider](../providers/msal.md)。</span><span class="sxs-lookup"><span data-stu-id="c3982-134">For the full list, see [Msal Provider](../providers/msal.md).</span></span>

### <a name="creating-an-appclient-id"></a><span data-ttu-id="c3982-135">创建应用/客户端 ID</span><span class="sxs-lookup"><span data-stu-id="c3982-135">Creating an app/client ID</span></span>
<span data-ttu-id="c3982-136">为了获取客户端 ID，需要在 Azure AD 中 [注册应用程序](../../auth-register-app-v2.md) 。</span><span class="sxs-lookup"><span data-stu-id="c3982-136">In order to get a client ID, you need to [register your application](../../auth-register-app-v2.md) in Azure AD.</span></span> 
><span data-ttu-id="c3982-137">**注意**： MSAL 仅支持 OAuth 的隐式流。</span><span class="sxs-lookup"><span data-stu-id="c3982-137">**Note**: MSAL only supports the Implicit Flow for OAuth.</span></span> <span data-ttu-id="c3982-138">请务必在 Azure 门户中的应用程序中启用隐式流， (默认情况下不启用它) 。</span><span class="sxs-lookup"><span data-stu-id="c3982-138">Make sure to enable Implicit Flow in your application in the Azure Portal (it is not enabled by default).</span></span> <span data-ttu-id="c3982-139">在 " **身份验证**" 下，找到 " **隐式授予** " 部分，然后选择 " **访问令牌** " 和 **ID 令牌**的复选框。</span><span class="sxs-lookup"><span data-stu-id="c3982-139">Under **Authentication**, find the **Implicit grant** section and select the checkboxes for **Access tokens** and **ID tokens**.</span></span> 

## <a name="add-components"></a><span data-ttu-id="c3982-140">添加组件</span><span class="sxs-lookup"><span data-stu-id="c3982-140">Add components</span></span>
<span data-ttu-id="c3982-141">初始化 MSAL 提供程序后，可以开始使用任何工具包组件。</span><span class="sxs-lookup"><span data-stu-id="c3982-141">After you initialize the MSAL provider, you can start using any of the Toolkit components.</span></span>

<span data-ttu-id="c3982-142">以下是使用 MSAL 提供程序的完整工作示例（HTML 中初始化的）和登录组件：</span><span class="sxs-lookup"><span data-stu-id="c3982-142">The following is a full working example using mgt-loader, the MSAL Provider initialized in HTML, and the Login component:</span></span>

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal-provider>
<mgt-login></mgt-login>
```

<span data-ttu-id="c3982-143">以下是使用 ES6 模块、MSAL 提供程序（HTML 中初始化）和登录组件的示例：</span><span class="sxs-lookup"><span data-stu-id="c3982-143">This is an example using the ES6 modules, the MSAL Provider initialized in HTML, and the Login component:</span></span>
```html
<script src="node_modules/@microsoft/mgt/dist/es6/components/providers/mgt-msal-provider.js"></script>
<script src="node_modules/@microsoft/mgt/dist/es6/components/mgt-login/mgt-login.js"></script>
<mgt-msal-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal-provider>
<mgt-login></mgt-login>
```

<span data-ttu-id="c3982-144">以下是使用 ES6 模块、在 JavaScript 中初始化的 MSAL 提供程序和登录组件的示例：</span><span class="sxs-lookup"><span data-stu-id="c3982-144">This is an example using the ES6 modules, the MSAL Provider initialized in JavaScript, and the Login component:</span></span>

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

## <a name="test-your-app"></a><span data-ttu-id="c3982-145">测试应用程序</span><span class="sxs-lookup"><span data-stu-id="c3982-145">Test your app</span></span>

<span data-ttu-id="c3982-146">为了测试您的应用程序，MSAL 要求将页面托管在用于身份验证重定向的 web 服务器中。</span><span class="sxs-lookup"><span data-stu-id="c3982-146">In order to test your app, MSAL requires the page to be hosted in a web server for the authentication redirects.</span></span> 

<span data-ttu-id="c3982-147">如果只是开始并且想要进行播放，可以在 Visual Studio Code 或任何类似的轻型开发服务器中使用 [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) 。</span><span class="sxs-lookup"><span data-stu-id="c3982-147">If you're just getting started and want to play around, you can use [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) in Visual Studio Code or any similar lightweight development server.</span></span> <span data-ttu-id="c3982-148">下载扩展并使用 live server 打开您的 HTML 文件。</span><span class="sxs-lookup"><span data-stu-id="c3982-148">Download the extension and open your HTML file using live server.</span></span> 
> <span data-ttu-id="c3982-149">**注意：** 确保将应用注册中的 **重定向 URI** 设置为承载您的应用程序的 localhost 端口。</span><span class="sxs-lookup"><span data-stu-id="c3982-149">**Note:** Make sure the **redirect URI** in your app registration is set to the localhost port your application is hosted on.</span></span> <span data-ttu-id="c3982-150">转到 [Azure 门户](https://portal.azure.com)中的应用程序注册，在 "管理" 下单击 " **身份验证** "，并添加正确的 **重定向 URI**。</span><span class="sxs-lookup"><span data-stu-id="c3982-150">Go to your app registration in the [Azure portal](https://portal.azure.com), click **Authentication** under manage, and add the correct **redirect URI**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="c3982-151">后续步骤</span><span class="sxs-lookup"><span data-stu-id="c3982-151">Next Steps</span></span>
- <span data-ttu-id="c3982-152">请参阅本分步教程，了解如何 [生成简单的 web 应用程序](https://developer.microsoft.com/microsoft-365/blogs/a-lap-around-microsoft-graph-toolkit-day-2-zero-to-hero/)。</span><span class="sxs-lookup"><span data-stu-id="c3982-152">Check out this step-by-step tutorial on [building a simple web app](https://developer.microsoft.com/microsoft-365/blogs/a-lap-around-microsoft-graph-toolkit-day-2-zero-to-hero/).</span></span>
- <span data-ttu-id="c3982-153">尝试 [样本](https://mgt.dev)中的组件。</span><span class="sxs-lookup"><span data-stu-id="c3982-153">Try out the components in the [playground](https://mgt.dev).</span></span>
- <span data-ttu-id="c3982-154">在 [堆栈溢出](https://aka.ms/mgt-question)时提出问题。</span><span class="sxs-lookup"><span data-stu-id="c3982-154">Ask a question on [Stack Overflow](https://aka.ms/mgt-question).</span></span>
- <span data-ttu-id="c3982-155">在 [GitHub](https://aka.ms/mgt)上报告错误或保留功能请求。</span><span class="sxs-lookup"><span data-stu-id="c3982-155">Report bugs or leave a feature request on [GitHub](https://aka.ms/mgt).</span></span>