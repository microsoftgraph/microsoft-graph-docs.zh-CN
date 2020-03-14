---
title: Microsoft Graph 工具包中的个人卡片组件
description: "\"个人卡片\" 组件是显示与某个人相关的详细信息的组件。"
localization_priority: Normal
author: vogtn
ms.openlocfilehash: 336e6beabc227a2574e41cf6a658d38fdabfcdcf
ms.sourcegitcommit: f2dffaca3e1c5b74a01b59e1b76dba1592a6a5d1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/14/2020
ms.locfileid: "42639924"
---
# <a name="person-card-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="487a5-103">Microsoft Graph 工具包中的个人卡片组件</span><span class="sxs-lookup"><span data-stu-id="487a5-103">Person-Card component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="487a5-104">个人卡片组件是一个响应性组件，用于显示与人员相关的更多信息。</span><span class="sxs-lookup"><span data-stu-id="487a5-104">A Person-Card component is a responsive component to display more information related to a person.</span></span> <span data-ttu-id="487a5-105">它通常用作`mgt-person`组件上的浮出控件。</span><span class="sxs-lookup"><span data-stu-id="487a5-105">It is generally used as a flyout on the `mgt-person` component.</span></span>

<span data-ttu-id="487a5-106">有关`mgt-person`组件的详细信息，请参阅 "[管理员文档](./person.md)"。</span><span class="sxs-lookup"><span data-stu-id="487a5-106">For more information about the `mgt-person` component, see [mgt-person docs](./person.md).</span></span>

## <a name="example"></a><span data-ttu-id="487a5-107">示例</span><span class="sxs-lookup"><span data-stu-id="487a5-107">Example</span></span>

<span data-ttu-id="487a5-108">下面的示例演示组件与组件的`mgt-person-card`配合`mgt-person`使用。</span><span class="sxs-lookup"><span data-stu-id="487a5-108">The following example shows the use of the `mgt-person-card` component with a `mgt-person` component.</span></span> <span data-ttu-id="487a5-109">将鼠标悬停在人员上以查看人员卡片，并使用代码编辑器查看[属性](#properties)如何更改组件的行为。</span><span class="sxs-lookup"><span data-stu-id="487a5-109">Hover over the person to see the Person Card and use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>
  
<iframe src="https://mgt.dev/iframe.html?id=components-mgt-person-card--person-card-hover&source=docs" height="400"></iframe>

[<span data-ttu-id="487a5-110">在 "dev" 中打开此示例</span><span class="sxs-lookup"><span data-stu-id="487a5-110">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-person-card--person-card-hover&source=docs)

## <a name="properties"></a><span data-ttu-id="487a5-111">属性</span><span class="sxs-lookup"><span data-stu-id="487a5-111">Properties</span></span>

<span data-ttu-id="487a5-112">组件使用 Microsoft Graph 提供有关用户的其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="487a5-112">The component uses Microsoft Graph to provide additional details about the user.</span></span> <span data-ttu-id="487a5-113">若要定义用户，必须使用的`mgt-person`**人员查询**属性。</span><span class="sxs-lookup"><span data-stu-id="487a5-113">To define a user, you must use the **person-query** property of `mgt-person`.</span></span>

| <span data-ttu-id="487a5-114">属性</span><span class="sxs-lookup"><span data-stu-id="487a5-114">Attribute</span></span>         | <span data-ttu-id="487a5-115">类型</span><span class="sxs-lookup"><span data-stu-id="487a5-115">Type</span></span>                     | <span data-ttu-id="487a5-116">说明</span><span class="sxs-lookup"><span data-stu-id="487a5-116">Description</span></span>                                                                           |
| ---------------- | -------------------------------- | ------------------------------------------------------------------------------------- |
| <span data-ttu-id="487a5-117">人员-详细信息</span><span class="sxs-lookup"><span data-stu-id="487a5-117">person-details</span></span> | <span data-ttu-id="487a5-118">MicrosoftGraph</span><span class="sxs-lookup"><span data-stu-id="487a5-118">MicrosoftGraph.User</span></span> <br> <span data-ttu-id="487a5-119">MicrosoftGraph</span><span class="sxs-lookup"><span data-stu-id="487a5-119">MicrosoftGraph.Person</span></span> <br> <span data-ttu-id="487a5-120">MicrosoftGraph。联系人</span><span class="sxs-lookup"><span data-stu-id="487a5-120">MicrosoftGraph.Contact</span></span> | <span data-ttu-id="487a5-121">由 Microsoft Graph 定义的 Person 对象，包含与用户相关的详细信息。</span><span class="sxs-lookup"><span data-stu-id="487a5-121">Person object as defined by Microsoft Graph, containing details related to the user.</span></span> |
| <span data-ttu-id="487a5-122">人员-图像</span><span class="sxs-lookup"><span data-stu-id="487a5-122">person-image</span></span>   | <span data-ttu-id="487a5-123">png/jpg/svg</span><span class="sxs-lookup"><span data-stu-id="487a5-123">png/jpg/svg</span></span>                    | <span data-ttu-id="487a5-124">与卡片中显示的人员相关的图像。</span><span class="sxs-lookup"><span data-stu-id="487a5-124">Image related to the person displayed in the card.</span></span>                                   |
| <span data-ttu-id="487a5-125">继承-详细信息</span><span class="sxs-lookup"><span data-stu-id="487a5-125">inherit-details</span></span>   | <span data-ttu-id="487a5-126">无。</span><span class="sxs-lookup"><span data-stu-id="487a5-126">None.</span></span>                  | <span data-ttu-id="487a5-127">允许人员卡片遍历父树 for `mgt-person` component 以使用相同`person-details`和`person-image`数据。</span><span class="sxs-lookup"><span data-stu-id="487a5-127">Allows person-card to walk parent tree for `mgt-person` component to use the same `person-details` and `person-image` data.</span></span>                      |


## <a name="templates"></a><span data-ttu-id="487a5-128">模板</span><span class="sxs-lookup"><span data-stu-id="487a5-128">Templates</span></span>

<span data-ttu-id="487a5-129">人员卡片组件使用允许您添加或替换部分组件的[模板](../templates.md)。</span><span class="sxs-lookup"><span data-stu-id="487a5-129">The Person-Card component uses [templates](../templates.md) that allow you to add or replace portions of the component.</span></span> <span data-ttu-id="487a5-130">若要指定模板，请在`<template>`组件内添加一个元素，并将`data-type`值设置为下列值之一。</span><span class="sxs-lookup"><span data-stu-id="487a5-130">To specify a template, include a `<template>` element inside of a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="487a5-131">数据类型</span><span class="sxs-lookup"><span data-stu-id="487a5-131">Data type</span></span> | <span data-ttu-id="487a5-132">数据上下文</span><span class="sxs-lookup"><span data-stu-id="487a5-132">Data context</span></span> | <span data-ttu-id="487a5-133">说明</span><span class="sxs-lookup"><span data-stu-id="487a5-133">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="487a5-134">设置</span><span class="sxs-lookup"><span data-stu-id="487a5-134">default</span></span> | <span data-ttu-id="487a5-135">`person`： Person details 对象</span><span class="sxs-lookup"><span data-stu-id="487a5-135">`person`: The person details object</span></span> <br> <span data-ttu-id="487a5-136">`personImage`：图像的 URL</span><span class="sxs-lookup"><span data-stu-id="487a5-136">`personImage`: The URL of the image</span></span> | <span data-ttu-id="487a5-137">默认模板会将整个组件替换为您自己的组件。</span><span class="sxs-lookup"><span data-stu-id="487a5-137">The default template replaces the entire component with your own.</span></span> |
| <span data-ttu-id="487a5-138">其他详细信息</span><span class="sxs-lookup"><span data-stu-id="487a5-138">additional-details</span></span> | <span data-ttu-id="487a5-139">`person`： Person details 对象</span><span class="sxs-lookup"><span data-stu-id="487a5-139">`person`: The person details object</span></span> <br> <span data-ttu-id="487a5-140">`personImage`：图像的 URL</span><span class="sxs-lookup"><span data-stu-id="487a5-140">`personImage`: the URL of the image</span></span> | <span data-ttu-id="487a5-141">用于向卡片中添加其他内容的模板。</span><span class="sxs-lookup"><span data-stu-id="487a5-141">The template used to add additional content to the card.</span></span> |

<span data-ttu-id="487a5-142">例如，可以使用模板自定义附加到`mgt-person`组件的组件和模板，以在卡片中添加其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="487a5-142">For example, you can use a template to customize the component attached to the `mgt-person` component and a template to add additional details in the card.</span></span> 

```html
    <mgt-person person-query="me" show-name show-email person-card="hover">
      <template data-type="person-card">
        <mgt-person-card inherit-details>
          <template data-type="additional-details">
            <h3>Stuffed Animal Friends:</h3>
            <ul>
              <li>Giraffe</li>
              <li>lion</li>
              <li>Rabbit</li>
            </ul>
          </template>
        </mgt-person-card>
      </template>
    </mgt-person>

```

## <a name="css-custom-properties"></a><span data-ttu-id="487a5-143">CSS 自定义属性</span><span class="sxs-lookup"><span data-stu-id="487a5-143">CSS custom properties</span></span>

<span data-ttu-id="487a5-144">`mgt-person-card`组件定义以下 CSS 自定义属性。</span><span class="sxs-lookup"><span data-stu-id="487a5-144">The `mgt-person-card` component defines the following CSS custom properties.</span></span>

```css
mgt-person-card {
  --font-size: 14px;
  --font-weight: 600;
  --height: '100%';
  --background-color: transparent;
}
```

<span data-ttu-id="487a5-145">若要了解详细信息，请参阅[样式组件](../style.md)。</span><span class="sxs-lookup"><span data-stu-id="487a5-145">To learn more, see [styling components](../style.md).</span></span>

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="487a5-146">Microsoft Graph 权限</span><span class="sxs-lookup"><span data-stu-id="487a5-146">Microsoft Graph permissions</span></span>

<span data-ttu-id="487a5-147">此组件使用 "[人员" 组件](./person.md)显示用户并继承所有权限。</span><span class="sxs-lookup"><span data-stu-id="487a5-147">This component uses the [Person component](./person.md) to display the user and inherits all permissions.</span></span> 

## <a name="authentication"></a><span data-ttu-id="487a5-148">身份验证</span><span class="sxs-lookup"><span data-stu-id="487a5-148">Authentication</span></span>

<span data-ttu-id="487a5-149">个人卡片控件使用[身份验证文档](./../providers.md)中所述的全局身份验证提供程序。</span><span class="sxs-lookup"><span data-stu-id="487a5-149">The Person-Card control uses the global authentication provider described in the [authentication documentation](./../providers.md).</span></span> 
