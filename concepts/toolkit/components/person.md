---
title: Microsoft Graph 服务中的人员Toolkit
description: 人员组件用于使用联系人的照片、姓名和/或电子邮件地址显示此人或联系人。
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 9ac8eebfaa4d95ccd935414329ab1dd145839dd2
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50475056"
---
# <a name="person-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="58fc4-103">Microsoft Graph 服务中的人员Toolkit</span><span class="sxs-lookup"><span data-stu-id="58fc4-103">Person component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="58fc4-104">人员组件用于通过使用联系人的照片、姓名、电子邮件地址或任何其他人员详细信息来显示此人或联系人。</span><span class="sxs-lookup"><span data-stu-id="58fc4-104">The person component is used to display a person or contact by using their photo, name, email address, or any other person details.</span></span>

<span data-ttu-id="58fc4-105">人员组件还使用 [mgt-person-card](./person-card.md) 显示包含有关用户的其他信息的飞出卡。</span><span class="sxs-lookup"><span data-stu-id="58fc4-105">The person component also uses the [mgt-person-card](./person-card.md) to display a flyout card with additional information about the user.</span></span> <span data-ttu-id="58fc4-106">有关详细信息，请参阅" [人员卡片"](#person-card) 部分。</span><span class="sxs-lookup"><span data-stu-id="58fc4-106">For details, see the [Person Card](#person-card) section.</span></span>

## <a name="example"></a><span data-ttu-id="58fc4-107">示例</span><span class="sxs-lookup"><span data-stu-id="58fc4-107">Example</span></span>

<span data-ttu-id="58fc4-108">以下示例显示使用该组件 `mgt-person` 的人。</span><span class="sxs-lookup"><span data-stu-id="58fc4-108">The following example displays a person using the `mgt-person` component.</span></span> <span data-ttu-id="58fc4-109">可以使用代码编辑器查看属性 [如何](#properties) 更改组件的行为。</span><span class="sxs-lookup"><span data-stu-id="58fc4-109">You can use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-person--person&source=docs" height="250"></iframe>

[<span data-ttu-id="58fc4-110">在 mgt.dev 中打开此示例</span><span class="sxs-lookup"><span data-stu-id="58fc4-110">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-person--person&source=docs)

## <a name="setting-the-person-details"></a><span data-ttu-id="58fc4-111">设置人员详细信息</span><span class="sxs-lookup"><span data-stu-id="58fc4-111">Setting the person details</span></span>

<span data-ttu-id="58fc4-112">可以使用三个属性来设置人员详细信息。</span><span class="sxs-lookup"><span data-stu-id="58fc4-112">You can use three properties to set the person details.</span></span> <span data-ttu-id="58fc4-113">每个实例仅使用以下属性之一：</span><span class="sxs-lookup"><span data-stu-id="58fc4-113">Use only one of the following properties per instance:</span></span>

* <span data-ttu-id="58fc4-114">设置 `user-id` 属性或 `userId` 属性以使用用户的 ID 从 Microsoft Graph 提取用户。</span><span class="sxs-lookup"><span data-stu-id="58fc4-114">Set the `user-id` attribute or `userId` property to fetch the user from Microsoft Graph by using their ID.</span></span>

* <span data-ttu-id="58fc4-115">设置 `person-query` 属性或 `personQuery` 属性以搜索 Microsoft Graph 中给定人员。</span><span class="sxs-lookup"><span data-stu-id="58fc4-115">Set the `person-query` attribute or `personQuery` property to search Microsoft Graph for a given person.</span></span> <span data-ttu-id="58fc4-116">它将选择第一个可用的人员并提取人员详细信息。</span><span class="sxs-lookup"><span data-stu-id="58fc4-116">It will choose the first person available and fetch the person details.</span></span> <span data-ttu-id="58fc4-117">电子邮件最好确保查询正确的人员，但名称也有效。</span><span class="sxs-lookup"><span data-stu-id="58fc4-117">An email works best to ensure the right person is queried, but a name works as well.</span></span>

* <span data-ttu-id="58fc4-118">设置 `person-presence` 属性以手动向个人头像添加状态 `personPresence` 锁屏提醒。</span><span class="sxs-lookup"><span data-stu-id="58fc4-118">Set the `person-presence` attribute or `personPresence` property to add a presence badge to person avatar manually.</span></span>

* <span data-ttu-id="58fc4-119">将 `avatar-size` 属性设置为 `avatarSize` 或确定头像 `small` `large` 的大小。</span><span class="sxs-lookup"><span data-stu-id="58fc4-119">Set the `avatar-size` attribute or `avatarSize` property to `small` or `large` to determine the size of avatar.</span></span> <span data-ttu-id="58fc4-120">这有助于向头像 [添加正确的状态锁](https://mgt.dev/?path=/story/components-mgt-person--person-presence-display-all) 屏提醒。</span><span class="sxs-lookup"><span data-stu-id="58fc4-120">This helps add the [correct presence badge](https://mgt.dev/?path=/story/components-mgt-person--person-presence-display-all) to avatar.</span></span> <span data-ttu-id="58fc4-121">你需要选择正确的相应的 css 自定义属性，如下所示以进一步自定义头像大小。</span><span class="sxs-lookup"><span data-stu-id="58fc4-121">You will need to choose the correct corresponding css custom properties shown below to further customize avatar size.</span></span> <span data-ttu-id="58fc4-122">默认情况下，该值设置为 `auto` ，该值将自动决定如何根据属性呈现 `view` 状态。</span><span class="sxs-lookup"><span data-stu-id="58fc4-122">By default, the value is set to `auto` which will automatically decide how to render the presence based on the `view` property.</span></span> <span data-ttu-id="58fc4-123">如果你的头 `small` 像小于 32px x 32px，我们建议使用。</span><span class="sxs-lookup"><span data-stu-id="58fc4-123">We recommend using `small` if your avatar is smaller than 32px by 32px.</span></span> 

* <span data-ttu-id="58fc4-124">使用 `person-details` 属性或 `personDetails` 属性手动设置人员详细信息，如以下示例所示。</span><span class="sxs-lookup"><span data-stu-id="58fc4-124">Use the `person-details` attribute or `personDetails` property to manually set the person details, as shown in the following example.</span></span>


    ```js
    let personControl = document.getElementById('myPersonControl');
    personControl.personDetails = {
        displayName: 'Nikola Metulev',
        mail: 'nikola@contoso.com',
        personImage: 'url'
    }
    ```

  <span data-ttu-id="58fc4-125">如果未提供图像，将提取一个 (（如果) ）。</span><span class="sxs-lookup"><span data-stu-id="58fc4-125">If no image is provided, one will be fetched (if available).</span></span>

## <a name="properties"></a><span data-ttu-id="58fc4-126">属性</span><span class="sxs-lookup"><span data-stu-id="58fc4-126">Properties</span></span>

<span data-ttu-id="58fc4-127">可以使用多个属性来自定义组件。</span><span class="sxs-lookup"><span data-stu-id="58fc4-127">You can use several properties to customize the component.</span></span>

| <span data-ttu-id="58fc4-128">属性</span><span class="sxs-lookup"><span data-stu-id="58fc4-128">Attribute</span></span>       | <span data-ttu-id="58fc4-129">属性</span><span class="sxs-lookup"><span data-stu-id="58fc4-129">Property</span></span>       | <span data-ttu-id="58fc4-130">说明</span><span class="sxs-lookup"><span data-stu-id="58fc4-130">Description</span></span>                                                   |
| -----------     | ----------     | ------------------------------------------------------------- |
| <span data-ttu-id="58fc4-131">user-id</span><span class="sxs-lookup"><span data-stu-id="58fc4-131">user-id</span></span>         | <span data-ttu-id="58fc4-132">userId</span><span class="sxs-lookup"><span data-stu-id="58fc4-132">userId</span></span>         | <span data-ttu-id="58fc4-133">设置为用户 ID 以从 Microsoft Graph 提取该用户的详细信息和图像。</span><span class="sxs-lookup"><span data-stu-id="58fc4-133">Set to a user id to fetch that user's details and image from Microsoft Graph.</span></span>|
| <span data-ttu-id="58fc4-134">person-query</span><span class="sxs-lookup"><span data-stu-id="58fc4-134">person-query</span></span>    | <span data-ttu-id="58fc4-135">personQuery</span><span class="sxs-lookup"><span data-stu-id="58fc4-135">personQuery</span></span>    | <span data-ttu-id="58fc4-136">设置为人员的名称或电子邮件，以在 Microsoft Graph 中搜索人员并提取第一个人的详细信息和图像。</span><span class="sxs-lookup"><span data-stu-id="58fc4-136">Set to a name or email of a person to search for a person in Microsoft Graph and fetch the first person's details and image.</span></span>|
| <span data-ttu-id="58fc4-137">person-details</span><span class="sxs-lookup"><span data-stu-id="58fc4-137">person-details</span></span>  | <span data-ttu-id="58fc4-138">personDetails</span><span class="sxs-lookup"><span data-stu-id="58fc4-138">personDetails</span></span>  | <span data-ttu-id="58fc4-139">设置为表示人员的对象。</span><span class="sxs-lookup"><span data-stu-id="58fc4-139">Set to an object representing a person.</span></span> <span data-ttu-id="58fc4-140">使用来自人员、用户、联系人或组、资源的对象。</span><span class="sxs-lookup"><span data-stu-id="58fc4-140">Works with object from the people, users, contacts, or group, resources.</span></span> |
| <span data-ttu-id="58fc4-141">回退详细信息</span><span class="sxs-lookup"><span data-stu-id="58fc4-141">fallback-details</span></span>| <span data-ttu-id="58fc4-142">fallbackDetails</span><span class="sxs-lookup"><span data-stu-id="58fc4-142">fallbackDetails</span></span>| <span data-ttu-id="58fc4-143">设置为在图中未找到用户/人员/联系人时代表人员的对象。</span><span class="sxs-lookup"><span data-stu-id="58fc4-143">Set to an object representing a person when no user/person/contact is found in the graph.</span></span>
| <span data-ttu-id="58fc4-144">person-image</span><span class="sxs-lookup"><span data-stu-id="58fc4-144">person-image</span></span>    | <span data-ttu-id="58fc4-145">personImage</span><span class="sxs-lookup"><span data-stu-id="58fc4-145">personImage</span></span>    | <span data-ttu-id="58fc4-146">设置要向人员显示的图像。</span><span class="sxs-lookup"><span data-stu-id="58fc4-146">Set the image to show for the person.</span></span> |
| <span data-ttu-id="58fc4-147">person-presence</span><span class="sxs-lookup"><span data-stu-id="58fc4-147">person-presence</span></span> | <span data-ttu-id="58fc4-148">personPresence</span><span class="sxs-lookup"><span data-stu-id="58fc4-148">personPresence</span></span> | <span data-ttu-id="58fc4-149">设置人员状态。</span><span class="sxs-lookup"><span data-stu-id="58fc4-149">Set the presence for the person.</span></span> |
| <span data-ttu-id="58fc4-150">fetch-image</span><span class="sxs-lookup"><span data-stu-id="58fc4-150">fetch-image</span></span>     | <span data-ttu-id="58fc4-151">fetchImage</span><span class="sxs-lookup"><span data-stu-id="58fc4-151">fetchImage</span></span>     | <span data-ttu-id="58fc4-152">将标志设置为 `personImage` 根据用户提供的对象自动从 Microsoft Graph `personDetails` 提取。</span><span class="sxs-lookup"><span data-stu-id="58fc4-152">Set flag to fetch `personImage` automatically from Microsoft Graph based on the `personDetails` object provided by the user.</span></span> |
| <span data-ttu-id="58fc4-153">头像类型</span><span class="sxs-lookup"><span data-stu-id="58fc4-153">avatar-type</span></span>     | <span data-ttu-id="58fc4-154">头像类型</span><span class="sxs-lookup"><span data-stu-id="58fc4-154">avatarType</span></span>     | <span data-ttu-id="58fc4-155">设置为 `initials` 或 `photo` 呈现任一显示状态 - 默认为照片。</span><span class="sxs-lookup"><span data-stu-id="58fc4-155">Set to `initials` or `photo` to render either display state - default is photo.</span></span> |
| <span data-ttu-id="58fc4-156">view</span><span class="sxs-lookup"><span data-stu-id="58fc4-156">view</span></span>            | <span data-ttu-id="58fc4-157">view</span><span class="sxs-lookup"><span data-stu-id="58fc4-157">view</span></span>           | <span data-ttu-id="58fc4-158">设置为控制人员呈现方式。</span><span class="sxs-lookup"><span data-stu-id="58fc4-158">Set to control how the person is rendered.</span></span> <span data-ttu-id="58fc4-159">默认值为 `avatar`</span><span class="sxs-lookup"><span data-stu-id="58fc4-159">Default is `avatar`</span></span> <br /> <span data-ttu-id="58fc4-160">`avatar` - 仅显示头像</span><span class="sxs-lookup"><span data-stu-id="58fc4-160">`avatar` - show only avatar</span></span> <br /> <span data-ttu-id="58fc4-161">`oneline` - 默认情况下显示头像 (`displayName` 第一) </span><span class="sxs-lookup"><span data-stu-id="58fc4-161">`oneline` - show avatar and first line (`displayName` by default)</span></span> <br /> <span data-ttu-id="58fc4-162">`twolines` - 显示头像和两行文本 (`displayName` `mail` 默认显示) </span><span class="sxs-lookup"><span data-stu-id="58fc4-162">`twolines` - show avatar and two lines of text (`displayName` and `mail` by default)</span></span>|
| <span data-ttu-id="58fc4-163">line1-property</span><span class="sxs-lookup"><span data-stu-id="58fc4-163">line1-property</span></span>  | <span data-ttu-id="58fc4-164">line1Property</span><span class="sxs-lookup"><span data-stu-id="58fc4-164">line1Property</span></span>  | <span data-ttu-id="58fc4-165">设置要用于第一行文本的 personDetails 的属性。</span><span class="sxs-lookup"><span data-stu-id="58fc4-165">Sets the property of the personDetails to use for the first line of text.</span></span> <span data-ttu-id="58fc4-166">默认值为“`displayName`”。</span><span class="sxs-lookup"><span data-stu-id="58fc4-166">Default is `displayName`.</span></span>|
| <span data-ttu-id="58fc4-167">line2-property</span><span class="sxs-lookup"><span data-stu-id="58fc4-167">line2-property</span></span>  | <span data-ttu-id="58fc4-168">line2Property</span><span class="sxs-lookup"><span data-stu-id="58fc4-168">line2Property</span></span>  | <span data-ttu-id="58fc4-169">设置要用于第二行文本的 personDetails 的属性。</span><span class="sxs-lookup"><span data-stu-id="58fc4-169">Sets the property of the personDetails to use for the second line of text.</span></span> <span data-ttu-id="58fc4-170">默认值为“`mail`”。</span><span class="sxs-lookup"><span data-stu-id="58fc4-170">Default is `mail`.</span></span>|
| <span data-ttu-id="58fc4-171">line3-property</span><span class="sxs-lookup"><span data-stu-id="58fc4-171">line3-property</span></span>  | <span data-ttu-id="58fc4-172">line3Property</span><span class="sxs-lookup"><span data-stu-id="58fc4-172">line3Property</span></span>  | <span data-ttu-id="58fc4-173">设置要用于第三行文本的 personDetails 的属性。</span><span class="sxs-lookup"><span data-stu-id="58fc4-173">Sets the property of the personDetails to use for the third line of text.</span></span> <span data-ttu-id="58fc4-174">默认值为“`jobTitle`”。</span><span class="sxs-lookup"><span data-stu-id="58fc4-174">Default is `jobTitle`.</span></span>|
| <span data-ttu-id="58fc4-175">show-presence</span><span class="sxs-lookup"><span data-stu-id="58fc4-175">show-presence</span></span>   | <span data-ttu-id="58fc4-176">showPresence</span><span class="sxs-lookup"><span data-stu-id="58fc4-176">showPresence</span></span>   | <span data-ttu-id="58fc4-177">设置用于显示人员状态的标志 - 默认值为 `false` 。</span><span class="sxs-lookup"><span data-stu-id="58fc4-177">Set flag to display person presence - default is `false`.</span></span>|

## <a name="css-custom-properties"></a><span data-ttu-id="58fc4-178">CSS 自定义属性</span><span class="sxs-lookup"><span data-stu-id="58fc4-178">CSS custom properties</span></span>

<span data-ttu-id="58fc4-179">组件 `mgt-person` 定义以下 CSS 自定义属性。</span><span class="sxs-lookup"><span data-stu-id="58fc4-179">The `mgt-person` component defines the following CSS custom properties.</span></span>

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

<span data-ttu-id="58fc4-180">若要了解更多信息，请参阅 [样式组件](../customize-components/style.md)。</span><span class="sxs-lookup"><span data-stu-id="58fc4-180">To learn more, see [styling components](../customize-components/style.md).</span></span>

## <a name="events"></a><span data-ttu-id="58fc4-181">活动</span><span class="sxs-lookup"><span data-stu-id="58fc4-181">Events</span></span>

<span data-ttu-id="58fc4-182">从组件中触发以下事件。</span><span class="sxs-lookup"><span data-stu-id="58fc4-182">The following events are fired from the component.</span></span>

| <span data-ttu-id="58fc4-183">事件</span><span class="sxs-lookup"><span data-stu-id="58fc4-183">Event</span></span> | <span data-ttu-id="58fc4-184">详情</span><span class="sxs-lookup"><span data-stu-id="58fc4-184">Detail</span></span> | <span data-ttu-id="58fc4-185">说明</span><span class="sxs-lookup"><span data-stu-id="58fc4-185">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="58fc4-186">line1clicked</span><span class="sxs-lookup"><span data-stu-id="58fc4-186">line1clicked</span></span> | <span data-ttu-id="58fc4-187">详细信息包含各自的 `person` 对象</span><span class="sxs-lookup"><span data-stu-id="58fc4-187">The detail contains the respective `person` object</span></span> | <span data-ttu-id="58fc4-188">单击第 1 行时触发。</span><span class="sxs-lookup"><span data-stu-id="58fc4-188">Fired when line1 is clicked.</span></span> |
| <span data-ttu-id="58fc4-189">line2clicked</span><span class="sxs-lookup"><span data-stu-id="58fc4-189">line2clicked</span></span> | <span data-ttu-id="58fc4-190">详细信息包含各自的 `person` 对象</span><span class="sxs-lookup"><span data-stu-id="58fc4-190">The detail contains the respective `person` object</span></span> | <span data-ttu-id="58fc4-191">单击第 2 行时触发。</span><span class="sxs-lookup"><span data-stu-id="58fc4-191">Fired when line2 is clicked.</span></span> |
| <span data-ttu-id="58fc4-192">line3clicked</span><span class="sxs-lookup"><span data-stu-id="58fc4-192">line3clicked</span></span> | <span data-ttu-id="58fc4-193">详细信息包含各自的 `person` 对象</span><span class="sxs-lookup"><span data-stu-id="58fc4-193">The detail contains the respective `person` object</span></span> | <span data-ttu-id="58fc4-194">单击第 3 行时触发。</span><span class="sxs-lookup"><span data-stu-id="58fc4-194">Fired when line3 is clicked.</span></span> |

## <a name="templates"></a><span data-ttu-id="58fc4-195">模板</span><span class="sxs-lookup"><span data-stu-id="58fc4-195">Templates</span></span>

<span data-ttu-id="58fc4-196">组件 `mgt-person` 支持 [多个模板](../customize-components/templates.md) ，允许您替换组件的某些部分。</span><span class="sxs-lookup"><span data-stu-id="58fc4-196">The `mgt-person` component supports several [templates](../customize-components/templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="58fc4-197">若要指定模板，请包含 `<template>` 组件中的元素，将值设置为下列 `data-type` 值之一：</span><span class="sxs-lookup"><span data-stu-id="58fc4-197">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following:</span></span>

| <span data-ttu-id="58fc4-198">数据类型</span><span class="sxs-lookup"><span data-stu-id="58fc4-198">Data type</span></span> | <span data-ttu-id="58fc4-199">数据上下文</span><span class="sxs-lookup"><span data-stu-id="58fc4-199">Data context</span></span> | <span data-ttu-id="58fc4-200">说明</span><span class="sxs-lookup"><span data-stu-id="58fc4-200">Description</span></span> |
| --------- | ------------ | ----------- |
| <span data-ttu-id="58fc4-201">loading</span><span class="sxs-lookup"><span data-stu-id="58fc4-201">loading</span></span> | <span data-ttu-id="58fc4-202">无</span><span class="sxs-lookup"><span data-stu-id="58fc4-202">none</span></span> | <span data-ttu-id="58fc4-203">组件在加载状态时要呈现的模板。</span><span class="sxs-lookup"><span data-stu-id="58fc4-203">The template to render while the component is in a loading state.</span></span> |
| <span data-ttu-id="58fc4-204">no-data</span><span class="sxs-lookup"><span data-stu-id="58fc4-204">no-data</span></span> | <span data-ttu-id="58fc4-205">无</span><span class="sxs-lookup"><span data-stu-id="58fc4-205">none</span></span> | <span data-ttu-id="58fc4-206">在无人员图像或数据可用时呈现的模板。</span><span class="sxs-lookup"><span data-stu-id="58fc4-206">The template to render when no person image or data is available.</span></span> | 
| <span data-ttu-id="58fc4-207">默认</span><span class="sxs-lookup"><span data-stu-id="58fc4-207">default</span></span> | <span data-ttu-id="58fc4-208">person：人员详细信息对象</span><span class="sxs-lookup"><span data-stu-id="58fc4-208">person: The person details object</span></span> <br> <span data-ttu-id="58fc4-209">`personImage`：图像的 URL</span><span class="sxs-lookup"><span data-stu-id="58fc4-209">`personImage`: The URL of the image</span></span> | <span data-ttu-id="58fc4-210">默认模板将整个组件替换为你自己的组件。</span><span class="sxs-lookup"><span data-stu-id="58fc4-210">The default template replaces the entire component with your own.</span></span> |
| <span data-ttu-id="58fc4-211">person-card</span><span class="sxs-lookup"><span data-stu-id="58fc4-211">person-card</span></span> | <span data-ttu-id="58fc4-212">person：人员详细信息对象</span><span class="sxs-lookup"><span data-stu-id="58fc4-212">person: The person details object</span></span> <br> <span data-ttu-id="58fc4-213">`personImage`：图像的 URL</span><span class="sxs-lookup"><span data-stu-id="58fc4-213">`personImage`: The URL of the image</span></span> | <span data-ttu-id="58fc4-214">用于更新悬停或单击时显示的 mgt-person-card 的模板。</span><span class="sxs-lookup"><span data-stu-id="58fc4-214">The template to update the mgt-person-card displayed on hover or click.</span></span> |
| <span data-ttu-id="58fc4-215">line1</span><span class="sxs-lookup"><span data-stu-id="58fc4-215">line1</span></span> | <span data-ttu-id="58fc4-216">person：人员详细信息对象</span><span class="sxs-lookup"><span data-stu-id="58fc4-216">person: The person details object</span></span> | <span data-ttu-id="58fc4-217">第一行人员元数据的模板。</span><span class="sxs-lookup"><span data-stu-id="58fc4-217">The template for the first line of person metadata.</span></span> |
| <span data-ttu-id="58fc4-218">line2</span><span class="sxs-lookup"><span data-stu-id="58fc4-218">line2</span></span> | <span data-ttu-id="58fc4-219">person：人员详细信息对象</span><span class="sxs-lookup"><span data-stu-id="58fc4-219">person: The person details object</span></span> | <span data-ttu-id="58fc4-220">第二行人员元数据的模板。</span><span class="sxs-lookup"><span data-stu-id="58fc4-220">The template for the second line of person metadata.</span></span> |
| <span data-ttu-id="58fc4-221">line3</span><span class="sxs-lookup"><span data-stu-id="58fc4-221">line3</span></span> | <span data-ttu-id="58fc4-222">person：人员详细信息对象</span><span class="sxs-lookup"><span data-stu-id="58fc4-222">person: The person details object</span></span> | <span data-ttu-id="58fc4-223">第三行人员元数据的模板。</span><span class="sxs-lookup"><span data-stu-id="58fc4-223">The template for the third line of person metadata.</span></span> |

<span data-ttu-id="58fc4-224">以下示例为人员组件定义模板。</span><span class="sxs-lookup"><span data-stu-id="58fc4-224">The following example defines a template for the person component.</span></span>

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

## <a name="person-card"></a><span data-ttu-id="58fc4-225">个人卡片</span><span class="sxs-lookup"><span data-stu-id="58fc4-225">Person card</span></span>

<span data-ttu-id="58fc4-226">组件 `mgt-person` 可以显示 `mgt-person-card` 鼠标悬停或单击。</span><span class="sxs-lookup"><span data-stu-id="58fc4-226">The `mgt-person` component can show an `mgt-person-card` on either hover or click.</span></span>

### <a name="add-the-control-to-the-html-page"></a><span data-ttu-id="58fc4-227">将控件添加到 HTML 页面</span><span class="sxs-lookup"><span data-stu-id="58fc4-227">Add the control to the HTML page</span></span>
```html
<mgt-person person-query="me" person-card="hover"></mgt-person>
```

| <span data-ttu-id="58fc4-228">属性</span><span class="sxs-lookup"><span data-stu-id="58fc4-228">Attribute</span></span>    |  <span data-ttu-id="58fc4-229">属性</span><span class="sxs-lookup"><span data-stu-id="58fc4-229">Property</span></span>     | <span data-ttu-id="58fc4-230">说明</span><span class="sxs-lookup"><span data-stu-id="58fc4-230">Description</span></span>                                                                     |
| ------------ | ------------- | ------------------------------------------------------------------------------- |
| <span data-ttu-id="58fc4-231">person-card</span><span class="sxs-lookup"><span data-stu-id="58fc4-231">person-card</span></span> | <span data-ttu-id="58fc4-232">personCardInteraction</span><span class="sxs-lookup"><span data-stu-id="58fc4-232">personCardInteraction</span></span> | <span data-ttu-id="58fc4-233">一个枚举，用于确定激活飞出面板或所需的用户 `hover` 操作 `click` 。</span><span class="sxs-lookup"><span data-stu-id="58fc4-233">An enumeration to determine user action necessary to activate flyout panel - `hover` or `click`.</span></span> <span data-ttu-id="58fc4-234">默认值为 `none`</span><span class="sxs-lookup"><span data-stu-id="58fc4-234">Default value is `none`</span></span> |


<span data-ttu-id="58fc4-235">有关模板、样式设置和属性详细信息，请参阅 Person Card [组件](./person-card.md)。</span><span class="sxs-lookup"><span data-stu-id="58fc4-235">For more information about templating, styling, and attributes, see [Person Card component](./person-card.md).</span></span>

## <a name="global-component-configuration"></a><span data-ttu-id="58fc4-236">全局组件配置</span><span class="sxs-lookup"><span data-stu-id="58fc4-236">Global component configuration</span></span>

<span data-ttu-id="58fc4-237">该类 `MgtPerson` 公开配置应用程序中所有 `config` 人员组件的静态对象。</span><span class="sxs-lookup"><span data-stu-id="58fc4-237">The `MgtPerson` class exposes a static `config` object that configures all person components in the application.</span></span>

<span data-ttu-id="58fc4-238">以下示例演示如何使用 config 对象。</span><span class="sxs-lookup"><span data-stu-id="58fc4-238">The following example shows how to use the config object.</span></span>

```ts
import { MgtPerson } from `@microsoft/mgt`;

MgtPerson.config.useContactApis = false;
```

<span data-ttu-id="58fc4-239">以下属性在 config 对象上可用。</span><span class="sxs-lookup"><span data-stu-id="58fc4-239">The following properties are available on the config object.</span></span>

| <span data-ttu-id="58fc4-240">属性</span><span class="sxs-lookup"><span data-stu-id="58fc4-240">Property</span></span> | <span data-ttu-id="58fc4-241">说明</span><span class="sxs-lookup"><span data-stu-id="58fc4-241">Description</span></span> |
| ------------ | ------------- |
| <span data-ttu-id="58fc4-242">useContactApis</span><span class="sxs-lookup"><span data-stu-id="58fc4-242">useContactApis</span></span> | <span data-ttu-id="58fc4-243">`boolean` - 指示人员组件是否可以使用 Microsoft Graph 个人联系人 API 搜索联系人详细信息和照片。</span><span class="sxs-lookup"><span data-stu-id="58fc4-243">`boolean` - Indicates whether the person component can use the Microsoft Graph personal contacts API to search for contact details and photos.</span></span> <span data-ttu-id="58fc4-244">默认值为 `true`。</span><span class="sxs-lookup"><span data-stu-id="58fc4-244">Default value is `true`.</span></span>  |

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="58fc4-245">Microsoft Graph 权限</span><span class="sxs-lookup"><span data-stu-id="58fc4-245">Microsoft Graph permissions</span></span>

<span data-ttu-id="58fc4-246">此控件使用以下 Microsoft Graph API 和权限。</span><span class="sxs-lookup"><span data-stu-id="58fc4-246">This control uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="58fc4-247">资源</span><span class="sxs-lookup"><span data-stu-id="58fc4-247">Resource</span></span> | <span data-ttu-id="58fc4-248">权限</span><span class="sxs-lookup"><span data-stu-id="58fc4-248">Permission</span></span>     |
| -| - |
| [<span data-ttu-id="58fc4-249">/me</span><span class="sxs-lookup"><span data-stu-id="58fc4-249">/me</span></span>](/graph/api/user-get)                              | <span data-ttu-id="58fc4-250">User.Read</span><span class="sxs-lookup"><span data-stu-id="58fc4-250">User.Read</span></span>          |
| [<span data-ttu-id="58fc4-251">/me/photo/$value</span><span class="sxs-lookup"><span data-stu-id="58fc4-251">/me/photo/$value</span></span>](/graph/api/profilephoto-get)        | <span data-ttu-id="58fc4-252">User.Read</span><span class="sxs-lookup"><span data-stu-id="58fc4-252">User.Read</span></span>          |
| [<span data-ttu-id="58fc4-253">/me/people/？$search=</span><span class="sxs-lookup"><span data-stu-id="58fc4-253">/me/people/?$search=</span></span>](/graph/api/user-list-people)     | <span data-ttu-id="58fc4-254">People.Read</span><span class="sxs-lookup"><span data-stu-id="58fc4-254">People.Read</span></span>        |
| [<span data-ttu-id="58fc4-255">/me/contacts/\*</span><span class="sxs-lookup"><span data-stu-id="58fc4-255">/me/contacts/\*</span></span>](/graph/api/user-list-contacts&tabs=cs) | <span data-ttu-id="58fc4-256">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="58fc4-256">Contacts.Read</span></span>      |
| [<span data-ttu-id="58fc4-257">/users/{id}/photo/$value</span><span class="sxs-lookup"><span data-stu-id="58fc4-257">/users/{id}/photo/$value</span></span>](/graph/api/user-list-people) | <span data-ttu-id="58fc4-258">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="58fc4-258">User.ReadBasic.All</span></span> |
| [<span data-ttu-id="58fc4-259">/me/presence</span><span class="sxs-lookup"><span data-stu-id="58fc4-259">/me/presence</span></span>](/graph/api/presence-get)                | <span data-ttu-id="58fc4-260">Presence.Read</span><span class="sxs-lookup"><span data-stu-id="58fc4-260">Presence.Read</span></span> |
| [<span data-ttu-id="58fc4-261">/users/{id}/presence</span><span class="sxs-lookup"><span data-stu-id="58fc4-261">/users/{id}/presence</span></span>](/graph/api/presence-get)        | <span data-ttu-id="58fc4-262">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="58fc4-262">Presence.Read.All</span></span> |

## <a name="authentication"></a><span data-ttu-id="58fc4-263">身份验证</span><span class="sxs-lookup"><span data-stu-id="58fc4-263">Authentication</span></span>

<span data-ttu-id="58fc4-264">该控件使用身份验证文档中介绍的全局身份验证提供程序[](../providers/providers.md)获取所需数据。</span><span class="sxs-lookup"><span data-stu-id="58fc4-264">The control uses the global authentication provider described in the [authentication documentation](../providers/providers.md) to fetch the required data.</span></span>

## <a name="extend-for-more-control"></a><span data-ttu-id="58fc4-265">扩展以更多控制</span><span class="sxs-lookup"><span data-stu-id="58fc4-265">Extend for more control</span></span>

<span data-ttu-id="58fc4-266">对于更复杂的方案或真正自定义的 UX，此组件公开了多个在组件扩展 `protected render*` 中替代的方法。</span><span class="sxs-lookup"><span data-stu-id="58fc4-266">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions.</span></span>

| <span data-ttu-id="58fc4-267">方法</span><span class="sxs-lookup"><span data-stu-id="58fc4-267">Method</span></span> | <span data-ttu-id="58fc4-268">说明</span><span class="sxs-lookup"><span data-stu-id="58fc4-268">Description</span></span> |
| - | - |
| <span data-ttu-id="58fc4-269">renderLoading</span><span class="sxs-lookup"><span data-stu-id="58fc4-269">renderLoading</span></span> | <span data-ttu-id="58fc4-270">呈现加载状态。</span><span class="sxs-lookup"><span data-stu-id="58fc4-270">Renders the loading state.</span></span> |
| <span data-ttu-id="58fc4-271">renderNoData</span><span class="sxs-lookup"><span data-stu-id="58fc4-271">renderNoData</span></span> | <span data-ttu-id="58fc4-272">当图像或人员数据不可用时呈现。</span><span class="sxs-lookup"><span data-stu-id="58fc4-272">Renders when no image or person data is available.</span></span> |
| <span data-ttu-id="58fc4-273">renderAvatar</span><span class="sxs-lookup"><span data-stu-id="58fc4-273">renderAvatar</span></span> | <span data-ttu-id="58fc4-274">呈现头像。</span><span class="sxs-lookup"><span data-stu-id="58fc4-274">Renders the avatar.</span></span> |
| <span data-ttu-id="58fc4-275">renderDetails</span><span class="sxs-lookup"><span data-stu-id="58fc4-275">renderDetails</span></span> | <span data-ttu-id="58fc4-276">呈现人员详细信息部分。</span><span class="sxs-lookup"><span data-stu-id="58fc4-276">Renders the person details part.</span></span> |
