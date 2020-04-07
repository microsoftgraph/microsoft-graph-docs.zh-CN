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
# <a name="person-card-component-in-the-microsoft-graph-toolkit"></a>Microsoft Graph 工具包中的个人卡片组件

个人卡片组件是一个响应性组件，用于显示与人员相关的更多信息。 它通常用作`mgt-person`组件上的浮出控件。

有关`mgt-person`组件的详细信息，请参阅 "[管理员文档](./person.md)"。

## <a name="example"></a>示例

下面的示例演示组件与组件的`mgt-person-card`配合`mgt-person`使用。 将鼠标悬停在人员上以查看人员卡片，并使用代码编辑器查看[属性](#properties)如何更改组件的行为。
  
<iframe src="https://mgt.dev/iframe.html?id=components-mgt-person-card--person-card-hover&source=docs" height="400"></iframe>

[在 "dev" 中打开此示例](https://mgt.dev/?path=/story/components-mgt-person-card--person-card-hover&source=docs)

## <a name="setup-for-teams-integrations"></a>团队集成设置

"人员-卡片" 组件允许用户联系目标人员，包括通过团队聊天。 如果在团队选项卡应用程序中使用组件，则可以确保组件深度链接直接链接到聊天，而不是通过设置`microsoftTeamsLib`中`TeamsProvider`的打开浏览器窗口。

如果人员卡片组件无法检测到团队库，组件将尝试改为打开团队 web 客户端。

```ts
import * as MicrosoftTeams from "@microsoft/teams-js/dist/MicrosoftTeams";
import {TeamsHelper} from '@microsoft/mgt';

TeamsHelper.microsoftTeamsLib = MicrosoftTeams;
```

有关`TeamsProvider`提供程序的详细信息，请参阅[Microsoft 团队提供商](../providers/teams.md)。

## <a name="properties"></a>属性

默认情况下， `mgt-person`组件会将人员详细信息传递给`mgt-person-card`组件。 但是，在对`mgt-person`组件进行模板化或使用`mgt-person-card`组件作为独立组件时，可以使用这些属性来更改此属性。

| 属性         | 类型                     | 说明                                                                           |
| ---------------- | -------------------------------- | ------------------------------------------------------------------------------------- |
| 人员-详细信息 | MicrosoftGraph <br> MicrosoftGraph <br> MicrosoftGraph。联系人 | 由 Microsoft Graph 定义的 Person 对象，包含与用户相关的详细信息。 |
| 人员-图像   | png/jpg/svg                    | 与卡片中显示的人员相关的图像。                                   |
| 继承-详细信息   | 无。                  | 允许人员卡片遍历父树 for `mgt-person` component 以使用相同`person-details`和`person-image`数据。                      |
| 用户 id | string | 允许开发人员提供用户 id 以检索在人员卡片组件上显示的数据 |
| 人员-查询 | string | 允许开发人员提供人员查询以检索在人员卡片组件上显示的数据 |


## <a name="templates"></a>模板

人员卡片组件使用允许您添加或替换部分组件的[模板](../templates.md)。 若要指定模板，请在`<template>`组件内添加一个元素，并将`data-type`值设置为下列值之一。

| 数据类型 | 数据上下文 | 说明 |
| - | - | - |
| 无数据 | 空 | 没有可用数据时使用的模板。
| 设置 | `person`： Person details 对象 <br> `personImage`：图像的 URL | 默认模板会将整个组件替换为您自己的组件。 |
| 人员-详细信息 | `person`： Person details 对象 | 用于呈现个人卡片顶部部分的模板。 |
| 联系人-详细信息 | `person`： Person details 对象 | 用于替代其他详细信息容器的联系人详细信息部分的模板。 |
| 其他详细信息 | `person`： Person details 对象 <br> `personImage`：图像的 URL | 用于将自定义内容添加到其他详细信息容器的模板。 |

例如，可以使用模板自定义附加到`mgt-person`组件的组件和模板，以在卡片中添加其他详细信息。 

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

## <a name="css-custom-properties"></a>CSS 自定义属性

`mgt-person-card`组件定义以下 CSS 自定义属性。 若要使用这些属性，必须将选择器定义为父`mgt-person`元素。 

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

若要了解详细信息，请参阅[样式组件](../style.md)。

## <a name="microsoft-graph-permissions"></a>Microsoft Graph 权限

此组件使用 "[人员" 组件](./person.md)显示用户并继承所有权限。 

## <a name="authentication"></a>身份验证

个人卡片控件使用[身份验证文档](./../providers.md)中所述的全局身份验证提供程序。 

## <a name="extend-for-more-control"></a>扩展以实现更多控制

对于更复杂的方案或真正的自定义 UX，此组件`protected render*`将公开几种用于在组件扩展中进行重写的方法。

| 方法 | 说明 |
| - | - |
| renderNoData | 在无人数据可用时呈现状态。 | 
| renderPersonDetails | 呈现人员卡片的主要正文（图像、名称、图标）。 |
| renderPersonImage | 呈现人员详细信息的图像部分。 |
| renderPersonName | 呈现人员详细信息的名称部分。 |
| renderPersonTitle | 呈现人员详细信息的标题部分。 |
| renderPersonSubtitle | 呈现人员详细信息的副标题部分。 |
| renderContactIcons | 呈现 "人员详细信息" 的 "联系人" 图标部分。 |
| renderExpandedDetailsButton | 呈现按钮以显示展开的详细信息。 |
| renderExpandedDetails | 在展开的详细信息容器中呈现内容。 |
| renderContactDetails | 呈现展开的详细信息的 "联系人详细信息" 部分。 |
| renderAdditionalDetails | 呈现展开的详细信息的其他详细信息部分。 |
