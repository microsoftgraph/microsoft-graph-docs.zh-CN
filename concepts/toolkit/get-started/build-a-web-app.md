---
title: 使用 Microsoft 网站生成 web Graph Toolkit
description: 开始使用 Microsoft Graph Toolkit 构建 Web Graph Toolkit。
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: 989e79c2b52f7e02fb61604d3011f13aced580ed
ms.sourcegitcommit: e4461c7eb8c3d265fc1aa766125e81b58c6e1099
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2021
ms.locfileid: "52941534"
---
# <a name="build-a-web-application-with-the-microsoft-graph-toolkit"></a><span data-ttu-id="bb464-103">使用 Microsoft 网站生成 web Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="bb464-103">Build a web application with the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="bb464-104">本主题介绍如何在用 vanilla JavaScript 编写的 Web Graph Toolkit Microsoft 应用程序入门。</span><span class="sxs-lookup"><span data-stu-id="bb464-104">This topic describes how to get started with the Microsoft Graph Toolkit in a web application written in vanilla JavaScript.</span></span> <span data-ttu-id="bb464-105">有关分步教程，请尝试 Microsoft Graph Toolkit[入门。](/learn/modules/msgraph-toolkit-intro/)</span><span class="sxs-lookup"><span data-stu-id="bb464-105">For a step-by-step tutorial, try the [Get started with Microsoft Graph Toolkit module](/learn/modules/msgraph-toolkit-intro/).</span></span> <span data-ttu-id="bb464-106">如果你想要了解如何将 web 应用程序与 web 框架Toolkit，[请参阅生成](./use-toolkit-with-react.md)Web (React) 或 生成[Web ](./use-toolkit-with-angular.md) (Angular) 。</span><span class="sxs-lookup"><span data-stu-id="bb464-106">If you would like to learn how to use the Toolkit with a web framework, see [Build a web app (React)](./use-toolkit-with-react.md) or [Build a web app (Angular)](./use-toolkit-with-angular.md).</span></span>

<span data-ttu-id="bb464-107">Microsoft Graph Toolkit入门包括以下步骤：</span><span class="sxs-lookup"><span data-stu-id="bb464-107">Getting started with the Microsoft Graph Toolkit involves the following steps:</span></span>
1. <span data-ttu-id="bb464-108">将 Microsoft Graph Toolkit添加到你的项目中。</span><span class="sxs-lookup"><span data-stu-id="bb464-108">Add Microsoft Graph Toolkit to your project.</span></span>
2. <span data-ttu-id="bb464-109">初始化 MSAL 2.0 提供程序。</span><span class="sxs-lookup"><span data-stu-id="bb464-109">Initialize the MSAL 2.0 Provider.</span></span>
3. <span data-ttu-id="bb464-110">添加组件。</span><span class="sxs-lookup"><span data-stu-id="bb464-110">Add components.</span></span>
4. <span data-ttu-id="bb464-111">测试应用程序。</span><span class="sxs-lookup"><span data-stu-id="bb464-111">Test your application.</span></span>

## <a name="add-the-microsoft-graph-toolkit-to-your-project"></a><span data-ttu-id="bb464-112">将 Microsoft Graph Toolkit添加到你的项目</span><span class="sxs-lookup"><span data-stu-id="bb464-112">Add the Microsoft Graph Toolkit to your project</span></span>
<span data-ttu-id="bb464-113">可以在应用程序中使用 Microsoft Graph Toolkit，方法为通过 unpkg (直接引用加载程序) 安装 npm 包。</span><span class="sxs-lookup"><span data-stu-id="bb464-113">You can use the Microsoft Graph Toolkit in your application by referencing the loader directly (via unpkg) or by installing the npm package.</span></span>

# <a name="unpkg"></a>[<span data-ttu-id="bb464-114">unpkg</span><span class="sxs-lookup"><span data-stu-id="bb464-114">unpkg</span></span>](#tab/html)
<span data-ttu-id="bb464-115">若要通过 mgt-loader Toolkit脚本，请向代码添加脚本中的引用：</span><span class="sxs-lookup"><span data-stu-id="bb464-115">To use the Toolkit via mgt-loader, add the reference in a script to your code:</span></span>

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
```
# <a name="npm"></a>[<span data-ttu-id="bb464-116">npm</span><span class="sxs-lookup"><span data-stu-id="bb464-116">npm</span></span>](#tab/npm)
<span data-ttu-id="bb464-117">通过 ES6 模块使用 Toolkit 可以完全控制捆绑过程，并允许您仅捆绑应用程序所需的代码。</span><span class="sxs-lookup"><span data-stu-id="bb464-117">Using the Toolkit via ES6 modules will give you full control of the bundling process and allow you to bundle only the code you need for your application.</span></span> <span data-ttu-id="bb464-118">若要使用 ES6 模块，请向项目添加 npm 包：</span><span class="sxs-lookup"><span data-stu-id="bb464-118">To use the ES6 modules, add the npm package to your project:</span></span>

```cmd
npm install @microsoft/mgt
```

---

## <a name="initialize-the-msal-20-provider"></a><span data-ttu-id="bb464-119">初始化 MSAL 2.0 提供程序</span><span class="sxs-lookup"><span data-stu-id="bb464-119">Initialize the MSAL 2.0 Provider</span></span>
<span data-ttu-id="bb464-120">Microsoft Graph Toolkit提供程序支持对组件的 Microsoft Graph进行身份验证和访问。</span><span class="sxs-lookup"><span data-stu-id="bb464-120">The Microsoft Graph Toolkit providers enable authentication and access to Microsoft Graph for the components.</span></span> <span data-ttu-id="bb464-121">若要了解更多信息，请参阅 [使用提供程序](../providers/providers.md)。</span><span class="sxs-lookup"><span data-stu-id="bb464-121">To learn more, see [Using the providers](../providers/providers.md).</span></span> <span data-ttu-id="bb464-122">[MSAL 2.0 提供程序](../providers/msal2.md)使用 msal-browser 登录用户并获取令牌。</span><span class="sxs-lookup"><span data-stu-id="bb464-122">The [MSAL 2.0 Provider](../providers/msal2.md) uses msal-browser to sign in users and acquire tokens.</span></span> <span data-ttu-id="bb464-123">可以在 HTML 或 JavaScript 中初始化此提供程序。</span><span class="sxs-lookup"><span data-stu-id="bb464-123">You can initialize this provider in your HTML or JavaScript.</span></span>

> <span data-ttu-id="bb464-124">**注意**：如果你当前正在使用 MSAL 提供程序，并且要更新到 MSAL 2.0 提供程序，请按照此处列出的 [步骤操作](../providers/msal2.md#migrating-from-msal-provider-to-msal-2-provider)。</span><span class="sxs-lookup"><span data-stu-id="bb464-124">**Note**: If you are currently using MSAL Provider and would like to update to MSAL 2.0 Provider, follow the steps listed [here](../providers/msal2.md#migrating-from-msal-provider-to-msal-2-provider).</span></span>
<span data-ttu-id="bb464-125">如果要使用自己的后端身份验证，请使用代理 [提供程序](../providers/proxy.md) 替代 MSAL 2.0 提供程序。</span><span class="sxs-lookup"><span data-stu-id="bb464-125">If you would like to use your own backend authentication, use the [Proxy Provider](../providers/proxy.md) in place of the MSAL 2.0 provider.</span></span>

<span data-ttu-id="bb464-126">可以选择在 HTML 或 JavaScript 代码中初始化提供程序。</span><span class="sxs-lookup"><span data-stu-id="bb464-126">You can choose to initialize the provider in either your HTML or your JavaScript code.</span></span> 

# <a name="html"></a>[<span data-ttu-id="bb464-127">HTML</span><span class="sxs-lookup"><span data-stu-id="bb464-127">HTML</span></span>](#tab/HTML)
<span data-ttu-id="bb464-128">将 `mgt-msal2-provider` 组件添加到 HTML 页面，将 设置为 `client-id` 应用程序 client-id。</span><span class="sxs-lookup"><span data-stu-id="bb464-128">Add the `mgt-msal2-provider` component to your HTML page and set the `client-id` to your application client-id.</span></span>

```html
<mgt-msal2-provider client-id="<YOUR_CLIENT_ID"></mgt-msal2-provider>
```
# <a name="javascript"></a>[<span data-ttu-id="bb464-129">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bb464-129">JavaScript</span></span>](#tab/JavaScript)
<span data-ttu-id="bb464-130">若要在 JavaScript 中初始化 MSAL 提供程序，请向应用程序添加以下代码：</span><span class="sxs-lookup"><span data-stu-id="bb464-130">To initialize the MSAL provider in your JavaScript, add the following code to your application:</span></span>

```javascript
import {Providers, Msal2Provider} from '@microsoft/mgt'

Providers.globalProvider = new Msal2Provider({
    clientId: "<YOUR_CLIENT_ID>"
})
```

---


<span data-ttu-id="bb464-131">客户端 ID 是初始化提供程序所需的唯一属性，但您可以设置其他选项。</span><span class="sxs-lookup"><span data-stu-id="bb464-131">The client ID is the only property required to initialize the provider, but you can set additional options.</span></span> <span data-ttu-id="bb464-132">有关完整列表，请参阅[Msal 2.0 Provider。](../providers/msal2.md)</span><span class="sxs-lookup"><span data-stu-id="bb464-132">For the full list, see [Msal 2.0 Provider](../providers/msal2.md).</span></span>

### <a name="creating-an-appclient-id"></a><span data-ttu-id="bb464-133">创建应用/客户端 ID</span><span class="sxs-lookup"><span data-stu-id="bb464-133">Creating an app/client ID</span></span>
<span data-ttu-id="bb464-134">若要获取客户端 ID，需要在 Azure AD 中 [注册](./add-aad-app-registration.md) 应用程序。</span><span class="sxs-lookup"><span data-stu-id="bb464-134">In order to get a client ID, you need to [register your application](./add-aad-app-registration.md) in Azure AD.</span></span> 

## <a name="add-components"></a><span data-ttu-id="bb464-135">添加组件</span><span class="sxs-lookup"><span data-stu-id="bb464-135">Add components</span></span>
<span data-ttu-id="bb464-136">初始化 MSAL 2.0 提供程序后，就可以开始使用任何Toolkit组件。</span><span class="sxs-lookup"><span data-stu-id="bb464-136">After you initialize the MSAL 2.0 provider, you can start using any of the Toolkit components.</span></span>

# <a name="html"></a>[<span data-ttu-id="bb464-137">HTML</span><span class="sxs-lookup"><span data-stu-id="bb464-137">HTML</span></span>](#tab/HTML)
<span data-ttu-id="bb464-138">下面是使用 mgt-loader 的完整工作示例、HTML 中初始化的 MSAL 提供程序和登录组件：</span><span class="sxs-lookup"><span data-stu-id="bb464-138">The following is a full working example using mgt-loader, the MSAL Provider initialized in HTML, and the Login component:</span></span>

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal2-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal2-provider>
<mgt-login></mgt-login>
```

<span data-ttu-id="bb464-139">这是使用 ES6 模块、HTML 中初始化的 MSAL 2.0 提供程序和登录组件的示例：</span><span class="sxs-lookup"><span data-stu-id="bb464-139">This is an example using the ES6 modules, the MSAL 2.0 Provider initialized in HTML, and the Login component:</span></span>

```html
<script type="module" src="node_modules/@microsoft/mgt/dist/es6/index.js"></script>

<mgt-msal2-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal2-provider>

<mgt-login></mgt-login>
```
# <a name="javascript"></a>[<span data-ttu-id="bb464-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bb464-140">JavaScript</span></span>](#tab/JavaScript)
<span data-ttu-id="bb464-141">这是使用 ES6 模块、在 JavaScript 中初始化的 MSAL 2.0 提供程序和登录组件的示例：</span><span class="sxs-lookup"><span data-stu-id="bb464-141">This is an example using the ES6 modules, the MSAL 2.0 Provider initialized in JavaScript, and the Login component:</span></span>

```javascript
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


## <a name="test-your-app"></a><span data-ttu-id="bb464-142">测试应用</span><span class="sxs-lookup"><span data-stu-id="bb464-142">Test your app</span></span>

<span data-ttu-id="bb464-143">为了测试你的应用，MSAL 要求将页面托管在 Web 服务器中，以便进行身份验证重定向。</span><span class="sxs-lookup"><span data-stu-id="bb464-143">In order to test your app, MSAL requires the page to be hosted in a web server for the authentication redirects.</span></span> 

<span data-ttu-id="bb464-144">如果你刚开始工作并且想要玩游戏，可以在 Visual Studio Code或任何类似的轻型开发服务器中使用[Live](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) Server。</span><span class="sxs-lookup"><span data-stu-id="bb464-144">If you're just getting started and want to play around, you can use [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) in Visual Studio Code or any similar lightweight development server.</span></span> <span data-ttu-id="bb464-145">下载扩展名，然后使用实时服务器打开 HTML 文件。</span><span class="sxs-lookup"><span data-stu-id="bb464-145">Download the extension and open your HTML file using live server.</span></span> 
> <span data-ttu-id="bb464-146">**注意：** 确保应用 **注册中的重定向 URI** 设置为托管应用程序的 localhost 端口。</span><span class="sxs-lookup"><span data-stu-id="bb464-146">**Note:** Make sure the **redirect URI** in your app registration is set to the localhost port your application is hosted on.</span></span> <span data-ttu-id="bb464-147">转到 Azure 门户中的应用注册 [，](https://portal.azure.com)单击"管理"下的"身份验证"，然后添加正确的 **重定向 URI。**</span><span class="sxs-lookup"><span data-stu-id="bb464-147">Go to your app registration in the [Azure portal](https://portal.azure.com), click **Authentication** under manage, and add the correct **redirect URI**.</span></span>

## <a name="track-a-users-sign-in-state"></a><span data-ttu-id="bb464-148">跟踪用户的登录状态</span><span class="sxs-lookup"><span data-stu-id="bb464-148">Track a user's sign in state</span></span>

<span data-ttu-id="bb464-149">你可以检测用户何时成功登录，并相应地显示特定组件。</span><span class="sxs-lookup"><span data-stu-id="bb464-149">You can detect when a user has successfully signed in and display specific components accordingly.</span></span> <span data-ttu-id="bb464-150">例如，如果用户已登录，则显示议程组件。</span><span class="sxs-lookup"><span data-stu-id="bb464-150">For example, display the agenda component if the user has signed in.</span></span> <span data-ttu-id="bb464-151">否则，显示登录界面。</span><span class="sxs-lookup"><span data-stu-id="bb464-151">Otherwise, display the sign in interface.</span></span>

<span data-ttu-id="bb464-152">可以通过计算 和 来确定用户是否 `globalProvider` 登录 `providerState` 。</span><span class="sxs-lookup"><span data-stu-id="bb464-152">You can determine if a user is signed in by evaluating the `globalProvider` and `providerState`.</span></span>

# <a name="html"></a>[<span data-ttu-id="bb464-153">HTML</span><span class="sxs-lookup"><span data-stu-id="bb464-153">HTML</span></span>](#tab/HTML)

<span data-ttu-id="bb464-154">如果使用的是 库 `mgt-loader` ，可以从 属性访问 和 `provider` `providerState` `mgt` 。</span><span class="sxs-lookup"><span data-stu-id="bb464-154">If you're using the `mgt-loader` library, you can access the `provider` and `providerState` from the `mgt` property.</span></span>

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>

<mgt-msal-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal-provider>

<div id="main"><mgt-login></mgt-login></div>

<script>
    const provider = mgt.Providers.globalProvider;
    const isLoggedIn = provider && provider.state === mgt.ProviderState.SignedIn

    // Show the mgt-agenda component ONLY if the user is logged in, show the mgt-login component if not
    function loadAgenda(){
        if(isLoggedIn){
            const main = document.getElementById("main");
            main.innerHTML = `<mgt-agenda></mgt-agenda>`;
        } else {
            main.innerHTML = `<mgt-login></mgt-login>`;
        }
    }

    loadAgenda();
</script>
```

# <a name="javascript"></a>[<span data-ttu-id="bb464-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bb464-155">JavaScript</span></span>](#tab/JavaScript)
<span data-ttu-id="bb464-156">如果你通过 npm Toolkit，可以从 `provider` 导入 和 `providerState` `@microsoft/mgt` 。</span><span class="sxs-lookup"><span data-stu-id="bb464-156">If you're using the Toolkit via the npm packages, you can import the `provider` and `providerState` from `@microsoft/mgt`.</span></span>

```javascript
import {Providers, ProviderState} from '@microsoft/mgt'

Providers.globalProvider = new MsalProvider({
    clientId: "<YOUR_CLIENT_ID>"
})

function isLoggedIn(){
    const provider = Providers.globalProvider;
    return provider && provider.state === ProviderState.SignedIn;
}

function loadAgenda(){
    const agenda = document.createElement("mgt-agenda");
    const loginComponent = document.createElement("mgt-login");
    if(isLoggedIn()){
        // the user is logged in, load their agenda
        document.body.innerHTML = `<mgt-agenda></mgt-agenda>`;
    } else {
        // the user is not logged in, show them the login component
        document.body.innerHTML = `<mgt-login></mgt-login>`
    }
}

loadAgenda();
```

---


## <a name="next-steps"></a><span data-ttu-id="bb464-157">后续步骤</span><span class="sxs-lookup"><span data-stu-id="bb464-157">Next Steps</span></span>
- <span data-ttu-id="bb464-158">请查看 Microsoft [Graph Toolkit](/learn/modules/msgraph-toolkit-intro/)入门教程。</span><span class="sxs-lookup"><span data-stu-id="bb464-158">Check out the [Get started with Microsoft Graph Toolkit](/learn/modules/msgraph-toolkit-intro/) step-by-step tutorial.</span></span>
- <span data-ttu-id="bb464-159">尝试在运动场中的 [组件](https://mgt.dev)。</span><span class="sxs-lookup"><span data-stu-id="bb464-159">Try out the components in the [playground](https://mgt.dev).</span></span>
- <span data-ttu-id="bb464-160">在 Stack [Overflow 上提问](https://aka.ms/mgt-question)。</span><span class="sxs-lookup"><span data-stu-id="bb464-160">Ask a question on [Stack Overflow](https://aka.ms/mgt-question).</span></span>
- <span data-ttu-id="bb464-161">报告 Bug 或将功能请求[保留GitHub。](https://aka.ms/mgt)</span><span class="sxs-lookup"><span data-stu-id="bb464-161">Report bugs or leave a feature request on [GitHub](https://aka.ms/mgt).</span></span>
