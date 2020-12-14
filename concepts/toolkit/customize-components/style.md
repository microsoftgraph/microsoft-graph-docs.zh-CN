---
title: 在 Microsoft Graph 中设置组件样式Toolkit
description: 使用 CSS 自定义属性修改 Microsoft Graph Toolkit组件样式。
localization_priority: Normal
author: beth-panx
ms.openlocfilehash: 33ccc02f182731d494820976632b7cec2425d077
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49663923"
---
# <a name="styling-components-in-the-microsoft-graph-toolkit"></a>在 Microsoft Graph 中设置组件样式Toolkit

每个 Microsoft Graph Toolkit组件都记录一组 [CSS](https://developer.mozilla.org/en-US/docs/Web/CSS/Using_CSS_custom_properties) 自定义属性，可用于更改某些元素的外观。 您可以在每个组件文档找到可用的自定义 CSS 属性。例如：

```css
mgt-person {
  --avatar-size: 34px;
}
```

除非提供 CSS 自定义属性，否则无法设置组件内部元素的样式。 组件子元素托管在卷影 [dom 中](https://developer.mozilla.org/en-US/docs/Web/Web_Components/Using_shadow_DOM)。

为了更灵活，请考虑使用 [自定义模板](./templates.md)。

## <a name="apply-themes"></a>应用主题

有两个主题可用 - 浅色和深色。 默认情况下，所有组件都使用浅色主题设置样式。 若要切换到深色主题，只需应用到 HTML `class="mgt-dark"` 页面部分。 该部分内的组件将应用深色主题。 以下示例显示了如何根据 HTML 的结构应用主题。

示例 1：全局主题

```html
<body class="mgt-light">
    <!-- light theme will apply to all components in this section -->
    <header><mgt-login></mgt-login></header>
    <article><mgt-agenda></mgt-agend></article>
    <footer></footer>
</body>
```

示例 2：单个组件主题

```html
<mgt-person-card class="mgt-dark"></mgt-person-card>
```

示例 3：区域主题

```html
<div class="mgt-light">
    <header class="mgt-dark">
        // login component will have dark theme
        <mgt-login></mgt-login>
    </header>
    <article>
        // agenda component will have light theme
        <mgt-agenda></mgt-agenda>
    </article>
</div>
```

示例 4：使用主题自定义 CSS

```html
<mgt-people-picker class="mgt-dark custom-class"></mgt-people-picker>
```
```css
mgt-people-picker.custom-class {
    --input-background-color: $custom-background-color;
    --input-border: $custom-input-border;
}
```
