---
title: People-Picker组件
description: 您可以使用 mgt-people-picker Web 组件搜索指定数量的人，然后通过 Microsoft Graph。
ms.localizationpriority: medium
author: elisenyang
ms.openlocfilehash: 110a28d5c9309d95591e210441784a63208fa02f
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63335365"
---
# <a name="people-picker-component-in-the-microsoft-graph-toolkit"></a>People-Picker Microsoft Graph Toolkit 中的组件

您可以使用 Web 组件 `mgt-people-picker` 来搜索用户和/或组。 默认情况下，组件将搜索组织中所有的用户和用户，但你可以将行为更改为同时搜索组或仅搜索组。 您还可以将搜索筛选到特定组。 此外，还可以允许用户输入并选择任何电子邮件地址。

## <a name="example"></a>示例

以下示例显示组件 `mgt-people-picker` 。 开始搜索名称以查看结果呈现，并使用代码编辑器查看属性 [如何更改组件](#properties) 的行为。

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-people-picker--people-picker&source=docs" height="450"></iframe>

[在 mgt.dev 中打开此示例](https://mgt.dev/?path=/story/components-mgt-people-picker--people-picker&source=docs)

## <a name="properties"></a>属性

默认情况下，组件`mgt-people-picker`从 和 终结点提取`/me/people``/users`人员。 使用以下属性更改此行为。

| 属性 | 属性 | 说明                                                                                                                                                                            |
| -------- | --------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| show-max | showMax   | 一个数字值，指示要显示的最大人数。 默认值为 6。                                                                                             |
| group-id    | groupId     | 一个字符串值，属于 Microsoft Graph定义组，用于进一步筛选搜索结果。                                                                            |
| transitive-search     | transitiveSearch      | 一个布尔值，用于执行可传递搜索，返回简单列表嵌套成员的成员的索引 - 默认情况下，不会使用可传递搜索。|
| type     | type      | 要搜索的实体类型。 可用选项包括：、`person`、`any``group`。 默认值为 `person`。 如果设置了属性，则此属性 `group-id` 无效。         
| user-type     | userType      | 要搜索的用户的类型。 可用选项包括：`any``user`、、组织用户或`contact`联系人。 默认值为 `any`。 |
| group-type     | groupType      | 要搜索的组类型。 可用选项包括：、`unified`、`mailenabledsecurity``security`、`distribution`、`any`。 默认值为 `any`。 如果该属性设置为 ， `type` 则此属性无效 `person`。  |
| selected-people  | selectedPeople     | 所选人员数组。 设置此值以编程方式选择人员。|
| people   | people    | 在搜索结果中找到并呈现的一组人员 |
| 占位符   | 占位符    | 用于说明如何使用该组件的默认文本。 默认值为 `Start typing a name`。
| default-selected-user-ids | defaultSelectedUserIds | 当提供以逗号分隔的 Microsoft Graph ID 字符串时，组件将呈现初始化时选择各自的用户。
| default-selected-group-ids | defaultSelectedGroupIds | 类似于 default-selected-user-ids，当提供以逗号分隔的 Microsoft Graph 组 ID 的字符串时，组件在初始化时将呈现选择各自的组。
| 选择模式 | selectionMode | 用于指示是允许为用户或组选择 (项目，还是) 一个项目。 可用选项包括：、`single``multiple`。 默认值为 `multiple`。
| disabled | disabled | 设置是否禁用人员选取器。 禁用后，用户将无法搜索或选择人员。
| disable-images | disableImages | 设置是否禁用提取和显示人员图像。 设置为 时 `true`，将显示用户缩写。
| allow-any-email | allowAnyEmail | 指示人员选取器是否可以在不选择人员的情况下接受电子邮件地址。 默认值为 `false`。 键入完电子邮件地址后 `,` ，可以按逗号 () `;` ，用分号 () ，按 Tab 键或输入键进行添加。
| user-ids | userIds | 逗号分隔用户 ID 的字符串。 键入查询时，它们只会显示在下拉菜单或搜索结果中。 例如， `48d31887-5fad-4d73-a9f5-3c356e68a038,24fcbca3-c3e2-48bf-9ffc-c7f81b81483d` 当输入已聚焦时，将在下拉列表中仅显示这两个用户。 键入搜索文本时，它将返回仅与两个用户 ID 中的用户匹配的结果。
| user-filters | userFilters | 指定查询用户终结点时使用的筛选条件。 它需要将 `user-type` 设置为 `user` 或 `contact`。 默认情况下，为 `user-type` ， `any` 这将导致在终结点块中 `people` 执行查询。 示例：`user-filters="startsWith(displayName,'a')"`。 此特性是可选的。 详细了解如何[支持筛选目录对象Azure AD属性](/graph/aad-advanced-queries?tabs=http#user-properties)。
| group-filters | groupFilters | 指定查询终结点时使用的筛选 `groups` 条件。 它需要将 `type` 设置为 `group`。 示例：`group-filters="startsWith(displayName,'a')"`。 此特性是可选的。
| people-filters | peopleFilters | 指定查询终结点时使用的筛选 `people` 条件。 它像以前一样使用。 示例：`people-filters="jobTitle eq 'Web Marketing Manager'"`。 此特性是可选的。 详细了解人员 [资源上的筛选和受支持的功能](/graph/people-example)。

下面是一个示例 `show-max` 。

```html
<mgt-people-picker show-max="4"> </mgt-people-picker>
```

## <a name="selected-people"></a>选定人员

组件的"所选人员"部分呈现开发人员或用户选择的每个人。 

![mgt-people-picker](./images/selected-people.png)

可以通过执行以下操作之一填充所选人员数据：

- `selectedPeople`直接设置属性，如以下示例所示。  

    ```javascript
    // personObject = User or Person from Microsoft Graph
    document.querySelector('mgt-people-picker').selectedPeople.push(personObject);
    ```

- `selectUsersById()`使用 方法，该方法接受 Microsoft graph 用户 [ID](/graph/api/resources/users) 数组，以查找关联的用户详细信息进行选择。

     >**注意：** 如果没有为 找到用户 `id`，则不会为此呈现任何数据 `id`。

    ```javascript
    // id = Microsoft graph User "id"
    document.querySelector('mgt-people-picker').selectUsersById(["id","id"])
    ```

- `selectGroupsById()`使用 方法，该方法接受 Microsoft graph 组 [ID](/graph/api/resources/group) 的数组，以查找 (用户) 组。

    ```javascript
    // groupid = Microsoft graph group "id"
    document.querySelector('mgt-people-picker').selectGroupsById(["groupid","groupid"])
    ```

## <a name="events"></a>活动

从组件中触发以下事件。

事件 | 何时发出 | 自定义数据 | Cancelable | 气泡 | 使用自定义模板
------|-------------------|--------------|:-----------:|:---------:|:---------------------------:|
`selectionChanged` | 用户在已选择/已选取人员列表中添加或删除了人员 | 选定人员数组 [](/graph/api/resources/user)[](/graph/api/resources/contact) `personImage`，其中人员可以是包含Graph URL 的其他属性的用户、人员或联系人 [](/graph/api/resources/person) | 否 | 否 | 是，除非您覆盖默认模板

有关处理事件的信息，请参阅 [事件](../customize-components/events.md)。

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

 `mgt-people-picker` 支持 [多个](../customize-components/templates.md) 模板，您可以使用这些模板替换组件的某些部分。 若要指定模板，请包含 `<template>` 组件中的元素，将 `data-type` 值设置为以下值之一。

| 数据类型 | 数据上下文 | 说明 |
| --- | --- | --- |
| default | null：无数据 | 用于替代整个组件的呈现的模板。
| loading | null：无数据 | 在请求图形时用于呈现选取器状态的模板。 |
| error | null：无数据 | 当用户搜索未返回任何用户时所使用的模板。 |
| no-data | null：无数据 | 如果用户搜索未返回任何用户，则使用备用模板。 |
| selected-person | person： The person details object | 用于呈现选定人员的模板。 |
| 人员 | person： The person details object | 下拉列表中用于呈现人员的模板。 |

以下示例演示如何使用模板 `error` 。

```html
<mgt-people-picker>
  <template data-type="error">
    <p>Sorry, no people were found</p>
  </template>
</mgt-people-picker>
```

## <a name="microsoft-graph-permissions"></a>Microsoft Graph 权限

此组件使用下列 Microsoft Graph API 和权限。

| 配置 | 权限 | API
| --- | ---------- | ------- |
| `group-id` set | People.Read、User.Read.All、GroupMember.Read.All | [/groups/\${groupId}/members](/graph/api/group-list-members) |
| `type``Person`设置为 或`any` | People.Read | [/me/people](/graph/api/user-list-people) |
| `type``Group`设置为 或 搜索用户，并`type`设置为 `Group` 或`any` | Group.Read.All | [/groups](/graph/api/group-list) |
| `default-selected-user-ids` set | User.ReadBasic.All | [/users](/graph/api/user-list) |
| 搜索用户，并 `type` 设置为 `Person` 或 `any` | People.Read、User.ReadBasic.All | [/me/people](/graph/api/user-list-people)、 [/users](/graph/api/user-list) |

## <a name="authentication"></a>身份验证

该控件使用身份验证文档中介绍的全局 [身份验证提供程序](../providers/providers.md)。

## <a name="cache"></a>缓存

|对象存储|缓存数据|备注|
|---------|-----------|-------|
|`groups`|组列表|设置为 时 `type` 使用 `PersonType.group`|
|`people`|人员列表|设置为 或 `type` `PersonType.person` 时使用 `PersonType.any`|
|`users`|用户列表|指定时 `groupId` 使用|

请参阅 [Caching](../customize-components/cache.md)，了解有关如何配置缓存的更多详细信息。

## <a name="extend-for-more-control"></a>扩展以了解更多控件

对于更复杂的方案或真正自定义的 UX `protected render*` ，此组件公开了多个在组件扩展中替代的方法。

| 方法 | 说明 |
| - | - |
| renderInput | 呈现输入文本框。 |
| renderSelectedPeople | 呈现所选人员令牌。 |
| renderSelectedPerson | 呈现个人个人令牌。 |
| renderFlyout | 呈现飞出部件版式。 |
| renderFlyoutContent | 在结果飞出控件中呈现相应的状态。 |
| renderLoading | 呈现加载状态。 |
| renderNoData | 当未找到搜索查询的结果时呈现状态。 |
| renderSearchResults | 呈现搜索结果列表。 |
| renderPersonResult | 呈现个人搜索结果。 |
