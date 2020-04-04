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
# <a name="microsoft-teams-channel-picker-component-in-the-microsoft-graph-toolkit"></a>Microsoft Graph 工具包中的 microsoft 团队频道选取器组件

A 您可以使用`mgt-teams-channel-picker`组件来搜索与用户相关联的 Microsoft 团队频道。 组件可以搜索用户加入的所有团队以及这些团队中的每个频道。 

## <a name="example"></a>示例

下面的示例演示了`mgt-teams-channel-picker`该组件。 开始搜索频道或团队以查看结果呈现。

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-teams-channel-picker--teams-channel-picker&source=docs" height="450"></iframe>

[在 "dev" 中打开此示例](https://mgt.dev/?path=/story/components-mgt-teams-channel-picker--teams-channel-picker&source=docs)

## <a name="getting-the-selected-channel"></a>获取所选频道

使用`selectedItem`属性可检索当前选定的通道和父团队。 如果未选择频道，则此值为 null。 `selectedItem`包含两个属性`channel` ：（[MicrosoftGraph](/graph/api/resources/channel?view=graph-rest-1.0)）和`team` （[MicrosoftGraph](/graph/api/resources/team?view=graph-rest-1.0)）。

```javascript
const channelPicker = document.querySelector('mgt-teams-channel-picker');
console.log(channelPicker.selectedItem.channel);
console.log(channelPicker.selectedItem.team);
```

## <a name="selecting-a-channel"></a>选择通道

使用`selectChannelById(channelId: string)`方法以编程方式选择通道。

> **注意：** 团队频道选取器仅支持单通道选择。

```javascript
const channelPicker = document.querySelector('mgt-teams-channel-picker');
const channelId = 'some-channel-id';
channelPicker.selectChannelById(channelId);
```

> **注意：** 提供的通道（以及后续 ID）必须属于已通过身份验证的用户加入的团队。 


## <a name="css-custom-properties"></a>CSS 自定义属性

`mgt-teams-channel-picker`组件定义以下 CSS 自定义属性。

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

## <a name="events"></a>事件
| 事件 | 详细信息 | 说明 |
| --- | --- | --- |
| selectionChanged | 详细信息包含`{channel : ` [MicrosoftGraph](/graph/api/resources/channel?view=graph-rest-1.0)`, team: `[MicrosoftGraph](/graph/api/resources/team?view=graph-rest-1.0)的当前选定项。`}` | 当用户在选择频道时进行更改时激发。 |

## <a name="templates"></a>模板

 `mgt-teams-channel-picker`支持多个模板，这些[模板](../templates.md)可用于替换组件的某些部分。 若要指定模板，请在`<template>`组件内添加一个元素，并`data-type`将值设置为下列值之一。

| 数据类型 | 数据上下文 | 说明 |
| --- | --- | --- |
| 装载 | null：无数据 | 在发出对 Microsoft Graph 的请求时用于呈现选取器状态的模板。 |
| error | null：无数据| 用户搜索不返回用户时使用的模板。 |


下面的示例演示如何使用`error`模板。

```html
<mgt-teams-channel-picker>
  <template data-type="error">
    <p>Sorry, no Teams or Channels were found</p>
  </template>
</mgt-teams-channel-picker>
```

## <a name="microsoft-graph-permissions"></a>Microsoft Graph 权限

此组件使用以下 Microsoft Graph Api 和权限。

| API                                                                                                              | 权限  |
| ---------------------------------------------------------------------------------------------------------------- | ----------- |
| [/me/joinedTeams](/graph/api/user-list-joinedteams?view=graph-rest-1.0)                    | User.Read.All        |
| [/teams/$ {id}/channels](/graph/api/channel-list?view=graph-rest-1.0) | Group.Read.All        |

## <a name="authentication"></a>身份验证

该控件使用[身份验证文档](./../providers.md)中介绍的全局身份验证提供程序。

## <a name="extend-for-more-control"></a>扩展以实现更多控制

对于更复杂的方案或真正的自定义 UX，此组件`protected render*`将公开几种用于在组件扩展中进行重写的方法：

| 方法 | 说明 |
| - | - |
| renderSelected | 在输入框中呈现选定的团队和频道。 |
| renderInput | 呈现输入框。 |
| renderDropdown | 呈现下拉列表。 |
| renderDropdownList | 以递归方式呈现下拉列表中的项。 |
| renderItem | 在下拉列表中呈现团队或通道。 |
| renderHighlightedText | 呈现通道文本，突出显示输入查询。 |
| renderLoading | 呈现加载下拉列表状态。 |
| renderError | 呈现下拉列表错误状态。 |
