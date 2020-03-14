---
title: 人员-选取器组件
description: 您可以使用 "人员-选取器 web 组件" 搜索指定数量的人员，并通过 Microsoft Graph 呈现结果列表。
localization_priority: Normal
author: vogtn
ms.openlocfilehash: 91b11006df02d563902b99c79c4b1ec09bb7e50a
ms.sourcegitcommit: f2dffaca3e1c5b74a01b59e1b76dba1592a6a5d1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/14/2020
ms.locfileid: "42639938"
---
# <a name="people-picker-component"></a><span data-ttu-id="122ba-103">人员-选取器组件</span><span class="sxs-lookup"><span data-stu-id="122ba-103">People-Picker component</span></span>

<span data-ttu-id="122ba-104">您可以使用`mgt-people-picker` web 组件搜索指定数量的人员，并通过 Microsoft Graph 呈现结果列表。</span><span class="sxs-lookup"><span data-stu-id="122ba-104">You can use the `mgt-people-picker` web component search for a specified number of people and render the list of results via Microsoft Graph.</span></span> <span data-ttu-id="122ba-105">默认情况下，组件将搜索所有人员;您还可以定义组属性以进一步筛选结果。</span><span class="sxs-lookup"><span data-stu-id="122ba-105">By default, the component will search for all people; you can also define a group property to further filter the results.</span></span>

<span data-ttu-id="122ba-106">如果要显示的用户数超过此`show-max`值，则不会在搜索列表中显示所有返回的人员数。</span><span class="sxs-lookup"><span data-stu-id="122ba-106">If the number of people to display exceeds the `show-max` value, not all people returned will be displayed in the search list.</span></span>

## <a name="example"></a><span data-ttu-id="122ba-107">示例</span><span class="sxs-lookup"><span data-stu-id="122ba-107">Example</span></span>

<span data-ttu-id="122ba-108">下面的示例演示了`mgt-people-picker`该组件。</span><span class="sxs-lookup"><span data-stu-id="122ba-108">The following example shows the `mgt-people-picker` component.</span></span> <span data-ttu-id="122ba-109">开始搜索名称以查看结果呈现，并使用代码编辑器查看[属性](#properties)如何更改组件的行为。</span><span class="sxs-lookup"><span data-stu-id="122ba-109">Start searching for a name to see the results render and use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-people-picker--people-picker&source=docs" height="450"></iframe>

[<span data-ttu-id="122ba-110">在 "dev" 中打开此示例</span><span class="sxs-lookup"><span data-stu-id="122ba-110">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-people-picker--people-picker&source=docs)

## <a name="properties"></a><span data-ttu-id="122ba-111">属性</span><span class="sxs-lookup"><span data-stu-id="122ba-111">Properties</span></span>

<span data-ttu-id="122ba-112">默认情况下， `mgt-people-picker`组件从`/me/people`终结点提取事件。</span><span class="sxs-lookup"><span data-stu-id="122ba-112">By default, the `mgt-people-picker` component fetches events from the `/me/people` endpoint.</span></span> <span data-ttu-id="122ba-113">使用以下属性来更改此行为。</span><span class="sxs-lookup"><span data-stu-id="122ba-113">Use the following attributes to change this behavior.</span></span>

| <span data-ttu-id="122ba-114">属性</span><span class="sxs-lookup"><span data-stu-id="122ba-114">Attribute</span></span> | <span data-ttu-id="122ba-115">属性</span><span class="sxs-lookup"><span data-stu-id="122ba-115">Property</span></span> | <span data-ttu-id="122ba-116">说明</span><span class="sxs-lookup"><span data-stu-id="122ba-116">Description</span></span>                                                                                                                                                                            |
| -------- | --------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="122ba-117">show-max</span><span class="sxs-lookup"><span data-stu-id="122ba-117">show-max</span></span> | <span data-ttu-id="122ba-118">showMax</span><span class="sxs-lookup"><span data-stu-id="122ba-118">showMax</span></span>   | <span data-ttu-id="122ba-119">一个指示要显示的最大用户数的数字值。</span><span class="sxs-lookup"><span data-stu-id="122ba-119">A number value to indicate the maximum number of people to show.</span></span> <span data-ttu-id="122ba-120">默认值为6。</span><span class="sxs-lookup"><span data-stu-id="122ba-120">the default value is 6.</span></span>                                                                                             |
| <span data-ttu-id="122ba-121">people</span><span class="sxs-lookup"><span data-stu-id="122ba-121">people</span></span>   | <span data-ttu-id="122ba-122">people</span><span class="sxs-lookup"><span data-stu-id="122ba-122">people</span></span>    | <span data-ttu-id="122ba-123">获取或设置组件呈现的人员列表的人员数组。</span><span class="sxs-lookup"><span data-stu-id="122ba-123">An array of people to get or set the list of people rendered by the component.</span></span> <span data-ttu-id="122ba-124">使用此属性可访问组件加载的人员。</span><span class="sxs-lookup"><span data-stu-id="122ba-124">Use this property to access the people loaded by the component.</span></span> <span data-ttu-id="122ba-125">设置此值可加载自己的人员。</span><span class="sxs-lookup"><span data-stu-id="122ba-125">Set this value to load your own people.</span></span> |
| <span data-ttu-id="122ba-126">group</span><span class="sxs-lookup"><span data-stu-id="122ba-126">group</span></span>    | <span data-ttu-id="122ba-127">group</span><span class="sxs-lookup"><span data-stu-id="122ba-127">group</span></span>     | <span data-ttu-id="122ba-128">一个 string 值，属于 Microsoft Graph 定义的组，用于进一步筛选搜索结果。</span><span class="sxs-lookup"><span data-stu-id="122ba-128">A string value that belongs to a Microsoft Graph defined group for further filtering of the search results.</span></span>                                                                            |
|  <span data-ttu-id="122ba-129">选定-人员</span><span class="sxs-lookup"><span data-stu-id="122ba-129">selected-people</span></span>  | <span data-ttu-id="122ba-130">selectedPeople</span><span class="sxs-lookup"><span data-stu-id="122ba-130">selectedPeople</span></span>     | <span data-ttu-id="122ba-131">一个类型`person`的数组，表示在组件中选定的人员。</span><span class="sxs-lookup"><span data-stu-id="122ba-131">An array of type  `person`, representing people selected in the component.</span></span> <span data-ttu-id="122ba-132">将此值设置为 "默认情况下选择所选人员"。</span><span class="sxs-lookup"><span data-stu-id="122ba-132">Set this value to choose selected people by default.</span></span>|

<span data-ttu-id="122ba-133">下面是一个`show-max`示例。</span><span class="sxs-lookup"><span data-stu-id="122ba-133">The following is a `show-max` example.</span></span>

```html
<mgt-people-picker show-max="4"> </mgt-people-picker>
```

## <a name="selected-people"></a><span data-ttu-id="122ba-134">选定人员</span><span class="sxs-lookup"><span data-stu-id="122ba-134">Selected people</span></span>

<span data-ttu-id="122ba-135">组件的 "选定人员" 部分将呈现由开发人员或用户选择的每个人。</span><span class="sxs-lookup"><span data-stu-id="122ba-135">The selected people section of the component renders each person chosen by the developer or user.</span></span> 

![组织-人员-选取器](./images/selected-people.png)

<span data-ttu-id="122ba-137">您可以通过执行下列操作之一来填充所选的人员数据：</span><span class="sxs-lookup"><span data-stu-id="122ba-137">You can populate selected people data by doing one of the following:</span></span>

- <span data-ttu-id="122ba-138">直接设置`selectedPeople`属性，如下面的示例所示。</span><span class="sxs-lookup"><span data-stu-id="122ba-138">Setting the `selectedPeople` property directly, as shown in the following example.</span></span>  

    ```javascript
    // personObject = User or Person from Microsoft Graph
    document.querySelector('mgt-people-picker').selectedPeople.push(personObject);
    ```

- <span data-ttu-id="122ba-139">使用此`selectUsersById()`方法可接受 Microsoft graph[用户 id](https://docs.microsoft.com/graph/api/resources/users?view=graph-rest-1.0)的数组，以查找有关所选内容的相关用户详细信息。</span><span class="sxs-lookup"><span data-stu-id="122ba-139">Using the `selectUsersById()` method, which accepts an array of Microsoft graph [user ids](https://docs.microsoft.com/graph/api/resources/users?view=graph-rest-1.0) to find associated user details for selection.</span></span>

     ><span data-ttu-id="122ba-140">**注意：** 如果找不到用户，则`id`不会为其呈现任何数据`id`。</span><span class="sxs-lookup"><span data-stu-id="122ba-140">**Note:** If no user is found for an `id`, no data will be rendered for that `id`.</span></span>

    ```javascript
    // id = Mirosoft graph User "id"
    document.querySelector('mgt-people-picker').selectUsersById(["id","id"])
    ```

## <a name="css-custom-properties"></a><span data-ttu-id="122ba-141">CSS 自定义属性</span><span class="sxs-lookup"><span data-stu-id="122ba-141">CSS custom properties</span></span>

<span data-ttu-id="122ba-142">`mgt-people-picker`组件定义以下 CSS 自定义属性。</span><span class="sxs-lookup"><span data-stu-id="122ba-142">The `mgt-people-picker` component defines the following CSS custom properties.</span></span>

```css
mgt-people-picker {
  --people-list-background-color: blue; /* Background-color for people under search */
  --accent-color: green; /* Color for separator of search input box and people */
}
```

## <a name="templates"></a><span data-ttu-id="122ba-143">模板</span><span class="sxs-lookup"><span data-stu-id="122ba-143">Templates</span></span>

 <span data-ttu-id="122ba-144">`mgt-people-picker`支持多个模板，这些[模板](../templates.md)可用于替换组件的某些部分。</span><span class="sxs-lookup"><span data-stu-id="122ba-144">`mgt-people-picker` supports several [templates](../templates.md) that you can use to replace certain parts of the component.</span></span> <span data-ttu-id="122ba-145">若要指定模板，请在`<template>`组件内添加一个元素，并`data-type`将值设置为下列值之一。</span><span class="sxs-lookup"><span data-stu-id="122ba-145">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="122ba-146">数据类型</span><span class="sxs-lookup"><span data-stu-id="122ba-146">Data type</span></span> | <span data-ttu-id="122ba-147">数据上下文</span><span class="sxs-lookup"><span data-stu-id="122ba-147">Data context</span></span> | <span data-ttu-id="122ba-148">说明</span><span class="sxs-lookup"><span data-stu-id="122ba-148">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="122ba-149">装载</span><span class="sxs-lookup"><span data-stu-id="122ba-149">loading</span></span> | <span data-ttu-id="122ba-150">null：无数据</span><span class="sxs-lookup"><span data-stu-id="122ba-150">null: no data</span></span> | <span data-ttu-id="122ba-151">在发出对 graph 的请求时用于呈现选取器状态的模板。</span><span class="sxs-lookup"><span data-stu-id="122ba-151">The template used to render the state of picker while request to graph is being made.</span></span> |
| <span data-ttu-id="122ba-152">error</span><span class="sxs-lookup"><span data-stu-id="122ba-152">error</span></span> | <span data-ttu-id="122ba-153">null：无数据</span><span class="sxs-lookup"><span data-stu-id="122ba-153">null: no data</span></span>| <span data-ttu-id="122ba-154">用户搜索不返回用户时使用的模板。</span><span class="sxs-lookup"><span data-stu-id="122ba-154">The template used if user search returns no users.</span></span> |
| <span data-ttu-id="122ba-155">选定的人员</span><span class="sxs-lookup"><span data-stu-id="122ba-155">selected-person</span></span> |<span data-ttu-id="122ba-156">人员：人员详细信息对象</span><span class="sxs-lookup"><span data-stu-id="122ba-156">person: The person details object</span></span>| <span data-ttu-id="122ba-157">呈现所选人员的模板。</span><span class="sxs-lookup"><span data-stu-id="122ba-157">The template to render selected people.</span></span> |
| <span data-ttu-id="122ba-158">朋友</span><span class="sxs-lookup"><span data-stu-id="122ba-158">person</span></span> | <span data-ttu-id="122ba-159">人员：人员详细信息对象</span><span class="sxs-lookup"><span data-stu-id="122ba-159">person: The person details object</span></span>| <span data-ttu-id="122ba-160">用于在下拉列表中呈现人员的模板。</span><span class="sxs-lookup"><span data-stu-id="122ba-160">The template to render people in the dropdown.</span></span> |

<span data-ttu-id="122ba-161">下面的示例演示如何使用`error`模板。</span><span class="sxs-lookup"><span data-stu-id="122ba-161">The following examples shows how to use the `error` template.</span></span>

```html
<mgt-people-picker>
  <template data-type="error">
    <p>Sorry, no people were found</p>
  </template>
</mgt-people-picker>
```

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="122ba-162">Microsoft Graph 权限</span><span class="sxs-lookup"><span data-stu-id="122ba-162">Microsoft Graph permissions</span></span>

<span data-ttu-id="122ba-163">此组件使用以下 Microsoft Graph Api 和权限。</span><span class="sxs-lookup"><span data-stu-id="122ba-163">This component uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="122ba-164">API</span><span class="sxs-lookup"><span data-stu-id="122ba-164">API</span></span>                                                                                                              | <span data-ttu-id="122ba-165">权限</span><span class="sxs-lookup"><span data-stu-id="122ba-165">Permission</span></span>  |
| ---------------------------------------------------------------------------------------------------------------- | ----------- |
| [<span data-ttu-id="122ba-166">/me/people</span><span class="sxs-lookup"><span data-stu-id="122ba-166">/me/people</span></span>](/graph/api/user-list-people?view=graph-rest-1.0)                    | <span data-ttu-id="122ba-167">People.Read</span><span class="sxs-lookup"><span data-stu-id="122ba-167">People.Read</span></span>        |
| [<span data-ttu-id="122ba-168">/groups/\${groupId}/members</span><span class="sxs-lookup"><span data-stu-id="122ba-168">/groups/\${groupId}/members</span></span>](/graph/api/group-list-members?view=graph-rest-1.0) | <span data-ttu-id="122ba-169">People.Read</span><span class="sxs-lookup"><span data-stu-id="122ba-169">People.Read</span></span>        |
| [<span data-ttu-id="122ba-170">/users/$ {userPrincipleName}</span><span class="sxs-lookup"><span data-stu-id="122ba-170">/users/${userPrincipleName} </span></span>](/graph/api/user-list-people?view=graph-rest-1.0)  | <span data-ttu-id="122ba-171">User.readbasic.all</span><span class="sxs-lookup"><span data-stu-id="122ba-171">User.Readbasic.All</span></span> |

## <a name="authentication"></a><span data-ttu-id="122ba-172">身份验证</span><span class="sxs-lookup"><span data-stu-id="122ba-172">Authentication</span></span>

<span data-ttu-id="122ba-173">该控件使用[身份验证文档](./../providers.md)中介绍的全局身份验证提供程序。</span><span class="sxs-lookup"><span data-stu-id="122ba-173">The control uses the global authentication provider described in the [authentication documentation](./../providers.md).</span></span>
