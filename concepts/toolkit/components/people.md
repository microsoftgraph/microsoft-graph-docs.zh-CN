---
title: Microsoft Graph 工具包中的 "人员" 组件
description: 您可以使用`mgt-people` web 组件显示一组用户或联系人，方法是使用其照片或缩写。
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 78dc1504d7f46756809abcf922dfcea431fd796c
ms.sourcegitcommit: f2dffaca3e1c5b74a01b59e1b76dba1592a6a5d1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/14/2020
ms.locfileid: "42639959"
---
# <a name="people-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="f8875-103">Microsoft Graph 工具包中的 "人员" 组件</span><span class="sxs-lookup"><span data-stu-id="f8875-103">People component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="f8875-104">您可以使用`mgt-people` web 组件显示一组用户或联系人，方法是使用其照片或缩写。</span><span class="sxs-lookup"><span data-stu-id="f8875-104">You can use the `mgt-people` web component to display a group of people or contacts by using their photos or initials.</span></span> <span data-ttu-id="f8875-105">默认情况下，它将显示登录用户最常使用的联系人。</span><span class="sxs-lookup"><span data-stu-id="f8875-105">By default, it will display the most frequent contacts for the signed in user.</span></span>

<span data-ttu-id="f8875-106">此组件使用多个 "控制[人员](./person.md)" 控件，但它可以绑定到一组人员描述符。</span><span class="sxs-lookup"><span data-stu-id="f8875-106">This component uses multiple [mgt-person](./person.md) controls, but it can be bound to a set of people descriptors.</span></span> <span data-ttu-id="f8875-107">如果要显示的人员多于`show-max`该值，则将添加一个数字以指示其他联系人的数量。</span><span class="sxs-lookup"><span data-stu-id="f8875-107">If there are more people to display than the `show-max` value, a number will be added to indicate the number of additional contacts.</span></span>

## <a name="example"></a><span data-ttu-id="f8875-108">示例</span><span class="sxs-lookup"><span data-stu-id="f8875-108">Example</span></span>

<span data-ttu-id="f8875-109">下面的示例展示了使用`mgt-people`组件显示的一组人员。</span><span class="sxs-lookup"><span data-stu-id="f8875-109">The following example shows a group of people displayed using the `mgt-people` component.</span></span> <span data-ttu-id="f8875-110">您可以使用代码编辑器来查看[属性](#properties)如何更改组件的行为。</span><span class="sxs-lookup"><span data-stu-id="f8875-110">You can use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-people--people&source=docs" height="350"></iframe>

[<span data-ttu-id="f8875-111">在 "dev" 中打开此示例</span><span class="sxs-lookup"><span data-stu-id="f8875-111">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-people--people&source=docs)

## <a name="properties"></a><span data-ttu-id="f8875-112">属性</span><span class="sxs-lookup"><span data-stu-id="f8875-112">Properties</span></span>

<span data-ttu-id="f8875-113">默认情况下， `mgt-people`组件使用`personType/class eq 'Person'`筛选器从`/me/people`终结点提取事件，以显示经常联系的用户。</span><span class="sxs-lookup"><span data-stu-id="f8875-113">By default, the `mgt-people` component fetches events from the `/me/people` endpoint with the `personType/class eq 'Person'` filter to display frequently contacted users.</span></span> <span data-ttu-id="f8875-114">您可以使用多个属性来更改此行为。</span><span class="sxs-lookup"><span data-stu-id="f8875-114">You can use several properties to change this behavior.</span></span>

| <span data-ttu-id="f8875-115">属性</span><span class="sxs-lookup"><span data-stu-id="f8875-115">Attribute</span></span> | <span data-ttu-id="f8875-116">属性</span><span class="sxs-lookup"><span data-stu-id="f8875-116">Property</span></span> | <span data-ttu-id="f8875-117">说明</span><span class="sxs-lookup"><span data-stu-id="f8875-117">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="f8875-118">show-max</span><span class="sxs-lookup"><span data-stu-id="f8875-118">show-max</span></span> | <span data-ttu-id="f8875-119">showMax</span><span class="sxs-lookup"><span data-stu-id="f8875-119">showMax</span></span> | <span data-ttu-id="f8875-120">指示要显示的最大用户数。</span><span class="sxs-lookup"><span data-stu-id="f8875-120">Indicates the maximum number of people to show.</span></span> <span data-ttu-id="f8875-121">默认值为3。</span><span class="sxs-lookup"><span data-stu-id="f8875-121">Default value is 3.</span></span> |
| <span data-ttu-id="f8875-122">people</span><span class="sxs-lookup"><span data-stu-id="f8875-122">people</span></span> | <span data-ttu-id="f8875-123">people</span><span class="sxs-lookup"><span data-stu-id="f8875-123">people</span></span> | <span data-ttu-id="f8875-124">获取或设置组件呈现的人员列表的人员数组。</span><span class="sxs-lookup"><span data-stu-id="f8875-124">An array of people to get or set the list of people rendered by the component.</span></span> <span data-ttu-id="f8875-125">使用此属性可访问组件加载的人员。</span><span class="sxs-lookup"><span data-stu-id="f8875-125">Use this property to access the people loaded by the component.</span></span> <span data-ttu-id="f8875-126">设置此值可加载自己的人员。</span><span class="sxs-lookup"><span data-stu-id="f8875-126">Set this value to load your own people.</span></span> |
| <span data-ttu-id="f8875-127">组 id</span><span class="sxs-lookup"><span data-stu-id="f8875-127">group-id</span></span> | <span data-ttu-id="f8875-128">groupId</span><span class="sxs-lookup"><span data-stu-id="f8875-128">groupId</span></span> | <span data-ttu-id="f8875-129">从各自的 ID 检索特定 Microsoft Graph 中的人员。</span><span class="sxs-lookup"><span data-stu-id="f8875-129">Retrieves people from a specific Microsoft Graph from the respective ID.</span></span> |
| <span data-ttu-id="f8875-130">用户 id</span><span class="sxs-lookup"><span data-stu-id="f8875-130">user-ids</span></span> | <span data-ttu-id="f8875-131">userIds</span><span class="sxs-lookup"><span data-stu-id="f8875-131">userIds</span></span> | <span data-ttu-id="f8875-132">给定一个 Microsoft Graph 用户`ids`的数组，组件将呈现这些用户。</span><span class="sxs-lookup"><span data-stu-id="f8875-132">Given an array of Microsoft Graph user `ids`, the component will render these users.</span></span>  |
| <span data-ttu-id="f8875-133">人员-卡片</span><span class="sxs-lookup"><span data-stu-id="f8875-133">person-card</span></span> | <span data-ttu-id="f8875-134">personCard</span><span class="sxs-lookup"><span data-stu-id="f8875-134">personCard</span></span> | <span data-ttu-id="f8875-135">一个枚举，用于确定激活浮出式面板- `hover`或`click`的必需用户操作。</span><span class="sxs-lookup"><span data-stu-id="f8875-135">An enumeration to determine user action necessary to activate flyout panel - `hover` or `click`.</span></span> <span data-ttu-id="f8875-136">默认值为 `none`。</span><span class="sxs-lookup"><span data-stu-id="f8875-136">Default value is `none`.</span></span> |


<span data-ttu-id="f8875-137">下面的示例设置要显示的最大用户数。</span><span class="sxs-lookup"><span data-stu-id="f8875-137">The following example sets the maximum number of people to show.</span></span>

```html
<mgt-people
  show-max="4">
</mgt-people>
```

## <a name="css-custom-properties"></a><span data-ttu-id="f8875-138">CSS 自定义属性</span><span class="sxs-lookup"><span data-stu-id="f8875-138">CSS custom properties</span></span>

<span data-ttu-id="f8875-139">`mgt-people`组件定义以下 CSS 自定义属性。</span><span class="sxs-lookup"><span data-stu-id="f8875-139">The `mgt-people` component defines the following CSS custom properties.</span></span>

```css
mgt-people {
  --list-margin: 8px 4px 8px 8px; /* Margin for component */
  --avatar-margin: 0 4px 0 0; /* Margin for each person */
}
```

## <a name="templates"></a><span data-ttu-id="f8875-140">模板</span><span class="sxs-lookup"><span data-stu-id="f8875-140">Templates</span></span>

<span data-ttu-id="f8875-141">支持多个[模板](../templates.md)，这些模板可用于替换组件的某些部分。 `mgt-people`</span><span class="sxs-lookup"><span data-stu-id="f8875-141">The `mgt-people` supports several [templates](../templates.md) that you can use to replace certain parts of the component.</span></span> <span data-ttu-id="f8875-142">若要指定模板，请在`<template>`组件内添加一个元素，并`data-type`将值设置为下列值之一。</span><span class="sxs-lookup"><span data-stu-id="f8875-142">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="f8875-143">数据类型</span><span class="sxs-lookup"><span data-stu-id="f8875-143">Data type</span></span> | <span data-ttu-id="f8875-144">数据上下文</span><span class="sxs-lookup"><span data-stu-id="f8875-144">Data context</span></span> | <span data-ttu-id="f8875-145">说明</span><span class="sxs-lookup"><span data-stu-id="f8875-145">Description</span></span> |
| --- | --- | --- |
| `default` | <span data-ttu-id="f8875-146">`people`： person 对象列表</span><span class="sxs-lookup"><span data-stu-id="f8875-146">`people`: list of person objects</span></span> | <span data-ttu-id="f8875-147">默认模板会将整个组件替换为您自己的组件。</span><span class="sxs-lookup"><span data-stu-id="f8875-147">The default template replaces the entire component with your own.</span></span> |
| `person` | <span data-ttu-id="f8875-148">`person`： person 对象</span><span class="sxs-lookup"><span data-stu-id="f8875-148">`person`: person object</span></span> | <span data-ttu-id="f8875-149">用于呈现每个人的模板。</span><span class="sxs-lookup"><span data-stu-id="f8875-149">The template used to render each person.</span></span> |
| `overflow` | <span data-ttu-id="f8875-150">`people`： person 对象列表</span><span class="sxs-lookup"><span data-stu-id="f8875-150">`people`: list of person objects</span></span> <br> <span data-ttu-id="f8875-151">`max`：显示的人员的数量</span><span class="sxs-lookup"><span data-stu-id="f8875-151">`max`: number of shown people</span></span> <br> <span data-ttu-id="f8875-152">`extra`：额外人员数</span><span class="sxs-lookup"><span data-stu-id="f8875-152">`extra`: number of extra people</span></span> | <span data-ttu-id="f8875-153">用于将数字呈现在人员列表右侧的最大值之后的模板。</span><span class="sxs-lookup"><span data-stu-id="f8875-153">The template used to render the number beyond the max to the right of the list of people.</span></span> |
| `no-data` | <span data-ttu-id="f8875-154">不传递数据上下文</span><span class="sxs-lookup"><span data-stu-id="f8875-154">No data context is passed</span></span> | <span data-ttu-id="f8875-155">没有可用数据时使用的模板。</span><span class="sxs-lookup"><span data-stu-id="f8875-155">The template used when no data is available.</span></span> |

<span data-ttu-id="f8875-156">下面的示例演示如何使用`person`模板。</span><span class="sxs-lookup"><span data-stu-id="f8875-156">The following examples shows how to use the `person` template.</span></span>

```html
<mgt-people>
  <template>
    <ul><li data-for="person in people">
      <mgt-person person-query="{{ person.userPrincipalName }}"></mgt-person>
      <h3>{{ person.displayName }}</h3>
      <p>{{ person.jobTitle }}</p>
      <p>{{ person.department }}</p>
    </li></ul>
  </template>
</mgt-people>
```

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="f8875-157">Microsoft Graph 权限</span><span class="sxs-lookup"><span data-stu-id="f8875-157">Microsoft Graph permissions</span></span>

<span data-ttu-id="f8875-158">此组件使用以下 Microsoft Graph Api 和权限：</span><span class="sxs-lookup"><span data-stu-id="f8875-158">This component uses the following Microsoft Graph APIs and permissions:</span></span>

| <span data-ttu-id="f8875-159">Resource</span><span class="sxs-lookup"><span data-stu-id="f8875-159">Resource</span></span> | <span data-ttu-id="f8875-160">权限</span><span class="sxs-lookup"><span data-stu-id="f8875-160">Permission</span></span> |
| - | - |
| [<span data-ttu-id="f8875-161">/me/people</span><span class="sxs-lookup"><span data-stu-id="f8875-161">/me/people</span></span>](/graph/api/user-list-people?view=graph-rest-1.0) | `People.Read` |

## <a name="authentication"></a><span data-ttu-id="f8875-162">身份验证</span><span class="sxs-lookup"><span data-stu-id="f8875-162">Authentication</span></span>

<span data-ttu-id="f8875-163">该控件使用[身份验证文档](./../providers.md)中介绍的全局身份验证提供程序。</span><span class="sxs-lookup"><span data-stu-id="f8875-163">The control uses the global authentication provider described in the [authentication documentation](./../providers.md).</span></span>
