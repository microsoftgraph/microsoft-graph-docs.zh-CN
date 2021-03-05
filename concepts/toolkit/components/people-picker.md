---
title: People-Picker组件
description: 可以使用 mgt-people-picker Web 组件搜索指定数量的人，然后通过 Microsoft Graph 呈现结果列表。
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: c9541130abe8f520b41a0bd4d52de9a167e18c24
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50475182"
---
# <a name="people-picker-component-in-the-microsoft-graph-toolkit"></a>People-Picker Microsoft Graph Toolkit

您可以使用 Web `mgt-people-picker` 组件搜索用户和/或组。 默认情况下，组件将搜索组织中所有用户和用户，但你可以更改行为以同时搜索组或仅搜索组。 您还可以将搜索筛选到特定组。

## <a name="example"></a>示例

以下示例显示 `mgt-people-picker` 组件。 开始搜索名称以查看结果呈现，并使用代码编辑器查看属性 [如何更改组件](#properties) 的行为。

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-people-picker--people-picker&source=docs" height="450"></iframe>

[在 mgt.dev 中打开此示例](https://mgt.dev/?path=/story/components-mgt-people-picker--people-picker&source=docs)

## <a name="properties"></a>属性

默认情况下， `mgt-people-picker` 该组件从和终结点 `/me/people` 提取 `/users` 人员。 使用以下属性可更改此行为。

| 属性 | 属性 | 说明                                                                                                                                                                            |
| -------- | --------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| show-max | showMax   | 一个数字值，指示要显示的最大人数。 默认值为 6。                                                                                             |
| group-id    | groupId     | 一个字符串值，属于 Microsoft Graph 定义的组，用于进一步筛选搜索结果。                                                                            |
| type     | type      | 要搜索的实体的类型。 可用选项有： `person` ， `group` 。 `any` 默认值为 `person`。 如果设置了属性， `group-id` 则此属性无效。         
| transitive-search     | transitiveSearch      | 一个布尔值，用于执行可传递搜索简单列表返回所有嵌套成员的成员的索引 - 默认情况下，不使用可传递搜索。|
| group-type     | groupType      | 要搜索的组类型。 可用选项有： `unified` ， ， ， `security` `mailenabledsecurity` `distribution` `any` 。 默认值为 `any`。 如果该属性设置为 ， `type` 则此属性无效 `person` 。                                                                           |
|  selected-people  | selectedPeople     | 所选人员数组。 设置此值以编程方式选择人员。|
| people   | people    | 在搜索结果中找到并呈现的一组人员 |
| 占位符   | 占位符    | 解释如何使用组件的默认文本。 默认值为 `Start typing a name`。
| default-selected-user-ids | defaultSelectedUserIds | 当提供以逗号分隔的 Microsoft Graph 用户 ID 的字符串时，组件在初始化时将按所选内容呈现相应的用户。
| 选择模式 | selectionMode | 用于指示是允许选择多个项目， (组选择) 单个项目。 可用选项包括： `single` `multiple` 、 。 默认值为 `multiple`。
| 已禁用 | 已禁用 | 设置是否禁用人员选取器。 禁用后，用户将无法搜索或选择人员。

下面是一 `show-max` 个示例。

```html
<mgt-people-picker show-max="4"> </mgt-people-picker>
```

## <a name="selected-people"></a>所选人员

组件的"所选人员"部分呈现开发人员或用户选择的每个人。 

![mgt-people-picker](./images/selected-people.png)

可以通过执行以下操作之一填充所选人员数据：

- 直接 `selectedPeople` 设置属性，如以下示例所示。  

    ```javascript
    // personObject = User or Person from Microsoft Graph
    document.querySelector('mgt-people-picker').selectedPeople.push(personObject);
    ```

- 使用此方法 `selectUsersById()` ，该方法接受 Microsoft graph 用户 [ID](/graph/api/resources/users) 数组，以查找关联的用户详细信息进行选择。

     >**注意：** 如果未找到用户， `id` 则不会为此呈现任何数据 `id` 。

    ```javascript
    // id = Microsoft graph User "id"
    document.querySelector('mgt-people-picker').selectUsersById(["id","id"])
    ```

## <a name="events"></a>活动

从组件中触发以下事件。

| 事件 | 说明 |
| --- | --- |
| `selectionChanged` | 用户在选定/选取人员列表中添加或删除了人员。|

## <a name="css-custom-properties"></a>CSS 自定义属性

组件 `mgt-people-picker` 定义以下 CSS 自定义属性。

```css
mgt-people-picker {
    --input-border: 2px rgba(255, 255, 255, 0.5) solid; /* sets all input area border */

      /* OR individual input border sides */
    --input-border-bottom: 2px rgba(255, 255, 255, 0.5) solid;
    --input-border-right: 2px rgba(255, 255, 255, 0.5) solid;
    --input-border-left: 2px rgba(255, 255, 255, 0.5) solid;
    --input-border-top: 2px rgba(255, 255, 255, 0.5) solid;

    --input-background-color: #1f1f1f; /* input area background color */
    --input-border-color--hover: #008394; /* input area border hover color */
    --input-border-color--focus: #0f78d4; /* input area border focus color */

    --dropdown-background-color: #1f1f1f; /* selection area background color */
    --dropdown-item-hover-background: #333d47; /* person background color on hover */
    
    --selected-person-background-color: #f1f1f1; /* person item background color */
    
    --color: white; /* input area border focus color */
    --placeholder-color: #f1f1f1; /* placeholder text color */
    --placeholder-color--focus: rgba(255, 255, 255, 0.8); /* placeholder text focus color */
}
```

## <a name="templates"></a>模板

 `mgt-people-picker` 支持 [多个模板](../customize-components/templates.md) ，您可以使用这些模板替换组件的某些部分。 若要指定模板，请包含组件 `<template>` 中的元素，将值设置为 `data-type` 下列值之一。

| 数据类型 | 数据上下文 | 说明 |
| --- | --- | --- |
| 默认 | null：无数据 | 用于覆盖整个组件的呈现的模板。
| loading | null：无数据 | 在请求图形时用于呈现选取器状态的模板。 |
| error | null：无数据 | 如果用户搜索未返回任何用户，则使用的模板。 |
| no-data | null：无数据 | 如果用户搜索未返回用户，则使用备用模板。 |
| selected-person | person：人员详细信息对象 | 用于呈现选定人员模板。 |
| person | person：人员详细信息对象 | 在下拉列表中呈现人员模板。 |

以下示例演示如何使用 `error` 模板。

```html
<mgt-people-picker>
  <template data-type="error">
    <p>Sorry, no people were found</p>
  </template>
</mgt-people-picker>
```

## <a name="microsoft-graph-permissions"></a>Microsoft Graph 权限

此组件使用以下 Microsoft Graph API 和权限。

| API                                                                                                              | 权限  |
| ---------------------------------------------------------------------------------------------------------------- | ----------- |
| [/me/people](/graph/api/user-list-people)                    | People.Read        |
| [/users](/graph/api/user-list)  | User.ReadBasic.All |
| [/groups](/group-list)  | Group.Read.All |
| [/groups/ \$ {groupId}/members](/graph/api/group-list-members) | User.ReadBasic.All        |
| [/users/${userPrincipleName} ](/graph/api/user-get)  | User.Read |

## <a name="authentication"></a>身份验证

该控件使用身份验证文档中介绍的全局 [身份验证提供程序](../providers/providers.md)。

## <a name="extend-for-more-control"></a>扩展以更多控制

对于更复杂的方案或真正自定义的 UX，此组件公开了多个在组件扩展 `protected render*` 中替代的方法。

| 方法 | 说明 |
| - | - |
| renderInput | 呈现输入文本框。 |
| renderSelectedPeople | 呈现所选人员令牌。 |
| renderSelectedPerson | 呈现个人个人令牌。 |
| renderFlyout | 呈现飞出部件版式。 |
| renderFlyoutContent | 在结果飞出中呈现相应的状态。 |
| renderLoading | 呈现加载状态。 |
| renderNoData | 当未找到搜索查询的结果时呈现状态。 |
| renderSearchResults | 呈现搜索结果列表。 |
| renderPersonResult | 呈现个人搜索结果。 |
