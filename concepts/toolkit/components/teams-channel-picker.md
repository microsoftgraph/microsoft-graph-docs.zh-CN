---
title: Microsoft Graph 工具包中的 microsoft 团队频道选取器组件
description: 您可以使用 "工作团队-频道选取器" 从 Microsoft Graph 中搜索与用户关联的频道和团队。
localization_priority: Normal
author: vogtn
ms.openlocfilehash: c8ade0fdfd41bde4d4a2ec643950b3faa8d24d98
ms.sourcegitcommit: 1bc5a0c179dce57e90349610566fb86e1b5fbf95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/04/2020
ms.locfileid: "43144383"
---
# <a name="microsoft-teams-channel-picker-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="8cb2a-103">Microsoft Graph 工具包中的 microsoft 团队频道选取器组件</span><span class="sxs-lookup"><span data-stu-id="8cb2a-103">Microsoft Teams Channel Picker component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="8cb2a-104">A 您可以使用`mgt-teams-channel-picker`组件来搜索与用户相关联的 Microsoft 团队频道。</span><span class="sxs-lookup"><span data-stu-id="8cb2a-104">A you can use the `mgt-teams-channel-picker` component to enable searches for Microsoft Teams channels associated with a user.</span></span> <span data-ttu-id="8cb2a-105">组件可以搜索用户加入的所有团队以及这些团队中的每个频道。</span><span class="sxs-lookup"><span data-stu-id="8cb2a-105">The component can search all teams the user has joined, and each channel in those teams.</span></span> 

## <a name="example"></a><span data-ttu-id="8cb2a-106">示例</span><span class="sxs-lookup"><span data-stu-id="8cb2a-106">Example</span></span>

<span data-ttu-id="8cb2a-107">下面的示例演示了`mgt-teams-channel-picker`该组件。</span><span class="sxs-lookup"><span data-stu-id="8cb2a-107">The following example shows the `mgt-teams-channel-picker` component.</span></span> <span data-ttu-id="8cb2a-108">开始搜索频道或团队以查看结果呈现。</span><span class="sxs-lookup"><span data-stu-id="8cb2a-108">Start searching for a channel or team to see the results render.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-teams-channel-picker--teams-channel-picker&source=docs" height="450"></iframe>

[<span data-ttu-id="8cb2a-109">在 "dev" 中打开此示例</span><span class="sxs-lookup"><span data-stu-id="8cb2a-109">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-teams-channel-picker--teams-channel-picker&source=docs)

## <a name="getting-the-selected-channel"></a><span data-ttu-id="8cb2a-110">获取所选频道</span><span class="sxs-lookup"><span data-stu-id="8cb2a-110">Getting the selected channel</span></span>

<span data-ttu-id="8cb2a-111">使用`selectedItem`属性可检索当前选定的通道和父团队。</span><span class="sxs-lookup"><span data-stu-id="8cb2a-111">Use the `selectedItem` property to retrieve the currently selected channel and parent team.</span></span> <span data-ttu-id="8cb2a-112">如果未选择频道，则此值为 null。</span><span class="sxs-lookup"><span data-stu-id="8cb2a-112">This value will be null if no channel has been selected.</span></span> <span data-ttu-id="8cb2a-113">`selectedItem`包含两个属性`channel` ：（[MicrosoftGraph](/graph/api/resources/channel?view=graph-rest-1.0)）和`team` （[MicrosoftGraph](/graph/api/resources/team?view=graph-rest-1.0)）。</span><span class="sxs-lookup"><span data-stu-id="8cb2a-113">`selectedItem` contains two properties: `channel` ([MicrosoftGraph.Channel](/graph/api/resources/channel?view=graph-rest-1.0)) and `team` ([MicrosoftGraph.Team](/graph/api/resources/team?view=graph-rest-1.0)).</span></span>

```javascript
const channelPicker = document.querySelector('mgt-teams-channel-picker');
console.log(channelPicker.selectedItem.channel);
console.log(channelPicker.selectedItem.team);
```

## <a name="selecting-a-channel"></a><span data-ttu-id="8cb2a-114">选择通道</span><span class="sxs-lookup"><span data-stu-id="8cb2a-114">Selecting a channel</span></span>

<span data-ttu-id="8cb2a-115">使用`selectChannelById(channelId: string)`方法以编程方式选择通道。</span><span class="sxs-lookup"><span data-stu-id="8cb2a-115">Use the `selectChannelById(channelId: string)` method to programmatically select a channel.</span></span>

> <span data-ttu-id="8cb2a-116">**注意：** 团队频道选取器仅支持单通道选择。</span><span class="sxs-lookup"><span data-stu-id="8cb2a-116">**Note:** the Teams channel picker only supports single channel selection.</span></span>

```javascript
const channelPicker = document.querySelector('mgt-teams-channel-picker');
const channelId = 'some-channel-id';
channelPicker.selectChannelById(channelId);
```

> <span data-ttu-id="8cb2a-117">**注意：** 提供的通道（以及后续 ID）必须属于已通过身份验证的用户加入的团队。</span><span class="sxs-lookup"><span data-stu-id="8cb2a-117">**Note:** The provided channel (and subsequent ID) must belong to a team that the authenticated user has joined.</span></span> 


## <a name="css-custom-properties"></a><span data-ttu-id="8cb2a-118">CSS 自定义属性</span><span class="sxs-lookup"><span data-stu-id="8cb2a-118">CSS custom properties</span></span>

<span data-ttu-id="8cb2a-119">`mgt-teams-channel-picker`组件定义以下 CSS 自定义属性。</span><span class="sxs-lookup"><span data-stu-id="8cb2a-119">The `mgt-teams-channel-picker` component defines the following CSS custom properties.</span></span>

```css
mgt-teams-channel-picker {
    --input-border: 2px rgba(255, 255, 255, 0.5) solid; /* sets all input area border */

      /* OR individual input border sides */
    --input-border-bottom: 2px rgba(255, 255, 255, 0.5) solid;
    --input-border-right: 2px rgba(255, 255, 255, 0.5) solid;
    --input-border-left: 2px rgba(255, 255, 255, 0.5) solid;
    --input-border-top: 2px rgba(255, 255, 255, 0.5) solid;

    --input-background-color: #1f1f1f; /* input area background color */
    --input-hover-color: #008394; /* input area border hover color */
    --input-focus-color: #0f78d4; /* input area border focus color */

    --dropdown-background-color: #1f1f1f; /* channel background color */
    --dropdown-item-hover-background: #333d47; /* channel or team hover background */
    --dropdown-item-selected-background: #0F78D4; /* selected channel background color */

    --font-color: white; /* input area border focus color */
    --arrow-fill: #ffffff;
    --placeholder-focus-color: rgba(255, 255, 255, 0.8); /* place holder text focus color */
}
```

## <a name="events"></a><span data-ttu-id="8cb2a-120">事件</span><span class="sxs-lookup"><span data-stu-id="8cb2a-120">Events</span></span>
| <span data-ttu-id="8cb2a-121">事件</span><span class="sxs-lookup"><span data-stu-id="8cb2a-121">Event</span></span> | <span data-ttu-id="8cb2a-122">详细信息</span><span class="sxs-lookup"><span data-stu-id="8cb2a-122">Detail</span></span> | <span data-ttu-id="8cb2a-123">说明</span><span class="sxs-lookup"><span data-stu-id="8cb2a-123">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="8cb2a-124">selectionChanged</span><span class="sxs-lookup"><span data-stu-id="8cb2a-124">selectionChanged</span></span> | <span data-ttu-id="8cb2a-125">详细信息包含`{channel : ` [MicrosoftGraph](/graph/api/resources/channel?view=graph-rest-1.0)`, team: `[MicrosoftGraph](/graph/api/resources/team?view=graph-rest-1.0)的当前选定项。`}`</span><span class="sxs-lookup"><span data-stu-id="8cb2a-125">The detail contains the currently selected item  of `{channel : `[MicrosoftGraph.Channel](/graph/api/resources/channel?view=graph-rest-1.0)`, team: `[MicrosoftGraph.Team](/graph/api/resources/team?view=graph-rest-1.0)`}`</span></span> | <span data-ttu-id="8cb2a-126">当用户在选择频道时进行更改时激发。</span><span class="sxs-lookup"><span data-stu-id="8cb2a-126">Fired when user makes a change in selection of a channel.</span></span> |

## <a name="templates"></a><span data-ttu-id="8cb2a-127">模板</span><span class="sxs-lookup"><span data-stu-id="8cb2a-127">Templates</span></span>

 <span data-ttu-id="8cb2a-128">`mgt-teams-channel-picker`支持多个模板，这些[模板](../templates.md)可用于替换组件的某些部分。</span><span class="sxs-lookup"><span data-stu-id="8cb2a-128">`mgt-teams-channel-picker` supports several [templates](../templates.md) that you can use to replace certain parts of the component.</span></span> <span data-ttu-id="8cb2a-129">若要指定模板，请在`<template>`组件内添加一个元素，并`data-type`将值设置为下列值之一。</span><span class="sxs-lookup"><span data-stu-id="8cb2a-129">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="8cb2a-130">数据类型</span><span class="sxs-lookup"><span data-stu-id="8cb2a-130">Data type</span></span> | <span data-ttu-id="8cb2a-131">数据上下文</span><span class="sxs-lookup"><span data-stu-id="8cb2a-131">Data context</span></span> | <span data-ttu-id="8cb2a-132">说明</span><span class="sxs-lookup"><span data-stu-id="8cb2a-132">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="8cb2a-133">装载</span><span class="sxs-lookup"><span data-stu-id="8cb2a-133">loading</span></span> | <span data-ttu-id="8cb2a-134">null：无数据</span><span class="sxs-lookup"><span data-stu-id="8cb2a-134">null: no data</span></span> | <span data-ttu-id="8cb2a-135">在发出对 Microsoft Graph 的请求时用于呈现选取器状态的模板。</span><span class="sxs-lookup"><span data-stu-id="8cb2a-135">The template used to render the state of the picker while the request to Microsoft Graph is being made.</span></span> |
| <span data-ttu-id="8cb2a-136">error</span><span class="sxs-lookup"><span data-stu-id="8cb2a-136">error</span></span> | <span data-ttu-id="8cb2a-137">null：无数据</span><span class="sxs-lookup"><span data-stu-id="8cb2a-137">null: no data</span></span>| <span data-ttu-id="8cb2a-138">用户搜索不返回用户时使用的模板。</span><span class="sxs-lookup"><span data-stu-id="8cb2a-138">The template used if user search returns no users.</span></span> |


<span data-ttu-id="8cb2a-139">下面的示例演示如何使用`error`模板。</span><span class="sxs-lookup"><span data-stu-id="8cb2a-139">The following example shows how to use the `error` template.</span></span>

```html
<mgt-teams-channel-picker>
  <template data-type="error">
    <p>Sorry, no Teams or Channels were found</p>
  </template>
</mgt-teams-channel-picker>
```

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="8cb2a-140">Microsoft Graph 权限</span><span class="sxs-lookup"><span data-stu-id="8cb2a-140">Microsoft Graph permissions</span></span>

<span data-ttu-id="8cb2a-141">此组件使用以下 Microsoft Graph Api 和权限。</span><span class="sxs-lookup"><span data-stu-id="8cb2a-141">This component uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="8cb2a-142">API</span><span class="sxs-lookup"><span data-stu-id="8cb2a-142">API</span></span>                                                                                                              | <span data-ttu-id="8cb2a-143">权限</span><span class="sxs-lookup"><span data-stu-id="8cb2a-143">Permission</span></span>  |
| ---------------------------------------------------------------------------------------------------------------- | ----------- |
| [<span data-ttu-id="8cb2a-144">/me/joinedTeams</span><span class="sxs-lookup"><span data-stu-id="8cb2a-144">/me/joinedTeams</span></span>](/graph/api/user-list-joinedteams?view=graph-rest-1.0)                    | <span data-ttu-id="8cb2a-145">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="8cb2a-145">User.Read.All</span></span>        |
| [<span data-ttu-id="8cb2a-146">/teams/$ {id}/channels</span><span class="sxs-lookup"><span data-stu-id="8cb2a-146">/teams/${id}/channels</span></span>](/graph/api/channel-list?view=graph-rest-1.0) | <span data-ttu-id="8cb2a-147">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="8cb2a-147">Group.Read.All</span></span>        |

## <a name="authentication"></a><span data-ttu-id="8cb2a-148">身份验证</span><span class="sxs-lookup"><span data-stu-id="8cb2a-148">Authentication</span></span>

<span data-ttu-id="8cb2a-149">该控件使用[身份验证文档](./../providers.md)中介绍的全局身份验证提供程序。</span><span class="sxs-lookup"><span data-stu-id="8cb2a-149">The control uses the global authentication provider described in the [authentication documentation](./../providers.md).</span></span>

## <a name="extend-for-more-control"></a><span data-ttu-id="8cb2a-150">扩展以实现更多控制</span><span class="sxs-lookup"><span data-stu-id="8cb2a-150">Extend for more control</span></span>

<span data-ttu-id="8cb2a-151">对于更复杂的方案或真正的自定义 UX，此组件`protected render*`将公开几种用于在组件扩展中进行重写的方法：</span><span class="sxs-lookup"><span data-stu-id="8cb2a-151">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions:</span></span>

| <span data-ttu-id="8cb2a-152">方法</span><span class="sxs-lookup"><span data-stu-id="8cb2a-152">Method</span></span> | <span data-ttu-id="8cb2a-153">说明</span><span class="sxs-lookup"><span data-stu-id="8cb2a-153">Description</span></span> |
| - | - |
| <span data-ttu-id="8cb2a-154">renderSelected</span><span class="sxs-lookup"><span data-stu-id="8cb2a-154">renderSelected</span></span> | <span data-ttu-id="8cb2a-155">在输入框中呈现选定的团队和频道。</span><span class="sxs-lookup"><span data-stu-id="8cb2a-155">Renders the selected team and channel in the input box.</span></span> |
| <span data-ttu-id="8cb2a-156">renderInput</span><span class="sxs-lookup"><span data-stu-id="8cb2a-156">renderInput</span></span> | <span data-ttu-id="8cb2a-157">呈现输入框。</span><span class="sxs-lookup"><span data-stu-id="8cb2a-157">Renders the input box.</span></span> |
| <span data-ttu-id="8cb2a-158">renderDropdown</span><span class="sxs-lookup"><span data-stu-id="8cb2a-158">renderDropdown</span></span> | <span data-ttu-id="8cb2a-159">呈现下拉列表。</span><span class="sxs-lookup"><span data-stu-id="8cb2a-159">Renders the dropdown.</span></span> |
| <span data-ttu-id="8cb2a-160">renderDropdownList</span><span class="sxs-lookup"><span data-stu-id="8cb2a-160">renderDropdownList</span></span> | <span data-ttu-id="8cb2a-161">以递归方式呈现下拉列表中的项。</span><span class="sxs-lookup"><span data-stu-id="8cb2a-161">Renders the items in the dropdown recursively.</span></span> |
| <span data-ttu-id="8cb2a-162">renderItem</span><span class="sxs-lookup"><span data-stu-id="8cb2a-162">renderItem</span></span> | <span data-ttu-id="8cb2a-163">在下拉列表中呈现团队或通道。</span><span class="sxs-lookup"><span data-stu-id="8cb2a-163">Renders a team or a channel in the dropdown list.</span></span> |
| <span data-ttu-id="8cb2a-164">renderHighlightedText</span><span class="sxs-lookup"><span data-stu-id="8cb2a-164">renderHighlightedText</span></span> | <span data-ttu-id="8cb2a-165">呈现通道文本，突出显示输入查询。</span><span class="sxs-lookup"><span data-stu-id="8cb2a-165">Renders the channel text, highlighting the input query.</span></span> |
| <span data-ttu-id="8cb2a-166">renderLoading</span><span class="sxs-lookup"><span data-stu-id="8cb2a-166">renderLoading</span></span> | <span data-ttu-id="8cb2a-167">呈现加载下拉列表状态。</span><span class="sxs-lookup"><span data-stu-id="8cb2a-167">Renders the loading dropdown state.</span></span> |
| <span data-ttu-id="8cb2a-168">renderError</span><span class="sxs-lookup"><span data-stu-id="8cb2a-168">renderError</span></span> | <span data-ttu-id="8cb2a-169">呈现下拉列表错误状态。</span><span class="sxs-lookup"><span data-stu-id="8cb2a-169">Renders the dropdown error state.</span></span> |
