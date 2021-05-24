---
title: SharePoint 框架 Microsoft Graph Toolkit
description: 使用 SharePoint 框架 Microsoft Graph Toolkit 库在解决方案Graph Toolkit Microsoft SharePoint 框架 Microsoft。
localization_priority: Normal
author: waldekmastykarz
ms.openlocfilehash: 5868f9fd523055d50f985f2fc8c8840563d56b28
ms.sourcegitcommit: 276a13a37c3772689dfc71f7cd47586c9581f27d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/24/2021
ms.locfileid: "52629488"
---
# <a name="sharepoint-framework-library-for-microsoft-graph-toolkit"></a><span data-ttu-id="bba2a-103">SharePoint 框架 Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="bba2a-103">SharePoint Framework library for Microsoft Graph Toolkit</span></span>

<span data-ttu-id="bba2a-104">使用 SharePoint 框架 Microsoft Graph Toolkit 库在解决方案Graph Toolkit Microsoft SharePoint 框架 Microsoft。</span><span class="sxs-lookup"><span data-stu-id="bba2a-104">Use the SharePoint Framework library for Microsoft Graph Toolkit to use Microsoft Graph Toolkit in SharePoint Framework solutions.</span></span>

<span data-ttu-id="bba2a-105">若要防止多个组件在页面上注册自己的一组 Microsoft Graph Toolkit 组件，您应该将此库部署到租户，并引用您在此库中的解决方案中使用的 Microsoft Graph Toolkit 组件。</span><span class="sxs-lookup"><span data-stu-id="bba2a-105">To prevent multiple components from registering their own set of Microsoft Graph Toolkit components on the page, you should deploy this library to your tenant and reference Microsoft Graph Toolkit components that you use in your solution from this library.</span></span>

## <a name="installation"></a><span data-ttu-id="bba2a-106">安装</span><span class="sxs-lookup"><span data-stu-id="bba2a-106">Installation</span></span>

<span data-ttu-id="bba2a-107">若要从Graph Toolkit加载 Microsoft 组件，请作为运行时依赖项将程序包添加到你的SharePoint 框架 `@microsoft/mgt-spfx` 项目中：</span><span class="sxs-lookup"><span data-stu-id="bba2a-107">To load Microsoft Graph Toolkit components from the library, add the `@microsoft/mgt-spfx` package as a runtime dependency to your SharePoint Framework project:</span></span>

```bash
npm install @microsoft/mgt-spfx
```

<span data-ttu-id="bba2a-108">或</span><span class="sxs-lookup"><span data-stu-id="bba2a-108">or</span></span>

```bash
yarn add @microsoft/mgt-spfx
```

<span data-ttu-id="bba2a-109">在将SharePoint 框架包部署到租户之前，你需要将SharePoint 框架 `@microsoft/mgt-spfx` 包部署到租户。</span><span class="sxs-lookup"><span data-stu-id="bba2a-109">Before deploying your SharePoint Framework package to your tenant, you will need to deploy the `@microsoft/mgt-spfx` SharePoint Framework package to your tenant.</span></span> <span data-ttu-id="bba2a-110">可以从项目发布部分下载与项目中使用的版本相对应的 `@microsoft/mgt-spfx` GitHub。 [](https://github.com/microsoftgraph/microsoft-graph-toolkit/releases)</span><span class="sxs-lookup"><span data-stu-id="bba2a-110">You can download the package corresponding to the version of `@microsoft/mgt-spfx` that you used in your project, from the [Releases](https://github.com/microsoftgraph/microsoft-graph-toolkit/releases) section on GitHub.</span></span>

>[!IMPORTANT]
><span data-ttu-id="bba2a-111">由于租户中只能安装 Microsoft Graph Toolkit 的 SharePoint 框架 库的一个版本，因此在解决方案中使用 Microsoft Graph Toolkit 之前，请确定组织或客户是否已部署并使用相同的版本的 SharePoint 框架 库。</span><span class="sxs-lookup"><span data-stu-id="bba2a-111">Because only one version of the SharePoint Framework library for Microsoft Graph Toolkit can be installed in the tenant, before you use the Microsoft Graph Toolkit in your solution, determine whether your organization or customer already has a version of the SharePoint Framework library deployed and use the same version.</span></span>

## <a name="usage"></a><span data-ttu-id="bba2a-112">用法</span><span class="sxs-lookup"><span data-stu-id="bba2a-112">Usage</span></span>

<span data-ttu-id="bba2a-113">生成SharePoint 框架 Web 部件和扩展时，请引用 Microsoft Graph Toolkit `Provider` `SharePointProvider` 和从 `@microsoft/mgt-spfx` 程序包。</span><span class="sxs-lookup"><span data-stu-id="bba2a-113">When building SharePoint Framework web parts and extensions, reference the Microsoft Graph Toolkit `Provider` and `SharePointProvider` from the `@microsoft/mgt-spfx` package.</span></span> <span data-ttu-id="bba2a-114">这将确保您的解决方案将使用 Microsoft Graph Toolkit已在页面上注册的组件，而不是实例化自己的组件。</span><span class="sxs-lookup"><span data-stu-id="bba2a-114">This will ensure that your solution will use Microsoft Graph Toolkit components that are already registered on the page, rather than instantiating its own.</span></span> <span data-ttu-id="bba2a-115">无论 Web 部件使用哪个 JavaScript 框架，实例化过程对于所有 Web 部件都是相同的。</span><span class="sxs-lookup"><span data-stu-id="bba2a-115">The instantiation process is the same for all web parts no matter which JavaScript framework they use.</span></span>

```ts
import { Providers, SharePointProvider } from '@microsoft/mgt-spfx';

// [...] trimmed for brevity

export default class MgtWebPart extends BaseClientSideWebPart<IMgtWebPartProps> {
  protected async onInit() {
    if (!Providers.globalProvider) {
      Providers.globalProvider = new SharePointProvider(this.context);
    }
  }

  // [...] trimmed for brevity
}
```

<span data-ttu-id="bba2a-116">使用框架（而非 React）生成 Web 部件时，可以直接在 Web 部件中加载组件：</span><span class="sxs-lookup"><span data-stu-id="bba2a-116">When building web parts using a framework other than React, you can load components directly in your web part:</span></span>

```ts
export default class MgtNoFrameworkWebPart extends BaseClientSideWebPart<IMgtNoFrameworkWebPartProps> {
  protected async onInit() {
    if (!Providers.globalProvider) {
      Providers.globalProvider = new SharePointProvider(this.context);
    }
  }

  public render(): void {
    this.domElement.innerHTML = `
      <div>
        <mgt-person person-query="me"></mgt-person>
      </div>`;
  }

  // [...] trimmed for brevity
}
```

### <a name="react"></a><span data-ttu-id="bba2a-117">React</span><span class="sxs-lookup"><span data-stu-id="bba2a-117">React</span></span>

<span data-ttu-id="bba2a-118">如果正在使用 Web 部件生成 web React，可以使用 `@microsoft/mgt-react` 包。</span><span class="sxs-lookup"><span data-stu-id="bba2a-118">If you're building a web part using React, you can use the `@microsoft/mgt-react` package.</span></span> <span data-ttu-id="bba2a-119">但是，请确保从路径导入React组件 `@microsoft/mgt-react/dist/es6/spfx` 。</span><span class="sxs-lookup"><span data-stu-id="bba2a-119">However, make sure to import all React components from the `@microsoft/mgt-react/dist/es6/spfx` path.</span></span> <span data-ttu-id="bba2a-120">这将确保你的解决方案将仅使用 Microsoft Graph Toolkit已在页面上注册的组件，而不是实例化自己的组件。</span><span class="sxs-lookup"><span data-stu-id="bba2a-120">This will ensure that your solution will only use Microsoft Graph Toolkit components that are already registered on the page, rather than instantiating its own.</span></span>

```tsx
import { Person } from '@microsoft/mgt-react/dist/es6/spfx';
import { ViewType } from '@microsoft/mgt-spfx';

// [...] trimmed for brevity

export default class MgtReact extends React.Component<IMgtReactProps, {}> {
  public render(): React.ReactElement<IMgtReactProps> {
    return (
      <div className={ styles.mgtReact }>
        <Person personQuery="me" view={ViewType.image}></Person>
      </div>
    );
  }
}
```

>[!IMPORTANT]
> <span data-ttu-id="bba2a-121">请确保解决方案Graph Toolkit导入的所有 Microsoft 网站都来自：</span><span class="sxs-lookup"><span data-stu-id="bba2a-121">Make sure all Microsoft Graph Toolkit imports in your solution are from either:</span></span>
> * <span data-ttu-id="bba2a-122">`@microsoft/mgt-spfx` 或 </span><span class="sxs-lookup"><span data-stu-id="bba2a-122">`@microsoft/mgt-spfx` or</span></span>
> * `@microsoft/mgt-react/dist/es6/spfx`
> 
> <span data-ttu-id="bba2a-123">不要从任何其他 Microsoft Graph Toolkit程序包 () ，以免打包自己的工具包副本并与其他 `@microsoft/mgt-*` 共享库。</span><span class="sxs-lookup"><span data-stu-id="bba2a-123">Do not import from any other Microsoft Graph Toolkit packages (`@microsoft/mgt-*`) to avoid packaging your own copy of the toolkit and colliding with the shared library.</span></span>

## <a name="see-also"></a><span data-ttu-id="bba2a-124">另请参阅</span><span class="sxs-lookup"><span data-stu-id="bba2a-124">See also</span></span>

* [<span data-ttu-id="bba2a-125">使用 Microsoft SharePoint生成 web Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="bba2a-125">Build a SharePoint web part with the Microsoft Graph Toolkit</span></span>](./build-a-sharepoint-web-part.md)
* [<span data-ttu-id="bba2a-126">了解身份验证提供程序</span><span class="sxs-lookup"><span data-stu-id="bba2a-126">Learn about authentication providers</span></span>](../providers/providers.md)
