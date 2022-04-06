---
title: 用于 Microsoft Graph 工具包 的 SharePoint 框架 库
description: 使用 Microsoft SharePoint 框架 库Graph Toolkit Microsoft Graph Toolkit解决方案SharePoint 框架 Microsoft 解决方案。
ms.localizationpriority: medium
author: sebastienlevert
ms.openlocfilehash: 952ff0852f4c1c0cf1efb2be2ab3cbe89d805f00
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2022
ms.locfileid: "64588790"
---
# <a name="sharepoint-framework-library-for-microsoft-graph-toolkit"></a>用于 Microsoft Graph 工具包 的 SharePoint 框架 库

使用 Microsoft SharePoint 框架 库Graph Toolkit Microsoft Graph Toolkit解决方案SharePoint 框架 Microsoft 解决方案。

若要防止多个组件在页面上注册自己的一组 Microsoft Graph Toolkit 组件，您应该将此库部署到租户，并引用您在此库中的解决方案中使用的 Microsoft Graph Toolkit 组件。

> [!CAUTION]
> Microsoft SharePoint 框架 库Graph Toolkit用于扩展SharePoint 框架 **非独立 Web 部件**。 如果你要生成独立 Web 部件，请不要使用 Microsoft SharePoint 框架库Graph Toolkit。 相反，如果你使用 Graph Toolkit程序包，请直接从 @microsoft/mgt (或 @microsoft/mgt-react React) Microsoft 应用。 SharePoint 框架不支持从独立 Web 部件引用库组件，这样做将导致独立 Web 部件中的运行时错误。

## <a name="installation"></a>安装

若要从Graph Toolkit`@microsoft/mgt-spfx`加载 Microsoft 组件，请作为运行时依赖项将程序包添加到你的SharePoint 框架项目中：

```bash
npm install @microsoft/mgt-spfx
```

或者

```bash
yarn add @microsoft/mgt-spfx
```

在将SharePoint 框架包`@microsoft/mgt-spfx`部署到租户之前，你需要将SharePoint 框架包部署到租户。 可以从项目上"`@microsoft/mgt-spfx`发布"部分下载与项目中使用的版本相对应的GitHub。[](https://github.com/microsoftgraph/microsoft-graph-toolkit/releases)

>[!IMPORTANT]
>由于租户中只能安装 Microsoft Graph 工具包 SharePoint 框架库的一个版本，因此在解决方案中使用 Microsoft Graph 工具包之前，请确定你的组织或客户是否已部署某 SharePoint 框架库版本并使用相同版本。

## <a name="usage"></a>用法

生成SharePoint 框架 Web 部件和扩展时，请引用 Microsoft Graph Toolkit`Provider`和`SharePointProvider`从程序包`@microsoft/mgt-spfx`。 这将确保你的解决方案将使用 Microsoft Graph Toolkit已在页面上注册的组件，而不是实例化自己的组件。 无论 Web 部件使用哪个 JavaScript 框架，实例化过程对于所有 Web 部件都是相同的。

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

使用框架（而非 React）生成 Web 部件时，可以直接在 Web 部件中加载组件：

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

### <a name="react"></a>React

如果正在使用 Web 部件生成 web React，可以使用 `@microsoft/mgt-react` 包。 但是，请确保从路径导入React组件`@microsoft/mgt-react/dist/es6/spfx`。 这将确保您的解决方案将仅使用 Microsoft Graph Toolkit已在页面上注册的组件，而不是实例化自己的组件。

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
> 确保解决方案Graph Toolkit导入的所有 Microsoft 产品都来自：
> * `@microsoft/mgt-spfx` 或
> * `@microsoft/mgt-react/dist/es6/spfx`
> 
> 不要从任何其他 Microsoft Graph Toolkit `@microsoft/mgt-*` 程序包 () ，以免打包自己的工具包副本并与其他 共享库。

## <a name="see-also"></a>另请参阅

* [使用 Microsoft Graph 工具包构建 SharePoint Web 部件](./build-a-sharepoint-web-part.md)
* [了解身份验证提供程序](../providers/providers.md)
