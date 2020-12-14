---
title: Microsoft Graph 功能中的人员Toolkit
description: 您可以使用 Web 组件通过用户的照片或缩写显示一 `mgt-people` 组人员或联系人。
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 9e19636c6f69784984d7438d53f57bac78fc6675
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49660056"
---
# <a name="people-component-in-the-microsoft-graph-toolkit"></a>Microsoft Graph 功能中的人员Toolkit

您可以使用 Web 组件通过用户的照片或缩写显示一 `mgt-people` 组人员或联系人。 默认情况下，它将显示已登录用户的最常见的联系人。

此组件使用多个 [人员](./person.md) 控制，但可以绑定到一组人员描述符。 如果显示人数多于该值，将添加一个数字以 `show-max` 指示其他联系人的数量。

## <a name="example"></a>示例

以下示例显示了使用组件显示的一组 `mgt-people` 人员。 可以使用代码编辑器查看属性 [如何](#properties) 更改组件的行为。

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-people--people&source=docs" height="350"></iframe>

[在 mgt.dev 中打开此示例](https://mgt.dev/?path=/story/components-mgt-people--people&source=docs)

## <a name="properties"></a>属性

默认情况下，组件通过筛选器从终结点提取事件 `mgt-people` `/me/people` `personType/class eq 'Person'` 以显示经常联系的用户。 可以使用多个属性更改此行为。

| 属性 | 属性 | 说明 |
| --- | --- | --- |
| show-max | showMax | 指示要显示的最大人数。 默认值为 3。 |
| people | people | 用于获取或设置组件呈现人员列表的一组人员。 使用此属性访问组件加载的人。 设置此值可加载您自己的人员。 |
| group-id | groupId | 从特定 Microsoft Graph 中检索相应 ID 中的人员。 |
| user-ids | userIds | 给定 Microsoft Graph 用户数组 `ids` 后，组件将呈现这些用户。  |
| people-queries | peopleQueries | 给定一组人员查询 (、upns、电子邮件) ，组件将呈现这些用户。 |
| person-card | personCard | 一个枚举，用于确定激活飞出面板所需的用户操作 - `hover` 或 `click` 。 默认值为 `none`。 |
| show-presence | showPresence | 一个布尔值，用于确定是否在人像上显示人员状态锁屏提醒。 |


以下示例设置要显示的最大人数。

```html
<mgt-people
  show-max="4">
</mgt-people>
```

## <a name="css-custom-properties"></a>CSS 自定义属性

该 `mgt-people` 组件定义以下 CSS 自定义属性。

```css
mgt-people {
  --list-margin: 8px 4px 8px 8px; /* Margin for component */
  --avatar-margin: 0 4px 0 0; /* Margin for each person */
  --color: #000000 /* Text color *?
}
```

## <a name="templates"></a>模板

支持 `mgt-people` [多个模板](../customize-components/templates.md) ，您可以使用这些模板替换组件的某些部分。 若要指定模板，请包含 `<template>` 组件中的元素，将值设置为下列 `data-type` 值之一。

| 数据类型 | 数据上下文 | 说明 |
| --- | --- | --- |
| `default` | `people`：人员对象列表 | 默认模板将整个组件替换为你自己的组件。 |
| `person` | `person`： person 对象 | 用于呈现每个人模板。 |
| `overflow` | `people`：人员对象列表 <br> `max`： 显示人员的数量 <br> `extra`：额外人员的数量 | 用于呈现超过人员列表右侧最大值的号码的模板。 |
| `no-data` | 不传递任何数据上下文 | 没有可用数据时使用的模板。 |
| `loading` | 不传递任何数据上下文 | 组件加载状态时所使用的模板。

以下示例显示如何使用 `person` 模板。

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

此组件使用以下 Microsoft Graph API 和权限：

| 资源 | 权限 |
| - | - |
| [/me/people](/graph/api/user-list-people) | `People.Read` |

使用默认模板时，需要其他 API 和权限。 此组件的默认模板使用 [mgt-person](person.md) 组件，这需要以下内容。

| 资源 | 权限 |
| - | - |
| [/users](/graph/api/user-list) | User.ReadBasic.All |

## <a name="authentication"></a>身份验证

该控件使用身份验证文档中介绍的全局 [身份验证提供程序](../providers/providers.md)。

## <a name="extend-for-more-control"></a>扩展以更多控制

对于更复杂的方案或真正自定义的 UX，此组件公开了多个在组件扩展中 `protected render*` 替代的方法。

| 方法 | 说明 |
| - | - |
| renderLoading | 呈现加载状态。 |
| renderNoData | 呈现空数据状态。 |
| renderPeople | 呈现人员列表，最多呈现 `show-max` 值。 |
| renderPerson | 呈现单个人员。 |
| renderOverflow | 呈现剩余人员超出该值 `show-max` 的表示形式。 |
