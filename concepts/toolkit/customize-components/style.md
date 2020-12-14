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
# <a name="styling-components-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="24e7b-103">在 Microsoft Graph 中设置组件样式Toolkit</span><span class="sxs-lookup"><span data-stu-id="24e7b-103">Styling components in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="24e7b-104">每个 Microsoft Graph Toolkit组件都记录一组 [CSS](https://developer.mozilla.org/en-US/docs/Web/CSS/Using_CSS_custom_properties) 自定义属性，可用于更改某些元素的外观。</span><span class="sxs-lookup"><span data-stu-id="24e7b-104">Each Microsoft Graph Toolkit component documents a set of [CSS custom properties](https://developer.mozilla.org/en-US/docs/Web/CSS/Using_CSS_custom_properties) that you can use to change the look and feel of certain elements.</span></span> <span data-ttu-id="24e7b-105">您可以在每个组件文档找到可用的自定义 CSS 属性。例如：</span><span class="sxs-lookup"><span data-stu-id="24e7b-105">You can find the available custom CSS properties in each component docs. For example:</span></span>

```css
mgt-person {
  --avatar-size: 34px;
}
```

<span data-ttu-id="24e7b-106">除非提供 CSS 自定义属性，否则无法设置组件内部元素的样式。</span><span class="sxs-lookup"><span data-stu-id="24e7b-106">You can't style internal elements of a component unless you provide a CSS custom property.</span></span> <span data-ttu-id="24e7b-107">组件子元素托管在卷影 [dom 中](https://developer.mozilla.org/en-US/docs/Web/Web_Components/Using_shadow_DOM)。</span><span class="sxs-lookup"><span data-stu-id="24e7b-107">The component child elements are hosted in a [shadow dom](https://developer.mozilla.org/en-US/docs/Web/Web_Components/Using_shadow_DOM).</span></span>

<span data-ttu-id="24e7b-108">为了更灵活，请考虑使用 [自定义模板](./templates.md)。</span><span class="sxs-lookup"><span data-stu-id="24e7b-108">For more flexibility, consider using [custom templates](./templates.md).</span></span>

## <a name="apply-themes"></a><span data-ttu-id="24e7b-109">应用主题</span><span class="sxs-lookup"><span data-stu-id="24e7b-109">Apply themes</span></span>

<span data-ttu-id="24e7b-110">有两个主题可用 - 浅色和深色。</span><span class="sxs-lookup"><span data-stu-id="24e7b-110">Two themes are available - light and dark.</span></span> <span data-ttu-id="24e7b-111">默认情况下，所有组件都使用浅色主题设置样式。</span><span class="sxs-lookup"><span data-stu-id="24e7b-111">By default, all components are styled with light theme.</span></span> <span data-ttu-id="24e7b-112">若要切换到深色主题，只需应用到 HTML `class="mgt-dark"` 页面部分。</span><span class="sxs-lookup"><span data-stu-id="24e7b-112">To switch to dark theme, you can simply apply `class="mgt-dark"` to the  section of your HTML page.</span></span> <span data-ttu-id="24e7b-113">该部分内的组件将应用深色主题。</span><span class="sxs-lookup"><span data-stu-id="24e7b-113">The components inside that section will have dark theme applied.</span></span> <span data-ttu-id="24e7b-114">以下示例显示了如何根据 HTML 的结构应用主题。</span><span class="sxs-lookup"><span data-stu-id="24e7b-114">The following examples show how themes will apply based on how you structure your HTML.</span></span>

<span data-ttu-id="24e7b-115">示例 1：全局主题</span><span class="sxs-lookup"><span data-stu-id="24e7b-115">Example 1: Global theme</span></span>

```html
<body class="mgt-light">
    <!-- light theme will apply to all components in this section -->
    <header><mgt-login></mgt-login></header>
    <article><mgt-agenda></mgt-agend></article>
    <footer></footer>
</body>
```

<span data-ttu-id="24e7b-116">示例 2：单个组件主题</span><span class="sxs-lookup"><span data-stu-id="24e7b-116">Example 2: Individual component theme</span></span>

```html
<mgt-person-card class="mgt-dark"></mgt-person-card>
```

<span data-ttu-id="24e7b-117">示例 3：区域主题</span><span class="sxs-lookup"><span data-stu-id="24e7b-117">Example 3: Regional theme</span></span>

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

<span data-ttu-id="24e7b-118">示例 4：使用主题自定义 CSS</span><span class="sxs-lookup"><span data-stu-id="24e7b-118">Example 4: Customize CSS with theme</span></span>

```html
<mgt-people-picker class="mgt-dark custom-class"></mgt-people-picker>
```
```css
mgt-people-picker.custom-class {
    --input-background-color: $custom-background-color;
    --input-border: $custom-input-border;
}
```
