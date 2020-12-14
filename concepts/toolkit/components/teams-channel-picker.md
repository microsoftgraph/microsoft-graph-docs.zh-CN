---
title: Microsoft Graph 中 Microsoft Teams 频道选取器Toolkit
description: 可以使用 mgt-teams-channel-picker 从 Microsoft Graph 搜索与用户关联的频道和团队。
localization_priority: Normal
author: vogtn
ms.openlocfilehash: c0b6e818f0c9c30314b5342fcfb6ef44978ec830
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49660006"
---
# <a name="microsoft-teams-channel-picker-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="a8071-103">Microsoft Graph 中 Microsoft Teams 频道选取器Toolkit</span><span class="sxs-lookup"><span data-stu-id="a8071-103">Microsoft Teams Channel Picker component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="a8071-104">可以使用该组件 `mgt-teams-channel-picker` 启用与用户关联的 Microsoft Teams 频道的搜索。</span><span class="sxs-lookup"><span data-stu-id="a8071-104">A you can use the `mgt-teams-channel-picker` component to enable searches for Microsoft Teams channels associated with a user.</span></span> <span data-ttu-id="a8071-105">组件可以搜索用户已加入的所有团队，以及这些团队中的每个频道。</span><span class="sxs-lookup"><span data-stu-id="a8071-105">The component can search all teams the user has joined, and each channel in those teams.</span></span> 

## <a name="example"></a><span data-ttu-id="a8071-106">示例</span><span class="sxs-lookup"><span data-stu-id="a8071-106">Example</span></span>

<span data-ttu-id="a8071-107">以下示例显示 `mgt-teams-channel-picker` 组件。</span><span class="sxs-lookup"><span data-stu-id="a8071-107">The following example shows the `mgt-teams-channel-picker` component.</span></span> <span data-ttu-id="a8071-108">开始搜索频道或团队以查看结果呈现。</span><span class="sxs-lookup"><span data-stu-id="a8071-108">Start searching for a channel or team to see the results render.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-teams-channel-picker--teams-channel-picker&source=docs" height="450"></iframe>

[<span data-ttu-id="a8071-109">在 mgt.dev 中打开此示例</span><span class="sxs-lookup"><span data-stu-id="a8071-109">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-teams-channel-picker--teams-channel-picker&source=docs)

## <a name="getting-the-selected-channel"></a><span data-ttu-id="a8071-110">获取所选频道</span><span class="sxs-lookup"><span data-stu-id="a8071-110">Getting the selected channel</span></span>

<span data-ttu-id="a8071-111">使用 `selectedItem` 该属性可检索当前选定的频道和父团队。</span><span class="sxs-lookup"><span data-stu-id="a8071-111">Use the `selectedItem` property to retrieve the currently selected channel and parent team.</span></span> <span data-ttu-id="a8071-112">如果未选择任何通道，则此值将为 null。</span><span class="sxs-lookup"><span data-stu-id="a8071-112">This value will be null if no channel has been selected.</span></span> <span data-ttu-id="a8071-113">`selectedItem` 包含两个 `channel` 属性： ([MicrosoftGraph.Channel](/graph/api/resources/channel)) 和 `team` ([MicrosoftGraph.Team](/graph/api/resources/team)) 。</span><span class="sxs-lookup"><span data-stu-id="a8071-113">`selectedItem` contains two properties: `channel` ([MicrosoftGraph.Channel](/graph/api/resources/channel)) and `team` ([MicrosoftGraph.Team](/graph/api/resources/team)).</span></span>

```javascript
const channelPicker = document.querySelector('mgt-teams-channel-picker');
console.log(channelPicker.selectedItem.channel);
console.log(channelPicker.selectedItem.team);
```

## <a name="selecting-a-channel"></a><span data-ttu-id="a8071-114">选择频道</span><span class="sxs-lookup"><span data-stu-id="a8071-114">Selecting a channel</span></span>

<span data-ttu-id="a8071-115">使用此方法 `selectChannelById(channelId: string)` 以编程方式选择频道。</span><span class="sxs-lookup"><span data-stu-id="a8071-115">Use the `selectChannelById(channelId: string)` method to programmatically select a channel.</span></span>

> <span data-ttu-id="a8071-116">**注意：Teams** 频道选取器仅支持单个频道选择。</span><span class="sxs-lookup"><span data-stu-id="a8071-116">**Note:** the Teams channel picker only supports single channel selection.</span></span>

```javascript
const channelPicker = document.querySelector('mgt-teams-channel-picker');
const channelId = 'some-channel-id';
channelPicker.selectChannelById(channelId);
```

> <span data-ttu-id="a8071-117">**注意：** 提供的频道 (和后续 ID) 必须属于经过身份验证的用户已加入的团队。</span><span class="sxs-lookup"><span data-stu-id="a8071-117">**Note:** The provided channel (and subsequent ID) must belong to a team that the authenticated user has joined.</span></span> 


## <a name="css-custom-properties"></a><span data-ttu-id="a8071-118">CSS 自定义属性</span><span class="sxs-lookup"><span data-stu-id="a8071-118">CSS custom properties</span></span>

<span data-ttu-id="a8071-119">该 `mgt-teams-channel-picker` 组件定义以下 CSS 自定义属性。</span><span class="sxs-lookup"><span data-stu-id="a8071-119">The `mgt-teams-channel-picker` component defines the following CSS custom properties.</span></span>

```css
mgt-teams-channel-picker {
    --input-border: 2px rgba(255, 255, 255, 0.5) solid; /* sets all input area border */

      /* OR individual input border sides */
    --input-border-bottom: 2px rgba(255, 255, 255, 0.5) solid;
    --input-border-right: 2px rgba(255, 255, 255, 0.5) solid;
    --input-border-left: 2px rgba(255, 255, 255, 0.5) solid;
    --input-border-top: 2px rgba(255, 255, 255, 0.5) solid;

    --input-background-color: #1f1f1f; /* input area background color */
    --input-border-color--hover: #008394; /* input area border hover color */
    --input-border-color--focus: #0f78d4; /* input area border focus color */

    --dropdown-background-color: #1f1f1f; /* channel background color */
    --dropdown-item-hover-background: #333d47; /* channel or team hover background */
    --dropdown-item-selected-background: #0F78D4; /* selected channel background color */

    --color: white; /* input area border focus color */
    --arrow-fill: #ffffff;
    --placeholder-color: #f1f1f1; /* placeholder text color */
    --placeholder-color--focus: rgba(255, 255, 255, 0.8); /* place holder text focus color */
}
```

## <a name="events"></a><span data-ttu-id="a8071-120">活动</span><span class="sxs-lookup"><span data-stu-id="a8071-120">Events</span></span>
| <span data-ttu-id="a8071-121">事件</span><span class="sxs-lookup"><span data-stu-id="a8071-121">Event</span></span> | <span data-ttu-id="a8071-122">详情</span><span class="sxs-lookup"><span data-stu-id="a8071-122">Detail</span></span> | <span data-ttu-id="a8071-123">说明</span><span class="sxs-lookup"><span data-stu-id="a8071-123">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="a8071-124">selectionChanged</span><span class="sxs-lookup"><span data-stu-id="a8071-124">selectionChanged</span></span> | <span data-ttu-id="a8071-125">详细信息包含 `{channel : ` [MicrosoftGraph.Channel](/graph/api/resources/channel) `, team: ` [MicrosoftGraph.Team 当前选定的项目](/graph/api/resources/team)`}`</span><span class="sxs-lookup"><span data-stu-id="a8071-125">The detail contains the currently selected item  of `{channel : `[MicrosoftGraph.Channel](/graph/api/resources/channel)`, team: `[MicrosoftGraph.Team](/graph/api/resources/team)`}`</span></span> | <span data-ttu-id="a8071-126">当用户对频道的选择做出更改时触发。</span><span class="sxs-lookup"><span data-stu-id="a8071-126">Fired when user makes a change in selection of a channel.</span></span> |

## <a name="templates"></a><span data-ttu-id="a8071-127">模板</span><span class="sxs-lookup"><span data-stu-id="a8071-127">Templates</span></span>

 <span data-ttu-id="a8071-128">`mgt-teams-channel-picker` 支持 [多个模板](../customize-components/templates.md) ，您可以使用这些模板替换组件的某些部分。</span><span class="sxs-lookup"><span data-stu-id="a8071-128">`mgt-teams-channel-picker` supports several [templates](../customize-components/templates.md) that you can use to replace certain parts of the component.</span></span> <span data-ttu-id="a8071-129">若要指定模板，请包含 `<template>` 组件中的元素，将值设置为下列 `data-type` 值之一。</span><span class="sxs-lookup"><span data-stu-id="a8071-129">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="a8071-130">数据类型</span><span class="sxs-lookup"><span data-stu-id="a8071-130">Data type</span></span> | <span data-ttu-id="a8071-131">数据上下文</span><span class="sxs-lookup"><span data-stu-id="a8071-131">Data context</span></span> | <span data-ttu-id="a8071-132">说明</span><span class="sxs-lookup"><span data-stu-id="a8071-132">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="a8071-133">loading</span><span class="sxs-lookup"><span data-stu-id="a8071-133">loading</span></span> | <span data-ttu-id="a8071-134">null：无数据</span><span class="sxs-lookup"><span data-stu-id="a8071-134">null: no data</span></span> | <span data-ttu-id="a8071-135">在向 Microsoft Graph 提出请求时用于呈现选取器状态的模板。</span><span class="sxs-lookup"><span data-stu-id="a8071-135">The template used to render the state of the picker while the request to Microsoft Graph is being made.</span></span> |
| <span data-ttu-id="a8071-136">error</span><span class="sxs-lookup"><span data-stu-id="a8071-136">error</span></span> | <span data-ttu-id="a8071-137">null：无数据</span><span class="sxs-lookup"><span data-stu-id="a8071-137">null: no data</span></span>| <span data-ttu-id="a8071-138">如果用户搜索未返回任何用户，则使用的模板。</span><span class="sxs-lookup"><span data-stu-id="a8071-138">The template used if user search returns no users.</span></span> |


<span data-ttu-id="a8071-139">以下示例显示如何使用 `error` 模板。</span><span class="sxs-lookup"><span data-stu-id="a8071-139">The following example shows how to use the `error` template.</span></span>

```html
<mgt-teams-channel-picker>
  <template data-type="error">
    <p>Sorry, no Teams or Channels were found</p>
  </template>
</mgt-teams-channel-picker>
```

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="a8071-140">Microsoft Graph 权限</span><span class="sxs-lookup"><span data-stu-id="a8071-140">Microsoft Graph permissions</span></span>

<span data-ttu-id="a8071-141">此组件使用以下 Microsoft Graph API 和权限。</span><span class="sxs-lookup"><span data-stu-id="a8071-141">This component uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="a8071-142">API</span><span class="sxs-lookup"><span data-stu-id="a8071-142">API</span></span>                                                                                                              | <span data-ttu-id="a8071-143">权限</span><span class="sxs-lookup"><span data-stu-id="a8071-143">Permission</span></span>  |
| ---------------------------------------------------------------------------------------------------------------- | ----------- |
| [<span data-ttu-id="a8071-144">/me/joinedTeams</span><span class="sxs-lookup"><span data-stu-id="a8071-144">/me/joinedTeams</span></span>](/graph/api/user-list-joinedteams)                    | <span data-ttu-id="a8071-145">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="a8071-145">User.Read.All</span></span>        |
| [<span data-ttu-id="a8071-146">/teams/${id}/channels</span><span class="sxs-lookup"><span data-stu-id="a8071-146">/teams/${id}/channels</span></span>](/graph/api/channel-list) | <span data-ttu-id="a8071-147">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="a8071-147">Group.Read.All</span></span>        |

## <a name="authentication"></a><span data-ttu-id="a8071-148">身份验证</span><span class="sxs-lookup"><span data-stu-id="a8071-148">Authentication</span></span>

<span data-ttu-id="a8071-149">该控件使用身份验证文档中介绍的全局 [身份验证提供程序](../providers/providers.md)。</span><span class="sxs-lookup"><span data-stu-id="a8071-149">The control uses the global authentication provider described in the [authentication documentation](../providers/providers.md).</span></span>

## <a name="extend-for-more-control"></a><span data-ttu-id="a8071-150">扩展以更多控制</span><span class="sxs-lookup"><span data-stu-id="a8071-150">Extend for more control</span></span>

<span data-ttu-id="a8071-151">对于更复杂的方案或真正自定义的 UX，此组件公开了多个在组件扩展中 `protected render*` 替代的方法：</span><span class="sxs-lookup"><span data-stu-id="a8071-151">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions:</span></span>

| <span data-ttu-id="a8071-152">方法</span><span class="sxs-lookup"><span data-stu-id="a8071-152">Method</span></span> | <span data-ttu-id="a8071-153">说明</span><span class="sxs-lookup"><span data-stu-id="a8071-153">Description</span></span> |
| - | - |
| <span data-ttu-id="a8071-154">renderSelected</span><span class="sxs-lookup"><span data-stu-id="a8071-154">renderSelected</span></span> | <span data-ttu-id="a8071-155">在输入框中呈现选定的团队和频道。</span><span class="sxs-lookup"><span data-stu-id="a8071-155">Renders the selected team and channel in the input box.</span></span> |
| <span data-ttu-id="a8071-156">renderInput</span><span class="sxs-lookup"><span data-stu-id="a8071-156">renderInput</span></span> | <span data-ttu-id="a8071-157">呈现输入框。</span><span class="sxs-lookup"><span data-stu-id="a8071-157">Renders the input box.</span></span> |
| <span data-ttu-id="a8071-158">renderDropdown</span><span class="sxs-lookup"><span data-stu-id="a8071-158">renderDropdown</span></span> | <span data-ttu-id="a8071-159">呈现下拉列表。</span><span class="sxs-lookup"><span data-stu-id="a8071-159">Renders the dropdown.</span></span> |
| <span data-ttu-id="a8071-160">renderDropdownList</span><span class="sxs-lookup"><span data-stu-id="a8071-160">renderDropdownList</span></span> | <span data-ttu-id="a8071-161">以递归方法呈现下拉列表中的项。</span><span class="sxs-lookup"><span data-stu-id="a8071-161">Renders the items in the dropdown recursively.</span></span> |
| <span data-ttu-id="a8071-162">renderItem</span><span class="sxs-lookup"><span data-stu-id="a8071-162">renderItem</span></span> | <span data-ttu-id="a8071-163">在下拉列表中呈现团队或频道。</span><span class="sxs-lookup"><span data-stu-id="a8071-163">Renders a team or a channel in the dropdown list.</span></span> |
| <span data-ttu-id="a8071-164">renderHighlightedText</span><span class="sxs-lookup"><span data-stu-id="a8071-164">renderHighlightedText</span></span> | <span data-ttu-id="a8071-165">呈现通道文本，突出显示输入查询。</span><span class="sxs-lookup"><span data-stu-id="a8071-165">Renders the channel text, highlighting the input query.</span></span> |
| <span data-ttu-id="a8071-166">renderLoading</span><span class="sxs-lookup"><span data-stu-id="a8071-166">renderLoading</span></span> | <span data-ttu-id="a8071-167">呈现加载下拉列表状态。</span><span class="sxs-lookup"><span data-stu-id="a8071-167">Renders the loading dropdown state.</span></span> |
| <span data-ttu-id="a8071-168">renderError</span><span class="sxs-lookup"><span data-stu-id="a8071-168">renderError</span></span> | <span data-ttu-id="a8071-169">呈现下拉列表错误状态。</span><span class="sxs-lookup"><span data-stu-id="a8071-169">Renders the dropdown error state.</span></span> |
