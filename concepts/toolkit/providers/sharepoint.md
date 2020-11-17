---
title: SharePoint 提供程序
description: 使用 SharePoint web 部件中的 SharePoint 提供程序为组件提供 Microsoft Graph 访问的功能。
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: c27a24ac1b5f41b97d749620edbae09794072bed
ms.sourcegitcommit: 186d738f04e5a558da423f2429165fb4fbe780aa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086747"
---
# <a name="sharepoint-provider"></a>SharePoint 提供程序

使用 SharePoint web 部件中的 SharePoint 提供程序为组件提供 Microsoft Graph 访问的功能。

若要了解有关身份验证提供程序的详细信息，请参阅 [提供程序](../providers.md)。

## <a name="get-started"></a>入门

在 web 部件的方法内初始化提供程序 `onInit()` 。

```ts

// import the providers at the top of the page
import {Providers, SharePointProvider} from '@microsoft/mgt';

// add the onInit() method if not already there in your web part class
protected async onInit() {
    Providers.globalProvider = new SharePointProvider(this.context);
}
```

现在您可以在方法中添加任何组件 `render()` ，它将使用 SharePoint 上下文来访问 Microsoft Graph。

```ts

public render(): void {
    this.domElement.innerHTML = `
      <mgt-agenda></mgt-agenda>
      `;
  }
```

>**注意：** Microsoft Graph 工具包需要 Typescript 3. x。 请确保您使用的是受支持的 Typescript 版本，方法是 [安装正确的编译器](https://github.com/SharePoint/sp-dev-docs/wiki/SharePoint-Framework-v1.8-release-notes#support-for-typescript-27-29-and-3x)。

## <a name="sample"></a>示例

有关如何 initalize SharePoint 提供程序的详细信息，请参阅 [Build a sharepoint web part](../get-started/build-a-sharepoint-web-part.md) 入门指南。

有关演示如何使用 SharePoint web 部件中的各种组件的预构建示例，请参阅 Microsoft Graph 工具包存储库中的 [SharePoint web 部件示例](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/sp-webpart) 。

## <a name="test-in-the-workbench"></a>在工作台中测试

如果只是开始使用 SharePoint web 部件，可以按照 [生成第一个 web 部件](/sharepoint/dev/spfx/web-parts/get-started/build-a-hello-world-web-part) 指南操作。

在创建 web 部件并准备好使用组件之后，您需要确保您的 web 部件具有访问 Microsoft Graph 的适当权限。 有关详细信息，请参阅 [在 SharePoint 框架中使用 Microsoft Graph](/sharepoint/dev/spfx/use-aad-tutorial)。

简言之，向添加适当的权限非常重要 `package-solution.json` 。 您需要将 web 部件包上传到 SharePoint，并让管理员批准请求的权限。

>[!TIP]
>" [构建 SharePoint web 部件](../get-started/build-a-sharepoint-web-part.md#configure-permissions) 入门指南" 提供了有关配置和批准权限的分步说明。

>**注意：** 如果你不确定要添加的权限，每个组件的文档都包含所需的所有权限。

## <a name="polyfills"></a>Polyfills.ts

如果您计划在 SPFx web 部件中支持 IE11，则必须使用 polyfills.ts。

若要了解详细信息，请参阅 [Microsoft Graph 工具包入门](../get-started/overview.md#polyfills)。
