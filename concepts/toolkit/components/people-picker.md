---
title: 人员-选取器组件
description: 您可以使用 "人员-选取器 web 组件" 搜索指定数量的人员，并通过 Microsoft Graph 呈现结果列表。
localization_priority: Normal
author: vogtn
ms.openlocfilehash: 175370b3c00ebaef0db85912c032898e2dacb5e7
ms.sourcegitcommit: 1bc5a0c179dce57e90349610566fb86e1b5fbf95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/04/2020
ms.locfileid: "43144301"
---
# <a name="people-picker-component-in-the-microsoft-graph-toolkit"></a>Microsoft Graph 工具包中的人员选取器组件

您可以使用`mgt-people-picker` web 组件搜索指定数量的人员，并通过 Microsoft Graph 呈现结果列表。 默认情况下，组件将搜索所有人员;您还可以定义组属性以进一步筛选结果。

如果要显示的用户数超过此`show-max`值，则不会在搜索列表中显示所有返回的人员数。

## <a name="example"></a>示例

下面的示例演示了`mgt-people-picker`该组件。 开始搜索名称以查看结果呈现，并使用代码编辑器查看[属性](#properties)如何更改组件的行为。

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-people-picker--people-picker&source=docs" height="450"></iframe>

[在 "dev" 中打开此示例](https://mgt.dev/?path=/story/components-mgt-people-picker--people-picker&source=docs)

## <a name="properties"></a>属性

默认情况下， `mgt-people-picker`组件从`/me/people`终结点提取事件。 使用以下属性来更改此行为。

| 属性 | 属性 | 说明                                                                                                                                                                            |
| -------- | --------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| show-max | showMax   | 一个指示要显示的最大用户数的数字值。 默认值为6。                                                                                             |
| people   | people    | 获取或设置组件呈现的人员列表的人员数组。 使用此属性可访问组件加载的人员。 设置此值可加载自己的人员。 |
| group    | group     | 一个 string 值，属于 Microsoft Graph 定义的组，用于进一步筛选搜索结果。                                                                            |
|  选定-人员  | selectedPeople     | 一个类型`person`的数组，表示在组件中选定的人员。 将此值设置为 "默认情况下选择所选人员"。|

下面是一个`show-max`示例。

```html
<mgt-people-picker show-max="4"> </mgt-people-picker>
```

## <a name="selected-people"></a>选定人员

组件的 "选定人员" 部分将呈现由开发人员或用户选择的每个人。 

![组织-人员-选取器](./images/selected-people.png)

您可以通过执行下列操作之一来填充所选的人员数据：

- 直接设置`selectedPeople`属性，如下面的示例所示。  

    ```javascript
    // personObject = User or Person from Microsoft Graph
    document.querySelector('mgt-people-picker').selectedPeople.push(personObject);
    ```

- 使用此`selectUsersById()`方法可接受 Microsoft graph[用户 id](https://docs.microsoft.com/graph/api/resources/users?view=graph-rest-1.0)的数组，以查找有关所选内容的相关用户详细信息。

     >**注意：** 如果找不到用户，则`id`不会为其呈现任何数据`id`。

    ```javascript
    // id = Mirosoft graph User "id"
    document.querySelector('mgt-people-picker').selectUsersById(["id","id"])
    ```

## <a name="css-custom-properties"></a>CSS 自定义属性

`mgt-people-picker`组件定义以下 CSS 自定义属性。

```css
mgt-people-picker {
  --people-list-background-color: blue; /* Background-color for people under search */
  --accent-color: green; /* Color for separator of search input box and people */
}
```

## <a name="templates"></a>模板

 `mgt-people-picker`支持多个模板，这些[模板](../templates.md)可用于替换组件的某些部分。 若要指定模板，请在`<template>`组件内添加一个元素，并`data-type`将值设置为下列值之一。

| 数据类型 | 数据上下文 | 说明 |
| --- | --- | --- |
| 设置 | null：无数据 | 用于覆盖整个组件的呈现的模板。
| 装载 | null：无数据 | 在发出对 graph 的请求时用于呈现选取器状态的模板。 |
| error | null：无数据 | 用户搜索不返回用户时使用的模板。 |
| 无数据 | null：无数据 | 如果用户搜索不返回用户，则使用备用模板。 |
| 选定的人员 | 人员：人员详细信息对象 | 呈现所选人员的模板。 |
| person | 人员：人员详细信息对象 | 用于在下拉列表中呈现人员的模板。 |

下面的示例演示如何使用`error`模板。

```html
<mgt-people-picker>
  <template data-type="error">
    <p>Sorry, no people were found</p>
  </template>
</mgt-people-picker>
```

## <a name="microsoft-graph-permissions"></a>Microsoft Graph 权限

此组件使用以下 Microsoft Graph Api 和权限。

| API                                                                                                              | 权限  |
| ---------------------------------------------------------------------------------------------------------------- | ----------- |
| [/me/people](/graph/api/user-list-people?view=graph-rest-1.0)                    | People.Read        |
| [/groups/\${groupId}/members](/graph/api/group-list-members?view=graph-rest-1.0) | People.Read        |
| [/users/$ {userPrincipleName}](/graph/api/user-list-people?view=graph-rest-1.0)  | User.readbasic.all |

## <a name="authentication"></a>身份验证

该控件使用[身份验证文档](./../providers.md)中介绍的全局身份验证提供程序。

## <a name="extend-for-more-control"></a>扩展以实现更多控制

对于更复杂的方案或真正的自定义 UX，此组件`protected render*`将公开几种用于在组件扩展中进行重写的方法。

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
