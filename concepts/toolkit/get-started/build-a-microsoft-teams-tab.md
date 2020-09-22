---
title: 使用 Microsoft Graph 工具包生成 Microsoft 团队选项卡
description: 开始使用 Microsoft Graph 工具包生成 Microsoft 团队选项卡。
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: e987d7030982901903789666f8eb3f0da5f4a093
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48059649"
---
# <a name="build-a-microsoft-teams-tab-with-the-microsoft-graph-toolkit"></a><span data-ttu-id="2d973-103">使用 Microsoft Graph 工具包生成 Microsoft 团队选项卡</span><span class="sxs-lookup"><span data-stu-id="2d973-103">Build a Microsoft Teams tab with the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="2d973-104">本主题介绍如何在 Microsoft 团队解决方案中开始使用 Microsoft Graph 工具包。</span><span class="sxs-lookup"><span data-stu-id="2d973-104">This topic covers how to get started using the Microsoft Graph Toolkit in a Microsoft Teams solution.</span></span> <span data-ttu-id="2d973-105">入门涉及以下步骤：</span><span class="sxs-lookup"><span data-stu-id="2d973-105">Getting started involves the following steps:</span></span>

1. <span data-ttu-id="2d973-106">使用自定义选项卡创建新的团队应用程序。</span><span class="sxs-lookup"><span data-stu-id="2d973-106">Create a new Teams application with a custom tab.</span></span>
2. <span data-ttu-id="2d973-107">设置 ngrok 并创建隧道。</span><span class="sxs-lookup"><span data-stu-id="2d973-107">Set up ngrok and create a tunnel.</span></span>
3. <span data-ttu-id="2d973-108">添加 Microsoft Graph 工具包。</span><span class="sxs-lookup"><span data-stu-id="2d973-108">Add the Microsoft Graph Toolkit.</span></span>
4. <span data-ttu-id="2d973-109">初始化 Microsoft 团队提供程序。</span><span class="sxs-lookup"><span data-stu-id="2d973-109">Initialize the Microsoft Teams provider.</span></span>
5. <span data-ttu-id="2d973-110">创建身份验证弹出页面。</span><span class="sxs-lookup"><span data-stu-id="2d973-110">Create the auth popup page.</span></span>
6. <span data-ttu-id="2d973-111">添加组件。</span><span class="sxs-lookup"><span data-stu-id="2d973-111">Add components.</span></span>
7. <span data-ttu-id="2d973-112">测试您的应用程序。</span><span class="sxs-lookup"><span data-stu-id="2d973-112">Test your app.</span></span>

## <a name="create-a-new-teams-application-with-a-custom-tab"></a><span data-ttu-id="2d973-113">使用自定义选项卡创建新的团队应用程序</span><span class="sxs-lookup"><span data-stu-id="2d973-113">Create a new Teams application with a custom tab</span></span>

<span data-ttu-id="2d973-114">创建新的团队应用程序最简单的方法是将 [Microsoft 团队工具包扩展](https://marketplace.visualstudio.com/items?itemName=TeamsDevApp.ms-teams-vscode-extension) 用于 Visual Studio Code。</span><span class="sxs-lookup"><span data-stu-id="2d973-114">The easiest way to create a new Teams app is to use the [Microsoft Teams Toolkit extension](https://marketplace.visualstudio.com/items?itemName=TeamsDevApp.ms-teams-vscode-extension) for Visual Studio Code.</span></span> <span data-ttu-id="2d973-115">按照说明 [设置新的团队项目](https://docs.microsoft.com/microsoftteams/platform/toolkit/visual-studio-code-overview#set-up-a-new-teams-project)。</span><span class="sxs-lookup"><span data-stu-id="2d973-115">Follow the instructions to [set up a new Teams project](https://docs.microsoft.com/microsoftteams/platform/toolkit/visual-studio-code-overview#set-up-a-new-teams-project).</span></span> <span data-ttu-id="2d973-116">进入 " **添加功能** " 屏幕时，依次选择 " **选项卡**" 和 " **个人" 选项卡**。</span><span class="sxs-lookup"><span data-stu-id="2d973-116">When you get to the **Add capabilities** screen, select **Tab**, and then **Personal tab**.</span></span>

## <a name="set-up-ngrok-and-create-a-tunnel"></a><span data-ttu-id="2d973-117">设置 ngrok 并创建隧道</span><span class="sxs-lookup"><span data-stu-id="2d973-117">Set up ngrok and create a tunnel</span></span>

<span data-ttu-id="2d973-118">为了稍后测试您的应用程序，您需要使用 HTTPS 以面向公众的 URL 托管应用程序。</span><span class="sxs-lookup"><span data-stu-id="2d973-118">In order to test your application later, you will need to host your application over a public-facing URL using HTTPS.</span></span> <span data-ttu-id="2d973-119">使用以下命令安装 [ngrok](https://ngrok.com/download) 并创建从 Internet 到 localhost：3000的隧道：</span><span class="sxs-lookup"><span data-stu-id="2d973-119">Install [ngrok](https://ngrok.com/download) and create a tunnel from the Internet to localhost:3000 with the following command:</span></span>

```bash
ngrok http 3000
```
<span data-ttu-id="2d973-120">在项目目录中，找到 `.publish\Development.env` 文件并将值替换为 `baseUrl0` 您的 ngrok URL。</span><span class="sxs-lookup"><span data-stu-id="2d973-120">In your project directory, locate the `.publish\Development.env` file and replace the value for `baseUrl0` with your ngrok URL.</span></span>

## <a name="add-the-microsoft-graph-toolkit"></a><span data-ttu-id="2d973-121">添加 Microsoft Graph 工具包</span><span class="sxs-lookup"><span data-stu-id="2d973-121">Add the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="2d973-122">您可以在应用程序中使用 Microsoft Graph 工具包，方法是通过 unpkg) 或安装 npm 程序包直接 (引用加载程序。</span><span class="sxs-lookup"><span data-stu-id="2d973-122">You can use the Microsoft Graph Toolkit in your application by referencing the loader directly (via unpkg) or by installing the npm package.</span></span> <span data-ttu-id="2d973-123">若要使用此工具包，你还需要 [Microsoft 团队 SDK](https://docs.microsoft.com/javascript/api/overview/msteams-client?view=msteams-client-js-latest)。</span><span class="sxs-lookup"><span data-stu-id="2d973-123">To use the Toolkit, you will also need the [Microsoft Teams SDK](https://docs.microsoft.com/javascript/api/overview/msteams-client?view=msteams-client-js-latest).</span></span>

### <a name="use-via-mgt-loader"></a><span data-ttu-id="2d973-124">通过预加载加载程序使用</span><span class="sxs-lookup"><span data-stu-id="2d973-124">Use via mgt-loader</span></span>
<span data-ttu-id="2d973-125">若要通过加载程序使用工具包和团队 SDK，请将以下引用添加到 `public/index.html` ：</span><span class="sxs-lookup"><span data-stu-id="2d973-125">To use the Toolkit and the Teams SDK via the loaders, add the following references to `public/index.html`:</span></span>

```html
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
```

### <a name="use-via-npm-es6-modules"></a><span data-ttu-id="2d973-126">通过 npm (ES6 模块使用) </span><span class="sxs-lookup"><span data-stu-id="2d973-126">Use via npm (ES6 modules)</span></span>
<span data-ttu-id="2d973-127">通过使用 ES6 模块中的工具包，可以完全控制捆绑过程，并允许您只捆绑应用程序所需的代码。</span><span class="sxs-lookup"><span data-stu-id="2d973-127">Using the Toolkit via ES6 modules will give you full control of the bundling process and allow you to bundle only the code you need for your application.</span></span> <span data-ttu-id="2d973-128">若要使用 ES6 模块，请将工具包和 Microsoft 团队 SDK 的 npm 包添加到项目中：</span><span class="sxs-lookup"><span data-stu-id="2d973-128">To use the ES6 modules, add the npm packages for both the Toolkit and the Microsoft Teams SDK to your project:</span></span>

```bash
npm install @microsoft/mgt @microsoft/teams-js
```

## <a name="initialize-the-teams-provider"></a><span data-ttu-id="2d973-129">初始化团队提供程序</span><span class="sxs-lookup"><span data-stu-id="2d973-129">Initialize the Teams provider</span></span>

<span data-ttu-id="2d973-130">Microsoft Graph 工具包提供程序启用对组件的 Microsoft Graph 的身份验证和访问。</span><span class="sxs-lookup"><span data-stu-id="2d973-130">The Microsoft Graph Toolkit providers enable authentication and access to Microsoft Graph for the components.</span></span> <span data-ttu-id="2d973-131">若要了解详细信息，请参阅 [使用提供程序](../providers.md)。</span><span class="sxs-lookup"><span data-stu-id="2d973-131">To learn more, see [Using the providers](../providers.md).</span></span> <span data-ttu-id="2d973-132">[团队提供程序](../providers/teams.md)处理需要与团队 SDK 实现的所有逻辑和交互，以对用户进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="2d973-132">The [Teams provider](../providers/teams.md) handles all of the logic and interactions that need to be implemented with the Teams SDK to authenticate the user.</span></span>

<span data-ttu-id="2d973-133">您可以选择在 HTML 或 JavaScript 代码中初始化提供程序。</span><span class="sxs-lookup"><span data-stu-id="2d973-133">You can choose to initialize the provider in either your HTML or your JavaScript code.</span></span> 

### <a name="initialize-in-html"></a><span data-ttu-id="2d973-134">在 HTML 中初始化</span><span class="sxs-lookup"><span data-stu-id="2d973-134">Initialize in HTML</span></span>

<span data-ttu-id="2d973-135">在中 `public/index.html` ，添加团队提供程序，如下所示。</span><span class="sxs-lookup"><span data-stu-id="2d973-135">In `public/index.html`, add the Teams provider as shown.</span></span>

```html
<mgt-teams-provider
  client-id="<YOUR_CLIENT_ID>"
  auth-popup-url="https://<YOUR_NGROK_URL>/auth.html"
></mgt-teams-provider>
```

<span data-ttu-id="2d973-136">将替换为您的 `<YOUR_CLIENT_ID>` 应用程序的客户端 ID 和 `<YOUR_NGROK_URL>` 您创建的 ngrok URL。</span><span class="sxs-lookup"><span data-stu-id="2d973-136">Replace `<YOUR_CLIENT_ID>` with the client ID for your application and `<YOUR_NGROK_URL>` with the ngrok URL you created.</span></span>

### <a name="initialize-in-javascript"></a><span data-ttu-id="2d973-137">在 JavaScript 中初始化</span><span class="sxs-lookup"><span data-stu-id="2d973-137">Initialize in JavaScript</span></span>

<span data-ttu-id="2d973-138">若要在 JavaScript 代码中初始化提供程序，请在 `src/components/App.js` 项目目录中找到该文件。</span><span class="sxs-lookup"><span data-stu-id="2d973-138">To initialize the provider in your JavaScript code, Locate the `src/components/App.js` file in your project directory.</span></span> <span data-ttu-id="2d973-139">导入团队提供程序并初始化提供程序。</span><span class="sxs-lookup"><span data-stu-id="2d973-139">Import the Teams Provider and initialize the provider.</span></span>

```js
import * as microsoftTeams from "@microsoft/teams-js/dist/MicrosoftTeams";
import { Providers, TeamsProvider } from '@microsoft/mgt';

TeamsProvider.microsoftTeamsLib = microsoftTeams;
Providers.globalProvider = new TeamsProvider ({
    clientId: '<YOUR_CLIENT_ID>',
    authPopupUrl: '/auth.html'
})
```
<span data-ttu-id="2d973-140">将替换为 `<YOUR_CLIENT_ID>` 应用程序的客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="2d973-140">Replace `<YOUR_CLIENT_ID>` with the client ID for your application.</span></span>

### <a name="creating-an-appclient-id"></a><span data-ttu-id="2d973-141">创建应用/客户端 ID</span><span class="sxs-lookup"><span data-stu-id="2d973-141">Creating an app/client ID</span></span>
<span data-ttu-id="2d973-142">为了获取客户端 ID，需要在 Azure AD 中 [注册应用程序](https://docs.microsoft.com/graph/auth-register-app-v2) 。</span><span class="sxs-lookup"><span data-stu-id="2d973-142">In order to get a client ID, you need to [register your application](https://docs.microsoft.com/graph/auth-register-app-v2) in Azure AD.</span></span> <span data-ttu-id="2d973-143">确保将 ngrok URL 的完整路径添加到 "重定向 Uri" 中的 "身份验证" 弹出页面 (例如， `https://<YOUR_NGROK_URL>/auth.html`) "。</span><span class="sxs-lookup"><span data-stu-id="2d973-143">Make sure to add your ngrok URL with the full path to the auth popup page to your redirect URIs (for example, `https://<YOUR_NGROK_URL>/auth.html`).</span></span>
><span data-ttu-id="2d973-144">**注意**： MSAL 仅支持 OAuth 的隐式流。</span><span class="sxs-lookup"><span data-stu-id="2d973-144">**Note**: MSAL only supports the Implicit Flow for OAuth.</span></span> <span data-ttu-id="2d973-145">请务必在 Azure 门户中的应用程序中启用隐式流， (默认情况下不启用它) 。</span><span class="sxs-lookup"><span data-stu-id="2d973-145">Make sure to enable Implicit Flow in your application in the Azure Portal (it is not enabled by default).</span></span> <span data-ttu-id="2d973-146">在 " **身份验证**" 下，找到 " **隐式授予** " 部分，然后选择 " **访问令牌** " 和 **ID 令牌**的复选框。</span><span class="sxs-lookup"><span data-stu-id="2d973-146">Under **Authentication**, find the **Implicit grant** section and select the checkboxes for **Access tokens** and **ID tokens**.</span></span> 

## <a name="create-the-auth-popup-page"></a><span data-ttu-id="2d973-147">创建身份验证弹出页面</span><span class="sxs-lookup"><span data-stu-id="2d973-147">Create the auth popup page</span></span>

<span data-ttu-id="2d973-148">若要允许用户登录，需要提供工作组应用将在弹出项中打开以遵循身份验证流的 URL。</span><span class="sxs-lookup"><span data-stu-id="2d973-148">In order to allow users to sign in, you need to provide a URL that the Teams app will open in a popup to follow the authentication flow.</span></span> <span data-ttu-id="2d973-149">URL 必须在您的域中，并且所有此页面都需要调用 `TeamsProvider.handleAuth()` 方法。</span><span class="sxs-lookup"><span data-stu-id="2d973-149">The URL needs to be in your domain, and all this page needs to do is call the `TeamsProvider.handleAuth()` method.</span></span>

<span data-ttu-id="2d973-150">您可以在 HTML 中执行此操作，方法是在文件夹中添加一个新 `auth.html` 文件 `public` (该文件应与) 相同的级别 `index.html` ，并添加以下代码：</span><span class="sxs-lookup"><span data-stu-id="2d973-150">You can do this in your HTML by adding a new `auth.html` file in the `public` folder (which should be at the same level as `index.html`) and adding the following code:</span></span> 

```html
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>

<script>
  mgt.TeamsProvider.handleAuth();
</script>
```

## <a name="add-components"></a><span data-ttu-id="2d973-151">添加组件</span><span class="sxs-lookup"><span data-stu-id="2d973-151">Add components</span></span>

<span data-ttu-id="2d973-152">现在，你已准备好将任何 Microsoft Graph 工具包组件添加到你的选项卡。</span><span class="sxs-lookup"><span data-stu-id="2d973-152">Now, you're ready to add any of the Microsoft Graph Toolkit components to your tab.</span></span> 

<span data-ttu-id="2d973-153">你可以像往常一样将组件添加到你的 HTML 中。</span><span class="sxs-lookup"><span data-stu-id="2d973-153">You can add components to your HTML as you normally would.</span></span> <span data-ttu-id="2d973-154">例如，若要添加登录组件，请将以下代码添加到的正文 `index.html` ：</span><span class="sxs-lookup"><span data-stu-id="2d973-154">For example, to add the Login component add the below code to the body of your `index.html`:</span></span>

```html
<mgt-login></mgt-login>
```

<span data-ttu-id="2d973-155">或者，可以将 JSX 中的组件添加到选项卡组件中。</span><span class="sxs-lookup"><span data-stu-id="2d973-155">Or, you can add the components in JSX to the Tab component.</span></span> <span data-ttu-id="2d973-156">`mgt-react`如果使用 Microsoft 团队工具包扩展创建了团队应用程序，我们建议使用库。</span><span class="sxs-lookup"><span data-stu-id="2d973-156">We recommend using the `mgt-react` library if you created your Teams app using the Microsoft Teams Toolkit extension.</span></span> <span data-ttu-id="2d973-157">若要了解详细信息，请参阅将 [Microsoft Graph 工具包与响应结合使用](./use-toolkit-with-react.md#using-mgt-react)</span><span class="sxs-lookup"><span data-stu-id="2d973-157">To learn more, see [Using Microsoft Graph Toolkit with React](./use-toolkit-with-react.md#using-mgt-react)</span></span>

<span data-ttu-id="2d973-158">首先，安装 `mgt-react` ：</span><span class="sxs-lookup"><span data-stu-id="2d973-158">First, install `mgt-react`:</span></span>

```bash
npm install @microsoft/mgt-react
```

<span data-ttu-id="2d973-159">找到 `src/components/Tab.js` 文件，并从库中导入要使用的组件 `mgt-react` 。</span><span class="sxs-lookup"><span data-stu-id="2d973-159">Locate the `src/components/Tab.js` file and import the components you want to use from the `mgt-react` library.</span></span> <span data-ttu-id="2d973-160">例如，若要添加 `Login` 组件，请使用：</span><span class="sxs-lookup"><span data-stu-id="2d973-160">For example to add the `Login` component use:</span></span>

```js
import { Login } from "@microsoft/mgt-react"
```

<span data-ttu-id="2d973-161">然后，将该组件添加到的 `return()` 方法语句中 `render()` `Tab` ：</span><span class="sxs-lookup"><span data-stu-id="2d973-161">Then, add the the component to the `return()` statement of the `render()` method of `Tab`:</span></span>

```jsx
render() {
  return(
    <Login />
  );
}
```

## <a name="test-your-application"></a><span data-ttu-id="2d973-162">测试应用程序</span><span class="sxs-lookup"><span data-stu-id="2d973-162">Test your application</span></span>

<span data-ttu-id="2d973-163">使用以下命令生成和运行应用程序：</span><span class="sxs-lookup"><span data-stu-id="2d973-163">Build and run your application using the following commands:</span></span>
```bash
npm install
npm start
```

<span data-ttu-id="2d973-164">若要测试应用程序，需要将应用程序上载到团队。</span><span class="sxs-lookup"><span data-stu-id="2d973-164">To test your application, you need to upload your application to Teams.</span></span> <span data-ttu-id="2d973-165">打开 "Microsoft 团队客户端"，在左侧菜单中选择 " **...** "，然后转到 **应用程序 Studio**。</span><span class="sxs-lookup"><span data-stu-id="2d973-165">Open the Microsoft Teams client, select the **...** on the left-hand menu and go to **App Studio**.</span></span> <span data-ttu-id="2d973-166">单击 " **清单编辑器** " 选项卡，然后选择 " **导入现有应用程序**"。</span><span class="sxs-lookup"><span data-stu-id="2d973-166">Click the **Manifest Editor** tab and select **Import an existing app**.</span></span>

<span data-ttu-id="2d973-167">找到您的项目目录，并上传到 **. publish**文件夹中的**Development.zip**文件。</span><span class="sxs-lookup"><span data-stu-id="2d973-167">Locate your project directory and upload the **Development.zip** file inside of the **.publish** folder.</span></span>

<span data-ttu-id="2d973-168">在应用程序加载后，向下滚动到左侧菜单，然后选择 " **测试和分发**"。</span><span class="sxs-lookup"><span data-stu-id="2d973-168">After your app has loaded, scroll down on the left menu and select **Test and Distribute**.</span></span> <span data-ttu-id="2d973-169">单击 " **安装** " 按钮，然后单击 " **添加**"。</span><span class="sxs-lookup"><span data-stu-id="2d973-169">Click the **Install** button and then click **Add**.</span></span> <span data-ttu-id="2d973-170">你将被重定向到你创建的选项卡。</span><span class="sxs-lookup"><span data-stu-id="2d973-170">You will be redirected to the tab you created.</span></span>

## <a name="next-steps"></a><span data-ttu-id="2d973-171">后续步骤</span><span class="sxs-lookup"><span data-stu-id="2d973-171">Next Steps</span></span>
- <span data-ttu-id="2d973-172">请参阅本分步教程，了解如何 [生成团队选项卡](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-10-microsoft-graph-toolkit-teams-provider/)。</span><span class="sxs-lookup"><span data-stu-id="2d973-172">Check out this step-by-step tutorial on [building a Teams tab](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-10-microsoft-graph-toolkit-teams-provider/).</span></span>
- <span data-ttu-id="2d973-173">尝试 [样本](https://mgt.dev)中的组件。</span><span class="sxs-lookup"><span data-stu-id="2d973-173">Try out the components in the [playground](https://mgt.dev).</span></span>
- <span data-ttu-id="2d973-174">在 [堆栈溢出](https://aka.ms/mgt-question)时提出问题。</span><span class="sxs-lookup"><span data-stu-id="2d973-174">Ask a question on [Stack Overflow](https://aka.ms/mgt-question).</span></span>
- <span data-ttu-id="2d973-175">在 [GitHub](https://aka.ms/mgt)上报告错误或保留功能请求。</span><span class="sxs-lookup"><span data-stu-id="2d973-175">Report bugs or leave a feature request on [GitHub](https://aka.ms/mgt).</span></span>



