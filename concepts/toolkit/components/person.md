---
title: Microsoft Graph 服务中的人员Toolkit
description: 人员组件用于通过使用个人或联系人的照片、姓名和/或电子邮件地址来显示此人或联系人。
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: cfe5f6b97c35c2704def8c4879522268cc8cc91e
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49660037"
---
# <a name="person-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="736aa-103">Microsoft Graph 服务中的人员Toolkit</span><span class="sxs-lookup"><span data-stu-id="736aa-103">Person component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="736aa-104">人员组件用于通过使用个人或联系人的照片、姓名、电子邮件地址或任何其他人员详细信息来显示此人或联系人。</span><span class="sxs-lookup"><span data-stu-id="736aa-104">The person component is used to display a person or contact by using their photo, name, email address, or any other person details.</span></span>

<span data-ttu-id="736aa-105">人员组件还使用 [mgt-person-card](./person-card.md) 显示包含有关用户的其他信息的飞出卡。</span><span class="sxs-lookup"><span data-stu-id="736aa-105">The person component also uses the [mgt-person-card](./person-card.md) to display a flyout card with additional information about the user.</span></span> <span data-ttu-id="736aa-106">有关详细信息，请参阅" [人员卡片"](#person-card) 部分。</span><span class="sxs-lookup"><span data-stu-id="736aa-106">For details, see the [Person Card](#person-card) section.</span></span>

## <a name="example"></a><span data-ttu-id="736aa-107">示例</span><span class="sxs-lookup"><span data-stu-id="736aa-107">Example</span></span>

<span data-ttu-id="736aa-108">以下示例显示使用该组件 `mgt-person` 的人。</span><span class="sxs-lookup"><span data-stu-id="736aa-108">The following example displays a person using the `mgt-person` component.</span></span> <span data-ttu-id="736aa-109">可以使用代码编辑器查看属性 [如何](#properties) 更改组件的行为。</span><span class="sxs-lookup"><span data-stu-id="736aa-109">You can use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-person--person&source=docs" height="250"></iframe>

[<span data-ttu-id="736aa-110">在 mgt.dev 中打开此示例</span><span class="sxs-lookup"><span data-stu-id="736aa-110">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-person--person&source=docs)

## <a name="setting-the-person-details"></a><span data-ttu-id="736aa-111">设置人员详细信息</span><span class="sxs-lookup"><span data-stu-id="736aa-111">Setting the person details</span></span>

<span data-ttu-id="736aa-112">可以使用三个属性来设置人员详细信息。</span><span class="sxs-lookup"><span data-stu-id="736aa-112">You can use three properties to set the person details.</span></span> <span data-ttu-id="736aa-113">每个实例仅使用以下属性之一：</span><span class="sxs-lookup"><span data-stu-id="736aa-113">Use only one of the following properties per instance:</span></span>

* <span data-ttu-id="736aa-114">设置 `user-id` 属性或 `userId` 属性以使用用户的 ID 从 Microsoft Graph 提取用户。</span><span class="sxs-lookup"><span data-stu-id="736aa-114">Set the `user-id` attribute or `userId` property to fetch the user from Microsoft Graph by using their ID.</span></span>

* <span data-ttu-id="736aa-115">设置 `person-query` 属性或 `personQuery` 属性以搜索 Microsoft Graph 中给定人员。</span><span class="sxs-lookup"><span data-stu-id="736aa-115">Set the `person-query` attribute or `personQuery` property to search Microsoft Graph for a given person.</span></span> <span data-ttu-id="736aa-116">它将选择第一个可用的人员并提取人员详细信息。</span><span class="sxs-lookup"><span data-stu-id="736aa-116">It will choose the first person available and fetch the person details.</span></span> <span data-ttu-id="736aa-117">电子邮件最适用于确保查询正确的人员，但名称也有效。</span><span class="sxs-lookup"><span data-stu-id="736aa-117">An email works best to ensure the right person is queried, but a name works as well.</span></span>

* <span data-ttu-id="736aa-118">设置 `person-presence` 属性或 `personPresence` 属性以手动向个人头像添加状态锁屏提醒。</span><span class="sxs-lookup"><span data-stu-id="736aa-118">Set the `person-presence` attribute or `personPresence` property to add a presence badge to person avatar manually.</span></span>

* <span data-ttu-id="736aa-119">将 `avatar-size` 属性或 `avatarSize` 属性设置为 `small` 或 `large` 确定头像的大小。</span><span class="sxs-lookup"><span data-stu-id="736aa-119">Set the `avatar-size` attribute or `avatarSize` property to `small` or `large` to determine the size of avatar.</span></span> <span data-ttu-id="736aa-120">这有助于向头像 [添加正确的状态](https://mgt.dev/?path=/story/components-mgt-person--person-presence-display-all) 锁屏提醒。</span><span class="sxs-lookup"><span data-stu-id="736aa-120">This helps add the [correct presence badge](https://mgt.dev/?path=/story/components-mgt-person--person-presence-display-all) to avatar.</span></span> <span data-ttu-id="736aa-121">你需要选择正确的相应的 css 自定义属性，如下所示以进一步自定义头像大小。</span><span class="sxs-lookup"><span data-stu-id="736aa-121">You will need to choose the correct corresponding css custom properties shown below to further customize avatar size.</span></span> <span data-ttu-id="736aa-122">默认情况下，该值设置为 `auto` ，该值将自动决定如何根据属性呈现 `view` 状态。</span><span class="sxs-lookup"><span data-stu-id="736aa-122">By default, the value is set to `auto` which will automatically decide how to render the presence based on the `view` property.</span></span> <span data-ttu-id="736aa-123">如果你的头像小于 `small` 32px x 32px，我们建议使用。</span><span class="sxs-lookup"><span data-stu-id="736aa-123">We recommend using `small` if your avatar is smaller than 32px by 32px.</span></span> 

* <span data-ttu-id="736aa-124">使用 `person-details` 属性或 `personDetails` 属性手动设置人员详细信息，如以下示例所示。</span><span class="sxs-lookup"><span data-stu-id="736aa-124">Use the `person-details` attribute or `personDetails` property to manually set the person details, as shown in the following example.</span></span>


    ```js
    let personControl = document.getElementById('myPersonControl');
    personControl.personDetails = {
        displayName: 'Nikola Metulev',
        mail: 'nikola@contoso.com',
        personImage: 'url'
    }
    ```

  <span data-ttu-id="736aa-125">如果未提供图像，将提取一个 (（如果) ）。</span><span class="sxs-lookup"><span data-stu-id="736aa-125">If no image is provided, one will be fetched (if available).</span></span>

## <a name="properties"></a><span data-ttu-id="736aa-126">属性</span><span class="sxs-lookup"><span data-stu-id="736aa-126">Properties</span></span>

<span data-ttu-id="736aa-127">可以使用多个属性来自定义组件。</span><span class="sxs-lookup"><span data-stu-id="736aa-127">You can use several properties to customize the component.</span></span>

| <span data-ttu-id="736aa-128">属性</span><span class="sxs-lookup"><span data-stu-id="736aa-128">Attribute</span></span>       | <span data-ttu-id="736aa-129">属性</span><span class="sxs-lookup"><span data-stu-id="736aa-129">Property</span></span>       | <span data-ttu-id="736aa-130">说明</span><span class="sxs-lookup"><span data-stu-id="736aa-130">Description</span></span>                                                   |
| -----------     | ----------     | ------------------------------------------------------------- |
| <span data-ttu-id="736aa-131">user-id</span><span class="sxs-lookup"><span data-stu-id="736aa-131">user-id</span></span>         | <span data-ttu-id="736aa-132">userId</span><span class="sxs-lookup"><span data-stu-id="736aa-132">userId</span></span>         | <span data-ttu-id="736aa-133">设置为用户 ID，从 Microsoft Graph 获取该用户的详细信息和图像。</span><span class="sxs-lookup"><span data-stu-id="736aa-133">Set to a user id to fetch that user's details and image from Microsoft Graph.</span></span>|
| <span data-ttu-id="736aa-134">person-query</span><span class="sxs-lookup"><span data-stu-id="736aa-134">person-query</span></span>    | <span data-ttu-id="736aa-135">personQuery</span><span class="sxs-lookup"><span data-stu-id="736aa-135">personQuery</span></span>    | <span data-ttu-id="736aa-136">设置为人员的名称或电子邮件，以在 Microsoft Graph 中搜索某人并提取第一个人的详细信息和图像。</span><span class="sxs-lookup"><span data-stu-id="736aa-136">Set to a name or email of a person to search for a person in Microsoft Graph and fetch the first person's details and image.</span></span>|
| <span data-ttu-id="736aa-137">person-details</span><span class="sxs-lookup"><span data-stu-id="736aa-137">person-details</span></span>  | <span data-ttu-id="736aa-138">personDetails</span><span class="sxs-lookup"><span data-stu-id="736aa-138">personDetails</span></span>  | <span data-ttu-id="736aa-139">设置为表示人员的对象。</span><span class="sxs-lookup"><span data-stu-id="736aa-139">Set to an object representing a person.</span></span> <span data-ttu-id="736aa-140">使用来自人员、用户、联系人或组、资源的对象。</span><span class="sxs-lookup"><span data-stu-id="736aa-140">Works with object from the people, users, contacts, or group, resources.</span></span> |
| <span data-ttu-id="736aa-141">person-image</span><span class="sxs-lookup"><span data-stu-id="736aa-141">person-image</span></span>    | <span data-ttu-id="736aa-142">personImage</span><span class="sxs-lookup"><span data-stu-id="736aa-142">personImage</span></span>    | <span data-ttu-id="736aa-143">设置要为人员显示的图像。</span><span class="sxs-lookup"><span data-stu-id="736aa-143">Set the image to show for the person.</span></span> |
| <span data-ttu-id="736aa-144">person-presence</span><span class="sxs-lookup"><span data-stu-id="736aa-144">person-presence</span></span> | <span data-ttu-id="736aa-145">personPresence</span><span class="sxs-lookup"><span data-stu-id="736aa-145">personPresence</span></span> | <span data-ttu-id="736aa-146">为人员设置状态。</span><span class="sxs-lookup"><span data-stu-id="736aa-146">Set the presence for the person.</span></span> |
| <span data-ttu-id="736aa-147">fetch-image</span><span class="sxs-lookup"><span data-stu-id="736aa-147">fetch-image</span></span>     | <span data-ttu-id="736aa-148">fetchImage</span><span class="sxs-lookup"><span data-stu-id="736aa-148">fetchImage</span></span>     | <span data-ttu-id="736aa-149">设置标志以 `personImage` 根据用户提供的对象自动从 Microsoft Graph `personDetails` 提取。</span><span class="sxs-lookup"><span data-stu-id="736aa-149">Set flag to fetch `personImage` automatically from Microsoft Graph based on the `personDetails` object provided by the user.</span></span> |
| <span data-ttu-id="736aa-150">view</span><span class="sxs-lookup"><span data-stu-id="736aa-150">view</span></span>            | <span data-ttu-id="736aa-151">view</span><span class="sxs-lookup"><span data-stu-id="736aa-151">view</span></span>           | <span data-ttu-id="736aa-152">设置为控制人员呈现方式。</span><span class="sxs-lookup"><span data-stu-id="736aa-152">Set to control how the person is rendered.</span></span> <span data-ttu-id="736aa-153">默认值为 `avatar`</span><span class="sxs-lookup"><span data-stu-id="736aa-153">Default is `avatar`</span></span> <br /> <span data-ttu-id="736aa-154">`avatar` - 仅显示头像</span><span class="sxs-lookup"><span data-stu-id="736aa-154">`avatar` - show only avatar</span></span> <br /> <span data-ttu-id="736aa-155">`oneline` - 默认显示头像 (`displayName` 第一) </span><span class="sxs-lookup"><span data-stu-id="736aa-155">`oneline` - show avatar and first line (`displayName` by default)</span></span> <br /> <span data-ttu-id="736aa-156">`twolines` - 显示头像和两行文本 (`displayName` `mail` 默认显示) </span><span class="sxs-lookup"><span data-stu-id="736aa-156">`twolines` - show avatar and two lines of text (`displayName` and `mail` by default)</span></span>|
| <span data-ttu-id="736aa-157">line1-property</span><span class="sxs-lookup"><span data-stu-id="736aa-157">line1-property</span></span>  | <span data-ttu-id="736aa-158">line1Property</span><span class="sxs-lookup"><span data-stu-id="736aa-158">line1Property</span></span>  | <span data-ttu-id="736aa-159">设置用于第一行文本的 personDetails 的属性。</span><span class="sxs-lookup"><span data-stu-id="736aa-159">Sets the property of the personDetails to use for the first line of text.</span></span> <span data-ttu-id="736aa-160">默认值为“`displayName`”。</span><span class="sxs-lookup"><span data-stu-id="736aa-160">Default is `displayName`.</span></span>|
| <span data-ttu-id="736aa-161">line2-property</span><span class="sxs-lookup"><span data-stu-id="736aa-161">line2-property</span></span>  | <span data-ttu-id="736aa-162">line2Property</span><span class="sxs-lookup"><span data-stu-id="736aa-162">line2Property</span></span>  | <span data-ttu-id="736aa-163">设置用于第二行文本的 personDetails 的属性。</span><span class="sxs-lookup"><span data-stu-id="736aa-163">Sets the property of the personDetails to use for the second line of text.</span></span> <span data-ttu-id="736aa-164">默认值为“`mail`”。</span><span class="sxs-lookup"><span data-stu-id="736aa-164">Default is `mail`.</span></span>|
| <span data-ttu-id="736aa-165">line3-property</span><span class="sxs-lookup"><span data-stu-id="736aa-165">line3-property</span></span>  | <span data-ttu-id="736aa-166">line3Property</span><span class="sxs-lookup"><span data-stu-id="736aa-166">line3Property</span></span>  | <span data-ttu-id="736aa-167">设置用于第三行文本的 personDetails 的属性。</span><span class="sxs-lookup"><span data-stu-id="736aa-167">Sets the property of the personDetails to use for the third line of text.</span></span> <span data-ttu-id="736aa-168">默认值为“`jobTitle`”。</span><span class="sxs-lookup"><span data-stu-id="736aa-168">Default is `jobTitle`.</span></span>|
| <span data-ttu-id="736aa-169">show-presence</span><span class="sxs-lookup"><span data-stu-id="736aa-169">show-presence</span></span>   | <span data-ttu-id="736aa-170">showPresence</span><span class="sxs-lookup"><span data-stu-id="736aa-170">showPresence</span></span>   | <span data-ttu-id="736aa-171">设置用于显示人员状态的标志 - 默认值为 `false` 。</span><span class="sxs-lookup"><span data-stu-id="736aa-171">Set flag to display person presence - default is `false`.</span></span>|

## <a name="css-custom-properties"></a><span data-ttu-id="736aa-172">CSS 自定义属性</span><span class="sxs-lookup"><span data-stu-id="736aa-172">CSS custom properties</span></span>

<span data-ttu-id="736aa-173">该 `mgt-person` 组件定义以下 CSS 自定义属性。</span><span class="sxs-lookup"><span data-stu-id="736aa-173">The `mgt-person` component defines the following CSS custom properties.</span></span>

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

<span data-ttu-id="736aa-174">若要了解更多信息，请参阅 [样式组件](../customize-components/style.md)。</span><span class="sxs-lookup"><span data-stu-id="736aa-174">To learn more, see [styling components](../customize-components/style.md).</span></span>

## <a name="templates"></a><span data-ttu-id="736aa-175">模板</span><span class="sxs-lookup"><span data-stu-id="736aa-175">Templates</span></span>

<span data-ttu-id="736aa-176">该 `mgt-person` 组件支持 [多个模板](../customize-components/templates.md) ，允许您替换组件的某些部分。</span><span class="sxs-lookup"><span data-stu-id="736aa-176">The `mgt-person` component supports several [templates](../customize-components/templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="736aa-177">若要指定模板，请包含组件 `<template>` 中的元素，将值设置为下列值 `data-type` 之一：</span><span class="sxs-lookup"><span data-stu-id="736aa-177">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following:</span></span>

| <span data-ttu-id="736aa-178">数据类型</span><span class="sxs-lookup"><span data-stu-id="736aa-178">Data type</span></span> | <span data-ttu-id="736aa-179">数据上下文</span><span class="sxs-lookup"><span data-stu-id="736aa-179">Data context</span></span> | <span data-ttu-id="736aa-180">说明</span><span class="sxs-lookup"><span data-stu-id="736aa-180">Description</span></span> |
| --------- | ------------ | ----------- |
| <span data-ttu-id="736aa-181">loading</span><span class="sxs-lookup"><span data-stu-id="736aa-181">loading</span></span> | <span data-ttu-id="736aa-182">无</span><span class="sxs-lookup"><span data-stu-id="736aa-182">none</span></span> | <span data-ttu-id="736aa-183">组件在加载状态时要呈现的模板。</span><span class="sxs-lookup"><span data-stu-id="736aa-183">The template to render while the component is in a loading state.</span></span> |
| <span data-ttu-id="736aa-184">no-data</span><span class="sxs-lookup"><span data-stu-id="736aa-184">no-data</span></span> | <span data-ttu-id="736aa-185">无</span><span class="sxs-lookup"><span data-stu-id="736aa-185">none</span></span> | <span data-ttu-id="736aa-186">在无人员图像或数据可用时要呈现的模板。</span><span class="sxs-lookup"><span data-stu-id="736aa-186">The template to render when no person image or data is available.</span></span> | 
| <span data-ttu-id="736aa-187">default</span><span class="sxs-lookup"><span data-stu-id="736aa-187">default</span></span> | <span data-ttu-id="736aa-188">person： The person details object</span><span class="sxs-lookup"><span data-stu-id="736aa-188">person: The person details object</span></span> <br> <span data-ttu-id="736aa-189">`personImage`：图像的 URL</span><span class="sxs-lookup"><span data-stu-id="736aa-189">`personImage`: The URL of the image</span></span> | <span data-ttu-id="736aa-190">默认模板将整个组件替换为你自己的组件。</span><span class="sxs-lookup"><span data-stu-id="736aa-190">The default template replaces the entire component with your own.</span></span> |
| <span data-ttu-id="736aa-191">person-card</span><span class="sxs-lookup"><span data-stu-id="736aa-191">person-card</span></span> | <span data-ttu-id="736aa-192">person： The person details object</span><span class="sxs-lookup"><span data-stu-id="736aa-192">person: The person details object</span></span> <br> <span data-ttu-id="736aa-193">`personImage`：图像的 URL</span><span class="sxs-lookup"><span data-stu-id="736aa-193">`personImage`: The URL of the image</span></span> | <span data-ttu-id="736aa-194">用于更新悬停或单击时显示的 mgt-person-card 的模板。</span><span class="sxs-lookup"><span data-stu-id="736aa-194">The template to update the mgt-person-card displayed on hover or click.</span></span> |

<span data-ttu-id="736aa-195">以下示例为人员组件定义模板。</span><span class="sxs-lookup"><span data-stu-id="736aa-195">The following example defines a template for the person component.</span></span>

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

## <a name="person-card"></a><span data-ttu-id="736aa-196">个人卡片</span><span class="sxs-lookup"><span data-stu-id="736aa-196">Person card</span></span>

<span data-ttu-id="736aa-197">组件 `mgt-person` 可以在悬 `mgt-person-card` 停或单击时显示。</span><span class="sxs-lookup"><span data-stu-id="736aa-197">The `mgt-person` component can show an `mgt-person-card` on either hover or click.</span></span>

### <a name="add-the-control-to-the-html-page"></a><span data-ttu-id="736aa-198">将控件添加到 HTML 页面</span><span class="sxs-lookup"><span data-stu-id="736aa-198">Add the control to the HTML page</span></span>
```html
<mgt-person person-query="me" person-card="hover"></mgt-person>
```

| <span data-ttu-id="736aa-199">属性</span><span class="sxs-lookup"><span data-stu-id="736aa-199">Attribute</span></span>    |  <span data-ttu-id="736aa-200">属性</span><span class="sxs-lookup"><span data-stu-id="736aa-200">Property</span></span>     | <span data-ttu-id="736aa-201">说明</span><span class="sxs-lookup"><span data-stu-id="736aa-201">Description</span></span>                                                                     |
| ------------ | ------------- | ------------------------------------------------------------------------------- |
| <span data-ttu-id="736aa-202">person-card</span><span class="sxs-lookup"><span data-stu-id="736aa-202">person-card</span></span> | <span data-ttu-id="736aa-203">personCardInteraction</span><span class="sxs-lookup"><span data-stu-id="736aa-203">personCardInteraction</span></span> | <span data-ttu-id="736aa-204">一个枚举，用于确定激活飞出面板所需的用户操作 - `hover` 或 `click` 。</span><span class="sxs-lookup"><span data-stu-id="736aa-204">An enumeration to determine user action necessary to activate flyout panel - `hover` or `click`.</span></span> <span data-ttu-id="736aa-205">默认值为 `none`</span><span class="sxs-lookup"><span data-stu-id="736aa-205">Default value is `none`</span></span> |


<span data-ttu-id="736aa-206">有关模板、样式设置和属性详细信息，请参阅 Person Card [组件](./person-card.md)。</span><span class="sxs-lookup"><span data-stu-id="736aa-206">For more information about templating, styling, and attributes, see [Person Card component](./person-card.md).</span></span>

## <a name="global-component-configuration"></a><span data-ttu-id="736aa-207">全局组件配置</span><span class="sxs-lookup"><span data-stu-id="736aa-207">Global component configuration</span></span>

<span data-ttu-id="736aa-208">该类 `MgtPerson` 公开配置应用程序中所有人员 `config` 组件的静态对象。</span><span class="sxs-lookup"><span data-stu-id="736aa-208">The `MgtPerson` class exposes a static `config` object that configures all person components in the application.</span></span>

<span data-ttu-id="736aa-209">下面的示例演示如何使用 config 对象。</span><span class="sxs-lookup"><span data-stu-id="736aa-209">The following example shows how to use the config object.</span></span>

```ts
import { MgtPerson } from `@microsoft/mgt`;

MgtPerson.config.useContactApis = false;
```

<span data-ttu-id="736aa-210">以下属性在 config 对象上可用。</span><span class="sxs-lookup"><span data-stu-id="736aa-210">The following properties are available on the config object.</span></span>

| <span data-ttu-id="736aa-211">属性</span><span class="sxs-lookup"><span data-stu-id="736aa-211">Property</span></span> | <span data-ttu-id="736aa-212">说明</span><span class="sxs-lookup"><span data-stu-id="736aa-212">Description</span></span> |
| ------------ | ------------- |
| <span data-ttu-id="736aa-213">useContactApis</span><span class="sxs-lookup"><span data-stu-id="736aa-213">useContactApis</span></span> | <span data-ttu-id="736aa-214">`boolean` - 指示人员组件是否可以使用 Microsoft Graph 个人联系人 API 搜索联系人详细信息和照片。</span><span class="sxs-lookup"><span data-stu-id="736aa-214">`boolean` - Indicates whether the person component can use the Microsoft Graph personal contacts API to search for contact details and photos.</span></span> <span data-ttu-id="736aa-215">默认值为 `true`。</span><span class="sxs-lookup"><span data-stu-id="736aa-215">Default value is `true`.</span></span>  |

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="736aa-216">Microsoft Graph 权限</span><span class="sxs-lookup"><span data-stu-id="736aa-216">Microsoft Graph permissions</span></span>

<span data-ttu-id="736aa-217">此控件使用以下 Microsoft Graph API 和权限。</span><span class="sxs-lookup"><span data-stu-id="736aa-217">This control uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="736aa-218">资源</span><span class="sxs-lookup"><span data-stu-id="736aa-218">Resource</span></span> | <span data-ttu-id="736aa-219">权限</span><span class="sxs-lookup"><span data-stu-id="736aa-219">Permission</span></span>     |
| -| - |
| [<span data-ttu-id="736aa-220">/me</span><span class="sxs-lookup"><span data-stu-id="736aa-220">/me</span></span>](/graph/api/user-get)                              | <span data-ttu-id="736aa-221">User.Read</span><span class="sxs-lookup"><span data-stu-id="736aa-221">User.Read</span></span>          |
| [<span data-ttu-id="736aa-222">/me/photo/$value</span><span class="sxs-lookup"><span data-stu-id="736aa-222">/me/photo/$value</span></span>](/graph/api/profilephoto-get)        | <span data-ttu-id="736aa-223">User.Read</span><span class="sxs-lookup"><span data-stu-id="736aa-223">User.Read</span></span>          |
| [<span data-ttu-id="736aa-224">/me/people/？$search=</span><span class="sxs-lookup"><span data-stu-id="736aa-224">/me/people/?$search=</span></span>](/graph/api/user-list-people)     | <span data-ttu-id="736aa-225">People.Read</span><span class="sxs-lookup"><span data-stu-id="736aa-225">People.Read</span></span>        |
| [<span data-ttu-id="736aa-226">/me/contacts/\*</span><span class="sxs-lookup"><span data-stu-id="736aa-226">/me/contacts/\*</span></span>](/graph/api/user-list-contacts&tabs=cs) | <span data-ttu-id="736aa-227">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="736aa-227">Contacts.Read</span></span>      |
| [<span data-ttu-id="736aa-228">/users/{id}/photo/$value</span><span class="sxs-lookup"><span data-stu-id="736aa-228">/users/{id}/photo/$value</span></span>](/graph/api/user-list-people) | <span data-ttu-id="736aa-229">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="736aa-229">User.ReadBasic.All</span></span> |
| [<span data-ttu-id="736aa-230">/me/presence</span><span class="sxs-lookup"><span data-stu-id="736aa-230">/me/presence</span></span>](/graph/api/presence-get)                | <span data-ttu-id="736aa-231">Presence.Read</span><span class="sxs-lookup"><span data-stu-id="736aa-231">Presence.Read</span></span> |
| [<span data-ttu-id="736aa-232">/users/{id}/presence</span><span class="sxs-lookup"><span data-stu-id="736aa-232">/users/{id}/presence</span></span>](/graph/api/presence-get)        | <span data-ttu-id="736aa-233">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="736aa-233">Presence.Read.All</span></span> |

## <a name="authentication"></a><span data-ttu-id="736aa-234">身份验证</span><span class="sxs-lookup"><span data-stu-id="736aa-234">Authentication</span></span>

<span data-ttu-id="736aa-235">该控件使用身份验证文档中介绍的全局身份验证提供程序[](../providers/providers.md)获取所需数据。</span><span class="sxs-lookup"><span data-stu-id="736aa-235">The control uses the global authentication provider described in the [authentication documentation](../providers/providers.md) to fetch the required data.</span></span>

## <a name="extend-for-more-control"></a><span data-ttu-id="736aa-236">扩展以更多控制</span><span class="sxs-lookup"><span data-stu-id="736aa-236">Extend for more control</span></span>

<span data-ttu-id="736aa-237">对于更复杂的方案或真正自定义的 UX，此组件公开了多个在组件扩展中 `protected render*` 替代的方法。</span><span class="sxs-lookup"><span data-stu-id="736aa-237">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions.</span></span>

| <span data-ttu-id="736aa-238">方法</span><span class="sxs-lookup"><span data-stu-id="736aa-238">Method</span></span> | <span data-ttu-id="736aa-239">说明</span><span class="sxs-lookup"><span data-stu-id="736aa-239">Description</span></span> |
| - | - |
| <span data-ttu-id="736aa-240">renderLoading</span><span class="sxs-lookup"><span data-stu-id="736aa-240">renderLoading</span></span> | <span data-ttu-id="736aa-241">呈现加载状态。</span><span class="sxs-lookup"><span data-stu-id="736aa-241">Renders the loading state.</span></span> |
| <span data-ttu-id="736aa-242">renderNoData</span><span class="sxs-lookup"><span data-stu-id="736aa-242">renderNoData</span></span> | <span data-ttu-id="736aa-243">当图像或人员数据不可用时呈现。</span><span class="sxs-lookup"><span data-stu-id="736aa-243">Renders when no image or person data is available.</span></span> |
| <span data-ttu-id="736aa-244">renderAvatar</span><span class="sxs-lookup"><span data-stu-id="736aa-244">renderAvatar</span></span> | <span data-ttu-id="736aa-245">呈现头像。</span><span class="sxs-lookup"><span data-stu-id="736aa-245">Renders the avatar.</span></span> |
| <span data-ttu-id="736aa-246">renderDetails</span><span class="sxs-lookup"><span data-stu-id="736aa-246">renderDetails</span></span> | <span data-ttu-id="736aa-247">呈现人员详细信息部分。</span><span class="sxs-lookup"><span data-stu-id="736aa-247">Renders the person details part.</span></span> |
