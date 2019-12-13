---
title: Microsoft Graph 工具包中的 "人员" 组件
description: 您可以使用`mgt-people` web 组件显示一组用户或联系人，方法是使用其照片或缩写。
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 5f85f0a72e8658a8fc734728ae76d79157da39de
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39955874"
---
# <a name="people-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="37610-103">Microsoft Graph 工具包中的 "人员" 组件</span><span class="sxs-lookup"><span data-stu-id="37610-103">People component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="37610-104">您可以使用`mgt-people` web 组件显示一组用户或联系人，方法是使用其照片或缩写。</span><span class="sxs-lookup"><span data-stu-id="37610-104">You can use the `mgt-people` web component to display a group of people or contacts by using their photos or initials.</span></span> <span data-ttu-id="37610-105">默认情况下，它将显示登录用户最常使用的联系人。</span><span class="sxs-lookup"><span data-stu-id="37610-105">By default, it will display the most frequent contacts for the signed in user.</span></span>

<span data-ttu-id="37610-106">此组件使用多个 "控制[人员](./person.md)" 控件，但它可以绑定到一组人员描述符。</span><span class="sxs-lookup"><span data-stu-id="37610-106">This component uses multiple [mgt-person](./person.md) controls, but it can be bound to a set of people descriptors.</span></span> <span data-ttu-id="37610-107">如果要显示的人员多于`show-max`该值，则将添加一个数字以指示其他联系人的数量。</span><span class="sxs-lookup"><span data-stu-id="37610-107">If there are more people to display than the `show-max` value, a number will be added to indicate the number of additional contacts.</span></span>

## <a name="example"></a><span data-ttu-id="37610-108">示例</span><span class="sxs-lookup"><span data-stu-id="37610-108">Example</span></span>

[<span data-ttu-id="37610-109">jsfiddle 示例</span><span class="sxs-lookup"><span data-stu-id="37610-109">jsfiddle example</span></span>](https://jsfiddle.net/metulev/az6pqy2r/)

```html
<mgt-people></mgt-people>
```

![组织-人员](./images/mgt-people.png)

## <a name="properties"></a><span data-ttu-id="37610-111">属性</span><span class="sxs-lookup"><span data-stu-id="37610-111">Properties</span></span>

<span data-ttu-id="37610-112">默认情况下， `mgt-people`组件使用`personType/class eq 'Person'`筛选器从`/me/people`终结点提取事件，以显示经常联系的用户。</span><span class="sxs-lookup"><span data-stu-id="37610-112">By default, the `mgt-people` component fetches events from the `/me/people` endpoint with the `personType/class eq 'Person'` filter to display frequently contacted users.</span></span> <span data-ttu-id="37610-113">您可以使用多个属性来更改此行为。</span><span class="sxs-lookup"><span data-stu-id="37610-113">You can use several properties to change this behavior.</span></span>

| <span data-ttu-id="37610-114">属性</span><span class="sxs-lookup"><span data-stu-id="37610-114">Attribute</span></span> | <span data-ttu-id="37610-115">属性</span><span class="sxs-lookup"><span data-stu-id="37610-115">Property</span></span> | <span data-ttu-id="37610-116">说明</span><span class="sxs-lookup"><span data-stu-id="37610-116">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="37610-117">show-max</span><span class="sxs-lookup"><span data-stu-id="37610-117">show-max</span></span> | <span data-ttu-id="37610-118">showMax</span><span class="sxs-lookup"><span data-stu-id="37610-118">showMax</span></span> | <span data-ttu-id="37610-119">指示要显示的最大用户数。</span><span class="sxs-lookup"><span data-stu-id="37610-119">Indicates the maximum number of people to show.</span></span> <span data-ttu-id="37610-120">默认值为3。</span><span class="sxs-lookup"><span data-stu-id="37610-120">Default value is 3.</span></span> |
| <span data-ttu-id="37610-121">people</span><span class="sxs-lookup"><span data-stu-id="37610-121">people</span></span> | <span data-ttu-id="37610-122">people</span><span class="sxs-lookup"><span data-stu-id="37610-122">people</span></span> | <span data-ttu-id="37610-123">获取或设置组件呈现的人员列表的人员数组。</span><span class="sxs-lookup"><span data-stu-id="37610-123">An array of people to get or set the list of people rendered by the component.</span></span> <span data-ttu-id="37610-124">使用此属性可访问组件加载的人员。</span><span class="sxs-lookup"><span data-stu-id="37610-124">Use this property to access the people loaded by the component.</span></span> <span data-ttu-id="37610-125">设置此值可加载自己的人员。</span><span class="sxs-lookup"><span data-stu-id="37610-125">Set this value to load your own people.</span></span> |
| <span data-ttu-id="37610-126">组 id</span><span class="sxs-lookup"><span data-stu-id="37610-126">group-id</span></span> | <span data-ttu-id="37610-127">groupId</span><span class="sxs-lookup"><span data-stu-id="37610-127">groupId</span></span> | <span data-ttu-id="37610-128">从各自的 ID 检索特定 Microsoft Graph 中的人员。</span><span class="sxs-lookup"><span data-stu-id="37610-128">Retrieves people from a specific Microsoft Graph from the respective ID.</span></span> |
| <span data-ttu-id="37610-129">用户 id</span><span class="sxs-lookup"><span data-stu-id="37610-129">user-ids</span></span> | <span data-ttu-id="37610-130">userIds</span><span class="sxs-lookup"><span data-stu-id="37610-130">userIds</span></span> | <span data-ttu-id="37610-131">给定一个 Microsoft Graph 用户`ids`的数组，组件将呈现这些用户。</span><span class="sxs-lookup"><span data-stu-id="37610-131">Given an array of Microsoft Graph user `ids`, the component will render these users.</span></span>  |
| <span data-ttu-id="37610-132">人员-卡片</span><span class="sxs-lookup"><span data-stu-id="37610-132">person-card</span></span> | <span data-ttu-id="37610-133">personCard</span><span class="sxs-lookup"><span data-stu-id="37610-133">personCard</span></span> | <span data-ttu-id="37610-134">一个枚举，用于确定激活浮出式面板- `hover`或`click`的必需用户操作。</span><span class="sxs-lookup"><span data-stu-id="37610-134">An enumeration to determine user action necessary to activate flyout panel - `hover` or `click`.</span></span> <span data-ttu-id="37610-135">默认值为 `none`。</span><span class="sxs-lookup"><span data-stu-id="37610-135">Default value is `none`.</span></span> |


<span data-ttu-id="37610-136">下面的示例设置要显示的最大用户数。</span><span class="sxs-lookup"><span data-stu-id="37610-136">The following example sets the maximum number of people to show.</span></span>

```html
<mgt-people
  show-max="4">
</mgt-people>
```

## <a name="css-custom-properties"></a><span data-ttu-id="37610-137">CSS 自定义属性</span><span class="sxs-lookup"><span data-stu-id="37610-137">CSS custom properties</span></span>

<span data-ttu-id="37610-138">`mgt-people`组件定义以下 CSS 自定义属性。</span><span class="sxs-lookup"><span data-stu-id="37610-138">The `mgt-people` component defines the following CSS custom properties.</span></span>

```css
mgt-people {
  --list-margin: 8px 4px 8px 8px; /* Margin for component */
  --avatar-margin: 0 4px 0 0; /* Margin for each person */
}
```

## <a name="templates"></a><span data-ttu-id="37610-139">模板</span><span class="sxs-lookup"><span data-stu-id="37610-139">Templates</span></span>

<span data-ttu-id="37610-140">支持多个[模板](../templates.md)，这些模板可用于替换组件的某些部分。 `mgt-people`</span><span class="sxs-lookup"><span data-stu-id="37610-140">The `mgt-people` supports several [templates](../templates.md) that you can use to replace certain parts of the component.</span></span> <span data-ttu-id="37610-141">若要指定模板，请在`<template>`组件内添加一个元素，并`data-type`将值设置为下列值之一。</span><span class="sxs-lookup"><span data-stu-id="37610-141">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="37610-142">数据类型</span><span class="sxs-lookup"><span data-stu-id="37610-142">Data type</span></span> | <span data-ttu-id="37610-143">数据上下文</span><span class="sxs-lookup"><span data-stu-id="37610-143">Data context</span></span> | <span data-ttu-id="37610-144">说明</span><span class="sxs-lookup"><span data-stu-id="37610-144">Description</span></span> |
| --- | --- | --- |
| `default` | <span data-ttu-id="37610-145">`people`： person 对象列表</span><span class="sxs-lookup"><span data-stu-id="37610-145">`people`: list of person objects</span></span> | <span data-ttu-id="37610-146">默认模板会将整个组件替换为您自己的组件。</span><span class="sxs-lookup"><span data-stu-id="37610-146">The default template replaces the entire component with your own.</span></span> |
| `person` | <span data-ttu-id="37610-147">`person`： person 对象</span><span class="sxs-lookup"><span data-stu-id="37610-147">`person`: person object</span></span> | <span data-ttu-id="37610-148">用于呈现每个人的模板。</span><span class="sxs-lookup"><span data-stu-id="37610-148">The template used to render each person.</span></span> |
| `overflow` | <span data-ttu-id="37610-149">`people`： person 对象列表</span><span class="sxs-lookup"><span data-stu-id="37610-149">`people`: list of person objects</span></span> <br> <span data-ttu-id="37610-150">`max`：显示的人员的数量</span><span class="sxs-lookup"><span data-stu-id="37610-150">`max`: number of shown people</span></span> <br> <span data-ttu-id="37610-151">`extra`：额外人员数</span><span class="sxs-lookup"><span data-stu-id="37610-151">`extra`: number of extra people</span></span> | <span data-ttu-id="37610-152">用于将数字呈现在人员列表右侧的最大值之后的模板。</span><span class="sxs-lookup"><span data-stu-id="37610-152">The template used to render the number beyond the max to the right of the list of people.</span></span> |
| `no-data` | <span data-ttu-id="37610-153">不传递数据上下文</span><span class="sxs-lookup"><span data-stu-id="37610-153">No data context is passed</span></span> | <span data-ttu-id="37610-154">没有可用数据时使用的模板。</span><span class="sxs-lookup"><span data-stu-id="37610-154">The template used when no data is available.</span></span> |

<span data-ttu-id="37610-155">下面的示例演示如何使用`person`模板。</span><span class="sxs-lookup"><span data-stu-id="37610-155">The following examples shows how to use the `person` template.</span></span>

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

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="37610-156">Microsoft Graph 权限</span><span class="sxs-lookup"><span data-stu-id="37610-156">Microsoft Graph permissions</span></span>

<span data-ttu-id="37610-157">此组件使用以下 Microsoft Graph Api 和权限：</span><span class="sxs-lookup"><span data-stu-id="37610-157">This component uses the following Microsoft Graph APIs and permissions:</span></span>

| <span data-ttu-id="37610-158">Resource</span><span class="sxs-lookup"><span data-stu-id="37610-158">Resource</span></span> | <span data-ttu-id="37610-159">权限</span><span class="sxs-lookup"><span data-stu-id="37610-159">Permission</span></span> |
| - | - |
| [<span data-ttu-id="37610-160">/me/people</span><span class="sxs-lookup"><span data-stu-id="37610-160">/me/people</span></span>](https://docs.microsoft.com/graph/api/user-list-people?view=graph-rest-1.0) | <span data-ttu-id="37610-161">People.Read</span><span class="sxs-lookup"><span data-stu-id="37610-161">People.Read</span></span> |

## <a name="authentication"></a><span data-ttu-id="37610-162">身份验证</span><span class="sxs-lookup"><span data-stu-id="37610-162">Authentication</span></span>

<span data-ttu-id="37610-163">该控件使用[身份验证文档](./../providers.md)中介绍的全局身份验证提供程序。</span><span class="sxs-lookup"><span data-stu-id="37610-163">The control uses the global authentication provider described in the [authentication documentation](./../providers.md).</span></span>
