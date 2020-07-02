---
title: Microsoft Graph 工具包中的 "人员" 组件
description: "\"人员\" 组件用于通过使用其照片、姓名和/或电子邮件地址显示人员或联系人。"
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 7fc3430755c08662186e235cd83d8790968f9ae3
ms.sourcegitcommit: 05645bc582d14781a9ca6b78ed598a4e7dc26869
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/01/2020
ms.locfileid: "44990239"
---
# <a name="person-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="ada63-103">Microsoft Graph 工具包中的 "人员" 组件</span><span class="sxs-lookup"><span data-stu-id="ada63-103">Person component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="ada63-104">"人员" 组件用于通过使用照片、姓名、电子邮件地址或任何其他人员详细信息来显示个人或联系人。</span><span class="sxs-lookup"><span data-stu-id="ada63-104">The person component is used to display a person or contact by using their photo, name, email address, or any other person details.</span></span>

<span data-ttu-id="ada63-105">"人员" 组件还使用 "管理员-[卡片](./person-card.md)" 显示带有有关用户的其他信息的飞出卡片。</span><span class="sxs-lookup"><span data-stu-id="ada63-105">The person component also uses the [mgt-person-card](./person-card.md) to display a flyout card with additional information about the user.</span></span> <span data-ttu-id="ada63-106">有关详细信息，请参阅 "[人员卡片](#person-card)" 部分。</span><span class="sxs-lookup"><span data-stu-id="ada63-106">For details, see the [Person Card](#person-card) section.</span></span>

## <a name="example"></a><span data-ttu-id="ada63-107">示例</span><span class="sxs-lookup"><span data-stu-id="ada63-107">Example</span></span>

<span data-ttu-id="ada63-108">下面的示例显示使用组件的人员 `mgt-person` 。</span><span class="sxs-lookup"><span data-stu-id="ada63-108">The following example displays a person using the `mgt-person` component.</span></span> <span data-ttu-id="ada63-109">您可以使用代码编辑器来查看[属性](#properties)如何更改组件的行为。</span><span class="sxs-lookup"><span data-stu-id="ada63-109">You can use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-person--person&source=docs" height="250"></iframe>

[<span data-ttu-id="ada63-110">在 "dev" 中打开此示例</span><span class="sxs-lookup"><span data-stu-id="ada63-110">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-person--person&source=docs)

## <a name="setting-the-person-details"></a><span data-ttu-id="ada63-111">设置人员详细信息</span><span class="sxs-lookup"><span data-stu-id="ada63-111">Setting the person details</span></span>

<span data-ttu-id="ada63-112">您可以使用三个属性来设置人员详细信息。</span><span class="sxs-lookup"><span data-stu-id="ada63-112">You can use three properties to set the person details.</span></span> <span data-ttu-id="ada63-113">每个实例仅使用下列属性之一：</span><span class="sxs-lookup"><span data-stu-id="ada63-113">Use only one of the following properties per instance:</span></span>

* <span data-ttu-id="ada63-114">`user-id` `userId` 通过使用其 ID 将属性或属性设置为从 Microsoft Graph 获取用户。</span><span class="sxs-lookup"><span data-stu-id="ada63-114">Set the `user-id` attribute or `userId` property to fetch the user from Microsoft Graph by using their ID.</span></span>

* <span data-ttu-id="ada63-115">将 `person-query` 属性或 `personQuery` 属性设置为在 Microsoft Graph 中搜索给定人员。</span><span class="sxs-lookup"><span data-stu-id="ada63-115">Set the `person-query` attribute or `personQuery` property to search Microsoft Graph for a given person.</span></span> <span data-ttu-id="ada63-116">它将选择第一个可用的人员并获取人员详细信息。</span><span class="sxs-lookup"><span data-stu-id="ada63-116">It will choose the first person available and fetch the person details.</span></span> <span data-ttu-id="ada63-117">电子邮件最适用于确保查询的是正确的人员，但名称也有效。</span><span class="sxs-lookup"><span data-stu-id="ada63-117">An email works best to ensure the right person is queried, but a name works as well.</span></span>

* <span data-ttu-id="ada63-118">将 `person-presence` 属性或 `personPresence` 属性设置为手动向用户头像添加状态标记。</span><span class="sxs-lookup"><span data-stu-id="ada63-118">Set the `person-presence` attribute or `personPresence` property to add a presence badge to person avatar manually.</span></span>

* <span data-ttu-id="ada63-119">将 `avatar-size` 属性或 `avatarSize` 属性设置为 `small` 或 `large` 以确定头像的大小。</span><span class="sxs-lookup"><span data-stu-id="ada63-119">Set the `avatar-size` attribute or `avatarSize` property to `small` or `large` to determine the size of avatar.</span></span> <span data-ttu-id="ada63-120">这有助于将[正确的状态标记](https://mgt.dev/?path=/story/components-mgt-person--person-presence-display-all)添加到头像。</span><span class="sxs-lookup"><span data-stu-id="ada63-120">This helps add the [correct presence badge](https://mgt.dev/?path=/story/components-mgt-person--person-presence-display-all) to avatar.</span></span> <span data-ttu-id="ada63-121">你将需要选择下面显示的正确的相应 css 自定义属性，以进一步自定义头像大小。</span><span class="sxs-lookup"><span data-stu-id="ada63-121">You will need to choose the correct corresponding css custom properties shown below to further customize avatar size.</span></span> <span data-ttu-id="ada63-122">默认情况下，此值设置为 `auto` 将自动决定如何基于属性呈现状态 `view` 。</span><span class="sxs-lookup"><span data-stu-id="ada63-122">By default, the value is set to `auto` which will automatically decide how to render the presence based on the `view` property.</span></span> <span data-ttu-id="ada63-123">`small`如果你的头像小于32，我们建议使用32。</span><span class="sxs-lookup"><span data-stu-id="ada63-123">We recommend using `small` if your avatar is smaller than 32px by 32px.</span></span> 

* <span data-ttu-id="ada63-124">使用 `person-details` 属性或 `personDetails` 属性可手动设置人员详细信息，如下面的示例所示。</span><span class="sxs-lookup"><span data-stu-id="ada63-124">Use the `person-details` attribute or `personDetails` property to manually set the person details, as shown in the following example.</span></span>


    ```js
    let personControl = document.getElementById('myPersonControl');
    personControl.personDetails = {
        displayName: 'Nikola Metulev',
        mail: 'nikola@contoso.com',
        personImage: 'url'
    }
    ```

  <span data-ttu-id="ada63-125">如果未提供图像，则将获取一个图像（如果可用）。</span><span class="sxs-lookup"><span data-stu-id="ada63-125">If no image is provided, one will be fetched (if available).</span></span>

## <a name="properties"></a><span data-ttu-id="ada63-126">属性</span><span class="sxs-lookup"><span data-stu-id="ada63-126">Properties</span></span>

<span data-ttu-id="ada63-127">您可以使用多个属性来自定义组件。</span><span class="sxs-lookup"><span data-stu-id="ada63-127">You can use several properties to customize the component.</span></span>

| <span data-ttu-id="ada63-128">属性</span><span class="sxs-lookup"><span data-stu-id="ada63-128">Attribute</span></span>       | <span data-ttu-id="ada63-129">属性</span><span class="sxs-lookup"><span data-stu-id="ada63-129">Property</span></span>       | <span data-ttu-id="ada63-130">说明</span><span class="sxs-lookup"><span data-stu-id="ada63-130">Description</span></span>                                                   |
| -----------     | ----------     | ------------------------------------------------------------- |
| <span data-ttu-id="ada63-131">用户 id</span><span class="sxs-lookup"><span data-stu-id="ada63-131">user-id</span></span>         | <span data-ttu-id="ada63-132">userId</span><span class="sxs-lookup"><span data-stu-id="ada63-132">userId</span></span>         | <span data-ttu-id="ada63-133">设置为用户 id，以从 Microsoft Graph 中获取该用户的详细信息和图像。</span><span class="sxs-lookup"><span data-stu-id="ada63-133">Set to a user id to fetch that user's details and image from Microsoft Graph.</span></span>|
| <span data-ttu-id="ada63-134">人员-查询</span><span class="sxs-lookup"><span data-stu-id="ada63-134">person-query</span></span>    | <span data-ttu-id="ada63-135">personQuery</span><span class="sxs-lookup"><span data-stu-id="ada63-135">personQuery</span></span>    | <span data-ttu-id="ada63-136">设置为要在 Microsoft Graph 中搜索人员的人员的姓名或电子邮件，并提取第一个人员的详细信息和图像。</span><span class="sxs-lookup"><span data-stu-id="ada63-136">Set to a name or email of a person to search for a person in Microsoft Graph and fetch the first person's details and image.</span></span>|
| <span data-ttu-id="ada63-137">人员-详细信息</span><span class="sxs-lookup"><span data-stu-id="ada63-137">person-details</span></span>  | <span data-ttu-id="ada63-138">personDetails</span><span class="sxs-lookup"><span data-stu-id="ada63-138">personDetails</span></span>  | <span data-ttu-id="ada63-139">设置为代表人员的对象。</span><span class="sxs-lookup"><span data-stu-id="ada63-139">Set to an object representing a person.</span></span> <span data-ttu-id="ada63-140">使用来自人员、用户、联系人或组资源的对象。</span><span class="sxs-lookup"><span data-stu-id="ada63-140">Works with object from the people, users, contacts, or group, resources.</span></span> |
| <span data-ttu-id="ada63-141">人员-图像</span><span class="sxs-lookup"><span data-stu-id="ada63-141">person-image</span></span>    | <span data-ttu-id="ada63-142">personImage</span><span class="sxs-lookup"><span data-stu-id="ada63-142">personImage</span></span>    | <span data-ttu-id="ada63-143">设置要为此人显示的图像。</span><span class="sxs-lookup"><span data-stu-id="ada63-143">Set the image to show for the person.</span></span> |
| <span data-ttu-id="ada63-144">人员-状态</span><span class="sxs-lookup"><span data-stu-id="ada63-144">person-presence</span></span> | <span data-ttu-id="ada63-145">personPresence</span><span class="sxs-lookup"><span data-stu-id="ada63-145">personPresence</span></span> | <span data-ttu-id="ada63-146">设置人员的状态。</span><span class="sxs-lookup"><span data-stu-id="ada63-146">Set the presence for the person.</span></span> |
| <span data-ttu-id="ada63-147">提取-图像</span><span class="sxs-lookup"><span data-stu-id="ada63-147">fetch-image</span></span>     | <span data-ttu-id="ada63-148">fetchImage</span><span class="sxs-lookup"><span data-stu-id="ada63-148">fetchImage</span></span>     | <span data-ttu-id="ada63-149">将标志设置为 `personImage` 根据用户提供的对象从 Microsoft Graph 自动获取 `personDetails` 。</span><span class="sxs-lookup"><span data-stu-id="ada63-149">Set flag to fetch `personImage` automatically from Microsoft Graph based on the `personDetails` object provided by the user.</span></span> |
| <span data-ttu-id="ada63-150">view</span><span class="sxs-lookup"><span data-stu-id="ada63-150">view</span></span>            | <span data-ttu-id="ada63-151">view</span><span class="sxs-lookup"><span data-stu-id="ada63-151">view</span></span>           | <span data-ttu-id="ada63-152">设置以控制如何呈现该人员。</span><span class="sxs-lookup"><span data-stu-id="ada63-152">Set to control how the person is rendered.</span></span> <span data-ttu-id="ada63-153">默认值为`avatar`</span><span class="sxs-lookup"><span data-stu-id="ada63-153">Default is `avatar`</span></span> <br /> <span data-ttu-id="ada63-154">`avatar`-仅显示头像</span><span class="sxs-lookup"><span data-stu-id="ada63-154">`avatar` - show only avatar</span></span> <br /> <span data-ttu-id="ada63-155">`oneline`-显示头像和第一行（ `displayName` 默认情况下）</span><span class="sxs-lookup"><span data-stu-id="ada63-155">`oneline` - show avatar and first line (`displayName` by default)</span></span> <br /> <span data-ttu-id="ada63-156">`twolines`-显示头像和两行文本（ `displayName` `mail` 默认情况下）</span><span class="sxs-lookup"><span data-stu-id="ada63-156">`twolines` - show avatar and two lines of text (`displayName` and `mail` by default)</span></span>|
| <span data-ttu-id="ada63-157">line1-属性</span><span class="sxs-lookup"><span data-stu-id="ada63-157">line1-property</span></span>  | <span data-ttu-id="ada63-158">line1Property</span><span class="sxs-lookup"><span data-stu-id="ada63-158">line1Property</span></span>  | <span data-ttu-id="ada63-159">设置要用于第一行文本的 personDetails 的属性。</span><span class="sxs-lookup"><span data-stu-id="ada63-159">Sets the property of the personDetails to use for the first line of text.</span></span> <span data-ttu-id="ada63-160">默认值为 `displayName`。</span><span class="sxs-lookup"><span data-stu-id="ada63-160">Default is `displayName`.</span></span>|
| <span data-ttu-id="ada63-161">line2-属性</span><span class="sxs-lookup"><span data-stu-id="ada63-161">line2-property</span></span>  | <span data-ttu-id="ada63-162">line2Property</span><span class="sxs-lookup"><span data-stu-id="ada63-162">line2Property</span></span>  | <span data-ttu-id="ada63-163">设置要用于第二行文本的 personDetails 的属性。</span><span class="sxs-lookup"><span data-stu-id="ada63-163">Sets the property of the personDetails to use for the second line of text.</span></span> <span data-ttu-id="ada63-164">默认值为 `mail`。</span><span class="sxs-lookup"><span data-stu-id="ada63-164">Default is `mail`.</span></span>|
| <span data-ttu-id="ada63-165">展示-状态</span><span class="sxs-lookup"><span data-stu-id="ada63-165">show-presence</span></span>   | <span data-ttu-id="ada63-166">showPresence</span><span class="sxs-lookup"><span data-stu-id="ada63-166">showPresence</span></span>   | <span data-ttu-id="ada63-167">设置显示人员状态的标志-默认值为 `false` 。</span><span class="sxs-lookup"><span data-stu-id="ada63-167">Set flag to display person presence - default is `false`.</span></span>|
| <span data-ttu-id="ada63-168">显示-名称</span><span class="sxs-lookup"><span data-stu-id="ada63-168">show-name</span></span>       | <span data-ttu-id="ada63-169">showName</span><span class="sxs-lookup"><span data-stu-id="ada63-169">showName</span></span>       | <span data-ttu-id="ada63-170">**已弃用-使用 `view` 。**</span><span class="sxs-lookup"><span data-stu-id="ada63-170">**DEPRECATED - use `view`.**</span></span>  <span data-ttu-id="ada63-171">设置用于显示人员显示名称的标志-默认为 `false` 。</span><span class="sxs-lookup"><span data-stu-id="ada63-171">Set flag to display person display name - default is `false`.</span></span> |
| <span data-ttu-id="ada63-172">显示-电子邮件</span><span class="sxs-lookup"><span data-stu-id="ada63-172">show-email</span></span>      | <span data-ttu-id="ada63-173">showEmail</span><span class="sxs-lookup"><span data-stu-id="ada63-173">showEmail</span></span>      | <span data-ttu-id="ada63-174">**已弃用-使用 `view` 。**</span><span class="sxs-lookup"><span data-stu-id="ada63-174">**DEPRECATED - use `view`.**</span></span> <span data-ttu-id="ada63-175">设置用于显示个人电子邮件的标志-默认为 `false` 。</span><span class="sxs-lookup"><span data-stu-id="ada63-175">Set flag to display person email - default is `false`.</span></span>        |

## <a name="css-custom-properties"></a><span data-ttu-id="ada63-176">CSS 自定义属性</span><span class="sxs-lookup"><span data-stu-id="ada63-176">CSS custom properties</span></span>

<span data-ttu-id="ada63-177">`mgt-person`组件定义以下 CSS 自定义属性。</span><span class="sxs-lookup"><span data-stu-id="ada63-177">The `mgt-person` component defines the following CSS custom properties.</span></span>

```css
mgt-person {
  --avatar-size: 48px;
  --avatar-border: 0;
  --avatar-border-radius: 50%;
  --initials-color: white;
  --initials-background-color: magenta;
  --font-family: 'Segoe UI';
  --font-size: 14px;
  --font-weight: 500;
  --color: black;
  --background-color: #ffffff;
  --text-transform: none;
  --line2-font-size: 12px;
  --line2-font-weight: 400;
  --line2-color: black;
  --line2-text-transform: none;
  --details-spacing: 12px;
}
```

<span data-ttu-id="ada63-178">若要了解详细信息，请参阅[样式组件](../style.md)。</span><span class="sxs-lookup"><span data-stu-id="ada63-178">To learn more, see [styling components](../style.md).</span></span>

## <a name="templates"></a><span data-ttu-id="ada63-179">模板</span><span class="sxs-lookup"><span data-stu-id="ada63-179">Templates</span></span>

<span data-ttu-id="ada63-180">`mgt-person`组件支持多个[模板](../templates.md)，这些模板允许您替换组件的某些部分。</span><span class="sxs-lookup"><span data-stu-id="ada63-180">The `mgt-person` component supports several [templates](../templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="ada63-181">若要指定模板，请在 `<template>` 组件内添加一个元素，并将 `data-type` 值设置为下列值之一：</span><span class="sxs-lookup"><span data-stu-id="ada63-181">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following:</span></span>

| <span data-ttu-id="ada63-182">数据类型</span><span class="sxs-lookup"><span data-stu-id="ada63-182">Data type</span></span> | <span data-ttu-id="ada63-183">数据上下文</span><span class="sxs-lookup"><span data-stu-id="ada63-183">Data context</span></span> | <span data-ttu-id="ada63-184">说明</span><span class="sxs-lookup"><span data-stu-id="ada63-184">Description</span></span> |
| --------- | ------------ | ----------- |
| <span data-ttu-id="ada63-185">装载</span><span class="sxs-lookup"><span data-stu-id="ada63-185">loading</span></span> | <span data-ttu-id="ada63-186">无</span><span class="sxs-lookup"><span data-stu-id="ada63-186">none</span></span> | <span data-ttu-id="ada63-187">要在组件处于 laoding 状态时呈现的模板。</span><span class="sxs-lookup"><span data-stu-id="ada63-187">The template to render while the component is in a laoding state.</span></span> |
| <span data-ttu-id="ada63-188">无数据</span><span class="sxs-lookup"><span data-stu-id="ada63-188">no-data</span></span> | <span data-ttu-id="ada63-189">无</span><span class="sxs-lookup"><span data-stu-id="ada63-189">none</span></span> | <span data-ttu-id="ada63-190">在没有人员图像或数据可用时要呈现的模板。</span><span class="sxs-lookup"><span data-stu-id="ada63-190">The template to render when no person image or data is available.</span></span> | 
| <span data-ttu-id="ada63-191"> 默认值</span><span class="sxs-lookup"><span data-stu-id="ada63-191">default</span></span> | <span data-ttu-id="ada63-192">人员：人员详细信息对象</span><span class="sxs-lookup"><span data-stu-id="ada63-192">person: The person details object</span></span> <br> <span data-ttu-id="ada63-193">`personImage`：图像的 URL</span><span class="sxs-lookup"><span data-stu-id="ada63-193">`personImage`: The URL of the image</span></span> | <span data-ttu-id="ada63-194">默认模板会将整个组件替换为您自己的组件。</span><span class="sxs-lookup"><span data-stu-id="ada63-194">The default template replaces the entire component with your own.</span></span> |
| <span data-ttu-id="ada63-195">人员-卡片</span><span class="sxs-lookup"><span data-stu-id="ada63-195">person-card</span></span> | <span data-ttu-id="ada63-196">人员：人员详细信息对象</span><span class="sxs-lookup"><span data-stu-id="ada63-196">person: The person details object</span></span> <br> <span data-ttu-id="ada63-197">`personImage`：图像的 URL</span><span class="sxs-lookup"><span data-stu-id="ada63-197">`personImage`: The URL of the image</span></span> | <span data-ttu-id="ada63-198">用于更新在悬停或单击时显示的 "管理员-卡片" 的模板。</span><span class="sxs-lookup"><span data-stu-id="ada63-198">The template to update the mgt-person-card displayed on hover or click.</span></span> |

<span data-ttu-id="ada63-199">下面的示例定义了 "人员" 组件的模板。</span><span class="sxs-lookup"><span data-stu-id="ada63-199">The following example defines a template for the person component.</span></span>

```html
<mgt-person>
  <template>
    <div data-if="personImage">
      <img src="{{personImage}}" />
    </div>
    <div data-else>
      {{person.displayName}}
    </div>
  </template>
</mgt-person>
```

## <a name="person-card"></a><span data-ttu-id="ada63-200">个人卡片</span><span class="sxs-lookup"><span data-stu-id="ada63-200">Person Card</span></span>

<span data-ttu-id="ada63-201">`mgt-person`组件可显示为 `mgt-person-card` 悬停或单击。</span><span class="sxs-lookup"><span data-stu-id="ada63-201">The `mgt-person` component can show an `mgt-person-card` on either hover or click.</span></span>

### <a name="add-the-control-to-the-html-page"></a><span data-ttu-id="ada63-202">将控件添加到 HTML 页面</span><span class="sxs-lookup"><span data-stu-id="ada63-202">Add the control to the HTML page</span></span>
```html
<mgt-person person-query="me" person-card="hover"></mgt-person>
```

| <span data-ttu-id="ada63-203">属性</span><span class="sxs-lookup"><span data-stu-id="ada63-203">Attribute</span></span>    |  <span data-ttu-id="ada63-204">属性</span><span class="sxs-lookup"><span data-stu-id="ada63-204">Property</span></span>     | <span data-ttu-id="ada63-205">说明</span><span class="sxs-lookup"><span data-stu-id="ada63-205">Description</span></span>                                                                     |
| ------------ | ------------- | ------------------------------------------------------------------------------- |
| <span data-ttu-id="ada63-206">人员-卡片</span><span class="sxs-lookup"><span data-stu-id="ada63-206">person-card</span></span> | <span data-ttu-id="ada63-207">personCardInteraction</span><span class="sxs-lookup"><span data-stu-id="ada63-207">personCardInteraction</span></span> | <span data-ttu-id="ada63-208">一个枚举，用于确定激活浮出式面板-或的必需用户操作 `hover` `click` 。</span><span class="sxs-lookup"><span data-stu-id="ada63-208">An enumeration to determine user action necessary to activate flyout panel - `hover` or `click`.</span></span> <span data-ttu-id="ada63-209">默认值为`none`</span><span class="sxs-lookup"><span data-stu-id="ada63-209">Default value is `none`</span></span> |


<span data-ttu-id="ada63-210">有关模板化、样式和属性的详细信息，请参阅[人员卡片组件](./person-card.md)。</span><span class="sxs-lookup"><span data-stu-id="ada63-210">For more information about templating, styling, and attributes, see [Person Card component](./person-card.md).</span></span>

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="ada63-211">Microsoft Graph 权限</span><span class="sxs-lookup"><span data-stu-id="ada63-211">Microsoft Graph permissions</span></span>

<span data-ttu-id="ada63-212">此控件使用以下 Microsoft Graph Api 和权限。</span><span class="sxs-lookup"><span data-stu-id="ada63-212">This control uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="ada63-213">资源</span><span class="sxs-lookup"><span data-stu-id="ada63-213">Resource</span></span>                                                                                                    | <span data-ttu-id="ada63-214">Permission</span><span class="sxs-lookup"><span data-stu-id="ada63-214">Permission</span></span>     |
| ----------------------------------------------------------------------------------------------------------- | -------------------- |
| [<span data-ttu-id="ada63-215">/me</span><span class="sxs-lookup"><span data-stu-id="ada63-215">/me</span></span>](/graph/api/user-get?view=graph-rest-1.0)                              | <span data-ttu-id="ada63-216">User.Read</span><span class="sxs-lookup"><span data-stu-id="ada63-216">User.Read</span></span>          |
| [<span data-ttu-id="ada63-217">/me/photo/$value</span><span class="sxs-lookup"><span data-stu-id="ada63-217">/me/photo/$value</span></span>](/graph/api/profilephoto-get?view=graph-rest-beta)        | <span data-ttu-id="ada63-218">User.Read</span><span class="sxs-lookup"><span data-stu-id="ada63-218">User.Read</span></span>          |
| [<span data-ttu-id="ada63-219">/me/people/？ $search =</span><span class="sxs-lookup"><span data-stu-id="ada63-219">/me/people/?$search=</span></span>](/graph/api/user-list-people?view=graph-rest-1.0)     | <span data-ttu-id="ada63-220">People.Read</span><span class="sxs-lookup"><span data-stu-id="ada63-220">People.Read</span></span>        |
| [<span data-ttu-id="ada63-221">/me/contacts/\*</span><span class="sxs-lookup"><span data-stu-id="ada63-221">/me/contacts/\*</span></span>](/graph/api/user-list-contacts?view=graph-rest-1.0&tabs=cs) | <span data-ttu-id="ada63-222">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="ada63-222">Contacts.Read</span></span>      |
| [<span data-ttu-id="ada63-223">/users/{id}/photo/$value</span><span class="sxs-lookup"><span data-stu-id="ada63-223">/users/{id}/photo/$value</span></span>](/graph/api/user-list-people?view=graph-rest-1.0) | <span data-ttu-id="ada63-224">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="ada63-224">User.ReadBasic.All</span></span> |
| [<span data-ttu-id="ada63-225">/me/presence</span><span class="sxs-lookup"><span data-stu-id="ada63-225">/me/presence</span></span>](/graph/api/presence-get?view=graph-rest-beta)                | <span data-ttu-id="ada63-226">Presence.Read</span><span class="sxs-lookup"><span data-stu-id="ada63-226">Presence.Read</span></span> |
| [<span data-ttu-id="ada63-227">/users/{id}/presence</span><span class="sxs-lookup"><span data-stu-id="ada63-227">/users/{id}/presence</span></span>](/graph/api/presence-get?view=graph-rest-beta)        | <span data-ttu-id="ada63-228">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="ada63-228">Presence.Read.All</span></span> |

> <span data-ttu-id="ada63-229">**注意：** 若要访问 `*/photo/$value` 个人 Microsoft 帐户的资源，请使用 Microsoft Graph beta 终结点。</span><span class="sxs-lookup"><span data-stu-id="ada63-229">**Note:** to access the `*/photo/$value` resources for personal Microsoft accounts, use the Microsoft Graph beta endpoint.</span></span>

## <a name="authentication"></a><span data-ttu-id="ada63-230">身份验证</span><span class="sxs-lookup"><span data-stu-id="ada63-230">Authentication</span></span>

<span data-ttu-id="ada63-231">该控件使用[身份验证文档](./../providers.md)中介绍的全局身份验证提供程序提取所需的数据。</span><span class="sxs-lookup"><span data-stu-id="ada63-231">The control uses the global authentication provider described in the [authentication documentation](./../providers.md) to fetch the required data.</span></span>

## <a name="extend-for-more-control"></a><span data-ttu-id="ada63-232">扩展以实现更多控制</span><span class="sxs-lookup"><span data-stu-id="ada63-232">Extend for more control</span></span>

<span data-ttu-id="ada63-233">对于更复杂的方案或真正的自定义 UX，此组件将公开几种 `protected render*` 用于在组件扩展中进行重写的方法。</span><span class="sxs-lookup"><span data-stu-id="ada63-233">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions.</span></span>

| <span data-ttu-id="ada63-234">方法</span><span class="sxs-lookup"><span data-stu-id="ada63-234">Method</span></span> | <span data-ttu-id="ada63-235">说明</span><span class="sxs-lookup"><span data-stu-id="ada63-235">Description</span></span> |
| - | - |
| <span data-ttu-id="ada63-236">renderLoading</span><span class="sxs-lookup"><span data-stu-id="ada63-236">renderLoading</span></span> | <span data-ttu-id="ada63-237">呈现加载状态。</span><span class="sxs-lookup"><span data-stu-id="ada63-237">Renders the loading state.</span></span> |
| <span data-ttu-id="ada63-238">renderNoData</span><span class="sxs-lookup"><span data-stu-id="ada63-238">renderNoData</span></span> | <span data-ttu-id="ada63-239">在没有图像或人员数据可用时呈现。</span><span class="sxs-lookup"><span data-stu-id="ada63-239">Renders when no image or person data is available.</span></span> |
| <span data-ttu-id="ada63-240">renderAvatar</span><span class="sxs-lookup"><span data-stu-id="ada63-240">renderAvatar</span></span> | <span data-ttu-id="ada63-241">呈现头像。</span><span class="sxs-lookup"><span data-stu-id="ada63-241">Renders the avatar.</span></span> |
| <span data-ttu-id="ada63-242">renderDetails</span><span class="sxs-lookup"><span data-stu-id="ada63-242">renderDetails</span></span> | <span data-ttu-id="ada63-243">呈现人员详细信息部分。</span><span class="sxs-lookup"><span data-stu-id="ada63-243">Renders the person details part.</span></span> |
