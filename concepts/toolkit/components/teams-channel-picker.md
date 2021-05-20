---
title: Microsoft TeamsMicrosoft 服务中的频道选取器Graph Toolkit
description: 可以使用 mgt-teams-channel-picker 从 Microsoft 网站搜索与用户关联的Graph。
localization_priority: Normal
author: vogtn
ms.openlocfilehash: aaa89b9fab5d9e29c35b7d2cabb0a494ca97d4b3
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579940"
---
# <a name="microsoft-teams-channel-picker-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="05b03-103">Microsoft TeamsMicrosoft 服务中的频道选取器Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="05b03-103">Microsoft Teams Channel Picker component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="05b03-104">可以使用组件 `mgt-teams-channel-picker` 为与用户关联的Microsoft Teams启用搜索。</span><span class="sxs-lookup"><span data-stu-id="05b03-104">A you can use the `mgt-teams-channel-picker` component to enable searches for Microsoft Teams channels associated with a user.</span></span> <span data-ttu-id="05b03-105">组件可以搜索用户已加入的所有团队，以及这些团队中的每个频道。</span><span class="sxs-lookup"><span data-stu-id="05b03-105">The component can search all teams the user has joined, and each channel in those teams.</span></span> 

## <a name="example"></a><span data-ttu-id="05b03-106">示例</span><span class="sxs-lookup"><span data-stu-id="05b03-106">Example</span></span>

<span data-ttu-id="05b03-107">以下示例显示 `mgt-teams-channel-picker` 组件。</span><span class="sxs-lookup"><span data-stu-id="05b03-107">The following example shows the `mgt-teams-channel-picker` component.</span></span> <span data-ttu-id="05b03-108">开始搜索频道或团队以查看结果呈现。</span><span class="sxs-lookup"><span data-stu-id="05b03-108">Start searching for a channel or team to see the results render.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-teams-channel-picker--teams-channel-picker&source=docs" height="450"></iframe>

[<span data-ttu-id="05b03-109">在"打开"mgt.dev</span><span class="sxs-lookup"><span data-stu-id="05b03-109">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-teams-channel-picker--teams-channel-picker&source=docs)

## <a name="getting-the-selected-channel"></a><span data-ttu-id="05b03-110">获取所选频道</span><span class="sxs-lookup"><span data-stu-id="05b03-110">Getting the selected channel</span></span>

<span data-ttu-id="05b03-111">使用 `selectedItem` 属性检索当前选定的频道和父团队。</span><span class="sxs-lookup"><span data-stu-id="05b03-111">Use the `selectedItem` property to retrieve the currently selected channel and parent team.</span></span> <span data-ttu-id="05b03-112">如果未选择任何通道，则此值将为 null。</span><span class="sxs-lookup"><span data-stu-id="05b03-112">This value will be null if no channel has been selected.</span></span> <span data-ttu-id="05b03-113">`selectedItem` 包含两个 `channel` 属性： ([MicrosoftGraph.Channel](/graph/api/resources/channel)) 和 `team` ([MicrosoftGraph.Team](/graph/api/resources/team)) 。</span><span class="sxs-lookup"><span data-stu-id="05b03-113">`selectedItem` contains two properties: `channel` ([MicrosoftGraph.Channel](/graph/api/resources/channel)) and `team` ([MicrosoftGraph.Team](/graph/api/resources/team)).</span></span>

```javascript
const channelPicker = document.querySelector('mgt-teams-channel-picker');
console.log(channelPicker.selectedItem.channel);
console.log(channelPicker.selectedItem.team);
```

## <a name="selecting-a-channel"></a><span data-ttu-id="05b03-114">选择频道</span><span class="sxs-lookup"><span data-stu-id="05b03-114">Selecting a channel</span></span>

<span data-ttu-id="05b03-115">使用 `selectChannelById(channelId: string)` 方法以编程方式选择通道。</span><span class="sxs-lookup"><span data-stu-id="05b03-115">Use the `selectChannelById(channelId: string)` method to programmatically select a channel.</span></span>

> <span data-ttu-id="05b03-116">**注意：Teams** 文件选取器仅支持单通道选择。</span><span class="sxs-lookup"><span data-stu-id="05b03-116">**Note:** the Teams channel picker only supports single channel selection.</span></span>

```javascript
const channelPicker = document.querySelector('mgt-teams-channel-picker');
const channelId = 'some-channel-id';
channelPicker.selectChannelById(channelId);
```

> <span data-ttu-id="05b03-117">**注意：** 提供的频道 (和后续 ID) 必须属于经过身份验证的用户已加入的团队。</span><span class="sxs-lookup"><span data-stu-id="05b03-117">**Note:** The provided channel (and subsequent ID) must belong to a team that the authenticated user has joined.</span></span> 


## <a name="css-custom-properties"></a><span data-ttu-id="05b03-118">CSS 自定义属性</span><span class="sxs-lookup"><span data-stu-id="05b03-118">CSS custom properties</span></span>

<span data-ttu-id="05b03-119">组件 `mgt-teams-channel-picker` 定义以下 CSS 自定义属性。</span><span class="sxs-lookup"><span data-stu-id="05b03-119">The `mgt-teams-channel-picker` component defines the following CSS custom properties.</span></span>

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

## <a name="events"></a><span data-ttu-id="05b03-120">活动</span><span class="sxs-lookup"><span data-stu-id="05b03-120">Events</span></span>
| <span data-ttu-id="05b03-121">事件</span><span class="sxs-lookup"><span data-stu-id="05b03-121">Event</span></span> | <span data-ttu-id="05b03-122">详情</span><span class="sxs-lookup"><span data-stu-id="05b03-122">Detail</span></span> | <span data-ttu-id="05b03-123">说明</span><span class="sxs-lookup"><span data-stu-id="05b03-123">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="05b03-124">selectionChanged</span><span class="sxs-lookup"><span data-stu-id="05b03-124">selectionChanged</span></span> | <span data-ttu-id="05b03-125">详细信息包含 `{channel : ` [MicrosoftGraph.Channel](/graph/api/resources/channel) `, team: ` [MicrosoftGraph.Team 当前选定的项](/graph/api/resources/team)`}`</span><span class="sxs-lookup"><span data-stu-id="05b03-125">The detail contains the currently selected item  of `{channel : `[MicrosoftGraph.Channel](/graph/api/resources/channel)`, team: `[MicrosoftGraph.Team](/graph/api/resources/team)`}`</span></span> | <span data-ttu-id="05b03-126">当用户在选择频道时更改时触发。</span><span class="sxs-lookup"><span data-stu-id="05b03-126">Fired when user makes a change in selection of a channel.</span></span> |

## <a name="templates"></a><span data-ttu-id="05b03-127">模板</span><span class="sxs-lookup"><span data-stu-id="05b03-127">Templates</span></span>

 <span data-ttu-id="05b03-128">`mgt-teams-channel-picker` 支持 [多个](../customize-components/templates.md) 模板，您可以使用这些模板替换组件的某些部分。</span><span class="sxs-lookup"><span data-stu-id="05b03-128">`mgt-teams-channel-picker` supports several [templates](../customize-components/templates.md) that you can use to replace certain parts of the component.</span></span> <span data-ttu-id="05b03-129">若要指定模板，请包含组件 `<template>` 中的元素，将值 `data-type` 设置为以下值之一。</span><span class="sxs-lookup"><span data-stu-id="05b03-129">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="05b03-130">数据类型</span><span class="sxs-lookup"><span data-stu-id="05b03-130">Data type</span></span> | <span data-ttu-id="05b03-131">数据上下文</span><span class="sxs-lookup"><span data-stu-id="05b03-131">Data context</span></span> | <span data-ttu-id="05b03-132">说明</span><span class="sxs-lookup"><span data-stu-id="05b03-132">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="05b03-133">loading</span><span class="sxs-lookup"><span data-stu-id="05b03-133">loading</span></span> | <span data-ttu-id="05b03-134">null：无数据</span><span class="sxs-lookup"><span data-stu-id="05b03-134">null: no data</span></span> | <span data-ttu-id="05b03-135">向 Microsoft 请求时用于呈现文件选取器Graph模板。</span><span class="sxs-lookup"><span data-stu-id="05b03-135">The template used to render the state of the picker while the request to Microsoft Graph is being made.</span></span> |
| <span data-ttu-id="05b03-136">error</span><span class="sxs-lookup"><span data-stu-id="05b03-136">error</span></span> | <span data-ttu-id="05b03-137">null：无数据</span><span class="sxs-lookup"><span data-stu-id="05b03-137">null: no data</span></span>| <span data-ttu-id="05b03-138">当用户搜索未返回任何用户时所使用的模板。</span><span class="sxs-lookup"><span data-stu-id="05b03-138">The template used if user search returns no users.</span></span> |


<span data-ttu-id="05b03-139">以下示例演示如何使用 `error` 模板。</span><span class="sxs-lookup"><span data-stu-id="05b03-139">The following example shows how to use the `error` template.</span></span>

```html
<mgt-teams-channel-picker>
  <template data-type="error">
    <p>Sorry, no Teams or Channels were found</p>
  </template>
</mgt-teams-channel-picker>
```

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="05b03-140">Microsoft Graph 权限</span><span class="sxs-lookup"><span data-stu-id="05b03-140">Microsoft Graph permissions</span></span>

<span data-ttu-id="05b03-141">默认情况下，此组件Graph Microsoft 应用程序 API 和权限。</span><span class="sxs-lookup"><span data-stu-id="05b03-141">This component uses the following Microsoft Graph APIs and permissions by default.</span></span>

| <span data-ttu-id="05b03-142">API</span><span class="sxs-lookup"><span data-stu-id="05b03-142">API</span></span>                                                                                                              | <span data-ttu-id="05b03-143">权限</span><span class="sxs-lookup"><span data-stu-id="05b03-143">Permission</span></span>  |
| ---------------------------------------------------------------------------------------------------------------- | ----------- |
| [<span data-ttu-id="05b03-144">/me/joinedTeams</span><span class="sxs-lookup"><span data-stu-id="05b03-144">/me/joinedTeams</span></span>](/graph/api/user-list-joinedteams)                    | <span data-ttu-id="05b03-145">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="05b03-145">User.Read.All</span></span>        |
| [<span data-ttu-id="05b03-146">/teams/${id}/channels</span><span class="sxs-lookup"><span data-stu-id="05b03-146">/teams/${id}/channels</span></span>](/graph/api/channel-list) | <span data-ttu-id="05b03-147">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="05b03-147">Group.Read.All</span></span>        |

<span data-ttu-id="05b03-148">在版本 2.2 中，所需的权限已更新为限制较少的基于Teams权限。</span><span class="sxs-lookup"><span data-stu-id="05b03-148">In version 2.2, the required permissions have been updated to the less restrictive Teams-based permissions.</span></span> <span data-ttu-id="05b03-149">若要避免发生意外更改，您需要通过全局配置选择加入新权限。</span><span class="sxs-lookup"><span data-stu-id="05b03-149">To avoid a breaking change, you need to opt in to the new permissions via a global config.</span></span>

```ts
import {MgtTeamsChannelPicker} from "@microsoft/mgt-components";

MgtTeamsChannelPicker.config.useTeamsBasedScopes = true;
```

<span data-ttu-id="05b03-150">设置为 `useTeamsBasedScopes` `true` 时，Teams选取器将使用以下范围。</span><span class="sxs-lookup"><span data-stu-id="05b03-150">With `useTeamsBasedScopes` set to `true`, the Teams Channel Picker will use the following scopes.</span></span> 

| <span data-ttu-id="05b03-151">API</span><span class="sxs-lookup"><span data-stu-id="05b03-151">API</span></span>                                                                                                              | <span data-ttu-id="05b03-152">权限</span><span class="sxs-lookup"><span data-stu-id="05b03-152">Permission</span></span>  |
| ---------------------------------------------------------------------------------------------------------------- | ----------- |
| [<span data-ttu-id="05b03-153">/me/joinedTeams</span><span class="sxs-lookup"><span data-stu-id="05b03-153">/me/joinedTeams</span></span>](/graph/api/user-list-joinedteams)                    | <span data-ttu-id="05b03-154">Team.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="05b03-154">Team.ReadBasic.All</span></span>        |
| [<span data-ttu-id="05b03-155">/teams/${id}/channels</span><span class="sxs-lookup"><span data-stu-id="05b03-155">/teams/${id}/channels</span></span>](/graph/api/channel-list) | <span data-ttu-id="05b03-156">Channel.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="05b03-156">Channel.ReadBasic.All</span></span>        |

<span data-ttu-id="05b03-157">这些权限将是下一个主要更新中的默认权限。</span><span class="sxs-lookup"><span data-stu-id="05b03-157">These will be the default permissions in the next major update.</span></span>

## <a name="authentication"></a><span data-ttu-id="05b03-158">身份验证</span><span class="sxs-lookup"><span data-stu-id="05b03-158">Authentication</span></span>

<span data-ttu-id="05b03-159">该控件使用身份验证文档中所述的全局 [身份验证提供程序](../providers/providers.md)。</span><span class="sxs-lookup"><span data-stu-id="05b03-159">The control uses the global authentication provider described in the [authentication documentation](../providers/providers.md).</span></span>

## <a name="cache"></a><span data-ttu-id="05b03-160">缓存</span><span class="sxs-lookup"><span data-stu-id="05b03-160">Cache</span></span>

<span data-ttu-id="05b03-161">`mgt-teams-channel-picker`组件不缓存任何数据。</span><span class="sxs-lookup"><span data-stu-id="05b03-161">The `mgt-teams-channel-picker` component doesn't cache any data.</span></span>

## <a name="extend-for-more-control"></a><span data-ttu-id="05b03-162">扩展以了解更多控件</span><span class="sxs-lookup"><span data-stu-id="05b03-162">Extend for more control</span></span>

<span data-ttu-id="05b03-163">对于更复杂的方案或真正自定义的 UX，此组件公开了多个在组件扩展 `protected render*` 中替代的方法：</span><span class="sxs-lookup"><span data-stu-id="05b03-163">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions:</span></span>

| <span data-ttu-id="05b03-164">方法</span><span class="sxs-lookup"><span data-stu-id="05b03-164">Method</span></span> | <span data-ttu-id="05b03-165">说明</span><span class="sxs-lookup"><span data-stu-id="05b03-165">Description</span></span> |
| - | - |
| <span data-ttu-id="05b03-166">renderSelected</span><span class="sxs-lookup"><span data-stu-id="05b03-166">renderSelected</span></span> | <span data-ttu-id="05b03-167">在输入框中呈现选定的团队和频道。</span><span class="sxs-lookup"><span data-stu-id="05b03-167">Renders the selected team and channel in the input box.</span></span> |
| <span data-ttu-id="05b03-168">renderInput</span><span class="sxs-lookup"><span data-stu-id="05b03-168">renderInput</span></span> | <span data-ttu-id="05b03-169">呈现输入框。</span><span class="sxs-lookup"><span data-stu-id="05b03-169">Renders the input box.</span></span> |
| <span data-ttu-id="05b03-170">renderDropdown</span><span class="sxs-lookup"><span data-stu-id="05b03-170">renderDropdown</span></span> | <span data-ttu-id="05b03-171">呈现下拉列表。</span><span class="sxs-lookup"><span data-stu-id="05b03-171">Renders the dropdown.</span></span> |
| <span data-ttu-id="05b03-172">renderDropdownList</span><span class="sxs-lookup"><span data-stu-id="05b03-172">renderDropdownList</span></span> | <span data-ttu-id="05b03-173">以递归方法呈现下拉列表中的项。</span><span class="sxs-lookup"><span data-stu-id="05b03-173">Renders the items in the dropdown recursively.</span></span> |
| <span data-ttu-id="05b03-174">renderItem</span><span class="sxs-lookup"><span data-stu-id="05b03-174">renderItem</span></span> | <span data-ttu-id="05b03-175">在下拉列表中呈现团队或频道。</span><span class="sxs-lookup"><span data-stu-id="05b03-175">Renders a team or a channel in the dropdown list.</span></span> |
| <span data-ttu-id="05b03-176">renderHighlightedText</span><span class="sxs-lookup"><span data-stu-id="05b03-176">renderHighlightedText</span></span> | <span data-ttu-id="05b03-177">呈现通道文本，突出显示输入查询。</span><span class="sxs-lookup"><span data-stu-id="05b03-177">Renders the channel text, highlighting the input query.</span></span> |
| <span data-ttu-id="05b03-178">renderLoading</span><span class="sxs-lookup"><span data-stu-id="05b03-178">renderLoading</span></span> | <span data-ttu-id="05b03-179">呈现加载下拉列表状态。</span><span class="sxs-lookup"><span data-stu-id="05b03-179">Renders the loading dropdown state.</span></span> |
| <span data-ttu-id="05b03-180">renderError</span><span class="sxs-lookup"><span data-stu-id="05b03-180">renderError</span></span> | <span data-ttu-id="05b03-181">呈现下拉列表错误状态。</span><span class="sxs-lookup"><span data-stu-id="05b03-181">Renders the dropdown error state.</span></span> |
