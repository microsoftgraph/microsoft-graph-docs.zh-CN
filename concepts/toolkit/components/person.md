---
title: Microsoft Graph 工具包中的 "人员" 组件
description: "\"人员\" 组件用于通过使用其照片、姓名和/或电子邮件地址显示人员或联系人。"
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: b9102259258bb691dee2c56449257740db7b1913
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2019
ms.locfileid: "35242954"
---
# <a name="person-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="965b2-103">Microsoft Graph 工具包中的 "人员" 组件</span><span class="sxs-lookup"><span data-stu-id="965b2-103">Person component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="965b2-104">"人员" 组件用于通过使用其照片、姓名和/或电子邮件地址显示人员或联系人。</span><span class="sxs-lookup"><span data-stu-id="965b2-104">The person component is used to display a person or contact by using their photo, name, and/or email address.</span></span> 

## <a name="example"></a><span data-ttu-id="965b2-105">示例</span><span class="sxs-lookup"><span data-stu-id="965b2-105">Example</span></span>

[<span data-ttu-id="965b2-106">jsfiddle 示例</span><span class="sxs-lookup"><span data-stu-id="965b2-106">jsfiddle example</span></span>](https://jsfiddle.net/metulev/0jkzfr42/)

### <a name="add-the-control-to-the-html-page"></a><span data-ttu-id="965b2-107">将控件添加到 HTML 页面</span><span class="sxs-lookup"><span data-stu-id="965b2-107">Add the control to the HTML page</span></span>
```html
<mgt-person person-query=""></mgt-person>
```

## <a name="setting-the-person-details"></a><span data-ttu-id="965b2-108">设置人员详细信息</span><span class="sxs-lookup"><span data-stu-id="965b2-108">Setting the person details</span></span>

<span data-ttu-id="965b2-109">您可以使用三个属性来设置人员详细信息。</span><span class="sxs-lookup"><span data-stu-id="965b2-109">You can use three properties to set the person details.</span></span> <span data-ttu-id="965b2-110">每个实例仅使用下列属性之一:</span><span class="sxs-lookup"><span data-stu-id="965b2-110">Use only one of the following properties per instance:</span></span>

* <span data-ttu-id="965b2-111">通过使用`user-id`其 ID `userId`将属性或属性设置为从 Microsoft Graph 获取用户。</span><span class="sxs-lookup"><span data-stu-id="965b2-111">Set the `user-id` attribute or `userId` property to fetch the user from Microsoft Graph by using their ID.</span></span>  

* <span data-ttu-id="965b2-112">将`person-query`属性或`personQuery`属性设置为在 Microsoft Graph 中搜索给定人员。</span><span class="sxs-lookup"><span data-stu-id="965b2-112">Set the `person-query` attribute or `personQuery` property to search Microsoft Graph for a given person.</span></span> <span data-ttu-id="965b2-113">它将选择第一个可用的人员并获取人员详细信息。</span><span class="sxs-lookup"><span data-stu-id="965b2-113">It will choose the first person available and fetch the person details.</span></span> <span data-ttu-id="965b2-114">电子邮件最适用于确保查询的是正确的人员, 但名称也有效。</span><span class="sxs-lookup"><span data-stu-id="965b2-114">An email works best to ensure the right person is queried, but a name works as well.</span></span>

* <span data-ttu-id="965b2-115">将`person-details`属性或`personDetails`属性设置为手动设置人员详细信息, 如下面的示例所示。</span><span class="sxs-lookup"><span data-stu-id="965b2-115">Set the `person-details` attribute or `personDetails` property to manually set the person details, as shown in the following example.</span></span>


    ```js
    let personControl = document.getElementById('myPersonControl');
    personControl.personDetails = {
        displayName: 'Nikola Metulev',
        email: 'nikola@contoso.com',
        image: 'url'
    }
    ```

  <span data-ttu-id="965b2-116">如果未提供图像, 则将获取一个图像 (如果可用)。</span><span class="sxs-lookup"><span data-stu-id="965b2-116">If no image is provided, one will be fetched (if available).</span></span>

## <a name="changing-how-the-component-looks"></a><span data-ttu-id="965b2-117">更改组件的外观</span><span class="sxs-lookup"><span data-stu-id="965b2-117">Changing how the component looks</span></span>

<span data-ttu-id="965b2-118">您可以使用多个 propertiesto 来自定义组件。</span><span class="sxs-lookup"><span data-stu-id="965b2-118">You can use several propertiesto customize the component.</span></span>

| <span data-ttu-id="965b2-119">属性</span><span class="sxs-lookup"><span data-stu-id="965b2-119">Property</span></span> | <span data-ttu-id="965b2-120">属性</span><span class="sxs-lookup"><span data-stu-id="965b2-120">Attribute</span></span> | <span data-ttu-id="965b2-121">说明</span><span class="sxs-lookup"><span data-stu-id="965b2-121">Description</span></span> |
| --- | --- | --- |
| `showName` | `show-name` | <span data-ttu-id="965b2-122">设置用于显示人员显示名称的标志-默认`false`为。</span><span class="sxs-lookup"><span data-stu-id="965b2-122">Set flag to display person display name - default is `false`.</span></span> |
| `showEmail` | `show-email` | <span data-ttu-id="965b2-123">设置用于显示个人电子邮件的标志- `false`默认为。</span><span class="sxs-lookup"><span data-stu-id="965b2-123">Set flag to display person email - default is `false`.</span></span> |

## <a name="css-custom-properties"></a><span data-ttu-id="965b2-124">CSS 自定义属性</span><span class="sxs-lookup"><span data-stu-id="965b2-124">CSS custom properties</span></span>

<span data-ttu-id="965b2-125">`mgt-person`组件定义以下 CSS 自定义属性。</span><span class="sxs-lookup"><span data-stu-id="965b2-125">The `mgt-person` component defines the following CSS custom properties.</span></span>

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

<span data-ttu-id="965b2-126">若要了解详细信息, 请参阅[样式组件](../style.md)。</span><span class="sxs-lookup"><span data-stu-id="965b2-126">To learn more, see [styling components](../style.md).</span></span>

## <a name="templates"></a><span data-ttu-id="965b2-127">模板</span><span class="sxs-lookup"><span data-stu-id="965b2-127">Templates</span></span>

<span data-ttu-id="965b2-128">组件支持多个[模板](../templates.md), 这些模板允许您替换组件的某些部分。 `mgt-person`</span><span class="sxs-lookup"><span data-stu-id="965b2-128">The `mgt-person` component supports several [templates](../templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="965b2-129">若要指定模板, 请在`<template>`组件内添加一个元素, 并`data-type`将值设置为下列值之一:</span><span class="sxs-lookup"><span data-stu-id="965b2-129">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following:</span></span>

| <span data-ttu-id="965b2-130">数据类型</span><span class="sxs-lookup"><span data-stu-id="965b2-130">Data type</span></span> | <span data-ttu-id="965b2-131">数据上下文</span><span class="sxs-lookup"><span data-stu-id="965b2-131">Data context</span></span> | <span data-ttu-id="965b2-132">说明</span><span class="sxs-lookup"><span data-stu-id="965b2-132">Description</span></span> |
| --- | --- | --- |
| `default` | <span data-ttu-id="965b2-133">`person`: person 对象</span><span class="sxs-lookup"><span data-stu-id="965b2-133">`person`: a person object</span></span> | <span data-ttu-id="965b2-134">默认模板会将整个组件替换为您自己的组件。</span><span class="sxs-lookup"><span data-stu-id="965b2-134">The default template replaces the entire component with your own.</span></span> |

<span data-ttu-id="965b2-135">下面的示例定义了 "人员" 组件的模板:</span><span class="sxs-lookup"><span data-stu-id="965b2-135">The following example defines a template for the person component:</span></span>

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

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="965b2-136">Microsoft Graph 权限</span><span class="sxs-lookup"><span data-stu-id="965b2-136">Microsoft Graph permissions</span></span>

<span data-ttu-id="965b2-137">此控件使用以下 Microsoft Graph Api 和权限。</span><span class="sxs-lookup"><span data-stu-id="965b2-137">This control uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="965b2-138">资源</span><span class="sxs-lookup"><span data-stu-id="965b2-138">Resource</span></span> | <span data-ttu-id="965b2-139">权限/范围</span><span class="sxs-lookup"><span data-stu-id="965b2-139">Permission/scope</span></span> |
| - | - |
| [<span data-ttu-id="965b2-140">/me</span><span class="sxs-lookup"><span data-stu-id="965b2-140">/me</span></span>](https://docs.microsoft.com/en-us/graph/api/user-get?view=graph-rest-1.0) | `User.Read` |
| [<span data-ttu-id="965b2-141">/me/photo/$value</span><span class="sxs-lookup"><span data-stu-id="965b2-141">/me/photo/$value</span></span>](https://docs.microsoft.com/en-us/graph/api/profilephoto-get?view=graph-rest-beta) | `User.Read` |
| [<span data-ttu-id="965b2-142">/me/people/？ $search =</span><span class="sxs-lookup"><span data-stu-id="965b2-142">/me/people/?$search=</span></span>](https://docs.microsoft.com/en-us/graph/api/user-list-people?view=graph-rest-1.0) | `People.Read` |
| [<span data-ttu-id="965b2-143">/me/contacts/\*</span><span class="sxs-lookup"><span data-stu-id="965b2-143">/me/contacts/\*</span></span>](https://docs.microsoft.com/en-us/graph/api/user-list-contacts?view=graph-rest-1.0&tabs=cs) | `Contacts.Read` |
| [<span data-ttu-id="965b2-144">/users/{id}/photo/$value</span><span class="sxs-lookup"><span data-stu-id="965b2-144">/users/{id}/photo/$value</span></span>](https://docs.microsoft.com/en-us/graph/api/user-list-people?view=graph-rest-1.0) | `User.ReadBasic.All` |

> <span data-ttu-id="965b2-145">**注意:** 若要访问`*/photo/$value`个人 Microsoft 帐户的资源, 请使用 Microsoft Graph beta 终结点。</span><span class="sxs-lookup"><span data-stu-id="965b2-145">**Note:** to access the `*/photo/$value` resources for personal Microsoft accounts, use the Microsoft Graph beta endpoint.</span></span>

## <a name="authentication"></a><span data-ttu-id="965b2-146">身份验证</span><span class="sxs-lookup"><span data-stu-id="965b2-146">Authentication</span></span>

<span data-ttu-id="965b2-147">该控件使用[身份验证文档](./../providers.md)中介绍的全局身份验证提供程序提取所需的数据。</span><span class="sxs-lookup"><span data-stu-id="965b2-147">The control uses the global authentication provider described in the [authentication documentation](./../providers.md) to fetch the required data.</span></span>
