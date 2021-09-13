---
title: 使用 Microsoft Graph 工具包构建 SharePoint Web 部件
description: 开始使用 Microsoft Graph 工具包构建 SharePoint Web 部件。
ms.localizationpriority: medium
author: elisenyang
ms.openlocfilehash: d30a2dd4fbaa89890124332528ed157e9043f8a9
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59083808"
---
# <a name="build-a-sharepoint-web-part-with-the-microsoft-graph-toolkit"></a>使用 Microsoft Graph 工具包构建 SharePoint Web 部件

本主题介绍如何在 [SharePoint 客户端 Web 部件](/sharepoint/dev/spfx/web-parts/overview-client-side-web-parts)中使用 Microsoft Graph 工具包组件。 开始使用涉及以下步骤：

1. 设置开发环境并创建 Web 部件。
1. 添加 Microsoft Graph 工具包 SharePoint 框架包。
1. 添加 SharePoint 提供程序。
1. 添加组件。
1. 配置权限。
1. 部署 Microsoft Graph 工具包 SharePoint 框架包。
1. 构建和部署 Web 部件。
1. 测试 Web 部件。

## <a name="set-up-your-sharepoint-framework-development-environment-and-create-a-new-web-part"></a>设置 SharePoint 框架开发环境并创建新的 Web 部件

按照步骤[设置 SharePoint 框架开发环境](/sharepoint/dev/spfx/set-up-your-development-environment)，然后[创建新的 Web 部件](/sharepoint/dev/spfx/web-parts/get-started/build-a-hello-world-web-part)。

## <a name="add-the-microsoft-graph-toolkit-sharepoint-framework-package"></a>添加 Microsoft Graph 工具包 SharePoint 框架包

为防止多个 SharePoint 框架组件在页面上注册自己的一组 Microsoft Graph 工具包组件，应该将 Microsoft Graph 工具包 SharePoint 框架包部署到你的租户，并从此包引用你在解决方案中使用的 Microsoft Graph 工具包组件。

Microsoft Graph 工具包 SharePoint 框架包包含 SharePoint 框架库，用于在 SharePoint 中注册 Microsoft Graph 工具包组件的单个实例。

使用以下命令安装 Microsoft Graph 工具包 SharePoint 框架 npm 包：

```bash
npm install @microsoft/mgt-spfx
```

## <a name="add-the-sharepoint-provider"></a>添加 SharePoint 提供程序

Microsoft Graph 工具包提供程序为组件启用身份验证和对 Microsoft Graph 的访问。 若要了解详细信息，请参阅[使用提供程序](../providers/providers.md)。 SharePoint Web 部件始终存在于经过身份验证的上下文中，因为用户必须登录才能访问托管 Web 部件的页面。 使用此上下文初始化 [SharePoint 提供程序](../providers/sharepoint.md)。

首先，将提供程序添加到 Web 部件。 在项目文件夹中找到 `src\webparts\<your-project>\<your-web-part>.ts` 文件，并将以下行添加到文件顶部，位于现有 `import` 语句的正下方：

```ts
import { Providers, SharePointProvider } from '@microsoft/mgt-spfx';
```

接下来，需要在 Web 部件的 `onInit()` 方法中使用经过身份验证的上下文初始化提供程序。 在同一文件中，在 `public render(): void {` 行之前添加以下代码：

```ts
protected async onInit() {
  if (!Providers.globalProvider) {
    Providers.globalProvider = new SharePointProvider(this.context);
  }
}
```

## <a name="add-components"></a>添加组件

现在，可以开始向 Web 部件添加组件。 只需将组件添加到 `render()` 方法内的 HTML，组件将使用 SharePoint 上下文访问Microsoft Graph。 例如，若要添加[“人员”组件](../components/person.md)，代码将如下所示：

```ts
public render(): void {
    this.domElement.innerHTML = `
      <mgt-person person-query="me" view="twolines"></mgt-person>
    `;
}
```

>[!NOTE]
> 如果使用 React 构建 Web 部件，请参阅 [@microsoft/mgt-spfx 文档](./mgt-spfx.md#react)了解如何使用 `@microsoft/mgt-react`。

## <a name="configure-permissions"></a>配置权限

若要从 SharePoint 框架应用程序调用 Microsoft Graph，你需要在解决方案包中请求所需的权限，Microsoft 365 租户管理员需要批准请求的权限。

若要将权限添加到解决方案包，请找到并打开 `config\package-solution.json` 文件，然后设置：

```json
"isDomainIsolated": false,
```

在该行正下方，添加以下内容：

```json
"webApiPermissionRequests":[],
```

根据使用的组件确定所需的 Microsoft Graph API 权限。 每个组件的文档页都提供组件所需的权限列表。 你需要将所需的每个权限添加到 `webApiPermissionRequests`。 例如，如果使用的是“人员”组件和“日程”组件，则 `webApiPermissionRequests` 可能如下所示：

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

## <a name="deploy-the-microsoft-graph-toolkit-sharepoint-framework-package"></a>部署 Microsoft Graph 工具包 SharePoint 框架包

在将 SharePoint 框架包部署到租户之前，需要将 Microsoft Graph 工具包 SharePoint 框架包部署到租户。 可以从 GitHub 上的“[版本](https://github.com/microsoftgraph/microsoft-graph-toolkit/releases)”部分下载与项目中使用的 Microsoft Graph 工具包版本相对应的包。

>[!IMPORTANT]
>由于租户中只能安装 Microsoft Graph 工具包 SharePoint 框架库的一个版本，因此在解决方案中使用 Microsoft Graph 工具包之前，请确定你的组织或客户是否已部署某 SharePoint 框架库版本并使用相同版本。

下载 Microsoft Graph 工具包 SharePoint 框架 .sppkg 包后，将其上传到你的 SharePoint Online 应用目录。 转到 [SharePoint 管理中心的“更多功能”页面](https://admin.microsoft.com/sharepoint?page=classicfeatures&modern=true)。 在“**应用**”下选择“**打开**”，然后单击“**应用程序目录**”和“**分发适用于 SharePoint 的应用程序**”。 上传 `.sppkg` 文件，然后单击“**部署**”。

## <a name="build-and-deploy-your-web-part"></a>构建和部署 Web 部件

现在，你将构建应用程序并将其部署到 SharePoint。 通过运行以下命令构建应用程序：

```bash
gulp build
gulp bundle
gulp package-solution
```

在 `sharepoint/solution` 文件夹中，将有一个新的 `.sppkg` 文件。 需要将此文件上传到 SharePoint Online 应用程序目录。 转到 [SharePoint 管理中心的“更多功能”页面](https://admin.microsoft.com/sharepoint?page=classicfeatures&modern=true)。 在“**应用**”下选择“**打开**”，然后单击“**应用程序目录**”和“**分发适用于 SharePoint 的应用程序**”。 上传 `.sppkg` 文件，然后单击“**部署**”。

接下来，需要以管理员身份批准权限。

转到 **SharePoint 管理中心**。 在左侧导航中，选择“**高级**”，然后选择“**API 访问**”。 你应该会看到你在 `config\package-solution.json` 文件中添加的每个权限的待处理请求。 选择并批准每个权限。

## <a name="test-your-web-part"></a>测试 Web 部件

你现在已准备好将 Web 部件添加到 SharePoint 页面并对其进行测试。你需要使用托管工作台来测试使用 Microsoft Graph 工具包的 Web 部件，因为组件需要经过身份验证的上下文才能调用 Microsoft Graph。 可以在 **https://<YOUR_TENANT>.sharepoint.com/_layouts/15/workbench.aspx** 找到托管工作台。

打开项目中的 `config\serve.json` 文件，并将 `initialPage` 的值替换为托管工作台的 url：
```json
"initialPage": "https://<YOUR_TENANT>.sharepoint.com/_layouts/15/workbench.aspx",
```
保存文件，然后在控制台中运行以下命令来构建和预览 Web 部件：

```bash
gulp serve
```

托管工作台将自动在浏览器中打开。 将 Web 部件添加到页面，你应该会看到带有 Microsoft Graph 工具包组件的 Web 部件正在运行！ 只要 gulp serve 命令仍在控制台中运行，你就可以继续编辑代码，然后刷新浏览器以查看更改。

## <a name="next-steps"></a>后续步骤
- 请查看此有关生成 web 部件SharePoint[分步教程](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-9-microsoft-graph-toolkit-sharepoint-provider/)。
- 在[样本](https://mgt.dev)中试用组件。
- 在 [Stack Overflow](https://aka.ms/mgt-question) 上提问。
- 在 [GitHub](https://aka.ms/mgt) 上报告 bug 或提出功能请求。
