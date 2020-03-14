---
title: Microsoft Graph 工具包入门
description: 开始在应用程序中使用 Microsoft 工具包。
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: 1537a686d25d885a898603ca576f688abdaab3e4
ms.sourcegitcommit: f2dffaca3e1c5b74a01b59e1b76dba1592a6a5d1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/14/2020
ms.locfileid: "42639931"
---
# <a name="get-started-with-the-microsoft-graph-toolkit"></a><span data-ttu-id="1194b-103">Microsoft Graph 工具包入门</span><span class="sxs-lookup"><span data-stu-id="1194b-103">Get started with the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="1194b-104">可以轻松地将 Microsoft Graph 工具包包含在 web 应用程序、SharePoint web 部件或 Microsoft "团队" 选项卡中。这些组件基于现有的 web 标准构建，并与任何 web 框架和新式浏览器兼容。</span><span class="sxs-lookup"><span data-stu-id="1194b-104">The Microsoft Graph Toolkit can easily be included in your web application, SharePoint web part, or Microsoft Teams tab. The components are built on existing web standards and are compatible with any web framework and modern browser.</span></span> <span data-ttu-id="1194b-105">本主题介绍如何开始在项目中使用 Microsoft Graph 工具包。</span><span class="sxs-lookup"><span data-stu-id="1194b-105">This topic describes how to get started using the Microsoft Graph Toolkit in your project.</span></span>

> [!VIDEO https://www.youtube-nocookie.com/embed/oZCGb2MMxa0]

<span data-ttu-id="1194b-106">您可以通过直接引用加载程序（通过 unpkg）或安装 npm 程序包，在应用程序中使用 Microsoft Graph 工具包。</span><span class="sxs-lookup"><span data-stu-id="1194b-106">You can use the Microsoft Graph Toolkit in your application by referencing the loader directly (via unpkg), or by installing the npm package.</span></span>

## <a name="use-via-mgt-loader"></a><span data-ttu-id="1194b-107">通过预加载加载程序使用</span><span class="sxs-lookup"><span data-stu-id="1194b-107">Use via mgt-loader</span></span>

<span data-ttu-id="1194b-108">若要通过预加载加载程序使用该工具包，请参阅以下示例。</span><span class="sxs-lookup"><span data-stu-id="1194b-108">To use the toolkit via mgt-loader, see the following example.</span></span>

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
```

<span data-ttu-id="1194b-109">然后，您可以开始在 HTML 页面中使用这些组件。</span><span class="sxs-lookup"><span data-stu-id="1194b-109">You can then start using the components in your HTML page.</span></span> <span data-ttu-id="1194b-110">下面是 MSAL 提供程序的完整工作示例。</span><span class="sxs-lookup"><span data-stu-id="1194b-110">The following is a full working example with the MSAL provider.</span></span>

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal-provider client-id="[CLIENT-ID]"></mgt-msal-provider>
<mgt-login></mgt-login>

<!-- <script>
    // alternatively, you can set the provider in code and provide more options
    mgt.Providers.globalProvider = new mgt.MsalProvider({clientId: '[CLIENT-ID]'});
</script> -->
```

> <span data-ttu-id="1194b-111">**注意：** MSAL 要求将页面托管在用于身份验证重定向的 web 服务器中。</span><span class="sxs-lookup"><span data-stu-id="1194b-111">**Note:** MSAL requires the page to be hosted in a web server for the authentication redirects.</span></span> <span data-ttu-id="1194b-112">如果只是开始并且想要进行播放，可以在 Visual Studio Code 中使用[live server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) 。</span><span class="sxs-lookup"><span data-stu-id="1194b-112">If you're just getting started and want to play around, you can use [live server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) in Visual Studio Code.</span></span>

## <a name="use-via-npm-es6-modules"></a><span data-ttu-id="1194b-113">通过 NPM （es6 模块）使用</span><span class="sxs-lookup"><span data-stu-id="1194b-113">Use via NPM (es6 modules)</span></span>

<span data-ttu-id="1194b-114">通过使用 es6 模块，可以完全控制捆绑过程，并且可以仅捆绑网站所需的代码。</span><span class="sxs-lookup"><span data-stu-id="1194b-114">By using the es6 modules, you have full control of the bundling process and you can bundle only the code you need for your site.</span></span> <span data-ttu-id="1194b-115">首先，添加 npm 包：</span><span class="sxs-lookup"><span data-stu-id="1194b-115">First, add the npm package:</span></span>

```bash
npm install @microsoft/mgt
```

<span data-ttu-id="1194b-116">现在，您可以引用正在使用的页面上的所有组件：</span><span class="sxs-lookup"><span data-stu-id="1194b-116">Now you can reference all components at the page you are using:</span></span>

```html
<script src="node_modules/@microsoft/mgt/dist/es6/components.js"></script>
```

<span data-ttu-id="1194b-117">或者，只引用所需的组件，避免加载其他所有内容：</span><span class="sxs-lookup"><span data-stu-id="1194b-117">Or, just reference the component you need and avoid loading everything else:</span></span>

```html
<script src="node_modules/@microsoft/mgt/dist/es6/components/mgt-login/mgt-login.js"></script>
```

<span data-ttu-id="1194b-118">同样，若要添加提供程序，可以将其添加为组件：</span><span class="sxs-lookup"><span data-stu-id="1194b-118">Similarly, to add a provider, you can add it as a component:</span></span>

```html
<script src="node_modules/@microsoft/mgt/dist/es6/components/providers/mgt-msal-provider.js"></script>

<mgt-msal-provider client-id="[CLIENT-ID]"></mgt-msal-provider>
```

<span data-ttu-id="1194b-119">或者，将其添加到代码中：</span><span class="sxs-lookup"><span data-stu-id="1194b-119">Or, add it in your code:</span></span>

```html
<script type="module">
  import { Providers, MsalProvider } from '@microsoft/mgt';

  Providers.globalProvider = new MsalProvider({ clientId: '[CLIENT-ID]' });
</script>
```

## <a name="providers"></a><span data-ttu-id="1194b-120">提供程序</span><span class="sxs-lookup"><span data-stu-id="1194b-120">Providers</span></span>

<span data-ttu-id="1194b-121">与[提供程序](./providers.md)配合使用时，组件的工作效果最佳。</span><span class="sxs-lookup"><span data-stu-id="1194b-121">The components work best when used with a [provider](./providers.md).</span></span> <span data-ttu-id="1194b-122">提供程序公开了组件用来调用 Microsoft Graph 的身份验证和 Api。</span><span class="sxs-lookup"><span data-stu-id="1194b-122">The provider exposes authentication and APIs that the components use to call Microsoft Graph.</span></span>

<span data-ttu-id="1194b-123">该工具包包含适用于[MSAL](./providers/msal.md)、 [SharePoint](./providers/sharepoint.md)和[团队](./providers/teams.md)的提供程序。</span><span class="sxs-lookup"><span data-stu-id="1194b-123">The toolkit contains providers for [MSAL](./providers/msal.md), [SharePoint](./providers/sharepoint.md), and [Teams](./providers/teams.md).</span></span> <span data-ttu-id="1194b-124">您还可以通过创建[自定义提供程序](./providers/custom.md)或将[ProxyProvider](./providers/proxy.md)与您自己的后端身份验证结合使用来使用自己的身份验证逻辑。</span><span class="sxs-lookup"><span data-stu-id="1194b-124">You can also use your own authentication logic by creating a [custom provider](./providers/custom.md), or using the [ProxyProvider](./providers/proxy.md) with your own backend authentication.</span></span> 

## <a name="polyfills"></a><span data-ttu-id="1194b-125">Polyfills.ts</span><span class="sxs-lookup"><span data-stu-id="1194b-125">Polyfills</span></span>

<span data-ttu-id="1194b-126">如果您正在使用 npm 程序包中的 es6 模块，请确保在项目中包含 polyfills.ts，因为它们不会自动包括在内。</span><span class="sxs-lookup"><span data-stu-id="1194b-126">If you're using the es6 modules from the npm package, make sure to include polyfills in your project as they are not included automatically.</span></span> <span data-ttu-id="1194b-127">若要了解详细信息，请参阅[polyfills.ts](https://www.webcomponents.org/polyfills)。</span><span class="sxs-lookup"><span data-stu-id="1194b-127">To learn more, see [polyfills](https://www.webcomponents.org/polyfills).</span></span>

<span data-ttu-id="1194b-128">如果要在 unpkg 上的捆绑包中使用 mgt-loader 脚本，则已包含 polyfills.ts。</span><span class="sxs-lookup"><span data-stu-id="1194b-128">If you're using the mgt-loader.js script from the bundle on unpkg, the polyfills are already included.</span></span>


## <a name="using-the-components-with-react-angular-and-other-frameworks"></a><span data-ttu-id="1194b-129">将组件与响应、角度和其他框架结合使用</span><span class="sxs-lookup"><span data-stu-id="1194b-129">Using the components with React, Angular, and other frameworks</span></span>

<span data-ttu-id="1194b-130">Web 组件基于几个 web 标准，可用于任何已在使用的框架。</span><span class="sxs-lookup"><span data-stu-id="1194b-130">Web components are based on several web standards and can be used with any framework you're already using.</span></span> <span data-ttu-id="1194b-131">但是，并非所有框架都以相同的方式处理 web 组件。</span><span class="sxs-lookup"><span data-stu-id="1194b-131">However, not all frameworks handle web components the same way.</span></span> <span data-ttu-id="1194b-132">若要了解根据您的框架可能应用的注意事项的详细信息，请参阅 project 中的[自定义元素](https://custom-elements-everywhere.com/)。</span><span class="sxs-lookup"><span data-stu-id="1194b-132">To learn more about the considerations that might apply depending on your framework, see the [Custom Elements Everywhere](https://custom-elements-everywhere.com/) project.</span></span>

<span data-ttu-id="1194b-133">以下各节简要介绍了如何将 Microsoft Graph 工具包组件与响应和角结合使用。</span><span class="sxs-lookup"><span data-stu-id="1194b-133">The following sections provide a quick overview of using the Microsoft Graph Toolkit components with React and Angular.</span></span>

### <a name="react"></a><span data-ttu-id="1194b-134">React</span><span class="sxs-lookup"><span data-stu-id="1194b-134">React</span></span>

<span data-ttu-id="1194b-135">"响应" 将所有数据以 HTML 属性的形式传递给自定义元素。</span><span class="sxs-lookup"><span data-stu-id="1194b-135">React passes all data to Custom Elements in the form of HTML attributes.</span></span> <span data-ttu-id="1194b-136">对于基元数据，这是很好的，但它在传递丰富数据（如对象或数组）时不起作用。</span><span class="sxs-lookup"><span data-stu-id="1194b-136">For primitive data this is fine, but it does not work when passing rich data, like objects or arrays.</span></span> <span data-ttu-id="1194b-137">在这些情况下，您需要使用将`ref`传递到对象中的。</span><span class="sxs-lookup"><span data-stu-id="1194b-137">In those cases you will need to use a `ref` to pass in the object.</span></span>

<span data-ttu-id="1194b-138">Ex</span><span class="sxs-lookup"><span data-stu-id="1194b-138">Ex:</span></span>

```jsx
// import all the components
import '@microsoft/mgt';

class App extends Component {
  render() {
    return <mgt-person show-name ref={el => (el.personDetails = { displayName: 'Nikola Metulev' })} />;
  }
}
```

<span data-ttu-id="1194b-139">由于反应实现其自己的合成事件系统，因此它无法侦听来自自定义元素的 DOM 事件，而不使用替代方法。</span><span class="sxs-lookup"><span data-stu-id="1194b-139">Because React implements its own synthetic event system, it cannot listen for DOM events coming from custom elements without the use of a workaround.</span></span> <span data-ttu-id="1194b-140">您需要使用`ref`来引用工具包组件，并手动将事件侦听器附加到 addEventListener，如下面的示例所示。</span><span class="sxs-lookup"><span data-stu-id="1194b-140">You will need to use a `ref` to reference the toolkit components and manually attach event listeners with addEventListener, as shown in the following example.</span></span>

```jsx
// you can just import a single component
import '@microsoft/mgt/dist/es6/components/mgt-login/mgt-login.js';

class App extends Component {
  render() {
    return <mgt-login ref="loginComponent" />;
  }

  componentDidMount() {
    this.refs.loginComponent.addEventListener('loginCompleted', e => {
      // handle event
    });
  }
}
```

#### <a name="react-typescript-and-tsx"></a><span data-ttu-id="1194b-141">响应、Typescript 和 TSX</span><span class="sxs-lookup"><span data-stu-id="1194b-141">React, Typescript, and TSX</span></span>

<span data-ttu-id="1194b-142">当您将自定义元素与响应和 Typescript 一起使用时，可能会出现已知问题。</span><span class="sxs-lookup"><span data-stu-id="1194b-142">A known issue can occur when you use custom elements with React and Typescript.</span></span> <span data-ttu-id="1194b-143">在尝试使用 tsx 中的组件时，Typescript 将引发错误。</span><span class="sxs-lookup"><span data-stu-id="1194b-143">Typescript will throw an error when trying to use a component in tsx.</span></span> <span data-ttu-id="1194b-144">解决方法是在代码中定义自定义元素，如下所示。</span><span class="sxs-lookup"><span data-stu-id="1194b-144">The workaround is to define the custom element in your code, as shown.</span></span>

```ts
declare global {
  namespace JSX {
    interface IntrinsicElements {
      'mgt-login': any;
    }
  }
}
```

<span data-ttu-id="1194b-145">然后，您可以在 tsx 中使用它`<mgt-login></mgt-login>`。</span><span class="sxs-lookup"><span data-stu-id="1194b-145">You can then use it in your tsx as `<mgt-login></mgt-login>`.</span></span>

### <a name="angular"></a><span data-ttu-id="1194b-146">Angular</span><span class="sxs-lookup"><span data-stu-id="1194b-146">Angular</span></span>

<span data-ttu-id="1194b-147">角度的默认绑定语法将始终设置元素的属性。</span><span class="sxs-lookup"><span data-stu-id="1194b-147">Angular's default binding syntax will always set properties on an element.</span></span> <span data-ttu-id="1194b-148">这适用于丰富的数据（如对象和数组），也适用于基元值。</span><span class="sxs-lookup"><span data-stu-id="1194b-148">This works well for rich data, like objects and arrays, and also works well for primitive values.</span></span>

<span data-ttu-id="1194b-149">若要使用自定义元素，首先将添加`app.module.ts` `CUSTOM_ELEMENT_SCHEMA`到`@NgModule() decorator`中的自定义元素，如下面的示例所示。</span><span class="sxs-lookup"><span data-stu-id="1194b-149">To use custom elements, first, enable custom elements in your `app.module.ts` by adding the `CUSTOM_ELEMENT_SCHEMA` to the `@NgModule() decorator`, as shown in the following example.</span></span>

```ts
import { BrowserModule } from '@angular/platform-browser';
import { NgModule, CUSTOM_ELEMENTS_SCHEMA } from '@angular/core';

import { AppComponent } from './app.component';

@NgModule({
  declarations: [AppComponent],
  imports: [BrowserModule],
  schemas: [CUSTOM_ELEMENTS_SCHEMA],
  providers: [],
  bootstrap: [AppComponent]
})
export class AppModule {}
```

<span data-ttu-id="1194b-150">然后，您可以导入要在组件\*的 ts 文件中使用的组件。</span><span class="sxs-lookup"><span data-stu-id="1194b-150">You can then import the component you'd like to use in your component \*.ts file.</span></span>

```ts
import { Component } from '@angular/core';
import '@microsoft/mgt/dist/es6/components/mgt-person/mgt-person';

@Component({
  selector: 'app-root',
  templateUrl: './app.component.html',
  styleUrls: ['./app.component.css']
})
export class AppComponent {
  person = {
    displayName: 'Nikola Metulev'
  };
}
```

<span data-ttu-id="1194b-151">最后，按您在模板中的通常方式使用组件。</span><span class="sxs-lookup"><span data-stu-id="1194b-151">Finally, use the component as you normally would in your template.</span></span>

```html
<mgt-person [personDetails]="person" show-name></mgt-person>
```
