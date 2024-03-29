---
title: Microsoft 服务中的人员Graph Toolkit
description: 可以使用 Web `mgt-people` 组件通过用户的照片或缩写显示一组人员或联系人。
ms.localizationpriority: medium
author: sebastienlevert
ms.openlocfilehash: 43bc1016a462a1463437f3090361dfdd997c860c
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2022
ms.locfileid: "64587103"
---
# <a name="people-component-in-the-microsoft-graph-toolkit"></a>Microsoft 服务中的人员Graph Toolkit

可以使用 Web `mgt-people` 组件通过用户的照片或缩写显示一组人员或联系人。 默认情况下，它将显示已登录用户的最常见的联系人。

此组件使用多个 [mgt-person](./person.md) 控件，但可以绑定到一组人员描述符。 如果要显示的人数多于 `show-max` 该值，将添加一个号码以指示其他联系人的数量。

## <a name="example"></a>示例

以下示例显示使用组件显示的一组 `mgt-people` 人员。 可以使用代码编辑器查看属性 [如何](#properties) 更改组件的行为。

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-people--people&source=docs" height="350"></iframe>

[在 mgt.dev 中打开此示例](https://mgt.dev/?path=/story/components-mgt-people--people&source=docs)

## <a name="properties"></a>属性

默认情况下，组件 `mgt-people` 通过筛选器 `/me/people` 从终结点提取 `personType/class eq 'Person'` 事件以显示经常联系的用户。 可以使用多个属性更改此行为。

| 属性 | 属性 | 说明 |
| --- | --- | --- |
| show-max | showMax | 指示要显示的最大人数。 默认值为 3。 |
| people | people | 用于获取或设置组件呈现的联系人列表的一组人员。 使用此属性访问组件加载的人。 设置此值以加载您自己的人员。 |
| group-id | groupId | 从特定 Microsoft Graph检索相应 ID 中的用户。 |
| user-ids | userIds | 给定一组 Microsoft Graph`ids`，组件将呈现这些用户。  |
| 人员查询 | peopleQueries | 给定一组人员查询 (、upns、电子邮件) ，组件将呈现这些用户。 |
| person-card | personCard | 一个枚举，用于确定激活飞出面板所需的用户操作 - `hover`、 `click`或 `none`。 默认值为 `hover`。 |
| show-presence | showPresence | 一个布尔值，用于确定是否在人像上显示个人状态锁屏提醒。 |
| resource | resource | 从 Microsoft 获取的资源Graph (例如， `/me/people`) 。 |
| scopes | scopes | 字符串的可选数组（如果使用 属性）或逗号分隔的范围（如果使用 属性）。 组件将使用这些作用域 (支持) ，以确保用户已同意适当的权限。 |
| version | version | 进行 GET 请求时使用的可选 API 版本。 默认值为“`v1.0`”。  |
| fallback-details| fallbackDetails| 在图中找不到用户/人员/联系人时，表示一个用户或多人的 IDynamicPerson 对象数组。

以下示例设置要显示的最大人数。

```html
<mgt-people
  show-max="4">
</mgt-people>
```

## <a name="css-custom-properties"></a>CSS 自定义属性

组件 `mgt-people` 定义以下 CSS 自定义属性。

```css
mgt-people {
  --list-margin: 8px 4px 8px 8px; /* Margin for component */
  --avatar-margin: 0 4px 0 0; /* Margin for each person */
  --color: #000000 /* Text color */
}
```

## <a name="templates"></a>模板

支持`mgt-people`[多个模板](../customize-components/templates.md)，您可以使用这些模板替换组件的某些部分。 若要指定模板，请包含 `<template>` 组件中的元素，将 `data-type` 值设置为以下值之一。

| 数据类型 | 数据上下文 | 说明 |
| --- | --- | --- |
| `default` | `people`：人员对象列表 | 默认模板将整个组件替换为你自己的组件。 |
| `person` | `person`：person 对象 | 用于呈现每个人模板。 |
| `overflow` | `people`：人员对象列表 <br> `max`：显示人数 <br> `extra`：额外人员的数量 | 用于呈现超过人员列表右侧最大值的号码的模板。 |
| `no-data` | 不传递任何数据上下文 | 没有可用数据时所使用的模板。 |
| `loading` | 不传递任何数据上下文 | 组件加载状态时所使用的模板。

以下示例演示如何使用模板 `person` 。

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

此组件使用下列 Microsoft Graph API 和权限：

| 配置 | 权限 | API
| --- | ---------- | ------- |
| `groupId` set | GroupMember.Read.All | [/groups/\${groupId}/members](/graph/api/group-list-members) |
| `userIds` set | User.ReadBasic.All | [/users/${userId}](/graph/api/user-get) |
| `peopleQueries` set | People.Read | [/me/people](/graph/api/user-list-people) |
| `resource` set | 中指定的权限 `scopes` | 在 中指定 `resource` |
| 默认配置 | People.Read | [/me/people](/graph/api/user-list-people) |
| `showPresence` set | Presence.Read.All | [/communications/getPresencesByUserId](/graph/api/cloudcommunications-getpresencesbyuserid) |

使用默认模板时，需要其他 API 和权限。 此组件的默认模板使用 [mgt-person](person.md) 组件。 有关所需权限的列表，请参阅其文档。

## <a name="authentication"></a>身份验证

该控件使用身份验证文档中介绍的全局 [身份验证提供程序](../providers/providers.md)。

## <a name="cache"></a>缓存

|对象存储|缓存数据|备注|
|---------|-----------|-------|
|`people`|有关与查询匹配的人的信息|指定时 `resource` 使用|
|`users`|有关与查询匹配的用户的信息|在 、 `groupId``userIds`或未指定`peopleQueries`任何属性时使用|
|`presence`|指定人员集状态|设置为 时 `showPresence` 使用 `true`|

> [!NOTE]
> 默认情况下，组件 `mgt-people` 使用该 [`mgt-person`](./person.md) 组件来显示有关人员的信息。 组件 `mgt-person` 自动下载并缓存每个人的照片。

若要详细了解如何配置缓存[，请参阅Caching](../customize-components/cache.md)。
## <a name="extend-for-more-control"></a>扩展以了解更多控件

对于更复杂的方案或真正自定义的 UX `protected render*` ，此组件公开了多个在组件扩展中替代的方法。

| 方法 | 说明 |
| - | - |
| renderLoading | 呈现加载状态。 |
| renderNoData | 呈现空数据状态。 |
| renderPeople | 呈现人员列表，最多呈现值 `show-max` 。 |
| renderPerson | 呈现单个人员。 |
| renderOverflow | 呈现值以外的剩余人的表示 `show-max` 形式。 |
