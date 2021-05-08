---
title: Microsoft Graph 功能中的人员Toolkit
description: 人员组件用于通过使用联系人的照片、姓名和/或电子邮件地址来显示此人或联系人。
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 5250919404ecccea1f01042d93aaf2b9fa4fc3b3
ms.sourcegitcommit: de3bc91a24d23b46bd0863487415fba8d8fce63c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/07/2021
ms.locfileid: "52266841"
---
# <a name="person-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="ec764-103">Microsoft Graph 功能中的人员Toolkit</span><span class="sxs-lookup"><span data-stu-id="ec764-103">Person component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="ec764-104">人员组件用于通过使用其照片、姓名、电子邮件地址或其他任何人员详细信息来显示此人或联系人。</span><span class="sxs-lookup"><span data-stu-id="ec764-104">The person component is used to display a person or contact by using their photo, name, email address, or any other person details.</span></span>

<span data-ttu-id="ec764-105">人员组件还使用 [mgt-person-card](./person-card.md) 显示包含有关用户的其他信息的飞出卡。</span><span class="sxs-lookup"><span data-stu-id="ec764-105">The person component also uses the [mgt-person-card](./person-card.md) to display a flyout card with additional information about the user.</span></span> <span data-ttu-id="ec764-106">有关详细信息，请参阅人员 [卡片](#person-card) 部分。</span><span class="sxs-lookup"><span data-stu-id="ec764-106">For details, see the [Person Card](#person-card) section.</span></span>

## <a name="example"></a><span data-ttu-id="ec764-107">示例</span><span class="sxs-lookup"><span data-stu-id="ec764-107">Example</span></span>

<span data-ttu-id="ec764-108">以下示例显示使用该组件 `mgt-person` 的人。</span><span class="sxs-lookup"><span data-stu-id="ec764-108">The following example displays a person using the `mgt-person` component.</span></span> <span data-ttu-id="ec764-109">可以使用代码编辑器查看 [属性如何](#properties) 更改组件的行为。</span><span class="sxs-lookup"><span data-stu-id="ec764-109">You can use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-person--person&source=docs" height="250"></iframe>

[<span data-ttu-id="ec764-110">在"打开"mgt.dev</span><span class="sxs-lookup"><span data-stu-id="ec764-110">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-person--person&source=docs)

## <a name="setting-the-person-details"></a><span data-ttu-id="ec764-111">设置人员详细信息</span><span class="sxs-lookup"><span data-stu-id="ec764-111">Setting the person details</span></span>

<span data-ttu-id="ec764-112">可以使用三个属性来设置人员详细信息。</span><span class="sxs-lookup"><span data-stu-id="ec764-112">You can use three properties to set the person details.</span></span> <span data-ttu-id="ec764-113">每个实例仅使用以下属性之一：</span><span class="sxs-lookup"><span data-stu-id="ec764-113">Use only one of the following properties per instance:</span></span>

* <span data-ttu-id="ec764-114">设置 `user-id` 属性或 `userId` 属性，以使用用户的 ID 从 Microsoft Graph 提取用户。</span><span class="sxs-lookup"><span data-stu-id="ec764-114">Set the `user-id` attribute or `userId` property to fetch the user from Microsoft Graph by using their ID.</span></span>

* <span data-ttu-id="ec764-115">设置 `person-query` 属性或 `personQuery` 属性以在 Microsoft Graph 中搜索给定人员。</span><span class="sxs-lookup"><span data-stu-id="ec764-115">Set the `person-query` attribute or `personQuery` property to search Microsoft Graph for a given person.</span></span> <span data-ttu-id="ec764-116">它将选择第一个可用的人员并提取该人员的详细信息。</span><span class="sxs-lookup"><span data-stu-id="ec764-116">It will choose the first person available and fetch the person details.</span></span> <span data-ttu-id="ec764-117">电子邮件最适用于确保查询正确的人员，但名称也有效。</span><span class="sxs-lookup"><span data-stu-id="ec764-117">An email works best to ensure the right person is queried, but a name works as well.</span></span>

* <span data-ttu-id="ec764-118">设置 `person-presence` 属性或 `personPresence` 属性以手动向个人头像添加状态锁屏提醒。</span><span class="sxs-lookup"><span data-stu-id="ec764-118">Set the `person-presence` attribute or `personPresence` property to add a presence badge to person avatar manually.</span></span>

* <span data-ttu-id="ec764-119">将 `avatar-size` 属性或 `avatarSize` 属性设置为 `small` 或 `large` 确定头像的大小。</span><span class="sxs-lookup"><span data-stu-id="ec764-119">Set the `avatar-size` attribute or `avatarSize` property to `small` or `large` to determine the size of avatar.</span></span> <span data-ttu-id="ec764-120">这有助于向头像 [添加正确的状态](https://mgt.dev/?path=/story/components-mgt-person--person-presence-display-all) 锁屏提醒。</span><span class="sxs-lookup"><span data-stu-id="ec764-120">This helps add the [correct presence badge](https://mgt.dev/?path=/story/components-mgt-person--person-presence-display-all) to avatar.</span></span> <span data-ttu-id="ec764-121">你将需要选择正确的相应的 css 自定义属性，如下所示以进一步自定义头像大小。</span><span class="sxs-lookup"><span data-stu-id="ec764-121">You will need to choose the correct corresponding css custom properties shown below to further customize avatar size.</span></span> <span data-ttu-id="ec764-122">默认情况下，值设置为 ，该值将自动根据 属性 `auto` 决定如何呈现 `view` 状态。</span><span class="sxs-lookup"><span data-stu-id="ec764-122">By default, the value is set to `auto` which will automatically decide how to render the presence based on the `view` property.</span></span> <span data-ttu-id="ec764-123">如果你的头 `small` 像小于 32px x 32px，我们建议使用 。</span><span class="sxs-lookup"><span data-stu-id="ec764-123">We recommend using `small` if your avatar is smaller than 32px by 32px.</span></span> 

* <span data-ttu-id="ec764-124">使用 `person-details` 属性 `personDetails` 或 属性手动设置人员详细信息，如以下示例所示。</span><span class="sxs-lookup"><span data-stu-id="ec764-124">Use the `person-details` attribute or `personDetails` property to manually set the person details, as shown in the following example.</span></span>


    ```js
    let personControl = document.getElementById('myPersonControl');
    personControl.personDetails = {
        displayName: 'Nikola Metulev',
        mail: 'nikola@contoso.com',
        personImage: 'url'
    }
    ```

  <span data-ttu-id="ec764-125">如果未提供图像，将提取一个 (（如果) ）。</span><span class="sxs-lookup"><span data-stu-id="ec764-125">If no image is provided, one will be fetched (if available).</span></span>

## <a name="properties"></a><span data-ttu-id="ec764-126">属性</span><span class="sxs-lookup"><span data-stu-id="ec764-126">Properties</span></span>

<span data-ttu-id="ec764-127">可以使用多个属性来自定义组件。</span><span class="sxs-lookup"><span data-stu-id="ec764-127">You can use several properties to customize the component.</span></span>

| <span data-ttu-id="ec764-128">属性</span><span class="sxs-lookup"><span data-stu-id="ec764-128">Attribute</span></span>       | <span data-ttu-id="ec764-129">属性</span><span class="sxs-lookup"><span data-stu-id="ec764-129">Property</span></span>       | <span data-ttu-id="ec764-130">说明</span><span class="sxs-lookup"><span data-stu-id="ec764-130">Description</span></span>                                                   |
| -----------     | ----------     | ------------------------------------------------------------- |
| <span data-ttu-id="ec764-131">user-id</span><span class="sxs-lookup"><span data-stu-id="ec764-131">user-id</span></span>         | <span data-ttu-id="ec764-132">userId</span><span class="sxs-lookup"><span data-stu-id="ec764-132">userId</span></span>         | <span data-ttu-id="ec764-133">设置为用户 ID 以从 Microsoft Graph 提取该用户的详细信息和图像。</span><span class="sxs-lookup"><span data-stu-id="ec764-133">Set to a user id to fetch that user's details and image from Microsoft Graph.</span></span>|
| <span data-ttu-id="ec764-134">person-query</span><span class="sxs-lookup"><span data-stu-id="ec764-134">person-query</span></span>    | <span data-ttu-id="ec764-135">personQuery</span><span class="sxs-lookup"><span data-stu-id="ec764-135">personQuery</span></span>    | <span data-ttu-id="ec764-136">设置为某人的姓名或电子邮件，以在 Microsoft Graph 中搜索某人并提取第一个人的详细信息和图像。</span><span class="sxs-lookup"><span data-stu-id="ec764-136">Set to a name or email of a person to search for a person in Microsoft Graph and fetch the first person's details and image.</span></span>|
| <span data-ttu-id="ec764-137">person-details</span><span class="sxs-lookup"><span data-stu-id="ec764-137">person-details</span></span>  | <span data-ttu-id="ec764-138">personDetails</span><span class="sxs-lookup"><span data-stu-id="ec764-138">personDetails</span></span>  | <span data-ttu-id="ec764-139">设置为表示人员的对象。</span><span class="sxs-lookup"><span data-stu-id="ec764-139">Set to an object representing a person.</span></span> <span data-ttu-id="ec764-140">使用来自人员、用户、联系人或组、资源的对象。</span><span class="sxs-lookup"><span data-stu-id="ec764-140">Works with object from the people, users, contacts, or group, resources.</span></span> |
| <span data-ttu-id="ec764-141">fallback-details</span><span class="sxs-lookup"><span data-stu-id="ec764-141">fallback-details</span></span>| <span data-ttu-id="ec764-142">fallbackDetails</span><span class="sxs-lookup"><span data-stu-id="ec764-142">fallbackDetails</span></span>| <span data-ttu-id="ec764-143">设置为一个对象，该对象表示在图形中找不到用户/人员/联系人时的用户。</span><span class="sxs-lookup"><span data-stu-id="ec764-143">Set to an object representing a person when no user/person/contact is found in the graph.</span></span>
| <span data-ttu-id="ec764-144">person-image</span><span class="sxs-lookup"><span data-stu-id="ec764-144">person-image</span></span>    | <span data-ttu-id="ec764-145">personImage</span><span class="sxs-lookup"><span data-stu-id="ec764-145">personImage</span></span>    | <span data-ttu-id="ec764-146">设置要向人员显示的图像。</span><span class="sxs-lookup"><span data-stu-id="ec764-146">Set the image to show for the person.</span></span> |
| <span data-ttu-id="ec764-147">person-presence</span><span class="sxs-lookup"><span data-stu-id="ec764-147">person-presence</span></span> | <span data-ttu-id="ec764-148">personPresence</span><span class="sxs-lookup"><span data-stu-id="ec764-148">personPresence</span></span> | <span data-ttu-id="ec764-149">为人员设置状态。</span><span class="sxs-lookup"><span data-stu-id="ec764-149">Set the presence for the person.</span></span> |
| <span data-ttu-id="ec764-150">fetch-image</span><span class="sxs-lookup"><span data-stu-id="ec764-150">fetch-image</span></span>     | <span data-ttu-id="ec764-151">fetchImage</span><span class="sxs-lookup"><span data-stu-id="ec764-151">fetchImage</span></span>     | <span data-ttu-id="ec764-152">将标志设置为 `personImage` 根据用户提供的对象自动从 Microsoft Graph `personDetails` 提取。</span><span class="sxs-lookup"><span data-stu-id="ec764-152">Set flag to fetch `personImage` automatically from Microsoft Graph based on the `personDetails` object provided by the user.</span></span> |
| <span data-ttu-id="ec764-153">头像类型</span><span class="sxs-lookup"><span data-stu-id="ec764-153">avatar-type</span></span>     | <span data-ttu-id="ec764-154">头像类型</span><span class="sxs-lookup"><span data-stu-id="ec764-154">avatarType</span></span>     | <span data-ttu-id="ec764-155">设置为 或 `initials` `photo` 呈现任一显示状态 - 默认为照片。</span><span class="sxs-lookup"><span data-stu-id="ec764-155">Set to `initials` or `photo` to render either display state - default is photo.</span></span> |
| <span data-ttu-id="ec764-156">view</span><span class="sxs-lookup"><span data-stu-id="ec764-156">view</span></span>            | <span data-ttu-id="ec764-157">view</span><span class="sxs-lookup"><span data-stu-id="ec764-157">view</span></span>           | <span data-ttu-id="ec764-158">设置为控制呈现人员的方式。</span><span class="sxs-lookup"><span data-stu-id="ec764-158">Set to control how the person is rendered.</span></span> <span data-ttu-id="ec764-159">默认值为 `avatar`</span><span class="sxs-lookup"><span data-stu-id="ec764-159">Default is `avatar`</span></span> <br /> <span data-ttu-id="ec764-160">`avatar` - 仅显示头像</span><span class="sxs-lookup"><span data-stu-id="ec764-160">`avatar` - show only avatar</span></span> <br /> <span data-ttu-id="ec764-161">`oneline` - 默认显示头像 (`displayName` 第一) </span><span class="sxs-lookup"><span data-stu-id="ec764-161">`oneline` - show avatar and first line (`displayName` by default)</span></span> <br /> <span data-ttu-id="ec764-162">`twolines` - 显示头像和两行文本 (`displayName` `mail` 默认显示) </span><span class="sxs-lookup"><span data-stu-id="ec764-162">`twolines` - show avatar and two lines of text (`displayName` and `mail` by default)</span></span>|
| <span data-ttu-id="ec764-163">line1-property</span><span class="sxs-lookup"><span data-stu-id="ec764-163">line1-property</span></span>  | <span data-ttu-id="ec764-164">line1Property</span><span class="sxs-lookup"><span data-stu-id="ec764-164">line1Property</span></span>  | <span data-ttu-id="ec764-165">设置要用于第一行文本的 personDetails 的属性。</span><span class="sxs-lookup"><span data-stu-id="ec764-165">Sets the property of the personDetails to use for the first line of text.</span></span> <span data-ttu-id="ec764-166">默认值为“`displayName`”。</span><span class="sxs-lookup"><span data-stu-id="ec764-166">Default is `displayName`.</span></span>|
| <span data-ttu-id="ec764-167">line2-property</span><span class="sxs-lookup"><span data-stu-id="ec764-167">line2-property</span></span>  | <span data-ttu-id="ec764-168">line2Property</span><span class="sxs-lookup"><span data-stu-id="ec764-168">line2Property</span></span>  | <span data-ttu-id="ec764-169">设置要用于第二行文本的 personDetails 的属性。</span><span class="sxs-lookup"><span data-stu-id="ec764-169">Sets the property of the personDetails to use for the second line of text.</span></span> <span data-ttu-id="ec764-170">默认值为“`mail`”。</span><span class="sxs-lookup"><span data-stu-id="ec764-170">Default is `mail`.</span></span>|
| <span data-ttu-id="ec764-171">line3-property</span><span class="sxs-lookup"><span data-stu-id="ec764-171">line3-property</span></span>  | <span data-ttu-id="ec764-172">line3Property</span><span class="sxs-lookup"><span data-stu-id="ec764-172">line3Property</span></span>  | <span data-ttu-id="ec764-173">设置要用于第三行文本的 personDetails 的属性。</span><span class="sxs-lookup"><span data-stu-id="ec764-173">Sets the property of the personDetails to use for the third line of text.</span></span> <span data-ttu-id="ec764-174">默认值为“`jobTitle`”。</span><span class="sxs-lookup"><span data-stu-id="ec764-174">Default is `jobTitle`.</span></span>|
| <span data-ttu-id="ec764-175">show-presence</span><span class="sxs-lookup"><span data-stu-id="ec764-175">show-presence</span></span>   | <span data-ttu-id="ec764-176">showPresence</span><span class="sxs-lookup"><span data-stu-id="ec764-176">showPresence</span></span>   | <span data-ttu-id="ec764-177">设置用于显示人员状态的标志 - 默认为 `false` 。</span><span class="sxs-lookup"><span data-stu-id="ec764-177">Set flag to display person presence - default is `false`.</span></span>|

## <a name="css-custom-properties"></a><span data-ttu-id="ec764-178">CSS 自定义属性</span><span class="sxs-lookup"><span data-stu-id="ec764-178">CSS custom properties</span></span>

<span data-ttu-id="ec764-179">组件 `mgt-person` 定义以下 CSS 自定义属性。</span><span class="sxs-lookup"><span data-stu-id="ec764-179">The `mgt-person` component defines the following CSS custom properties.</span></span>

```css
mgt-person {
  --avatar-size: 48px;
  --avatar-border: 0;
  --avatar-border-radius: 50%;
  
  --initials-color: white;
  --initials-background-color: magenta;

  --presence-background-color: #ffffff;
  --presence-icon-color: #ffffff;

  --font-family: 'Segoe UI';
  --font-size: 14px;
  --font-weight: 500;
  --color: black;
  --text-transform: none;

  --line2-font-size: 12px;
  --line2-font-weight: 400;
  --line2-color: black;
  --line2-text-transform: none;

  --line3-font-size: 12px;
  --line3-font-weight: 400;
  --line3-color: black;
  --line3-text-transform: none;

  --details-spacing: 12px;
}
```

<span data-ttu-id="ec764-180">若要了解更多信息，请参阅 [设置组件样式](../customize-components/style.md)。</span><span class="sxs-lookup"><span data-stu-id="ec764-180">To learn more, see [styling components](../customize-components/style.md).</span></span>

## <a name="events"></a><span data-ttu-id="ec764-181">事件</span><span class="sxs-lookup"><span data-stu-id="ec764-181">Events</span></span>

<span data-ttu-id="ec764-182">从组件中触发以下事件。</span><span class="sxs-lookup"><span data-stu-id="ec764-182">The following events are fired from the component.</span></span>

| <span data-ttu-id="ec764-183">事件</span><span class="sxs-lookup"><span data-stu-id="ec764-183">Event</span></span> | <span data-ttu-id="ec764-184">详情</span><span class="sxs-lookup"><span data-stu-id="ec764-184">Detail</span></span> | <span data-ttu-id="ec764-185">说明</span><span class="sxs-lookup"><span data-stu-id="ec764-185">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="ec764-186">line1clicked</span><span class="sxs-lookup"><span data-stu-id="ec764-186">line1clicked</span></span> | <span data-ttu-id="ec764-187">详细信息包含各自的 `person` 对象</span><span class="sxs-lookup"><span data-stu-id="ec764-187">The detail contains the respective `person` object</span></span> | <span data-ttu-id="ec764-188">在单击第 1 行时触发。</span><span class="sxs-lookup"><span data-stu-id="ec764-188">Fired when line1 is clicked.</span></span> |
| <span data-ttu-id="ec764-189">line2clicked</span><span class="sxs-lookup"><span data-stu-id="ec764-189">line2clicked</span></span> | <span data-ttu-id="ec764-190">详细信息包含各自的 `person` 对象</span><span class="sxs-lookup"><span data-stu-id="ec764-190">The detail contains the respective `person` object</span></span> | <span data-ttu-id="ec764-191">在单击第 2 行时触发。</span><span class="sxs-lookup"><span data-stu-id="ec764-191">Fired when line2 is clicked.</span></span> |
| <span data-ttu-id="ec764-192">line3clicked</span><span class="sxs-lookup"><span data-stu-id="ec764-192">line3clicked</span></span> | <span data-ttu-id="ec764-193">详细信息包含各自的 `person` 对象</span><span class="sxs-lookup"><span data-stu-id="ec764-193">The detail contains the respective `person` object</span></span> | <span data-ttu-id="ec764-194">在单击第 3 行时触发。</span><span class="sxs-lookup"><span data-stu-id="ec764-194">Fired when line3 is clicked.</span></span> |

## <a name="templates"></a><span data-ttu-id="ec764-195">模板</span><span class="sxs-lookup"><span data-stu-id="ec764-195">Templates</span></span>

<span data-ttu-id="ec764-196">组件 `mgt-person` 支持 [多个模板](../customize-components/templates.md) ，允许您替换组件的某些部分。</span><span class="sxs-lookup"><span data-stu-id="ec764-196">The `mgt-person` component supports several [templates](../customize-components/templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="ec764-197">若要指定模板，请包含组件 `<template>` 中的元素，将值 `data-type` 设置为下列值之一：</span><span class="sxs-lookup"><span data-stu-id="ec764-197">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following:</span></span>

| <span data-ttu-id="ec764-198">数据类型</span><span class="sxs-lookup"><span data-stu-id="ec764-198">Data type</span></span> | <span data-ttu-id="ec764-199">数据上下文</span><span class="sxs-lookup"><span data-stu-id="ec764-199">Data context</span></span> | <span data-ttu-id="ec764-200">说明</span><span class="sxs-lookup"><span data-stu-id="ec764-200">Description</span></span> |
| --------- | ------------ | ----------- |
| <span data-ttu-id="ec764-201">loading</span><span class="sxs-lookup"><span data-stu-id="ec764-201">loading</span></span> | <span data-ttu-id="ec764-202">无</span><span class="sxs-lookup"><span data-stu-id="ec764-202">none</span></span> | <span data-ttu-id="ec764-203">组件在加载状态时要呈现的模板。</span><span class="sxs-lookup"><span data-stu-id="ec764-203">The template to render while the component is in a loading state.</span></span> |
| <span data-ttu-id="ec764-204">no-data</span><span class="sxs-lookup"><span data-stu-id="ec764-204">no-data</span></span> | <span data-ttu-id="ec764-205">无</span><span class="sxs-lookup"><span data-stu-id="ec764-205">none</span></span> | <span data-ttu-id="ec764-206">在没有任何人员图像或数据可用时要呈现的模板。</span><span class="sxs-lookup"><span data-stu-id="ec764-206">The template to render when no person image or data is available.</span></span> | 
| <span data-ttu-id="ec764-207">default</span><span class="sxs-lookup"><span data-stu-id="ec764-207">default</span></span> | <span data-ttu-id="ec764-208">person： The person details object</span><span class="sxs-lookup"><span data-stu-id="ec764-208">person: The person details object</span></span> <br> <span data-ttu-id="ec764-209">`personImage`：图像的 URL</span><span class="sxs-lookup"><span data-stu-id="ec764-209">`personImage`: The URL of the image</span></span> | <span data-ttu-id="ec764-210">默认模板将整个组件替换为你自己的组件。</span><span class="sxs-lookup"><span data-stu-id="ec764-210">The default template replaces the entire component with your own.</span></span> |
| <span data-ttu-id="ec764-211">person-card</span><span class="sxs-lookup"><span data-stu-id="ec764-211">person-card</span></span> | <span data-ttu-id="ec764-212">person： The person details object</span><span class="sxs-lookup"><span data-stu-id="ec764-212">person: The person details object</span></span> <br> <span data-ttu-id="ec764-213">`personImage`：图像的 URL</span><span class="sxs-lookup"><span data-stu-id="ec764-213">`personImage`: The URL of the image</span></span> | <span data-ttu-id="ec764-214">用于更新悬停或单击时显示的 mgt-person-card 的模板。</span><span class="sxs-lookup"><span data-stu-id="ec764-214">The template to update the mgt-person-card displayed on hover or click.</span></span> |
| <span data-ttu-id="ec764-215">line1</span><span class="sxs-lookup"><span data-stu-id="ec764-215">line1</span></span> | <span data-ttu-id="ec764-216">person： The person details object</span><span class="sxs-lookup"><span data-stu-id="ec764-216">person: The person details object</span></span> | <span data-ttu-id="ec764-217">第一行人员元数据的模板。</span><span class="sxs-lookup"><span data-stu-id="ec764-217">The template for the first line of person metadata.</span></span> |
| <span data-ttu-id="ec764-218">line2</span><span class="sxs-lookup"><span data-stu-id="ec764-218">line2</span></span> | <span data-ttu-id="ec764-219">person： The person details object</span><span class="sxs-lookup"><span data-stu-id="ec764-219">person: The person details object</span></span> | <span data-ttu-id="ec764-220">第二行人员元数据的模板。</span><span class="sxs-lookup"><span data-stu-id="ec764-220">The template for the second line of person metadata.</span></span> |
| <span data-ttu-id="ec764-221">line3</span><span class="sxs-lookup"><span data-stu-id="ec764-221">line3</span></span> | <span data-ttu-id="ec764-222">person： The person details object</span><span class="sxs-lookup"><span data-stu-id="ec764-222">person: The person details object</span></span> | <span data-ttu-id="ec764-223">第三行人员元数据的模板。</span><span class="sxs-lookup"><span data-stu-id="ec764-223">The template for the third line of person metadata.</span></span> |

<span data-ttu-id="ec764-224">下面的示例定义人员组件的模板。</span><span class="sxs-lookup"><span data-stu-id="ec764-224">The following example defines a template for the person component.</span></span>

```html
<!-- Retemplate the entire person component -->
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

<!-- Retemplate the line properties -->
<mgt-person view="threeLines">
  <template data-type="line1">
    <div>
      Hello, my name is: {{person.displayName}}
    </div>
  </template>
  <template data-type="line2">
    <div>
      Super cool
    </div>
  </template>
  <template data-type="line3">
    <div>
      Loves MGT
    </div>
  </template>
</mgt-person>
```

## <a name="person-card"></a><span data-ttu-id="ec764-225">个人卡片</span><span class="sxs-lookup"><span data-stu-id="ec764-225">Person card</span></span>

<span data-ttu-id="ec764-226">组件 `mgt-person` 可以在悬停 `mgt-person-card` 或单击时显示 。</span><span class="sxs-lookup"><span data-stu-id="ec764-226">The `mgt-person` component can show an `mgt-person-card` on either hover or click.</span></span>

### <a name="add-the-control-to-the-html-page"></a><span data-ttu-id="ec764-227">将控件添加到 HTML 页面</span><span class="sxs-lookup"><span data-stu-id="ec764-227">Add the control to the HTML page</span></span>
```html
<mgt-person person-query="me" person-card="hover"></mgt-person>
```

| <span data-ttu-id="ec764-228">属性</span><span class="sxs-lookup"><span data-stu-id="ec764-228">Attribute</span></span>    |  <span data-ttu-id="ec764-229">属性</span><span class="sxs-lookup"><span data-stu-id="ec764-229">Property</span></span>     | <span data-ttu-id="ec764-230">说明</span><span class="sxs-lookup"><span data-stu-id="ec764-230">Description</span></span>                                                                     |
| ------------ | ------------- | ------------------------------------------------------------------------------- |
| <span data-ttu-id="ec764-231">person-card</span><span class="sxs-lookup"><span data-stu-id="ec764-231">person-card</span></span> | <span data-ttu-id="ec764-232">personCardInteraction</span><span class="sxs-lookup"><span data-stu-id="ec764-232">personCardInteraction</span></span> | <span data-ttu-id="ec764-233">一个枚举，用于确定激活飞出面板或 所需的用户 `hover` 操作 `click` 。</span><span class="sxs-lookup"><span data-stu-id="ec764-233">An enumeration to determine user action necessary to activate flyout panel - `hover` or `click`.</span></span> <span data-ttu-id="ec764-234">默认值为 `none`</span><span class="sxs-lookup"><span data-stu-id="ec764-234">Default value is `none`</span></span> |


<span data-ttu-id="ec764-235">有关模板、样式设置和属性详细信息，请参阅 Person Card [component](./person-card.md)。</span><span class="sxs-lookup"><span data-stu-id="ec764-235">For more information about templating, styling, and attributes, see [Person Card component](./person-card.md).</span></span>

## <a name="global-component-configuration"></a><span data-ttu-id="ec764-236">全局组件配置</span><span class="sxs-lookup"><span data-stu-id="ec764-236">Global component configuration</span></span>

<span data-ttu-id="ec764-237">类 `MgtPerson` 公开一个 `config` 静态对象，该对象配置应用程序中的每个人组件。</span><span class="sxs-lookup"><span data-stu-id="ec764-237">The `MgtPerson` class exposes a static `config` object that configures all person components in the application.</span></span>

<span data-ttu-id="ec764-238">以下示例演示如何使用 config 对象。</span><span class="sxs-lookup"><span data-stu-id="ec764-238">The following example shows how to use the config object.</span></span>

```ts
import { MgtPerson } from `@microsoft/mgt`;

MgtPerson.config.useContactApis = false;
```

<span data-ttu-id="ec764-239">以下属性在 config 对象上可用。</span><span class="sxs-lookup"><span data-stu-id="ec764-239">The following properties are available on the config object.</span></span>

| <span data-ttu-id="ec764-240">属性</span><span class="sxs-lookup"><span data-stu-id="ec764-240">Property</span></span> | <span data-ttu-id="ec764-241">说明</span><span class="sxs-lookup"><span data-stu-id="ec764-241">Description</span></span> |
| ------------ | ------------- |
| <span data-ttu-id="ec764-242">useContactApis</span><span class="sxs-lookup"><span data-stu-id="ec764-242">useContactApis</span></span> | <span data-ttu-id="ec764-243">`boolean` - 指示人员组件是否可以使用 Microsoft Graph 个人联系人 API 搜索联系人详细信息和照片。</span><span class="sxs-lookup"><span data-stu-id="ec764-243">`boolean` - Indicates whether the person component can use the Microsoft Graph personal contacts API to search for contact details and photos.</span></span> <span data-ttu-id="ec764-244">默认值为 `true`。</span><span class="sxs-lookup"><span data-stu-id="ec764-244">Default value is `true`.</span></span>  |

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="ec764-245">Microsoft Graph 权限</span><span class="sxs-lookup"><span data-stu-id="ec764-245">Microsoft Graph permissions</span></span>

<span data-ttu-id="ec764-246">此控件使用下列 Microsoft Graph API 和权限。</span><span class="sxs-lookup"><span data-stu-id="ec764-246">This control uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="ec764-247">Resource</span><span class="sxs-lookup"><span data-stu-id="ec764-247">Resource</span></span> | <span data-ttu-id="ec764-248">权限</span><span class="sxs-lookup"><span data-stu-id="ec764-248">Permission</span></span>     |
| -| - |
| [<span data-ttu-id="ec764-249">/me</span><span class="sxs-lookup"><span data-stu-id="ec764-249">/me</span></span>](/graph/api/user-get)                              | <span data-ttu-id="ec764-250">User.Read</span><span class="sxs-lookup"><span data-stu-id="ec764-250">User.Read</span></span>          |
| [<span data-ttu-id="ec764-251">/me/photo/$value</span><span class="sxs-lookup"><span data-stu-id="ec764-251">/me/photo/$value</span></span>](/graph/api/profilephoto-get)        | <span data-ttu-id="ec764-252">User.Read</span><span class="sxs-lookup"><span data-stu-id="ec764-252">User.Read</span></span>          |
| [<span data-ttu-id="ec764-253">/me/people/？$search=</span><span class="sxs-lookup"><span data-stu-id="ec764-253">/me/people/?$search=</span></span>](/graph/api/user-list-people)     | <span data-ttu-id="ec764-254">People.Read</span><span class="sxs-lookup"><span data-stu-id="ec764-254">People.Read</span></span>        |
| [<span data-ttu-id="ec764-255">/me/contacts/\*</span><span class="sxs-lookup"><span data-stu-id="ec764-255">/me/contacts/\*</span></span>](/graph/api/user-list-contacts&tabs=cs) | <span data-ttu-id="ec764-256">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="ec764-256">Contacts.Read</span></span>      |
| [<span data-ttu-id="ec764-257">/users/{id}/photo/$value</span><span class="sxs-lookup"><span data-stu-id="ec764-257">/users/{id}/photo/$value</span></span>](/graph/api/user-list-people) | <span data-ttu-id="ec764-258">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="ec764-258">User.ReadBasic.All</span></span> |
| [<span data-ttu-id="ec764-259">/me/presence</span><span class="sxs-lookup"><span data-stu-id="ec764-259">/me/presence</span></span>](/graph/api/presence-get)                | <span data-ttu-id="ec764-260">Presence.Read</span><span class="sxs-lookup"><span data-stu-id="ec764-260">Presence.Read</span></span> |
| [<span data-ttu-id="ec764-261">/users/{id}/presence</span><span class="sxs-lookup"><span data-stu-id="ec764-261">/users/{id}/presence</span></span>](/graph/api/presence-get)        | <span data-ttu-id="ec764-262">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="ec764-262">Presence.Read.All</span></span> |

## <a name="authentication"></a><span data-ttu-id="ec764-263">身份验证</span><span class="sxs-lookup"><span data-stu-id="ec764-263">Authentication</span></span>

<span data-ttu-id="ec764-264">该控件使用身份验证文档中介绍的全局身份验证提供程序[](../providers/providers.md)获取所需数据。</span><span class="sxs-lookup"><span data-stu-id="ec764-264">The control uses the global authentication provider described in the [authentication documentation](../providers/providers.md) to fetch the required data.</span></span>

## <a name="cache"></a><span data-ttu-id="ec764-265">缓存</span><span class="sxs-lookup"><span data-stu-id="ec764-265">Cache</span></span>

|<span data-ttu-id="ec764-266">对象存储</span><span class="sxs-lookup"><span data-stu-id="ec764-266">Object store</span></span>|<span data-ttu-id="ec764-267">缓存数据</span><span class="sxs-lookup"><span data-stu-id="ec764-267">Cached data</span></span>|<span data-ttu-id="ec764-268">备注</span><span class="sxs-lookup"><span data-stu-id="ec764-268">Remarks</span></span>|
|---------|-----------|-------|
|`photos`|<span data-ttu-id="ec764-269">人员照片</span><span class="sxs-lookup"><span data-stu-id="ec764-269">Person's photo</span></span>|<span data-ttu-id="ec764-270">使用 时 `avatarType` ，将 设置为 `photo` `fetchImage` ，将 设置为 `true`</span><span class="sxs-lookup"><span data-stu-id="ec764-270">Used, when `avatarType` is set to `photo` and `fetchImage` is set to `true`</span></span>|
|`presence`|<span data-ttu-id="ec764-271">人员状态</span><span class="sxs-lookup"><span data-stu-id="ec764-271">Person's presence</span></span>|<span data-ttu-id="ec764-272">已使用， `showPresence` 设置为 `true`</span><span class="sxs-lookup"><span data-stu-id="ec764-272">Used, when `showPresence` is set to `true`</span></span>|
|`users`|<span data-ttu-id="ec764-273">人员的用户信息</span><span class="sxs-lookup"><span data-stu-id="ec764-273">Person's user information</span></span>|

<span data-ttu-id="ec764-274">若要 [详细了解](../customize-components/cache.md) 如何配置缓存，请参阅缓存。</span><span class="sxs-lookup"><span data-stu-id="ec764-274">See [Caching](../customize-components/cache.md) for more details on how to configure the cache.</span></span>

## <a name="extend-for-more-control"></a><span data-ttu-id="ec764-275">扩展以了解更多控件</span><span class="sxs-lookup"><span data-stu-id="ec764-275">Extend for more control</span></span>

<span data-ttu-id="ec764-276">对于更复杂的方案或真正自定义的 UX，此组件公开了多个在组件扩展 `protected render*` 中替代的方法。</span><span class="sxs-lookup"><span data-stu-id="ec764-276">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions.</span></span>

| <span data-ttu-id="ec764-277">方法</span><span class="sxs-lookup"><span data-stu-id="ec764-277">Method</span></span> | <span data-ttu-id="ec764-278">说明</span><span class="sxs-lookup"><span data-stu-id="ec764-278">Description</span></span> |
| - | - |
| <span data-ttu-id="ec764-279">renderLoading</span><span class="sxs-lookup"><span data-stu-id="ec764-279">renderLoading</span></span> | <span data-ttu-id="ec764-280">呈现加载状态。</span><span class="sxs-lookup"><span data-stu-id="ec764-280">Renders the loading state.</span></span> |
| <span data-ttu-id="ec764-281">renderNoData</span><span class="sxs-lookup"><span data-stu-id="ec764-281">renderNoData</span></span> | <span data-ttu-id="ec764-282">当图像或人员数据不可用时呈现。</span><span class="sxs-lookup"><span data-stu-id="ec764-282">Renders when no image or person data is available.</span></span> |
| <span data-ttu-id="ec764-283">renderAvatar</span><span class="sxs-lookup"><span data-stu-id="ec764-283">renderAvatar</span></span> | <span data-ttu-id="ec764-284">呈现头像。</span><span class="sxs-lookup"><span data-stu-id="ec764-284">Renders the avatar.</span></span> |
| <span data-ttu-id="ec764-285">renderDetails</span><span class="sxs-lookup"><span data-stu-id="ec764-285">renderDetails</span></span> | <span data-ttu-id="ec764-286">呈现人员详细信息部分。</span><span class="sxs-lookup"><span data-stu-id="ec764-286">Renders the person details part.</span></span> |
