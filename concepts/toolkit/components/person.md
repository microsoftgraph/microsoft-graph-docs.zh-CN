---
title: Microsoft 服务中的人员Graph Toolkit
description: 人员组件用于通过使用联系人的照片、姓名和/或电子邮件地址来显示此人或联系人。
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 46ba7c780985e71d68fe9270f165292136f2e46b
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579947"
---
# <a name="person-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="3cd40-103">Microsoft 服务中的人员Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="3cd40-103">Person component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="3cd40-104">人员组件用于通过使用其照片、姓名、电子邮件地址或其他任何人员详细信息来显示此人或联系人。</span><span class="sxs-lookup"><span data-stu-id="3cd40-104">The person component is used to display a person or contact by using their photo, name, email address, or any other person details.</span></span>

<span data-ttu-id="3cd40-105">人员组件还使用 [mgt-person-card](./person-card.md) 显示包含有关用户的其他信息的飞出卡。</span><span class="sxs-lookup"><span data-stu-id="3cd40-105">The person component also uses the [mgt-person-card](./person-card.md) to display a flyout card with additional information about the user.</span></span> <span data-ttu-id="3cd40-106">有关详细信息，请参阅人员 [卡片](#person-card) 部分。</span><span class="sxs-lookup"><span data-stu-id="3cd40-106">For details, see the [Person Card](#person-card) section.</span></span>

## <a name="example"></a><span data-ttu-id="3cd40-107">示例</span><span class="sxs-lookup"><span data-stu-id="3cd40-107">Example</span></span>

<span data-ttu-id="3cd40-108">以下示例显示使用该组件 `mgt-person` 的人。</span><span class="sxs-lookup"><span data-stu-id="3cd40-108">The following example displays a person using the `mgt-person` component.</span></span> <span data-ttu-id="3cd40-109">可以使用代码编辑器查看 [属性如何](#properties) 更改组件的行为。</span><span class="sxs-lookup"><span data-stu-id="3cd40-109">You can use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-person--person&source=docs" height="250"></iframe>

[<span data-ttu-id="3cd40-110">在"打开"mgt.dev</span><span class="sxs-lookup"><span data-stu-id="3cd40-110">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-person--person&source=docs)

## <a name="setting-the-person-details"></a><span data-ttu-id="3cd40-111">设置人员详细信息</span><span class="sxs-lookup"><span data-stu-id="3cd40-111">Setting the person details</span></span>

<span data-ttu-id="3cd40-112">可以使用三个属性来设置人员详细信息。</span><span class="sxs-lookup"><span data-stu-id="3cd40-112">You can use three properties to set the person details.</span></span> <span data-ttu-id="3cd40-113">每个实例仅使用以下属性之一：</span><span class="sxs-lookup"><span data-stu-id="3cd40-113">Use only one of the following properties per instance:</span></span>

* <span data-ttu-id="3cd40-114">设置 `user-id` 属性或 `userId` 属性以通过使用用户的 ID 从 Microsoft Graph获取用户。</span><span class="sxs-lookup"><span data-stu-id="3cd40-114">Set the `user-id` attribute or `userId` property to fetch the user from Microsoft Graph by using their ID.</span></span>

* <span data-ttu-id="3cd40-115">设置 `person-query` 属性或 `personQuery` 属性以搜索 Microsoft Graph给定人员。</span><span class="sxs-lookup"><span data-stu-id="3cd40-115">Set the `person-query` attribute or `personQuery` property to search Microsoft Graph for a given person.</span></span> <span data-ttu-id="3cd40-116">它将选择第一个可用的人员并提取该人员的详细信息。</span><span class="sxs-lookup"><span data-stu-id="3cd40-116">It will choose the first person available and fetch the person details.</span></span> <span data-ttu-id="3cd40-117">电子邮件最适用于确保查询正确的人员，但名称也有效。</span><span class="sxs-lookup"><span data-stu-id="3cd40-117">An email works best to ensure the right person is queried, but a name works as well.</span></span>

* <span data-ttu-id="3cd40-118">设置 `person-presence` 属性或 `personPresence` 属性以手动向个人头像添加状态锁屏提醒。</span><span class="sxs-lookup"><span data-stu-id="3cd40-118">Set the `person-presence` attribute or `personPresence` property to add a presence badge to person avatar manually.</span></span>

* <span data-ttu-id="3cd40-119">将 `avatar-size` 属性或 `avatarSize` 属性设置为 `small` 或 `large` 确定头像的大小。</span><span class="sxs-lookup"><span data-stu-id="3cd40-119">Set the `avatar-size` attribute or `avatarSize` property to `small` or `large` to determine the size of avatar.</span></span> <span data-ttu-id="3cd40-120">这有助于向头像 [添加正确的状态](https://mgt.dev/?path=/story/components-mgt-person--person-presence-display-all) 锁屏提醒。</span><span class="sxs-lookup"><span data-stu-id="3cd40-120">This helps add the [correct presence badge](https://mgt.dev/?path=/story/components-mgt-person--person-presence-display-all) to avatar.</span></span> <span data-ttu-id="3cd40-121">你将需要选择正确的相应的 css 自定义属性，如下所示以进一步自定义头像大小。</span><span class="sxs-lookup"><span data-stu-id="3cd40-121">You will need to choose the correct corresponding css custom properties shown below to further customize avatar size.</span></span> <span data-ttu-id="3cd40-122">默认情况下，值设置为 ，该值将自动根据 属性 `auto` 决定如何呈现 `view` 状态。</span><span class="sxs-lookup"><span data-stu-id="3cd40-122">By default, the value is set to `auto` which will automatically decide how to render the presence based on the `view` property.</span></span> <span data-ttu-id="3cd40-123">如果你的头 `small` 像小于 32px x 32px，我们建议使用 。</span><span class="sxs-lookup"><span data-stu-id="3cd40-123">We recommend using `small` if your avatar is smaller than 32px by 32px.</span></span> 

* <span data-ttu-id="3cd40-124">使用 `person-details` 属性 `personDetails` 或 属性手动设置人员详细信息，如以下示例所示。</span><span class="sxs-lookup"><span data-stu-id="3cd40-124">Use the `person-details` attribute or `personDetails` property to manually set the person details, as shown in the following example.</span></span>


    ```js
    let personControl = document.getElementById('myPersonControl');
    personControl.personDetails = {
        displayName: 'Nikola Metulev',
        mail: 'nikola@contoso.com',
        personImage: 'url'
    }
    ```

  <span data-ttu-id="3cd40-125">如果未提供图像，将提取一个 (（如果) ）。</span><span class="sxs-lookup"><span data-stu-id="3cd40-125">If no image is provided, one will be fetched (if available).</span></span>

* <span data-ttu-id="3cd40-126">默认情况下，人员组件将仅请求标准 Microsoft Graph属性[集。](/graph/api/user-get?&tabs=http#optional-query-parameters)</span><span class="sxs-lookup"><span data-stu-id="3cd40-126">By default, the person component will only request the standard Microsoft Graph user set of [properties](/graph/api/user-get?&tabs=http#optional-query-parameters).</span></span> <span data-ttu-id="3cd40-127">为了请求其他属性，请将其声明为 的任何部分 `line(x)Property` 。</span><span class="sxs-lookup"><span data-stu-id="3cd40-127">In order to request additional properties, declare them as any part of the `line(x)Property`.</span></span> 


## <a name="properties"></a><span data-ttu-id="3cd40-128">属性</span><span class="sxs-lookup"><span data-stu-id="3cd40-128">Properties</span></span>

<span data-ttu-id="3cd40-129">可以使用多个属性来自定义组件。</span><span class="sxs-lookup"><span data-stu-id="3cd40-129">You can use several properties to customize the component.</span></span>

| <span data-ttu-id="3cd40-130">属性</span><span class="sxs-lookup"><span data-stu-id="3cd40-130">Attribute</span></span>       | <span data-ttu-id="3cd40-131">属性</span><span class="sxs-lookup"><span data-stu-id="3cd40-131">Property</span></span>       | <span data-ttu-id="3cd40-132">说明</span><span class="sxs-lookup"><span data-stu-id="3cd40-132">Description</span></span>                                                   |
| -----------     | ----------     | ------------------------------------------------------------- |
| <span data-ttu-id="3cd40-133">user-id</span><span class="sxs-lookup"><span data-stu-id="3cd40-133">user-id</span></span>         | <span data-ttu-id="3cd40-134">userId</span><span class="sxs-lookup"><span data-stu-id="3cd40-134">userId</span></span>         | <span data-ttu-id="3cd40-135">设置为用户 ID 以从 Microsoft Graph 获取该用户的详细信息和Graph。</span><span class="sxs-lookup"><span data-stu-id="3cd40-135">Set to a user id to fetch that user's details and image from Microsoft Graph.</span></span>|
| <span data-ttu-id="3cd40-136">person-query</span><span class="sxs-lookup"><span data-stu-id="3cd40-136">person-query</span></span>    | <span data-ttu-id="3cd40-137">personQuery</span><span class="sxs-lookup"><span data-stu-id="3cd40-137">personQuery</span></span>    | <span data-ttu-id="3cd40-138">设置为某人的姓名或电子邮件，以在 Microsoft Graph并提取第一个人的详细信息和图像。</span><span class="sxs-lookup"><span data-stu-id="3cd40-138">Set to a name or email of a person to search for a person in Microsoft Graph and fetch the first person's details and image.</span></span>|
| <span data-ttu-id="3cd40-139">person-details</span><span class="sxs-lookup"><span data-stu-id="3cd40-139">person-details</span></span>  | <span data-ttu-id="3cd40-140">personDetails</span><span class="sxs-lookup"><span data-stu-id="3cd40-140">personDetails</span></span>  | <span data-ttu-id="3cd40-141">设置为表示人员的对象。</span><span class="sxs-lookup"><span data-stu-id="3cd40-141">Set to an object representing a person.</span></span> <span data-ttu-id="3cd40-142">使用来自人员、用户、联系人或组、资源的对象。</span><span class="sxs-lookup"><span data-stu-id="3cd40-142">Works with object from the people, users, contacts, or group, resources.</span></span> |
| <span data-ttu-id="3cd40-143">fallback-details</span><span class="sxs-lookup"><span data-stu-id="3cd40-143">fallback-details</span></span>| <span data-ttu-id="3cd40-144">fallbackDetails</span><span class="sxs-lookup"><span data-stu-id="3cd40-144">fallbackDetails</span></span>| <span data-ttu-id="3cd40-145">设置为一个对象，该对象表示在图形中找不到用户/人员/联系人时的用户。</span><span class="sxs-lookup"><span data-stu-id="3cd40-145">Set to an object representing a person when no user/person/contact is found in the graph.</span></span>
| <span data-ttu-id="3cd40-146">person-image</span><span class="sxs-lookup"><span data-stu-id="3cd40-146">person-image</span></span>    | <span data-ttu-id="3cd40-147">personImage</span><span class="sxs-lookup"><span data-stu-id="3cd40-147">personImage</span></span>    | <span data-ttu-id="3cd40-148">设置要向人员显示的图像。</span><span class="sxs-lookup"><span data-stu-id="3cd40-148">Set the image to show for the person.</span></span> |
| <span data-ttu-id="3cd40-149">person-presence</span><span class="sxs-lookup"><span data-stu-id="3cd40-149">person-presence</span></span> | <span data-ttu-id="3cd40-150">personPresence</span><span class="sxs-lookup"><span data-stu-id="3cd40-150">personPresence</span></span> | <span data-ttu-id="3cd40-151">为人员设置状态。</span><span class="sxs-lookup"><span data-stu-id="3cd40-151">Set the presence for the person.</span></span> |
| <span data-ttu-id="3cd40-152">fetch-image</span><span class="sxs-lookup"><span data-stu-id="3cd40-152">fetch-image</span></span>     | <span data-ttu-id="3cd40-153">fetchImage</span><span class="sxs-lookup"><span data-stu-id="3cd40-153">fetchImage</span></span>     | <span data-ttu-id="3cd40-154">将标志设置为根据Graph自动从 Microsoft 网站 `personImage` `personDetails` 提取。</span><span class="sxs-lookup"><span data-stu-id="3cd40-154">Set flag to fetch `personImage` automatically from Microsoft Graph based on the `personDetails` object provided by the user.</span></span> |
| <span data-ttu-id="3cd40-155">头像类型</span><span class="sxs-lookup"><span data-stu-id="3cd40-155">avatar-type</span></span>     | <span data-ttu-id="3cd40-156">头像类型</span><span class="sxs-lookup"><span data-stu-id="3cd40-156">avatarType</span></span>     | <span data-ttu-id="3cd40-157">设置为 或 `initials` `photo` 呈现任一显示状态 - 默认为照片。</span><span class="sxs-lookup"><span data-stu-id="3cd40-157">Set to `initials` or `photo` to render either display state - default is photo.</span></span> |
| <span data-ttu-id="3cd40-158">view</span><span class="sxs-lookup"><span data-stu-id="3cd40-158">view</span></span>            | <span data-ttu-id="3cd40-159">view</span><span class="sxs-lookup"><span data-stu-id="3cd40-159">view</span></span>           | <span data-ttu-id="3cd40-160">设置为控制呈现人员的方式。</span><span class="sxs-lookup"><span data-stu-id="3cd40-160">Set to control how the person is rendered.</span></span> <span data-ttu-id="3cd40-161">默认值为 `avatar`</span><span class="sxs-lookup"><span data-stu-id="3cd40-161">Default is `avatar`</span></span> <br /> <span data-ttu-id="3cd40-162">`avatar` - 仅显示头像</span><span class="sxs-lookup"><span data-stu-id="3cd40-162">`avatar` - show only avatar</span></span> <br /> <span data-ttu-id="3cd40-163">`oneline` - 默认显示头像 (`displayName` 第一) </span><span class="sxs-lookup"><span data-stu-id="3cd40-163">`oneline` - show avatar and first line (`displayName` by default)</span></span> <br /> <span data-ttu-id="3cd40-164">`twolines` - 显示头像和两行文本 (`displayName` `mail` 默认显示) </span><span class="sxs-lookup"><span data-stu-id="3cd40-164">`twolines` - show avatar and two lines of text (`displayName` and `mail` by default)</span></span>|
| <span data-ttu-id="3cd40-165">line1-property</span><span class="sxs-lookup"><span data-stu-id="3cd40-165">line1-property</span></span>  | <span data-ttu-id="3cd40-166">line1Property</span><span class="sxs-lookup"><span data-stu-id="3cd40-166">line1Property</span></span>  | <span data-ttu-id="3cd40-167">设置要用于第一行文本的 personDetails 的属性。</span><span class="sxs-lookup"><span data-stu-id="3cd40-167">Sets the property of the personDetails to use for the first line of text.</span></span> <span data-ttu-id="3cd40-168">默认值为“`displayName`”。</span><span class="sxs-lookup"><span data-stu-id="3cd40-168">Default is `displayName`.</span></span>|
| <span data-ttu-id="3cd40-169">line2-property</span><span class="sxs-lookup"><span data-stu-id="3cd40-169">line2-property</span></span>  | <span data-ttu-id="3cd40-170">line2Property</span><span class="sxs-lookup"><span data-stu-id="3cd40-170">line2Property</span></span>  | <span data-ttu-id="3cd40-171">设置要用于第二行文本的 personDetails 的属性。</span><span class="sxs-lookup"><span data-stu-id="3cd40-171">Sets the property of the personDetails to use for the second line of text.</span></span> <span data-ttu-id="3cd40-172">默认值为“`mail`”。</span><span class="sxs-lookup"><span data-stu-id="3cd40-172">Default is `mail`.</span></span>|
| <span data-ttu-id="3cd40-173">line3-property</span><span class="sxs-lookup"><span data-stu-id="3cd40-173">line3-property</span></span>  | <span data-ttu-id="3cd40-174">line3Property</span><span class="sxs-lookup"><span data-stu-id="3cd40-174">line3Property</span></span>  | <span data-ttu-id="3cd40-175">设置要用于第三行文本的 personDetails 的属性。</span><span class="sxs-lookup"><span data-stu-id="3cd40-175">Sets the property of the personDetails to use for the third line of text.</span></span> <span data-ttu-id="3cd40-176">默认值为“`jobTitle`”。</span><span class="sxs-lookup"><span data-stu-id="3cd40-176">Default is `jobTitle`.</span></span>|
| <span data-ttu-id="3cd40-177">show-presence</span><span class="sxs-lookup"><span data-stu-id="3cd40-177">show-presence</span></span>   | <span data-ttu-id="3cd40-178">showPresence</span><span class="sxs-lookup"><span data-stu-id="3cd40-178">showPresence</span></span>   | <span data-ttu-id="3cd40-179">设置用于显示人员状态的标志 - 默认为 `false` 。</span><span class="sxs-lookup"><span data-stu-id="3cd40-179">Set flag to display person presence - default is `false`.</span></span>|

## <a name="css-custom-properties"></a><span data-ttu-id="3cd40-180">CSS 自定义属性</span><span class="sxs-lookup"><span data-stu-id="3cd40-180">CSS custom properties</span></span>

<span data-ttu-id="3cd40-181">组件 `mgt-person` 定义以下 CSS 自定义属性。</span><span class="sxs-lookup"><span data-stu-id="3cd40-181">The `mgt-person` component defines the following CSS custom properties.</span></span>

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

<span data-ttu-id="3cd40-182">若要了解更多信息，请参阅 [设置组件样式](../customize-components/style.md)。</span><span class="sxs-lookup"><span data-stu-id="3cd40-182">To learn more, see [styling components](../customize-components/style.md).</span></span>

## <a name="events"></a><span data-ttu-id="3cd40-183">活动</span><span class="sxs-lookup"><span data-stu-id="3cd40-183">Events</span></span>

<span data-ttu-id="3cd40-184">从组件中触发以下事件。</span><span class="sxs-lookup"><span data-stu-id="3cd40-184">The following events are fired from the component.</span></span>

| <span data-ttu-id="3cd40-185">事件</span><span class="sxs-lookup"><span data-stu-id="3cd40-185">Event</span></span> | <span data-ttu-id="3cd40-186">详情</span><span class="sxs-lookup"><span data-stu-id="3cd40-186">Detail</span></span> | <span data-ttu-id="3cd40-187">说明</span><span class="sxs-lookup"><span data-stu-id="3cd40-187">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="3cd40-188">line1clicked</span><span class="sxs-lookup"><span data-stu-id="3cd40-188">line1clicked</span></span> | <span data-ttu-id="3cd40-189">详细信息包含各自的 `person` 对象</span><span class="sxs-lookup"><span data-stu-id="3cd40-189">The detail contains the respective `person` object</span></span> | <span data-ttu-id="3cd40-190">在单击第 1 行时触发。</span><span class="sxs-lookup"><span data-stu-id="3cd40-190">Fired when line1 is clicked.</span></span> |
| <span data-ttu-id="3cd40-191">line2clicked</span><span class="sxs-lookup"><span data-stu-id="3cd40-191">line2clicked</span></span> | <span data-ttu-id="3cd40-192">详细信息包含各自的 `person` 对象</span><span class="sxs-lookup"><span data-stu-id="3cd40-192">The detail contains the respective `person` object</span></span> | <span data-ttu-id="3cd40-193">在单击第 2 行时触发。</span><span class="sxs-lookup"><span data-stu-id="3cd40-193">Fired when line2 is clicked.</span></span> |
| <span data-ttu-id="3cd40-194">line3clicked</span><span class="sxs-lookup"><span data-stu-id="3cd40-194">line3clicked</span></span> | <span data-ttu-id="3cd40-195">详细信息包含各自的 `person` 对象</span><span class="sxs-lookup"><span data-stu-id="3cd40-195">The detail contains the respective `person` object</span></span> | <span data-ttu-id="3cd40-196">在单击第 3 行时触发。</span><span class="sxs-lookup"><span data-stu-id="3cd40-196">Fired when line3 is clicked.</span></span> |

## <a name="templates"></a><span data-ttu-id="3cd40-197">模板</span><span class="sxs-lookup"><span data-stu-id="3cd40-197">Templates</span></span>

<span data-ttu-id="3cd40-198">组件 `mgt-person` 支持 [多个模板](../customize-components/templates.md) ，允许您替换组件的某些部分。</span><span class="sxs-lookup"><span data-stu-id="3cd40-198">The `mgt-person` component supports several [templates](../customize-components/templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="3cd40-199">若要指定模板，请包含组件 `<template>` 中的元素，将值 `data-type` 设置为下列值之一：</span><span class="sxs-lookup"><span data-stu-id="3cd40-199">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following:</span></span>

| <span data-ttu-id="3cd40-200">数据类型</span><span class="sxs-lookup"><span data-stu-id="3cd40-200">Data type</span></span> | <span data-ttu-id="3cd40-201">数据上下文</span><span class="sxs-lookup"><span data-stu-id="3cd40-201">Data context</span></span> | <span data-ttu-id="3cd40-202">说明</span><span class="sxs-lookup"><span data-stu-id="3cd40-202">Description</span></span> |
| --------- | ------------ | ----------- |
| <span data-ttu-id="3cd40-203">loading</span><span class="sxs-lookup"><span data-stu-id="3cd40-203">loading</span></span> | <span data-ttu-id="3cd40-204">无</span><span class="sxs-lookup"><span data-stu-id="3cd40-204">none</span></span> | <span data-ttu-id="3cd40-205">组件在加载状态时要呈现的模板。</span><span class="sxs-lookup"><span data-stu-id="3cd40-205">The template to render while the component is in a loading state.</span></span> |
| <span data-ttu-id="3cd40-206">no-data</span><span class="sxs-lookup"><span data-stu-id="3cd40-206">no-data</span></span> | <span data-ttu-id="3cd40-207">无</span><span class="sxs-lookup"><span data-stu-id="3cd40-207">none</span></span> | <span data-ttu-id="3cd40-208">在没有任何人员图像或数据可用时要呈现的模板。</span><span class="sxs-lookup"><span data-stu-id="3cd40-208">The template to render when no person image or data is available.</span></span> | 
| <span data-ttu-id="3cd40-209">default</span><span class="sxs-lookup"><span data-stu-id="3cd40-209">default</span></span> | <span data-ttu-id="3cd40-210">person： The person details object</span><span class="sxs-lookup"><span data-stu-id="3cd40-210">person: The person details object</span></span> <br> <span data-ttu-id="3cd40-211">`personImage`：图像的 URL</span><span class="sxs-lookup"><span data-stu-id="3cd40-211">`personImage`: The URL of the image</span></span> <br> <span data-ttu-id="3cd40-212">`personPresence`：人员状态详细信息对象</span><span class="sxs-lookup"><span data-stu-id="3cd40-212">`personPresence`: The presence details object for person</span></span>  | <span data-ttu-id="3cd40-213">默认模板将整个组件替换为你自己的组件。</span><span class="sxs-lookup"><span data-stu-id="3cd40-213">The default template replaces the entire component with your own.</span></span> |
| <span data-ttu-id="3cd40-214">person-card</span><span class="sxs-lookup"><span data-stu-id="3cd40-214">person-card</span></span> | <span data-ttu-id="3cd40-215">person： The person details object</span><span class="sxs-lookup"><span data-stu-id="3cd40-215">person: The person details object</span></span> <br> <span data-ttu-id="3cd40-216">`personImage`：图像的 URL</span><span class="sxs-lookup"><span data-stu-id="3cd40-216">`personImage`: The URL of the image</span></span> | <span data-ttu-id="3cd40-217">用于更新悬停或单击时显示的 mgt-person-card 的模板。</span><span class="sxs-lookup"><span data-stu-id="3cd40-217">The template to update the mgt-person-card displayed on hover or click.</span></span> |
| <span data-ttu-id="3cd40-218">line1</span><span class="sxs-lookup"><span data-stu-id="3cd40-218">line1</span></span> | <span data-ttu-id="3cd40-219">person： The person details object</span><span class="sxs-lookup"><span data-stu-id="3cd40-219">person: The person details object</span></span> | <span data-ttu-id="3cd40-220">第一行人员元数据的模板。</span><span class="sxs-lookup"><span data-stu-id="3cd40-220">The template for the first line of person metadata.</span></span> |
| <span data-ttu-id="3cd40-221">line2</span><span class="sxs-lookup"><span data-stu-id="3cd40-221">line2</span></span> | <span data-ttu-id="3cd40-222">person： The person details object</span><span class="sxs-lookup"><span data-stu-id="3cd40-222">person: The person details object</span></span> | <span data-ttu-id="3cd40-223">第二行人员元数据的模板。</span><span class="sxs-lookup"><span data-stu-id="3cd40-223">The template for the second line of person metadata.</span></span> |
| <span data-ttu-id="3cd40-224">line3</span><span class="sxs-lookup"><span data-stu-id="3cd40-224">line3</span></span> | <span data-ttu-id="3cd40-225">person： The person details object</span><span class="sxs-lookup"><span data-stu-id="3cd40-225">person: The person details object</span></span> | <span data-ttu-id="3cd40-226">第三行人员元数据的模板。</span><span class="sxs-lookup"><span data-stu-id="3cd40-226">The template for the third line of person metadata.</span></span> |

<span data-ttu-id="3cd40-227">下面的示例定义人员组件的模板。</span><span class="sxs-lookup"><span data-stu-id="3cd40-227">The following example defines a template for the person component.</span></span>

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

## <a name="person-card"></a><span data-ttu-id="3cd40-228">个人卡片</span><span class="sxs-lookup"><span data-stu-id="3cd40-228">Person card</span></span>

<span data-ttu-id="3cd40-229">组件 `mgt-person` 可以在悬停 `mgt-person-card` 或单击时显示 。</span><span class="sxs-lookup"><span data-stu-id="3cd40-229">The `mgt-person` component can show an `mgt-person-card` on either hover or click.</span></span>

### <a name="add-the-control-to-the-html-page"></a><span data-ttu-id="3cd40-230">将控件添加到 HTML 页面</span><span class="sxs-lookup"><span data-stu-id="3cd40-230">Add the control to the HTML page</span></span>
```html
<mgt-person person-query="me" person-card="hover"></mgt-person>
```

| <span data-ttu-id="3cd40-231">属性</span><span class="sxs-lookup"><span data-stu-id="3cd40-231">Attribute</span></span>    |  <span data-ttu-id="3cd40-232">属性</span><span class="sxs-lookup"><span data-stu-id="3cd40-232">Property</span></span>     | <span data-ttu-id="3cd40-233">说明</span><span class="sxs-lookup"><span data-stu-id="3cd40-233">Description</span></span>                                                                     |
| ------------ | ------------- | ------------------------------------------------------------------------------- |
| <span data-ttu-id="3cd40-234">person-card</span><span class="sxs-lookup"><span data-stu-id="3cd40-234">person-card</span></span> | <span data-ttu-id="3cd40-235">personCardInteraction</span><span class="sxs-lookup"><span data-stu-id="3cd40-235">personCardInteraction</span></span> | <span data-ttu-id="3cd40-236">一个枚举，用于确定激活飞出面板或 所需的用户 `hover` 操作 `click` 。</span><span class="sxs-lookup"><span data-stu-id="3cd40-236">An enumeration to determine user action necessary to activate flyout panel - `hover` or `click`.</span></span> <span data-ttu-id="3cd40-237">默认值为 `none`</span><span class="sxs-lookup"><span data-stu-id="3cd40-237">Default value is `none`</span></span> |


<span data-ttu-id="3cd40-238">有关模板、样式设置和属性详细信息，请参阅 Person Card [component](./person-card.md)。</span><span class="sxs-lookup"><span data-stu-id="3cd40-238">For more information about templating, styling, and attributes, see [Person Card component](./person-card.md).</span></span>

## <a name="global-component-configuration"></a><span data-ttu-id="3cd40-239">全局组件配置</span><span class="sxs-lookup"><span data-stu-id="3cd40-239">Global component configuration</span></span>

<span data-ttu-id="3cd40-240">类 `MgtPerson` 公开一个 `config` 静态对象，该对象配置应用程序中的每个人组件。</span><span class="sxs-lookup"><span data-stu-id="3cd40-240">The `MgtPerson` class exposes a static `config` object that configures all person components in the application.</span></span>

<span data-ttu-id="3cd40-241">以下示例演示如何使用 config 对象。</span><span class="sxs-lookup"><span data-stu-id="3cd40-241">The following example shows how to use the config object.</span></span>

```ts
import { MgtPerson } from `@microsoft/mgt`;

MgtPerson.config.useContactApis = false;
```

<span data-ttu-id="3cd40-242">以下属性在 config 对象上可用。</span><span class="sxs-lookup"><span data-stu-id="3cd40-242">The following properties are available on the config object.</span></span>

| <span data-ttu-id="3cd40-243">属性</span><span class="sxs-lookup"><span data-stu-id="3cd40-243">Property</span></span> | <span data-ttu-id="3cd40-244">说明</span><span class="sxs-lookup"><span data-stu-id="3cd40-244">Description</span></span> |
| ------------ | ------------- |
| <span data-ttu-id="3cd40-245">useContactApis</span><span class="sxs-lookup"><span data-stu-id="3cd40-245">useContactApis</span></span> | <span data-ttu-id="3cd40-246">`boolean`- 指示人员组件是否可以使用 Microsoft Graph联系人 API 搜索联系人详细信息和照片。</span><span class="sxs-lookup"><span data-stu-id="3cd40-246">`boolean` - Indicates whether the person component can use the Microsoft Graph personal contacts API to search for contact details and photos.</span></span> <span data-ttu-id="3cd40-247">默认值为 `true`。</span><span class="sxs-lookup"><span data-stu-id="3cd40-247">Default value is `true`.</span></span>  |

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="3cd40-248">Microsoft Graph 权限</span><span class="sxs-lookup"><span data-stu-id="3cd40-248">Microsoft Graph permissions</span></span>

<span data-ttu-id="3cd40-249">此控件使用下列 Microsoft Graph API 和权限。</span><span class="sxs-lookup"><span data-stu-id="3cd40-249">This control uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="3cd40-250">资源</span><span class="sxs-lookup"><span data-stu-id="3cd40-250">Resource</span></span> | <span data-ttu-id="3cd40-251">权限</span><span class="sxs-lookup"><span data-stu-id="3cd40-251">Permission</span></span>     |
| -| - |
| [<span data-ttu-id="3cd40-252">/me</span><span class="sxs-lookup"><span data-stu-id="3cd40-252">/me</span></span>](/graph/api/user-get)                              | <span data-ttu-id="3cd40-253">User.Read</span><span class="sxs-lookup"><span data-stu-id="3cd40-253">User.Read</span></span>          |
| [<span data-ttu-id="3cd40-254">/me/photo/$value</span><span class="sxs-lookup"><span data-stu-id="3cd40-254">/me/photo/$value</span></span>](/graph/api/profilephoto-get)        | <span data-ttu-id="3cd40-255">User.Read</span><span class="sxs-lookup"><span data-stu-id="3cd40-255">User.Read</span></span>          |
| [<span data-ttu-id="3cd40-256">/me/people/？$search=</span><span class="sxs-lookup"><span data-stu-id="3cd40-256">/me/people/?$search=</span></span>](/graph/api/user-list-people)     | <span data-ttu-id="3cd40-257">People.Read</span><span class="sxs-lookup"><span data-stu-id="3cd40-257">People.Read</span></span>        |
| [<span data-ttu-id="3cd40-258">/me/contacts/\*</span><span class="sxs-lookup"><span data-stu-id="3cd40-258">/me/contacts/\*</span></span>](/graph/api/user-list-contacts&tabs=cs) | <span data-ttu-id="3cd40-259">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="3cd40-259">Contacts.Read</span></span>      |
| [<span data-ttu-id="3cd40-260">/users/{id}/photo/$value</span><span class="sxs-lookup"><span data-stu-id="3cd40-260">/users/{id}/photo/$value</span></span>](/graph/api/user-list-people) | <span data-ttu-id="3cd40-261">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="3cd40-261">User.ReadBasic.All</span></span> |
| [<span data-ttu-id="3cd40-262">/me/presence</span><span class="sxs-lookup"><span data-stu-id="3cd40-262">/me/presence</span></span>](/graph/api/presence-get)                | <span data-ttu-id="3cd40-263">Presence.Read</span><span class="sxs-lookup"><span data-stu-id="3cd40-263">Presence.Read</span></span> |
| [<span data-ttu-id="3cd40-264">/users/{id}/presence</span><span class="sxs-lookup"><span data-stu-id="3cd40-264">/users/{id}/presence</span></span>](/graph/api/presence-get)        | <span data-ttu-id="3cd40-265">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="3cd40-265">Presence.Read.All</span></span> |

## <a name="authentication"></a><span data-ttu-id="3cd40-266">身份验证</span><span class="sxs-lookup"><span data-stu-id="3cd40-266">Authentication</span></span>

<span data-ttu-id="3cd40-267">该控件使用身份验证文档中介绍的全局身份验证提供程序[](../providers/providers.md)获取所需数据。</span><span class="sxs-lookup"><span data-stu-id="3cd40-267">The control uses the global authentication provider described in the [authentication documentation](../providers/providers.md) to fetch the required data.</span></span>

## <a name="cache"></a><span data-ttu-id="3cd40-268">缓存</span><span class="sxs-lookup"><span data-stu-id="3cd40-268">Cache</span></span>

|<span data-ttu-id="3cd40-269">对象存储</span><span class="sxs-lookup"><span data-stu-id="3cd40-269">Object store</span></span>|<span data-ttu-id="3cd40-270">缓存数据</span><span class="sxs-lookup"><span data-stu-id="3cd40-270">Cached data</span></span>|<span data-ttu-id="3cd40-271">备注</span><span class="sxs-lookup"><span data-stu-id="3cd40-271">Remarks</span></span>|
|---------|-----------|-------|
|`photos`|<span data-ttu-id="3cd40-272">人员照片</span><span class="sxs-lookup"><span data-stu-id="3cd40-272">Person's photo</span></span>|<span data-ttu-id="3cd40-273">使用 时 `avatarType` ，将 设置为 `photo` `fetchImage` ，将 设置为 `true`</span><span class="sxs-lookup"><span data-stu-id="3cd40-273">Used, when `avatarType` is set to `photo` and `fetchImage` is set to `true`</span></span>|
|`presence`|<span data-ttu-id="3cd40-274">人员状态</span><span class="sxs-lookup"><span data-stu-id="3cd40-274">Person's presence</span></span>|<span data-ttu-id="3cd40-275">已使用， `showPresence` 设置为 `true`</span><span class="sxs-lookup"><span data-stu-id="3cd40-275">Used, when `showPresence` is set to `true`</span></span>|
|`users`|<span data-ttu-id="3cd40-276">人员的用户信息</span><span class="sxs-lookup"><span data-stu-id="3cd40-276">Person's user information</span></span>|

<span data-ttu-id="3cd40-277">请参阅[Caching，](../customize-components/cache.md)了解有关如何配置缓存的更多详细信息。</span><span class="sxs-lookup"><span data-stu-id="3cd40-277">See [Caching](../customize-components/cache.md) for more details on how to configure the cache.</span></span>

## <a name="extend-for-more-control"></a><span data-ttu-id="3cd40-278">扩展以了解更多控件</span><span class="sxs-lookup"><span data-stu-id="3cd40-278">Extend for more control</span></span>

<span data-ttu-id="3cd40-279">对于更复杂的方案或真正自定义的 UX，此组件公开了多个在组件扩展 `protected render*` 中替代的方法。</span><span class="sxs-lookup"><span data-stu-id="3cd40-279">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions.</span></span>

| <span data-ttu-id="3cd40-280">方法</span><span class="sxs-lookup"><span data-stu-id="3cd40-280">Method</span></span> | <span data-ttu-id="3cd40-281">说明</span><span class="sxs-lookup"><span data-stu-id="3cd40-281">Description</span></span> |
| - | - |
| <span data-ttu-id="3cd40-282">renderLoading</span><span class="sxs-lookup"><span data-stu-id="3cd40-282">renderLoading</span></span> | <span data-ttu-id="3cd40-283">呈现加载状态。</span><span class="sxs-lookup"><span data-stu-id="3cd40-283">Renders the loading state.</span></span> |
| <span data-ttu-id="3cd40-284">renderNoData</span><span class="sxs-lookup"><span data-stu-id="3cd40-284">renderNoData</span></span> | <span data-ttu-id="3cd40-285">当图像或人员数据不可用时呈现。</span><span class="sxs-lookup"><span data-stu-id="3cd40-285">Renders when no image or person data is available.</span></span> |
| <span data-ttu-id="3cd40-286">renderAvatar</span><span class="sxs-lookup"><span data-stu-id="3cd40-286">renderAvatar</span></span> | <span data-ttu-id="3cd40-287">呈现头像。</span><span class="sxs-lookup"><span data-stu-id="3cd40-287">Renders the avatar.</span></span> |
| <span data-ttu-id="3cd40-288">renderDetails</span><span class="sxs-lookup"><span data-stu-id="3cd40-288">renderDetails</span></span> | <span data-ttu-id="3cd40-289">呈现人员详细信息部分。</span><span class="sxs-lookup"><span data-stu-id="3cd40-289">Renders the person details part.</span></span> |
