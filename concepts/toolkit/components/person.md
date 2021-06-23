---
title: Microsoft 服务中的人员Graph Toolkit
description: 人员组件用于通过使用联系人的照片、姓名和/或电子邮件地址来显示此人或联系人。
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 7f35b5c1a3ef764995d319e9e603489b50a1fe2c
ms.sourcegitcommit: 9ac6bbab3df22e7629cf2bde796b527337c680aa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/23/2021
ms.locfileid: "53082046"
---
# <a name="person-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="229cc-103">Microsoft 服务中的人员Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="229cc-103">Person component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="229cc-104">人员组件用于通过使用其照片、姓名、电子邮件地址或其他任何人员详细信息来显示此人或联系人。</span><span class="sxs-lookup"><span data-stu-id="229cc-104">The person component is used to display a person or contact by using their photo, name, email address, or any other person details.</span></span>

<span data-ttu-id="229cc-105">人员组件还使用 [mgt-person-card](./person-card.md) 显示包含有关用户的其他信息的飞出卡。</span><span class="sxs-lookup"><span data-stu-id="229cc-105">The person component also uses the [mgt-person-card](./person-card.md) to display a flyout card with additional information about the user.</span></span> <span data-ttu-id="229cc-106">有关详细信息，请参阅人员 [卡片](#person-card) 部分。</span><span class="sxs-lookup"><span data-stu-id="229cc-106">For details, see the [Person Card](#person-card) section.</span></span>

## <a name="example"></a><span data-ttu-id="229cc-107">示例</span><span class="sxs-lookup"><span data-stu-id="229cc-107">Example</span></span>

<span data-ttu-id="229cc-108">以下示例显示使用该组件 `mgt-person` 的人。</span><span class="sxs-lookup"><span data-stu-id="229cc-108">The following example displays a person using the `mgt-person` component.</span></span> <span data-ttu-id="229cc-109">可以使用代码编辑器查看 [属性如何](#properties) 更改组件的行为。</span><span class="sxs-lookup"><span data-stu-id="229cc-109">You can use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-person--person&source=docs" height="250"></iframe>

[<span data-ttu-id="229cc-110">在 mgt.dev 中打开此示例</span><span class="sxs-lookup"><span data-stu-id="229cc-110">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-person--person&source=docs)

## <a name="setting-the-person-details"></a><span data-ttu-id="229cc-111">设置人员详细信息</span><span class="sxs-lookup"><span data-stu-id="229cc-111">Setting the person details</span></span>

<span data-ttu-id="229cc-112">可以使用三个属性来设置人员详细信息。</span><span class="sxs-lookup"><span data-stu-id="229cc-112">You can use three properties to set the person details.</span></span> <span data-ttu-id="229cc-113">每个实例仅使用以下属性之一：</span><span class="sxs-lookup"><span data-stu-id="229cc-113">Use only one of the following properties per instance:</span></span>

* <span data-ttu-id="229cc-114">设置 `user-id` 属性或 `userId` 属性以通过使用用户的 ID 从 Microsoft Graph获取用户。</span><span class="sxs-lookup"><span data-stu-id="229cc-114">Set the `user-id` attribute or `userId` property to fetch the user from Microsoft Graph by using their ID.</span></span>

* <span data-ttu-id="229cc-115">设置 `person-query` 属性或 `personQuery` 属性以搜索 Microsoft Graph给定人员。</span><span class="sxs-lookup"><span data-stu-id="229cc-115">Set the `person-query` attribute or `personQuery` property to search Microsoft Graph for a given person.</span></span> <span data-ttu-id="229cc-116">它将选择第一个可用的人员并提取该人员的详细信息。</span><span class="sxs-lookup"><span data-stu-id="229cc-116">It will choose the first person available and fetch the person details.</span></span> <span data-ttu-id="229cc-117">电子邮件最适用于确保查询正确的人员，但名称也有效。</span><span class="sxs-lookup"><span data-stu-id="229cc-117">An email works best to ensure the right person is queried, but a name works as well.</span></span>

* <span data-ttu-id="229cc-118">设置 `person-presence` 属性或 `personPresence` 属性以手动向个人头像添加状态锁屏提醒。</span><span class="sxs-lookup"><span data-stu-id="229cc-118">Set the `person-presence` attribute or `personPresence` property to add a presence badge to person avatar manually.</span></span>

* <span data-ttu-id="229cc-119">将 `avatar-size` 属性或 `avatarSize` 属性设置为 `small` 或 `large` 确定头像的大小。</span><span class="sxs-lookup"><span data-stu-id="229cc-119">Set the `avatar-size` attribute or `avatarSize` property to `small` or `large` to determine the size of avatar.</span></span> <span data-ttu-id="229cc-120">这有助于向头像 [添加正确的状态](https://mgt.dev/?path=/story/components-mgt-person--person-presence-display-all) 锁屏提醒。</span><span class="sxs-lookup"><span data-stu-id="229cc-120">This helps add the [correct presence badge](https://mgt.dev/?path=/story/components-mgt-person--person-presence-display-all) to avatar.</span></span> <span data-ttu-id="229cc-121">你将需要选择正确的相应的 css 自定义属性，如下所示以进一步自定义头像大小。</span><span class="sxs-lookup"><span data-stu-id="229cc-121">You will need to choose the correct corresponding css custom properties shown below to further customize avatar size.</span></span> <span data-ttu-id="229cc-122">默认情况下，值设置为 ，该值将自动根据 属性 `auto` 决定如何呈现 `view` 状态。</span><span class="sxs-lookup"><span data-stu-id="229cc-122">By default, the value is set to `auto` which will automatically decide how to render the presence based on the `view` property.</span></span> <span data-ttu-id="229cc-123">如果你的头 `small` 像小于 32px x 32px，我们建议使用 。</span><span class="sxs-lookup"><span data-stu-id="229cc-123">We recommend using `small` if your avatar is smaller than 32px by 32px.</span></span> 

* <span data-ttu-id="229cc-124">使用 `person-details` 属性 `personDetails` 或 属性手动设置人员详细信息，如以下示例所示。</span><span class="sxs-lookup"><span data-stu-id="229cc-124">Use the `person-details` attribute or `personDetails` property to manually set the person details, as shown in the following example.</span></span>


    ```js
    let personControl = document.getElementById('myPersonControl');
    personControl.personDetails = {
        displayName: 'Nikola Metulev',
        mail: 'nikola@contoso.com',
        personImage: 'url'
    }
    ```

  <span data-ttu-id="229cc-125">如果未提供图像，将提取一个 (（如果) ）。</span><span class="sxs-lookup"><span data-stu-id="229cc-125">If no image is provided, one will be fetched (if available).</span></span>

* <span data-ttu-id="229cc-126">默认情况下，人员组件将仅请求标准 Microsoft Graph属性[集。](/graph/api/user-get?&tabs=http#optional-query-parameters)</span><span class="sxs-lookup"><span data-stu-id="229cc-126">By default, the person component will only request the standard Microsoft Graph user set of [properties](/graph/api/user-get?&tabs=http#optional-query-parameters).</span></span> <span data-ttu-id="229cc-127">为了请求其他属性，请将其声明为 的任何部分 `line(x)Property` 。</span><span class="sxs-lookup"><span data-stu-id="229cc-127">In order to request additional properties, declare them as any part of the `line(x)Property`.</span></span> 


## <a name="properties"></a><span data-ttu-id="229cc-128">属性</span><span class="sxs-lookup"><span data-stu-id="229cc-128">Properties</span></span>

<span data-ttu-id="229cc-129">可以使用多个属性来自定义组件。</span><span class="sxs-lookup"><span data-stu-id="229cc-129">You can use several properties to customize the component.</span></span>

| <span data-ttu-id="229cc-130">属性</span><span class="sxs-lookup"><span data-stu-id="229cc-130">Attribute</span></span>       | <span data-ttu-id="229cc-131">属性</span><span class="sxs-lookup"><span data-stu-id="229cc-131">Property</span></span>       | <span data-ttu-id="229cc-132">说明</span><span class="sxs-lookup"><span data-stu-id="229cc-132">Description</span></span>                                                   |
| -----------     | ----------     | ------------------------------------------------------------- |
| <span data-ttu-id="229cc-133">user-id</span><span class="sxs-lookup"><span data-stu-id="229cc-133">user-id</span></span>         | <span data-ttu-id="229cc-134">userId</span><span class="sxs-lookup"><span data-stu-id="229cc-134">userId</span></span>         | <span data-ttu-id="229cc-135">设置为用户 ID 以从 Microsoft Graph 获取该用户的详细信息和Graph。</span><span class="sxs-lookup"><span data-stu-id="229cc-135">Set to a user id to fetch that user's details and image from Microsoft Graph.</span></span>|
| <span data-ttu-id="229cc-136">person-query</span><span class="sxs-lookup"><span data-stu-id="229cc-136">person-query</span></span>    | <span data-ttu-id="229cc-137">personQuery</span><span class="sxs-lookup"><span data-stu-id="229cc-137">personQuery</span></span>    | <span data-ttu-id="229cc-138">设置为某人的姓名或电子邮件，以在 Microsoft Graph并提取第一个人的详细信息和图像。</span><span class="sxs-lookup"><span data-stu-id="229cc-138">Set to a name or email of a person to search for a person in Microsoft Graph and fetch the first person's details and image.</span></span>|
| <span data-ttu-id="229cc-139">person-details</span><span class="sxs-lookup"><span data-stu-id="229cc-139">person-details</span></span>  | <span data-ttu-id="229cc-140">personDetails</span><span class="sxs-lookup"><span data-stu-id="229cc-140">personDetails</span></span>  | <span data-ttu-id="229cc-141">设置为表示人员的对象。</span><span class="sxs-lookup"><span data-stu-id="229cc-141">Set to an object representing a person.</span></span> <span data-ttu-id="229cc-142">使用来自人员、用户、联系人或组、资源的对象。</span><span class="sxs-lookup"><span data-stu-id="229cc-142">Works with object from the people, users, contacts, or group, resources.</span></span> |
| <span data-ttu-id="229cc-143">fallback-details</span><span class="sxs-lookup"><span data-stu-id="229cc-143">fallback-details</span></span>| <span data-ttu-id="229cc-144">fallbackDetails</span><span class="sxs-lookup"><span data-stu-id="229cc-144">fallbackDetails</span></span>| <span data-ttu-id="229cc-145">设置为一个对象，该对象表示在图形中找不到用户/人员/联系人时的用户。</span><span class="sxs-lookup"><span data-stu-id="229cc-145">Set to an object representing a person when no user/person/contact is found in the graph.</span></span>
| <span data-ttu-id="229cc-146">person-image</span><span class="sxs-lookup"><span data-stu-id="229cc-146">person-image</span></span>    | <span data-ttu-id="229cc-147">personImage</span><span class="sxs-lookup"><span data-stu-id="229cc-147">personImage</span></span>    | <span data-ttu-id="229cc-148">设置要向人员显示的图像。</span><span class="sxs-lookup"><span data-stu-id="229cc-148">Set the image to show for the person.</span></span> |
| <span data-ttu-id="229cc-149">person-presence</span><span class="sxs-lookup"><span data-stu-id="229cc-149">person-presence</span></span> | <span data-ttu-id="229cc-150">personPresence</span><span class="sxs-lookup"><span data-stu-id="229cc-150">personPresence</span></span> | <span data-ttu-id="229cc-151">为人员设置状态。</span><span class="sxs-lookup"><span data-stu-id="229cc-151">Set the presence for the person.</span></span> |
| <span data-ttu-id="229cc-152">fetch-image</span><span class="sxs-lookup"><span data-stu-id="229cc-152">fetch-image</span></span>     | <span data-ttu-id="229cc-153">fetchImage</span><span class="sxs-lookup"><span data-stu-id="229cc-153">fetchImage</span></span>     | <span data-ttu-id="229cc-154">将标志设置为根据Graph自动从 Microsoft 网站 `personImage` `personDetails` 提取。</span><span class="sxs-lookup"><span data-stu-id="229cc-154">Set flag to fetch `personImage` automatically from Microsoft Graph based on the `personDetails` object provided by the user.</span></span> |
| <span data-ttu-id="229cc-155">头像类型</span><span class="sxs-lookup"><span data-stu-id="229cc-155">avatar-type</span></span>     | <span data-ttu-id="229cc-156">头像类型</span><span class="sxs-lookup"><span data-stu-id="229cc-156">avatarType</span></span>     | <span data-ttu-id="229cc-157">设置为 或 `initials` `photo` 呈现任一显示状态 - 默认为照片。</span><span class="sxs-lookup"><span data-stu-id="229cc-157">Set to `initials` or `photo` to render either display state - default is photo.</span></span> |
| <span data-ttu-id="229cc-158">view</span><span class="sxs-lookup"><span data-stu-id="229cc-158">view</span></span>            | <span data-ttu-id="229cc-159">view</span><span class="sxs-lookup"><span data-stu-id="229cc-159">view</span></span>           | <span data-ttu-id="229cc-160">设置为控制呈现人员的方式。</span><span class="sxs-lookup"><span data-stu-id="229cc-160">Set to control how the person is rendered.</span></span> <span data-ttu-id="229cc-161">默认值为 `avatar`</span><span class="sxs-lookup"><span data-stu-id="229cc-161">Default is `avatar`</span></span> <br /> <span data-ttu-id="229cc-162">`avatar` - 仅显示头像</span><span class="sxs-lookup"><span data-stu-id="229cc-162">`avatar` - show only avatar</span></span> <br /> <span data-ttu-id="229cc-163">`oneline` - 默认显示头像 (`displayName` 第一) </span><span class="sxs-lookup"><span data-stu-id="229cc-163">`oneline` - show avatar and first line (`displayName` by default)</span></span> <br /> <span data-ttu-id="229cc-164">`twolines` - 显示头像和两行文本 (`displayName` `mail` 默认显示) </span><span class="sxs-lookup"><span data-stu-id="229cc-164">`twolines` - show avatar and two lines of text (`displayName` and `mail` by default)</span></span>|
| <span data-ttu-id="229cc-165">line1-property</span><span class="sxs-lookup"><span data-stu-id="229cc-165">line1-property</span></span>  | <span data-ttu-id="229cc-166">line1Property</span><span class="sxs-lookup"><span data-stu-id="229cc-166">line1Property</span></span>  | <span data-ttu-id="229cc-167">设置要用于第一行文本的 personDetails 的属性。</span><span class="sxs-lookup"><span data-stu-id="229cc-167">Sets the property of the personDetails to use for the first line of text.</span></span> <span data-ttu-id="229cc-168">默认值为“`displayName`”。</span><span class="sxs-lookup"><span data-stu-id="229cc-168">Default is `displayName`.</span></span>|
| <span data-ttu-id="229cc-169">line2-property</span><span class="sxs-lookup"><span data-stu-id="229cc-169">line2-property</span></span>  | <span data-ttu-id="229cc-170">line2Property</span><span class="sxs-lookup"><span data-stu-id="229cc-170">line2Property</span></span>  | <span data-ttu-id="229cc-171">设置要用于第二行文本的 personDetails 的属性。</span><span class="sxs-lookup"><span data-stu-id="229cc-171">Sets the property of the personDetails to use for the second line of text.</span></span> <span data-ttu-id="229cc-172">默认值为“`mail`”。</span><span class="sxs-lookup"><span data-stu-id="229cc-172">Default is `mail`.</span></span>|
| <span data-ttu-id="229cc-173">line3-property</span><span class="sxs-lookup"><span data-stu-id="229cc-173">line3-property</span></span>  | <span data-ttu-id="229cc-174">line3Property</span><span class="sxs-lookup"><span data-stu-id="229cc-174">line3Property</span></span>  | <span data-ttu-id="229cc-175">设置要用于第三行文本的 personDetails 的属性。</span><span class="sxs-lookup"><span data-stu-id="229cc-175">Sets the property of the personDetails to use for the third line of text.</span></span> <span data-ttu-id="229cc-176">默认值为“`jobTitle`”。</span><span class="sxs-lookup"><span data-stu-id="229cc-176">Default is `jobTitle`.</span></span>|
| <span data-ttu-id="229cc-177">show-presence</span><span class="sxs-lookup"><span data-stu-id="229cc-177">show-presence</span></span>   | <span data-ttu-id="229cc-178">showPresence</span><span class="sxs-lookup"><span data-stu-id="229cc-178">showPresence</span></span>   | <span data-ttu-id="229cc-179">设置用于显示人员状态的标志 - 默认为 `false` 。</span><span class="sxs-lookup"><span data-stu-id="229cc-179">Set flag to display person presence - default is `false`.</span></span>|

## <a name="css-custom-properties"></a><span data-ttu-id="229cc-180">CSS 自定义属性</span><span class="sxs-lookup"><span data-stu-id="229cc-180">CSS custom properties</span></span>

<span data-ttu-id="229cc-181">组件 `mgt-person` 定义以下 CSS 自定义属性。</span><span class="sxs-lookup"><span data-stu-id="229cc-181">The `mgt-person` component defines the following CSS custom properties.</span></span>

```css
mgt-person {
  --avatar-size: 48px;
  --avatar-border: 0;
  --avatar-border-radius: 50%;
  --avatar-cursor: default;
  
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

<span data-ttu-id="229cc-182">若要了解更多信息，请参阅 [设置组件样式](../customize-components/style.md)。</span><span class="sxs-lookup"><span data-stu-id="229cc-182">To learn more, see [styling components](../customize-components/style.md).</span></span>

## <a name="events"></a><span data-ttu-id="229cc-183">活动</span><span class="sxs-lookup"><span data-stu-id="229cc-183">Events</span></span>

<span data-ttu-id="229cc-184">从组件中触发以下事件。</span><span class="sxs-lookup"><span data-stu-id="229cc-184">The following events are fired from the component.</span></span>

| <span data-ttu-id="229cc-185">事件</span><span class="sxs-lookup"><span data-stu-id="229cc-185">Event</span></span> | <span data-ttu-id="229cc-186">详情</span><span class="sxs-lookup"><span data-stu-id="229cc-186">Detail</span></span> | <span data-ttu-id="229cc-187">说明</span><span class="sxs-lookup"><span data-stu-id="229cc-187">Description</span></span> |
| --- | --- | --- |
| `line1clicked` | <span data-ttu-id="229cc-188">详细信息包含各自的 `person` 对象</span><span class="sxs-lookup"><span data-stu-id="229cc-188">The detail contains the respective `person` object</span></span> | <span data-ttu-id="229cc-189">在单击第 1 行时触发。</span><span class="sxs-lookup"><span data-stu-id="229cc-189">Fired when line1 is clicked.</span></span> |
| `line2clicked` | <span data-ttu-id="229cc-190">详细信息包含各自的 `person` 对象</span><span class="sxs-lookup"><span data-stu-id="229cc-190">The detail contains the respective `person` object</span></span> | <span data-ttu-id="229cc-191">在单击第 2 行时触发。</span><span class="sxs-lookup"><span data-stu-id="229cc-191">Fired when line2 is clicked.</span></span> |
| `line3clicked` | <span data-ttu-id="229cc-192">详细信息包含各自的 `person` 对象</span><span class="sxs-lookup"><span data-stu-id="229cc-192">The detail contains the respective `person` object</span></span> | <span data-ttu-id="229cc-193">在单击第 3 行时触发。</span><span class="sxs-lookup"><span data-stu-id="229cc-193">Fired when line3 is clicked.</span></span> |

<span data-ttu-id="229cc-194">有关处理事件的信息，请参阅 [事件](../customize-components/events.md)。</span><span class="sxs-lookup"><span data-stu-id="229cc-194">For more information about handling events, see [events](../customize-components/events.md).</span></span>

## <a name="templates"></a><span data-ttu-id="229cc-195">模板</span><span class="sxs-lookup"><span data-stu-id="229cc-195">Templates</span></span>

<span data-ttu-id="229cc-196">组件 `mgt-person` 支持 [多个模板](../customize-components/templates.md) ，允许您替换组件的某些部分。</span><span class="sxs-lookup"><span data-stu-id="229cc-196">The `mgt-person` component supports several [templates](../customize-components/templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="229cc-197">若要指定模板，请包含组件 `<template>` 中的元素，将值 `data-type` 设置为下列值之一：</span><span class="sxs-lookup"><span data-stu-id="229cc-197">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following:</span></span>

| <span data-ttu-id="229cc-198">数据类型</span><span class="sxs-lookup"><span data-stu-id="229cc-198">Data type</span></span> | <span data-ttu-id="229cc-199">数据上下文</span><span class="sxs-lookup"><span data-stu-id="229cc-199">Data context</span></span> | <span data-ttu-id="229cc-200">说明</span><span class="sxs-lookup"><span data-stu-id="229cc-200">Description</span></span> |
| --------- | ------------ | ----------- |
| <span data-ttu-id="229cc-201">loading</span><span class="sxs-lookup"><span data-stu-id="229cc-201">loading</span></span> | <span data-ttu-id="229cc-202">无</span><span class="sxs-lookup"><span data-stu-id="229cc-202">none</span></span> | <span data-ttu-id="229cc-203">组件在加载状态时要呈现的模板。</span><span class="sxs-lookup"><span data-stu-id="229cc-203">The template to render while the component is in a loading state.</span></span> |
| <span data-ttu-id="229cc-204">no-data</span><span class="sxs-lookup"><span data-stu-id="229cc-204">no-data</span></span> | <span data-ttu-id="229cc-205">无</span><span class="sxs-lookup"><span data-stu-id="229cc-205">none</span></span> | <span data-ttu-id="229cc-206">在没有任何人员图像或数据可用时要呈现的模板。</span><span class="sxs-lookup"><span data-stu-id="229cc-206">The template to render when no person image or data is available.</span></span> | 
| <span data-ttu-id="229cc-207">default</span><span class="sxs-lookup"><span data-stu-id="229cc-207">default</span></span> | <span data-ttu-id="229cc-208">person： The person details object</span><span class="sxs-lookup"><span data-stu-id="229cc-208">person: The person details object</span></span> <br> <span data-ttu-id="229cc-209">`personImage`：图像的 URL</span><span class="sxs-lookup"><span data-stu-id="229cc-209">`personImage`: The URL of the image</span></span> <br> <span data-ttu-id="229cc-210">`personPresence`：人员状态详细信息对象</span><span class="sxs-lookup"><span data-stu-id="229cc-210">`personPresence`: The presence details object for person</span></span>  | <span data-ttu-id="229cc-211">默认模板将整个组件替换为你自己的组件。</span><span class="sxs-lookup"><span data-stu-id="229cc-211">The default template replaces the entire component with your own.</span></span> |
| <span data-ttu-id="229cc-212">person-card</span><span class="sxs-lookup"><span data-stu-id="229cc-212">person-card</span></span> | <span data-ttu-id="229cc-213">person： The person details object</span><span class="sxs-lookup"><span data-stu-id="229cc-213">person: The person details object</span></span> <br> <span data-ttu-id="229cc-214">`personImage`：图像的 URL</span><span class="sxs-lookup"><span data-stu-id="229cc-214">`personImage`: The URL of the image</span></span> | <span data-ttu-id="229cc-215">用于更新悬停或单击时显示的 mgt-person-card 的模板。</span><span class="sxs-lookup"><span data-stu-id="229cc-215">The template to update the mgt-person-card displayed on hover or click.</span></span> |
| <span data-ttu-id="229cc-216">line1</span><span class="sxs-lookup"><span data-stu-id="229cc-216">line1</span></span> | <span data-ttu-id="229cc-217">person： The person details object</span><span class="sxs-lookup"><span data-stu-id="229cc-217">person: The person details object</span></span> | <span data-ttu-id="229cc-218">第一行人员元数据的模板。</span><span class="sxs-lookup"><span data-stu-id="229cc-218">The template for the first line of person metadata.</span></span> |
| <span data-ttu-id="229cc-219">line2</span><span class="sxs-lookup"><span data-stu-id="229cc-219">line2</span></span> | <span data-ttu-id="229cc-220">person： The person details object</span><span class="sxs-lookup"><span data-stu-id="229cc-220">person: The person details object</span></span> | <span data-ttu-id="229cc-221">第二行人员元数据的模板。</span><span class="sxs-lookup"><span data-stu-id="229cc-221">The template for the second line of person metadata.</span></span> |
| <span data-ttu-id="229cc-222">line3</span><span class="sxs-lookup"><span data-stu-id="229cc-222">line3</span></span> | <span data-ttu-id="229cc-223">person： The person details object</span><span class="sxs-lookup"><span data-stu-id="229cc-223">person: The person details object</span></span> | <span data-ttu-id="229cc-224">第三行人员元数据的模板。</span><span class="sxs-lookup"><span data-stu-id="229cc-224">The template for the third line of person metadata.</span></span> |

<span data-ttu-id="229cc-225">下面的示例定义人员组件的模板。</span><span class="sxs-lookup"><span data-stu-id="229cc-225">The following example defines a template for the person component.</span></span>

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

## <a name="person-card"></a><span data-ttu-id="229cc-226">个人卡片</span><span class="sxs-lookup"><span data-stu-id="229cc-226">Person card</span></span>

<span data-ttu-id="229cc-227">组件 `mgt-person` 可以在悬停 `mgt-person-card` 或单击时显示 。</span><span class="sxs-lookup"><span data-stu-id="229cc-227">The `mgt-person` component can show an `mgt-person-card` on either hover or click.</span></span>

### <a name="add-the-control-to-the-html-page"></a><span data-ttu-id="229cc-228">将控件添加到 HTML 页面</span><span class="sxs-lookup"><span data-stu-id="229cc-228">Add the control to the HTML page</span></span>
```html
<mgt-person person-query="me" person-card="hover"></mgt-person>
```

| <span data-ttu-id="229cc-229">属性</span><span class="sxs-lookup"><span data-stu-id="229cc-229">Attribute</span></span>    |  <span data-ttu-id="229cc-230">属性</span><span class="sxs-lookup"><span data-stu-id="229cc-230">Property</span></span>     | <span data-ttu-id="229cc-231">说明</span><span class="sxs-lookup"><span data-stu-id="229cc-231">Description</span></span>                                                                     |
| ------------ | ------------- | ------------------------------------------------------------------------------- |
| <span data-ttu-id="229cc-232">person-card</span><span class="sxs-lookup"><span data-stu-id="229cc-232">person-card</span></span> | <span data-ttu-id="229cc-233">personCardInteraction</span><span class="sxs-lookup"><span data-stu-id="229cc-233">personCardInteraction</span></span> | <span data-ttu-id="229cc-234">一个枚举，用于确定激活飞出面板或 所需的用户 `hover` 操作 `click` 。</span><span class="sxs-lookup"><span data-stu-id="229cc-234">An enumeration to determine user action necessary to activate flyout panel - `hover` or `click`.</span></span> <span data-ttu-id="229cc-235">默认值为 `none`</span><span class="sxs-lookup"><span data-stu-id="229cc-235">Default value is `none`</span></span> |


<span data-ttu-id="229cc-236">有关模板、样式设置和属性详细信息，请参阅 Person Card [component](./person-card.md)。</span><span class="sxs-lookup"><span data-stu-id="229cc-236">For more information about templating, styling, and attributes, see [Person Card component](./person-card.md).</span></span>

## <a name="global-component-configuration"></a><span data-ttu-id="229cc-237">全局组件配置</span><span class="sxs-lookup"><span data-stu-id="229cc-237">Global component configuration</span></span>

<span data-ttu-id="229cc-238">类 `MgtPerson` 公开一个 `config` 静态对象，该对象配置应用程序中的每个人组件。</span><span class="sxs-lookup"><span data-stu-id="229cc-238">The `MgtPerson` class exposes a static `config` object that configures all person components in the application.</span></span>

<span data-ttu-id="229cc-239">以下示例演示如何使用 config 对象。</span><span class="sxs-lookup"><span data-stu-id="229cc-239">The following example shows how to use the config object.</span></span>

```ts
import { MgtPerson } from `@microsoft/mgt`;

MgtPerson.config.useContactApis = false;
```

<span data-ttu-id="229cc-240">以下属性在 config 对象上可用。</span><span class="sxs-lookup"><span data-stu-id="229cc-240">The following properties are available on the config object.</span></span>

| <span data-ttu-id="229cc-241">属性</span><span class="sxs-lookup"><span data-stu-id="229cc-241">Property</span></span> | <span data-ttu-id="229cc-242">说明</span><span class="sxs-lookup"><span data-stu-id="229cc-242">Description</span></span> |
| ------------ | ------------- |
| <span data-ttu-id="229cc-243">useContactApis</span><span class="sxs-lookup"><span data-stu-id="229cc-243">useContactApis</span></span> | <span data-ttu-id="229cc-244">`boolean`- 指示人员组件是否可以使用 Microsoft Graph联系人 API 搜索联系人详细信息和照片。</span><span class="sxs-lookup"><span data-stu-id="229cc-244">`boolean` - Indicates whether the person component can use the Microsoft Graph personal contacts API to search for contact details and photos.</span></span> <span data-ttu-id="229cc-245">默认值为 `true`。</span><span class="sxs-lookup"><span data-stu-id="229cc-245">Default value is `true`.</span></span>  |

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="229cc-246">Microsoft Graph 权限</span><span class="sxs-lookup"><span data-stu-id="229cc-246">Microsoft Graph permissions</span></span>

<span data-ttu-id="229cc-247">此控件使用下列 Microsoft Graph API 和权限。</span><span class="sxs-lookup"><span data-stu-id="229cc-247">This control uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="229cc-248">配置</span><span class="sxs-lookup"><span data-stu-id="229cc-248">Configuration</span></span> | <span data-ttu-id="229cc-249">权限</span><span class="sxs-lookup"><span data-stu-id="229cc-249">Permission</span></span> | <span data-ttu-id="229cc-250">API</span><span class="sxs-lookup"><span data-stu-id="229cc-250">API</span></span> |
| ------------- | ---------- | --- |
| <span data-ttu-id="229cc-251">`personDetails` set without image， `fetchImage` set to ， set to ， `true` `avatarType` `photo` retrieved person is a contact and `useContactApis` set to `true`</span><span class="sxs-lookup"><span data-stu-id="229cc-251">`personDetails` set without image, `fetchImage` set to `true`, `avatarType` set to `photo`, retrieved person is a contact and `useContactApis` set to `true`</span></span> | <span data-ttu-id="229cc-252">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="229cc-252">Contacts.Read</span></span> | [<span data-ttu-id="229cc-253">/me/contacts/\*</span><span class="sxs-lookup"><span data-stu-id="229cc-253">/me/contacts/\*</span></span>](/graph/api/user-list-contacts) |
| <span data-ttu-id="229cc-254">`personDetails` set without image， `fetchImage` set to ， set to and person is not a contact or is set `true` `avatarType` `photo` `useContactApis` to `false`</span><span class="sxs-lookup"><span data-stu-id="229cc-254">`personDetails` set without image, `fetchImage` set to `true`, `avatarType` set to `photo` and person is not a contact or `useContactApis` is set to `false`</span></span> | <span data-ttu-id="229cc-255">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="229cc-255">User.ReadBasic.All</span></span> | [<span data-ttu-id="229cc-256">/users/{id}/photo/$value</span><span class="sxs-lookup"><span data-stu-id="229cc-256">/users/{id}/photo/$value</span></span>](/graph/api/profilephoto-get) |
| <span data-ttu-id="229cc-257">`personDetails` set without image， `fetchImage` set to ， set to and user specified via `true` `avatarType` `photo` email</span><span class="sxs-lookup"><span data-stu-id="229cc-257">`personDetails` set without image, `fetchImage` set to `true`, `avatarType` set to `photo` and user specified via email</span></span> | <span data-ttu-id="229cc-258">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="229cc-258">User.ReadBasic.All</span></span> | [<span data-ttu-id="229cc-259">/users/{id}/photo/$value</span><span class="sxs-lookup"><span data-stu-id="229cc-259">/users/{id}/photo/$value</span></span>](/graph/api/profilephoto-get) |
| <span data-ttu-id="229cc-260">`personDetails` set without image， `fetchImage` set to ， set to and contact specified via `true` `avatarType` `photo` email</span><span class="sxs-lookup"><span data-stu-id="229cc-260">`personDetails` set without image, `fetchImage` set to `true`, `avatarType` set to `photo` and contact specified via email</span></span> | <span data-ttu-id="229cc-261">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="229cc-261">Contacts.Read</span></span> | [<span data-ttu-id="229cc-262">/me/contacts/\*</span><span class="sxs-lookup"><span data-stu-id="229cc-262">/me/contacts/\*</span></span>](/graph/api/user-list-contacts) |
| <span data-ttu-id="229cc-263">`userId` set</span><span class="sxs-lookup"><span data-stu-id="229cc-263">`userId` set</span></span> | <span data-ttu-id="229cc-264">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="229cc-264">User.ReadBasic.All</span></span> | [<span data-ttu-id="229cc-265">/users/{id}</span><span class="sxs-lookup"><span data-stu-id="229cc-265">/users/{id}</span></span>](/graph/api/user-list-people) |
| <span data-ttu-id="229cc-266">`personQuery` 设置为 `me` ， `avatarType` 设置为 `photo`</span><span class="sxs-lookup"><span data-stu-id="229cc-266">`personQuery` set to `me` and `avatarType` set to `photo`</span></span> | <span data-ttu-id="229cc-267">User.Read</span><span class="sxs-lookup"><span data-stu-id="229cc-267">User.Read</span></span> | [<span data-ttu-id="229cc-268">/me/photo/$value</span><span class="sxs-lookup"><span data-stu-id="229cc-268">/me/photo/$value</span></span>](/graph/api/profilephoto-get) |
| <span data-ttu-id="229cc-269">`personQuery` 设置为 `me` ， `avatarType` 并设置为其他内容 `photo`</span><span class="sxs-lookup"><span data-stu-id="229cc-269">`personQuery` set to `me` and `avatarType` set to something else than `photo`</span></span> | <span data-ttu-id="229cc-270">User.Read</span><span class="sxs-lookup"><span data-stu-id="229cc-270">User.Read</span></span> | [<span data-ttu-id="229cc-271">/me</span><span class="sxs-lookup"><span data-stu-id="229cc-271">/me</span></span>](/graph/api/user-get) |
| <span data-ttu-id="229cc-272">`personQuery` 设置为值，而不是 `me` `useContactApis` 设置为 `true`</span><span class="sxs-lookup"><span data-stu-id="229cc-272">`personQuery` set to a value other than `me` and `useContactApis` set to `true`</span></span> | <span data-ttu-id="229cc-273">People.Read、User.ReadBasic.All、Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="229cc-273">People.Read, User.ReadBasic.All, Contacts.Read</span></span> | <span data-ttu-id="229cc-274">[/me/people/？$search=](/graph/api/user-list-people)、 [/users？$search=](/graph/api/user-list-people)、 [/me/contacts/ \* ](/graph/api/user-list-contacts)</span><span class="sxs-lookup"><span data-stu-id="229cc-274">[/me/people/?$search=](/graph/api/user-list-people), [/users?$search=](/graph/api/user-list-people), [/me/contacts/\*](/graph/api/user-list-contacts)</span></span> |
| <span data-ttu-id="229cc-275">`personQuery` 设置为值，而不是 `me` `useContactApis` 设置为 `false`</span><span class="sxs-lookup"><span data-stu-id="229cc-275">`personQuery` set to a value other than `me` and `useContactApis` set to `false`</span></span> | <span data-ttu-id="229cc-276">People.Read、User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="229cc-276">People.Read, User.ReadBasic.All</span></span> | <span data-ttu-id="229cc-277">[/me/people/？$search=](/graph/api/user-list-people)、 [/users？$search=](/graph/api/user-list-people)</span><span class="sxs-lookup"><span data-stu-id="229cc-277">[/me/people/?$search=](/graph/api/user-list-people), [/users?$search=](/graph/api/user-list-people)</span></span> |
| <span data-ttu-id="229cc-278">`showPresence` 设置为 `true` ， `personQuery` 设置为 `me`</span><span class="sxs-lookup"><span data-stu-id="229cc-278">`showPresence` set to `true` and `personQuery` set to `me`</span></span> | <span data-ttu-id="229cc-279">Presence.Read</span><span class="sxs-lookup"><span data-stu-id="229cc-279">Presence.Read</span></span> | [<span data-ttu-id="229cc-280">/me/presence</span><span class="sxs-lookup"><span data-stu-id="229cc-280">/me/presence</span></span>](/graph/api/presence-get) |
| <span data-ttu-id="229cc-281">`showPresence` 设置为 `true` 并 `personQuery` 设置为 `me`</span><span class="sxs-lookup"><span data-stu-id="229cc-281">`showPresence` set to `true` and `personQuery` set to a value other than `me`</span></span> | <span data-ttu-id="229cc-282">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="229cc-282">Presence.Read.All</span></span> | [<span data-ttu-id="229cc-283">/users/{id}/presence</span><span class="sxs-lookup"><span data-stu-id="229cc-283">/users/{id}/presence</span></span>](/graph/api/presence-get) |
| <span data-ttu-id="229cc-284">`personCardInteraction` 设置为除 `PersonCardInteraction.none`</span><span class="sxs-lookup"><span data-stu-id="229cc-284">`personCardInteraction` set to a value other than `PersonCardInteraction.none`</span></span> | <span data-ttu-id="229cc-285">查看 [个人卡片权限](/graph/toolkit/components/person-card#microsoft-graph-permissions)</span><span class="sxs-lookup"><span data-stu-id="229cc-285">See [person card permissions](/graph/toolkit/components/person-card#microsoft-graph-permissions)</span></span> | <span data-ttu-id="229cc-286">查看 [个人卡片 API 调用](/graph/toolkit/components/person-card#microsoft-graph-permissions)</span><span class="sxs-lookup"><span data-stu-id="229cc-286">See [person card API calls](/graph/toolkit/components/person-card#microsoft-graph-permissions)</span></span> |

## <a name="authentication"></a><span data-ttu-id="229cc-287">身份验证</span><span class="sxs-lookup"><span data-stu-id="229cc-287">Authentication</span></span>

<span data-ttu-id="229cc-288">该控件使用身份验证文档中介绍的全局身份验证提供程序[](../providers/providers.md)获取所需数据。</span><span class="sxs-lookup"><span data-stu-id="229cc-288">The control uses the global authentication provider described in the [authentication documentation](../providers/providers.md) to fetch the required data.</span></span>

## <a name="cache"></a><span data-ttu-id="229cc-289">缓存</span><span class="sxs-lookup"><span data-stu-id="229cc-289">Cache</span></span>

|<span data-ttu-id="229cc-290">对象存储</span><span class="sxs-lookup"><span data-stu-id="229cc-290">Object store</span></span>|<span data-ttu-id="229cc-291">缓存数据</span><span class="sxs-lookup"><span data-stu-id="229cc-291">Cached data</span></span>|<span data-ttu-id="229cc-292">备注</span><span class="sxs-lookup"><span data-stu-id="229cc-292">Remarks</span></span>|
|---------|-----------|-------|
|`photos`|<span data-ttu-id="229cc-293">人员照片</span><span class="sxs-lookup"><span data-stu-id="229cc-293">Person's photo</span></span>|<span data-ttu-id="229cc-294">使用 时 `avatarType` ，将 设置为 `photo` `fetchImage` ，将 设置为 `true`</span><span class="sxs-lookup"><span data-stu-id="229cc-294">Used, when `avatarType` is set to `photo` and `fetchImage` is set to `true`</span></span>|
|`presence`|<span data-ttu-id="229cc-295">人员状态</span><span class="sxs-lookup"><span data-stu-id="229cc-295">Person's presence</span></span>|<span data-ttu-id="229cc-296">已使用， `showPresence` 设置为 `true`</span><span class="sxs-lookup"><span data-stu-id="229cc-296">Used, when `showPresence` is set to `true`</span></span>|
|`users`|<span data-ttu-id="229cc-297">人员的用户信息</span><span class="sxs-lookup"><span data-stu-id="229cc-297">Person's user information</span></span>|

<span data-ttu-id="229cc-298">请参阅[Caching，](../customize-components/cache.md)了解有关如何配置缓存的更多详细信息。</span><span class="sxs-lookup"><span data-stu-id="229cc-298">See [Caching](../customize-components/cache.md) for more details on how to configure the cache.</span></span>

## <a name="extend-for-more-control"></a><span data-ttu-id="229cc-299">扩展以了解更多控件</span><span class="sxs-lookup"><span data-stu-id="229cc-299">Extend for more control</span></span>

<span data-ttu-id="229cc-300">对于更复杂的方案或真正自定义的 UX，此组件公开了多个在组件扩展 `protected render*` 中替代的方法。</span><span class="sxs-lookup"><span data-stu-id="229cc-300">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions.</span></span>

| <span data-ttu-id="229cc-301">方法</span><span class="sxs-lookup"><span data-stu-id="229cc-301">Method</span></span> | <span data-ttu-id="229cc-302">说明</span><span class="sxs-lookup"><span data-stu-id="229cc-302">Description</span></span> |
| - | - |
| <span data-ttu-id="229cc-303">renderLoading</span><span class="sxs-lookup"><span data-stu-id="229cc-303">renderLoading</span></span> | <span data-ttu-id="229cc-304">呈现加载状态。</span><span class="sxs-lookup"><span data-stu-id="229cc-304">Renders the loading state.</span></span> |
| <span data-ttu-id="229cc-305">renderNoData</span><span class="sxs-lookup"><span data-stu-id="229cc-305">renderNoData</span></span> | <span data-ttu-id="229cc-306">当图像或人员数据不可用时呈现。</span><span class="sxs-lookup"><span data-stu-id="229cc-306">Renders when no image or person data is available.</span></span> |
| <span data-ttu-id="229cc-307">renderAvatar</span><span class="sxs-lookup"><span data-stu-id="229cc-307">renderAvatar</span></span> | <span data-ttu-id="229cc-308">呈现头像。</span><span class="sxs-lookup"><span data-stu-id="229cc-308">Renders the avatar.</span></span> |
| <span data-ttu-id="229cc-309">renderDetails</span><span class="sxs-lookup"><span data-stu-id="229cc-309">renderDetails</span></span> | <span data-ttu-id="229cc-310">呈现人员详细信息部分。</span><span class="sxs-lookup"><span data-stu-id="229cc-310">Renders the person details part.</span></span> |
