---
title: 使用 Microsoft Graph 工具包生成 SharePoint web 部件
description: 开始使用 Microsoft Graph 工具包生成 SharePoint web 部件。
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: bdc2d6679c145f3f50d908bbf0e4e417234c4dc9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48059648"
---
# <a name="build-a-sharepoint-web-part-with-the-microsoft-graph-toolkit"></a>使用 Microsoft Graph 工具包生成 SharePoint web 部件

本主题介绍如何在 [SharePoint 客户端 web 部件](https://docs.microsoft.com/sharepoint/dev/spfx/web-parts/overview-client-side-web-parts)中使用 Microsoft Graph 工具包组件。 入门涉及以下步骤：

1. 设置开发环境并创建 web 部件。
2. 更新项目中的 TypeScript。
3. 添加 Microsoft Graph 工具包。
4. 添加 SharePoint 提供程序。
5. 添加组件。
6. 配置权限。
7. 生成和部署 web 部件。
8. 测试 web 部件。

## <a name="set-up-your-sharepoint-framework-development-environment-and-create-a-new-web-part"></a>设置 SharePoint 框架开发环境并创建新的 web 部件

按照 [设置 SharePoint 框架开发环境](https://docs.microsoft.com/sharepoint/dev/spfx/set-up-your-development-environment) 的步骤操作，然后 [创建一个新的 web 部件](https://docs.microsoft.com/sharepoint/dev/spfx/web-parts/get-started/build-a-hello-world-web-part)。

## <a name="update-typescript-in-your-project"></a>更新项目中的 TypeScript

Microsoft Graph 工具包需要 Typescript 3. x。 将工具包添加到项目之前，请确保使用 [的是受支持的 Typescript 版本](https://github.com/SharePoint/sp-dev-docs/wiki/SharePoint-Framework-v1.8-release-notes#support-for-typescript-27-29-and-3x)。 例如，若要添加 Typescript 3.7，请使用以下命令：

```bash
npm install @microsoft/rush-stack-compiler-3.7 --save-dev
```
然后， `tsconfig.json` 在项目文件夹中找到该文件，打开该文件，然后查找此行：

```json
"extends": "./node_modules/@microsoft/rush-stack-compiler-3.3/includes/tsconfig-web.json",
```
将此行替换为：

```json
"extends": "./node_modules/@microsoft/rush-stack-compiler-3.7/includes/tsconfig-web.json",
```

## <a name="add-the-microsoft-graph-toolkit"></a>添加 Microsoft Graph 工具包

使用以下命令安装 Microsoft Graph 工具包 npm 包和 polyfills.ts：

```bash
npm install @microsoft/mgt
```
如果您计划在 web 部件中支持 IE11，则需要执行其他步骤以确保跨浏览器的兼容性：

1. 安装以下程序包：
```bash
npm install -D babel-loader @babel/core @babel/preset-env webpack
npm install -D @webcomponents/webcomponentsjs regenerator-runtime core-js
```

2. 将以下代码添加到 `gulpfile.js` 中，请在上面添加 `build.initialize(gulp)` ：
```ts
build.configureWebpack.mergeConfig({
  additionalConfiguration: (generatedConfiguration) => {
    generatedConfiguration.module.rules.push(
      {
        test: /\.m?js$/, use:
        {
          loader: "babel-loader",
          options:
          {
            presets: [["@babel/preset-env",
              {
                targets: {
                  "ie": "11"
                }
              }]]
          }
        }
      }
    );

    return generatedConfiguration;
  }
});
```
3. 在您的 `src\webparts\<your-project>\<your-web-part>.ts` 文件中，在下一步中将以下 polyfills.ts 导入到 SharePoint 提供程序之前。

```ts
import 'regenerator-runtime/runtime';
import 'core-js/es/number';
import 'core-js/es/math';
import 'core-js/es/string';
import 'core-js/es/date';
import 'core-js/es/array';
import 'core-js/es/regexp';
import '@webcomponents/webcomponentsjs/webcomponents-bundle.js';
```

## <a name="add-the-sharepoint-provider"></a>添加 SharePoint 提供程序

Microsoft Graph 工具包提供程序启用对组件的 Microsoft Graph 的身份验证和访问。 若要了解详细信息，请参阅 [使用提供程序](../providers.md)。 SharePoint web 部件始终存在于已验证的上下文中，因为用户已必须登录才能转到承载 web 部件的页面。 使用此上下文初始化 [SharePoint 提供程序](../providers/sharepoint.md)。

首先，将提供程序添加到 web 部件中。 `src\webparts\<your-project>\<your-web-part>.ts`在项目文件夹中找到该文件，并将以下行添加到文件顶部，并在现有语句的正下方 `import` ：

```ts
import { Providers, SharePointProvider } from '@microsoft/mgt';
```

接下来，您需要使用 web 部件的方法内的经过身份验证的上下文初始化提供程序 `onInit()` 。 在同一文件中，将以下代码添加到行的前面 `public render(): void {` ：

```ts
protected async onInit() {
    Providers.globalProvider = new SharePointProvider(this.context)
}
```

## <a name="add-components"></a>添加组件

现在，您可以开始向 web 部件中添加组件。 只需将组件添加到方法内的 HTML `render()` ，组件将使用 SharePoint 上下文来访问 Microsoft Graph。 例如，若要添加 " [人员" 组件](../components/person.md)，您的代码将如下所示：

```ts
public render(): void {
    this.domElement.innerHTML = `
      <mgt-person person-query="me" view="twolines"><mgt-person>
    `;
}
```

## <a name="configure-permissions"></a>配置权限

若要从 SharePoint 框架应用程序调用 Microsoft Graph，需要在解决方案包中请求所需的权限，并且 Microsoft 365 租户管理员需要批准请求的权限。

若要将权限添加到解决方案包，请找到并打开 `config\package-solution.json` 文件并设置以下内容：

```json
"isDomainIsolated": false,
```

在该行的正下方，添加以下内容：

```json
"webApiPermissionRequests":[],
```

根据所使用的组件，确定所需的 Microsoft Graph API 权限。 每个组件的文档页面提供组件所需权限的列表。 您需要将所需的每个权限添加到 `webApiPermissionRequests` 。 例如，如果您使用的是 "人员" 组件和 "议程" 组件， `webApiPermissionRequests` 可能如下所示：

```json
"webApiPermissionRequests": [
  {
    "resource": "Microsoft Graph",
    "scope": "User.Read"
  },
  {
    "resource": "Microsoft Graph",
    "scope": "Calendars.Read"
  }
]
```
## <a name="build-and-deploy-your-web-part"></a>生成和部署 web 部件

现在，将生成应用程序并将其部署到 SharePoint。 通过运行以下命令生成应用程序：

```bash
gulp build
gulp bundle
gulp package-solution
```

在 `sharepoint/solution` 文件夹中，将会有一个新 `.sppkg` 文件。 您需要将此文件上载到您的 SharePoint Online 应用程序目录。 转到 [SharePoint 管理中心的 "更多功能" 页](https://admin.microsoft.com/sharepoint?page=classicfeatures&modern=true)。 依次选择 "在**应用程序**下**打开**"、"**应用程序目录**" 和 "**分发 SharePoint 相关应用程序**"。 上传 `.sppkg` 文件，然后单击 " **部署**"。

接下来，您需要以管理员身份批准权限。

转到您的 **SharePoint 管理中心**。 在左侧导航栏中，选择 " **高级** "，然后选择 " **API 访问**"。 您应查看您在文件中添加的每个权限的挂起请求 `config\package-solution.json` 。 选择并批准每个权限。

## <a name="test-your-web-part"></a>测试 web 部件

现在，您可以将 web 部件添加到 SharePoint 页面并将其测试出来。您需要使用托管的工作台测试使用 Microsoft Graph 工具包的 web 部件，因为这些组件需要经过身份验证的上下文才能调用 Microsoft Graph。 您可以在 **https://<YOUR_TENANT sharepoint.com/_layouts/15/workbench.aspx>** 找到托管的工作台。

`config\serve.json`在项目中打开文件，并将 "" 的值替换为 `initialPage` 托管的工作台的 url：
```json
"initialPage": "https://<YOUR_TENANT>.sharepoint.com/_layouts/15/workbench.aspx",
```
保存该文件，然后在控制台中运行以下命令，以生成并预览 web 部件：

```bash
gulp serve
```

托管的工作台将自动在浏览器中打开。 将 web 部件添加到页面中，并应在操作中看到包含 Microsoft Graph 工具包组件的 web 部件！ 只要 gulp 服务命令仍在控制台中运行，您就可以继续对代码进行编辑，然后刷新浏览器以查看所做的更改。

## <a name="next-steps"></a>后续步骤
- 请参阅本分步教程，了解如何 [生成 SharePoint web 部件](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-9-microsoft-graph-toolkit-sharepoint-provider/)。
- 尝试 [样本](https://mgt.dev)中的组件。
- 在 [堆栈溢出](https://aka.ms/mgt-question)时提出问题。
- 在 [GitHub](https://aka.ms/mgt)上报告错误或保留功能请求。


