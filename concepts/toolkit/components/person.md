---
title: Microsoft Graph 工具包中的 "人员" 组件
description: "\"人员\" 组件用于通过使用其照片、姓名和/或电子邮件地址显示人员或联系人。"
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 0202d8bc8c8ae23f98cb4add9f9d5ca96afea04d
ms.sourcegitcommit: f2dffaca3e1c5b74a01b59e1b76dba1592a6a5d1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/14/2020
ms.locfileid: "42639952"
---
# <a name="person-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="82e9e-103">Microsoft Graph 工具包中的 "人员" 组件</span><span class="sxs-lookup"><span data-stu-id="82e9e-103">Person component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="82e9e-104">"人员" 组件用于通过使用其照片、姓名和/或电子邮件地址显示人员或联系人。</span><span class="sxs-lookup"><span data-stu-id="82e9e-104">The person component is used to display a person or contact by using their photo, name, and/or email address.</span></span>

<span data-ttu-id="82e9e-105">"人员" 组件还使用 "管理员-[卡片](./person-card.md)" 显示带有有关用户的其他信息的飞出卡片。</span><span class="sxs-lookup"><span data-stu-id="82e9e-105">The person component also uses the [mgt-person-card](./person-card.md) to display a flyout card with additional information about the user.</span></span> <span data-ttu-id="82e9e-106">有关详细信息，请参阅 "[人员卡片](#person-card)" 部分。</span><span class="sxs-lookup"><span data-stu-id="82e9e-106">For details, see the [Person Card](#person-card) section.</span></span>

## <a name="example"></a><span data-ttu-id="82e9e-107">示例</span><span class="sxs-lookup"><span data-stu-id="82e9e-107">Example</span></span>

<span data-ttu-id="82e9e-108">下面的示例显示使用组件的`mgt-person`人员。</span><span class="sxs-lookup"><span data-stu-id="82e9e-108">The following example displays a person using the `mgt-person` component.</span></span> <span data-ttu-id="82e9e-109">您可以使用代码编辑器来查看[属性](#properties)如何更改组件的行为。</span><span class="sxs-lookup"><span data-stu-id="82e9e-109">You can use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-person--person&source=docs" height="250"></iframe>

[<span data-ttu-id="82e9e-110">在 "dev" 中打开此示例</span><span class="sxs-lookup"><span data-stu-id="82e9e-110">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-person--person&source=docs)

## <a name="setting-the-person-details"></a><span data-ttu-id="82e9e-111">设置人员详细信息</span><span class="sxs-lookup"><span data-stu-id="82e9e-111">Setting the person details</span></span>

<span data-ttu-id="82e9e-112">您可以使用三个属性来设置人员详细信息。</span><span class="sxs-lookup"><span data-stu-id="82e9e-112">You can use three properties to set the person details.</span></span> <span data-ttu-id="82e9e-113">每个实例仅使用下列属性之一：</span><span class="sxs-lookup"><span data-stu-id="82e9e-113">Use only one of the following properties per instance:</span></span>

* <span data-ttu-id="82e9e-114">通过使用`user-id`其 ID `userId`将属性或属性设置为从 Microsoft Graph 获取用户。</span><span class="sxs-lookup"><span data-stu-id="82e9e-114">Set the `user-id` attribute or `userId` property to fetch the user from Microsoft Graph by using their ID.</span></span>

* <span data-ttu-id="82e9e-115">将`person-query`属性或`personQuery`属性设置为在 Microsoft Graph 中搜索给定人员。</span><span class="sxs-lookup"><span data-stu-id="82e9e-115">Set the `person-query` attribute or `personQuery` property to search Microsoft Graph for a given person.</span></span> <span data-ttu-id="82e9e-116">它将选择第一个可用的人员并获取人员详细信息。</span><span class="sxs-lookup"><span data-stu-id="82e9e-116">It will choose the first person available and fetch the person details.</span></span> <span data-ttu-id="82e9e-117">电子邮件最适用于确保查询的是正确的人员，但名称也有效。</span><span class="sxs-lookup"><span data-stu-id="82e9e-117">An email works best to ensure the right person is queried, but a name works as well.</span></span>

* <span data-ttu-id="82e9e-118">将`person-details`属性或`personDetails`属性设置为手动设置人员详细信息，如下面的示例所示。</span><span class="sxs-lookup"><span data-stu-id="82e9e-118">Set the `person-details` attribute or `personDetails` property to manually set the person details, as shown in the following example.</span></span>


    ```js
    let personControl = document.getElementById('myPersonControl');
    personControl.personDetails = {
        displayName: 'Nikola Metulev',
        email: 'nikola@contoso.com',
        image: 'url'
    }
    ```

  <span data-ttu-id="82e9e-119">如果未提供图像，则将获取一个图像（如果可用）。</span><span class="sxs-lookup"><span data-stu-id="82e9e-119">If no image is provided, one will be fetched (if available).</span></span>

## <a name="properties"></a><span data-ttu-id="82e9e-120">属性</span><span class="sxs-lookup"><span data-stu-id="82e9e-120">Properties</span></span>

<span data-ttu-id="82e9e-121">您可以使用多个属性来自定义组件。</span><span class="sxs-lookup"><span data-stu-id="82e9e-121">You can use several properties to customize the component.</span></span>

| <span data-ttu-id="82e9e-122">属性</span><span class="sxs-lookup"><span data-stu-id="82e9e-122">Attribute</span></span>    | <span data-ttu-id="82e9e-123">属性</span><span class="sxs-lookup"><span data-stu-id="82e9e-123">Property</span></span>   | <span data-ttu-id="82e9e-124">说明</span><span class="sxs-lookup"><span data-stu-id="82e9e-124">Description</span></span>                                                   |
| -----------  | ---------- | ------------------------------------------------------------- |
| <span data-ttu-id="82e9e-125">显示-名称</span><span class="sxs-lookup"><span data-stu-id="82e9e-125">show-name</span></span>    | <span data-ttu-id="82e9e-126">showName</span><span class="sxs-lookup"><span data-stu-id="82e9e-126">showName</span></span>   | <span data-ttu-id="82e9e-127">设置用于显示人员显示名称的标志-默认`false`为。</span><span class="sxs-lookup"><span data-stu-id="82e9e-127">Set flag to display person display name - default is `false`.</span></span> |
| <span data-ttu-id="82e9e-128">显示-电子邮件</span><span class="sxs-lookup"><span data-stu-id="82e9e-128">show-email</span></span>   | <span data-ttu-id="82e9e-129">showEmail</span><span class="sxs-lookup"><span data-stu-id="82e9e-129">showEmail</span></span>  | <span data-ttu-id="82e9e-130">设置用于显示个人电子邮件的标志- `false`默认为。</span><span class="sxs-lookup"><span data-stu-id="82e9e-130">Set flag to display person email - default is `false`.</span></span>        |

## <a name="css-custom-properties"></a><span data-ttu-id="82e9e-131">CSS 自定义属性</span><span class="sxs-lookup"><span data-stu-id="82e9e-131">CSS custom properties</span></span>

<span data-ttu-id="82e9e-132">`mgt-person`组件定义以下 CSS 自定义属性。</span><span class="sxs-lookup"><span data-stu-id="82e9e-132">The `mgt-person` component defines the following CSS custom properties.</span></span>

```css
mgt-person {
  --avatar-size-s: 24px;
  --avatar-size: 48px; // avatar size when both name and email are shown
  --avatar-font-size--s: 16px;
  --avatar-font-size: 32px; // font-size when both name and email are shown
  --avatar-border: 0;
  --initials-color: white;
  --initials-background-color: magenta;
  --font-size: 12px;
  --font-weight: 500;
  --color: black;
  --email-font-size: 12px;
  --email-color: black;
}
```

<span data-ttu-id="82e9e-133">若要了解详细信息，请参阅[样式组件](../style.md)。</span><span class="sxs-lookup"><span data-stu-id="82e9e-133">To learn more, see [styling components](../style.md).</span></span>

## <a name="templates"></a><span data-ttu-id="82e9e-134">模板</span><span class="sxs-lookup"><span data-stu-id="82e9e-134">Templates</span></span>

<span data-ttu-id="82e9e-135">组件支持多个[模板](../templates.md)，这些模板允许您替换组件的某些部分。 `mgt-person`</span><span class="sxs-lookup"><span data-stu-id="82e9e-135">The `mgt-person` component supports several [templates](../templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="82e9e-136">若要指定模板，请在`<template>`组件内添加一个元素，并`data-type`将值设置为下列值之一：</span><span class="sxs-lookup"><span data-stu-id="82e9e-136">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following:</span></span>

| <span data-ttu-id="82e9e-137">数据类型</span><span class="sxs-lookup"><span data-stu-id="82e9e-137">Data type</span></span>     | <span data-ttu-id="82e9e-138">数据上下文</span><span class="sxs-lookup"><span data-stu-id="82e9e-138">Data context</span></span>              | <span data-ttu-id="82e9e-139">说明</span><span class="sxs-lookup"><span data-stu-id="82e9e-139">Description</span></span>                                                       |
| ---------     | ------------------------- | ----------------------------------------------------------------- |
| <span data-ttu-id="82e9e-140">设置</span><span class="sxs-lookup"><span data-stu-id="82e9e-140">default</span></span>     | <span data-ttu-id="82e9e-141">人员：人员详细信息对象</span><span class="sxs-lookup"><span data-stu-id="82e9e-141">person: The person details object</span></span> <br> <span data-ttu-id="82e9e-142">`personImage`：图像的 URL</span><span class="sxs-lookup"><span data-stu-id="82e9e-142">`personImage`: The URL of the image</span></span> | <span data-ttu-id="82e9e-143">默认模板会将整个组件替换为您自己的组件。</span><span class="sxs-lookup"><span data-stu-id="82e9e-143">The default template replaces the entire component with your own.</span></span> |
| <span data-ttu-id="82e9e-144">人员-卡片</span><span class="sxs-lookup"><span data-stu-id="82e9e-144">person-card</span></span> | <span data-ttu-id="82e9e-145">人员：人员详细信息对象</span><span class="sxs-lookup"><span data-stu-id="82e9e-145">person: The person details object</span></span> <br> <span data-ttu-id="82e9e-146">`personImage`：图像的 URL</span><span class="sxs-lookup"><span data-stu-id="82e9e-146">`personImage`: The URL of the image</span></span> | <span data-ttu-id="82e9e-147">用于更新在悬停或单击时显示的 "管理员-卡片" 的模板。</span><span class="sxs-lookup"><span data-stu-id="82e9e-147">The template to update the mgt-person-card displayed on hover or click.</span></span> |

<span data-ttu-id="82e9e-148">下面的示例定义了 "人员" 组件的模板。</span><span class="sxs-lookup"><span data-stu-id="82e9e-148">The following example defines a template for the person component.</span></span>

```html
<mgt-person>
  <template>
    <div data-if="person.image">
      <img src="{{person.image}}" />
    </div>
    <div data-else>
      {{person.displayName}}
    </div>
  </template>
</mgt-person>
```

## <a name="person-card"></a><span data-ttu-id="82e9e-149">个人卡片</span><span class="sxs-lookup"><span data-stu-id="82e9e-149">Person Card</span></span>

<span data-ttu-id="82e9e-150">`mgt-person`组件可显示为`mgt-person-card`悬停或单击。</span><span class="sxs-lookup"><span data-stu-id="82e9e-150">The `mgt-person` component can show an `mgt-person-card` on either hover or click.</span></span>

### <a name="add-the-control-to-the-html-page"></a><span data-ttu-id="82e9e-151">将控件添加到 HTML 页面</span><span class="sxs-lookup"><span data-stu-id="82e9e-151">Add the control to the HTML page</span></span>
```html
<mgt-person person-query="me" person-card="hover"></mgt-person>
```

| <span data-ttu-id="82e9e-152">属性</span><span class="sxs-lookup"><span data-stu-id="82e9e-152">Attribute</span></span>    |  <span data-ttu-id="82e9e-153">属性</span><span class="sxs-lookup"><span data-stu-id="82e9e-153">Property</span></span>     | <span data-ttu-id="82e9e-154">说明</span><span class="sxs-lookup"><span data-stu-id="82e9e-154">Description</span></span>                                                                     |
| ------------ | ------------- | ------------------------------------------------------------------------------- |
| <span data-ttu-id="82e9e-155">人员-卡片</span><span class="sxs-lookup"><span data-stu-id="82e9e-155">person-card</span></span> | <span data-ttu-id="82e9e-156">personCard</span><span class="sxs-lookup"><span data-stu-id="82e9e-156">personCard</span></span> | <span data-ttu-id="82e9e-157">一个枚举，用于确定激活浮出式面板- `hover`或`click`的必需用户操作。</span><span class="sxs-lookup"><span data-stu-id="82e9e-157">An enumeration to determine user action necessary to activate flyout panel - `hover` or `click`.</span></span> <span data-ttu-id="82e9e-158">默认值为`none`</span><span class="sxs-lookup"><span data-stu-id="82e9e-158">Default value is `none`</span></span> |


<span data-ttu-id="82e9e-159">有关模板化、样式和属性的详细信息，请参阅[人员卡片组件](./person-card.md)。</span><span class="sxs-lookup"><span data-stu-id="82e9e-159">For more information about templating, styling, and attributes, see [Person Card component](./person-card.md).</span></span>

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="82e9e-160">Microsoft Graph 权限</span><span class="sxs-lookup"><span data-stu-id="82e9e-160">Microsoft Graph permissions</span></span>

<span data-ttu-id="82e9e-161">此控件使用以下 Microsoft Graph Api 和权限。</span><span class="sxs-lookup"><span data-stu-id="82e9e-161">This control uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="82e9e-162">Resource</span><span class="sxs-lookup"><span data-stu-id="82e9e-162">Resource</span></span>                                                                                                    | <span data-ttu-id="82e9e-163">权限</span><span class="sxs-lookup"><span data-stu-id="82e9e-163">Permission</span></span>     |
| ----------------------------------------------------------------------------------------------------------- | -------------------- |
| [<span data-ttu-id="82e9e-164">/me</span><span class="sxs-lookup"><span data-stu-id="82e9e-164">/me</span></span>](/graph/api/user-get?view=graph-rest-1.0)                              | <span data-ttu-id="82e9e-165">User.Read</span><span class="sxs-lookup"><span data-stu-id="82e9e-165">User.Read</span></span>          |
| [<span data-ttu-id="82e9e-166">/me/photo/$value</span><span class="sxs-lookup"><span data-stu-id="82e9e-166">/me/photo/$value</span></span>](/graph/api/profilephoto-get?view=graph-rest-beta)        | <span data-ttu-id="82e9e-167">User.Read</span><span class="sxs-lookup"><span data-stu-id="82e9e-167">User.Read</span></span>          |
| [<span data-ttu-id="82e9e-168">/me/people/？ $search =</span><span class="sxs-lookup"><span data-stu-id="82e9e-168">/me/people/?$search=</span></span>](/graph/api/user-list-people?view=graph-rest-1.0)     | <span data-ttu-id="82e9e-169">People.Read</span><span class="sxs-lookup"><span data-stu-id="82e9e-169">People.Read</span></span>        |
| [<span data-ttu-id="82e9e-170">/me/contacts/\*</span><span class="sxs-lookup"><span data-stu-id="82e9e-170">/me/contacts/\*</span></span>](/graph/api/user-list-contacts?view=graph-rest-1.0&tabs=cs) | <span data-ttu-id="82e9e-171">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="82e9e-171">Contacts.Read</span></span>      |
| [<span data-ttu-id="82e9e-172">/users/{id}/photo/$value</span><span class="sxs-lookup"><span data-stu-id="82e9e-172">/users/{id}/photo/$value</span></span>](/graph/api/user-list-people?view=graph-rest-1.0) | <span data-ttu-id="82e9e-173">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="82e9e-173">User.ReadBasic.All</span></span> |

> <span data-ttu-id="82e9e-174">**注意：** 若要访问`*/photo/$value`个人 Microsoft 帐户的资源，请使用 Microsoft Graph beta 终结点。</span><span class="sxs-lookup"><span data-stu-id="82e9e-174">**Note:** to access the `*/photo/$value` resources for personal Microsoft accounts, use the Microsoft Graph beta endpoint.</span></span>

## <a name="authentication"></a><span data-ttu-id="82e9e-175">身份验证</span><span class="sxs-lookup"><span data-stu-id="82e9e-175">Authentication</span></span>

<span data-ttu-id="82e9e-176">该控件使用[身份验证文档](./../providers.md)中介绍的全局身份验证提供程序提取所需的数据。</span><span class="sxs-lookup"><span data-stu-id="82e9e-176">The control uses the global authentication provider described in the [authentication documentation](./../providers.md) to fetch the required data.</span></span>
