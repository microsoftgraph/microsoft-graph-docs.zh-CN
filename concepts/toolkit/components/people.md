---
title: Microsoft Graph 工具包中的 "人员" 组件
description: 您可以使用 `mgt-people` web 组件显示一组用户或联系人，方法是使用其照片或缩写。
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 8e942ad0cca446dc8bf982249a7593b8299fe22e
ms.sourcegitcommit: 566d09c17f9d641b6fac9b9159405a3cc41e037b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/20/2020
ms.locfileid: "45183972"
---
# <a name="people-component-in-the-microsoft-graph-toolkit"></a>Microsoft Graph 工具包中的 "人员" 组件

您可以使用 `mgt-people` web 组件显示一组用户或联系人，方法是使用其照片或缩写。 默认情况下，它将显示登录用户最常使用的联系人。

此组件使用多个 "控制[人员](./person.md)" 控件，但它可以绑定到一组人员描述符。 如果要显示的人员多于 `show-max` 该值，则将添加一个数字以指示其他联系人的数量。

## <a name="example"></a>示例

下面的示例展示了使用组件显示的一组人员 `mgt-people` 。 您可以使用代码编辑器来查看[属性](#properties)如何更改组件的行为。

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-people--people&source=docs" height="350"></iframe>

[在 "dev" 中打开此示例](https://mgt.dev/?path=/story/components-mgt-people--people&source=docs)

## <a name="properties"></a>属性

默认情况下， `mgt-people` 组件 `/me/people` 使用筛选器从终结点提取事件， `personType/class eq 'Person'` 以显示经常联系的用户。 您可以使用多个属性来更改此行为。

| 属性 | 属性 | 说明 |
| --- | --- | --- |
| show-max | showMax | 指示要显示的最大用户数。 默认值为3。 |
| people | people | 获取或设置组件呈现的人员列表的人员数组。 使用此属性可访问组件加载的人员。 设置此值可加载自己的人员。 |
| 组 id | groupId | 从各自的 ID 检索特定 Microsoft Graph 中的人员。 |
| 用户 id | userIds | 给定一个 Microsoft Graph 用户的数组 `ids` ，组件将呈现这些用户。  |
| 人员-查询 | peopleQueries | 如果给定一组人员查询（名称、upn、电子邮件），组件将呈现这些用户。 |
| 人员-卡片 | personCard | 一个枚举，用于确定激活浮出式面板-或的必需用户操作 `hover` `click` 。 默认值为 `none`。 |
| 展示-状态 | showPresence | 一个 boolean 类型的值，用于确定是否在人员图像上显示人员状态徽章。 |


下面的示例设置要显示的最大用户数。

```html
<mgt-people
  show-max="4">
</mgt-people>
```

## <a name="css-custom-properties"></a>CSS 自定义属性

`mgt-people`组件定义以下 CSS 自定义属性。

```css
mgt-people {
  --list-margin: 8px 4px 8px 8px; /* Margin for component */
  --avatar-margin: 0 4px 0 0; /* Margin for each person */
}
```

## <a name="templates"></a>模板

`mgt-people`支持多个[模板](../templates.md)，这些模板可用于替换组件的某些部分。 若要指定模板，请在 `<template>` 组件内添加一个元素，并将 `data-type` 值设置为下列值之一。

| 数据类型 | 数据上下文 | 说明 |
| --- | --- | --- |
| `default` | `people`： person 对象列表 | 默认模板会将整个组件替换为您自己的组件。 |
| `person` | `person`： person 对象 | 用于呈现每个人的模板。 |
| `overflow` | `people`： person 对象列表 <br> `max`：显示的人员的数量 <br> `extra`：额外人员数 | 用于将数字呈现在人员列表右侧的最大值之后的模板。 |
| `no-data` | 不传递数据上下文 | 没有可用数据时使用的模板。 |
| `loading` | 不传递数据上下文 | 组件加载状态时使用的模板。

下面的示例演示如何使用 `person` 模板。

```html
<mgt-people>
  <template>
    <ul><li data-for="person in people">
      <mgt-person person-query="{{ person.userPrincipalName }}"></mgt-person>
      <h3>{{ person.displayName }}</h3>
      <p>{{ person.jobTitle }}</p>
      <p>{{ person.department }}</p>
    </li></ul>
  </template>
</mgt-people>
```

## <a name="microsoft-graph-permissions"></a>Microsoft Graph 权限

此组件使用以下 Microsoft Graph Api 和权限：

| 资源 | 权限 |
| - | - |
| [/me/people](/graph/api/user-list-people?view=graph-rest-1.0) | `People.Read` |

使用默认模板时，需要其他 Api 和权限。 此组件的默认模板使用需要执行以下各项的 "[管理员](person.md)" 组件。

| 资源 | 权限 |
| - | - |
| [/users](/graph/api/user-list?view=graph-rest-1.0) | User.readbasic.all |
| [/me/calendarview](/graph/api/user-list-contacts?view=graph-rest-1.0) | Contacts.Read |

## <a name="authentication"></a>身份验证

该控件使用[身份验证文档](./../providers.md)中介绍的全局身份验证提供程序。

## <a name="extend-for-more-control"></a>扩展以实现更多控制

对于更复杂的方案或真正的自定义 UX，此组件将公开几种 `protected render*` 用于在组件扩展中进行重写的方法。

| 方法 | 说明 |
| - | - |
| renderLoading | 呈现加载状态。 |
| renderNoData | 呈现空数据状态。 |
| renderPeople | 呈现最大值的人员列表 `show-max` 。 |
| renderPerson | 呈现单个人员。 |
| renderOverflow | 呈现除值之外的剩余人员的表示形式 `show-max` 。 |
