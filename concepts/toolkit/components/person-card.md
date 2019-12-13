---
title: Microsoft Graph 工具包中的个人卡片组件
description: "\"个人卡片\" 组件是显示与某个人相关的详细信息的组件。"
localization_priority: Normal
author: vogtn
ms.openlocfilehash: 7f4f20773b152db037d3b57481aa5e8638866f52
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39955867"
---
# <a name="person-card-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="8bc33-103">Microsoft Graph 工具包中的个人卡片组件</span><span class="sxs-lookup"><span data-stu-id="8bc33-103">Person-Card component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="8bc33-104">个人卡片组件是一个响应性组件，用于显示与人员相关的更多信息。</span><span class="sxs-lookup"><span data-stu-id="8bc33-104">A Person-Card component is a responsive component to display more information related to a person.</span></span> <span data-ttu-id="8bc33-105">它通常用作`mgt-person`组件上的浮出控件。</span><span class="sxs-lookup"><span data-stu-id="8bc33-105">It is generally used as a flyout on the `mgt-person` component.</span></span>

<span data-ttu-id="8bc33-106">有关`mgt-person`组件的详细信息，请参阅 "[管理员文档](./person.md)"。</span><span class="sxs-lookup"><span data-stu-id="8bc33-106">For more information about the `mgt-person` component, see [mgt-person docs](./person.md).</span></span>
  
## <a name="example"></a><span data-ttu-id="8bc33-107">示例</span><span class="sxs-lookup"><span data-stu-id="8bc33-107">Example</span></span>

```html
<mgt-person-card person-details="{personObject}" person-image="imgUrl"></mgt-person-card>
```

## <a name="properties"></a><span data-ttu-id="8bc33-108">属性</span><span class="sxs-lookup"><span data-stu-id="8bc33-108">Properties</span></span>

<span data-ttu-id="8bc33-109">组件使用 Microsoft Graph 提供有关用户的其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="8bc33-109">The component uses Microsoft Graph to provide additional details about the user.</span></span> <span data-ttu-id="8bc33-110">若要定义用户，必须使用的`mgt-person`**人员查询**属性。</span><span class="sxs-lookup"><span data-stu-id="8bc33-110">To define a user, you must use the **person-query** property of `mgt-person`.</span></span>

| <span data-ttu-id="8bc33-111">属性</span><span class="sxs-lookup"><span data-stu-id="8bc33-111">Attribute</span></span>         | <span data-ttu-id="8bc33-112">类型</span><span class="sxs-lookup"><span data-stu-id="8bc33-112">Type</span></span>                     | <span data-ttu-id="8bc33-113">说明</span><span class="sxs-lookup"><span data-stu-id="8bc33-113">Description</span></span>                                                                           |
| ---------------- | -------------------------------- | ------------------------------------------------------------------------------------- |
| <span data-ttu-id="8bc33-114">人员-详细信息</span><span class="sxs-lookup"><span data-stu-id="8bc33-114">person-details</span></span> | <span data-ttu-id="8bc33-115">MicrosoftGraph</span><span class="sxs-lookup"><span data-stu-id="8bc33-115">MicrosoftGraph.User</span></span> <br> <span data-ttu-id="8bc33-116">MicrosoftGraph</span><span class="sxs-lookup"><span data-stu-id="8bc33-116">MicrosoftGraph.Person</span></span> <br> <span data-ttu-id="8bc33-117">MicrosoftGraph。联系人</span><span class="sxs-lookup"><span data-stu-id="8bc33-117">MicrosoftGraph.Contact</span></span> | <span data-ttu-id="8bc33-118">由 Microsoft Graph 定义的 Person 对象，包含与用户相关的详细信息。</span><span class="sxs-lookup"><span data-stu-id="8bc33-118">Person object as defined by Microsoft Graph, containing details related to the user.</span></span> |
| <span data-ttu-id="8bc33-119">人员-图像</span><span class="sxs-lookup"><span data-stu-id="8bc33-119">person-image</span></span>   | <span data-ttu-id="8bc33-120">png/jpg/svg</span><span class="sxs-lookup"><span data-stu-id="8bc33-120">png/jpg/svg</span></span>                    | <span data-ttu-id="8bc33-121">与卡片中显示的人员相关的图像。</span><span class="sxs-lookup"><span data-stu-id="8bc33-121">Image related to the person displayed in the card.</span></span>                                   |
| <span data-ttu-id="8bc33-122">继承-详细信息</span><span class="sxs-lookup"><span data-stu-id="8bc33-122">inherit-details</span></span>   | <span data-ttu-id="8bc33-123">无。</span><span class="sxs-lookup"><span data-stu-id="8bc33-123">None.</span></span>                  | <span data-ttu-id="8bc33-124">允许人员卡片遍历父树 for `mgt-person` component 以使用相同`person-details`和`person-image`数据。</span><span class="sxs-lookup"><span data-stu-id="8bc33-124">Allows person-card to walk parent tree for `mgt-person` component to use the same `person-details` and `person-image` data.</span></span>                      |


## <a name="templates"></a><span data-ttu-id="8bc33-125">模板</span><span class="sxs-lookup"><span data-stu-id="8bc33-125">Templates</span></span>

<span data-ttu-id="8bc33-126">人员卡片组件使用允许您添加或替换部分组件的[模板](../templates.md)。</span><span class="sxs-lookup"><span data-stu-id="8bc33-126">The Person-Card component uses [templates](../templates.md) that allow you to add or replace portions of the component.</span></span> <span data-ttu-id="8bc33-127">若要指定模板，请在`<template>`组件内添加一个元素，并将`data-type`值设置为下列值之一。</span><span class="sxs-lookup"><span data-stu-id="8bc33-127">To specify a template, include a `<template>` element inside of a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="8bc33-128">数据类型</span><span class="sxs-lookup"><span data-stu-id="8bc33-128">Data type</span></span> | <span data-ttu-id="8bc33-129">数据上下文</span><span class="sxs-lookup"><span data-stu-id="8bc33-129">Data context</span></span> | <span data-ttu-id="8bc33-130">说明</span><span class="sxs-lookup"><span data-stu-id="8bc33-130">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="8bc33-131">设置</span><span class="sxs-lookup"><span data-stu-id="8bc33-131">default</span></span> | <span data-ttu-id="8bc33-132">`person`： Person details 对象</span><span class="sxs-lookup"><span data-stu-id="8bc33-132">`person`: The person details object</span></span> <br> <span data-ttu-id="8bc33-133">`personImage`：图像的 URL</span><span class="sxs-lookup"><span data-stu-id="8bc33-133">`personImage`: The URL of the image</span></span> | <span data-ttu-id="8bc33-134">默认模板会将整个组件替换为您自己的组件。</span><span class="sxs-lookup"><span data-stu-id="8bc33-134">The default template replaces the entire component with your own.</span></span> |
| <span data-ttu-id="8bc33-135">其他详细信息</span><span class="sxs-lookup"><span data-stu-id="8bc33-135">additional-details</span></span> | <span data-ttu-id="8bc33-136">`person`： Person details 对象</span><span class="sxs-lookup"><span data-stu-id="8bc33-136">`person`: The person details object</span></span> <br> <span data-ttu-id="8bc33-137">`personImage`：图像的 URL</span><span class="sxs-lookup"><span data-stu-id="8bc33-137">`personImage`: the URL of the image</span></span> | <span data-ttu-id="8bc33-138">用于向卡片中添加其他内容的模板。</span><span class="sxs-lookup"><span data-stu-id="8bc33-138">The template used to add additional content to the card.</span></span> |

<span data-ttu-id="8bc33-139">例如，可以使用模板自定义附加到`mgt-person`组件的组件和模板，以在卡片中添加其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="8bc33-139">For example, you can use a template to customize the component attached to the `mgt-person` component and a template to add additional details in the card.</span></span> 

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

## <a name="css-custom-properties"></a><span data-ttu-id="8bc33-140">CSS 自定义属性</span><span class="sxs-lookup"><span data-stu-id="8bc33-140">CSS custom properties</span></span>

<span data-ttu-id="8bc33-141">`mgt-person-card`组件定义以下 CSS 自定义属性。</span><span class="sxs-lookup"><span data-stu-id="8bc33-141">The `mgt-person-card` component defines the following CSS custom properties.</span></span>

```css
mgt-person-card {
  --font-size: 14px;
  --font-weight: 600;
  --height: '100%';
  --background-color: transparent;
}
```

<span data-ttu-id="8bc33-142">若要了解详细信息，请参阅[样式组件](../style.md)。</span><span class="sxs-lookup"><span data-stu-id="8bc33-142">To learn more, see [styling components](../style.md).</span></span>

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="8bc33-143">Microsoft Graph 权限</span><span class="sxs-lookup"><span data-stu-id="8bc33-143">Microsoft Graph permissions</span></span>

<span data-ttu-id="8bc33-144">此组件使用 "[人员" 组件](./person.md)显示用户并继承所有权限。</span><span class="sxs-lookup"><span data-stu-id="8bc33-144">This component uses the [Person component](./person.md) to display the user and inherits all permissions.</span></span> 

## <a name="authentication"></a><span data-ttu-id="8bc33-145">身份验证</span><span class="sxs-lookup"><span data-stu-id="8bc33-145">Authentication</span></span>

<span data-ttu-id="8bc33-146">个人卡片控件使用[身份验证文档](./../providers.md)中所述的全局身份验证提供程序。</span><span class="sxs-lookup"><span data-stu-id="8bc33-146">The Person-Card control uses the global authentication provider described in the [authentication documentation](./../providers.md).</span></span> 
