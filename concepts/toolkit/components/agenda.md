---
title: Microsoft Graph 工具包中的 "议程" 组件
description: "\"管理中心议程\" web 组件用于表示用户或组日历中的事件。"
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 0afe3546541e38349404b80abac48073b90f7eb4
ms.sourcegitcommit: d9e94c109c0934cc93f340aafa1dccaa1a5da9c7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37275731"
---
# <a name="agenda-component-in-the-microsoft-graph-toolkit"></a>Microsoft Graph 工具包中的 "议程" 组件

`mgt-agenda` Web 组件表示用户或组日历中的事件。 默认情况下，日历会在当前日期的用户事件中显示当前登录的用户事件。 组件还可以使用从 Microsoft Graph 返回事件的任何终结点。 

## <a name="example"></a>示例

[jsfiddle 示例](https://jsfiddle.net/metulev/ojt2c7vp/)

```html
<mgt-agenda group-by-day></mgt-agenda>
```

![计划-议程](./images/mgt-agenda.png)

## <a name="properties"></a>属性

默认情况下， `mgt-agenda`组件从`/me/calendarview`终结点提取事件并显示当天的事件。 有几个可用于更改此行为的属性。

| 属性 | 属性 | 说明 |
| --- | --- | --- |
| date | date | 一个字符串，表示要从 Microsoft Graph 中提取的事件的开始日期。 值应采用可由[日期构造函数](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date)进行分析的格式，如果`event-query`设置了属性，则值不起作用。 |
| 之前 | 之前 | 从 Microsoft Graph 提取的天数-默认值为3。如果`event-query`设置了属性，则此值不起作用。 |
| showMax | show-max | 一个数字，用于指示要显示的最大事件数。 未设置默认值（无最大值）。 |
| groupId | 组 id | 要使用的组日历的字符串 ID，而不是当前登录的用户日历。 |
| eventQuery | 事件查询 | 一个字符串，表示从 Microsoft Graph 提取事件时要使用的替代查询。 （可选）通过将委派作用域与`|` （`/groups/GROUP-ID-GUID/calendar/calendarView | group.read.all`）分隔来将其添加到字符串的末尾。 |
| 活动 | 活动 | 一个事件数组，用于获取或设置组件呈现的事件的列表-使用此属性可访问组件加载的事件。 将此值设置为加载您自己的事件-如果值是由开发人员`date`设置`days`的， `event-query`则、或属性不起作用。 |
| groupByDay | 逐天分组 | 按天对事件分组的布尔值不按默认事件进行分组。 |

下面的示例更改组件的行为，以获取特定日期的数据，最长为三天。

```html
<mgt-agenda
  group-by-day
  date="May 7, 2019"
  days="3"
  ></mgt-agenda>
```

下面的示例将更改组件的行为，以从特定查询中获取数据。

```html
<mgt-agenda
  event-query="/me/events?orderby=start/dateTime"
  ></mgt-agenda>
```

## <a name="css-custom-properties"></a>CSS 自定义属性

`mgt-agenda`组件定义这些 CSS 自定义属性

```css
mgt-agenda {
  --event-box-shadow: 0px 2px 8px rgba(0, 0, 0, 0.092);
  --event-margin: 0px 10px 14px 10px;
  --event-padding: 8px 0px;
  --event-background: #ffffff;
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

若要了解详细信息，请参阅[样式组件](../style.md)。

## <a name="templates"></a>模板

组件支持多个[模板](../templates.md)，这些模板允许您替换组件的某些部分。 `mgt-agenda` 若要指定模板，请在`<template>`组件内添加一个元素，并将`data-type`值设置为下列值之一：

| 数据类型 | 数据上下文 | 说明 |
| --- | --- | --- |
| `default` | `events`：事件对象的列表 | 默认模板会将整个组件替换为您自己的组件。 |
| `event` | `event`： event 对象 | 用于呈现每个事件的模板。 |
| `header` | `header`： string | 用于呈现每天的标题的模板。 |
| `other` | `event`： event 对象 | 用于呈现每个事件的其他内容的模板。 |
| `no-data` | 不传递数据上下文 | 没有可用事件时使用的模板。 |
| `loading` | 不传递数据上下文 | 加载数据时使用的模板。 |

下面的示例演示如何使用`event`模板：

```html
<mgt-agenda>
  <template data-type="event">
    <button class="eventButton">
      <div class="event-subject">{{ event.subject }}</div>
      <div data-for="attendee in event.attendees">
        <mgt-person
          person-query="{{ attendee.emailAddress.name }}"
          show-name
          show-email>
        </mgt-person>
      </div>
    </button>
  </template>
  <template data-type="no-data">
    There are no events found!
  </template>
</mgt-agenda>
```

若要了解详细信息，请参阅[模板](../templates.md)。

## <a name="graph-scopes"></a>图表范围

此组件使用以下 Microsoft Graph Api 和权限：

| resource | 权限/范围 |
| - | - |
| [/me/calendarview](https://docs.microsoft.com/en-us/graph/api/calendar-list-calendarview?view=graph-rest-1.0) | `Calendars.Read` |

组件允许您指定要调用的其他 Microsoft Graph 查询（例如`/groups/{id}/calendar/calendarView`）。 在这种情况下，将作用域追加到字符串的末尾，并将其分隔`|`

## <a name="authentication"></a>身份验证

登录控件利用[身份验证文档](./../providers.md)中所述的全局验证提供程序。 

