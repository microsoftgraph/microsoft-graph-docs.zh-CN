---
title: 使用 Microsoft Graph 工具生成 Microsoft Teams Toolkit
description: 开始使用 Microsoft Graph 工具生成 Microsoft Teams Toolkit。
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: 915bbe562fec9ef0bcbd5ae6d67d8497ea7e72eb
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50963272"
---
# <a name="build-a-microsoft-teams-tab-with-the-microsoft-graph-toolkit"></a><span data-ttu-id="cbcdd-103">使用 Microsoft Graph 工具生成 Microsoft Teams Toolkit</span><span class="sxs-lookup"><span data-stu-id="cbcdd-103">Build a Microsoft Teams tab with the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="cbcdd-104">本主题介绍如何开始在 Microsoft Teams 解决方案Toolkit Microsoft Graph 应用。</span><span class="sxs-lookup"><span data-stu-id="cbcdd-104">This topic covers how to get started using the Microsoft Graph Toolkit in a Microsoft Teams solution.</span></span> <span data-ttu-id="cbcdd-105">入门包括以下步骤：</span><span class="sxs-lookup"><span data-stu-id="cbcdd-105">Getting started involves the following steps:</span></span>

1. <span data-ttu-id="cbcdd-106">使用自定义选项卡创建新的 Teams 应用程序。</span><span class="sxs-lookup"><span data-stu-id="cbcdd-106">Create a new Teams application with a custom tab.</span></span>
2. <span data-ttu-id="cbcdd-107">添加 Microsoft Graph Toolkit。</span><span class="sxs-lookup"><span data-stu-id="cbcdd-107">Add the Microsoft Graph Toolkit.</span></span>
3. <span data-ttu-id="cbcdd-108">初始化 Microsoft Teams 提供程序。</span><span class="sxs-lookup"><span data-stu-id="cbcdd-108">Initialize the Microsoft Teams provider.</span></span>
4. <span data-ttu-id="cbcdd-109">创建身份验证弹出窗口页面。</span><span class="sxs-lookup"><span data-stu-id="cbcdd-109">Create the auth popup page.</span></span>
5. <span data-ttu-id="cbcdd-110">添加组件。</span><span class="sxs-lookup"><span data-stu-id="cbcdd-110">Add components.</span></span>
6. <span data-ttu-id="cbcdd-111">测试你的应用。</span><span class="sxs-lookup"><span data-stu-id="cbcdd-111">Test your app.</span></span>

## <a name="create-a-new-teams-application-with-a-custom-tab"></a><span data-ttu-id="cbcdd-112">使用自定义选项卡创建新的 Teams 应用程序</span><span class="sxs-lookup"><span data-stu-id="cbcdd-112">Create a new Teams application with a custom tab</span></span>

<span data-ttu-id="cbcdd-113">创建新 Teams 应用的最简单方法是使用 [Microsoft Teams](https://marketplace.visualstudio.com/items?itemName=TeamsDevApp.ms-teams-vscode-extension) Toolkit扩展进行Visual Studio代码。</span><span class="sxs-lookup"><span data-stu-id="cbcdd-113">The easiest way to create a new Teams app is to use the [Microsoft Teams Toolkit extension](https://marketplace.visualstudio.com/items?itemName=TeamsDevApp.ms-teams-vscode-extension) for Visual Studio Code.</span></span> <span data-ttu-id="cbcdd-114">按照说明 [设置新的 Teams 项目](/microsoftteams/platform/toolkit/visual-studio-code-overview#set-up-a-new-teams-project)。</span><span class="sxs-lookup"><span data-stu-id="cbcdd-114">Follow the instructions to [set up a new Teams project](/microsoftteams/platform/toolkit/visual-studio-code-overview#set-up-a-new-teams-project).</span></span> <span data-ttu-id="cbcdd-115">When you get to the **Add capabilities** screen， select **Tab**， and then **Personal tab**.</span><span class="sxs-lookup"><span data-stu-id="cbcdd-115">When you get to the **Add capabilities** screen, select **Tab**, and then **Personal tab**.</span></span>

## <a name="add-the-microsoft-graph-toolkit"></a><span data-ttu-id="cbcdd-116">添加 Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="cbcdd-116">Add the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="cbcdd-117">可以在应用程序中使用 Microsoft Graph Toolkit，方法为通过 unpkg (直接引用加载程序) 安装 npm 包。</span><span class="sxs-lookup"><span data-stu-id="cbcdd-117">You can use the Microsoft Graph Toolkit in your application by referencing the loader directly (via unpkg) or by installing the npm package.</span></span> <span data-ttu-id="cbcdd-118">若要使用Toolkit，你还需要 [Microsoft Teams SDK](/javascript/api/overview/msteams-client?view=msteams-client-js-latest)。</span><span class="sxs-lookup"><span data-stu-id="cbcdd-118">To use the Toolkit, you will also need the [Microsoft Teams SDK](/javascript/api/overview/msteams-client?view=msteams-client-js-latest).</span></span>

### <a name="use-via-mgt-loader"></a><span data-ttu-id="cbcdd-119">通过 mgt-loader 使用</span><span class="sxs-lookup"><span data-stu-id="cbcdd-119">Use via mgt-loader</span></span>
<span data-ttu-id="cbcdd-120">若要通过Toolkit使用 Toolkit 和 Teams SDK，在 文件中添加以下 `<head>` `public/index.html` 引用：</span><span class="sxs-lookup"><span data-stu-id="cbcdd-120">To use the Toolkit and the Teams SDK via the loaders, add the following references inside the `<head>` of the `public/index.html` file:</span></span>

```html
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
```

### <a name="use-via-npm-es6-modules"></a><span data-ttu-id="cbcdd-121">通过 npm (ES6 模块) </span><span class="sxs-lookup"><span data-stu-id="cbcdd-121">Use via npm (ES6 modules)</span></span>
<span data-ttu-id="cbcdd-122">通过 ES6 模块Toolkit可完全控制捆绑过程，并允许您仅捆绑应用程序所需的代码。</span><span class="sxs-lookup"><span data-stu-id="cbcdd-122">Using the Toolkit via ES6 modules will give you full control of the bundling process and allow you to bundle only the code you need for your application.</span></span> <span data-ttu-id="cbcdd-123">若要使用 ES6 模块，请为项目添加 Toolkit 和 Microsoft Teams SDK 的 npm 包：</span><span class="sxs-lookup"><span data-stu-id="cbcdd-123">To use the ES6 modules, add the npm packages for both the Toolkit and the Microsoft Teams SDK to your project:</span></span>

```bash
npm install @microsoft/mgt @microsoft/teams-js
```

## <a name="initialize-the-teams-provider"></a><span data-ttu-id="cbcdd-124">初始化 Teams 提供商</span><span class="sxs-lookup"><span data-stu-id="cbcdd-124">Initialize the Teams provider</span></span>

<span data-ttu-id="cbcdd-125">Microsoft Graph Toolkit提供程序支持对组件的 Microsoft Graph 进行身份验证和访问。</span><span class="sxs-lookup"><span data-stu-id="cbcdd-125">The Microsoft Graph Toolkit providers enable authentication and access to Microsoft Graph for the components.</span></span> <span data-ttu-id="cbcdd-126">若要了解更多信息，请参阅 [使用提供程序](../providers/providers.md)。</span><span class="sxs-lookup"><span data-stu-id="cbcdd-126">To learn more, see [Using the providers](../providers/providers.md).</span></span> <span data-ttu-id="cbcdd-127">[Teams 提供程序](../providers/teams.md)处理所有需要通过 Teams SDK 实现以对用户进行身份验证的逻辑和交互。</span><span class="sxs-lookup"><span data-stu-id="cbcdd-127">The [Teams provider](../providers/teams.md) handles all of the logic and interactions that need to be implemented with the Teams SDK to authenticate the user.</span></span>

<span data-ttu-id="cbcdd-128">可以选择在 HTML 或 JavaScript 代码中初始化提供程序。</span><span class="sxs-lookup"><span data-stu-id="cbcdd-128">You can choose to initialize the provider in either your HTML or your JavaScript code.</span></span> 

### <a name="initialize-in-html"></a><span data-ttu-id="cbcdd-129">在 HTML 中初始化</span><span class="sxs-lookup"><span data-stu-id="cbcdd-129">Initialize in HTML</span></span>

<span data-ttu-id="cbcdd-130">在 `public/index.html` 中，将 Teams 提供商添加到 `<body>` 中，如下所示。</span><span class="sxs-lookup"><span data-stu-id="cbcdd-130">In `public/index.html`, add the Teams provider into the `<body>`, as shown.</span></span>

```html
<mgt-teams-provider
  client-id="<YOUR_CLIENT_ID>"
  auth-popup-url="/auth.html"
></mgt-teams-provider>
```

<span data-ttu-id="cbcdd-131">将 `<YOUR_CLIENT_ID>` 替换为应用程序的客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="cbcdd-131">Replace `<YOUR_CLIENT_ID>` with the client ID for your application.</span></span> 

### <a name="initialize-in-javascript"></a><span data-ttu-id="cbcdd-132">在 JavaScript 中初始化</span><span class="sxs-lookup"><span data-stu-id="cbcdd-132">Initialize in JavaScript</span></span>

<span data-ttu-id="cbcdd-133">若要在 JavaScript 代码中初始化提供程序，请在 `src/components/App.js` 项目目录中找到文件。</span><span class="sxs-lookup"><span data-stu-id="cbcdd-133">To initialize the provider in your JavaScript code, Locate the `src/components/App.js` file in your project directory.</span></span> <span data-ttu-id="cbcdd-134">导入 Teams 提供商并初始化提供商。</span><span class="sxs-lookup"><span data-stu-id="cbcdd-134">Import the Teams Provider and initialize the provider.</span></span>

```js
import * as microsoftTeams from "@microsoft/teams-js";
import { Providers, TeamsProvider } from '@microsoft/mgt';

TeamsProvider.microsoftTeamsLib = microsoftTeams;
Providers.globalProvider = new TeamsProvider ({
    clientId: '<YOUR_CLIENT_ID>',
    authPopupUrl: '/auth.html'
})
```
<span data-ttu-id="cbcdd-135">将 `<YOUR_CLIENT_ID>` 替换为应用程序的客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="cbcdd-135">Replace `<YOUR_CLIENT_ID>` with the client ID for your application.</span></span>

### <a name="creating-an-appclient-id"></a><span data-ttu-id="cbcdd-136">创建应用/客户端 ID</span><span class="sxs-lookup"><span data-stu-id="cbcdd-136">Creating an app/client ID</span></span>

<span data-ttu-id="cbcdd-137">若要获取客户端 ID，需要注册 Azure Active Directory 应用程序。</span><span class="sxs-lookup"><span data-stu-id="cbcdd-137">To get a client ID, you need to register an Azure Active Directory application.</span></span> <span data-ttu-id="cbcdd-138">按照创建 Azure [Active Directory 应用文章中的步骤](./add-aad-app-registration.md) 操作。</span><span class="sxs-lookup"><span data-stu-id="cbcdd-138">Follow the steps in the [Create an Azure Active Directory app](./add-aad-app-registration.md) article.</span></span>

<span data-ttu-id="cbcdd-139">请确保在应用注册中将重定向 **URI** 设置为指向 `auth.html` 你的页面。</span><span class="sxs-lookup"><span data-stu-id="cbcdd-139">Make sure to set the **redirect URI** in your app registration to point to your `auth.html` page.</span></span> <span data-ttu-id="cbcdd-140">例如，如果你正在 上运行你的应用， `localhost:3000` 将重定向 URI 设置为 `https://localhost:3000/auth.html` 。</span><span class="sxs-lookup"><span data-stu-id="cbcdd-140">For example, if you are running your app on `localhost:3000`, set the redirect URI to `https://localhost:3000/auth.html`.</span></span>

><span data-ttu-id="cbcdd-141">**注意**：MSAL 仅支持 OAuth 的隐式流。</span><span class="sxs-lookup"><span data-stu-id="cbcdd-141">**Note**: MSAL only supports the Implicit Flow for OAuth.</span></span> <span data-ttu-id="cbcdd-142">请确保在 Azure 门户应用程序中启用隐式流 (默认情况下不会启用它) 。</span><span class="sxs-lookup"><span data-stu-id="cbcdd-142">Make sure to enable Implicit Flow in your application in the Azure Portal (it is not enabled by default).</span></span> <span data-ttu-id="cbcdd-143">在 **身份验证** 下，找到 **隐式授予** 部分，并选中 **访问** 令牌和 **ID 令牌的复选框**。</span><span class="sxs-lookup"><span data-stu-id="cbcdd-143">Under **Authentication**, find the **Implicit grant** section and select the checkboxes for **Access tokens** and **ID tokens**.</span></span> 

## <a name="create-the-auth-popup-page"></a><span data-ttu-id="cbcdd-144">创建身份验证弹出页</span><span class="sxs-lookup"><span data-stu-id="cbcdd-144">Create the auth popup page</span></span>

<span data-ttu-id="cbcdd-145">为了允许用户登录，你需要提供 Teams 应用将在弹出窗口中打开的 URL，以遵循身份验证流程。</span><span class="sxs-lookup"><span data-stu-id="cbcdd-145">In order to allow users to sign in, you need to provide a URL that the Teams app will open in a popup to follow the authentication flow.</span></span> <span data-ttu-id="cbcdd-146">URL 需要位于域中，此页面需要执行的所有操作就是调用 `TeamsProvider.handleAuth()` 方法。</span><span class="sxs-lookup"><span data-stu-id="cbcdd-146">The URL needs to be in your domain, and all this page needs to do is call the `TeamsProvider.handleAuth()` method.</span></span>

<span data-ttu-id="cbcdd-147">为此，可以在文件夹中添加一个新文件 (该文件应处于与) 相同的级别，并 `auth.html` `public` `index.html` 添加以下代码：</span><span class="sxs-lookup"><span data-stu-id="cbcdd-147">You can do this by adding a new `auth.html` file in the `public` folder (which should be at the same level as `index.html`) and adding the following code:</span></span> 

```html
<!DOCTYPE html>
<html>
  <head>
    <script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
    <script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
  </head>

  <body>
    <script>
      mgt.TeamsProvider.handleAuth();
    </script>
  </body>
</html>
```

## <a name="add-components"></a><span data-ttu-id="cbcdd-148">添加组件</span><span class="sxs-lookup"><span data-stu-id="cbcdd-148">Add components</span></span>

<span data-ttu-id="cbcdd-149">现在，你已准备好将任何 Microsoft Graph Toolkit组件添加到你的选项卡。</span><span class="sxs-lookup"><span data-stu-id="cbcdd-149">Now, you're ready to add any of the Microsoft Graph Toolkit components to your tab.</span></span> 

<span data-ttu-id="cbcdd-150">您可以像平常一样向 HTML 添加组件。</span><span class="sxs-lookup"><span data-stu-id="cbcdd-150">You can add components to your HTML as you normally would.</span></span> <span data-ttu-id="cbcdd-151">例如，若要添加 Login 组件，将以下代码添加到 的正文 `index.html` 中：</span><span class="sxs-lookup"><span data-stu-id="cbcdd-151">For example, to add the Login component add the below code to the body of your `index.html`:</span></span>

```html
<mgt-login></mgt-login>
```

<span data-ttu-id="cbcdd-152">或者，可以将 JSX 中的组件添加到选项卡组件。</span><span class="sxs-lookup"><span data-stu-id="cbcdd-152">Or, you can add the components in JSX to the Tab component.</span></span> <span data-ttu-id="cbcdd-153">如果你使用 Microsoft Teams 应用扩展创建了 Teams 应用，我们建议 `mgt-react` Toolkit库。</span><span class="sxs-lookup"><span data-stu-id="cbcdd-153">We recommend using the `mgt-react` library if you created your Teams app using the Microsoft Teams Toolkit extension.</span></span> <span data-ttu-id="cbcdd-154">若要了解更多信息，请参阅 [将 Microsoft Graph Toolkit React](./use-toolkit-with-react.md)</span><span class="sxs-lookup"><span data-stu-id="cbcdd-154">To learn more, see [Using Microsoft Graph Toolkit with React](./use-toolkit-with-react.md)</span></span>

<span data-ttu-id="cbcdd-155">首先，安装 `mgt-react` ：</span><span class="sxs-lookup"><span data-stu-id="cbcdd-155">First, install `mgt-react`:</span></span>

```bash
npm install @microsoft/mgt-react
```

<span data-ttu-id="cbcdd-156">找到 `src/components/Tab.js` 文件，然后从库导入想要使用 `mgt-react` 的组件。</span><span class="sxs-lookup"><span data-stu-id="cbcdd-156">Locate the `src/components/Tab.js` file and import the components you want to use from the `mgt-react` library.</span></span> <span data-ttu-id="cbcdd-157">例如，若要添加 `Login` 组件，请使用：</span><span class="sxs-lookup"><span data-stu-id="cbcdd-157">For example, to add the `Login` component use:</span></span>

```js
import { Login } from "@microsoft/mgt-react"
```

<span data-ttu-id="cbcdd-158">然后，将组件添加到 方法的 `return()` `render()` 语句 `Tab` 中：</span><span class="sxs-lookup"><span data-stu-id="cbcdd-158">Then, add the the component to the `return()` statement of the `render()` method of `Tab`:</span></span>

```jsx
render() {
  return(
    <Login />
  );
}
```

## <a name="test-your-application"></a><span data-ttu-id="cbcdd-159">测试应用程序</span><span class="sxs-lookup"><span data-stu-id="cbcdd-159">Test your application</span></span>

<span data-ttu-id="cbcdd-160">使用下列命令生成并运行应用程序：</span><span class="sxs-lookup"><span data-stu-id="cbcdd-160">Build and run your application using the following commands:</span></span>
```bash
npm install
npm start
```

<span data-ttu-id="cbcdd-161">若要测试应用程序，可以通过 Teams Toolkit 扩展将应用安装到 Teams。</span><span class="sxs-lookup"><span data-stu-id="cbcdd-161">To test your application, you can install your app to Teams via the Teams Toolkit Extension.</span></span> <span data-ttu-id="cbcdd-162">打开 Teams Toolkit 扩展，然后单击 **"打开 Microsoft Teams Toolkit"。**</span><span class="sxs-lookup"><span data-stu-id="cbcdd-162">Open the Teams Toolkit Extension and click **Open Microsoft Teams Toolkit**.</span></span> <span data-ttu-id="cbcdd-163">单击 **左侧菜单中的 App Studio，** 向下滚动并选择测试和 **分发，然后\*\*\*\*安装**。</span><span class="sxs-lookup"><span data-stu-id="cbcdd-163">Click **App Studio** in the left menu, scroll down and select **Test and Distribute**, then **Install**.</span></span> <span data-ttu-id="cbcdd-164">Teams 将在浏览器中打开，并且你将被重定向到你创建的选项卡。</span><span class="sxs-lookup"><span data-stu-id="cbcdd-164">Teams will open in your browser, and you will be redirected to the tab you created.</span></span> <span data-ttu-id="cbcdd-165">你应该能够看到登录组件，并使用它登录到你的应用程序。</span><span class="sxs-lookup"><span data-stu-id="cbcdd-165">You should be able to see the Login component and use it to sign in to your application.</span></span>

## <a name="next-steps"></a><span data-ttu-id="cbcdd-166">后续步骤</span><span class="sxs-lookup"><span data-stu-id="cbcdd-166">Next Steps</span></span>
- <span data-ttu-id="cbcdd-167">请查看此有关生成 Teams 选项卡 [的分步教程](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-10-microsoft-graph-toolkit-teams-provider/)。</span><span class="sxs-lookup"><span data-stu-id="cbcdd-167">Check out this step-by-step tutorial on [building a Teams tab](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-10-microsoft-graph-toolkit-teams-provider/).</span></span>
- <span data-ttu-id="cbcdd-168">尝试在运动场中的 [组件](https://mgt.dev)。</span><span class="sxs-lookup"><span data-stu-id="cbcdd-168">Try out the components in the [playground](https://mgt.dev).</span></span>
- <span data-ttu-id="cbcdd-169">在 Stack [Overflow 上提问](https://aka.ms/mgt-question)。</span><span class="sxs-lookup"><span data-stu-id="cbcdd-169">Ask a question on [Stack Overflow](https://aka.ms/mgt-question).</span></span>
- <span data-ttu-id="cbcdd-170">在 GitHub 上报告 Bug 或保留 [功能请求](https://aka.ms/mgt)。</span><span class="sxs-lookup"><span data-stu-id="cbcdd-170">Report bugs or leave a feature request on [GitHub](https://aka.ms/mgt).</span></span>
