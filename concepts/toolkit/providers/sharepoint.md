---
title: SharePoint 提供程序
description: 使用 SharePoint Web 部件中的 SharePoint 提供程序为组件提供 Microsoft Graph访问权限。
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: c052c3a5bc790b7e9e4316c4a8a8aac4d2d3d7dd
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579688"
---
# <a name="sharepoint-provider"></a>SharePoint 提供程序

使用 SharePoint Web 部件中的 SharePoint 提供程序为组件提供 Microsoft Graph访问权限。

若要了解有关身份验证提供程序的信息 [，请参阅提供程序](./providers.md)。

## <a name="get-started"></a>入门

在 Web 部件 `onInit()` 的方法中初始化提供程序。

```ts
// import the providers at the top of the page
import {Providers, SharePointProvider} from '@microsoft/mgt-spfx';

// add the onInit() method if not already there in your web part class
protected async onInit() {
  Providers.globalProvider = new SharePointProvider(this.context);
}
```

现在，可以在方法中添加任何组件，它将使用 SharePoint `render()` 上下文访问 Microsoft Graph。

```ts
public render(): void {
  this.domElement.innerHTML = `
    <mgt-agenda></mgt-agenda>
    `;
}
```

>**注意：** Microsoft Graph Toolkit Typescript 3.7 或更高版本。 通过安装正确的编译器，确保 [你使用的是](https://github.com/SharePoint/sp-dev-docs/wiki/SharePoint-Framework-v1.8-release-notes#support-for-typescript-27-29-and-3x)支持的 Typescript 版本。

## <a name="sample"></a>示例

若要详细了解如何初始化 SharePoint 提供程序，请参阅生成SharePoint [Web](../get-started/build-a-sharepoint-web-part.md)部件入门指南。

有关展示如何使用 SharePoint Web 部件中各种组件的预建示例，请参阅 Microsoft SharePoint [web](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/sp-webpart)部件库中的 Graph Toolkit 示例。

## <a name="test-in-the-workbench"></a>在工作台中测试

如果你刚开始使用 web SharePoint，可以按照生成[首个 Web](/sharepoint/dev/spfx/web-parts/get-started/build-a-hello-world-web-part)部件指南。

创建 Web 部件并准备好使用这些组件后，你需要确保 Web 部件具有访问 Microsoft Graph。 有关详细信息，请参阅使用[microsoft Graph中的SharePoint 框架。](/sharepoint/dev/spfx/use-aad-tutorial)

简而言之，向 中添加正确的权限非常重要 `package-solution.json` 。 你需要将 Web 部件包上传到SharePoint管理员批准请求的权限。

>[!TIP]
>构建[SharePoint Web](../get-started/build-a-sharepoint-web-part.md#configure-permissions)部件入门指南提供了配置和批准权限的分步说明。

>**注意** ：如果不确定要添加哪些权限，每个组件的文档将包含它所需的全部权限。

## <a name="polyfills"></a>Polyfills

如果计划在 Web 部件中支持 IE11 SPFx，则必须使用填充。

若要了解更多信息，请参阅[Microsoft Graph Toolkit 入门](../get-started/overview.md#polyfills)。
