---
title: Microsoft Graph 工具包 (预览)
description: Microsoft Graph 工具包是框架不可知的 web 组件以及用于访问和使用 Microsoft Graph 的帮助程序的集合。
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: ca55500217ab23f9e6a2744da61f332e745af398
ms.sourcegitcommit: 705b32b9a64516d8138fab34c173b7df4f78a6ad
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/05/2019
ms.locfileid: "35576401"
---
# <a name="microsoft-graph-toolkit-preview"></a><span data-ttu-id="0a960-103">Microsoft Graph 工具包 (预览)</span><span class="sxs-lookup"><span data-stu-id="0a960-103">Microsoft Graph Toolkit (preview)</span></span>

<span data-ttu-id="0a960-104">Microsoft Graph 工具包是框架不可知的 web 组件以及用于访问和使用 Microsoft Graph 的帮助程序的集合。</span><span class="sxs-lookup"><span data-stu-id="0a960-104">The Microsoft Graph Toolkit is a collection of framework-agnostic web components and helpers for accessing and working with Microsoft Graph.</span></span> <span data-ttu-id="0a960-105">所有组件都可以访问 Microsoft Graph, 而无需进行任何自定义。</span><span class="sxs-lookup"><span data-stu-id="0a960-105">All components can access Microsoft Graph without any customization required.</span></span>

> [!NOTE]
> <span data-ttu-id="0a960-106">此库处于预览阶段, 处于早期开发阶段。</span><span class="sxs-lookup"><span data-stu-id="0a960-106">This library is in preview and is in early development.</span></span> <span data-ttu-id="0a960-107">我们希望根据来自社区的反馈对所有组件和 Api 进行更改和改进。</span><span class="sxs-lookup"><span data-stu-id="0a960-107">We expect to make changes and improvements to all components and APIs based on feedback from the community.</span></span>

## <a name="get-started"></a><span data-ttu-id="0a960-108">入门</span><span class="sxs-lookup"><span data-stu-id="0a960-108">Get started</span></span>

<span data-ttu-id="0a960-109">您可以通过直接引用加载程序 (通过 unpkg) 或安装 npm 程序包来使用这些组件。</span><span class="sxs-lookup"><span data-stu-id="0a960-109">You can use the components by referencing the loader directly (via unpkg), or by installing the npm package.</span></span>

<span data-ttu-id="0a960-110">有关如何开始使用 Microsoft Graph 工具包的详细信息, 请参阅[入门视频](https://www.youtube.com/watch?v=oZCGb2MMxa0)。</span><span class="sxs-lookup"><span data-stu-id="0a960-110">For details about how to get started with the Microsoft Graph Toolkit, see the [Get started video](https://www.youtube.com/watch?v=oZCGb2MMxa0).</span></span>

### <a name="use-via-mgt-loader"></a><span data-ttu-id="0a960-111">通过预加载加载程序使用</span><span class="sxs-lookup"><span data-stu-id="0a960-111">Use via mgt-loader</span></span>

<span data-ttu-id="0a960-112">请参阅下列[jsfiddle 示例](https://jsfiddle.net/metulev/9phqxLd5/)。</span><span class="sxs-lookup"><span data-stu-id="0a960-112">See the folowing [jsfiddle example](https://jsfiddle.net/metulev/9phqxLd5/).</span></span>

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
```

<span data-ttu-id="0a960-113">然后, 您可以开始在 HTML 页面中使用这些组件。</span><span class="sxs-lookup"><span data-stu-id="0a960-113">You can then start using the components in your HTML page.</span></span> <span data-ttu-id="0a960-114">下面是 MSAL 提供程序的完整工作示例。</span><span class="sxs-lookup"><span data-stu-id="0a960-114">The following is a full working example with the MSAL provider.</span></span>

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal-provider client-id="[CLIENT-ID]"></mgt-msal-provider>
<mgt-login></mgt-login>

<!-- <script>
    // alternatively, you can set the provider in code and provide more options
    mgt.Providers.globalProvider = new mgt.MsalProvider({clientId: '[CLIENT-ID]'});
</script> -->
```

> <span data-ttu-id="0a960-115">**注意:** MSAL 要求将页面托管在用于身份验证重定向的 web 服务器中。</span><span class="sxs-lookup"><span data-stu-id="0a960-115">**Note:** MSAL requires the page to be hosted in a web server for the authentication redirects.</span></span> <span data-ttu-id="0a960-116">如果只是开始并且想要进行播放, 可以在 Visual Studio Code 中使用[live server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) 。</span><span class="sxs-lookup"><span data-stu-id="0a960-116">If you're just getting started and want to play around, you can use [live server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) in Visual Studio Code.</span></span>

### <a name="use-via-npm-es6-modules"></a><span data-ttu-id="0a960-117">通过 NPM (es6 模块) 使用</span><span class="sxs-lookup"><span data-stu-id="0a960-117">Use via NPM (es6 modules)</span></span>

<span data-ttu-id="0a960-118">通过使用 es6 模块, 可以完全控制捆绑过程, 并且可以仅捆绑网站所需的代码。</span><span class="sxs-lookup"><span data-stu-id="0a960-118">By using the es6 modules, you have full control of the bundling process and you can bundle only the code you need for your site.</span></span> <span data-ttu-id="0a960-119">首先, 添加 npm 包:</span><span class="sxs-lookup"><span data-stu-id="0a960-119">First, add the npm package:</span></span>

```bash
npm install @microsoft/mgt
```

<span data-ttu-id="0a960-120">现在, 您可以引用正在使用的页面上的所有组件:</span><span class="sxs-lookup"><span data-stu-id="0a960-120">Now you can reference all components at the page you are using:</span></span>

```html
<script src="node_modules/@microsoft/mgt/dist/es6/components.js"></script>
```

<span data-ttu-id="0a960-121">或者, 只引用所需的组件, 避免加载其他所有内容:</span><span class="sxs-lookup"><span data-stu-id="0a960-121">Or, just reference the component you need and avoid loading everything else:</span></span>

```html
<script src="node_modules/@microsoft/mgt/dist/es6/components/mgt-login/mgt-login.js"></script>
```

<span data-ttu-id="0a960-122">同样, 若要添加提供程序, 可以将其添加为组件:</span><span class="sxs-lookup"><span data-stu-id="0a960-122">Similarly, to add a provider, you can add it as a component:</span></span>

```html
<script src="node_modules/@microsoft/mgt/dist/es6/components/providers/mgt-msal-provider.js"></script>

<mgt-msal-provider client-id="[CLIENT-ID]"></mgt-msal-provider>
```

<span data-ttu-id="0a960-123">或者, 将其添加到代码中:</span><span class="sxs-lookup"><span data-stu-id="0a960-123">or, add it in your code:</span></span>

```html
<script type="module">
  import { Providers, MsalProvider } from '@microsoft/mgt';

  Providers.globalProvider = new MsalProvider({ clientId: '[CLIENT-ID]' });
</script>
```

## <a name="providers"></a><span data-ttu-id="0a960-124">商会</span><span class="sxs-lookup"><span data-stu-id="0a960-124">Providers</span></span>

<span data-ttu-id="0a960-125">与[提供程序](./providers.md)配合使用时, 组件的工作效果最佳。</span><span class="sxs-lookup"><span data-stu-id="0a960-125">The components work best when used with a [provider](./providers.md).</span></span> <span data-ttu-id="0a960-126">提供程序公开了组件用来调用 Microsoft Graph 的身份验证和 Api。</span><span class="sxs-lookup"><span data-stu-id="0a960-126">The provider exposes authentication and APIs that the components use to call Microsoft Graph.</span></span>

<span data-ttu-id="0a960-127">该工具包包含适用于[MSAL](./providers/msal.md)、 [SharePoint](./providers/sharepoint.md)、[团队](./providers/teams.md)和 Office 加载项的提供程序 (即将推出)。</span><span class="sxs-lookup"><span data-stu-id="0a960-127">The toolkit contains providers for [MSAL](./providers/msal.md), [SharePoint](./providers/sharepoint.md), [Teams](./providers/teams.md), and Office Add-ins (coming soon).</span></span> <span data-ttu-id="0a960-128">您还可以通过扩展 [IProvider] 抽象类来创建自己的提供程序。</span><span class="sxs-lookup"><span data-stu-id="0a960-128">You can also create your own providers by extending the [IProvider] abstract class.</span></span>

## <a name="polyfills"></a><span data-ttu-id="0a960-129">Polyfills.ts</span><span class="sxs-lookup"><span data-stu-id="0a960-129">Polyfills</span></span>

<span data-ttu-id="0a960-130">如果您正在使用 npm 程序包中的 es6 模块, 请确保在项目中包含 polyfills.ts, 因为它们不会自动包括在内。</span><span class="sxs-lookup"><span data-stu-id="0a960-130">If you're using the es6 modules from the npm package, make sure to include polyfills in your project as they are not included automatically.</span></span> <span data-ttu-id="0a960-131">若要了解详细信息, 请参阅[polyfills.ts](https://www.webcomponents.org/polyfills)。</span><span class="sxs-lookup"><span data-stu-id="0a960-131">To learn more, see [polyfills](https://www.webcomponents.org/polyfills).</span></span>

<span data-ttu-id="0a960-132">如果要在 unpkg 上的捆绑包中使用 mgt-loader 脚本, 则已包含 polyfills.ts。</span><span class="sxs-lookup"><span data-stu-id="0a960-132">If you're using the mgt-loader.js script from the bundle on unpkg, the polyfills are already included.</span></span>


## <a name="using-the-components-with-react-angular-and-other-frameworks"></a><span data-ttu-id="0a960-133">将组件与响应、角度和其他框架结合使用</span><span class="sxs-lookup"><span data-stu-id="0a960-133">Using the components with React, Angular, and other frameworks</span></span>

<span data-ttu-id="0a960-134">Web 组件基于几个 web 标准, 可用于任何已在使用的框架。</span><span class="sxs-lookup"><span data-stu-id="0a960-134">Web components are based on several web standards and can be used with any framework you're already using.</span></span> <span data-ttu-id="0a960-135">但是, 并非所有框架都以相同的方式处理 web 组件。</span><span class="sxs-lookup"><span data-stu-id="0a960-135">However, not all frameworks handle web components the same way.</span></span> <span data-ttu-id="0a960-136">若要了解根据您的框架可能应用的注意事项的详细信息, 请参阅 project 中的[自定义元素](https://custom-elements-everywhere.com/)。</span><span class="sxs-lookup"><span data-stu-id="0a960-136">To learn more about the considerations that might apply depending on your framework, see the [Custom Elements Everywhere](https://custom-elements-everywhere.com/) project.</span></span>

<span data-ttu-id="0a960-137">以下各节简要介绍了如何将 Microsoft Graph 工具包组件与响应和角结合使用。</span><span class="sxs-lookup"><span data-stu-id="0a960-137">The following sections provide a quick overview of using the Microsoft Graph Toolkit components with React and Angular.</span></span>

### <a name="react"></a><span data-ttu-id="0a960-138">React</span><span class="sxs-lookup"><span data-stu-id="0a960-138">React</span></span>

<span data-ttu-id="0a960-139">"响应" 将所有数据以 HTML 属性的形式传递给自定义元素。</span><span class="sxs-lookup"><span data-stu-id="0a960-139">React passes all data to Custom Elements in the form of HTML attributes.</span></span> <span data-ttu-id="0a960-140">对于基元数据, 这是很好的, 但它在传递丰富数据 (如对象或数组) 时不起作用。</span><span class="sxs-lookup"><span data-stu-id="0a960-140">For primitive data this is fine, but it does not work when passing rich data, like objects or arrays.</span></span> <span data-ttu-id="0a960-141">在这些情况下, 您需要使用将`ref`传递到对象中的。</span><span class="sxs-lookup"><span data-stu-id="0a960-141">In those cases you will need to use a `ref` to pass in the object.</span></span>

<span data-ttu-id="0a960-142">Ex</span><span class="sxs-lookup"><span data-stu-id="0a960-142">Ex:</span></span>

```jsx
// import all the components
import '@microsoft/mgt';

class App extends Component {
  render() {
    return <mgt-person show-name ref={el => (el.personDetails = { displayName: 'Nikola Metulev' })} />;
  }
}
```

<span data-ttu-id="0a960-143">由于反应实现其自己的合成事件系统, 因此它无法侦听来自自定义元素的 DOM 事件, 而不使用替代方法。</span><span class="sxs-lookup"><span data-stu-id="0a960-143">Because React implements its own synthetic event system, it cannot listen for DOM events coming from custom elements without the use of a workaround.</span></span> <span data-ttu-id="0a960-144">您需要使用`ref`来引用工具包组件, 并手动将事件侦听器附加到 addEventListener, 如下面的示例所示。</span><span class="sxs-lookup"><span data-stu-id="0a960-144">You will need to use a `ref` to reference the toolkit components and manually attach event listeners with addEventListener, as shown in the following example.</span></span>

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

#### <a name="react-typescript-and-tsx"></a><span data-ttu-id="0a960-145">响应、Typescript 和 TSX</span><span class="sxs-lookup"><span data-stu-id="0a960-145">React, Typescript, and TSX</span></span>

<span data-ttu-id="0a960-146">当您将自定义元素与响应和 Typescript 一起使用时, 可能会出现已知问题。</span><span class="sxs-lookup"><span data-stu-id="0a960-146">A known issue can occur when you use custom elements with React and Typescript.</span></span> <span data-ttu-id="0a960-147">在尝试使用 tsx 中的组件时, Typescript 将引发错误。</span><span class="sxs-lookup"><span data-stu-id="0a960-147">Typescript will throw an error when trying to use a component in tsx.</span></span> <span data-ttu-id="0a960-148">解决方法是在代码中定义自定义元素, 如下所示。</span><span class="sxs-lookup"><span data-stu-id="0a960-148">The workaround is to define the custom element in your code, as shown.</span></span>

```ts
declare global {
  namespace JSX {
    interface IntrinsicElements {
      'mgt-login': any;
    }
  }
}
```

<span data-ttu-id="0a960-149">然后, 您可以在 tsx 中使用它`<mgt-login></mgt-login>`。</span><span class="sxs-lookup"><span data-stu-id="0a960-149">You can then use it in your tsx as `<mgt-login></mgt-login>`.</span></span>

### <a name="angular"></a><span data-ttu-id="0a960-150">Angular</span><span class="sxs-lookup"><span data-stu-id="0a960-150">Angular</span></span>

<span data-ttu-id="0a960-151">角度的默认绑定语法将始终设置元素的属性。</span><span class="sxs-lookup"><span data-stu-id="0a960-151">Angular's default binding syntax will always set properties on an element.</span></span> <span data-ttu-id="0a960-152">这适用于丰富的数据 (如对象和数组), 也适用于基元值。</span><span class="sxs-lookup"><span data-stu-id="0a960-152">This works well for rich data, like objects and arrays, and also works well for primitive values.</span></span>

<span data-ttu-id="0a960-153">若要使用自定义元素, 首先将添加`app.module.ts` `CUSTOM_ELEMENT_SCHEMA`到`@NgModule() decorator`中的自定义元素, 如下面的示例所示。</span><span class="sxs-lookup"><span data-stu-id="0a960-153">To use custom elements, first, enable custom elements in your `app.module.ts` by adding the `CUSTOM_ELEMENT_SCHEMA` to the `@NgModule() decorator`, as shown in the following example.</span></span>

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

<span data-ttu-id="0a960-154">然后, 您可以导入要在组件\*的 ts 文件中使用的组件。</span><span class="sxs-lookup"><span data-stu-id="0a960-154">You can then import the component you'd like to use in your component \*.ts file.</span></span>

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

<span data-ttu-id="0a960-155">最后, 按您在模板中的通常方式使用组件。</span><span class="sxs-lookup"><span data-stu-id="0a960-155">Finally, use the component as you normally would in your template.</span></span>

```html
<mgt-person [personDetails]="person" show-name></mgt-person>
```
