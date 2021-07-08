---
title: Microsoft TeamsMicrosoft 服务中的频道选取器Graph Toolkit
description: 可以使用 mgt-teams-channel-picker 从 Microsoft 网站搜索与用户关联的Graph。
localization_priority: Normal
author: vogtn
ms.openlocfilehash: cd27db315de6b46c10c18e300ddb899ea042e428
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334729"
---
# <a name="microsoft-teams-channel-picker-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="cd68e-103">Microsoft TeamsMicrosoft 服务中的频道选取器Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="cd68e-103">Microsoft Teams Channel Picker component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="cd68e-104">可以使用组件 `mgt-teams-channel-picker` 为与用户关联的Microsoft Teams启用搜索。</span><span class="sxs-lookup"><span data-stu-id="cd68e-104">A you can use the `mgt-teams-channel-picker` component to enable searches for Microsoft Teams channels associated with a user.</span></span> <span data-ttu-id="cd68e-105">组件可以搜索用户已加入的所有团队，以及这些团队中的每个频道。</span><span class="sxs-lookup"><span data-stu-id="cd68e-105">The component can search all teams the user has joined, and each channel in those teams.</span></span> 

## <a name="example"></a><span data-ttu-id="cd68e-106">示例</span><span class="sxs-lookup"><span data-stu-id="cd68e-106">Example</span></span>

<span data-ttu-id="cd68e-107">以下示例显示 `mgt-teams-channel-picker` 组件。</span><span class="sxs-lookup"><span data-stu-id="cd68e-107">The following example shows the `mgt-teams-channel-picker` component.</span></span> <span data-ttu-id="cd68e-108">开始搜索频道或团队以查看结果呈现。</span><span class="sxs-lookup"><span data-stu-id="cd68e-108">Start searching for a channel or team to see the results render.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-teams-channel-picker--teams-channel-picker&source=docs" height="450"></iframe>

[<span data-ttu-id="cd68e-109">在 mgt.dev 中打开此示例</span><span class="sxs-lookup"><span data-stu-id="cd68e-109">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-teams-channel-picker--teams-channel-picker&source=docs)

## <a name="getting-the-selected-channel"></a><span data-ttu-id="cd68e-110">获取所选频道</span><span class="sxs-lookup"><span data-stu-id="cd68e-110">Getting the selected channel</span></span>

<span data-ttu-id="cd68e-111">使用 `selectedItem` 属性检索当前选定的频道和父团队。</span><span class="sxs-lookup"><span data-stu-id="cd68e-111">Use the `selectedItem` property to retrieve the currently selected channel and parent team.</span></span> <span data-ttu-id="cd68e-112">如果未选择任何通道，则此值将为 null。</span><span class="sxs-lookup"><span data-stu-id="cd68e-112">This value will be null if no channel has been selected.</span></span> <span data-ttu-id="cd68e-113">`selectedItem` 包含两个 `channel` 属性： ([MicrosoftGraph.Channel](/graph/api/resources/channel)) 和 `team` ([MicrosoftGraph.Team](/graph/api/resources/team)) 。</span><span class="sxs-lookup"><span data-stu-id="cd68e-113">`selectedItem` contains two properties: `channel` ([MicrosoftGraph.Channel](/graph/api/resources/channel)) and `team` ([MicrosoftGraph.Team](/graph/api/resources/team)).</span></span>

```javascript
const channelPicker = document.querySelector('mgt-teams-channel-picker');
console.log(channelPicker.selectedItem.channel);
console.log(channelPicker.selectedItem.team);
```

## <a name="selecting-a-channel"></a><span data-ttu-id="cd68e-114">选择频道</span><span class="sxs-lookup"><span data-stu-id="cd68e-114">Selecting a channel</span></span>

<span data-ttu-id="cd68e-115">使用 `selectChannelById(channelId: string)` 方法以编程方式选择通道。</span><span class="sxs-lookup"><span data-stu-id="cd68e-115">Use the `selectChannelById(channelId: string)` method to programmatically select a channel.</span></span>

> <span data-ttu-id="cd68e-116">**注意：Teams** 文件选取器仅支持单通道选择。</span><span class="sxs-lookup"><span data-stu-id="cd68e-116">**Note:** the Teams channel picker only supports single channel selection.</span></span>

```javascript
const channelPicker = document.querySelector('mgt-teams-channel-picker');
const channelId = 'some-channel-id';
channelPicker.selectChannelById(channelId);
```

> <span data-ttu-id="cd68e-117">**注意：** 提供的频道 (和后续 ID) 必须属于经过身份验证的用户已加入的团队。</span><span class="sxs-lookup"><span data-stu-id="cd68e-117">**Note:** The provided channel (and subsequent ID) must belong to a team that the authenticated user has joined.</span></span> 


## <a name="css-custom-properties"></a><span data-ttu-id="cd68e-118">CSS 自定义属性</span><span class="sxs-lookup"><span data-stu-id="cd68e-118">CSS custom properties</span></span>

<span data-ttu-id="cd68e-119">组件 `mgt-teams-channel-picker` 定义以下 CSS 自定义属性。</span><span class="sxs-lookup"><span data-stu-id="cd68e-119">The `mgt-teams-channel-picker` component defines the following CSS custom properties.</span></span>

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

## <a name="events"></a><span data-ttu-id="cd68e-120">活动</span><span class="sxs-lookup"><span data-stu-id="cd68e-120">Events</span></span>

<span data-ttu-id="cd68e-121">事件</span><span class="sxs-lookup"><span data-stu-id="cd68e-121">Event</span></span> | <span data-ttu-id="cd68e-122">何时发出</span><span class="sxs-lookup"><span data-stu-id="cd68e-122">When is it emitted</span></span> | <span data-ttu-id="cd68e-123">自定义数据</span><span class="sxs-lookup"><span data-stu-id="cd68e-123">Custom data</span></span> | <span data-ttu-id="cd68e-124">Cancelable</span><span class="sxs-lookup"><span data-stu-id="cd68e-124">Cancelable</span></span> | <span data-ttu-id="cd68e-125">气泡</span><span class="sxs-lookup"><span data-stu-id="cd68e-125">Bubbles</span></span> | <span data-ttu-id="cd68e-126">使用自定义模板</span><span class="sxs-lookup"><span data-stu-id="cd68e-126">Works with custom template</span></span>
------|-------------------|--------------|:-----------:|:---------:|:---------------------------:|
`selectionChanged` | <span data-ttu-id="cd68e-127">在用户更改频道选择时触发</span><span class="sxs-lookup"><span data-stu-id="cd68e-127">Fired when user makes a change in selection of a channel</span></span> | <span data-ttu-id="cd68e-128">当前选择的项目作为 `{ channel: ` [频道](/graph/api/resources/channel) `, team: ` [团队](/graph/api/resources/team)`}`</span><span class="sxs-lookup"><span data-stu-id="cd68e-128">The currently selected item as `{ channel: `[channel](/graph/api/resources/channel)`, team: `[team](/graph/api/resources/team)`}`</span></span> | <span data-ttu-id="cd68e-129">否</span><span class="sxs-lookup"><span data-stu-id="cd68e-129">No</span></span> | <span data-ttu-id="cd68e-130">否</span><span class="sxs-lookup"><span data-stu-id="cd68e-130">No</span></span> | <span data-ttu-id="cd68e-131">是</span><span class="sxs-lookup"><span data-stu-id="cd68e-131">Yes</span></span>

<span data-ttu-id="cd68e-132">有关处理事件的信息，请参阅 [事件](../customize-components/events.md)。</span><span class="sxs-lookup"><span data-stu-id="cd68e-132">For more information about handling events, see [events](../customize-components/events.md).</span></span>

## <a name="templates"></a><span data-ttu-id="cd68e-133">模板</span><span class="sxs-lookup"><span data-stu-id="cd68e-133">Templates</span></span>

<span data-ttu-id="cd68e-134">`mgt-teams-channel-picker` 支持 [多个](../customize-components/templates.md) 模板，您可以使用这些模板替换组件的某些部分。</span><span class="sxs-lookup"><span data-stu-id="cd68e-134">`mgt-teams-channel-picker` supports several [templates](../customize-components/templates.md) that you can use to replace certain parts of the component.</span></span> <span data-ttu-id="cd68e-135">若要指定模板，请包含组件 `<template>` 中的元素，将值 `data-type` 设置为以下值之一。</span><span class="sxs-lookup"><span data-stu-id="cd68e-135">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="cd68e-136">数据类型</span><span class="sxs-lookup"><span data-stu-id="cd68e-136">Data type</span></span> | <span data-ttu-id="cd68e-137">数据上下文</span><span class="sxs-lookup"><span data-stu-id="cd68e-137">Data context</span></span> | <span data-ttu-id="cd68e-138">说明</span><span class="sxs-lookup"><span data-stu-id="cd68e-138">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="cd68e-139">loading</span><span class="sxs-lookup"><span data-stu-id="cd68e-139">loading</span></span> | <span data-ttu-id="cd68e-140">null：无数据</span><span class="sxs-lookup"><span data-stu-id="cd68e-140">null: no data</span></span> | <span data-ttu-id="cd68e-141">向 Microsoft 请求时用于呈现文件选取器Graph模板。</span><span class="sxs-lookup"><span data-stu-id="cd68e-141">The template used to render the state of the picker while the request to Microsoft Graph is being made.</span></span> |
| <span data-ttu-id="cd68e-142">error</span><span class="sxs-lookup"><span data-stu-id="cd68e-142">error</span></span> | <span data-ttu-id="cd68e-143">null：无数据</span><span class="sxs-lookup"><span data-stu-id="cd68e-143">null: no data</span></span>| <span data-ttu-id="cd68e-144">当用户搜索未返回任何用户时所使用的模板。</span><span class="sxs-lookup"><span data-stu-id="cd68e-144">The template used if user search returns no users.</span></span> |

<span data-ttu-id="cd68e-145">以下示例演示如何使用 `error` 模板。</span><span class="sxs-lookup"><span data-stu-id="cd68e-145">The following example shows how to use the `error` template.</span></span>

```html
<mgt-teams-channel-picker>
  <template data-type="error">
    <p>Sorry, no Teams or Channels were found</p>
  </template>
</mgt-teams-channel-picker>
```

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="cd68e-146">Microsoft Graph 权限</span><span class="sxs-lookup"><span data-stu-id="cd68e-146">Microsoft Graph permissions</span></span>

<span data-ttu-id="cd68e-147">默认情况下，此组件Graph Microsoft 应用程序 API 和权限。</span><span class="sxs-lookup"><span data-stu-id="cd68e-147">This component uses the following Microsoft Graph APIs and permissions by default.</span></span>

| <span data-ttu-id="cd68e-148">API</span><span class="sxs-lookup"><span data-stu-id="cd68e-148">API</span></span>                                                                                                              | <span data-ttu-id="cd68e-149">权限</span><span class="sxs-lookup"><span data-stu-id="cd68e-149">Permission</span></span>  |
| ---------------------------------------------------------------------------------------------------------------- | ----------- |
| [<span data-ttu-id="cd68e-150">/me/joinedTeams</span><span class="sxs-lookup"><span data-stu-id="cd68e-150">/me/joinedTeams</span></span>](/graph/api/user-list-joinedteams)                    | <span data-ttu-id="cd68e-151">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="cd68e-151">User.Read.All</span></span>        |
| [<span data-ttu-id="cd68e-152">/teams/${id}/channels</span><span class="sxs-lookup"><span data-stu-id="cd68e-152">/teams/${id}/channels</span></span>](/graph/api/channel-list) | <span data-ttu-id="cd68e-153">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="cd68e-153">Group.Read.All</span></span>        |

<span data-ttu-id="cd68e-154">在版本 2.2 中，所需的权限已更新为限制较少的基于Teams权限。</span><span class="sxs-lookup"><span data-stu-id="cd68e-154">In version 2.2, the required permissions have been updated to the less restrictive Teams-based permissions.</span></span> <span data-ttu-id="cd68e-155">若要避免发生意外更改，您需要通过全局配置选择加入新权限。</span><span class="sxs-lookup"><span data-stu-id="cd68e-155">To avoid a breaking change, you need to opt in to the new permissions via a global config.</span></span>

```ts
import {MgtTeamsChannelPicker} from "@microsoft/mgt-components";

MgtTeamsChannelPicker.config.useTeamsBasedScopes = true;
```

<span data-ttu-id="cd68e-156">设置为 `useTeamsBasedScopes` `true` 时，Teams选取器将使用以下范围。</span><span class="sxs-lookup"><span data-stu-id="cd68e-156">With `useTeamsBasedScopes` set to `true`, the Teams Channel Picker will use the following scopes.</span></span> 

| <span data-ttu-id="cd68e-157">API</span><span class="sxs-lookup"><span data-stu-id="cd68e-157">API</span></span>                                                                                                              | <span data-ttu-id="cd68e-158">权限</span><span class="sxs-lookup"><span data-stu-id="cd68e-158">Permission</span></span>  |
| ---------------------------------------------------------------------------------------------------------------- | ----------- |
| [<span data-ttu-id="cd68e-159">/me/joinedTeams</span><span class="sxs-lookup"><span data-stu-id="cd68e-159">/me/joinedTeams</span></span>](/graph/api/user-list-joinedteams)                    | <span data-ttu-id="cd68e-160">Team.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="cd68e-160">Team.ReadBasic.All</span></span>        |
| [<span data-ttu-id="cd68e-161">/teams/${id}/channels</span><span class="sxs-lookup"><span data-stu-id="cd68e-161">/teams/${id}/channels</span></span>](/graph/api/channel-list) | <span data-ttu-id="cd68e-162">Channel.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="cd68e-162">Channel.ReadBasic.All</span></span>        |

<span data-ttu-id="cd68e-163">这些权限将是下一个主要更新中的默认权限。</span><span class="sxs-lookup"><span data-stu-id="cd68e-163">These will be the default permissions in the next major update.</span></span>

## <a name="authentication"></a><span data-ttu-id="cd68e-164">身份验证</span><span class="sxs-lookup"><span data-stu-id="cd68e-164">Authentication</span></span>

<span data-ttu-id="cd68e-165">该控件使用身份验证文档中所述的全局 [身份验证提供程序](../providers/providers.md)。</span><span class="sxs-lookup"><span data-stu-id="cd68e-165">The control uses the global authentication provider described in the [authentication documentation](../providers/providers.md).</span></span>

## <a name="cache"></a><span data-ttu-id="cd68e-166">缓存</span><span class="sxs-lookup"><span data-stu-id="cd68e-166">Cache</span></span>

<span data-ttu-id="cd68e-167">`mgt-teams-channel-picker`组件不缓存任何数据。</span><span class="sxs-lookup"><span data-stu-id="cd68e-167">The `mgt-teams-channel-picker` component doesn't cache any data.</span></span>

## <a name="extend-for-more-control"></a><span data-ttu-id="cd68e-168">扩展以了解更多控件</span><span class="sxs-lookup"><span data-stu-id="cd68e-168">Extend for more control</span></span>

<span data-ttu-id="cd68e-169">对于更复杂的方案或真正自定义的 UX，此组件公开了多个在组件扩展 `protected render*` 中替代的方法：</span><span class="sxs-lookup"><span data-stu-id="cd68e-169">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions:</span></span>

| <span data-ttu-id="cd68e-170">方法</span><span class="sxs-lookup"><span data-stu-id="cd68e-170">Method</span></span> | <span data-ttu-id="cd68e-171">说明</span><span class="sxs-lookup"><span data-stu-id="cd68e-171">Description</span></span> |
| - | - |
| <span data-ttu-id="cd68e-172">renderSelected</span><span class="sxs-lookup"><span data-stu-id="cd68e-172">renderSelected</span></span> | <span data-ttu-id="cd68e-173">在输入框中呈现选定的团队和频道。</span><span class="sxs-lookup"><span data-stu-id="cd68e-173">Renders the selected team and channel in the input box.</span></span> |
| <span data-ttu-id="cd68e-174">renderInput</span><span class="sxs-lookup"><span data-stu-id="cd68e-174">renderInput</span></span> | <span data-ttu-id="cd68e-175">呈现输入框。</span><span class="sxs-lookup"><span data-stu-id="cd68e-175">Renders the input box.</span></span> |
| <span data-ttu-id="cd68e-176">renderDropdown</span><span class="sxs-lookup"><span data-stu-id="cd68e-176">renderDropdown</span></span> | <span data-ttu-id="cd68e-177">呈现下拉列表。</span><span class="sxs-lookup"><span data-stu-id="cd68e-177">Renders the dropdown.</span></span> |
| <span data-ttu-id="cd68e-178">renderDropdownList</span><span class="sxs-lookup"><span data-stu-id="cd68e-178">renderDropdownList</span></span> | <span data-ttu-id="cd68e-179">以递归方法呈现下拉列表中的项。</span><span class="sxs-lookup"><span data-stu-id="cd68e-179">Renders the items in the dropdown recursively.</span></span> |
| <span data-ttu-id="cd68e-180">renderItem</span><span class="sxs-lookup"><span data-stu-id="cd68e-180">renderItem</span></span> | <span data-ttu-id="cd68e-181">在下拉列表中呈现团队或频道。</span><span class="sxs-lookup"><span data-stu-id="cd68e-181">Renders a team or a channel in the dropdown list.</span></span> |
| <span data-ttu-id="cd68e-182">renderHighlightedText</span><span class="sxs-lookup"><span data-stu-id="cd68e-182">renderHighlightedText</span></span> | <span data-ttu-id="cd68e-183">呈现通道文本，突出显示输入查询。</span><span class="sxs-lookup"><span data-stu-id="cd68e-183">Renders the channel text, highlighting the input query.</span></span> |
| <span data-ttu-id="cd68e-184">renderLoading</span><span class="sxs-lookup"><span data-stu-id="cd68e-184">renderLoading</span></span> | <span data-ttu-id="cd68e-185">呈现加载下拉列表状态。</span><span class="sxs-lookup"><span data-stu-id="cd68e-185">Renders the loading dropdown state.</span></span> |
| <span data-ttu-id="cd68e-186">renderError</span><span class="sxs-lookup"><span data-stu-id="cd68e-186">renderError</span></span> | <span data-ttu-id="cd68e-187">呈现下拉列表错误状态。</span><span class="sxs-lookup"><span data-stu-id="cd68e-187">Renders the dropdown error state.</span></span> |
