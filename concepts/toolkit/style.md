---
title: 设置 Microsoft Graph 工具包的样式
description: 使用 CSS 自定义属性修改组件样式
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 41262c4e58973d84f4fec56a6d5abe8dfaf555ef
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2019
ms.locfileid: "35242960"
---
# <a name="styling-components-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="a5ee1-103">Microsoft Graph 工具包中的样式组件</span><span class="sxs-lookup"><span data-stu-id="a5ee1-103">Styling components in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="a5ee1-104">使用 CSS 自定义属性修改组件样式。</span><span class="sxs-lookup"><span data-stu-id="a5ee1-104">Use CSS custom properties to modify the component styles.</span></span>

<span data-ttu-id="a5ee1-105">每个组件都介绍一组[CSS 自定义属性](https://developer.mozilla.org/en-US/docs/Web/CSS/Using_CSS_custom_properties), 您可以使用这些属性来更改特定元素的外观和感觉。</span><span class="sxs-lookup"><span data-stu-id="a5ee1-105">Each component documents a set of [CSS custom properties](https://developer.mozilla.org/en-US/docs/Web/CSS/Using_CSS_custom_properties) that you can use to change the look and feel of certain elements.</span></span> <span data-ttu-id="a5ee1-106">例如：</span><span class="sxs-lookup"><span data-stu-id="a5ee1-106">For example:</span></span>

```css
mgt-person {
  --avatar-size: 34px;
}
```

<span data-ttu-id="a5ee1-107">除非提供 CSS 自定义属性, 否则无法对组件的内部元素进行样式。</span><span class="sxs-lookup"><span data-stu-id="a5ee1-107">You can't style internal elements of a component unless you provide a CSS custom property.</span></span> <span data-ttu-id="a5ee1-108">组件子元素承载于[阴影 dom](https://developer.mozilla.org/en-US/docs/Web/Web_Components/Using_shadow_DOM)中。</span><span class="sxs-lookup"><span data-stu-id="a5ee1-108">The component child elements are hosted in a [shadow dom](https://developer.mozilla.org/en-US/docs/Web/Web_Components/Using_shadow_DOM).</span></span>

<span data-ttu-id="a5ee1-109">为了获得更大的灵活性, 请考虑使用[自定义模板](./templates.md)。</span><span class="sxs-lookup"><span data-stu-id="a5ee1-109">For more flexibility, consider using [custom templates](./templates.md).</span></span>

## <a name="disable-the-shadow-dom-experimental"></a><span data-ttu-id="a5ee1-110">禁用阴影 dom (实验)</span><span class="sxs-lookup"><span data-stu-id="a5ee1-110">Disable the shadow dom (experimental)</span></span>

<span data-ttu-id="a5ee1-111">您可以通过在使用任何设计标记之前将`useShadowDom` `MgtBaseComponent`类的静态属性设置为 false, 从而禁用影子 dom, 并使用常规浏览器样式表直接设置内部元素的样式。</span><span class="sxs-lookup"><span data-stu-id="a5ee1-111">You can disable the shadow dom, and directly style internal elements using normal browser stylesheets, by setting the static property `useShadowDom` of the `MgtBaseComponent` class to false before using any MGT tags.</span></span>


```html
<script type="module">
  import { MgtBaseComponent } from './dist/es6/components/baseComponent.js';
   MgtBaseComponent.useShadowRoot = false;
</script>

<script type="module" src="./dist/es6/components/mgt-tasks/mgt-tasks.js"></script>
````
