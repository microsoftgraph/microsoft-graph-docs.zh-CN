---
title: Agenda component in the Microsoft Graph Toolkit
description: mgt-agenda Web 组件用于表示用户或组日历中的事件。
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: e66ffed1f10de5c4c9b9b322d9070074ec707000
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49659546"
---
# <a name="agenda-component-in-the-microsoft-graph-toolkit"></a>Agenda component in the Microsoft Graph Toolkit

Web `mgt-agenda` 组件表示用户或组日历中的事件。 默认情况下，日历显示当前日期的当前登录用户事件。 该组件还可使用从 Microsoft Graph 返回事件的任何终结点。

## <a name="example"></a>示例

以下示例显示使用组件显示的登录用户的日历 `mgt-agenda` 事件。 可以使用代码编辑器查看属性 [如何](#properties) 更改组件的行为。

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-agenda--simple&source=docs" height="500"></iframe>

[在 mgt.dev 中打开此示例](https://mgt.dev/?path=/story/components-mgt-agenda--simple&source=docs)

## <a name="properties"></a>属性

默认情况下， `mgt-agenda` 组件从终结点提取事件 `/me/calendarview` 并显示当天的事件。 有几个属性可用于更改此行为。

| 属性 | 属性 | 说明 |
| --- | --- | --- |
| date | date | 一个字符串，表示从 Microsoft Graph 提取的事件的开始日期。 值应采用 Date 构造函数可以分析的格式 [-](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date) 如果设置了属性，则值 `event-query` 无效。 |
| days | days | 从 Microsoft Graph 获取的天数 -默认值为 3 - 如果设置了属性，则值 `event-query` 无效。 |
| show-max | showMax | 一个数字，指示要显示的最大事件数。 默认值未设置为最大 (值) 。 |
| group-id | groupId | 组日历的字符串 ID，而不是当前登录用户的日历。 |
| event-query | eventQuery | 一个字符串，表示从 Microsoft Graph 提取事件时所使用的备用查询。 （可选）在字符串末尾添加委派作用域，用 `|` `/groups/GROUP-ID-GUID/calendar/calendarView | group.read.all` () 。 |
| events | events | 用于获取或设置组件呈现的事件列表的事件数组 - 使用此属性访问组件加载的事件。 将此值设置为加载你自己的事件 - 如果值由开发人员设置，则 `date` ， 或 `days` `event-query` 属性不起作用。 |
| 按天分组 | groupByDay | 按天对事件进行分组的布尔值 - 默认情况下不对事件进行分组。 |
| preferred-timezone | preferredTimezone | 从 Microsoft Graph 检索事件时要使用的首选时区的名称;例如 `Pacific Standard Time` ，。 默认情况下，此属性使用 UTC 时区。 可以通过调用终结点并读取 timeZone 属性的值来检索当前 `me/mailboxSettings` **用户** 的首选时区。 |

以下示例将组件的行为更改为获取特定日期和最多三天的数据。

```html
<mgt-agenda
  group-by-day
  date="May 7, 2019"
  days="3"
  ></mgt-agenda>
```

以下示例将组件的行为更改为从特定查询提取数据。

```html
<mgt-agenda
  event-query="/me/events?orderby=start/dateTime"
  ></mgt-agenda>
```

## <a name="methods"></a>方法
| 方法 | 说明 |
| --- | --- |
| 重新加载 ()  | 调用该方法以根据组件的属性重新加载具有潜在新数据的组件。 |

## <a name="css-custom-properties"></a>CSS 自定义属性

组件 `mgt-agenda` 定义这些 CSS 自定义属性

```css
mgt-agenda {
  --event-box-shadow: 0px 2px 8px rgba(0, 0, 0, 0.092);
  --event-margin: 0px 10px 14px 10px;
  --event-padding: 8px 0px;
  --event-background-color: #ffffff;
  --event-border: solid 2px rgba(0, 0, 0, 0);

  --agenda-header-margin: 40px 10px 14px 10px;
  --agenda-header-font-size: 24px;
  --agenda-header-color: #333333;

  --event-time-font-size: 12px;
  --event-time-color: #000000;

  --event-subject-font-size: 19px;
  --event-subject-color: #333333;

  --event-location-font-size: 12px;
  --event-location-color: #000000;
}
```

若要了解更多信息，请参阅 [样式组件](../customize-components/style.md)。

## <a name="templates"></a>模板

该 `mgt-agenda` 组件支持 [多个模板](../customize-components/templates.md) ，允许您替换组件的某些部分。 若要指定模板，请包含组件中的元素，将值设置为下列值 `<template>` `data-type` 之一：

| 数据类型 | 数据上下文 | 说明 |
| --- | --- | --- |
| `default` | `events`：事件对象列表 | 默认模板将整个组件替换为你自己的组件。 |
| `event` | `event`： event 对象 | 用于呈现每个事件的模板。 |
| `event-other` | `event`： event 对象 | 用于呈现每个事件的其他内容的模板。 |
| `header` | `header`： string | 用于呈现每天的标题的模板。 |
| `loading` | 不传递任何数据上下文 | 加载数据时所使用的模板。 |
| `no-data` | 不传递任何数据上下文 | 没有可用事件时使用的模板。 |

以下示例演示了如何使用 `event` 模板：

```html
<mgt-agenda>
  <template data-type="event">
    <button class="eventButton">
      <div class="event-subject">{{ event.subject }}</div>
      <div data-for="attendee in event.attendees">
        <mgt-person
          person-query="{{ attendee.emailAddress.name }}"
          view="twolines">
        </mgt-person>
      </div>
    </button>
  </template>
  <template data-type="no-data">
    There are no events found!
  </template>
</mgt-agenda>
```

若要了解更多信息，请参阅 [模板](../customize-components/templates.md)。

## <a name="events"></a>活动

从控件中触发以下事件。

| 事件 | 说明 |
| --- | --- |
| eventClick | 用户单击或点击事件。|

## <a name="permissions"></a>权限

此组件使用以下 Microsoft Graph API 和权限：

| 资源 | 权限 |
| - | - |
| [/me/calendarview](/graph/api/calendar-list-calendarview) | Calendars.Read |

该组件允许你指定其他 Microsoft Graph 查询来调用 (， `/groups/{id}/calendar/calendarView` 如) 。 在这种情况下，将权限附加到字符串的末尾，以分隔符 `|` 。

使用默认模板和默认 `renderAttendees` 模板时，需要其他 API 和权限。 此组件的默认模板对具有与会者的事件使用 [mgt-people](people.md) 组件，这需要以下内容。

| 资源 | 权限 |
| - | - |
| [/users](/graph/api/user-list) | Users.ReadBasic.All |
| [/me/calendarview](/graph/api/user-list-people) | People.Read |
| [/me/calendarview](/graph/api/user-list-contacts) | Contacts.Read |

## <a name="authentication"></a>身份验证

登录控件使用身份验证文档中介绍的全局 [身份验证提供程序](../providers/providers.md)。

## <a name="extend-for-more-control"></a>扩展以更多控制

对于更复杂的方案或真正自定义的 UX，此组件公开多个 render* 方法以在组件扩展 `protected` 中替代。

| 方法 | 说明 |
| - | - |
| renderLoading | 在组件加载时呈现加载状态。 |
| renderNoData | 呈现空数据状态。 |
| renderGroups | 将事件数据分类到组中，然后使用组标头呈现它们。 |
| renderHeader | 呈现组标头。 |
| renderEvents | 呈现事件对象的列表。 |
| renderEvent | 呈现单数事件及其所有部分。
| renderTitle | 呈现事件标题部件。 |
| renderLocation | 呈现事件位置部分。 |
| renderAttendees | 呈现事件参与者部分。 |
| renderOther | 呈现其他事件内容。 |
