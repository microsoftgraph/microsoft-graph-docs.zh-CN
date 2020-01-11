---
title: 人员-选取器组件
description: 您可以使用 "人员-选取器 web 组件" 搜索指定数量的人员，并通过 Microsoft Graph 呈现结果列表。
localization_priority: Normal
author: vogtn
ms.openlocfilehash: 65ff9382de97ddcd7a0b4bd8a315f8350a80ec35
ms.sourcegitcommit: 2a601cffdb8df375b2ee32a1f35b8f71e0ffd04f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2020
ms.locfileid: "41023122"
---
# <a name="people-picker-component"></a>人员-选取器组件

您可以使用`mgt-people-picker` web 组件搜索指定数量的人员，并通过 Microsoft Graph 呈现结果列表。 默认情况下，组件将搜索所有人员;您还可以定义组属性以进一步筛选结果。

如果要显示的用户数超过此`show-max`值，则不会在搜索列表中显示所有返回的人员数。

## <a name="example"></a>示例

[jsfiddle 示例](https://jsfiddle.net/metulev/jdv38fg0/)

```html
<mgt-people-picker></mgt-people-picker>
```

![组织-人员-选取器](./images/mgt-people-picker-image.png)

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

| 数据类型 | 数据上下文 | Description |
| --- | --- | --- |
| 装载 | null：无数据 | 在发出对 graph 的请求时用于呈现选取器状态的模板。 |
| error | null：无数据| 用户搜索不返回用户时使用的模板。 |
| 选定的人员 |人员：人员详细信息对象| 呈现所选人员的模板。 |
| 朋友 | 人员：人员详细信息对象| 用于在下拉列表中呈现人员的模板。 |

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
