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
# <a name="sharepoint-provider"></a><span data-ttu-id="74dae-103">SharePoint 提供程序</span><span class="sxs-lookup"><span data-stu-id="74dae-103">SharePoint provider</span></span>

<span data-ttu-id="74dae-104">使用 SharePoint Web 部件中的 SharePoint 提供程序为组件提供 Microsoft Graph 访问权限。</span><span class="sxs-lookup"><span data-stu-id="74dae-104">Use the SharePoint provider inside your SharePoint web parts to power the components with Microsoft Graph access.</span></span>

<span data-ttu-id="74dae-105">若要了解有关身份验证提供程序的信息，请参阅"[提供程序"。](./providers.md)</span><span class="sxs-lookup"><span data-stu-id="74dae-105">To learn more about authentication providers, see [Providers](./providers.md).</span></span>

## <a name="get-started"></a><span data-ttu-id="74dae-106">入门</span><span class="sxs-lookup"><span data-stu-id="74dae-106">Get started</span></span>

<span data-ttu-id="74dae-107">在 Web 部件 `onInit()` 的方法内初始化提供程序。</span><span class="sxs-lookup"><span data-stu-id="74dae-107">Initialize the provider inside the `onInit()` method of your web part.</span></span>

```ts

// import the providers at the top of the page
import {Providers, SharePointProvider} from '@microsoft/mgt';

// add the onInit() method if not already there in your web part class
protected async onInit() {
    Providers.globalProvider = new SharePointProvider(this.context);
}
```

<span data-ttu-id="74dae-108">现在可以在方法中添加任何组件，它将 `render()` 使用 SharePoint 上下文访问 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="74dae-108">Now you can add any component in your `render()` method and it will use the SharePoint context to access Microsoft Graph.</span></span>

```ts

public render(): void {
    this.domElement.innerHTML = `
      <mgt-agenda></mgt-agenda>
      `;
  }
```

><span data-ttu-id="74dae-109">**注意：** Microsoft Graph Toolkit Typescript 3.x。</span><span class="sxs-lookup"><span data-stu-id="74dae-109">**Note:** The Microsoft Graph Toolkit requires Typescript 3.x.</span></span> <span data-ttu-id="74dae-110">通过安装正确的编译器，确保你使用的是支持的 Typescript [版本](https://github.com/SharePoint/sp-dev-docs/wiki/SharePoint-Framework-v1.8-release-notes#support-for-typescript-27-29-and-3x)。</span><span class="sxs-lookup"><span data-stu-id="74dae-110">Make sure you're using a supported version of Typescript by [installing the right compiler](https://github.com/SharePoint/sp-dev-docs/wiki/SharePoint-Framework-v1.8-release-notes#support-for-typescript-27-29-and-3x).</span></span>

## <a name="sample"></a><span data-ttu-id="74dae-111">示例</span><span class="sxs-lookup"><span data-stu-id="74dae-111">Sample</span></span>

<span data-ttu-id="74dae-112">若要详细了解如何初始化 SharePoint 提供程序，请参阅"生成 [SharePoint Web](../get-started/build-a-sharepoint-web-part.md) 部件入门指南"。</span><span class="sxs-lookup"><span data-stu-id="74dae-112">For details about how to initalize the SharePoint provider, see the [Build a SharePoint web part](../get-started/build-a-sharepoint-web-part.md) getting started guide.</span></span>

<span data-ttu-id="74dae-113">有关展示如何使用 SharePoint Web 部件中各种组件的预建示例，请参阅 Microsoft Graph Toolkit存储库中的 [SharePoint](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/sp-webpart) Web 部件示例。</span><span class="sxs-lookup"><span data-stu-id="74dae-113">For a pre-built example that shows you how to use the various components in your SharePoint web parts, see the [SharePoint web part sample](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/sp-webpart) in the Microsoft Graph Toolkit repository.</span></span>

## <a name="test-in-the-workbench"></a><span data-ttu-id="74dae-114">在工作台中测试</span><span class="sxs-lookup"><span data-stu-id="74dae-114">Test in the workbench</span></span>

<span data-ttu-id="74dae-115">如果刚开始使用 SharePoint Web 部件，可以按照"生成第一个 Web 部件"[指南。](/sharepoint/dev/spfx/web-parts/get-started/build-a-hello-world-web-part)</span><span class="sxs-lookup"><span data-stu-id="74dae-115">If you're just getting started with SharePoint web parts, you can follow the [Build your first web part](/sharepoint/dev/spfx/web-parts/get-started/build-a-hello-world-web-part) guidance.</span></span>

<span data-ttu-id="74dae-116">创建 Web 部件并准备好使用这些组件后，需要确保您的 Web 部件具有访问 Microsoft Graph 的合适权限。</span><span class="sxs-lookup"><span data-stu-id="74dae-116">After you've created a web part, and you're ready to use the components, you will need to make sure that your web part has the right permissions to access Microsoft Graph.</span></span> <span data-ttu-id="74dae-117">有关详细信息，请参阅[在 SharePoint 框架中使用 Microsoft Graph。](/sharepoint/dev/spfx/use-aad-tutorial)</span><span class="sxs-lookup"><span data-stu-id="74dae-117">For details, see [Consume Microsoft Graph in the SharePoint Framework](/sharepoint/dev/spfx/use-aad-tutorial).</span></span>

<span data-ttu-id="74dae-118">简而言之，向您的添加正确的权限非常重要 `package-solution.json` 。</span><span class="sxs-lookup"><span data-stu-id="74dae-118">In short, it's important to add the right permission to your `package-solution.json`.</span></span> <span data-ttu-id="74dae-119">您需要将 Web 部件包上载到 SharePoint，并让管理员批准请求的权限。</span><span class="sxs-lookup"><span data-stu-id="74dae-119">You will need to upload a package of your web part to SharePoint and have an administrator approve the requested permissions.</span></span>

>[!TIP]
><span data-ttu-id="74dae-120">" [生成 SharePoint Web](../get-started/build-a-sharepoint-web-part.md#configure-permissions) 部件入门指南"提供有关配置和批准权限的分步说明。</span><span class="sxs-lookup"><span data-stu-id="74dae-120">The [Build a SharePoint web part](../get-started/build-a-sharepoint-web-part.md#configure-permissions) getting started guide provides step-by-step instructions for configuring and approving permissions.</span></span>

><span data-ttu-id="74dae-121">**注意** ：如果不确定要添加哪些权限，每个组件的文档将包含它所需的全部权限。</span><span class="sxs-lookup"><span data-stu-id="74dae-121">**Note:** if you're not sure what permissions to add, the documentation for each component includes all the permissions it needs.</span></span>

## <a name="polyfills"></a><span data-ttu-id="74dae-122">填充</span><span class="sxs-lookup"><span data-stu-id="74dae-122">Polyfills</span></span>

<span data-ttu-id="74dae-123">如果计划在 SPFx Web 部件中支持 IE11，则必须使用填充。</span><span class="sxs-lookup"><span data-stu-id="74dae-123">If you plan to support IE11 in your SPFx webparts, you must use polyfills.</span></span>

<span data-ttu-id="74dae-124">若要了解更多信息，请参阅 [Microsoft Graph](../get-started/overview.md#polyfills)Toolkit。</span><span class="sxs-lookup"><span data-stu-id="74dae-124">To learn more, see [Getting started with Microsoft Graph Toolkit](../get-started/overview.md#polyfills).</span></span>
