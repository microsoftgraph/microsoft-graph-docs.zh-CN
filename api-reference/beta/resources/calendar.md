---
title: 日历资源类型
description: 日历即事件容器。 可以是用户的日历，也可以是 Office 365 组的默认日历。
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 4901b7a9a0c4d633f9d8bc9a6826fd71beccf770
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33338770"
---
# <a name="calendar-resource-type"></a>日历资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

日历即事件容器。 可以是[用户](user.md)的日历，也可以是 Office 365 [组](group.md)的默认日历。

> **注意：** 与用户日历和组日历交互的方式稍有不同：

 - 只能将用户日历组织到 [calendarGroup](calendargroup.md) 中。
 - Outlook 将代表组自动接受所有会议请求。 只能[接受](../api/event-accept.md)、[暂时接受](../api/event-tentativelyaccept.md)或[拒绝](../api/event-decline.md)用户日历中的会议请求。
  - Outlook 不支持对组事件提供提醒。 只能[推迟](../api/event-snoozereminder.md)或[取消](../api/event-dismissreminder.md)用户日历的[提醒](reminder.md)。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[列出日历](../api/user-list-calendars.md)|[日历](calendar.md) 集合|获取所有用户的日历，或者获取默认或其他特定日历组中的日历。|
|[创建日历](../api/user-post-calendars.md) |[calendar](calendar.md)| 在默认日历组或用户的指定日历组中新建日历。|
|[Get calendar](../api/calendar-get.md) | [calendar](calendar.md) |获取 **calendar** 对象的属性和关系。 可以是用户的日历，也可以是 Office 365 组的默认日历。 |
|[Update](../api/calendar-update.md) | [calendar](calendar.md)  |更新 **calendar** 对象的属性。 可以是用户的日历，也可以是 Office 365 组的默认日历。 |
|[Delete](../api/calendar-delete.md) | 无 |删除 calendar 对象。 |
|[列出 calendarView](../api/calendar-list-calendarview.md) |[事件](event.md) 集合| 从用户的主日历 `(../me/calendarview)` 或指定日历中，获取由时间范围定义的日历视图中的事件发生次数、异常和单个实例。|
|[列出事件](../api/calendar-list-events.md) |[事件](event.md) 集合| 检索日历中的事件列表。该列表包含单实例会议和系列主控事件。|
|[创建事件](../api/calendar-post-events.md) |[event](event.md)| 在默认或指定日历中创建新事件。|
|[getSchedule](../api/calendar-getschedule.md) |[scheduleInformation](scheduleinformation.md) 集合|获取用户、通讯组列表或资源在指定时间段内的忙/闲状态信息。 |
|[findMeetingTimes](../api/user-findmeetingtimes.md) |[meetingTimeSuggestionsResult](meetingtimesuggestionsresult.md) |根据组织者和与会者忙/闲状态以及时间或地点约束，建议会议时间和地点。 |
|[创建单值扩展属性](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[日历](calendar.md)  |在新建或现有日历中创建一个或多个单值扩展属性。   |
|[获取包含单值扩展属性的日历](../api/singlevaluelegacyextendedproperty-get.md)  | [日历](calendar.md) | 通过使用 `$expand` 或 `$filter` 获取包含一个单值扩展属性的日历。 |
|[创建多值扩展属性](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [日历](calendar.md) | 在新建或现有的日历中创建一个或多个多值扩展属性。  |
|[获取包含多值扩展属性的日历](../api/multivaluelegacyextendedproperty-get.md)  | [日历](calendar.md) | 使用 `$expand` 获取包含一个多值扩展属性的日历。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|canEdit |布尔 |如果用户可以写入日历则为 true，否则为 false。对于创建此日历的用户，此属性为 true。此属性对于共享日历并且授予写入访问权限的用户同样为 true。 |
|canShare |布尔 |如果用户有权共享日历则为 ture，否则为 false。只有创建日历的用户才可以进行共享。 |
|canViewPrivateItems |Boolean |如果用户可以读取已标记为私有的日历项，则为 true，否则返回 false。 |
|changeKey|字符串|标识 calendar 对象的版本。每次日历更改时，changeKey 也将更改。这样，Exchange 可以将更改应用于该对象的正确版本。只读。|
|color|String|在 UI 中指定将该日历与其他日历区分开来的颜色主题。属性值有：LightBlue=0、LightGreen=1、LightOrange=2、LightGray=3、LightYellow=4、LightTeal=5、LightPink=6、LightBrown=7、LightRed=8、MaxColor=9、Auto=-1|
|hexColor|String|一种表示日历的颜色。 该颜色由 6 位 3 字节十六进制数表示。 每个字节表示颜色的红色、绿色和蓝色分量之一（位于 00 到 FF 范围内，以十六进制表示法表示）。 |
|id|String|组的唯一标识符。只读。|
|isDefaultCalendar|Boolean|如果此日历是用户的默认日历，则值为 true，否则为 false。|
|isShared |Boolean |如果用户已与其他用户共享日历，则值为 true，否则为 false。 由于只有创建日历的用户才能共享日历，因此同一用户的 **isShared** 和 **isSharedWithMe** 不能为 true。 |
|isSharedWithMe |Boolean |如果用户已共享此日历，则值为 true，否则为 false。 对于日历所有者，此属性始终为 false。  |
|name|String|日历名称。|
|owner |[emailAddress](emailaddress.md) | 如果设置，则表示创建或添加日历的用户。对于用户创建或添加的日历，将 **owner** 属性设置为用户。对于与用户共享的日历，将 **owner** 属性设置为与此用户共享该日历的人员。 |

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|calendarView|[event](event.md) 集合|日历的日历视图。导航属性。只读。|
|events|[event](event.md) 集合|日历中的事件。导航属性。只读。|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) 集合| 为日历定义的多值扩展属性的集合。只读。可为 Null。|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection| 为日历定义的单值扩展属性的集合。只读。可为 Null。|

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
  "canEdit": "boolean",
  "canShare": "boolean",
  "canViewPrivateItems": "boolean",
  "changeKey": "string",
  "color": "String",
  "hexColor": "String",
  "id": "string (identifier)",
  "isDefaultCalendar": "boolean",
  "isShared": "boolean",
  "isSharedWithMe": "boolean",
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
