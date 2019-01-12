---
title: 日历资源类型
description: 日历即事件容器。 可以是用户的日历，也可以是 Office 365 组的默认日历。
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 6d7f926c26b0fdcf0c70e7f6d02593cff8bb46a6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917620"
---
# <a name="calendar-resource-type"></a>日历资源类型

日历即事件容器。 可以是[用户](user.md)的日历，也可以是 Office 365 [组](group.md)的默认日历。

> **注意：** 有几个您可以与用户日历和日历组进行交互的方式不同：

 - 您可以组织只有用户日历中[calendarGroup](calendargroup.md)。
 - Outlook 自动接受代表组的所有会议请求。 您可以为用户日历仅[接受](../api/event-accept.md)、[暂时接受](../api/event-tentativelyaccept.md)或[拒绝](../api/event-decline.md)会议请求。
  - Outlook 不支持为组事件的提醒。 您可以为仅用户日历[snooze](../api/event-snoozereminder.md)或[消除](../api/event-dismissreminder.md)的[提醒](reminder.md)。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[列出日历](../api/user-list-calendars.md)|[日历](calendar.md) 集合|获取所有用户的日历，或者获取默认或其他特定日历组中的日历。|
|[创建日历](../api/user-post-calendars.md) |[calendar](calendar.md)| 在默认日历组或用户的指定日历组中新建日历。|
|[Get calendar](../api/calendar-get.md) | [calendar](calendar.md) |获取 **calendar** 对象的属性和关系。 可以是用户的日历，也可以是 Office 365 组的默认日历。 |
|[Update](../api/calendar-update.md) | [calendar](calendar.md)  |更新 **calendar** 对象的属性。 可以是用户的日历，也可以是 Office 365 组的默认日历。 |
|[Delete](../api/calendar-delete.md) | 无 |删除 calendar 对象。 |
|[列出 calendarView](../api/calendar-list-calendarview.md) |[事件](event.md) 集合| 从用户的主日历 `(../me/calendarview)` 或指定日历中，获取由时间范围定义的日历视图中的事件发生次数、异常和单个实例。|
|[列出事件](../api/calendar-list-events.md) |[事件](event.md) 集合| 检索日历中的事件列表。该列表包含单个实例会议和系列主控形状。|
|[创建事件](../api/calendar-post-events.md) |[事件](event.md)| 创建默认或指定的日历中的新事件。|
|[findMeetingTimes](../api/user-findmeetingtimes.md) |[meetingTimeSuggestionsResult](meetingtimesuggestionsresult.md) |建议的会议时间内和基于组织者和与会者可用性和时间或位置的约束位置。 |
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
|color|calendarColor|在 UI 中指定将该日历与其他日历区分开来的颜色主题。属性值有：LightBlue=0、LightGreen=1、LightOrange=2、LightGray=3、LightYellow=4、LightTeal=5、LightPink=6、LightBrown=7、LightRed=8、MaxColor=9、Auto=-1|
|id|String|组的唯一标识符。只读。|
|name|String|日历名称。|
|owner |[emailAddress](emailaddress.md) | 如果设置，则表示创建或添加日历的用户。对于用户创建或添加的日历，将 **owner** 属性设置为用户。对于与用户共享的日历，将 **owner** 属性设置为与此用户共享该日历的人员。 |

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
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
  "canEdit": "boolean",
  "canShare": "boolean",
  "canViewPrivateItems": "boolean",
  "changeKey": "string",
  "color": "String",
  "id": "string (identifier)",
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
