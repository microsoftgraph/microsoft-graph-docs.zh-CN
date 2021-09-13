---
title: Microsoft 服务中的人员Graph Toolkit
description: 可以使用 Web 组件通过用户的照片或缩写显示一组 `mgt-people` 人员或联系人。
ms.localizationpriority: medium
author: nmetulev
ms.openlocfilehash: c93de8e60260d654624ae84896953dffe8f2e0b4
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59083815"
---
# <a name="people-component-in-the-microsoft-graph-toolkit"></a>Microsoft 服务中的人员Graph Toolkit

可以使用 Web 组件通过用户的照片或缩写显示一组 `mgt-people` 人员或联系人。 默认情况下，它将显示已登录用户的最常见的联系人。

此组件使用多个 [mgt-person](./person.md) 控件，但可以绑定到一组人员描述符。 如果要显示的人数多于该值，将添加一个号码以 `show-max` 指示其他联系人的数量。

## <a name="example"></a>示例

以下示例显示使用组件显示的一组 `mgt-people` 人员。 可以使用代码编辑器查看属性 [如何](#properties) 更改组件的行为。

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-people--people&source=docs" height="350"></iframe>

[在 mgt.dev 中打开此示例](https://mgt.dev/?path=/story/components-mgt-people--people&source=docs)

## <a name="properties"></a>属性

默认情况下，组件 `mgt-people` 通过筛选器从终结点 `/me/people` 提取事件 `personType/class eq 'Person'` 以显示经常联系的用户。 可以使用多个属性更改此行为。

| 属性 | 属性 | 说明 |
| --- | --- | --- |
| show-max | showMax | 指示要显示的最大人数。 默认值为 3。 |
| people | people | 用于获取或设置组件呈现的联系人列表的一组人员。 使用此属性访问组件加载的人。 设置此值以加载您自己的人员。 |
| group-id | groupId | 从特定 Microsoft Graph检索相应 ID 中的人员。 |
| user-ids | userIds | 给定一组 Microsoft `ids` Graph，组件将呈现这些用户。  |
| 人员查询 | peopleQueries | 给定一组人员查询 (、upns、电子邮件) ，组件将呈现这些用户。 |
| person-card | personCard | 一个枚举，用于确定激活飞出面板或 所需的用户 `hover` 操作 `click` 。 默认值为 `none`。 |
| show-presence | showPresence | 一个布尔值，用于确定是否在人像上显示个人状态锁屏提醒。 |
| resource | resource | 从 Microsoft 获取的资源Graph (例如 `/me/people` ，) 。 |
| scopes | scopes | 字符串的可选数组（如果使用 属性）或逗号分隔的范围（如果使用 属性）。 组件将使用这些作用域 (支持) ，以确保用户已同意适当的权限。 |
| version | version | 进行 GET 请求时使用的可选 API 版本。 默认值为 `v1.0`。  |

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
  --color: #000000 /* Text color *?
}
```

## <a name="templates"></a>模板

`mgt-people`支持[多个模板](../customize-components/templates.md)，您可以使用这些模板替换组件的某些部分。 若要指定模板，请包含组件 `<template>` 中的元素，将值 `data-type` 设置为以下值之一。

| 数据类型 | 数据上下文 | 说明 |
| --- | --- | --- |
| `default` | `people`：人员对象列表 | 默认模板将整个组件替换为你自己的组件。 |
| `person` | `person`：person 对象 | 用于呈现每个人模板。 |
| `overflow` | `people`：人员对象列表 <br> `max`：显示人数 <br> `extra`：额外人员的数量 | 用于呈现超过人员列表右侧最大值的号码的模板。 |
| `no-data` | 不传递任何数据上下文 | 没有可用数据时所使用的模板。 |
| `loading` | 不传递任何数据上下文 | 组件加载状态时所使用的模板。

以下示例演示如何使用 `person` 模板。

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
| `groupId` set | User.Read.All、People.Read | [/groups/ \$ {groupId}/members](/graph/api/group-list-members) |
| `userIds` set | User.ReadBasic.All | [/users/${userId}](/graph/api/user-get) |
| `peopleQueries` set | People.Read | [/me/people](/graph/api/user-list-people) |
| `resource` set | 中指定的权限 `scopes` | 在 中指定 `resource` |
| 默认配置 | People.Read | [/me/people](/graph/api/user-list-people) |
| `showPresence` set | Presence.Read.All | [/communications/getPresencesByUserId](/graph/api/cloudcommunications-getpresencesbyuserid) |

使用默认模板时，需要其他 API 和权限。 此组件的默认模板使用 [mgt-person](person.md) 组件。 有关所需权限的列表，请参阅其文档。

## <a name="authentication"></a>身份验证

该控件使用身份验证文档中所述的全局 [身份验证提供程序](../providers/providers.md)。

## <a name="cache"></a>缓存

|对象存储|缓存数据|备注|
|---------|-----------|-------|
|`people`|有关与查询匹配的人的信息|指定时 `resource` 使用|
|`users`|有关与查询匹配的用户的信息|在 `groupId` 、 `userIds` 或 `peopleQueries` 未指定任何属性时使用|
|`presence`|指定人员集状态|设置为 `showPresence` 时使用 `true`|

> [!NOTE]
> 默认情况下， `mgt-people` 组件使用该 [`mgt-person`](./person.md) 组件来显示有关人员的信息。 `mgt-person`组件自动下载并缓存每个人的照片。

请参阅[Caching，](../customize-components/cache.md)了解有关如何配置缓存的更多详细信息。
## <a name="extend-for-more-control"></a>扩展以了解更多控件

对于更复杂的方案或真正自定义的 UX，此组件公开了多个在组件扩展 `protected render*` 中替代的方法。

| 方法 | 说明 |
| - | - |
| renderLoading | 呈现加载状态。 |
| renderNoData | 呈现空数据状态。 |
| renderPeople | 呈现人员列表，最多呈现 `show-max` 值。 |
| renderPerson | 呈现单个人员。 |
| renderOverflow | 呈现值以外的剩余人的 `show-max` 表示形式。 |
