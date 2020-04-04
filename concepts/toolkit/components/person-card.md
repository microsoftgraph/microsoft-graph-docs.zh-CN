---
title: Microsoft Graph 工具包中的个人卡片组件
description: "\"个人卡片\" 组件是显示与某个人相关的详细信息的组件。"
localization_priority: Normal
author: vogtn
ms.openlocfilehash: 3d440f1340f9ee3f40c37538b1befcacd9867dc1
ms.sourcegitcommit: 1bc5a0c179dce57e90349610566fb86e1b5fbf95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/04/2020
ms.locfileid: "43144287"
---
# <a name="person-card-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="a9c9c-103">Microsoft Graph 工具包中的个人卡片组件</span><span class="sxs-lookup"><span data-stu-id="a9c9c-103">Person-Card component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="a9c9c-104">个人卡片组件是一个响应性组件，用于显示与人员相关的更多信息。</span><span class="sxs-lookup"><span data-stu-id="a9c9c-104">A Person-Card component is a responsive component to display more information related to a person.</span></span> <span data-ttu-id="a9c9c-105">它通常用作`mgt-person`组件上的浮出控件。</span><span class="sxs-lookup"><span data-stu-id="a9c9c-105">It is generally used as a flyout on the `mgt-person` component.</span></span>

<span data-ttu-id="a9c9c-106">有关`mgt-person`组件的详细信息，请参阅 "[管理员文档](./person.md)"。</span><span class="sxs-lookup"><span data-stu-id="a9c9c-106">For more information about the `mgt-person` component, see [mgt-person docs](./person.md).</span></span>

## <a name="example"></a><span data-ttu-id="a9c9c-107">示例</span><span class="sxs-lookup"><span data-stu-id="a9c9c-107">Example</span></span>

<span data-ttu-id="a9c9c-108">下面的示例演示组件与组件的`mgt-person-card`配合`mgt-person`使用。</span><span class="sxs-lookup"><span data-stu-id="a9c9c-108">The following example shows the use of the `mgt-person-card` component with a `mgt-person` component.</span></span> <span data-ttu-id="a9c9c-109">将鼠标悬停在人员上以查看人员卡片，并使用代码编辑器查看[属性](#properties)如何更改组件的行为。</span><span class="sxs-lookup"><span data-stu-id="a9c9c-109">Hover over the person to see the Person Card and use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>
  
<iframe src="https://mgt.dev/iframe.html?id=components-mgt-person-card--person-card-hover&source=docs" height="400"></iframe>

[<span data-ttu-id="a9c9c-110">在 "dev" 中打开此示例</span><span class="sxs-lookup"><span data-stu-id="a9c9c-110">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-person-card--person-card-hover&source=docs)

## <a name="setup-for-teams-integrations"></a><span data-ttu-id="a9c9c-111">团队集成设置</span><span class="sxs-lookup"><span data-stu-id="a9c9c-111">Setup for Teams integrations</span></span>

<span data-ttu-id="a9c9c-112">"人员-卡片" 组件允许用户联系目标人员，包括通过团队聊天。</span><span class="sxs-lookup"><span data-stu-id="a9c9c-112">The Person-Card component allows the user to contact the target person, including via Teams chat.</span></span> <span data-ttu-id="a9c9c-113">如果在团队选项卡应用程序中使用组件，则可以确保组件深度链接直接链接到聊天，而不是通过设置`microsoftTeamsLib`中`TeamsProvider`的打开浏览器窗口。</span><span class="sxs-lookup"><span data-stu-id="a9c9c-113">If using the component inside a Teams tab app, you can ensure that the component deep links directly to chat instead of opening a browser window by setting the `microsoftTeamsLib` in `TeamsProvider`.</span></span>

<span data-ttu-id="a9c9c-114">如果人员卡片组件无法检测到团队库，组件将尝试改为打开团队 web 客户端。</span><span class="sxs-lookup"><span data-stu-id="a9c9c-114">If the Person-Card component is unable to detect the Teams lib, the component will attempt to open the Teams web client instead.</span></span>

```ts
import * as MicrosoftTeams from "@microsoft/teams-js/dist/MicrosoftTeams";
import {TeamsHelper} from '@microsoft/mgt';

TeamsHelper.microsoftTeamsLib = MicrosoftTeams;
```

<span data-ttu-id="a9c9c-115">有关`TeamsProvider`提供程序的详细信息，请参阅[Microsoft 团队提供商](../providers/teams.md)。</span><span class="sxs-lookup"><span data-stu-id="a9c9c-115">For more information about the `TeamsProvider` provider, see [Microsoft Teams provider](../providers/teams.md).</span></span>

## <a name="properties"></a><span data-ttu-id="a9c9c-116">属性</span><span class="sxs-lookup"><span data-stu-id="a9c9c-116">Properties</span></span>

<span data-ttu-id="a9c9c-117">组件使用 Microsoft Graph 提供有关用户的其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="a9c9c-117">The component uses Microsoft Graph to provide additional details about the user.</span></span> <span data-ttu-id="a9c9c-118">若要定义用户，必须使用的`mgt-person`**人员查询**属性。</span><span class="sxs-lookup"><span data-stu-id="a9c9c-118">To define a user, you must use the **person-query** property of `mgt-person`.</span></span>

| <span data-ttu-id="a9c9c-119">属性</span><span class="sxs-lookup"><span data-stu-id="a9c9c-119">Attribute</span></span>         | <span data-ttu-id="a9c9c-120">类型</span><span class="sxs-lookup"><span data-stu-id="a9c9c-120">Type</span></span>                     | <span data-ttu-id="a9c9c-121">说明</span><span class="sxs-lookup"><span data-stu-id="a9c9c-121">Description</span></span>                                                                           |
| ---------------- | -------------------------------- | ------------------------------------------------------------------------------------- |
| <span data-ttu-id="a9c9c-122">人员-详细信息</span><span class="sxs-lookup"><span data-stu-id="a9c9c-122">person-details</span></span> | <span data-ttu-id="a9c9c-123">MicrosoftGraph</span><span class="sxs-lookup"><span data-stu-id="a9c9c-123">MicrosoftGraph.User</span></span> <br> <span data-ttu-id="a9c9c-124">MicrosoftGraph</span><span class="sxs-lookup"><span data-stu-id="a9c9c-124">MicrosoftGraph.Person</span></span> <br> <span data-ttu-id="a9c9c-125">MicrosoftGraph。联系人</span><span class="sxs-lookup"><span data-stu-id="a9c9c-125">MicrosoftGraph.Contact</span></span> | <span data-ttu-id="a9c9c-126">由 Microsoft Graph 定义的 Person 对象，包含与用户相关的详细信息。</span><span class="sxs-lookup"><span data-stu-id="a9c9c-126">Person object as defined by Microsoft Graph, containing details related to the user.</span></span> |
| <span data-ttu-id="a9c9c-127">人员-图像</span><span class="sxs-lookup"><span data-stu-id="a9c9c-127">person-image</span></span>   | <span data-ttu-id="a9c9c-128">png/jpg/svg</span><span class="sxs-lookup"><span data-stu-id="a9c9c-128">png/jpg/svg</span></span>                    | <span data-ttu-id="a9c9c-129">与卡片中显示的人员相关的图像。</span><span class="sxs-lookup"><span data-stu-id="a9c9c-129">Image related to the person displayed in the card.</span></span>                                   |
| <span data-ttu-id="a9c9c-130">继承-详细信息</span><span class="sxs-lookup"><span data-stu-id="a9c9c-130">inherit-details</span></span>   | <span data-ttu-id="a9c9c-131">无。</span><span class="sxs-lookup"><span data-stu-id="a9c9c-131">None.</span></span>                  | <span data-ttu-id="a9c9c-132">允许人员卡片遍历父树 for `mgt-person` component 以使用相同`person-details`和`person-image`数据。</span><span class="sxs-lookup"><span data-stu-id="a9c9c-132">Allows person-card to walk parent tree for `mgt-person` component to use the same `person-details` and `person-image` data.</span></span>                      |


## <a name="templates"></a><span data-ttu-id="a9c9c-133">模板</span><span class="sxs-lookup"><span data-stu-id="a9c9c-133">Templates</span></span>

<span data-ttu-id="a9c9c-134">人员卡片组件使用允许您添加或替换部分组件的[模板](../templates.md)。</span><span class="sxs-lookup"><span data-stu-id="a9c9c-134">The Person-Card component uses [templates](../templates.md) that allow you to add or replace portions of the component.</span></span> <span data-ttu-id="a9c9c-135">若要指定模板，请在`<template>`组件内添加一个元素，并将`data-type`值设置为下列值之一。</span><span class="sxs-lookup"><span data-stu-id="a9c9c-135">To specify a template, include a `<template>` element inside of a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="a9c9c-136">数据类型</span><span class="sxs-lookup"><span data-stu-id="a9c9c-136">Data type</span></span> | <span data-ttu-id="a9c9c-137">数据上下文</span><span class="sxs-lookup"><span data-stu-id="a9c9c-137">Data context</span></span> | <span data-ttu-id="a9c9c-138">说明</span><span class="sxs-lookup"><span data-stu-id="a9c9c-138">Description</span></span> |
| - | - | - |
| <span data-ttu-id="a9c9c-139">无数据</span><span class="sxs-lookup"><span data-stu-id="a9c9c-139">no-data</span></span> | <span data-ttu-id="a9c9c-140">空</span><span class="sxs-lookup"><span data-stu-id="a9c9c-140">null</span></span> | <span data-ttu-id="a9c9c-141">没有可用数据时使用的模板。</span><span class="sxs-lookup"><span data-stu-id="a9c9c-141">The template used when no data is available.</span></span>
| <span data-ttu-id="a9c9c-142">设置</span><span class="sxs-lookup"><span data-stu-id="a9c9c-142">default</span></span> | <span data-ttu-id="a9c9c-143">`person`： Person details 对象</span><span class="sxs-lookup"><span data-stu-id="a9c9c-143">`person`: The person details object</span></span> <br> <span data-ttu-id="a9c9c-144">`personImage`：图像的 URL</span><span class="sxs-lookup"><span data-stu-id="a9c9c-144">`personImage`: The URL of the image</span></span> | <span data-ttu-id="a9c9c-145">默认模板会将整个组件替换为您自己的组件。</span><span class="sxs-lookup"><span data-stu-id="a9c9c-145">The default template replaces the entire component with your own.</span></span> |
| <span data-ttu-id="a9c9c-146">人员-详细信息</span><span class="sxs-lookup"><span data-stu-id="a9c9c-146">person-details</span></span> | <span data-ttu-id="a9c9c-147">`person`： Person details 对象</span><span class="sxs-lookup"><span data-stu-id="a9c9c-147">`person`: The person details object</span></span> | <span data-ttu-id="a9c9c-148">用于呈现个人卡片顶部部分的模板。</span><span class="sxs-lookup"><span data-stu-id="a9c9c-148">The template used to render the top part of the person card.</span></span> |
| <span data-ttu-id="a9c9c-149">联系人-详细信息</span><span class="sxs-lookup"><span data-stu-id="a9c9c-149">contact-details</span></span> | <span data-ttu-id="a9c9c-150">`person`： Person details 对象</span><span class="sxs-lookup"><span data-stu-id="a9c9c-150">`person`: The person details object</span></span> | <span data-ttu-id="a9c9c-151">用于替代其他详细信息容器的联系人详细信息部分的模板。</span><span class="sxs-lookup"><span data-stu-id="a9c9c-151">The template used to override the contact details part of the additional details container.</span></span> |
| <span data-ttu-id="a9c9c-152">其他详细信息</span><span class="sxs-lookup"><span data-stu-id="a9c9c-152">additional-details</span></span> | <span data-ttu-id="a9c9c-153">`person`： Person details 对象</span><span class="sxs-lookup"><span data-stu-id="a9c9c-153">`person`: The person details object</span></span> <br> <span data-ttu-id="a9c9c-154">`personImage`：图像的 URL</span><span class="sxs-lookup"><span data-stu-id="a9c9c-154">`personImage`: the URL of the image</span></span> | <span data-ttu-id="a9c9c-155">用于将自定义内容添加到其他详细信息容器的模板。</span><span class="sxs-lookup"><span data-stu-id="a9c9c-155">The template used to add custom content to the additional details container.</span></span> |

<span data-ttu-id="a9c9c-156">例如，可以使用模板自定义附加到`mgt-person`组件的组件和模板，以在卡片中添加其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="a9c9c-156">For example, you can use a template to customize the component attached to the `mgt-person` component and a template to add additional details in the card.</span></span> 

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

## <a name="css-custom-properties"></a><span data-ttu-id="a9c9c-157">CSS 自定义属性</span><span class="sxs-lookup"><span data-stu-id="a9c9c-157">CSS custom properties</span></span>

<span data-ttu-id="a9c9c-158">`mgt-person-card`组件定义以下 CSS 自定义属性。</span><span class="sxs-lookup"><span data-stu-id="a9c9c-158">The `mgt-person-card` component defines the following CSS custom properties.</span></span> <span data-ttu-id="a9c9c-159">若要使用这些属性，必须将选择器定义为父`mgt-person`元素。</span><span class="sxs-lookup"><span data-stu-id="a9c9c-159">To use these properties, you must define the selector as the parent `mgt-person` element.</span></span> 

```css
mgt-person {
  --person-card-display-name-font-size: 40px;
  --person-card-display-name-color: #ffffff;
  --person-card-title-font-size: 20px;
  --person-card-title-color: #ffffff;
  --person-card-subtitle-font-size: 10px;
  --person-card-subtitle-color: #ffffff;
  --person-card-details-title-font-size: 10px;
  --person-card-details-title-color: #b3bf0a;
  --person-card-details-item-font-size: 20px;
  --person-card-details-item-color: #3abf0a;
  --person-card-background-color: #000000;
}
```

<span data-ttu-id="a9c9c-160">若要了解详细信息，请参阅[样式组件](../style.md)。</span><span class="sxs-lookup"><span data-stu-id="a9c9c-160">To learn more, see [styling components](../style.md).</span></span>

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="a9c9c-161">Microsoft Graph 权限</span><span class="sxs-lookup"><span data-stu-id="a9c9c-161">Microsoft Graph permissions</span></span>

<span data-ttu-id="a9c9c-162">此组件使用 "[人员" 组件](./person.md)显示用户并继承所有权限。</span><span class="sxs-lookup"><span data-stu-id="a9c9c-162">This component uses the [Person component](./person.md) to display the user and inherits all permissions.</span></span> 

## <a name="authentication"></a><span data-ttu-id="a9c9c-163">身份验证</span><span class="sxs-lookup"><span data-stu-id="a9c9c-163">Authentication</span></span>

<span data-ttu-id="a9c9c-164">个人卡片控件使用[身份验证文档](./../providers.md)中所述的全局身份验证提供程序。</span><span class="sxs-lookup"><span data-stu-id="a9c9c-164">The Person-Card control uses the global authentication provider described in the [authentication documentation](./../providers.md).</span></span> 

## <a name="extend-for-more-control"></a><span data-ttu-id="a9c9c-165">扩展以实现更多控制</span><span class="sxs-lookup"><span data-stu-id="a9c9c-165">Extend for more control</span></span>

<span data-ttu-id="a9c9c-166">对于更复杂的方案或真正的自定义 UX，此组件`protected render*`将公开几种用于在组件扩展中进行重写的方法。</span><span class="sxs-lookup"><span data-stu-id="a9c9c-166">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions.</span></span>

| <span data-ttu-id="a9c9c-167">方法</span><span class="sxs-lookup"><span data-stu-id="a9c9c-167">Method</span></span> | <span data-ttu-id="a9c9c-168">说明</span><span class="sxs-lookup"><span data-stu-id="a9c9c-168">Description</span></span> |
| - | - |
| <span data-ttu-id="a9c9c-169">renderNoData</span><span class="sxs-lookup"><span data-stu-id="a9c9c-169">renderNoData</span></span> | <span data-ttu-id="a9c9c-170">在无人数据可用时呈现状态。</span><span class="sxs-lookup"><span data-stu-id="a9c9c-170">Renders a state when no person data is available.</span></span> | 
| <span data-ttu-id="a9c9c-171">renderPersonDetails</span><span class="sxs-lookup"><span data-stu-id="a9c9c-171">renderPersonDetails</span></span> | <span data-ttu-id="a9c9c-172">呈现人员卡片的主要正文（图像、名称、图标）。</span><span class="sxs-lookup"><span data-stu-id="a9c9c-172">Renders the main body of the person card (image, name, icons).</span></span> |
| <span data-ttu-id="a9c9c-173">renderPersonImage</span><span class="sxs-lookup"><span data-stu-id="a9c9c-173">renderPersonImage</span></span> | <span data-ttu-id="a9c9c-174">呈现人员详细信息的图像部分。</span><span class="sxs-lookup"><span data-stu-id="a9c9c-174">Renders the image part of the person details.</span></span> |
| <span data-ttu-id="a9c9c-175">renderPersonName</span><span class="sxs-lookup"><span data-stu-id="a9c9c-175">renderPersonName</span></span> | <span data-ttu-id="a9c9c-176">呈现人员详细信息的名称部分。</span><span class="sxs-lookup"><span data-stu-id="a9c9c-176">Renders the name part of the person details.</span></span> |
| <span data-ttu-id="a9c9c-177">renderPersonTitle</span><span class="sxs-lookup"><span data-stu-id="a9c9c-177">renderPersonTitle</span></span> | <span data-ttu-id="a9c9c-178">呈现人员详细信息的标题部分。</span><span class="sxs-lookup"><span data-stu-id="a9c9c-178">Renders the title part of the person details.</span></span> |
| <span data-ttu-id="a9c9c-179">renderPersonSubtitle</span><span class="sxs-lookup"><span data-stu-id="a9c9c-179">renderPersonSubtitle</span></span> | <span data-ttu-id="a9c9c-180">呈现人员详细信息的副标题部分。</span><span class="sxs-lookup"><span data-stu-id="a9c9c-180">Renders the subtitle part of the person details.</span></span> |
| <span data-ttu-id="a9c9c-181">renderContactIcons</span><span class="sxs-lookup"><span data-stu-id="a9c9c-181">renderContactIcons</span></span> | <span data-ttu-id="a9c9c-182">呈现 "人员详细信息" 的 "联系人" 图标部分。</span><span class="sxs-lookup"><span data-stu-id="a9c9c-182">Renders the contact icons part of the person details.</span></span> |
| <span data-ttu-id="a9c9c-183">renderExpandedDetailsButton</span><span class="sxs-lookup"><span data-stu-id="a9c9c-183">renderExpandedDetailsButton</span></span> | <span data-ttu-id="a9c9c-184">呈现按钮以显示展开的详细信息。</span><span class="sxs-lookup"><span data-stu-id="a9c9c-184">Renders the button to show the expanded details.</span></span> |
| <span data-ttu-id="a9c9c-185">renderExpandedDetails</span><span class="sxs-lookup"><span data-stu-id="a9c9c-185">renderExpandedDetails</span></span> | <span data-ttu-id="a9c9c-186">在展开的详细信息容器中呈现内容。</span><span class="sxs-lookup"><span data-stu-id="a9c9c-186">Renders the content in the expanded details container.</span></span> |
| <span data-ttu-id="a9c9c-187">renderContactDetails</span><span class="sxs-lookup"><span data-stu-id="a9c9c-187">renderContactDetails</span></span> | <span data-ttu-id="a9c9c-188">呈现展开的详细信息的 "联系人详细信息" 部分。</span><span class="sxs-lookup"><span data-stu-id="a9c9c-188">Renders the contact details part of the expanded details.</span></span> |
| <span data-ttu-id="a9c9c-189">renderAdditionalDetails</span><span class="sxs-lookup"><span data-stu-id="a9c9c-189">renderAdditionalDetails</span></span> | <span data-ttu-id="a9c9c-190">呈现展开的详细信息的其他详细信息部分。</span><span class="sxs-lookup"><span data-stu-id="a9c9c-190">Renders the additional details part of the expanded details.</span></span> |

