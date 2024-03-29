---
title: Microsoft 计划中的议程Graph Toolkit
description: mgt-agenda Web 组件用于表示用户或组日历中的事件。
ms.localizationpriority: medium
author: sebastienlevert
ms.openlocfilehash: 6787f7d5ce8804b4f24306b0b17ad47024d227b5
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589047"
---
# <a name="agenda-component-in-the-microsoft-graph-toolkit"></a>Microsoft 计划中的议程Graph Toolkit

Web `mgt-agenda` 组件表示用户或组日历中的事件。 默认情况下，日历显示当前日期的当前已登录用户事件。 该组件还可使用从 Microsoft Graph 返回事件的任何终结点。

## <a name="example"></a>示例

以下示例显示使用 组件显示的已登录用户的日历 `mgt-agenda` 事件。 可以使用代码编辑器查看属性 [如何](#properties) 更改组件的行为。

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-agenda--simple&source=docs" height="500"></iframe>

[在 mgt.dev 中打开此示例](https://mgt.dev/?path=/story/components-mgt-agenda--simple&source=docs)

## <a name="properties"></a>属性

默认情况下，组件 `mgt-agenda` 从终结点提取 `/me/calendarview` 事件并显示当天的事件。 有几种属性可用于更改此行为。

| 属性 | 属性 | 说明 |
| --- | --- | --- |
| date | date | 一个字符串，表示从 Microsoft Graph 提取的事件的开始日期。 值应采用 Date 构造函数可以分析[的格式 - 如果](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date)`event-query`设置了属性，则值无效。 |
| days | days | 从 Microsoft Graph获取的天数 - 默认值为 3 - `event-query` 如果设置了属性，则值无效。 |
| show-max | showMax | 一个数字，指示要显示的最大事件数。 默认值未设置为没有 (最大值) 。 |
| group-id | groupId | 使用组日历的字符串 ID，而不是当前登录用户的日历。 |
| event-query | eventQuery | 一个字符串，表示在从 Microsoft 网站提取事件时所使用的Graph。 （可选）在 `|` `/groups/GROUP-ID-GUID/calendar/calendarView | group.read.all` 字符串末尾添加委派作用域，用 () 。 |
| events | events | 用于获取或设置组件呈现的事件列表的事件数组 - 使用此属性访问组件加载的事件。 设置此值以加载你自己的事件 - 如果值由开发人员设置， `date`则 、 `days`或 `event-query` 属性不起作用。 |
| 按天分组 | groupByDay | 按天对事件进行分组的布尔值 - 默认情况下不对事件进行分组。 |
| preferred-timezone | preferredTimezone | 从 Microsoft 网站检索事件时使用的首选时区Graph例如， `Pacific Standard Time`。 默认情况下，此属性使用 UTC 时区。 通过调用 终结点 `me/mailboxSettings` 并读取 timeZone 属性的值，可以检索当前 **用户的首选** 时区。 |

以下示例将组件的行为更改为获取特定日期的数据，最多三天。

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
| reload ()  | 调用 方法，根据组件的属性使用潜在的新数据重新加载组件。 |

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

若要了解更多信息，请参阅 [设置组件样式](../customize-components/style.md)。

## <a name="templates"></a>模板

组件 `mgt-agenda` 支持 [多个模板](../customize-components/templates.md) ，允许您替换组件的某些部分。 若要指定模板，请包含 `<template>` 组件内的元素，将 `data-type` 值设置为下列值之一：

| 数据类型 | 数据上下文 | 说明 |
| --- | --- | --- |
| `default` | `events`：event 对象列表 | 默认模板将整个组件替换为你自己的组件。 |
| `event` | `event`： event 对象 | 用于呈现每个事件的模板。 |
| `event-other` | `event`： event 对象 | 用于呈现每个事件的其他内容的模板。 |
| `header` | `header`： string | 用于呈现每天的标题的模板。 |
| `loading` | 不传递任何数据上下文 | 加载数据时所使用的模板。 |
| `no-data` | 不传递任何数据上下文 | 没有可用事件时所使用的模板。 |

以下示例演示如何使用 `event` 模板：

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

## <a name="events"></a>事件

从控件中触发以下事件。

事件 | 何时发出 | 自定义数据 | Cancelable | 气泡 | 使用自定义模板
------|-------------------|--------------|:-----------:|:---------:|:---------------------------:|
`eventClick` | 用户单击或点击事件。 | 选定 [事件](/graph/api/resources/event) | 否 | 否 | 是，使用自定义 **事件** 模板

有关处理事件的信息，请参阅 [事件](../customize-components/events.md)。

## <a name="microsoft-graph-permissions"></a>Microsoft Graph 权限

此组件使用下列 Microsoft Graph API 和权限：

| 配置 | 权限 | API
| - | - | - |
| default | Calendars.Read | [/me/calendarview](/graph/api/calendar-list-calendarview) |

该组件允许你指定其他 Microsoft Graph查询来调用 (，如) `/groups/{id}/calendar/calendarView` 。 在这种情况下，将权限追加到字符串的末尾，以 分隔。`|`

使用默认模板和默认模板时 `renderAttendees` ，需要其他 API 和权限。 此组件的默认模板对具有与会者的事件使用 [mgt-people](people.md) 组件，并继承所有权限。

## <a name="authentication"></a>身份验证

登录控件使用身份验证文档中介绍的全局 [身份验证提供程序](../providers/providers.md)。

## <a name="cache"></a>缓存

组件 `mgt-agenda` 不缓存任何数据。

## <a name="extend-for-more-control"></a>扩展以了解更多控件

对于更复杂的方案或真正自定义的 UX `protected` ，此组件公开多个 render* 方法以在组件扩展中替代。

| 方法 | 说明 |
| - | - |
| renderLoading | 在组件加载时呈现加载状态。 |
| renderNoData | 呈现空数据状态。 |
| renderGroups | 将事件数据按组排序，然后使用组标头呈现它们。 |
| renderHeader | 呈现组标头。 |
| renderEvents | 呈现 event 对象的列表。 |
| renderEvent | 呈现单数事件及其所有部分。
| renderTitle | 呈现事件标题部件。 |
| renderLocation | 呈现事件位置部分。 |
| renderAttendees | 呈现事件参与者部分。 |
| renderOther | 呈现其他事件内容。 |
