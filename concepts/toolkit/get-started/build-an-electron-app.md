---
title: 将 Microsoft Graph Toolkit与一起使用
description: 开始在一个"Toolkit"应用程序中使用 Microsoft Graph 应用。
localization_priority: Normal
author: amrutha95
ms.openlocfilehash: ad0d13ceb8a6ef12535dd635bf7eb011d765db9d
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50471417"
---
# <a name="use-the-microsoft-graph-toolkit-with-electron"></a>将 Microsoft Graph Toolkit与一起使用

本文介绍使用 Microsoft Graph 应用创建Toolkit应用并连接到 Microsoft 365 的分步过程。 完成这些步骤后，你将拥有一个"一体"应用，该应用显示 Microsoft 365 中当前已登录用户的即将进行的约会。

## <a name="create-an-electron-app"></a>创建一个"小元素"应用 
通过克隆快速启动类型库创建新的" [一些"](https://github.com/electron/electron-quick-start-typescript) 应用。 这将使用 TypeScript 创建新的一个"一年一次"应用，这将帮助您编写更可靠的代码并避免运行时错误。

```cmd
git clone https://github.com/electron/electron-quick-start-typescript
```

将工作目录更改为新创建的应用并安装所有依赖项。

```cmd
cd electron-quick-start-typescript
npm install
```

安装包含@microsoft Microsoft Graph 连接的 Web 组件的"@microsoft/mgt-components"程序包。

```cmd
npm i @microsoft/mgt-components
```

同时 `@microsoft/mgt-electron-provider` 安装 `@microsoft/mgt-element` 和 npm 程序包。 这将允许你使用 MSAL 为应用提供身份验证，并使用 Microsoft Graph Toolkit组件。

```cmd
npm i @microsoft/mgt-element @microsoft/mgt-electron-provider
```

确认你可以运行该应用。

```cmd
npm start
```

## <a name="create-an-appclient-id"></a>创建应用/客户端 ID

### <a name="add-new-application-registration-in-azure-ad-to-get-a-client-id"></a>在 Azure AD 中添加新应用程序注册，获取客户端 ID

若要在 Azure AD (Azure Active Directory) 创建应用程序，需要添加新的应用程序注册，然后配置应用名称和重定向 URI。

若要在 Azure AD 中创建应用，请执行以下操作：

1. 转到 [Azure 门户](https://portal.azure.com)。
1. 从菜单中，选择 **Azure Active Directory**。
1. 从 Azure Active Directory 菜单中，选择 **应用注册**。
1. 从顶部菜单中，选择 **"新建注册"** 按钮。
1. 输入应用的名称;例如 `My Electron-App` ，。
1. 对于受支持的帐户类型 [](/azure/active-directory/develop/single-and-multi-tenant-apps#who-can-sign-in-to-your-app)类型，选择任何组织目录中的帐户 (任何 Azure AD 目录 - 多租户) 和个人 Microsoft 帐户 (例如 **Skype、Xbox) 。**
1. 在"重定向 **URI"** 字段中的下拉列表中，选择 **"** 公共客户端/本机 (移动&桌面) ，在 URL 字段中输入 `msal://redirect` 。
1. 通过选择"注册"按钮 **确认** 更改。
1. 转到应用程序注册。
1. 验证是否位于"概述 **"** 页上。
1. 从 **Essentials** 部分，将 Application (**客户端的值) ID** 属性。

## <a name="configure-the-microsoft-graph-toolkit-authentication-provider"></a>配置 Microsoft Graph Toolkit身份验证提供程序

### <a name="initializing-electronprovider-in-your-renderer-process"></a>在呈现器进程中初始化IzingErProvider

负责与主进程中的 (通信) 请求访问令牌，并接收有关 mgt 组件正常工作所需的已登录状态 `ElectronProvider` `ElectronAuthenticator` 的信息。 

若要初始化， `ElectronProvider` 请向 *src/renderer.ts 文件添加以下* 代码。
```ts
import {Providers} from '@microsoft/mgt-element';
import {ElectronProvider} from '@microsoft/mgt-electron-provider/dist/Provider';
// import the mgt components so we can use them in our html
import '@microsoft/mgt-components';

// initialize the auth provider globally
Providers.globalProvider = new ElectronProvider();
```

### <a name="initializing-electronauthenticator-in-your-main-process"></a>在主进程中初始化Authenticator

负责为 MSAL 身份验证设置配置变量、获取访问令牌以及与 `ElectronAuthenticator` `ElectronProvider` . 在主进程中初始化它并设置配置变量，如 `ElectronAuthenticator` 客户端 ID 和所需作用域。 

首先，打开 *src/main.ts，* 然后从页面顶部导入 `ElectronAuthenticator`  `MsalElectronConfig` `@microsoft/mgt-electron-provider` 和导入。

```ts
import { ElectronAuthenticator, MsalElectronConfig } from '@microsoft/mgt-electron-provider/dist/Authenticator'; 
```
Next, add these lines of code in the `createWindow()` function to initialize the ElectronAuthenticator, right after where `mainWindow` is declared. 使用 `<your_client_id>` 应用注册中的客户端 ID 替换。

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

### <a name="set-nodeintegration-to-true"></a>将 nodeIntegration 设置为 true
 
在创建 BrowserWindow 新实例的 main.ts 中，请确保在 `nodeIntegration` `true` webPreferences 下设置为。 如果跳过此步骤，可能会出现错误 ```Uncaught ReferenceError: require is not defined``` 。 若要保持简单，请删除任何预加载脚本。

```ts
const mainWindow = new BrowserWindow({
  height: 600,
  webPreferences: {
    nodeIntegration: true //Set this to true
  },
  width: 800
});
```
 
### <a name="add-components-to-your-html-page"></a>将组件添加到 HTML 页面
 
向应用添加一些内容。 现在，可以使用index.htm *l* 页中的 Microsoft Graph 工具包组件，并显示用户议程。 将index.htm *l* 页的内容替换为以下内容。
 
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
 >**注意：** 如果要将其复制到现有文件，请删除任何 Content-Security-Policy 响应标头 `meta` 或标记。
 
 ### <a name="bundle-your-app-using-webpack"></a>使用 webpack 捆绑应用
 
在运行应用之前，需要捆绑代码，以确保所有模块化依赖项都包含在最终有效负载中。 如果你已经绑定应用代码，可以跳过此步骤。
 
 #### <a name="install-webpack"></a>安装 webpack
 
 ```cmd 
 npm install webpack webpack-cli ts-loader --save-dev
 ```
 
 #### <a name="webpackconfigjs"></a>webpack.config.js
 
在项目的 *webpack.config.js* 文件夹中创建一个新的应用程序文件，并粘贴以下配置。
 
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
 
 如你所见，前端 (呈现器) 和后端 (主进程) 分开捆绑。 这是因为在"一线"中，呈现器进程在浏览器上下文中运行，主进程在节点上下文中运行。
 
 #### <a name="add-the-webpacking-script-in-packagejson"></a>将 webpacking 脚本添加到 ```package.json```
 
 在 . ```scripts``` ```package.json```
 
 ```json
"scripts": {
   "webpack": "webpack",
   "start": "npm run webpack && electron dist/main.js"
 }                
 ```
 
 #### <a name="run-your-app"></a>运行应用
 
 ```cmd
 npm start
 ```

### <a name="add-token-caching-capabilities-to-your-app-and-enable-silent-sign-ins-advanced"></a>向应用添加令牌缓存功能，并启用无提示登录 (高级) 

MSAL 节点默认支持内存中缓存，并提供 ICachePlugin 接口来执行缓存序列化，但不提供将令牌缓存存储到磁盘的默认方法。 如果需要永久缓存存储来启用无提示登录或跨平台缓存，我们建议使用 MSAL 节点提供的默认实现作为 [扩展](https://github.com/AzureAD/microsoft-authentication-library-for-js/tree/dev/extensions/msal-node-extensions)。 你可以导入此插件，在初始化时传递缓存插件的实例 `ElectronAuthenticator` 。

```ts
let config: MsalElectronConfig = {
  ...
  cachePlugin: new PersistenceCachePlugin(filePersistence) //filePersistence is the instance of type IPersistence that you will need to create
};
```
若要详细了解如何实现此方案，请参阅 [microsoft-authentication-library-for-js](https://github.com/AzureAD/microsoft-authentication-library-for-js/blob/dev/extensions/samples/msal-node-extensions/index.js) 示例。

## <a name="next-steps"></a>后续步骤
- 尝试在运动场 [中的组件](https://mgt.dev)。
- 在 Microsoft 问答 [上&问题](https://aka.ms/askgraph)。
- 报告 Bug 或在 GitHub 上保留 [功能请求](https://aka.ms/mgt)。
    
