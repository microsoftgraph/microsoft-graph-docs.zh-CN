---
title: 使用 Microsoft SharePoint生成 web Graph Toolkit
description: 开始使用 Microsoft Graph Toolkit生成 SharePoint Web 部件。
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: c1f4be864c9e762e164980bc20abb4195df5c9f7
ms.sourcegitcommit: 276a13a37c3772689dfc71f7cd47586c9581f27d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/24/2021
ms.locfileid: "52629131"
---
# <a name="build-a-sharepoint-web-part-with-the-microsoft-graph-toolkit"></a>使用 Microsoft SharePoint生成 web Graph Toolkit

本主题介绍如何使用 Microsoft Graph Toolkit客户端 Web SharePoint[中的组件](/sharepoint/dev/spfx/web-parts/overview-client-side-web-parts)。 入门包括以下步骤：

1. 设置开发环境并创建 Web 部件。
1. 添加 Microsoft Graph Toolkit SharePoint 框架程序包。
1. 添加SharePoint提供程序。
1. 添加组件。
1. 配置权限。
1. 部署 Microsoft Graph Toolkit SharePoint 框架程序包。
1. 生成和部署 Web 部件。
1. 测试 Web 部件。

## <a name="set-up-your-sharepoint-framework-development-environment-and-create-a-new-web-part"></a>设置开发SharePoint 框架并创建新的 Web 部件

按照步骤设置[开发SharePoint 框架，](/sharepoint/dev/spfx/set-up-your-development-environment)然后[创建新的 Web 部件](/sharepoint/dev/spfx/web-parts/get-started/build-a-hello-world-web-part)。

## <a name="add-the-microsoft-graph-toolkit-sharepoint-framework-package"></a>添加 Microsoft Graph Toolkit SharePoint 框架包

若要防止多个 SharePoint 框架 组件在页面上注册自己的一组 Microsoft Graph Toolkit 组件，您应将 Microsoft Graph Toolkit SharePoint 框架 程序包部署到租户，并引用在此程序包的解决方案中使用的 Microsoft Graph Toolkit 组件。

Microsoft Graph Toolkit SharePoint 框架 包包含一个SharePoint 框架库，该库在 SharePoint 中注册 Microsoft Graph Toolkit 组件的单个实例。

使用下列Graph Toolkit SharePoint 框架安装 Microsoft Graph Toolkit SharePoint 框架 npm 包：

```bash
npm install @microsoft/mgt-spfx
```

## <a name="add-the-sharepoint-provider"></a>添加SharePoint提供程序

Microsoft Graph Toolkit提供程序支持对组件的 Microsoft Graph进行身份验证和访问。 若要了解更多信息，请参阅 [使用提供程序](../providers/providers.md)。 SharePoint Web 部件始终存在于经过身份验证的上下文中，因为用户已经必须登录才能访问托管 Web 部件的页面。 使用此上下文初始化SharePoint[提供程序](../providers/sharepoint.md)。

首先，将提供程序添加到 Web 部件。 在项目文件夹中找到文件，将以下行添加到文件顶部，位于现有语句 `src\webparts\<your-project>\<your-web-part>.ts` `import` 的正下方：

```ts
import { Providers, SharePointProvider } from '@microsoft/mgt-spfx';
```

接下来，你需要在 Web 部件的方法内使用经过身份验证的上下文初始化 `onInit()` 提供程序。 在同一文件中，将以下代码添加到 行 `public render(): void {` 的正前：

```ts
protected async onInit() {
  if (!Providers.globalProvider) {
    Providers.globalProvider = new SharePointProvider(this.context);
  }
}
```

## <a name="add-components"></a>添加组件

现在，你可以开始向 Web 部件添加组件。 只需将组件添加到 方法内的 HTML，组件将使用 SharePoint 上下文访问 `render()` Microsoft Graph。 例如，若要添加 [Person 组件](../components/person.md)，代码将如下所示：

```ts
public render(): void {
    this.domElement.innerHTML = `
      <mgt-person person-query="me" view="twolines"></mgt-person>
    `;
}
```

>[!NOTE]
> 如果要使用 web 部件生成 web React，请参阅[@microsoft/mgt-spfx](./mgt-spfx.md#react)文档，了解如何使用 `@microsoft/mgt-react` 。

## <a name="configure-permissions"></a>配置权限

若要从 Graph 应用程序调用 Microsoft SharePoint 框架，您需要在解决方案包中请求所需的权限，Microsoft 365租户管理员需要批准请求的权限。

若要将权限添加到解决方案包，请找到并打开 `config\package-solution.json` 文件并设置：

```json
"isDomainIsolated": false,
```

在该行正下方，添加以下内容：

```json
"webApiPermissionRequests":[],
```

根据你Graph，确定你需要哪些 Microsoft 应用 API 权限。 每个组件的文档页都提供组件所需的权限列表。 你需要将所需的每个权限添加到 `webApiPermissionRequests` 。 例如，如果你使用的是人员组件和议程组件，你可能 `webApiPermissionRequests` 如下所示：

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

## <a name="deploy-the-microsoft-graph-toolkit-sharepoint-framework-package"></a>部署 Microsoft Graph Toolkit SharePoint 框架 程序包

在将SharePoint 框架包部署到租户之前，你需要将 Microsoft Graph Toolkit SharePoint 框架包部署到租户。 可以从项目上的"发布"部分下载与Graph Toolkit Microsoft GitHub 版本相对应的程序包。 [](https://github.com/microsoftgraph/microsoft-graph-toolkit/releases)

>[!IMPORTANT]
>由于租户中只能安装 Microsoft Graph Toolkit 的 SharePoint 框架 库的一个版本，因此在解决方案中使用 Microsoft Graph Toolkit 之前，请确定组织或客户是否已部署并使用相同的版本的 SharePoint 框架 库。

下载 Microsoft Graph Toolkit SharePoint 框架 .sppkg 程序包后，将其上传到 SharePoint Online 应用目录。 转到管理[中心的更多功能SharePoint页面](https://admin.microsoft.com/sharepoint?page=classicfeatures&modern=true)。 选择 **"应用程序**"下的"打开 **"，** 然后单击"**应用程序** 目录"，然后分配 **SharePoint。** Upload文件 `.sppkg` ，然后单击"部署 **"。**

## <a name="build-and-deploy-your-web-part"></a>生成和部署 Web 部件

现在，将生成应用程序并部署到SharePoint。 通过运行以下命令构建应用程序：

```bash
gulp build
gulp bundle
gulp package-solution
```

在 `sharepoint/solution` 文件夹中，将会有一个新 `.sppkg` 文件。 你需要将此文件上载到 SharePoint Online 应用程序目录。 转到管理[中心的更多功能SharePoint页面](https://admin.microsoft.com/sharepoint?page=classicfeatures&modern=true)。 选择 **"应用程序**"下的"打开 **"，** 然后单击"**应用程序** 目录"，然后分配 **SharePoint。** Upload文件 `.sppkg` ，然后单击"部署 **"。**

接下来，您需要以管理员角色批准权限。

转到你的SharePoint **管理中心**。 在左侧导航栏中，选择 **"高级"，** 然后选择 **"API 访问"。** 应看到文件中添加的每个权限的挂起 `config\package-solution.json` 请求。 选择并批准每个权限。

## <a name="test-your-web-part"></a>测试 Web 部件

现在，你已准备好将 Web 部件添加到SharePoint并进行测试。你将需要使用托管的工作台来测试使用 Microsoft Graph Toolkit因为组件需要经过身份验证的上下文才能调用 Microsoft Graph。 可在 **https：//<YOUR_TENANT>.sharepoint.com/_layouts/15/workbench.aspx 找到托管的工作台**。

打开 `config\serve.json` 项目中的文件，将 的值替换为 `initialPage` 托管工作台的 url：
```json
"initialPage": "https://<YOUR_TENANT>.sharepoint.com/_layouts/15/workbench.aspx",
```
保存文件，然后在控制台中运行以下命令以生成和预览 Web 部件：

```bash
gulp serve
```

托管的工作台将自动在浏览器中打开。 将 Web 部件添加到页面，你应该会看到 Web 部件与 Microsoft Graph Toolkit组件在操作！ 只要 gulp serve 命令仍在控制台中运行，就可以继续编辑代码，然后仅刷新浏览器以查看更改。

## <a name="next-steps"></a>后续步骤
- 请查看此有关生成 web 部件SharePoint[分步教程](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-9-microsoft-graph-toolkit-sharepoint-provider/)。
- 尝试在运动场中的 [组件](https://mgt.dev)。
- 在 Stack [Overflow 上提问](https://aka.ms/mgt-question)。
- 报告 Bug 或将功能请求[保留GitHub。](https://aka.ms/mgt)
