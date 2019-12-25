---
title: SharePoint 提供程序
description: 使用 SharePoint web 部件中的 SharePoint 提供程序为组件提供 Microsoft Graph 访问的功能。
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 74605fa4c2acc2919a73f7b6bef1460480883c34
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40868546"
---
# <a name="sharepoint-provider"></a><span data-ttu-id="cb0e9-103">SharePoint 提供程序</span><span class="sxs-lookup"><span data-stu-id="cb0e9-103">SharePoint provider</span></span>

<span data-ttu-id="cb0e9-104">使用 SharePoint web 部件中的 SharePoint 提供程序为组件提供 Microsoft Graph 访问的功能。</span><span class="sxs-lookup"><span data-stu-id="cb0e9-104">Use the SharePoint provider inside your SharePoint web parts to power the components with Microsoft Graph access.</span></span>

<span data-ttu-id="cb0e9-105">若要了解详细信息，请参阅[提供程序](../providers.md)。</span><span class="sxs-lookup"><span data-stu-id="cb0e9-105">To learn more, see [Providers](../providers.md).</span></span>

## <a name="get-started"></a><span data-ttu-id="cb0e9-106">入门</span><span class="sxs-lookup"><span data-stu-id="cb0e9-106">Get started</span></span>

<span data-ttu-id="cb0e9-107">在 web 部件的`onInit()`方法内初始化提供程序。</span><span class="sxs-lookup"><span data-stu-id="cb0e9-107">Initialize the provider inside the `onInit()` method of your web part.</span></span>

```ts

// import the providers at the top of the page
import {Providers, SharePointProvider} from '@microsoft/mgt/dist/commonjs';

// add the onInit() method if not already there in your web part class
protected async onInit() {
    Providers.globalProvider = new SharePointProvider(this.context);
}
```

<span data-ttu-id="cb0e9-108">现在您可以在`render()`方法中添加任何组件，它将使用 SharePoint 上下文来访问 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="cb0e9-108">Now you can add any component in your `render()` method and it will use the SharePoint context to access Microsoft Graph.</span></span>

```ts

public render(): void {
    this.domElement.innerHTML = `
      <mgt-agenda></mgt-agenda>
      `;
  }
```

><span data-ttu-id="cb0e9-109">**注意：** Microsoft Graph 工具包需要 Typescript 3. x。</span><span class="sxs-lookup"><span data-stu-id="cb0e9-109">**Note:** The Microsoft Graph Toolkit requires Typescript 3.x.</span></span> <span data-ttu-id="cb0e9-110">请确保您使用的是受支持的 Typescript 版本，方法是[安装正确的编译器](https://github.com/SharePoint/sp-dev-docs/wiki/SharePoint-Framework-v1.8-release-notes#support-for-typescript-27-29-and-3x)。</span><span class="sxs-lookup"><span data-stu-id="cb0e9-110">Make sure you're using a supported version of Typescript by [installing the right compiler](https://github.com/SharePoint/sp-dev-docs/wiki/SharePoint-Framework-v1.8-release-notes#support-for-typescript-27-29-and-3x).</span></span>

## <a name="sample"></a><span data-ttu-id="cb0e9-111">示例</span><span class="sxs-lookup"><span data-stu-id="cb0e9-111">Sample</span></span>

<span data-ttu-id="cb0e9-112">有关演示如何使用 SharePoint web 部件中的各种组件的示例，请参阅 Microsoft Graph 工具包存储库中的[SharePoint web 部件示例](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/sp-webpart)。</span><span class="sxs-lookup"><span data-stu-id="cb0e9-112">For an example that shows you how to use the various components in your SharePoint web parts, see the [SharePoint webpart sample](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/sp-webpart) in the Microsoft Graph Toolkit repository.</span></span>

## <a name="test-in-the-workbench"></a><span data-ttu-id="cb0e9-113">在工作台中测试</span><span class="sxs-lookup"><span data-stu-id="cb0e9-113">Test in the workbench</span></span>

<span data-ttu-id="cb0e9-114">如果只是开始使用 SharePoint web 部件，可以按照[生成第一个 web 部件](https://docs.microsoft.com/sharepoint/dev/spfx/web-parts/get-started/build-a-hello-world-web-part)指南操作。</span><span class="sxs-lookup"><span data-stu-id="cb0e9-114">If you're just getting started with SharePoint web parts, you can follow the [Build your first web part](https://docs.microsoft.com/sharepoint/dev/spfx/web-parts/get-started/build-a-hello-world-web-part) guidance.</span></span>

<span data-ttu-id="cb0e9-115">在创建 web 部件并准备好使用组件之后，您需要确保您的 web 部件具有访问 Microsoft Graph 的适当权限。</span><span class="sxs-lookup"><span data-stu-id="cb0e9-115">After you've created a web part, and you're ready to use the components, you will need to make sure that your web part has the right permissions to access Microsoft Graph.</span></span> <span data-ttu-id="cb0e9-116">有关详细信息，请参阅[在 SharePoint 框架中使用 Microsoft Graph](/sharepoint/dev/spfx/use-aad-tutorial)。</span><span class="sxs-lookup"><span data-stu-id="cb0e9-116">For details, see [Consume Microsoft Graph in the SharePoint Framework](/sharepoint/dev/spfx/use-aad-tutorial).</span></span>

<span data-ttu-id="cb0e9-117">简言之，向添加适当的权限非常重要`package-solution.json`。</span><span class="sxs-lookup"><span data-stu-id="cb0e9-117">In short, it's important to add the right permission to your `package-solution.json`.</span></span> <span data-ttu-id="cb0e9-118">您需要将 web 部件包上传到 SharePoint，并让管理员批准请求的权限。</span><span class="sxs-lookup"><span data-stu-id="cb0e9-118">You will need to upload a package of your web part to SharePoint and have an administrator approve the requested permissions.</span></span>

><span data-ttu-id="cb0e9-119">**提示：** 如果你不确定要添加的权限，每个组件的文档都包含所需的所有权限。</span><span class="sxs-lookup"><span data-stu-id="cb0e9-119">**Tip:** if you're not sure what permissions to add, the documentation for each component includes all the permissions it needs.</span></span>
