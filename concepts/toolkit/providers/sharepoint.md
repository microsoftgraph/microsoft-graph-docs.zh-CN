---
title: SharePoint 提供程序
description: 使用 SharePoint Web 部件中的 SharePoint 提供程序为组件提供 Microsoft Graph 访问权限。
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: bb657e8fb5d6d9a775fb41e5c5c9fa6bf4662926
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49657294"
---
# <a name="sharepoint-provider"></a>SharePoint 提供程序

使用 SharePoint Web 部件中的 SharePoint 提供程序为组件提供 Microsoft Graph 访问权限。

若要了解有关身份验证提供程序的信息，请参阅"[提供程序"。](./providers.md)

## <a name="get-started"></a>入门

在 Web 部件 `onInit()` 的方法内初始化提供程序。

```ts

// import the providers at the top of the page
import {Providers, SharePointProvider} from '@microsoft/mgt';

// add the onInit() method if not already there in your web part class
protected async onInit() {
    Providers.globalProvider = new SharePointProvider(this.context);
}
```

现在可以在方法中添加任何组件，它将 `render()` 使用 SharePoint 上下文访问 Microsoft Graph。

```ts

public render(): void {
    this.domElement.innerHTML = `
      <mgt-agenda></mgt-agenda>
      `;
  }
```

>**注意：** Microsoft Graph Toolkit Typescript 3.x。 通过安装正确的编译器，确保你使用的是支持的 Typescript [版本](https://github.com/SharePoint/sp-dev-docs/wiki/SharePoint-Framework-v1.8-release-notes#support-for-typescript-27-29-and-3x)。

## <a name="sample"></a>示例

若要详细了解如何初始化 SharePoint 提供程序，请参阅"生成 [SharePoint Web](../get-started/build-a-sharepoint-web-part.md) 部件入门指南"。

有关展示如何使用 SharePoint Web 部件中各种组件的预建示例，请参阅 Microsoft Graph Toolkit存储库中的 [SharePoint](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/sp-webpart) Web 部件示例。

## <a name="test-in-the-workbench"></a>在工作台中测试

如果刚开始使用 SharePoint Web 部件，可以按照"生成第一个 Web 部件"[指南。](/sharepoint/dev/spfx/web-parts/get-started/build-a-hello-world-web-part)

创建 Web 部件并准备好使用这些组件后，需要确保您的 Web 部件具有访问 Microsoft Graph 的合适权限。 有关详细信息，请参阅[在 SharePoint 框架中使用 Microsoft Graph。](/sharepoint/dev/spfx/use-aad-tutorial)

简而言之，向您的添加正确的权限非常重要 `package-solution.json` 。 您需要将 Web 部件包上载到 SharePoint，并让管理员批准请求的权限。

>[!TIP]
>" [生成 SharePoint Web](../get-started/build-a-sharepoint-web-part.md#configure-permissions) 部件入门指南"提供有关配置和批准权限的分步说明。

>**注意** ：如果不确定要添加哪些权限，每个组件的文档将包含它所需的全部权限。

## <a name="polyfills"></a>填充

如果计划在 SPFx Web 部件中支持 IE11，则必须使用填充。

若要了解更多信息，请参阅 [Microsoft Graph](../get-started/overview.md#polyfills)Toolkit。
