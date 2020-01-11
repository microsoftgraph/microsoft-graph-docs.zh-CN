---
title: 人员-选取器组件
description: 您可以使用 "人员-选取器 web 组件" 搜索指定数量的人员，并通过 Microsoft Graph 呈现结果列表。
localization_priority: Normal
author: vogtn
ms.openlocfilehash: 65ff9382de97ddcd7a0b4bd8a315f8350a80ec35
ms.sourcegitcommit: 2a601cffdb8df375b2ee32a1f35b8f71e0ffd04f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2020
ms.locfileid: "41023122"
---
# <a name="people-picker-component"></a><span data-ttu-id="a0599-103">人员-选取器组件</span><span class="sxs-lookup"><span data-stu-id="a0599-103">People-Picker component</span></span>

<span data-ttu-id="a0599-104">您可以使用`mgt-people-picker` web 组件搜索指定数量的人员，并通过 Microsoft Graph 呈现结果列表。</span><span class="sxs-lookup"><span data-stu-id="a0599-104">You can use the `mgt-people-picker` web component search for a specified number of people and render the list of results via Microsoft Graph.</span></span> <span data-ttu-id="a0599-105">默认情况下，组件将搜索所有人员;您还可以定义组属性以进一步筛选结果。</span><span class="sxs-lookup"><span data-stu-id="a0599-105">By default, the component will search for all people; you can also define a group property to further filter the results.</span></span>

<span data-ttu-id="a0599-106">如果要显示的用户数超过此`show-max`值，则不会在搜索列表中显示所有返回的人员数。</span><span class="sxs-lookup"><span data-stu-id="a0599-106">If the number of people to display exceeds the `show-max` value, not all people returned will be displayed in the search list.</span></span>

## <a name="example"></a><span data-ttu-id="a0599-107">示例</span><span class="sxs-lookup"><span data-stu-id="a0599-107">Example</span></span>

[<span data-ttu-id="a0599-108">jsfiddle 示例</span><span class="sxs-lookup"><span data-stu-id="a0599-108">jsfiddle example</span></span>](https://jsfiddle.net/metulev/jdv38fg0/)

```html
<mgt-people-picker></mgt-people-picker>
```

![组织-人员-选取器](./images/mgt-people-picker-image.png)

## <a name="properties"></a><span data-ttu-id="a0599-110">属性</span><span class="sxs-lookup"><span data-stu-id="a0599-110">Properties</span></span>

<span data-ttu-id="a0599-111">默认情况下， `mgt-people-picker`组件从`/me/people`终结点提取事件。</span><span class="sxs-lookup"><span data-stu-id="a0599-111">By default, the `mgt-people-picker` component fetches events from the `/me/people` endpoint.</span></span> <span data-ttu-id="a0599-112">使用以下属性来更改此行为。</span><span class="sxs-lookup"><span data-stu-id="a0599-112">Use the following attributes to change this behavior.</span></span>

| <span data-ttu-id="a0599-113">属性</span><span class="sxs-lookup"><span data-stu-id="a0599-113">Attribute</span></span> | <span data-ttu-id="a0599-114">属性</span><span class="sxs-lookup"><span data-stu-id="a0599-114">Property</span></span> | <span data-ttu-id="a0599-115">说明</span><span class="sxs-lookup"><span data-stu-id="a0599-115">Description</span></span>                                                                                                                                                                            |
| -------- | --------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="a0599-116">show-max</span><span class="sxs-lookup"><span data-stu-id="a0599-116">show-max</span></span> | <span data-ttu-id="a0599-117">showMax</span><span class="sxs-lookup"><span data-stu-id="a0599-117">showMax</span></span>   | <span data-ttu-id="a0599-118">一个指示要显示的最大用户数的数字值。</span><span class="sxs-lookup"><span data-stu-id="a0599-118">A number value to indicate the maximum number of people to show.</span></span> <span data-ttu-id="a0599-119">默认值为6。</span><span class="sxs-lookup"><span data-stu-id="a0599-119">the default value is 6.</span></span>                                                                                             |
| <span data-ttu-id="a0599-120">people</span><span class="sxs-lookup"><span data-stu-id="a0599-120">people</span></span>   | <span data-ttu-id="a0599-121">people</span><span class="sxs-lookup"><span data-stu-id="a0599-121">people</span></span>    | <span data-ttu-id="a0599-122">获取或设置组件呈现的人员列表的人员数组。</span><span class="sxs-lookup"><span data-stu-id="a0599-122">An array of people to get or set the list of people rendered by the component.</span></span> <span data-ttu-id="a0599-123">使用此属性可访问组件加载的人员。</span><span class="sxs-lookup"><span data-stu-id="a0599-123">Use this property to access the people loaded by the component.</span></span> <span data-ttu-id="a0599-124">设置此值可加载自己的人员。</span><span class="sxs-lookup"><span data-stu-id="a0599-124">Set this value to load your own people.</span></span> |
| <span data-ttu-id="a0599-125">group</span><span class="sxs-lookup"><span data-stu-id="a0599-125">group</span></span>    | <span data-ttu-id="a0599-126">group</span><span class="sxs-lookup"><span data-stu-id="a0599-126">group</span></span>     | <span data-ttu-id="a0599-127">一个 string 值，属于 Microsoft Graph 定义的组，用于进一步筛选搜索结果。</span><span class="sxs-lookup"><span data-stu-id="a0599-127">A string value that belongs to a Microsoft Graph defined group for further filtering of the search results.</span></span>                                                                            |
|  <span data-ttu-id="a0599-128">选定-人员</span><span class="sxs-lookup"><span data-stu-id="a0599-128">selected-people</span></span>  | <span data-ttu-id="a0599-129">selectedPeople</span><span class="sxs-lookup"><span data-stu-id="a0599-129">selectedPeople</span></span>     | <span data-ttu-id="a0599-130">一个类型`person`的数组，表示在组件中选定的人员。</span><span class="sxs-lookup"><span data-stu-id="a0599-130">An array of type  `person`, representing people selected in the component.</span></span> <span data-ttu-id="a0599-131">将此值设置为 "默认情况下选择所选人员"。</span><span class="sxs-lookup"><span data-stu-id="a0599-131">Set this value to choose selected people by default.</span></span>|

<span data-ttu-id="a0599-132">下面是一个`show-max`示例。</span><span class="sxs-lookup"><span data-stu-id="a0599-132">The following is a `show-max` example.</span></span>

```html
<mgt-people-picker show-max="4"> </mgt-people-picker>
```

## <a name="selected-people"></a><span data-ttu-id="a0599-133">选定人员</span><span class="sxs-lookup"><span data-stu-id="a0599-133">Selected people</span></span>

<span data-ttu-id="a0599-134">组件的 "选定人员" 部分将呈现由开发人员或用户选择的每个人。</span><span class="sxs-lookup"><span data-stu-id="a0599-134">The selected people section of the component renders each person chosen by the developer or user.</span></span> 

![组织-人员-选取器](./images/selected-people.png)

<span data-ttu-id="a0599-136">您可以通过执行下列操作之一来填充所选的人员数据：</span><span class="sxs-lookup"><span data-stu-id="a0599-136">You can populate selected people data by doing one of the following:</span></span>

- <span data-ttu-id="a0599-137">直接设置`selectedPeople`属性，如下面的示例所示。</span><span class="sxs-lookup"><span data-stu-id="a0599-137">Setting the `selectedPeople` property directly, as shown in the following example.</span></span>  

    ```javascript
    // personObject = User or Person from Microsoft Graph
    document.querySelector('mgt-people-picker').selectedPeople.push(personObject);
    ```

- <span data-ttu-id="a0599-138">使用此`selectUsersById()`方法可接受 Microsoft graph[用户 id](https://docs.microsoft.com/graph/api/resources/users?view=graph-rest-1.0)的数组，以查找有关所选内容的相关用户详细信息。</span><span class="sxs-lookup"><span data-stu-id="a0599-138">Using the `selectUsersById()` method, which accepts an array of Microsoft graph [user ids](https://docs.microsoft.com/graph/api/resources/users?view=graph-rest-1.0) to find associated user details for selection.</span></span>

     ><span data-ttu-id="a0599-139">**注意：** 如果找不到用户，则`id`不会为其呈现任何数据`id`。</span><span class="sxs-lookup"><span data-stu-id="a0599-139">**Note:** If no user is found for an `id`, no data will be rendered for that `id`.</span></span>

    ```javascript
    // id = Mirosoft graph User "id"
    document.querySelector('mgt-people-picker').selectUsersById(["id","id"])
    ```

## <a name="css-custom-properties"></a><span data-ttu-id="a0599-140">CSS 自定义属性</span><span class="sxs-lookup"><span data-stu-id="a0599-140">CSS custom properties</span></span>

<span data-ttu-id="a0599-141">`mgt-people-picker`组件定义以下 CSS 自定义属性。</span><span class="sxs-lookup"><span data-stu-id="a0599-141">The `mgt-people-picker` component defines the following CSS custom properties.</span></span>

```css
mgt-people-picker {
  --people-list-background-color: blue; /* Background-color for people under search */
  --accent-color: green; /* Color for separator of search input box and people */
}
```

## <a name="templates"></a><span data-ttu-id="a0599-142">模板</span><span class="sxs-lookup"><span data-stu-id="a0599-142">Templates</span></span>

 <span data-ttu-id="a0599-143">`mgt-people-picker`支持多个模板，这些[模板](../templates.md)可用于替换组件的某些部分。</span><span class="sxs-lookup"><span data-stu-id="a0599-143">`mgt-people-picker` supports several [templates](../templates.md) that you can use to replace certain parts of the component.</span></span> <span data-ttu-id="a0599-144">若要指定模板，请在`<template>`组件内添加一个元素，并`data-type`将值设置为下列值之一。</span><span class="sxs-lookup"><span data-stu-id="a0599-144">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="a0599-145">数据类型</span><span class="sxs-lookup"><span data-stu-id="a0599-145">Data type</span></span> | <span data-ttu-id="a0599-146">数据上下文</span><span class="sxs-lookup"><span data-stu-id="a0599-146">Data context</span></span> | <span data-ttu-id="a0599-147">Description</span><span class="sxs-lookup"><span data-stu-id="a0599-147">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="a0599-148">装载</span><span class="sxs-lookup"><span data-stu-id="a0599-148">loading</span></span> | <span data-ttu-id="a0599-149">null：无数据</span><span class="sxs-lookup"><span data-stu-id="a0599-149">null: no data</span></span> | <span data-ttu-id="a0599-150">在发出对 graph 的请求时用于呈现选取器状态的模板。</span><span class="sxs-lookup"><span data-stu-id="a0599-150">The template used to render the state of picker while request to graph is being made.</span></span> |
| <span data-ttu-id="a0599-151">error</span><span class="sxs-lookup"><span data-stu-id="a0599-151">error</span></span> | <span data-ttu-id="a0599-152">null：无数据</span><span class="sxs-lookup"><span data-stu-id="a0599-152">null: no data</span></span>| <span data-ttu-id="a0599-153">用户搜索不返回用户时使用的模板。</span><span class="sxs-lookup"><span data-stu-id="a0599-153">The template used if user search returns no users.</span></span> |
| <span data-ttu-id="a0599-154">选定的人员</span><span class="sxs-lookup"><span data-stu-id="a0599-154">selected-person</span></span> |<span data-ttu-id="a0599-155">人员：人员详细信息对象</span><span class="sxs-lookup"><span data-stu-id="a0599-155">person: The person details object</span></span>| <span data-ttu-id="a0599-156">呈现所选人员的模板。</span><span class="sxs-lookup"><span data-stu-id="a0599-156">The template to render selected people.</span></span> |
| <span data-ttu-id="a0599-157">朋友</span><span class="sxs-lookup"><span data-stu-id="a0599-157">person</span></span> | <span data-ttu-id="a0599-158">人员：人员详细信息对象</span><span class="sxs-lookup"><span data-stu-id="a0599-158">person: The person details object</span></span>| <span data-ttu-id="a0599-159">用于在下拉列表中呈现人员的模板。</span><span class="sxs-lookup"><span data-stu-id="a0599-159">The template to render people in the dropdown.</span></span> |

<span data-ttu-id="a0599-160">下面的示例演示如何使用`error`模板。</span><span class="sxs-lookup"><span data-stu-id="a0599-160">The following examples shows how to use the `error` template.</span></span>

```html
<mgt-people-picker>
  <template data-type="error">
    <p>Sorry, no people were found</p>
  </template>
</mgt-people-picker>
```

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="a0599-161">Microsoft Graph 权限</span><span class="sxs-lookup"><span data-stu-id="a0599-161">Microsoft Graph permissions</span></span>

<span data-ttu-id="a0599-162">此组件使用以下 Microsoft Graph Api 和权限。</span><span class="sxs-lookup"><span data-stu-id="a0599-162">This component uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="a0599-163">API</span><span class="sxs-lookup"><span data-stu-id="a0599-163">API</span></span>                                                                                                              | <span data-ttu-id="a0599-164">权限</span><span class="sxs-lookup"><span data-stu-id="a0599-164">Permission</span></span>  |
| ---------------------------------------------------------------------------------------------------------------- | ----------- |
| [<span data-ttu-id="a0599-165">/me/people</span><span class="sxs-lookup"><span data-stu-id="a0599-165">/me/people</span></span>](/graph/api/user-list-people?view=graph-rest-1.0)                    | <span data-ttu-id="a0599-166">People.Read</span><span class="sxs-lookup"><span data-stu-id="a0599-166">People.Read</span></span>        |
| [<span data-ttu-id="a0599-167">/groups/\${groupId}/members</span><span class="sxs-lookup"><span data-stu-id="a0599-167">/groups/\${groupId}/members</span></span>](/graph/api/group-list-members?view=graph-rest-1.0) | <span data-ttu-id="a0599-168">People.Read</span><span class="sxs-lookup"><span data-stu-id="a0599-168">People.Read</span></span>        |
| [<span data-ttu-id="a0599-169">/users/$ {userPrincipleName}</span><span class="sxs-lookup"><span data-stu-id="a0599-169">/users/${userPrincipleName} </span></span>](/graph/api/user-list-people?view=graph-rest-1.0)  | <span data-ttu-id="a0599-170">User.readbasic.all</span><span class="sxs-lookup"><span data-stu-id="a0599-170">User.Readbasic.All</span></span> |

## <a name="authentication"></a><span data-ttu-id="a0599-171">身份验证</span><span class="sxs-lookup"><span data-stu-id="a0599-171">Authentication</span></span>

<span data-ttu-id="a0599-172">该控件使用[身份验证文档](./../providers.md)中介绍的全局身份验证提供程序。</span><span class="sxs-lookup"><span data-stu-id="a0599-172">The control uses the global authentication provider described in the [authentication documentation](./../providers.md).</span></span>
