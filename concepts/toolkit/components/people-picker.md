---
title: People-Picker组件
description: 可以使用 mgt-people-picker Web 组件搜索指定数量的人员，并通过 Microsoft Graph 呈现结果列表。
ms.localizationpriority: medium
author: sebastienlevert
ms.openlocfilehash: 4cc135fef448ecadc67a0ad1ba93e5be609d1258
ms.sourcegitcommit: 5516b107d72caef6ec042fe74228be4031b32fa5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2022
ms.locfileid: "65060708"
---
# <a name="people-picker-component-in-the-microsoft-graph-toolkit"></a>Microsoft Graph Toolkit中的People-Picker组件

可以使用 `mgt-people-picker` Web 组件搜索人员和/或组。 默认情况下，组件将搜索组织中的所有人员和用户，但你可以将行为更改为同时搜索组或仅搜索组。 还可以将搜索筛选为特定组。 此外，你可以允许用户输入并选择任何电子邮件地址。

## <a name="example"></a>示例

下面的示例显示了组 `mgt-people-picker` 件。 开始搜索名称以查看结果呈现，并使用代码编辑器查看 [属性](#properties) 如何更改组件的行为。

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-people-picker--people-picker&source=docs" height="450"></iframe>

[在 mgt.dev 中打开此示例](https://mgt.dev/?path=/story/components-mgt-people-picker--people-picker&source=docs)

## <a name="properties"></a>属性

默认情况下，组 `mgt-people-picker` 件从 `/me/people` 终结点和 `/users` 终结点提取人员。 使用以下属性更改此行为。

| 属性 | 属性 | 说明                                                                                                                                                                            |
| -------- | --------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| show-max | showMax   | 一个数字值，用于指示要显示的最大人数。 默认值为 6。                                                                                             |
| group-id    | groupId     | 属于 Microsoft Graph定义组的字符串值，用于进一步筛选搜索结果。                                                                            |
| transitive-search     | transitiveSearch      | 用于执行可传递搜索的布尔值返回所有嵌套成员的平面列表 - 默认情况下不使用可传递搜索。|
| type     | type      | 要搜索的实体的类型。 可用选项为： `person`， ， `group`。 `any` 默认值为 `person`。 如果 `group-id` 设置了属性，则此属性无效。         
| user-type     | userType      | 要搜索的用户的类型。 可用选项包括： `any`组织 `user` 用户或 `contact` 联系人。 默认值为 `any`。 |
| group-type     | groupType      | 要搜索的组类型。 可用选项为： `unified`， `security`， `mailenabledsecurity`， ， `distribution`。 `any` 默认值为 `any`。 如果属性设置为`person`，`type`则此属性不起作用。  |
| selected-people  | selectedPeople     | 选定人员的数组。 设置此值以以编程方式选择人员。|
| people   | people    | 在搜索结果中找到和呈现的人员数组 |
| 占 位 符   | 占 位 符    | 用于解释如何使用组件的默认文本。 默认值为 `Start typing a name`。
| default-selected-user-ids | defaultSelectedUserIds | 当提供逗号分隔的 Microsoft Graph用户 ID 字符串时，组件会在初始化时呈现所选的相应用户。
| default-selected-group-ids | defaultSelectedGroupIds | 与默认的 selected-user-id 类似，当提供逗号分隔的 Microsoft Graph 组 ID 字符串时，组件会在初始化时呈现所选的相应组。
| selection-mode | selectionMode | 用于指示是允许选择多个项目 (用户或组) 还是只选择单个项目。 可用选项包括： `single`. `multiple` 默认值为 `multiple`。
| 禁用 | 禁用 | 设置是否禁用人员选取器。 禁用后，用户无法搜索或选择人员。
| disable-images | disableImages | 设置是否禁用人员图像的提取和显示。 设置为 `true`时，将改为显示用户首字母缩写。
| allow-any-email | allowAnyEmail | 指示人员选取器是否可以在不选择人员的情况下接受电子邮件地址。 默认值为 `false`。 键入电子邮件地址后，可以按逗号 () `,` 、分号 (`;`) 、选项卡或输入键来添加它。
| user-ids | userIds | 逗号分隔用户 ID 字符串。 只有在键入查询时，它们才会显示在下拉菜单或搜索结果上。 例如 `48d31887-5fad-4d73-a9f5-3c356e68a038,24fcbca3-c3e2-48bf-9ffc-c7f81b81483d` ，仅当输入处于焦点时，才会在下拉列表中显示这两个用户。 键入搜索文本时，它将返回仅与两个用户 ID 中的用户匹配的结果。
| user-filters | userFilters | 指定查询用户终结点时要使用的筛选条件。 它要求 `user-type` 设置为 `user` 或 `contact`。 默认情况下， `user-type` 是 `any` 且这会导致查询在终结点块中 `people` 进行。 示例：`user-filters="startsWith(displayName,'a')"`。 此特性是可选的。 详细了解如何[支持筛选Azure AD目录对象的用户属性](/graph/aad-advanced-queries?tabs=http#user-properties)。
| group-filters | groupFilters | 指定查询终结点时 `groups` 要使用的筛选条件。 它需要 `type` 设置为 `group`。 示例：`group-filters="startsWith(displayName,'a')"`。 此特性是可选的。
| people-filters | peopleFilters | 指定查询终结点时 `people` 要使用的筛选条件。 它按其方式使用。 示例：`people-filters="jobTitle eq 'Web Marketing Manager'"`。 此特性是可选的。 详细了解 [人员资源上的筛选和支持的功能](/graph/people-example)。
| group-ids | groupIds | 逗号分隔组 ID 的字符串。 可用结果应限制为指定的组。 将显示在下拉菜单上并通过搜索体验显示的用户应仅来自指定的组 ID。 例如， `02bd9fd6-8f93-4758-87c3-1fb73740a315,06f62f70-9827-4e6e-93ef-8e0f2d9b7b23` 将仅显示属于这些组的用户。 键入搜索文本时，它将返回仅与两个组 ID 中的用户匹配的结果。 如果 `group-id` 定义了此属性，则不使用此属性。 如果设置了该属性，`type`则默认情况下为`group`默认`true``trnsitive-search`值。 如果使用 `group-type` 属性设置该属性， `type` 则可以是 `any` 或 `group`。 `type`如果是`person`，则不使用该属性。

下面是一个 `show-max` 示例。

```html
<mgt-people-picker show-max="4"> </mgt-people-picker>
```

## <a name="selected-people"></a>所选人员

组件的选定人员部分呈现开发人员或用户选择的每个人。 

![mgt-people-picker](./images/selected-people.png)

可以通过执行以下操作之一来填充所选人员数据：

- 直接设置属性 `selectedPeople` ，如以下示例所示。  

    ```javascript
    // personObject = User or Person from Microsoft Graph
    document.querySelector('mgt-people-picker').selectedPeople.push(personObject);
    ```

- 使用该 `selectUsersById()` 方法，该方法接受 Microsoft graph [用户 ID](/graph/api/resources/users) 的数组，以查找所选内容的相关用户详细信息。

     >**注意：** 如果找不到 `id`用户，则不会为此 `id`呈现任何数据。

    ```javascript
    // id = Microsoft graph User "id"
    document.querySelector('mgt-people-picker').selectUsersById(["id","id"])
    ```

- `selectGroupsById()`使用该方法，该方法接受 Microsoft graph [组 ID](/graph/api/resources/group) 的数组，以查找组 (与关联用户) 。

    ```javascript
    // groupid = Microsoft graph group "id"
    document.querySelector('mgt-people-picker').selectGroupsById(["groupid","groupid"])
    ```

## <a name="events"></a>活动

从组件触发以下事件。

Event | 何时发出 | 自定义数据 | 可取消 | 泡沫 | 使用自定义模板
------|-------------------|--------------|:-----------:|:---------:|:---------------------------:|
`selectionChanged` | 用户从选定/选定人员列表中添加或删除了一个人 | 所选人员的数组，其中一个人可以是Graph[用户](/graph/api/resources/user)、[人员](/graph/api/resources/person)或[与](/graph/api/resources/contact)包含用户照片 URL 的其他`personImage`属性的联系人 | 否 | 否 | 是，除非重写默认模板

有关处理事件的详细信息，请参阅 [事件](../customize-components/events.md)。

## <a name="css-custom-properties"></a>CSS 自定义属性

该 `mgt-people-picker` 组件定义以下 CSS 自定义属性。

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

 `mgt-people-picker` 支持多个 [模板](../customize-components/templates.md) ，可用于替换组件的某些部分。 若要指定模板，请在组件中包含一个 `<template>` 元素， `data-type` 并将值设置为下列值之一。

| 数据类型 | 数据上下文 | 说明 |
| --- | --- | --- |
| 默认 | null：无数据 | 用于替代整个组件呈现的模板。
| 加载 | null：无数据 | 发出图形请求时用于呈现选取器状态的模板。 |
| error | null：无数据 | 如果用户搜索不返回任何用户，则使用的模板。 |
| no-data | null：无数据 | 如果用户搜索不返回任何用户，则使用替代模板。 |
| selected-person | 人员：人员详细信息对象 | 用于呈现所选人员的模板。 |
| 人 | 人员：人员详细信息对象 | 用于在下拉列表中呈现人员的模板。 |

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

| 配置 | 权限 | API
| --- | ---------- | ------- |
| `group-id` 设置 | People.Read、User.Read.All、GroupMember.Read.All | [/groups/\${groupId}/members](/graph/api/group-list-members) |
| `type` 设置为 `Person` 或 `any` | People.Read | [/me/people](/graph/api/user-list-people) |
| `type` 设置为 `Group` 或搜索用户并 `type` 设置为 `Group` 或 `any` | Group.Read.All | [/groups](/graph/api/group-list) |
| `default-selected-user-ids` 设置 | User.ReadBasic.All | [/users](/graph/api/user-list) |
| 搜索用户并 `type` 设置为 `Person` 或 `any` | People.Read、User.ReadBasic.All | [/me/people](/graph/api/user-list-people)、 [/users](/graph/api/user-list) |

## <a name="authentication"></a>身份验证

该控件使用 [身份验证文档](../providers/providers.md)中所述的全局身份验证提供程序。

## <a name="cache"></a>缓存

|对象存储|缓存的数据|备注|
|---------|-----------|-------|
|`groups`|组列表|将时间 `type` 设置为 `PersonType.group`|
|`people`|人员列表|`type`何时设置为`PersonType.person`或`PersonType.any`|
|`users`|用户列表|指定时 `groupId` 使用|

有关如何配置缓存的更多详细信息，请参阅[Caching](../customize-components/cache.md)。

## <a name="extend-for-more-control"></a>扩展以获得更多控制

对于更复杂的方案或真正自定义的 UX，此组件公开了用于在组件扩展中重写的几 `protected render*` 种方法。

| 方法 | 说明 |
| - | - |
| renderInput | 呈现输入文本框。 |
| renderSelectedPeople | 呈现所选人员令牌。 |
| renderSelectedPerson | 呈现个人令牌。 |
| renderFlyout | 呈现浮出控件部件版式。 |
| renderFlyoutContent | 在结果浮出控件中呈现适当的状态。 |
| renderLoading | 呈现加载状态。 |
| renderNoData | 在未找到搜索查询的结果时呈现状态。 |
| renderSearchResults | 呈现搜索结果列表。 |
| renderPersonResult | 呈现个人搜索结果。 |
