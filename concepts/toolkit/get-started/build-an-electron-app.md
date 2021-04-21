---
title: 将 Microsoft Graph Toolkit与管理
description: 在"电子"应用程序中Toolkit Microsoft Graph 应用入门。
localization_priority: Normal
author: amrutha95
ms.openlocfilehash: b57315e3fcc44f94cc18d3f4a93826b00a5ce4b9
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920052"
---
# <a name="use-the-microsoft-graph-toolkit-with-electron"></a><span data-ttu-id="c0e9f-103">将 Microsoft Graph Toolkit与管理</span><span class="sxs-lookup"><span data-stu-id="c0e9f-103">Use the Microsoft Graph Toolkit with Electron</span></span>

<span data-ttu-id="c0e9f-104">本文介绍了使用 Microsoft Graph 应用创建Toolkit应用并连接到 Microsoft 365 的分步过程。</span><span class="sxs-lookup"><span data-stu-id="c0e9f-104">This article describes the step-by-step process of using the Microsoft Graph Toolkit to create an Electron app and connect it to Microsoft 365.</span></span> <span data-ttu-id="c0e9f-105">完成这些步骤后，你将拥有一个显示 Microsoft 365 中当前已登录用户的即将进行的约会的"展示"应用。</span><span class="sxs-lookup"><span data-stu-id="c0e9f-105">After completing the steps, you'll have a Electron app that shows the upcoming appointments of the currently signed in user from Microsoft 365.</span></span>

## <a name="create-an-electron-app"></a><span data-ttu-id="c0e9f-106">创建一个"时价"应用</span><span class="sxs-lookup"><span data-stu-id="c0e9f-106">Create an Electron app</span></span> 
<span data-ttu-id="c0e9f-107">通过克隆 [显示快速启动类型代码存储库来创建新的一个](https://github.com/electron/electron-quick-start-typescript) "显示"应用。</span><span class="sxs-lookup"><span data-stu-id="c0e9f-107">Create a new Electron app by cloning the [electron-quick-start-typescript](https://github.com/electron/electron-quick-start-typescript) repository.</span></span> <span data-ttu-id="c0e9f-108">这将使用 TypeScript 创建一个新的"显示"应用，这将帮助你编写更可靠的代码并避免运行时错误。</span><span class="sxs-lookup"><span data-stu-id="c0e9f-108">This will create a new Electron app using TypeScript, which will help you write more robust code and avoid runtime errors.</span></span>

```cmd
git clone https://github.com/electron/electron-quick-start-typescript
```

<span data-ttu-id="c0e9f-109">将工作目录更改为新创建的应用并安装所有依赖项。</span><span class="sxs-lookup"><span data-stu-id="c0e9f-109">Change the working directory to the newly created app and install all dependencies.</span></span>

```cmd
cd electron-quick-start-typescript
npm install
```

<span data-ttu-id="c0e9f-110">安装"@microsoft/mgt-components"程序包，其中包含所有连接到 Microsoft Graph 的 Web 组件。</span><span class="sxs-lookup"><span data-stu-id="c0e9f-110">Install the '@microsoft/mgt-components' package that contains all the Microsoft Graph-connected web components.</span></span>

```cmd
npm i @microsoft/mgt-components
```

<span data-ttu-id="c0e9f-111">同时安装 `@microsoft/mgt-electron-provider` `@microsoft/mgt-element` 和 npm 包。</span><span class="sxs-lookup"><span data-stu-id="c0e9f-111">Install the `@microsoft/mgt-electron-provider` and `@microsoft/mgt-element` npm packages as well.</span></span> <span data-ttu-id="c0e9f-112">这将允许你使用 MSAL 为应用提供身份验证，并使用 Microsoft Graph Toolkit组件。</span><span class="sxs-lookup"><span data-stu-id="c0e9f-112">These will allow you to provide authentication for your app using MSAL and use the Microsoft Graph Toolkit components.</span></span>

```cmd
npm i @microsoft/mgt-element @microsoft/mgt-electron-provider
```

<span data-ttu-id="c0e9f-113">确认你可以运行该应用。</span><span class="sxs-lookup"><span data-stu-id="c0e9f-113">Confirm that you can run the app.</span></span>

```cmd
npm start
```

## <a name="create-an-appclient-id"></a><span data-ttu-id="c0e9f-114">创建应用/客户端 ID</span><span class="sxs-lookup"><span data-stu-id="c0e9f-114">Create an app/client ID</span></span>

### <a name="add-new-application-registration-in-azure-ad-to-get-a-client-id"></a><span data-ttu-id="c0e9f-115">在 Azure AD 中添加新的应用程序注册，获取客户端 ID</span><span class="sxs-lookup"><span data-stu-id="c0e9f-115">Add new application registration in Azure AD to get a client ID</span></span>

<span data-ttu-id="c0e9f-116">若要在 Azure AD (Azure Active Directory) 创建应用程序，需要添加新的应用程序注册，然后配置应用名称和重定向 URI。</span><span class="sxs-lookup"><span data-stu-id="c0e9f-116">To create an application in Azure Active Directory (Azure AD), you need to add a new application registration, and then configure an app name and redirect URI.</span></span>

<span data-ttu-id="c0e9f-117">若要在 Azure AD 中创建应用，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="c0e9f-117">To create the app in Azure AD:</span></span>

1. <span data-ttu-id="c0e9f-118">转到 [Azure 门户](https://portal.azure.com)。</span><span class="sxs-lookup"><span data-stu-id="c0e9f-118">Go to the [Azure portal](https://portal.azure.com).</span></span>
1. <span data-ttu-id="c0e9f-119">从菜单中，选择 **"Azure Active Directory"。**</span><span class="sxs-lookup"><span data-stu-id="c0e9f-119">From the menu, select **Azure Active Directory**.</span></span>
1. <span data-ttu-id="c0e9f-120">从"Azure Active Directory"菜单中，选择 **"应用注册"。**</span><span class="sxs-lookup"><span data-stu-id="c0e9f-120">From the Azure Active Directory menu, select **App registrations**.</span></span>
1. <span data-ttu-id="c0e9f-121">从顶部菜单中，选择"新建 **注册"** 按钮。</span><span class="sxs-lookup"><span data-stu-id="c0e9f-121">From the top menu, select the **New registration** button.</span></span>
1. <span data-ttu-id="c0e9f-122">输入应用的名称;例如， `My Electron-App` 。</span><span class="sxs-lookup"><span data-stu-id="c0e9f-122">Enter the name for your app; for example, `My Electron-App`.</span></span>
1. <span data-ttu-id="c0e9f-123">对于受支持的帐户类型 [](/azure/active-directory/develop/single-and-multi-tenant-apps#who-can-sign-in-to-your-app)类型，选择任何组织目录中的帐户 (任何 Azure AD 目录 - 多租户) 和个人 Microsoft 帐户 **(例如 Skype、Xbox) 。**</span><span class="sxs-lookup"><span data-stu-id="c0e9f-123">For the type of [supported account types](/azure/active-directory/develop/single-and-multi-tenant-apps#who-can-sign-in-to-your-app), select **Accounts in any organizational directory (Any Azure AD directory - Multitenant) and personal Microsoft accounts (e.g. Skype, Xbox)**.</span></span>
1. <span data-ttu-id="c0e9f-124">在" **重定向 URI"** 字段中的下拉列表中，选择"公共客户端/本机 (**移动 & 桌面) "，在**"URL"字段中输入 `msal://redirect` 。</span><span class="sxs-lookup"><span data-stu-id="c0e9f-124">In the **Redirect URI** field, in the dropdown, select **Public client/native (mobile & desktop)**, and in the URL field, enter `msal://redirect`.</span></span>
1. <span data-ttu-id="c0e9f-125">通过选择"注册" **按钮确认** 更改。</span><span class="sxs-lookup"><span data-stu-id="c0e9f-125">Confirm changes by selecting the **Register** button.</span></span>
1. <span data-ttu-id="c0e9f-126">转到应用程序注册。</span><span class="sxs-lookup"><span data-stu-id="c0e9f-126">Go to your application registration.</span></span>
1. <span data-ttu-id="c0e9f-127">验证是否位于"概述 **"** 页上。</span><span class="sxs-lookup"><span data-stu-id="c0e9f-127">Verify that you are on the **Overview** page.</span></span>
1. <span data-ttu-id="c0e9f-128">从 **Essentials** 部分，将 Application (**客户端的值**) ID 属性。</span><span class="sxs-lookup"><span data-stu-id="c0e9f-128">From the **Essentials** section, copy the value of the **Application (client) ID** property.</span></span>

## <a name="configure-the-microsoft-graph-toolkit-authentication-provider"></a><span data-ttu-id="c0e9f-129">配置 Microsoft Graph Toolkit身份验证提供程序</span><span class="sxs-lookup"><span data-stu-id="c0e9f-129">Configure the Microsoft Graph Toolkit authentication provider</span></span>

### <a name="initializing-electronprovider-in-your-renderer-process"></a><span data-ttu-id="c0e9f-130">在呈现器进程中初始化一个显示器Provider</span><span class="sxs-lookup"><span data-stu-id="c0e9f-130">Initializing ElectronProvider in your renderer process</span></span>

<span data-ttu-id="c0e9f-131">负责与主进程中 (用户通信) 请求访问令牌，并接收有关 mgt 组件正常工作所需的登录 `ElectronProvider` `ElectronAuthenticator` 状态的信息。</span><span class="sxs-lookup"><span data-stu-id="c0e9f-131">The `ElectronProvider` is responsible for communicating with `ElectronAuthenticator` (in the main process) to request access tokens and receive information regarding signed in state that is required for the mgt components to work.</span></span> 

<span data-ttu-id="c0e9f-132">若要初始化 `ElectronProvider` ，请向 *src/renderer.ts 文件添加以下* 代码。</span><span class="sxs-lookup"><span data-stu-id="c0e9f-132">To initialize the `ElectronProvider`, add the following code to the *src/renderer.ts* file.</span></span>
```ts
import {Providers} from '@microsoft/mgt-element';
import {ElectronProvider} from '@microsoft/mgt-electron-provider/dist/Provider';
// import the mgt components so we can use them in our html
import '@microsoft/mgt-components';

// initialize the auth provider globally
Providers.globalProvider = new ElectronProvider();
```

### <a name="initializing-electronauthenticator-in-your-main-process"></a><span data-ttu-id="c0e9f-133">在主进程中初始化一个操作方法</span><span class="sxs-lookup"><span data-stu-id="c0e9f-133">Initializing ElectronAuthenticator in your main process</span></span>

<span data-ttu-id="c0e9f-134">负责为 MSAL 身份验证设置配置变量、获取访问令牌并与 `ElectronAuthenticator` 通信 `ElectronProvider` 。</span><span class="sxs-lookup"><span data-stu-id="c0e9f-134">The `ElectronAuthenticator` is responsible for setting up the configuration variables for MSAL authentication, acquiring access tokens, and communicating with the `ElectronProvider`.</span></span> <span data-ttu-id="c0e9f-135">在主进程中初始化 ，并设置配置变量，如客户端 `ElectronAuthenticator` ID 和所需作用域。</span><span class="sxs-lookup"><span data-stu-id="c0e9f-135">Initialize the `ElectronAuthenticator` in the main process and set up the configuration variables such as client ID and required scopes.</span></span> 

<span data-ttu-id="c0e9f-136">首先，打开 *src/main.ts，* 从页面顶部 `ElectronAuthenticator` 导入 和  `MsalElectronConfig` `@microsoft/mgt-electron-provider` 。</span><span class="sxs-lookup"><span data-stu-id="c0e9f-136">First, open *src/main.ts* and import `ElectronAuthenticator` and  `MsalElectronConfig` from `@microsoft/mgt-electron-provider` at the top of the page.</span></span>

```ts
import { ElectronAuthenticator, MsalElectronConfig } from '@microsoft/mgt-electron-provider/dist/Authenticator'; 
```
<span data-ttu-id="c0e9f-137">接下来，在 函数中添加这些代码行，以初始化在 声明位置之后 `createWindow()` 的一个 `mainWindow` 。。</span><span class="sxs-lookup"><span data-stu-id="c0e9f-137">Next, add these lines of code in the `createWindow()` function to initialize the ElectronAuthenticator, right after where `mainWindow` is declared.</span></span> <span data-ttu-id="c0e9f-138">将 `<your_client_id>` 替换为应用注册中的客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="c0e9f-138">Replace `<your_client_id>` with the client ID from your app registration.</span></span>

```ts
const config: MsalElectronConfig = {
  clientId: '<your_client_id>',
  mainWindow: mainWindow, //This is the BrowserWindow instance that requires authentication
  scopes: [
    'user.read',
        'user.read',
        'people.read',
        'user.readbasic.all',
        'contacts.read',
        'presence.read.all',
        'presence.read',
        'user.read.all',
        'calendars.read'
  ],
};
ElectronAuthenticator.initialize(config);
```

### <a name="set-nodeintegration-to-true"></a><span data-ttu-id="c0e9f-139">将 nodeIntegration 设置为 true</span><span class="sxs-lookup"><span data-stu-id="c0e9f-139">Set nodeIntegration to true</span></span>
 
<span data-ttu-id="c0e9f-140">在创建 BrowserWindow 的新实例的 main.ts 中，请确保在 `nodeIntegration` `true` webPreferences 下设置为 。</span><span class="sxs-lookup"><span data-stu-id="c0e9f-140">In main.ts, where the new instance of BrowserWindow is created, make sure that you set `nodeIntegration` to `true` under webPreferences.</span></span> <span data-ttu-id="c0e9f-141">如果跳过此步骤，则可能会遇到 ```Uncaught ReferenceError: require is not defined``` 错误。</span><span class="sxs-lookup"><span data-stu-id="c0e9f-141">If you skip this step, you might run into a ```Uncaught ReferenceError: require is not defined``` error.</span></span> <span data-ttu-id="c0e9f-142">若要保持简单，请删除任何预加载脚本。</span><span class="sxs-lookup"><span data-stu-id="c0e9f-142">To keep this simple, remove any preloading scripts.</span></span>

```ts
const mainWindow = new BrowserWindow({
  height: 600,
  webPreferences: {
    nodeIntegration: true //Set this to true
  },
  width: 800
});
```
 
### <a name="add-components-to-your-html-page"></a><span data-ttu-id="c0e9f-143">将组件添加到 HTML 页面</span><span class="sxs-lookup"><span data-stu-id="c0e9f-143">Add components to your HTML page</span></span>
 
<span data-ttu-id="c0e9f-144">向应用添加一些内容。</span><span class="sxs-lookup"><span data-stu-id="c0e9f-144">Add some content to your app.</span></span> <span data-ttu-id="c0e9f-145">现在，可以使用index.htm *页面中* 的 Microsoft Graph 工具包组件，并显示用户议程。</span><span class="sxs-lookup"><span data-stu-id="c0e9f-145">You can now use the Microsoft Graph toolkit components in your *index.html* page and show the user's agenda.</span></span> <span data-ttu-id="c0e9f-146">将 *"index.htm"页* 的内容替换为以下内容。</span><span class="sxs-lookup"><span data-stu-id="c0e9f-146">Replace the content of the *index.html* page with the following.</span></span>
 
 ```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="UTF-8" />
    <title>Sample Electron-MGT App</title>
  </head>
  <body>
    <mgt-login></mgt-login>
    <mgt-agenda group-by-day></mgt-agenda>
    <script type="module" src="./dist/renderer.js"></script>
  </body>
</html>
 ```
 ><span data-ttu-id="c0e9f-147">**注意：** 如果将其复制到现有文件，请删除任何 Content-Security-Policy 响应标头 `meta` 或标记。</span><span class="sxs-lookup"><span data-stu-id="c0e9f-147">**Note:** Remove any Content-Security-Policy response headers or `meta` tags if you are copying this onto an existing file.</span></span>
 
 ### <a name="bundle-your-app-using-webpack"></a><span data-ttu-id="c0e9f-148">使用 webpack 捆绑应用</span><span class="sxs-lookup"><span data-stu-id="c0e9f-148">Bundle your app using webpack</span></span>
 
<span data-ttu-id="c0e9f-149">在运行应用之前，你需要捆绑代码，以确保所有模块化依赖项都包含在最终负载中。</span><span class="sxs-lookup"><span data-stu-id="c0e9f-149">Before you can run the app, you  need to bundle your code to ensure that all your modular dependencies are included in the final payload.</span></span> <span data-ttu-id="c0e9f-150">如果你已经绑定应用代码，可以跳过此步骤。</span><span class="sxs-lookup"><span data-stu-id="c0e9f-150">If you are already bundling your app code, you can skip this step.</span></span>
 
 #### <a name="install-webpack"></a><span data-ttu-id="c0e9f-151">安装 webpack</span><span class="sxs-lookup"><span data-stu-id="c0e9f-151">Install webpack</span></span>
 
 ```cmd 
 npm install webpack webpack-cli ts-loader --save-dev
 ```
 
 #### <a name="webpackconfigjs"></a><span data-ttu-id="c0e9f-152">webpack.config.js</span><span class="sxs-lookup"><span data-stu-id="c0e9f-152">webpack.config.js</span></span>
 
<span data-ttu-id="c0e9f-153">在项目的 *webpack.config.js* 文件夹中创建一个新的项目文件，并粘贴以下配置。</span><span class="sxs-lookup"><span data-stu-id="c0e9f-153">Create a new *webpack.config.js* file in the root folder of your project, and paste the following configuration.</span></span>
 
 ```js
 const path = require('path');
 module.exports = [
  {
    mode: 'development',
    entry: './src/renderer.ts',
    target: 'electron-renderer',
    module: {
      rules: [
        {
          test: /\.ts$/,
          include: [/src/],
          use: [{ loader: 'ts-loader' }]
        }
      ]
    },
    output: {
      path: __dirname + '/dist',
      filename: 'renderer.js'
    },
    resolve: {
      extensions: ['.ts', '.js'],
      modules: ['node_modules', path.resolve(__dirname + 'src')]
    }
  },
  {
    mode: 'development',
    entry: './src/main.ts',
    target: 'electron-main',
    module: {
      rules: [
        {
          test: /\.ts$/,
          include: [/src/],
          use: [{ loader: 'ts-loader' }]
        }
      ]
    },
    output: {
      path: __dirname + '/dist',
      filename: 'main.js'
    },
    resolve: {
      extensions: ['.ts', '.js'],
      modules: ['node_modules', path.resolve(__dirname + 'src')]
    }
  }
 ];

 ```
 
 <span data-ttu-id="c0e9f-154">如你所见，前端 (呈现器) 和后端 (主进程) 分开捆绑。</span><span class="sxs-lookup"><span data-stu-id="c0e9f-154">As you can see, the front end (renderer process) and the back-end (main process), are bundled separately.</span></span> <span data-ttu-id="c0e9f-155">这是因为在"In一线"中，呈现器进程在浏览器上下文中运行，而主进程在节点上下文中运行。</span><span class="sxs-lookup"><span data-stu-id="c0e9f-155">This is because in Electron, the renderer process runs in the browser context and the main process runs in the node context.</span></span>
 
 #### <a name="add-the-webpacking-script-in-packagejson"></a><span data-ttu-id="c0e9f-156">将 webpacking 脚本添加到 ```package.json```</span><span class="sxs-lookup"><span data-stu-id="c0e9f-156">Add the webpacking script in ```package.json```</span></span>
 
 <span data-ttu-id="c0e9f-157">在 中添加以下 ```scripts``` 代码 ```package.json``` 。</span><span class="sxs-lookup"><span data-stu-id="c0e9f-157">Add the following under ```scripts``` in your ```package.json```.</span></span>
 
 ```json
"scripts": {
   "webpack": "webpack",
   "start": "npm run webpack && electron dist/main.js"
 }                
 ```
 
 #### <a name="run-your-app"></a><span data-ttu-id="c0e9f-158">运行应用</span><span class="sxs-lookup"><span data-stu-id="c0e9f-158">Run your app</span></span>
 
 ```cmd
 npm start
 ```

### <a name="add-token-caching-capabilities-to-your-app-and-enable-silent-sign-ins-advanced"></a><span data-ttu-id="c0e9f-159">向应用添加令牌缓存功能，并启用无提示登录 (高级) </span><span class="sxs-lookup"><span data-stu-id="c0e9f-159">Add token caching capabilities to your app and enable silent sign ins (advanced)</span></span>

<span data-ttu-id="c0e9f-160">MSAL 节点默认支持内存中缓存，并提供 ICachePlugin 接口以执行缓存序列化，但不提供将令牌缓存存储到磁盘的默认方法。</span><span class="sxs-lookup"><span data-stu-id="c0e9f-160">MSAL Node supports an in-memory cache by default and provides the ICachePlugin interface to perform cache serialization, but does not provide a default way of storing the token cache to disk.</span></span> <span data-ttu-id="c0e9f-161">如果需要永久缓存存储来启用无提示登录或跨平台缓存，我们建议使用 MSAL Node 提供的默认实现作为 [扩展](https://github.com/AzureAD/microsoft-authentication-library-for-js/tree/dev/extensions/msal-node-extensions)。</span><span class="sxs-lookup"><span data-stu-id="c0e9f-161">If you need persistent cache storage to enable silent sign ins or cross-platform caching, we recommend using the default implementation provided by MSAL Node as an [extension](https://github.com/AzureAD/microsoft-authentication-library-for-js/tree/dev/extensions/msal-node-extensions).</span></span> <span data-ttu-id="c0e9f-162">你可以导入此插件，在初始化 时传递缓存插件的实例 `ElectronAuthenticator` 。</span><span class="sxs-lookup"><span data-stu-id="c0e9f-162">You can import this plugin, and pass the instance of the cache plugin while initializing `ElectronAuthenticator`.</span></span>

```ts
let config: MsalElectronConfig = {
  ...
  cachePlugin: new PersistenceCachePlugin(filePersistence) //filePersistence is the instance of type IPersistence that you will need to create
};
```
<span data-ttu-id="c0e9f-163">若要详细了解如何实现此操作，请参阅 [microsoft-authentication-library-for-js](https://github.com/AzureAD/microsoft-authentication-library-for-js/blob/dev/extensions/samples/msal-node-extensions/index.js) 示例。</span><span class="sxs-lookup"><span data-stu-id="c0e9f-163">For more details about how to implement this, see the [microsoft-authentication-library-for-js](https://github.com/AzureAD/microsoft-authentication-library-for-js/blob/dev/extensions/samples/msal-node-extensions/index.js) sample.</span></span>

## <a name="next-steps"></a><span data-ttu-id="c0e9f-164">后续步骤</span><span class="sxs-lookup"><span data-stu-id="c0e9f-164">Next Steps</span></span>
- <span data-ttu-id="c0e9f-165">尝试在运动场中的 [组件](https://mgt.dev)。</span><span class="sxs-lookup"><span data-stu-id="c0e9f-165">Try out the components in the [playground](https://mgt.dev).</span></span>
- <span data-ttu-id="c0e9f-166">在 Microsoft [问答中&问题](/answers/products/m365#microsoft-graph)。</span><span class="sxs-lookup"><span data-stu-id="c0e9f-166">Ask a question on [Microsoft Q&A](/answers/products/m365#microsoft-graph).</span></span>
- <span data-ttu-id="c0e9f-167">在 GitHub 上报告 Bug 或保留 [功能请求](https://aka.ms/mgt)。</span><span class="sxs-lookup"><span data-stu-id="c0e9f-167">Report bugs or leave a feature request on [GitHub](https://aka.ms/mgt).</span></span>
