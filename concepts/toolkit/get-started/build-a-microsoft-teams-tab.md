---
title: 使用 Microsoft Graph 工具生成 Microsoft Teams Toolkit
description: 开始使用 Microsoft Graph Toolkit 构建 Microsoft Teams 选项卡。
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: 757c7eb8a94b0f6936a21f5ecb6f126cde36b6ad
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721563"
---
# <a name="build-a-microsoft-teams-tab-with-the-microsoft-graph-toolkit"></a><span data-ttu-id="d686d-103">使用 Microsoft Graph 工具生成 Microsoft Teams Toolkit</span><span class="sxs-lookup"><span data-stu-id="d686d-103">Build a Microsoft Teams tab with the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="d686d-104">本主题介绍如何在 Microsoft Teams 解决方案中开始使用 Microsoft Graph Toolkit。</span><span class="sxs-lookup"><span data-stu-id="d686d-104">This topic covers how to get started using the Microsoft Graph Toolkit in a Microsoft Teams solution.</span></span> <span data-ttu-id="d686d-105">入门包括以下步骤：</span><span class="sxs-lookup"><span data-stu-id="d686d-105">Getting started involves the following steps:</span></span>

1. <span data-ttu-id="d686d-106">使用自定义选项卡创建新的 Teams 应用程序。</span><span class="sxs-lookup"><span data-stu-id="d686d-106">Create a new Teams application with a custom tab.</span></span>
2. <span data-ttu-id="d686d-107">设置 ngrok 并创建隧道。</span><span class="sxs-lookup"><span data-stu-id="d686d-107">Set up ngrok and create a tunnel.</span></span>
3. <span data-ttu-id="d686d-108">添加 Microsoft Graph Toolkit。</span><span class="sxs-lookup"><span data-stu-id="d686d-108">Add the Microsoft Graph Toolkit.</span></span>
4. <span data-ttu-id="d686d-109">初始化 Microsoft Teams 提供程序。</span><span class="sxs-lookup"><span data-stu-id="d686d-109">Initialize the Microsoft Teams provider.</span></span>
5. <span data-ttu-id="d686d-110">创建身份验证弹出页。</span><span class="sxs-lookup"><span data-stu-id="d686d-110">Create the auth popup page.</span></span>
6. <span data-ttu-id="d686d-111">添加组件。</span><span class="sxs-lookup"><span data-stu-id="d686d-111">Add components.</span></span>
7. <span data-ttu-id="d686d-112">测试你的应用。</span><span class="sxs-lookup"><span data-stu-id="d686d-112">Test your app.</span></span>

## <a name="create-a-new-teams-application-with-a-custom-tab"></a><span data-ttu-id="d686d-113">使用自定义选项卡创建新的 Teams 应用程序</span><span class="sxs-lookup"><span data-stu-id="d686d-113">Create a new Teams application with a custom tab</span></span>

<span data-ttu-id="d686d-114">创建新 Teams 应用的最简单方法是使用 [Microsoft Teams](https://marketplace.visualstudio.com/items?itemName=TeamsDevApp.ms-teams-vscode-extension) Toolkit扩展Visual Studio Code。</span><span class="sxs-lookup"><span data-stu-id="d686d-114">The easiest way to create a new Teams app is to use the [Microsoft Teams Toolkit extension](https://marketplace.visualstudio.com/items?itemName=TeamsDevApp.ms-teams-vscode-extension) for Visual Studio Code.</span></span> <span data-ttu-id="d686d-115">按照说明 [设置新的 Teams 项目](/microsoftteams/platform/toolkit/visual-studio-code-overview#set-up-a-new-teams-project)。</span><span class="sxs-lookup"><span data-stu-id="d686d-115">Follow the instructions to [set up a new Teams project](/microsoftteams/platform/toolkit/visual-studio-code-overview#set-up-a-new-teams-project).</span></span> <span data-ttu-id="d686d-116">当你进入"添加 **功能** "屏幕时，选择 **"选项卡**"，然后选择" **个人"选项卡**。</span><span class="sxs-lookup"><span data-stu-id="d686d-116">When you get to the **Add capabilities** screen, select **Tab**, and then **Personal tab**.</span></span>

## <a name="set-up-ngrok-and-create-a-tunnel"></a><span data-ttu-id="d686d-117">设置 ngrok 并创建隧道</span><span class="sxs-lookup"><span data-stu-id="d686d-117">Set up ngrok and create a tunnel</span></span>

<span data-ttu-id="d686d-118">为了稍后测试应用程序，您需要使用 HTTPS 通过面向公众的 URL 承载应用程序。</span><span class="sxs-lookup"><span data-stu-id="d686d-118">In order to test your application later, you will need to host your application over a public-facing URL using HTTPS.</span></span> <span data-ttu-id="d686d-119">通过 [以下命令安装 ngrok，](https://ngrok.com/download) 并创建从 Internet 到 localhost：3000 的隧道：</span><span class="sxs-lookup"><span data-stu-id="d686d-119">Install [ngrok](https://ngrok.com/download) and create a tunnel from the Internet to localhost:3000 with the following command:</span></span>

```bash
ngrok http 3000
```
<span data-ttu-id="d686d-120">在项目目录中，找到 `.publish\Development.env` 该文件，并将其值替换为 `baseUrl0` ngrok URL。</span><span class="sxs-lookup"><span data-stu-id="d686d-120">In your project directory, locate the `.publish\Development.env` file and replace the value for `baseUrl0` with your ngrok URL.</span></span>

## <a name="add-the-microsoft-graph-toolkit"></a><span data-ttu-id="d686d-121">添加 Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="d686d-121">Add the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="d686d-122">可以在应用程序中使用 Microsoft Graph Toolkit，方法为通过 unpkg (或安装 npm 包) 加载程序。</span><span class="sxs-lookup"><span data-stu-id="d686d-122">You can use the Microsoft Graph Toolkit in your application by referencing the loader directly (via unpkg) or by installing the npm package.</span></span> <span data-ttu-id="d686d-123">若要使用Toolkit，你还需要[Microsoft Teams SDK。](/javascript/api/overview/msteams-client?view=msteams-client-js-latest)</span><span class="sxs-lookup"><span data-stu-id="d686d-123">To use the Toolkit, you will also need the [Microsoft Teams SDK](/javascript/api/overview/msteams-client?view=msteams-client-js-latest).</span></span>

### <a name="use-via-mgt-loader"></a><span data-ttu-id="d686d-124">通过 mgt-loader 使用</span><span class="sxs-lookup"><span data-stu-id="d686d-124">Use via mgt-loader</span></span>
<span data-ttu-id="d686d-125">若要通过Toolkit使用 Toolkit 和 Teams SDK，请添加以下引用 `public/index.html` ：</span><span class="sxs-lookup"><span data-stu-id="d686d-125">To use the Toolkit and the Teams SDK via the loaders, add the following references to `public/index.html`:</span></span>

```html
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
```

### <a name="use-via-npm-es6-modules"></a><span data-ttu-id="d686d-126">通过 npm (ES6 模块) </span><span class="sxs-lookup"><span data-stu-id="d686d-126">Use via npm (ES6 modules)</span></span>
<span data-ttu-id="d686d-127">使用Toolkit ES6 模块进行绑定将让你完全控制捆绑过程，并允许你仅捆绑应用程序所需的代码。</span><span class="sxs-lookup"><span data-stu-id="d686d-127">Using the Toolkit via ES6 modules will give you full control of the bundling process and allow you to bundle only the code you need for your application.</span></span> <span data-ttu-id="d686d-128">若要使用 ES6 模块，请为项目添加 Toolkit 和 Microsoft Teams SDK 的 npm 包：</span><span class="sxs-lookup"><span data-stu-id="d686d-128">To use the ES6 modules, add the npm packages for both the Toolkit and the Microsoft Teams SDK to your project:</span></span>

```bash
npm install @microsoft/mgt @microsoft/teams-js
```

## <a name="initialize-the-teams-provider"></a><span data-ttu-id="d686d-129">初始化 Teams 提供程序</span><span class="sxs-lookup"><span data-stu-id="d686d-129">Initialize the Teams provider</span></span>

<span data-ttu-id="d686d-130">Microsoft Graph Toolkit提供程序支持对组件的 Microsoft Graph 进行身份验证和访问。</span><span class="sxs-lookup"><span data-stu-id="d686d-130">The Microsoft Graph Toolkit providers enable authentication and access to Microsoft Graph for the components.</span></span> <span data-ttu-id="d686d-131">若要了解更多信息，请参阅["使用提供程序"。](../providers/providers.md)</span><span class="sxs-lookup"><span data-stu-id="d686d-131">To learn more, see [Using the providers](../providers/providers.md).</span></span> <span data-ttu-id="d686d-132">[Teams 提供程序](../providers/teams.md)处理需要通过 Teams SDK 实现以对用户进行身份验证的所有逻辑和交互。</span><span class="sxs-lookup"><span data-stu-id="d686d-132">The [Teams provider](../providers/teams.md) handles all of the logic and interactions that need to be implemented with the Teams SDK to authenticate the user.</span></span>

<span data-ttu-id="d686d-133">你可以选择在 HTML 或 JavaScript 代码中初始化提供程序。</span><span class="sxs-lookup"><span data-stu-id="d686d-133">You can choose to initialize the provider in either your HTML or your JavaScript code.</span></span> 

### <a name="initialize-in-html"></a><span data-ttu-id="d686d-134">在 HTML 中初始化</span><span class="sxs-lookup"><span data-stu-id="d686d-134">Initialize in HTML</span></span>

<span data-ttu-id="d686d-135">In `public/index.html` ， add the Teams provider as shown.</span><span class="sxs-lookup"><span data-stu-id="d686d-135">In `public/index.html`, add the Teams provider as shown.</span></span>

```html
<mgt-teams-provider
  client-id="<YOUR_CLIENT_ID>"
  auth-popup-url="https://<YOUR_NGROK_URL>/auth.html"
></mgt-teams-provider>
```

<span data-ttu-id="d686d-136">用 `<YOUR_CLIENT_ID>` 应用程序的客户端 ID 和 `<YOUR_NGROK_URL>` 您创建的 ngrok URL 替换。</span><span class="sxs-lookup"><span data-stu-id="d686d-136">Replace `<YOUR_CLIENT_ID>` with the client ID for your application and `<YOUR_NGROK_URL>` with the ngrok URL you created.</span></span>

### <a name="initialize-in-javascript"></a><span data-ttu-id="d686d-137">在 JavaScript 中初始化</span><span class="sxs-lookup"><span data-stu-id="d686d-137">Initialize in JavaScript</span></span>

<span data-ttu-id="d686d-138">若要在 JavaScript 代码中初始化提供程序，请在项目 `src/components/App.js` 目录中找到该文件。</span><span class="sxs-lookup"><span data-stu-id="d686d-138">To initialize the provider in your JavaScript code, Locate the `src/components/App.js` file in your project directory.</span></span> <span data-ttu-id="d686d-139">导入 Teams 提供商并初始化提供商。</span><span class="sxs-lookup"><span data-stu-id="d686d-139">Import the Teams Provider and initialize the provider.</span></span>

```js
import * as microsoftTeams from "@microsoft/teams-js";
import { Providers, TeamsProvider } from '@microsoft/mgt';

TeamsProvider.microsoftTeamsLib = microsoftTeams;
Providers.globalProvider = new TeamsProvider ({
    clientId: '<YOUR_CLIENT_ID>',
    authPopupUrl: '/auth.html'
})
```
<span data-ttu-id="d686d-140">替换为 `<YOUR_CLIENT_ID>` 应用程序的客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="d686d-140">Replace `<YOUR_CLIENT_ID>` with the client ID for your application.</span></span>

### <a name="creating-an-appclient-id"></a><span data-ttu-id="d686d-141">创建应用/客户端 ID</span><span class="sxs-lookup"><span data-stu-id="d686d-141">Creating an app/client ID</span></span>
<span data-ttu-id="d686d-142">若要获取客户端 ID，需要在 Azure AD [中注册应用程序](../../auth-register-app-v2.md) 。</span><span class="sxs-lookup"><span data-stu-id="d686d-142">In order to get a client ID, you need to [register your application](../../auth-register-app-v2.md) in Azure AD.</span></span> <span data-ttu-id="d686d-143">请确保将您的 ngrok URL 与身份验证弹出窗口页面的完整路径添加到重定向 URI (例如 `https://<YOUR_NGROK_URL>/auth.html` ，) 。</span><span class="sxs-lookup"><span data-stu-id="d686d-143">Make sure to add your ngrok URL with the full path to the auth popup page to your redirect URIs (for example, `https://<YOUR_NGROK_URL>/auth.html`).</span></span>
><span data-ttu-id="d686d-144">**注意**：MSAL 仅支持 OAuth 的隐式流。</span><span class="sxs-lookup"><span data-stu-id="d686d-144">**Note**: MSAL only supports the Implicit Flow for OAuth.</span></span> <span data-ttu-id="d686d-145">请确保在 Azure 门户中启用应用程序中的隐式流 (默认情况下不会启用它) 。</span><span class="sxs-lookup"><span data-stu-id="d686d-145">Make sure to enable Implicit Flow in your application in the Azure Portal (it is not enabled by default).</span></span> <span data-ttu-id="d686d-146">在 **"身份验证**"下，找到 **隐式授予** 部分，并选中 **访问** 令牌和 **ID 令牌的复选框**。</span><span class="sxs-lookup"><span data-stu-id="d686d-146">Under **Authentication**, find the **Implicit grant** section and select the checkboxes for **Access tokens** and **ID tokens**.</span></span> 

## <a name="create-the-auth-popup-page"></a><span data-ttu-id="d686d-147">创建身份验证弹出页</span><span class="sxs-lookup"><span data-stu-id="d686d-147">Create the auth popup page</span></span>

<span data-ttu-id="d686d-148">为了允许用户登录，你需要提供 Teams 应用将在弹出窗口中打开的 URL，以遵循身份验证流。</span><span class="sxs-lookup"><span data-stu-id="d686d-148">In order to allow users to sign in, you need to provide a URL that the Teams app will open in a popup to follow the authentication flow.</span></span> <span data-ttu-id="d686d-149">URL 需要位于域中，此页面需要执行的所有操作就是调用 `TeamsProvider.handleAuth()` 该方法。</span><span class="sxs-lookup"><span data-stu-id="d686d-149">The URL needs to be in your domain, and all this page needs to do is call the `TeamsProvider.handleAuth()` method.</span></span>

<span data-ttu-id="d686d-150">您可以通过在文件夹文件夹中添加新文件来在 HTML 中 (该文件应处于与) 相同的级别，并添加 `auth.html` `public` `index.html` 以下代码：</span><span class="sxs-lookup"><span data-stu-id="d686d-150">You can do this in your HTML by adding a new `auth.html` file in the `public` folder (which should be at the same level as `index.html`) and adding the following code:</span></span> 

```html
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>

<script>
  mgt.TeamsProvider.handleAuth();
</script>
```

## <a name="add-components"></a><span data-ttu-id="d686d-151">添加组件</span><span class="sxs-lookup"><span data-stu-id="d686d-151">Add components</span></span>

<span data-ttu-id="d686d-152">现在，你已准备好将任何 Microsoft Graph Toolkit组件添加到你的选项卡。</span><span class="sxs-lookup"><span data-stu-id="d686d-152">Now, you're ready to add any of the Microsoft Graph Toolkit components to your tab.</span></span> 

<span data-ttu-id="d686d-153">您可以像正常操作一样将组件添加到 HTML。</span><span class="sxs-lookup"><span data-stu-id="d686d-153">You can add components to your HTML as you normally would.</span></span> <span data-ttu-id="d686d-154">例如，若要添加登录组件，请向以下代码的正文添加 `index.html` ：</span><span class="sxs-lookup"><span data-stu-id="d686d-154">For example, to add the Login component add the below code to the body of your `index.html`:</span></span>

```html
<mgt-login></mgt-login>
```

<span data-ttu-id="d686d-155">或者，可以将 JSX 中的组件添加到 Tab 组件。</span><span class="sxs-lookup"><span data-stu-id="d686d-155">Or, you can add the components in JSX to the Tab component.</span></span> <span data-ttu-id="d686d-156">如果你使用 Microsoft Teams 应用扩展创建了 Teams 应用， `mgt-react` 我们建议Toolkit库。</span><span class="sxs-lookup"><span data-stu-id="d686d-156">We recommend using the `mgt-react` library if you created your Teams app using the Microsoft Teams Toolkit extension.</span></span> <span data-ttu-id="d686d-157">若要了解更多信息，请参阅 [将 Microsoft Graph Toolkit React](./use-toolkit-with-react.md)</span><span class="sxs-lookup"><span data-stu-id="d686d-157">To learn more, see [Using Microsoft Graph Toolkit with React](./use-toolkit-with-react.md)</span></span>

<span data-ttu-id="d686d-158">首先，安装 `mgt-react` ：</span><span class="sxs-lookup"><span data-stu-id="d686d-158">First, install `mgt-react`:</span></span>

```bash
npm install @microsoft/mgt-react
```

<span data-ttu-id="d686d-159">找到 `src/components/Tab.js` 该文件，然后从库导入想要使用 `mgt-react` 的组件。</span><span class="sxs-lookup"><span data-stu-id="d686d-159">Locate the `src/components/Tab.js` file and import the components you want to use from the `mgt-react` library.</span></span> <span data-ttu-id="d686d-160">例如，若要添加 `Login` 组件，请使用：</span><span class="sxs-lookup"><span data-stu-id="d686d-160">For example, to add the `Login` component use:</span></span>

```js
import { Login } from "@microsoft/mgt-react"
```

<span data-ttu-id="d686d-161">然后，将组件添加到 `return()` 以下方法 `render()` 的语句 `Tab` 中：</span><span class="sxs-lookup"><span data-stu-id="d686d-161">Then, add the the component to the `return()` statement of the `render()` method of `Tab`:</span></span>

```jsx
render() {
  return(
    <Login />
  );
}
```

## <a name="test-your-application"></a><span data-ttu-id="d686d-162">测试应用程序</span><span class="sxs-lookup"><span data-stu-id="d686d-162">Test your application</span></span>

<span data-ttu-id="d686d-163">使用以下命令生成并运行应用程序：</span><span class="sxs-lookup"><span data-stu-id="d686d-163">Build and run your application using the following commands:</span></span>
```bash
npm install
npm start
```

<span data-ttu-id="d686d-164">若要测试应用程序，需要将应用程序上载到 Teams。</span><span class="sxs-lookup"><span data-stu-id="d686d-164">To test your application, you need to upload your application to Teams.</span></span> <span data-ttu-id="d686d-165">打开 Microsoft Teams 客户端，选择左侧菜单上的 **...，** 然后转到 **App Studio。**</span><span class="sxs-lookup"><span data-stu-id="d686d-165">Open the Microsoft Teams client, select the **...** on the left-hand menu and go to **App Studio**.</span></span> <span data-ttu-id="d686d-166">单击清单 **编辑器** 选项卡，然后选择 **"导入现有应用"。**</span><span class="sxs-lookup"><span data-stu-id="d686d-166">Click the **Manifest Editor** tab and select **Import an existing app**.</span></span>

<span data-ttu-id="d686d-167">找到项目目录，Development.zip **.publish\*\*\*\*文件夹内** 上传文件。</span><span class="sxs-lookup"><span data-stu-id="d686d-167">Locate your project directory and upload the **Development.zip** file inside of the **.publish** folder.</span></span>

<span data-ttu-id="d686d-168">加载应用后，向下滚动左侧菜单，然后选择"**测试和分发"。**</span><span class="sxs-lookup"><span data-stu-id="d686d-168">After your app has loaded, scroll down on the left menu and select **Test and Distribute**.</span></span> <span data-ttu-id="d686d-169">单击 **"安装**"按钮，然后单击"**添加"。**</span><span class="sxs-lookup"><span data-stu-id="d686d-169">Click the **Install** button and then click **Add**.</span></span> <span data-ttu-id="d686d-170">您将重定向到您创建的选项卡。</span><span class="sxs-lookup"><span data-stu-id="d686d-170">You will be redirected to the tab you created.</span></span>

## <a name="next-steps"></a><span data-ttu-id="d686d-171">后续步骤</span><span class="sxs-lookup"><span data-stu-id="d686d-171">Next Steps</span></span>
- <span data-ttu-id="d686d-172">请查看此有关生成 Teams 选项卡的 [分步教程](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-10-microsoft-graph-toolkit-teams-provider/)。</span><span class="sxs-lookup"><span data-stu-id="d686d-172">Check out this step-by-step tutorial on [building a Teams tab](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-10-microsoft-graph-toolkit-teams-provider/).</span></span>
- <span data-ttu-id="d686d-173">尝试在运动场 [中的组件](https://mgt.dev)。</span><span class="sxs-lookup"><span data-stu-id="d686d-173">Try out the components in the [playground](https://mgt.dev).</span></span>
- <span data-ttu-id="d686d-174">在 Stack [Overflow](https://aka.ms/mgt-question)上提问。</span><span class="sxs-lookup"><span data-stu-id="d686d-174">Ask a question on [Stack Overflow](https://aka.ms/mgt-question).</span></span>
- <span data-ttu-id="d686d-175">报告 Bug 或在 GitHub 上保留 [功能请求](https://aka.ms/mgt)。</span><span class="sxs-lookup"><span data-stu-id="d686d-175">Report bugs or leave a feature request on [GitHub](https://aka.ms/mgt).</span></span>
