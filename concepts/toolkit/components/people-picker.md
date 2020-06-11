---
title: 人员-选取器组件
description: 您可以使用 "人员-选取器 web 组件" 搜索指定数量的人员，并通过 Microsoft Graph 呈现结果列表。
localization_priority: Normal
author: vogtn
ms.openlocfilehash: e3e656c6aef0ab2af9878fb3e4738ade912c4685
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44681884"
---
# <a name="people-picker-component-in-the-microsoft-graph-toolkit"></a>Microsoft Graph 工具包中的人员选取器组件

您可以使用 `mgt-people-picker` web 组件搜索人员和/或组。 默认情况下，该组件将搜索组织中的所有人员和用户，但您也可以将该行为更改为同时搜索组或仅搜索组。 您还可以将搜索筛选到特定的组。

## <a name="example"></a>示例

下面的示例演示了该 `mgt-people-picker` 组件。 开始搜索名称以查看结果呈现，并使用代码编辑器查看[属性](#properties)如何更改组件的行为。

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-people-picker--people-picker&source=docs" height="450"></iframe>

[在 "dev" 中打开此示例](https://mgt.dev/?path=/story/components-mgt-people-picker--people-picker&source=docs)

## <a name="properties"></a>属性

默认情况下， `mgt-people-picker` 组件从 `/me/people` 和 `/users` 终结点提取人员。 使用以下属性来更改此行为。

| 属性 | 属性 | 说明                                                                                                                                                                            |
| -------- | --------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| show-max | showMax   | 一个指示要显示的最大用户数的数字值。 默认值为6。                                                                                             |
| 组 id    | groupId     | 一个 string 值，属于 Microsoft Graph 定义的组，用于进一步筛选搜索结果。                                                                            |
| type     | type      | 要搜索的实体的类型。 可用选项包括： `person` 、 `group` 、 `any` 。 默认值为 `person`。 如果设置了属性，则此属性不起作用 `group-id` 。                                                                            |
| group 类型     | groupType      | 要搜索的组类型。 可用选项包括： `unified` 、 `security` 、 `mailenabledsecurity` 、 `distribution` 、 `any` 。 默认值为 `any`。 如果该 `type` 属性设置为，则此属性不起作用 `person` 。                                                                           |
|  选定-人员  | selectedPeople     | 选定人员的数组。 将此值设置为以编程方式选择人员。|
| people   | people    | 在搜索结果中找到并呈现的人员的数组 |

下面是一个 `show-max` 示例。

```html
<mgt-people-picker show-max="4"> </mgt-people-picker>
```

## <a name="selected-people"></a>选定人员

组件的 "选定人员" 部分将呈现由开发人员或用户选择的每个人。 

![组织-人员-选取器](./images/selected-people.png)

您可以通过执行下列操作之一来填充所选的人员数据：

- 直接设置 `selectedPeople` 属性，如下面的示例所示。  

    ```javascript
    // personObject = User or Person from Microsoft Graph
    document.querySelector('mgt-people-picker').selectedPeople.push(personObject);
    ```

- 使用此 `selectUsersById()` 方法可接受 Microsoft graph[用户 id](https://docs.microsoft.com/graph/api/resources/users?view=graph-rest-1.0)的数组，以查找有关所选内容的相关用户详细信息。

     >**注意：** 如果找不到用户，则 `id` 不会为其呈现任何数据 `id` 。

    ```javascript
    // id = Mirosoft graph User "id"
    document.querySelector('mgt-people-picker').selectUsersById(["id","id"])
    ```

## <a name="events"></a>活动

将从组件中触发以下事件。

| 事件 | 说明 |
| --- | --- |
| `selectionChanged` | 用户在所选/选取的人员列表中添加或删除了人员。|

## <a name="css-custom-properties"></a>CSS 自定义属性

`mgt-people-picker`组件定义以下 CSS 自定义属性。

```css
mgt-people-picker {
    --input-border: 2px rgba(255, 255, 255, 0.5) solid; /* sets all input area border */

      /* OR individual input border sides */
    --input-border-bottom: 2px rgba(255, 255, 255, 0.5) solid;
    --input-border-right: 2px rgba(255, 255, 255, 0.5) solid;
    --input-border-left: 2px rgba(255, 255, 255, 0.5) solid;
    --input-border-top: 2px rgba(255, 255, 255, 0.5) solid;

    --input-background-color: #1f1f1f; /* input area background color */
    --input-hover-color: #008394; /* input area border hover color */
    --input-focus-color: #0f78d4; /* input area border focus color */

    --dropdown-background-color: #1f1f1f; /* selection area background color */
    --dropdown-item-hover-background: #333d47; /* person background color on hover */

    --font-color: white; /* input area border focus color */
    --placeholder-default-color: #f1f1f1; /* placeholder text color default*/
    --placeholder-focus-color: rgba(255, 255, 255, 0.8); /* placeholder text focus color */
}
```

## <a name="templates"></a>模板

 `mgt-people-picker`支持多个模板，这些[模板](../templates.md)可用于替换组件的某些部分。 若要指定模板，请在 `<template>` 组件内添加一个元素，并将 `data-type` 值设置为下列值之一。

| 数据类型 | 数据上下文 | Description |
| --- | --- | --- |
|  默认值 | null：无数据 | 用于覆盖整个组件的呈现的模板。
| 装载 | null：无数据 | 在发出对 graph 的请求时用于呈现选取器状态的模板。 |
| error | null：无数据 | 用户搜索不返回用户时使用的模板。 |
| 无数据 | null：无数据 | 如果用户搜索不返回用户，则使用备用模板。 |
| 选定的人员 | 人员：人员详细信息对象 | 呈现所选人员的模板。 |
| 朋友 | 人员：人员详细信息对象 | 用于在下拉列表中呈现人员的模板。 |

下面的示例演示如何使用 `error` 模板。

```html
<mgt-people-picker>
  <template data-type="error">
    <p>Sorry, no people were found</p>
  </template>
</mgt-people-picker>
```

## <a name="microsoft-graph-permissions"></a>Microsoft Graph 权限

此组件使用以下 Microsoft Graph Api 和权限。

| API                                                                                                              | Permission  |
| ---------------------------------------------------------------------------------------------------------------- | ----------- |
| [/me/people](/graph/api/user-list-people?view=graph-rest-1.0)                    | People.Read        |
| [/users](/graph/api/user-list?view=graph-rest-1.0)  | User.ReadBasic.All |
| [/groups](/group-list?view=graph-rest-beta)  | Group.Read.All |
| [/groups/ \$ {groupId}/members](/graph/api/group-list-members?view=graph-rest-1.0) | User.ReadBasic.All        |
| [/users/$ {userPrincipleName}](/graph/api/user-get?view=graph-rest-1.0)  | User.Read |

## <a name="authentication"></a>身份验证

该控件使用[身份验证文档](./../providers.md)中介绍的全局身份验证提供程序。

## <a name="extend-for-more-control"></a>扩展以实现更多控制

对于更复杂的方案或真正的自定义 UX，此组件将公开几种 `protected render*` 用于在组件扩展中进行重写的方法。

| 方法 | 说明 |
| - | - |
| renderInput | 呈现输入文本框。 |
| renderSelectedPeople | 呈现所选人员标记。 |
| renderSelectedPerson | 呈现单个人员标记。 |
| renderFlyout | 呈现浮出控件的镶边。 |
| renderFlyoutContent | 在 "结果" 浮出控件中呈现适当的状态。 |
| renderLoading | 呈现加载状态。 |
| renderNoData | 在未找到搜索查询的结果时呈现状态。 |
| renderSearchResults | 呈现搜索结果的列表。 |
| renderPersonResult | 呈现单个个人的搜索结果。 |
