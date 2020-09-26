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
# <a name="build-a-web-application-with-the-microsoft-graph-toolkit"></a>使用 Microsoft Graph 工具包生成 web 应用程序

本主题介绍如何在使用 vanilla JavaScript 编写的 web 应用程序中开始使用 Microsoft Graph 工具包。 如果您想了解如何将此工具包与 web 框架结合使用，请参阅 [将此工具包与 "使用](./use-toolkit-with-react.md) " 进行响应或 [使用具有角度的工具包](./use-toolkit-with-angular.md)。

Microsoft Graph 工具包入门包括以下步骤：
1. 将 Microsoft Graph 工具包添加到项目中。
2. 初始化 MSAL 提供程序。
3. 添加组件。
4. 测试应用程序。

## <a name="add-the-microsoft-graph-toolkit-to-your-project"></a>将 Microsoft Graph 工具包添加到项目中
您可以在应用程序中使用 Microsoft Graph 工具包，方法是通过 unpkg) 或安装 npm 程序包直接 (引用加载程序。

### <a name="use-via-mgt-loader"></a>通过预加载加载程序使用
若要通过预加载程序使用该工具包，请将脚本中的引用添加到代码中：

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
```

### <a name="use-via-npm-es6-modules"></a>通过 npm (ES6 模块使用) 
通过使用 ES6 模块中的工具包，可以完全控制捆绑过程，并允许您只捆绑应用程序所需的代码。 若要使用 ES6 模块，请将 npm 包添加到项目中：

```bash
npm install @microsoft/mgt
```
> **注意**：如果您针对的是不是本机支持 web 组件的浏览器（如 IE11），则可能需要 [包含 polyfills.ts](./overview.md#polyfills)。

现在，您可以通过以下方式引用应用程序中的所有工具包组件：

```html
<script src="node_modules/@microsoft/mgt/dist/es6/components.js"></script>
```
或者，只引用所需的组件，避免加载其他内容。 例如，若要添加 MSAL 提供程序：

```html
<script src="node_modules/@microsoft/mgt/dist/es6/components/providers/mgt-msal-provider.js"></script>
```

## <a name="initialize-the-msal-provider"></a>初始化 MSAL 提供程序
Microsoft Graph 工具包提供程序启用对组件的 Microsoft Graph 的身份验证和访问。 若要了解详细信息，请参阅 [使用提供程序](../providers.md)。 [MSAL 提供程序](../providers/msal.md)使用 MSAL.js 登录用户和获取令牌。 您可以在 HTML 或 JavaScript 中初始化 MSAL 提供程序。

如果要使用自己的后端身份验证，请使用 [代理提供程序](../providers/proxy.md) 替换 MSAL 提供程序。

您可以选择在 HTML 或 JavaScript 代码中初始化提供程序。 

### <a name="initialize-in-your-html-page"></a>在 HTML 页面中初始化
将 `mgt-msal-provider` 组件添加到 HTML 页面，并将设置 `client-id` 为应用程序客户端 id。

```html
<mgt-msal-provider client-id="<YOUR_CLIENT_ID"></mgt-msal-provider>
```
### <a name="initialize-in-javascript"></a>在 JavaScript 中初始化
若要在 JavaScript 中初始化 MSAL 提供程序，请将以下代码添加到应用程序：

```js
import {Providers, MsalProvider} from '@microsoft/mgt'

Providers.globalProvider = new MsalProvider({
    clientId: "<YOUR_CLIENT_ID>"
})
```
客户端 ID 是初始化提供程序所需的唯一属性，但您可以设置其他选项。 有关完整列表，请参阅 [Msal Provider](../providers/msal.md)。

### <a name="creating-an-appclient-id"></a>创建应用/客户端 ID
为了获取客户端 ID，需要在 Azure AD 中 [注册应用程序](../../auth-register-app-v2.md) 。 
>**注意**： MSAL 仅支持 OAuth 的隐式流。 请务必在 Azure 门户中的应用程序中启用隐式流， (默认情况下不启用它) 。 在 " **身份验证**" 下，找到 " **隐式授予** " 部分，然后选择 " **访问令牌** " 和 **ID 令牌**的复选框。 

## <a name="add-components"></a>添加组件
初始化 MSAL 提供程序后，可以开始使用任何工具包组件。

以下是使用 MSAL 提供程序的完整工作示例（HTML 中初始化的）和登录组件：

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal-provider>
<mgt-login></mgt-login>
```

以下是使用 ES6 模块、MSAL 提供程序（HTML 中初始化）和登录组件的示例：
```html
<script src="node_modules/@microsoft/mgt/dist/es6/components/providers/mgt-msal-provider.js"></script>
<script src="node_modules/@microsoft/mgt/dist/es6/components/mgt-login/mgt-login.js"></script>
<mgt-msal-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal-provider>
<mgt-login></mgt-login>
```

以下是使用 ES6 模块、在 JavaScript 中初始化的 MSAL 提供程序和登录组件的示例：

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

## <a name="test-your-app"></a>测试应用程序

为了测试您的应用程序，MSAL 要求将页面托管在用于身份验证重定向的 web 服务器中。 

如果只是开始并且想要进行播放，可以在 Visual Studio Code 或任何类似的轻型开发服务器中使用 [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) 。 下载扩展并使用 live server 打开您的 HTML 文件。 
> **注意：** 确保将应用注册中的 **重定向 URI** 设置为承载您的应用程序的 localhost 端口。 转到 [Azure 门户](https://portal.azure.com)中的应用程序注册，在 "管理" 下单击 " **身份验证** "，并添加正确的 **重定向 URI**。

## <a name="next-steps"></a>后续步骤
- 请参阅本分步教程，了解如何 [生成简单的 web 应用程序](https://developer.microsoft.com/microsoft-365/blogs/a-lap-around-microsoft-graph-toolkit-day-2-zero-to-hero/)。
- 尝试 [样本](https://mgt.dev)中的组件。
- 在 [堆栈溢出](https://aka.ms/mgt-question)时提出问题。
- 在 [GitHub](https://aka.ms/mgt)上报告错误或保留功能请求。