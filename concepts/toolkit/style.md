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
# <a name="styling-components-in-the-microsoft-graph-toolkit"></a>Microsoft Graph 工具包中的样式组件

使用 CSS 自定义属性修改组件样式。

每个组件都介绍一组[CSS 自定义属性](https://developer.mozilla.org/en-US/docs/Web/CSS/Using_CSS_custom_properties), 您可以使用这些属性来更改特定元素的外观和感觉。 例如：

```css
mgt-person {
  --avatar-size: 34px;
}
```

除非提供 CSS 自定义属性, 否则无法对组件的内部元素进行样式。 组件子元素承载于[阴影 dom](https://developer.mozilla.org/en-US/docs/Web/Web_Components/Using_shadow_DOM)中。

为了获得更大的灵活性, 请考虑使用[自定义模板](./templates.md)。

## <a name="disable-the-shadow-dom-experimental"></a>禁用阴影 dom (实验)

您可以通过在使用任何设计标记之前将`useShadowDom` `MgtBaseComponent`类的静态属性设置为 false, 从而禁用影子 dom, 并使用常规浏览器样式表直接设置内部元素的样式。


```html
<script type="module">
  import { MgtBaseComponent } from './dist/es6/components/baseComponent.js';
   MgtBaseComponent.useShadowRoot = false;
</script>

<script type="module" src="./dist/es6/components/mgt-tasks/mgt-tasks.js"></script>
````
