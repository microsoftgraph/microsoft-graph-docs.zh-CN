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
# <a name="microsoft-teams-channel-picker-component-in-the-microsoft-graph-toolkit"></a>Microsoft Graph 中 Microsoft Teams 频道选取器Toolkit

可以使用该组件 `mgt-teams-channel-picker` 启用与用户关联的 Microsoft Teams 频道的搜索。 组件可以搜索用户已加入的所有团队，以及这些团队中的每个频道。 

## <a name="example"></a>示例

以下示例显示 `mgt-teams-channel-picker` 组件。 开始搜索频道或团队以查看结果呈现。

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-teams-channel-picker--teams-channel-picker&source=docs" height="450"></iframe>

[在 mgt.dev 中打开此示例](https://mgt.dev/?path=/story/components-mgt-teams-channel-picker--teams-channel-picker&source=docs)

## <a name="getting-the-selected-channel"></a>获取所选频道

使用 `selectedItem` 该属性可检索当前选定的频道和父团队。 如果未选择任何通道，则此值将为 null。 `selectedItem` 包含两个 `channel` 属性： ([MicrosoftGraph.Channel](/graph/api/resources/channel)) 和 `team` ([MicrosoftGraph.Team](/graph/api/resources/team)) 。

```javascript
const channelPicker = document.querySelector('mgt-teams-channel-picker');
console.log(channelPicker.selectedItem.channel);
console.log(channelPicker.selectedItem.team);
```

## <a name="selecting-a-channel"></a>选择频道

使用此方法 `selectChannelById(channelId: string)` 以编程方式选择频道。

> **注意：Teams** 频道选取器仅支持单个频道选择。

```javascript
const channelPicker = document.querySelector('mgt-teams-channel-picker');
const channelId = 'some-channel-id';
channelPicker.selectChannelById(channelId);
```

> **注意：** 提供的频道 (和后续 ID) 必须属于经过身份验证的用户已加入的团队。 


## <a name="css-custom-properties"></a>CSS 自定义属性

该 `mgt-teams-channel-picker` 组件定义以下 CSS 自定义属性。

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

## <a name="events"></a>活动
| 事件 | 详情 | 说明 |
| --- | --- | --- |
| selectionChanged | 详细信息包含 `{channel : ` [MicrosoftGraph.Channel](/graph/api/resources/channel) `, team: ` [MicrosoftGraph.Team 当前选定的项目](/graph/api/resources/team)`}` | 当用户对频道的选择做出更改时触发。 |

## <a name="templates"></a>模板

 `mgt-teams-channel-picker` 支持 [多个模板](../customize-components/templates.md) ，您可以使用这些模板替换组件的某些部分。 若要指定模板，请包含 `<template>` 组件中的元素，将值设置为下列 `data-type` 值之一。

| 数据类型 | 数据上下文 | 说明 |
| --- | --- | --- |
| loading | null：无数据 | 在向 Microsoft Graph 提出请求时用于呈现选取器状态的模板。 |
| error | null：无数据| 如果用户搜索未返回任何用户，则使用的模板。 |


以下示例显示如何使用 `error` 模板。

```html
<mgt-teams-channel-picker>
  <template data-type="error">
    <p>Sorry, no Teams or Channels were found</p>
  </template>
</mgt-teams-channel-picker>
```

## <a name="microsoft-graph-permissions"></a>Microsoft Graph 权限

此组件使用以下 Microsoft Graph API 和权限。

| API                                                                                                              | 权限  |
| ---------------------------------------------------------------------------------------------------------------- | ----------- |
| [/me/joinedTeams](/graph/api/user-list-joinedteams)                    | User.Read.All        |
| [/teams/${id}/channels](/graph/api/channel-list) | Group.Read.All        |

## <a name="authentication"></a>身份验证

该控件使用身份验证文档中介绍的全局 [身份验证提供程序](../providers/providers.md)。

## <a name="extend-for-more-control"></a>扩展以更多控制

对于更复杂的方案或真正自定义的 UX，此组件公开了多个在组件扩展中 `protected render*` 替代的方法：

| 方法 | 说明 |
| - | - |
| renderSelected | 在输入框中呈现选定的团队和频道。 |
| renderInput | 呈现输入框。 |
| renderDropdown | 呈现下拉列表。 |
| renderDropdownList | 以递归方法呈现下拉列表中的项。 |
| renderItem | 在下拉列表中呈现团队或频道。 |
| renderHighlightedText | 呈现通道文本，突出显示输入查询。 |
| renderLoading | 呈现加载下拉列表状态。 |
| renderError | 呈现下拉列表错误状态。 |
