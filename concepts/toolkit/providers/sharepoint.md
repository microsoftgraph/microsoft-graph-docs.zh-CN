---
title: SharePoint 提供程序
description: 使用 SharePoint Web 部件中的 SharePoint 提供程序为组件提供 Microsoft Graph访问权限。
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: eb5e5c5935e51fe7574c41feb57700f473567707
ms.sourcegitcommit: 276a13a37c3772689dfc71f7cd47586c9581f27d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/24/2021
ms.locfileid: "52629124"
---
# <a name="sharepoint-provider"></a>SharePoint 提供程序

使用 SharePoint Web 部件中的 SharePoint 提供程序为组件提供 Microsoft Graph访问权限。

若要了解有关身份验证提供程序的信息 [，请参阅提供程序](./providers.md)。

## <a name="get-started"></a>入门

在 Web 部件 `onInit()` 的方法中初始化提供程序。 此示例使用[ `@microsoft/mgt-spfx` 包](../get-started/mgt-spfx.md)。

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

## <a name="test-in-the-workbench"></a>在工作台中测试

如果你刚开始使用 web SharePoint，可以按照生成[首个 Web](/sharepoint/dev/spfx/web-parts/get-started/build-a-hello-world-web-part)部件指南。

创建 Web 部件并准备好使用这些组件后，你需要确保 Web 部件具有访问 Microsoft Graph。 有关详细信息，请参阅使用[microsoft Graph中的SharePoint 框架。](/sharepoint/dev/spfx/use-aad-tutorial)

简而言之，向 中添加正确的权限非常重要 `package-solution.json` 。 你需要将 Web 部件包上传到SharePoint管理员批准请求的权限。

>[!TIP]
>构建[SharePoint Web](../get-started/build-a-sharepoint-web-part.md#configure-permissions)部件入门指南提供了配置和批准权限的分步说明。

>**注意** ：如果不确定要添加哪些权限，每个组件的文档将包含它所需的全部权限。