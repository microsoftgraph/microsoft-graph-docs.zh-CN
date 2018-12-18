---
title: 事件资源类型
description: 日历中的事件。
author: angelgolfer-ms
ms.openlocfilehash: 45b5131b14e9bf50c8dc0bc3db869b706a3068ba
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27340647"
---
# <a name="event-resource-type"></a>事件资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

日历中的事件。

该资源支持：

- 将您自己的数据添加到自定义属性，作为[扩展](/graph/extensibility-overview)。
- 订阅[更改通知](/graph/webhooks)。
- 通过提供 [delta](../api/event-delta.md) 函数使用[增量查询](/graph/delta-query-overview)跟踪增量添加、删除和更新。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "attachments",
    "calendar",
    "extensions",
    "instances",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "@odata.type": "microsoft.graph.event"
}-->

```json
{
  "attendees": [{"@odata.type": "microsoft.graph.attendee"}],
  "body": {"@odata.type": "microsoft.graph.itemBody"},
  "bodyPreview": "string",
  "categories": ["string"],
  "changeKey": "string",
  "createdDateTime": "String (timestamp)",
  "end": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "hasAttachments": true,
  "iud": "string",
  "id": "string (identifier)",
  "importance": "String",
  "isAllDay": true,
  "isCancelled": true,
  "isOrganizer": true,
  "isReminderOn": true,
  "lastModifiedDateTime": "String (timestamp)",
  "location": {"@odata.type": "microsoft.graph.location"},
  "locations": [{"@odata.type": "microsoft.graph.location"}],
  "onlineMeetingUrl": "string",
  "organizer": {"@odata.type": "microsoft.graph.recipient"},
  "originalEndTimeZone": "string",
  "originalStart": "String (timestamp)",
  "originalStartTimeZone": "string",
  "recurrence": {"@odata.type": "microsoft.graph.patternedRecurrence"},
  "reminderMinutesBeforeStart": 1024,
  "responseRequested": true,
  "responseStatus": {"@odata.type": "microsoft.graph.responseStatus"},
  "sensitivity": "String",
  "seriesMasterId": "string",
  "showAs": "String",
  "start": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "subject": "string",
  "type": "String",
  "webLink": "string",
  
  "attachments": [ { "@odata.type": "microsoft.graph.attachment" } ],
  "calendar": { "@odata.type": "microsoft.graph.calendar" },
  "extensions": [ { "@odata.type": "microsoft.graph.extension" } ],
  "instances": [ { "@odata.type": "microsoft.graph.event" }],
  "multiValueExtendedProperties": [ { "@odata.type": "microsoft.graph.multiValueLegacyExtendedProperty" }],
  "singleValueExtendedProperties": [ { "@odata.type": "microsoft.graph.singleValueLegacyExtendedProperty" }]
}

```
## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|attendees|[Attendee](attendee.md)集合|事件的与会者集合。|
|body|[ItemBody](itembody.md)|与事件相关联的邮件正文。可以是 HTML 格式或文本格式。|
|bodyPreview|字符串|与事件相关联的邮件预览。文本格式。|
|categories|String collection|与事件相关联的类别。 每个类别对应于[outlookCategory](outlookcategory.md)为用户定义的**displayName**属性。|
|changeKey|String|标识 event 对象的版本。每次事件更改时，ChangeKey 也将更改。这样，Exchange 可以将更改应用于该对象的正确版本。|
|createdDateTime|DateTimeOffset|时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|end|[DateTimeTimeZone](datetimetimezone.md)|事件的结束日期和时间。|
|hasAttachments|Boolean|如果事件包含附件，则设置为 true。|
|id|String| 只读。|
|importance|String|事件的重要性。 可取值为：`low`、`normal`、`high`。|
|isAllDay|Boolean|如果事件持续一整天，则设置为 true。|
|isCancelled|Boolean|如果事件已取消，则设置为 true。|
|isOrganizer|Boolean|如果邮件发件人也是组织者，则设置为 true。|
|isReminderOn|Boolean|如果设置警报以提醒用户有事件，则设置为 true。|
|lastModifiedDateTime|DateTimeOffset|时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|location|[位置](location.md)|事件的位置。|
|locations|[位置](location.md)集合|举办或参加活动的地点。 **location** 和 **locations** 属性总是相互对应。 如果更新 **location** 属性，**locations** 集合中所有以前的位置都将被删除并替换为新的 **location** 值。 |
|onlineMeetingUrl|String|在线会议的 URL。 仅组织者指定为联机会议如 Skype 事件时，该属性是设置。 只读。|
|organizer|[Recipient](recipient.md)|事件的组织者。|
|originalEndTimeZone|String|创建事件时设置的结束时区。 `tzone://Microsoft/Custom` 值表示旧的自定义时区已在桌面版 Outlook 中设置。|
|originalStart|DateTimeOffset|时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|originalStartTimeZone|字符串|创建事件时设置的开始时区。`tzone://Microsoft/Custom` 值表示旧的自定义时区在桌面版 Outlook 中设置。|
|recurrence|[PatternedRecurrence](patternedrecurrence.md)|事件的定期模式。|
|reminderMinutesBeforeStart|Int32|事件开始时间（即提醒警报发生时间）之前的分钟数。|
|responseRequested|Boolean|如果发件人希望接收事件被接受或拒绝时的响应，则设置为 true。|
|responseStatus|[ResponseStatus](responsestatus.md)|指示在事件消息的响应中发送的响应类型。|
|sensitivity|String| 可能的值是：`normal`、`personal`、`private`、`confidential`。|
|seriesMasterId|String|定期系列主项目，如果该事件是定期系列的一部分的 ID。|
|showAs|String|要显示的状态。 可取值为：`free`、`tentative`、`busy`、`oof`、`workingElsewhere`、`unknown`。|
|start|[DateTimeTimeZone](datetimetimezone.md)|事件的开始时间。|
|subject|String|事件的主题行文本。|
|type|String|事件类型。 可取值为 `singleInstance`、`occurrence`、`exception`、`seriesMaster`。 只读|
|uid|String|由不同日历间的所有事件实例共享的唯一标识符。 **注意：** 此属性的作用相同`iCalUid`v1.0 终结点上, 对[事件资源](/graph/api/resources/event?view=graph-rest-1.0)的属性，但不是保证具有相同的值。|
|webLink|String|要在 Outlook Web App 中打开事件的 URL。<br/><br/>如果你通过 Outlook Web App 登录邮箱，该事件将在浏览器中打开。如果尚未使用浏览器登录，系统将提示你登录。<br/><br/>可以从 iFrame 中访问此 URL。|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|attachments|[附件](attachment.md) 集合|事件[FileAttachment](fileattachment.md)和[ItemAttachment](itemattachment.md)， [referenceAttachment](referenceattachment.md)附件的集合。 导航属性。 只读。 可为 Null。|
|calendar|[Calendar](calendar.md)|包含事件的日历。导航属性。只读。|
|extensions|[扩展](extension.md)集合|定义的事件的打开扩展的集合。 可为 Null。|
|instances|[Event](event.md) collection|事件的实例。导航属性。只读。可为 Null。|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) 集合| 为事件定义的多值扩展属性的集合。只读。可为 Null。|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection| 为事件定义的单值扩展属性的集合。只读。可为 Null。|

## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[列出事件](../api/user-list-events.md)|[Event](event.md) collection |检索用户邮箱中的 [event](../resources/event.md) 对象列表。该列表包含单个实例会议和系列主控形状。|
|[创建事件](../api/user-post-events.md) |[事件](event.md)| 通过发布到实例集合创建新事件。|
|[获取事件](../api/event-get.md) | [事件](event.md) |读取 event 对象的属性和关系。|
|[更新](../api/event-update.md) | [事件](event.md)   |更新事件对象。 |
|[删除](../api/event-delete.md) | 无 |删除事件对象。 |
|[cancel](../api/event-cancel.md) | 无 | 从组织者的取消消息发送给所有与会者和取消指定的会议。 |
|[接受](../api/event-accept.md)|无|接受指定的事件。|
|[tentativelyAccept](../api/event-tentativelyaccept.md)|无|暂时接受指定的事件。|
|[拒绝](../api/event-decline.md)|无|拒绝对指定事件的邀请。|
|[转发](../api/event-forward.md)|无|允许将会议请求转发到新收件人的组织者或与会者的会议事件。|
|[delta](../api/event-delta.md)|[事件](event.md)集合|获取用户主日历的 **calendarView**（事件范围）中已添加、删除或更新的事件集。|
|[dismissReminder](../api/event-dismissreminder.md)|无|消除指定事件的提醒。|
|[snoozeReminder](../api/event-snoozereminder.md)|无|暂停指定事件的提醒。|
|[列出实例](../api/event-list-instances.md) |[Event](event.md) collection| 获取 Event 对象集合。|
|**附件**| | |
|[列出附件](../api/event-list-attachments.md) |[附件](attachment.md) 集合| 获取事件的所有附件。|
|[Add attachment](../api/event-post-attachments.md) |[Attachment](attachment.md)| 通过发布到附件集合，向事件添加新附件。|
|**开放扩展**| | |
|[创建开放扩展](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| 创建开放扩展，并将自定义属性添加到新资源或现有资源。|
|[获取开放扩展](../api/opentypeextension-get.md) |[openTypeExtension](opentypeextension.md) 集合| 获取扩展名称标识的开放扩展。|
|**架构扩展**| | |
|[添加架构扩展值](/graph/extensibility-schema-groups) || 创建架构扩展定义，然后使用它向资源添加自定义键入数据。|
|**扩展属性**| | |
|[创建单值扩展属性](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[事件](event.md)  |在新建或现有事件中创建一个或多个单值扩展属性。   |
|[获取具有单值扩展属性的事件](../api/singlevaluelegacyextendedproperty-get.md)  | [事件](event.md) | 通过使用 `$expand` 或 `$filter` 获取包含单值扩展属性的事件。 |
|[创建多值扩展属性](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [事件](event.md) | 在新建或现有的事件中创建一个或多个多值扩展属性。  |
|[获取具有多值扩展属性的事件](../api/multivaluelegacyextendedproperty-get.md)  | [事件](event.md) | 使用 `$expand` 获取包含一个多值扩展属性的事件。 |

## <a name="see-also"></a>另请参阅

- [使用增量查询跟踪 Microsoft Graph 数据更改](/graph/delta-query-overview)
- [获取文件夹中事件的增量更改](/graph/delta-query-events)
- [使用扩展向资源添加自定义数据](/graph/extensibility-overview)
- [使用开放扩展向用户添加自定义数据](/graph/extensibility-open-users)
- [使用架构扩展向组添加自定义数据](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "event resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
