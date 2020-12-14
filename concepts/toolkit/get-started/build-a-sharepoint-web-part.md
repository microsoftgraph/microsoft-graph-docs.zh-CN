---
title: 使用 Microsoft Graph 部件生成 SharePoint Toolkit
description: 开始使用 Microsoft Graph Toolkit生成 SharePoint Web 部件。
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: d07a597c69ae998c75e3d4698cb0513cff056e56
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49659748"
---
# <a name="build-a-sharepoint-web-part-with-the-microsoft-graph-toolkit"></a>使用 Microsoft Graph 部件生成 SharePoint Toolkit

本主题介绍如何使用 Microsoft Graph Toolkit SharePoint 客户端 Web [部件中的组件](/sharepoint/dev/spfx/web-parts/overview-client-side-web-parts)。 入门包括以下步骤：

1. 设置开发环境并创建 Web 部件。
2. 更新项目中的 TypeScript。
3. 添加 Microsoft Graph Toolkit。
4. 添加 SharePoint 提供程序。
5. 添加组件。
6. 配置权限。
7. 生成和部署 Web 部件。
8. 测试 Web 部件。

## <a name="set-up-your-sharepoint-framework-development-environment-and-create-a-new-web-part"></a>设置 SharePoint 框架开发环境并创建新的 Web 部件

按照步骤设置[SharePoint 框架开发环境，](/sharepoint/dev/spfx/set-up-your-development-environment)[然后创建新的 Web 部件](/sharepoint/dev/spfx/web-parts/get-started/build-a-hello-world-web-part)。

## <a name="update-typescript-in-your-project"></a>更新项目中的 TypeScript

Microsoft Graph Toolkit Typescript 3.x。 在将Toolkit项目之前，请确保你使用的是支持的 [Typescript 版本](https://github.com/SharePoint/sp-dev-docs/wiki/SharePoint-Framework-v1.8-release-notes#support-for-typescript-27-29-and-3x)。 例如，若要添加 Typescript 3.7，请使用以下命令：

```bash
npm install @microsoft/rush-stack-compiler-3.7 --save-dev
```
然后，在 `tsconfig.json` 项目文件夹中找到该文件，打开该文件，然后查找以下行：

```json
"extends": "./node_modules/@microsoft/rush-stack-compiler-3.3/includes/tsconfig-web.json",
```
将该行替换为：

```json
"extends": "./node_modules/@microsoft/rush-stack-compiler-3.7/includes/tsconfig-web.json",
```

## <a name="add-the-microsoft-graph-toolkit"></a>添加 Microsoft Graph Toolkit

通过以下Toolkit安装 Microsoft Graph Toolkit npm 包和填充：

```bash
npm install @microsoft/mgt
```
如果计划在 Web 部件中支持 IE11，则需要执行其他步骤以确保跨浏览器兼容性：

1. 安装以下程序包：
```bash
npm install -D babel-loader @babel/core @babel/preset-env webpack
npm install -D @webcomponents/webcomponentsjs regenerator-runtime core-js
```

2. 将以下代码添加到 `gulpfile.js` 正上方 `build.initialize(gulp)` ：
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
3. 在文件中，在 SharePoint 提供程序下一步 `src\webparts\<your-project>\<your-web-part>.ts` 中导入以下填充。

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

Microsoft Graph Toolkit提供程序为组件启用身份验证并访问 Microsoft Graph。 若要了解更多信息，请参阅["使用提供程序"。](../providers/providers.md) SharePoint Web 部件始终存在于经过身份验证的上下文中，因为用户已经必须登录才能访问承载 Web 部件的页面。 使用此上下文初始化 [SharePoint 提供程序](../providers/sharepoint.md)。

首先，将提供程序添加到 Web 部件。 在项目文件夹中找到该文件，将以下行添加到文件顶部，位于现有语句 `src\webparts\<your-project>\<your-web-part>.ts` `import` 的正下方：

```ts
import { Providers, SharePointProvider } from '@microsoft/mgt';
```

接下来，您需要在 Web 部件的方法内使用经过身份验证的上下文初始化 `onInit()` 提供程序。 在同一文件中，将以下代码添加到该行 `public render(): void {` 的正前：

```ts
protected async onInit() {
    Providers.globalProvider = new SharePointProvider(this.context)
}
```

## <a name="add-components"></a>添加组件

现在，你可以开始向 Web 部件添加组件。 只需将组件添加到方法内的 HTML，组件将使用 `render()` SharePoint 上下文访问 Microsoft Graph。 例如，若要添加 [Person 组件](../components/person.md)，代码将如下所示：

```ts
public render(): void {
    this.domElement.innerHTML = `
      <mgt-person person-query="me" view="twolines"><mgt-person>
    `;
}
```

## <a name="configure-permissions"></a>配置权限

若要从 SharePoint 框架应用程序调用 Microsoft Graph，需要在解决方案包中请求所需的权限，并且 Microsoft 365 租户管理员需要批准请求的权限。

若要将权限添加到解决方案包，请找到并打开 `config\package-solution.json` 该文件并设置：

```json
"isDomainIsolated": false,
```

在该行正下方，添加以下内容：

```json
"webApiPermissionRequests":[],
```

根据你使用的组件确定你需要哪些 Microsoft Graph API 权限。 每个组件的文档页都提供组件所需的权限列表。 您需要将所需的每个权限添加到 `webApiPermissionRequests` 。 例如，如果你使用的是"人员"组件和"议程"组件，可能 `webApiPermissionRequests` 如下所示：

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
## <a name="build-and-deploy-your-web-part"></a>生成和部署 Web 部件

现在，将生成应用程序，并部署到 SharePoint。 通过运行以下命令生成应用程序：

```bash
gulp build
gulp bundle
gulp package-solution
```

该 `sharepoint/solution` 文件夹中有一个新 `.sppkg` 文件。 您需要将此文件上载到 SharePoint Online 应用程序目录。 转到 [SharePoint 管理中心的"更多功能"页](https://admin.microsoft.com/sharepoint?page=classicfeatures&modern=true)。 选择 **"应用程序****"下的"打开"，** 然后单击 **"应用程序目录****"，然后分发 SharePoint 应用程序**。 上载文件 `.sppkg` ，然后单击"部署 **"。**

接下来，您需要以管理员角色批准权限。

转到 **SharePoint 管理中心**。 在左侧导航栏中，选择 **"高级**"，然后选择 **"API Access"。** 应看到针对在文件中添加的每个权限的挂起 `config\package-solution.json` 请求。 选择并批准每个权限。

## <a name="test-your-web-part"></a>测试 Web 部件

现在可以将 Web 部件添加到 SharePoint 页面并进行测试。你将需要使用托管的工作台来测试使用 Microsoft Graph Toolkit因为组件需要经过身份验证的上下文才能调用 Microsoft Graph。 您可以在 **https：//<YOUR_TENANT>.sharepoint.com/_layouts/15/workbench.aspx** 找到托管的工作台。

打开项目中的文件，将值替换为托管工作台的 `config\serve.json` `initialPage` URL：
```json
"initialPage": "https://<YOUR_TENANT>.sharepoint.com/_layouts/15/workbench.aspx",
```
保存该文件，然后在控制台中运行以下命令以生成和预览 Web 部件：

```bash
gulp serve
```

托管的工作台将自动在浏览器中打开。 将 Web 部件添加到页面，你应该会看到你的 Web 部件与 Microsoft Graph Toolkit组件在操作！ 只要 gulp serve 命令仍在控制台中运行，就可以继续编辑代码，然后刷新浏览器以查看更改。

## <a name="next-steps"></a>后续步骤
- 请查看此有关生成 SharePoint Web 部件 [分步教程](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-9-microsoft-graph-toolkit-sharepoint-provider/)。
- 尝试在运动场 [中的组件](https://mgt.dev)。
- 在 Stack [Overflow](https://aka.ms/mgt-question)上提问。
- 在 GitHub 上报告 Bug 或保留 [功能请求](https://aka.ms/mgt)。