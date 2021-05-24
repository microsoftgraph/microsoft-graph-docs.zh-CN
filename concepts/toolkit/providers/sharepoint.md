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
# <a name="sharepoint-provider"></a><span data-ttu-id="6b626-103">SharePoint 提供程序</span><span class="sxs-lookup"><span data-stu-id="6b626-103">SharePoint provider</span></span>

<span data-ttu-id="6b626-104">使用 SharePoint Web 部件中的 SharePoint 提供程序为组件提供 Microsoft Graph访问权限。</span><span class="sxs-lookup"><span data-stu-id="6b626-104">Use the SharePoint provider inside your SharePoint web parts to power the components with Microsoft Graph access.</span></span>

<span data-ttu-id="6b626-105">若要了解有关身份验证提供程序的信息 [，请参阅提供程序](./providers.md)。</span><span class="sxs-lookup"><span data-stu-id="6b626-105">To learn more about authentication providers, see [Providers](./providers.md).</span></span>

## <a name="get-started"></a><span data-ttu-id="6b626-106">入门</span><span class="sxs-lookup"><span data-stu-id="6b626-106">Get started</span></span>

<span data-ttu-id="6b626-107">在 Web 部件 `onInit()` 的方法中初始化提供程序。</span><span class="sxs-lookup"><span data-stu-id="6b626-107">Initialize the provider inside the `onInit()` method of your web part.</span></span> <span data-ttu-id="6b626-108">此示例使用[ `@microsoft/mgt-spfx` 包](../get-started/mgt-spfx.md)。</span><span class="sxs-lookup"><span data-stu-id="6b626-108">This example uses the [`@microsoft/mgt-spfx` package](../get-started/mgt-spfx.md).</span></span>

```ts
// import the providers at the top of the page
import {Providers, SharePointProvider} from '@microsoft/mgt-spfx';

// add the onInit() method if not already there in your web part class
protected async onInit() {
  Providers.globalProvider = new SharePointProvider(this.context);
}
```

<span data-ttu-id="6b626-109">现在，可以在方法中添加任何组件，它将使用 SharePoint `render()` 上下文访问 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="6b626-109">Now you can add any component in your `render()` method and it will use the SharePoint context to access Microsoft Graph.</span></span>

```ts
public render(): void {
  this.domElement.innerHTML = `
    <mgt-agenda></mgt-agenda>
    `;
}
```

><span data-ttu-id="6b626-110">**注意：** Microsoft Graph Toolkit Typescript 3.7 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="6b626-110">**Note:** The Microsoft Graph Toolkit requires Typescript 3.7 or newer.</span></span> <span data-ttu-id="6b626-111">通过安装正确的编译器，确保 [你使用的是](https://github.com/SharePoint/sp-dev-docs/wiki/SharePoint-Framework-v1.8-release-notes#support-for-typescript-27-29-and-3x)支持的 Typescript 版本。</span><span class="sxs-lookup"><span data-stu-id="6b626-111">Make sure you're using a supported version of Typescript by [installing the right compiler](https://github.com/SharePoint/sp-dev-docs/wiki/SharePoint-Framework-v1.8-release-notes#support-for-typescript-27-29-and-3x).</span></span>

## <a name="sample"></a><span data-ttu-id="6b626-112">示例</span><span class="sxs-lookup"><span data-stu-id="6b626-112">Sample</span></span>

<span data-ttu-id="6b626-113">若要详细了解如何初始化 SharePoint 提供程序，请参阅生成SharePoint [Web](../get-started/build-a-sharepoint-web-part.md)部件入门指南。</span><span class="sxs-lookup"><span data-stu-id="6b626-113">For details about how to initialize the SharePoint provider, see the [Build a SharePoint web part](../get-started/build-a-sharepoint-web-part.md) getting started guide.</span></span>

## <a name="test-in-the-workbench"></a><span data-ttu-id="6b626-114">在工作台中测试</span><span class="sxs-lookup"><span data-stu-id="6b626-114">Test in the workbench</span></span>

<span data-ttu-id="6b626-115">如果你刚开始使用 web SharePoint，可以按照生成[首个 Web](/sharepoint/dev/spfx/web-parts/get-started/build-a-hello-world-web-part)部件指南。</span><span class="sxs-lookup"><span data-stu-id="6b626-115">If you're just getting started with SharePoint web parts, you can follow the [Build your first web part](/sharepoint/dev/spfx/web-parts/get-started/build-a-hello-world-web-part) guidance.</span></span>

<span data-ttu-id="6b626-116">创建 Web 部件并准备好使用这些组件后，你需要确保 Web 部件具有访问 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="6b626-116">After you've created a web part, and you're ready to use the components, you will need to make sure that your web part has the right permissions to access Microsoft Graph.</span></span> <span data-ttu-id="6b626-117">有关详细信息，请参阅使用[microsoft Graph中的SharePoint 框架。](/sharepoint/dev/spfx/use-aad-tutorial)</span><span class="sxs-lookup"><span data-stu-id="6b626-117">For details, see [Consume Microsoft Graph in the SharePoint Framework](/sharepoint/dev/spfx/use-aad-tutorial).</span></span>

<span data-ttu-id="6b626-118">简而言之，向 中添加正确的权限非常重要 `package-solution.json` 。</span><span class="sxs-lookup"><span data-stu-id="6b626-118">In short, it's important to add the right permission to your `package-solution.json`.</span></span> <span data-ttu-id="6b626-119">你需要将 Web 部件包上传到SharePoint管理员批准请求的权限。</span><span class="sxs-lookup"><span data-stu-id="6b626-119">You will need to upload a package of your web part to SharePoint and have an administrator approve the requested permissions.</span></span>

>[!TIP]
><span data-ttu-id="6b626-120">构建[SharePoint Web](../get-started/build-a-sharepoint-web-part.md#configure-permissions)部件入门指南提供了配置和批准权限的分步说明。</span><span class="sxs-lookup"><span data-stu-id="6b626-120">The [Build a SharePoint web part](../get-started/build-a-sharepoint-web-part.md#configure-permissions) getting started guide provides step-by-step instructions for configuring and approving permissions.</span></span>

><span data-ttu-id="6b626-121">**注意** ：如果不确定要添加哪些权限，每个组件的文档将包含它所需的全部权限。</span><span class="sxs-lookup"><span data-stu-id="6b626-121">**Note:** if you're not sure what permissions to add, the documentation for each component includes all the permissions it needs.</span></span>