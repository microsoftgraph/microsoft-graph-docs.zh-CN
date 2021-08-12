---
title: 日历资源类型
description: 日历即事件容器。 它可以是用户的日历，或者是 Microsoft 365 组的默认日历。
localization_priority: Priority
author: harini84
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: a412e6f8a8a8faa78cbe8f09f17635742bbd1e2c60a470cf1e5f9e544d424717
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54130392"
---
# <a name="calendar-resource-type"></a>日历资源类型

命名空间：microsoft.graph

表示[事件](event.md)资源的容器。 它可以是 [用户](user.md)的日历，或者 Microsoft 365 [组](group.md)的默认日历。

> **注意：** 与用户日历和组日历交互的方式稍有不同：

- 只能将用户日历组织到 [calendarGroup](calendargroup.md) 中。
- Outlook 将代表组自动接受所有会议请求。 只能[接受](../api/event-accept.md)、[暂时接受](../api/event-tentativelyaccept.md)或[拒绝](../api/event-decline.md)用户日历中的会议请求。
- Outlook 不支持对组事件提供提醒。 只能[推迟](../api/event-snoozereminder.md)或[取消](../api/event-dismissreminder.md)用户日历的[提醒](reminder.md)。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[列出日历](../api/user-list-calendars.md)|[日历](calendar.md) 集合|获取所有用户的日历，或者获取默认或其他特定日历组中的日历。|
|[创建日历](../api/user-post-calendars.md) |[calendar](calendar.md)| 在默认日历组或用户的指定日历组中新建日历。|
|[Get calendar](../api/calendar-get.md) | [calendar](calendar.md) |获取 **calendar** 对象的属性和关系。 可以是用户的日历，也可以是 Microsoft 365 组的默认日历。 |
|[更新](../api/calendar-update.md) | [calendar](calendar.md)  |更新 **calendar** 对象的属性。 可以是用户的日历，也可以是 Microsoft 365 组的默认日历。 |
|[删除](../api/calendar-delete.md) | 无 |删除 calendar 对象。 |
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
| 属性     | 类型   |Description|
|:---------------|:--------|:----------|
|allowedOnlineMeetingProviders|OnlineMeetingProviderType 集合| 表示此日历中可用于创建联机会议的联机会议服务提供商。 可取值为：`unknown`、`skypeForBusiness`、`skypeForConsumer`、`teamsForBusiness`。|
|canEdit |Boolean |`true` 如果用户可以写入日历，则 `false` 更改。 此属性 `true` 日历的用户所使用。 此属性也 `true` 已共享日历并授予写入访问权限的用户使用。 |
|canShare |Boolean |`true` 如果用户有共享日历的权限，则 `false` 更改。 只有创建日历的用户才可以进行共享。 |
|canViewPrivateItems |Boolean |`true` 如果用户可以阅读标记为私密的日历项目，则 `false` 更改。 |
|changeKey|字符串|标识 calendar 对象的版本。每次日历更改时，changeKey 也将更改。这样，Exchange 可以将更改应用于该对象的正确版本。只读。|
|颜色|calendarColor|在 UI 中指定将该日历与其他日历区分开来的颜色主题。 属性值为： `auto`、 `lightBlue`、 `lightGreen`、 `lightOrange`、 `lightGray`、 `lightYellow`、 `lightTeal`、 `lightPink`、 `lightBrown`、 `lightRed`、 `maxColor`。|
|defaultOnlineMeetingProvider|onlineMeetingProviderType|从此日历发送的会议的默认联机会议提供商。 可取值为：`unknown`、`skypeForBusiness`、`skypeForConsumer`、`teamsForBusiness`。|
|hexColor |String |日历颜色，以三个十六进制值的六进制值（每个值从 00 到 FF）表示，表示 RGB 颜色空间内颜色的红色、绿色或蓝色组成部分。 若用户从未明确设置日历的颜色，则此属性为空。 只读。|
|id|String|日历的唯一标识符。只读。|
|isDefaultCalendar|Boolean|`true` 如果这是默认情况下创建新事件的默认日历，则 `false` 更改。|
|isRemovable|Boolean| 表示是否可以从用户邮箱删除此用户日志。|
|isTallyingResponses|Boolean|表示此用户日历是否支持会议响应跟踪。 仅从用户的主日志发送的会议邀请支持会议响应跟踪。|
|name|String|日历名称。|
|owner |[emailAddress](emailaddress.md) | 如果设置，则表示创建或添加日历的用户。对于用户创建或添加的日历，将 **owner** 属性设置为用户。对于与用户共享的日历，将 **owner** 属性设置为与此用户共享该日历的人员。 |

## <a name="relationships"></a>关系
| 关系 | 类型   |Description|
|:---------------|:--------|:----------|
|calendarPermissions|[calendarPermission](calendarpermission.md) 集合| 共享日历的用户的权限。|
|calendarView|[事件](event.md) 集合|日历的日历视图。导航属性。只读。|
|events|[事件](event.md) 集合|日历中的事件。导航属性。只读。|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) 集合| 为日历定义的多值扩展属性的集合。只读。可为 Null。|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection| 为日历定义的单值扩展属性的集合。只读。可为 Null。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "calendarView",
    "events",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.calendar",
  "@odata.annotations": [
    {
      "property": "calendarView",
      "capabilities": {
        "changeTracking": true,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "navigability": "single",
        "searchable": false,
        "updatable": false
      }
    },
    {
      "property": "events",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "navigability": "single",
        "searchable": false
      }
    }
  ]
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
  "isTallyingResponses": "boolean",
  "name": "string",
  "owner": {"@odata.type": "microsoft.graph.emailAddress"}
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "calendar resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

