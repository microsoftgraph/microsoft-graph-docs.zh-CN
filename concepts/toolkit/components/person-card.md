---
title: Microsoft Graph 工具包中的个人卡片组件
description: "\"个人卡片\" 组件是显示与某个人相关的详细信息的组件。"
localization_priority: Normal
author: vogtn
ms.openlocfilehash: 60989eddf28fd421a4cf35fcc6bd9f7433aa9852
ms.sourcegitcommit: 9edfcf99706c8490cd5832a1c706a88a89e24db1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2020
ms.locfileid: "43160308"
---
# <a name="person-card-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="16013-103">Microsoft Graph 工具包中的个人卡片组件</span><span class="sxs-lookup"><span data-stu-id="16013-103">Person-Card component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="16013-104">个人卡片组件是一个响应性组件，用于显示与人员相关的更多信息。</span><span class="sxs-lookup"><span data-stu-id="16013-104">A Person-Card component is a responsive component to display more information related to a person.</span></span> <span data-ttu-id="16013-105">它通常用作`mgt-person`组件上的浮出控件。</span><span class="sxs-lookup"><span data-stu-id="16013-105">It is generally used as a flyout on the `mgt-person` component.</span></span>

<span data-ttu-id="16013-106">有关`mgt-person`组件的详细信息，请参阅 "[管理员文档](./person.md)"。</span><span class="sxs-lookup"><span data-stu-id="16013-106">For more information about the `mgt-person` component, see [mgt-person docs](./person.md).</span></span>

## <a name="example"></a><span data-ttu-id="16013-107">示例</span><span class="sxs-lookup"><span data-stu-id="16013-107">Example</span></span>

<span data-ttu-id="16013-108">下面的示例演示组件与组件的`mgt-person-card`配合`mgt-person`使用。</span><span class="sxs-lookup"><span data-stu-id="16013-108">The following example shows the use of the `mgt-person-card` component with a `mgt-person` component.</span></span> <span data-ttu-id="16013-109">将鼠标悬停在人员上以查看人员卡片，并使用代码编辑器查看[属性](#properties)如何更改组件的行为。</span><span class="sxs-lookup"><span data-stu-id="16013-109">Hover over the person to see the Person Card and use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>
  
<iframe src="https://mgt.dev/iframe.html?id=components-mgt-person-card--person-card-hover&source=docs" height="400"></iframe>

[<span data-ttu-id="16013-110">在 "dev" 中打开此示例</span><span class="sxs-lookup"><span data-stu-id="16013-110">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-person-card--person-card-hover&source=docs)

## <a name="setup-for-teams-integrations"></a><span data-ttu-id="16013-111">团队集成设置</span><span class="sxs-lookup"><span data-stu-id="16013-111">Setup for Teams integrations</span></span>

<span data-ttu-id="16013-112">"人员-卡片" 组件允许用户联系目标人员，包括通过团队聊天。</span><span class="sxs-lookup"><span data-stu-id="16013-112">The Person-Card component allows the user to contact the target person, including via Teams chat.</span></span> <span data-ttu-id="16013-113">如果在团队选项卡应用程序中使用组件，则可以确保组件深度链接直接链接到聊天，而不是通过设置`microsoftTeamsLib`中`TeamsProvider`的打开浏览器窗口。</span><span class="sxs-lookup"><span data-stu-id="16013-113">If using the component inside a Teams tab app, you can ensure that the component deep links directly to chat instead of opening a browser window by setting the `microsoftTeamsLib` in `TeamsProvider`.</span></span>

<span data-ttu-id="16013-114">如果人员卡片组件无法检测到团队库，组件将尝试改为打开团队 web 客户端。</span><span class="sxs-lookup"><span data-stu-id="16013-114">If the Person-Card component is unable to detect the Teams lib, the component will attempt to open the Teams web client instead.</span></span>

```ts
import * as MicrosoftTeams from "@microsoft/teams-js/dist/MicrosoftTeams";
import {TeamsHelper} from '@microsoft/mgt';

TeamsHelper.microsoftTeamsLib = MicrosoftTeams;
```

<span data-ttu-id="16013-115">有关`TeamsProvider`提供程序的详细信息，请参阅[Microsoft 团队提供商](../providers/teams.md)。</span><span class="sxs-lookup"><span data-stu-id="16013-115">For more information about the `TeamsProvider` provider, see [Microsoft Teams provider](../providers/teams.md).</span></span>

## <a name="properties"></a><span data-ttu-id="16013-116">属性</span><span class="sxs-lookup"><span data-stu-id="16013-116">Properties</span></span>

<span data-ttu-id="16013-117">默认情况下， `mgt-person`组件会将人员详细信息传递给`mgt-person-card`组件。</span><span class="sxs-lookup"><span data-stu-id="16013-117">By default, the `mgt-person` component will pass the person details to the `mgt-person-card` component.</span></span> <span data-ttu-id="16013-118">但是，在对`mgt-person`组件进行模板化或使用`mgt-person-card`组件作为独立组件时，可以使用这些属性来更改此属性。</span><span class="sxs-lookup"><span data-stu-id="16013-118">However, you can use these attributes to change this when templating the `mgt-person` component or when using the `mgt-person-card` component as a standalone component.</span></span>

| <span data-ttu-id="16013-119">属性</span><span class="sxs-lookup"><span data-stu-id="16013-119">Attribute</span></span>         | <span data-ttu-id="16013-120">类型</span><span class="sxs-lookup"><span data-stu-id="16013-120">Type</span></span>                     | <span data-ttu-id="16013-121">说明</span><span class="sxs-lookup"><span data-stu-id="16013-121">Description</span></span>                                                                           |
| ---------------- | -------------------------------- | ------------------------------------------------------------------------------------- |
| <span data-ttu-id="16013-122">人员-详细信息</span><span class="sxs-lookup"><span data-stu-id="16013-122">person-details</span></span> | <span data-ttu-id="16013-123">MicrosoftGraph</span><span class="sxs-lookup"><span data-stu-id="16013-123">MicrosoftGraph.User</span></span> <br> <span data-ttu-id="16013-124">MicrosoftGraph</span><span class="sxs-lookup"><span data-stu-id="16013-124">MicrosoftGraph.Person</span></span> <br> <span data-ttu-id="16013-125">MicrosoftGraph。联系人</span><span class="sxs-lookup"><span data-stu-id="16013-125">MicrosoftGraph.Contact</span></span> | <span data-ttu-id="16013-126">由 Microsoft Graph 定义的 Person 对象，包含与用户相关的详细信息。</span><span class="sxs-lookup"><span data-stu-id="16013-126">Person object as defined by Microsoft Graph, containing details related to the user.</span></span> |
| <span data-ttu-id="16013-127">人员-图像</span><span class="sxs-lookup"><span data-stu-id="16013-127">person-image</span></span>   | <span data-ttu-id="16013-128">png/jpg/svg</span><span class="sxs-lookup"><span data-stu-id="16013-128">png/jpg/svg</span></span>                    | <span data-ttu-id="16013-129">与卡片中显示的人员相关的图像。</span><span class="sxs-lookup"><span data-stu-id="16013-129">Image related to the person displayed in the card.</span></span>                                   |
| <span data-ttu-id="16013-130">继承-详细信息</span><span class="sxs-lookup"><span data-stu-id="16013-130">inherit-details</span></span>   | <span data-ttu-id="16013-131">无。</span><span class="sxs-lookup"><span data-stu-id="16013-131">None.</span></span>                  | <span data-ttu-id="16013-132">允许人员卡片遍历父树 for `mgt-person` component 以使用相同`person-details`和`person-image`数据。</span><span class="sxs-lookup"><span data-stu-id="16013-132">Allows person-card to walk parent tree for `mgt-person` component to use the same `person-details` and `person-image` data.</span></span>                      |
| <span data-ttu-id="16013-133">用户 id</span><span class="sxs-lookup"><span data-stu-id="16013-133">user-id</span></span> | <span data-ttu-id="16013-134">string</span><span class="sxs-lookup"><span data-stu-id="16013-134">string</span></span> | <span data-ttu-id="16013-135">允许开发人员提供用户 id 以检索在人员卡片组件上显示的数据</span><span class="sxs-lookup"><span data-stu-id="16013-135">Allows developers to supply user-id to retrive data shown on person-card component</span></span> |
| <span data-ttu-id="16013-136">人员-查询</span><span class="sxs-lookup"><span data-stu-id="16013-136">person-query</span></span> | <span data-ttu-id="16013-137">string</span><span class="sxs-lookup"><span data-stu-id="16013-137">string</span></span> | <span data-ttu-id="16013-138">允许开发人员提供人员查询以检索在人员卡片组件上显示的数据</span><span class="sxs-lookup"><span data-stu-id="16013-138">Allows developers to supply person-query to retrive data shown on person-card component</span></span> |


## <a name="templates"></a><span data-ttu-id="16013-139">模板</span><span class="sxs-lookup"><span data-stu-id="16013-139">Templates</span></span>

<span data-ttu-id="16013-140">人员卡片组件使用允许您添加或替换部分组件的[模板](../templates.md)。</span><span class="sxs-lookup"><span data-stu-id="16013-140">The Person-Card component uses [templates](../templates.md) that allow you to add or replace portions of the component.</span></span> <span data-ttu-id="16013-141">若要指定模板，请在`<template>`组件内添加一个元素，并将`data-type`值设置为下列值之一。</span><span class="sxs-lookup"><span data-stu-id="16013-141">To specify a template, include a `<template>` element inside of a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="16013-142">数据类型</span><span class="sxs-lookup"><span data-stu-id="16013-142">Data type</span></span> | <span data-ttu-id="16013-143">数据上下文</span><span class="sxs-lookup"><span data-stu-id="16013-143">Data context</span></span> | <span data-ttu-id="16013-144">说明</span><span class="sxs-lookup"><span data-stu-id="16013-144">Description</span></span> |
| - | - | - |
| <span data-ttu-id="16013-145">无数据</span><span class="sxs-lookup"><span data-stu-id="16013-145">no-data</span></span> | <span data-ttu-id="16013-146">空</span><span class="sxs-lookup"><span data-stu-id="16013-146">null</span></span> | <span data-ttu-id="16013-147">没有可用数据时使用的模板。</span><span class="sxs-lookup"><span data-stu-id="16013-147">The template used when no data is available.</span></span>
| <span data-ttu-id="16013-148">设置</span><span class="sxs-lookup"><span data-stu-id="16013-148">default</span></span> | <span data-ttu-id="16013-149">`person`： Person details 对象</span><span class="sxs-lookup"><span data-stu-id="16013-149">`person`: The person details object</span></span> <br> <span data-ttu-id="16013-150">`personImage`：图像的 URL</span><span class="sxs-lookup"><span data-stu-id="16013-150">`personImage`: The URL of the image</span></span> | <span data-ttu-id="16013-151">默认模板会将整个组件替换为您自己的组件。</span><span class="sxs-lookup"><span data-stu-id="16013-151">The default template replaces the entire component with your own.</span></span> |
| <span data-ttu-id="16013-152">人员-详细信息</span><span class="sxs-lookup"><span data-stu-id="16013-152">person-details</span></span> | <span data-ttu-id="16013-153">`person`： Person details 对象</span><span class="sxs-lookup"><span data-stu-id="16013-153">`person`: The person details object</span></span> | <span data-ttu-id="16013-154">用于呈现个人卡片顶部部分的模板。</span><span class="sxs-lookup"><span data-stu-id="16013-154">The template used to render the top part of the person card.</span></span> |
| <span data-ttu-id="16013-155">联系人-详细信息</span><span class="sxs-lookup"><span data-stu-id="16013-155">contact-details</span></span> | <span data-ttu-id="16013-156">`person`： Person details 对象</span><span class="sxs-lookup"><span data-stu-id="16013-156">`person`: The person details object</span></span> | <span data-ttu-id="16013-157">用于替代其他详细信息容器的联系人详细信息部分的模板。</span><span class="sxs-lookup"><span data-stu-id="16013-157">The template used to override the contact details part of the additional details container.</span></span> |
| <span data-ttu-id="16013-158">其他详细信息</span><span class="sxs-lookup"><span data-stu-id="16013-158">additional-details</span></span> | <span data-ttu-id="16013-159">`person`： Person details 对象</span><span class="sxs-lookup"><span data-stu-id="16013-159">`person`: The person details object</span></span> <br> <span data-ttu-id="16013-160">`personImage`：图像的 URL</span><span class="sxs-lookup"><span data-stu-id="16013-160">`personImage`: the URL of the image</span></span> | <span data-ttu-id="16013-161">用于将自定义内容添加到其他详细信息容器的模板。</span><span class="sxs-lookup"><span data-stu-id="16013-161">The template used to add custom content to the additional details container.</span></span> |

<span data-ttu-id="16013-162">例如，可以使用模板自定义附加到`mgt-person`组件的组件和模板，以在卡片中添加其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="16013-162">For example, you can use a template to customize the component attached to the `mgt-person` component and a template to add additional details in the card.</span></span> 

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

## <a name="css-custom-properties"></a><span data-ttu-id="16013-163">CSS 自定义属性</span><span class="sxs-lookup"><span data-stu-id="16013-163">CSS custom properties</span></span>

<span data-ttu-id="16013-164">`mgt-person-card`组件定义以下 CSS 自定义属性。</span><span class="sxs-lookup"><span data-stu-id="16013-164">The `mgt-person-card` component defines the following CSS custom properties.</span></span> <span data-ttu-id="16013-165">若要使用这些属性，必须将选择器定义为父`mgt-person`元素。</span><span class="sxs-lookup"><span data-stu-id="16013-165">To use these properties, you must define the selector as the parent `mgt-person` element.</span></span> 

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

<span data-ttu-id="16013-166">若要了解详细信息，请参阅[样式组件](../style.md)。</span><span class="sxs-lookup"><span data-stu-id="16013-166">To learn more, see [styling components](../style.md).</span></span>

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="16013-167">Microsoft Graph 权限</span><span class="sxs-lookup"><span data-stu-id="16013-167">Microsoft Graph permissions</span></span>

<span data-ttu-id="16013-168">此组件使用 "[人员" 组件](./person.md)显示用户并继承所有权限。</span><span class="sxs-lookup"><span data-stu-id="16013-168">This component uses the [Person component](./person.md) to display the user and inherits all permissions.</span></span> 

## <a name="authentication"></a><span data-ttu-id="16013-169">身份验证</span><span class="sxs-lookup"><span data-stu-id="16013-169">Authentication</span></span>

<span data-ttu-id="16013-170">个人卡片控件使用[身份验证文档](./../providers.md)中所述的全局身份验证提供程序。</span><span class="sxs-lookup"><span data-stu-id="16013-170">The Person-Card control uses the global authentication provider described in the [authentication documentation](./../providers.md).</span></span> 

## <a name="extend-for-more-control"></a><span data-ttu-id="16013-171">扩展以实现更多控制</span><span class="sxs-lookup"><span data-stu-id="16013-171">Extend for more control</span></span>

<span data-ttu-id="16013-172">对于更复杂的方案或真正的自定义 UX，此组件`protected render*`将公开几种用于在组件扩展中进行重写的方法。</span><span class="sxs-lookup"><span data-stu-id="16013-172">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions.</span></span>

| <span data-ttu-id="16013-173">方法</span><span class="sxs-lookup"><span data-stu-id="16013-173">Method</span></span> | <span data-ttu-id="16013-174">说明</span><span class="sxs-lookup"><span data-stu-id="16013-174">Description</span></span> |
| - | - |
| <span data-ttu-id="16013-175">renderNoData</span><span class="sxs-lookup"><span data-stu-id="16013-175">renderNoData</span></span> | <span data-ttu-id="16013-176">在无人数据可用时呈现状态。</span><span class="sxs-lookup"><span data-stu-id="16013-176">Renders a state when no person data is available.</span></span> | 
| <span data-ttu-id="16013-177">renderPersonDetails</span><span class="sxs-lookup"><span data-stu-id="16013-177">renderPersonDetails</span></span> | <span data-ttu-id="16013-178">呈现人员卡片的主要正文（图像、名称、图标）。</span><span class="sxs-lookup"><span data-stu-id="16013-178">Renders the main body of the person card (image, name, icons).</span></span> |
| <span data-ttu-id="16013-179">renderPersonImage</span><span class="sxs-lookup"><span data-stu-id="16013-179">renderPersonImage</span></span> | <span data-ttu-id="16013-180">呈现人员详细信息的图像部分。</span><span class="sxs-lookup"><span data-stu-id="16013-180">Renders the image part of the person details.</span></span> |
| <span data-ttu-id="16013-181">renderPersonName</span><span class="sxs-lookup"><span data-stu-id="16013-181">renderPersonName</span></span> | <span data-ttu-id="16013-182">呈现人员详细信息的名称部分。</span><span class="sxs-lookup"><span data-stu-id="16013-182">Renders the name part of the person details.</span></span> |
| <span data-ttu-id="16013-183">renderPersonTitle</span><span class="sxs-lookup"><span data-stu-id="16013-183">renderPersonTitle</span></span> | <span data-ttu-id="16013-184">呈现人员详细信息的标题部分。</span><span class="sxs-lookup"><span data-stu-id="16013-184">Renders the title part of the person details.</span></span> |
| <span data-ttu-id="16013-185">renderPersonSubtitle</span><span class="sxs-lookup"><span data-stu-id="16013-185">renderPersonSubtitle</span></span> | <span data-ttu-id="16013-186">呈现人员详细信息的副标题部分。</span><span class="sxs-lookup"><span data-stu-id="16013-186">Renders the subtitle part of the person details.</span></span> |
| <span data-ttu-id="16013-187">renderContactIcons</span><span class="sxs-lookup"><span data-stu-id="16013-187">renderContactIcons</span></span> | <span data-ttu-id="16013-188">呈现 "人员详细信息" 的 "联系人" 图标部分。</span><span class="sxs-lookup"><span data-stu-id="16013-188">Renders the contact icons part of the person details.</span></span> |
| <span data-ttu-id="16013-189">renderExpandedDetailsButton</span><span class="sxs-lookup"><span data-stu-id="16013-189">renderExpandedDetailsButton</span></span> | <span data-ttu-id="16013-190">呈现按钮以显示展开的详细信息。</span><span class="sxs-lookup"><span data-stu-id="16013-190">Renders the button to show the expanded details.</span></span> |
| <span data-ttu-id="16013-191">renderExpandedDetails</span><span class="sxs-lookup"><span data-stu-id="16013-191">renderExpandedDetails</span></span> | <span data-ttu-id="16013-192">在展开的详细信息容器中呈现内容。</span><span class="sxs-lookup"><span data-stu-id="16013-192">Renders the content in the expanded details container.</span></span> |
| <span data-ttu-id="16013-193">renderContactDetails</span><span class="sxs-lookup"><span data-stu-id="16013-193">renderContactDetails</span></span> | <span data-ttu-id="16013-194">呈现展开的详细信息的 "联系人详细信息" 部分。</span><span class="sxs-lookup"><span data-stu-id="16013-194">Renders the contact details part of the expanded details.</span></span> |
| <span data-ttu-id="16013-195">renderAdditionalDetails</span><span class="sxs-lookup"><span data-stu-id="16013-195">renderAdditionalDetails</span></span> | <span data-ttu-id="16013-196">呈现展开的详细信息的其他详细信息部分。</span><span class="sxs-lookup"><span data-stu-id="16013-196">Renders the additional details part of the expanded details.</span></span> |
