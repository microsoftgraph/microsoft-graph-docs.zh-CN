---
title: Microsoft Graph 工具包中的 "人员" 组件
description: "\"人员\" 组件用于通过使用其照片、姓名和/或电子邮件地址显示人员或联系人。"
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: b4664cf545c858dbb2d49ad5191ab7cf5118092e
ms.sourcegitcommit: d9e94c109c0934cc93f340aafa1dccaa1a5da9c7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37275701"
---
# <a name="person-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="c8db6-103">Microsoft Graph 工具包中的 "人员" 组件</span><span class="sxs-lookup"><span data-stu-id="c8db6-103">Person component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="c8db6-104">"人员" 组件用于通过使用其照片、姓名和/或电子邮件地址显示人员或联系人。</span><span class="sxs-lookup"><span data-stu-id="c8db6-104">The person component is used to display a person or contact by using their photo, name, and/or email address.</span></span> 

<span data-ttu-id="c8db6-105">"人员" 组件还使用 "管理员-[卡片](./person-card.md)" 显示带有有关用户的其他信息的飞出卡片。</span><span class="sxs-lookup"><span data-stu-id="c8db6-105">The person component also uses the [mgt-person-card](./person-card.md) to display a flyout card with additional information about the user.</span></span> <span data-ttu-id="c8db6-106">有关详细信息，请参阅 "[人员卡片](#person-card)" 部分。</span><span class="sxs-lookup"><span data-stu-id="c8db6-106">For details, see the [Person Card](#person-card) section.</span></span>

## <a name="example"></a><span data-ttu-id="c8db6-107">示例</span><span class="sxs-lookup"><span data-stu-id="c8db6-107">Example</span></span>

[<span data-ttu-id="c8db6-108">jsfiddle 示例</span><span class="sxs-lookup"><span data-stu-id="c8db6-108">jsfiddle example</span></span>](https://jsfiddle.net/metulev/0jkzfr42/)

### <a name="add-the-control-to-the-html-page"></a><span data-ttu-id="c8db6-109">将控件添加到 HTML 页面</span><span class="sxs-lookup"><span data-stu-id="c8db6-109">Add the control to the HTML page</span></span>
```html
<mgt-person person-query=""></mgt-person>
```

## <a name="setting-the-person-details"></a><span data-ttu-id="c8db6-110">设置人员详细信息</span><span class="sxs-lookup"><span data-stu-id="c8db6-110">Setting the person details</span></span>

<span data-ttu-id="c8db6-111">您可以使用三个属性来设置人员详细信息。</span><span class="sxs-lookup"><span data-stu-id="c8db6-111">You can use three properties to set the person details.</span></span> <span data-ttu-id="c8db6-112">每个实例仅使用下列属性之一：</span><span class="sxs-lookup"><span data-stu-id="c8db6-112">Use only one of the following properties per instance:</span></span>

* <span data-ttu-id="c8db6-113">通过使用`user-id`其 ID `userId`将属性或属性设置为从 Microsoft Graph 获取用户。</span><span class="sxs-lookup"><span data-stu-id="c8db6-113">Set the `user-id` attribute or `userId` property to fetch the user from Microsoft Graph by using their ID.</span></span>  

* <span data-ttu-id="c8db6-114">将`person-query`属性或`personQuery`属性设置为在 Microsoft Graph 中搜索给定人员。</span><span class="sxs-lookup"><span data-stu-id="c8db6-114">Set the `person-query` attribute or `personQuery` property to search Microsoft Graph for a given person.</span></span> <span data-ttu-id="c8db6-115">它将选择第一个可用的人员并获取人员详细信息。</span><span class="sxs-lookup"><span data-stu-id="c8db6-115">It will choose the first person available and fetch the person details.</span></span> <span data-ttu-id="c8db6-116">电子邮件最适用于确保查询的是正确的人员，但名称也有效。</span><span class="sxs-lookup"><span data-stu-id="c8db6-116">An email works best to ensure the right person is queried, but a name works as well.</span></span>

* <span data-ttu-id="c8db6-117">将`person-details`属性或`personDetails`属性设置为手动设置人员详细信息，如下面的示例所示。</span><span class="sxs-lookup"><span data-stu-id="c8db6-117">Set the `person-details` attribute or `personDetails` property to manually set the person details, as shown in the following example.</span></span>


    ```js
    let personControl = document.getElementById('myPersonControl');
    personControl.personDetails = {
        displayName: 'Nikola Metulev',
        email: 'nikola@contoso.com',
        image: 'url'
    }
    ```

  <span data-ttu-id="c8db6-118">如果未提供图像，则将获取一个图像（如果可用）。</span><span class="sxs-lookup"><span data-stu-id="c8db6-118">If no image is provided, one will be fetched (if available).</span></span>

## <a name="changing-how-the-component-looks"></a><span data-ttu-id="c8db6-119">更改组件的外观</span><span class="sxs-lookup"><span data-stu-id="c8db6-119">Changing how the component looks</span></span>

<span data-ttu-id="c8db6-120">您可以使用多个属性来自定义组件。</span><span class="sxs-lookup"><span data-stu-id="c8db6-120">You can use several properties to customize the component.</span></span>

| <span data-ttu-id="c8db6-121">属性</span><span class="sxs-lookup"><span data-stu-id="c8db6-121">Property</span></span>    | <span data-ttu-id="c8db6-122">属性</span><span class="sxs-lookup"><span data-stu-id="c8db6-122">Attribute</span></span>    | <span data-ttu-id="c8db6-123">说明</span><span class="sxs-lookup"><span data-stu-id="c8db6-123">Description</span></span>                                                   |
| ----------- | ------------ | ------------------------------------------------------------- |
| <span data-ttu-id="c8db6-124">showName</span><span class="sxs-lookup"><span data-stu-id="c8db6-124">showName</span></span>  | <span data-ttu-id="c8db6-125">显示-名称</span><span class="sxs-lookup"><span data-stu-id="c8db6-125">show-name</span></span>  | <span data-ttu-id="c8db6-126">设置用于显示人员显示名称的标志-默认`false`为。</span><span class="sxs-lookup"><span data-stu-id="c8db6-126">Set flag to display person display name - default is `false`.</span></span> |
| <span data-ttu-id="c8db6-127">showEmail</span><span class="sxs-lookup"><span data-stu-id="c8db6-127">showEmail</span></span> | <span data-ttu-id="c8db6-128">显示-电子邮件</span><span class="sxs-lookup"><span data-stu-id="c8db6-128">show-email</span></span> | <span data-ttu-id="c8db6-129">设置用于显示个人电子邮件的标志- `false`默认为。</span><span class="sxs-lookup"><span data-stu-id="c8db6-129">Set flag to display person email - default is `false`.</span></span>        |

## <a name="css-custom-properties"></a><span data-ttu-id="c8db6-130">CSS 自定义属性</span><span class="sxs-lookup"><span data-stu-id="c8db6-130">CSS custom properties</span></span>

<span data-ttu-id="c8db6-131">`mgt-person`组件定义以下 CSS 自定义属性。</span><span class="sxs-lookup"><span data-stu-id="c8db6-131">The `mgt-person` component defines the following CSS custom properties.</span></span>

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

<span data-ttu-id="c8db6-132">若要了解详细信息，请参阅[样式组件](../style.md)。</span><span class="sxs-lookup"><span data-stu-id="c8db6-132">To learn more, see [styling components](../style.md).</span></span>

## <a name="templates"></a><span data-ttu-id="c8db6-133">模板</span><span class="sxs-lookup"><span data-stu-id="c8db6-133">Templates</span></span>

<span data-ttu-id="c8db6-134">组件支持多个[模板](../templates.md)，这些模板允许您替换组件的某些部分。 `mgt-person`</span><span class="sxs-lookup"><span data-stu-id="c8db6-134">The `mgt-person` component supports several [templates](../templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="c8db6-135">若要指定模板，请在`<template>`组件内添加一个元素，并`data-type`将值设置为下列值之一：</span><span class="sxs-lookup"><span data-stu-id="c8db6-135">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following:</span></span>

| <span data-ttu-id="c8db6-136">数据类型</span><span class="sxs-lookup"><span data-stu-id="c8db6-136">Data type</span></span>     | <span data-ttu-id="c8db6-137">数据上下文</span><span class="sxs-lookup"><span data-stu-id="c8db6-137">Data context</span></span>              | <span data-ttu-id="c8db6-138">说明</span><span class="sxs-lookup"><span data-stu-id="c8db6-138">Description</span></span>                                                       |
| ---------     | ------------------------- | ----------------------------------------------------------------- |
| <span data-ttu-id="c8db6-139">设置</span><span class="sxs-lookup"><span data-stu-id="c8db6-139">default</span></span>     | <span data-ttu-id="c8db6-140">人员：人员详细信息对象</span><span class="sxs-lookup"><span data-stu-id="c8db6-140">person: The person details object</span></span> <br> <span data-ttu-id="c8db6-141">`personImage`：图像的 URL</span><span class="sxs-lookup"><span data-stu-id="c8db6-141">`personImage`: The URL of the image</span></span> | <span data-ttu-id="c8db6-142">默认模板会将整个组件替换为您自己的组件。</span><span class="sxs-lookup"><span data-stu-id="c8db6-142">The default template replaces the entire component with your own.</span></span> |
| <span data-ttu-id="c8db6-143">人员-卡片</span><span class="sxs-lookup"><span data-stu-id="c8db6-143">person-card</span></span> | <span data-ttu-id="c8db6-144">人员：人员详细信息对象</span><span class="sxs-lookup"><span data-stu-id="c8db6-144">person: The person details object</span></span> <br> <span data-ttu-id="c8db6-145">`personImage`：图像的 URL</span><span class="sxs-lookup"><span data-stu-id="c8db6-145">`personImage`: The URL of the image</span></span> | <span data-ttu-id="c8db6-146">用于更新在悬停或单击时显示的 "管理员-卡片" 的模板。</span><span class="sxs-lookup"><span data-stu-id="c8db6-146">The template to update the mgt-person-card displayed on hover or click.</span></span> |

<span data-ttu-id="c8db6-147">下面的示例定义了 "人员" 组件的模板。</span><span class="sxs-lookup"><span data-stu-id="c8db6-147">The following example defines a template for the person component.</span></span>

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

## <a name="person-card"></a><span data-ttu-id="c8db6-148">个人卡片</span><span class="sxs-lookup"><span data-stu-id="c8db6-148">Person Card</span></span>

<span data-ttu-id="c8db6-149">`mgt-person`组件可显示为`mgt-person-card`悬停或单击。</span><span class="sxs-lookup"><span data-stu-id="c8db6-149">The `mgt-person` component can show an `mgt-person-card` on either hover or click.</span></span>

### <a name="add-the-control-to-the-html-page"></a><span data-ttu-id="c8db6-150">将控件添加到 HTML 页面</span><span class="sxs-lookup"><span data-stu-id="c8db6-150">Add the control to the HTML page</span></span>
```html
<mgt-person person-query="me" person-card="hover"></mgt-person>
```

| <span data-ttu-id="c8db6-151">属性</span><span class="sxs-lookup"><span data-stu-id="c8db6-151">Property</span></span>     | <span data-ttu-id="c8db6-152">属性</span><span class="sxs-lookup"><span data-stu-id="c8db6-152">Attribute</span></span>     | <span data-ttu-id="c8db6-153">说明</span><span class="sxs-lookup"><span data-stu-id="c8db6-153">Description</span></span>                                                                     |
| ------------ | ------------- | ------------------------------------------------------------------------------- |
| <span data-ttu-id="c8db6-154">personCard</span><span class="sxs-lookup"><span data-stu-id="c8db6-154">personCard</span></span> | <span data-ttu-id="c8db6-155">人员-卡片</span><span class="sxs-lookup"><span data-stu-id="c8db6-155">person-card</span></span> | <span data-ttu-id="c8db6-156">一个枚举，用于确定激活浮出式面板- `hover`或`click`的必需用户操作。</span><span class="sxs-lookup"><span data-stu-id="c8db6-156">An enumeration to determine user action necessary to activate flyout panel - `hover` or `click`.</span></span> <span data-ttu-id="c8db6-157">默认值为`none`</span><span class="sxs-lookup"><span data-stu-id="c8db6-157">Default value is `none`</span></span> |


<span data-ttu-id="c8db6-158">有关模板化、样式和属性的详细信息，请参阅[人员卡片组件](./person-card.md)。</span><span class="sxs-lookup"><span data-stu-id="c8db6-158">For more information about templating, styling, and attributes, see [Person Card component](./person-card.md).</span></span>

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="c8db6-159">Microsoft Graph 权限</span><span class="sxs-lookup"><span data-stu-id="c8db6-159">Microsoft Graph permissions</span></span>

<span data-ttu-id="c8db6-160">此控件使用以下 Microsoft Graph Api 和权限。</span><span class="sxs-lookup"><span data-stu-id="c8db6-160">This control uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="c8db6-161">资源</span><span class="sxs-lookup"><span data-stu-id="c8db6-161">Resource</span></span>                                                                                                    | <span data-ttu-id="c8db6-162">权限</span><span class="sxs-lookup"><span data-stu-id="c8db6-162">Permission</span></span>     |
| ----------------------------------------------------------------------------------------------------------- | -------------------- |
| [<span data-ttu-id="c8db6-163">/me</span><span class="sxs-lookup"><span data-stu-id="c8db6-163">/me</span></span>](https://docs.microsoft.com/en-us/graph/api/user-get?view=graph-rest-1.0)                              | <span data-ttu-id="c8db6-164">User.Read</span><span class="sxs-lookup"><span data-stu-id="c8db6-164">User.Read</span></span>          |
| [<span data-ttu-id="c8db6-165">/me/photo/$value</span><span class="sxs-lookup"><span data-stu-id="c8db6-165">/me/photo/$value</span></span>](https://docs.microsoft.com/en-us/graph/api/profilephoto-get?view=graph-rest-beta)        | <span data-ttu-id="c8db6-166">User.Read</span><span class="sxs-lookup"><span data-stu-id="c8db6-166">User.Read</span></span>          |
| [<span data-ttu-id="c8db6-167">/me/people/？ $search =</span><span class="sxs-lookup"><span data-stu-id="c8db6-167">/me/people/?$search=</span></span>](https://docs.microsoft.com/en-us/graph/api/user-list-people?view=graph-rest-1.0)     | <span data-ttu-id="c8db6-168">People.Read</span><span class="sxs-lookup"><span data-stu-id="c8db6-168">People.Read</span></span>        |
| [<span data-ttu-id="c8db6-169">/me/contacts/\*</span><span class="sxs-lookup"><span data-stu-id="c8db6-169">/me/contacts/\*</span></span>](https://docs.microsoft.com/en-us/graph/api/user-list-contacts?view=graph-rest-1.0&tabs=cs) | <span data-ttu-id="c8db6-170">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="c8db6-170">Contacts.Read</span></span>      |
| [<span data-ttu-id="c8db6-171">/users/{id}/photo/$value</span><span class="sxs-lookup"><span data-stu-id="c8db6-171">/users/{id}/photo/$value</span></span>](https://docs.microsoft.com/en-us/graph/api/user-list-people?view=graph-rest-1.0) | <span data-ttu-id="c8db6-172">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="c8db6-172">User.ReadBasic.All</span></span> |

> <span data-ttu-id="c8db6-173">**注意：** 若要访问`*/photo/$value`个人 Microsoft 帐户的资源，请使用 Microsoft Graph beta 终结点。</span><span class="sxs-lookup"><span data-stu-id="c8db6-173">**Note:** to access the `*/photo/$value` resources for personal Microsoft accounts, use the Microsoft Graph beta endpoint.</span></span>

## <a name="authentication"></a><span data-ttu-id="c8db6-174">身份验证</span><span class="sxs-lookup"><span data-stu-id="c8db6-174">Authentication</span></span>

<span data-ttu-id="c8db6-175">该控件使用[身份验证文档](./../providers.md)中介绍的全局身份验证提供程序提取所需的数据。</span><span class="sxs-lookup"><span data-stu-id="c8db6-175">The control uses the global authentication provider described in the [authentication documentation](./../providers.md) to fetch the required data.</span></span>
