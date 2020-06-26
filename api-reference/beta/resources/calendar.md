---
title: 日历资源类型
description: 日历即事件容器。 它可以是用户的日历，也可以是 Microsoft 365 组的默认日历。
localization_priority: Priority
author: harini84
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 6eabbb23ddcab85baf4277f25c586b4affd2c6bc
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897818"
---
# <a name="calendar-resource-type"></a>日历资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

日历即事件容器。 它可以是[用户](user.md)的日历，也可以是 Microsoft 365[组](group.md)的默认日历。

> **注意：** 与用户日历和组日历交互的方式稍有不同：

- 只能将用户日历组织到 [calendarGroup](calendargroup.md) 中。
- Outlook 将代表组自动接受所有会议请求。 只能[接受](../api/event-accept.md)、[暂时接受](../api/event-tentativelyaccept.md)或[拒绝](../api/event-decline.md)用户日历中的会议请求。
- Outlook 不支持对组事件提供提醒。 只能[推迟](../api/event-snoozereminder.md)或[取消](../api/event-dismissreminder.md)用户日历的[提醒](reminder.md)。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[列出日历](../api/user-list-calendars.md)|[日历](calendar.md) 集合|获取所有用户的日历，或者获取默认或其他特定日历组中的日历。|
|[创建日历](../api/user-post-calendars.md) |[calendar](calendar.md)| 在默认日历组或用户的指定日历组中新建日历。|
|[Get calendar](../api/calendar-get.md) | [calendar](calendar.md) |获取 **calendar** 对象的属性和关系。 日历可以是用户的一个，也可以是 Microsoft 365 组的默认日历。 |
|[Update](../api/calendar-update.md) | [calendar](calendar.md)  |更新 **calendar** 对象的属性。 日历可以是用户的一个，也可以是 Microsoft 365 组的默认日历。 |
|[Delete](../api/calendar-delete.md) | 无 |删除 calendar 对象。 |
|[列出 calendarView](../api/calendar-list-calendarview.md) |[事件](event.md) 集合| 从用户的主日历 `(../me/calendarview)` 或指定日历中，获取由时间范围定义的日历视图中的事件发生次数、异常和单个实例。|
|[列出事件](../api/calendar-list-events.md) |[事件](event.md) 集合| Retrieve a list of events in a calendar.  The list contains single instance meetings and series masters.|
|[创建事件](../api/calendar-post-events.md) |[event](event.md)| 在默认或指定日历中创建新事件。|
|[getSchedule](../api/calendar-getschedule.md) |[scheduleInformation](scheduleinformation.md) 集合|获取用户、通讯组列表或资源在指定时间段内的忙/闲状态信息。 |
|[findMeetingTimes](../api/user-findmeetingtimes.md) |[meetingTimeSuggestionsResult](meetingtimesuggestionsresult.md) |根据组织者和与会者忙/闲状态以及时间或地点约束，建议会议时间和地点。 |
|[创建单值扩展属性](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[日历](calendar.md)  |在新建或现有日历中创建一个或多个单值扩展属性。   |
|[获取包含单值扩展属性的日历](../api/singlevaluelegacyextendedproperty-get.md)  | [日历](calendar.md) | 通过使用 `$expand` 或 `$filter` 获取包含一个单值扩展属性的日历。 |
|[创建多值扩展属性](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [日历](calendar.md) | 在新建或现有的日历中创建一个或多个多值扩展属性。  |
|[获取包含多值扩展属性的日历](../api/multivaluelegacyextendedproperty-get.md)  | [日历](calendar.md) | 使用 `$expand` 获取包含一个多值扩展属性的日历。 |

## <a name="properties"></a>属性
| 属性     | 类型   |Description|
|:---------------|:--------|:----------|
|allowedOnlineMeetingProviders|string 集合| 表示此日历中可用于创建联机会议的联机会议服务提供商。 可取值为：`unknown`、`skypeForBusiness`、`skypeForConsumer`、`teamsForBusiness`。|
|calendarGroupId|字符串|要在其中创建日历的 [calendarGroup](calendargroup.md)。 若用户从未显式设置日历的组，此属性为空。|
|canEdit |布尔 |True if the user can write to the calendar, false otherwise. This property is true for the user who created the calendar. This property is also true for a user who has been shared a calendar and granted write access, through an Outlook client or the corresponding [calendarPermission](calendarpermission.md) resource. Read-only.|
|canShare |Boolean |如果用户有权共享日历则为 ture，否则为 false。 只有创建日历的用户才可以进行共享。 只读。|
|canViewPrivateItems |Boolean |如果用户可以读取已标记为私有的日历项，则为 true，否则返回 false。 此属性通过 Outlook 客户端或相应的 [calendarPermission](calendarpermission.md) 资源进行设定。 只读。|
|changeKey|String|Identifies the version of the calendar object. Every time the calendar is changed, changeKey changes as well. This allows Exchange to apply changes to the correct version of the object. Read-only.|
|color|String|Specifies the color theme to distinguish the calendar from other calendars in a UI. The property values are: LightBlue=0, LightGreen=1, LightOrange=2, LightGray=3, LightYellow=4, LightTeal=5, LightPink=6, LightBrown=7, LightRed=8, MaxColor=9, Auto=-1|
|defaultOnlineMeetingProvider|onlineMeetingProviderType|从此日历发送的会议的默认联机会议提供商。 可取值为：`unknown`、`skypeForBusiness`、`skypeForConsumer`、`teamsForBusiness`。|
|hexColor|String|日历颜色，使用十六进制颜色代码表示，其中包含三个十六进制值，每个值介于 00 到 FF 之间，表示 RGB 颜色空间中颜色的红色、绿色或蓝色组件。 若用户从未显式设置日历的颜色，此属性为空。 |
|id|String|The calendar's unique identifier. Read-only.|
|isDefaultCalendar|Boolean|若此为默认用于新建事件的默认日志则为 True，反之为 false。|
|isRemovable|Boolean| 表示是否可以从用户邮箱删除此用户日志。|
|isShared |Boolean |如果用户已与其他用户共享日历，则值为 true，否则为 false。 由于只有创建日历的用户才能共享日历，因此同一用户的 **isShared** 和 **isSharedWithMe** 不能为 true。 共享在 Outlook 客户端中发起时，此属性设定，当共享通过客户端或相应的 [calendarPermission](calendarpermission.md) 资源取消时，可重置属性。 只读。|
|isSharedWithMe |Boolean |如果用户已共享此日历，则值为 true，否则为 false。 对于日历所有者，此属性始终为 false。 共享在 Outlook 客户端中发起时，此属性设定，当共享通过客户端或相应的 [calendarPermission](calendarpermission.md) 资源取消时，可重置属性。 只读。 |
|isTallyingResponses|Boolean|表示此用户日历是否支持会议响应跟踪。 仅从用户的主日志发送的会议邀请支持会议响应跟踪。|
|name|String|日历名称。|
|owner |[emailAddress](emailaddress.md) | 如果设置，则表示创建或添加日历的用户。 对于用户创建或添加的日历，将 **owner** 属性设置为用户。 对于与用户共享的日历，将 **owner** 属性设置为与此用户共享该日历的人员。 只读。|

## <a name="relationships"></a>关系
| 关系 | 类型   |Description|
|:---------------|:--------|:----------|
|calendarPermissions|[calendarPermission](calendarpermission.md) 集合| 共享日历的用户的权限。|
|calendarView|[event](event.md) 集合|The calendar view for the calendar. Navigation property. Read-only.|
|events|[event](event.md) 集合|The events in the calendar. Navigation property. Read-only.|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) 集合| The collection of multi-value extended properties defined for the calendar. Read-only. Nullable.|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection| The collection of single-value extended properties defined for the calendar. Read-only. Nullable.|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "calendarView",
    "events",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.calendar"
}-->

```json
{
  "allowedOnlineMeetingProviders": ["string"],
  "canEdit": "boolean",
  "canShare": "boolean",
  "canViewPrivateItems": "boolean",
  "changeKey": "string",
  "color": "String",
  "defaultOnlineMeetingProvider": "string",
  "hexColor": "String",
  "id": "string (identifier)",
  "isDefaultCalendar": "boolean",
  "isRemovable": "boolean",
  "isShared": "boolean",
  "isSharedWithMe": "boolean",
  "isTallyingResponses": "boolean",
  "name": "string",
  "owner": {"@odata.type": "microsoft.graph.emailAddress"}
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "calendar resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
