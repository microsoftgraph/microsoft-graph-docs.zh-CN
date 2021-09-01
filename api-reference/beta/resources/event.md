---
title: 事件资源类型
description: 日历中的事件。
author: harini84
ms.localizationpriority: high
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 372de4192c0cf4687fa37a128bc68d9eeb77711c
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/30/2021
ms.locfileid: "58696902"
---
# <a name="event-resource-type"></a>事件资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[用户](user.md)日历或 Microsoft 365 [组](group.md)默认日历中的事件。

**事件** 中包含的最大与会者人数，以及发送自 Exchange Online 邮箱的 [eventMessage](eventmessage.md) 中的收件人数上限都是 500 人。 有关详细信息，请参阅[发送限制](/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#sending-limits)。

该资源支持：

- 将你自己的数据作为[扩展](/graph/extensibility-overview)添加到自定义属性。
- 订阅[更改通知](/graph/webhooks)。
- 通过提供 [delta](../api/event-delta.md) 函数，使用 [delta 查询](/graph/delta-query-overview)跟踪增量添加、删除和更新。

> **注释：** 与用户日历、组日历及其事件交互的方式稍有不同：

- 只可以组织 [calendarGroup](calendargroup.md) 中的用户日历。
- 只能将 [attachment](attachment.md) 对象添加到用户日历中的事件，而不能添加到组日历中的事件。
- Outlook 将代表组自动接受所有会议请求。 只可以 [接受](../api/event-accept.md)、[暂时接受](../api/event-tentativelyaccept.md)或 [拒绝](../api/event-decline.md)_用户_ 日历中的会议请求。
- Outlook 不支持对组事件提供提醒。 只可以 [暂停](../api/event-snoozereminder.md)或 [消除](../api/event-dismissreminder.md)_用户_ 日历中的 [提醒](reminder.md)。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
   "keyProperty": "id",
  "optionalProperties": [
    "attachments",
    "calendar",
    "extensions",
    "instances",
    "singleValueExtendedProperties",
    "multiValueExtendedProperties"
  ],
  "@odata.type": "microsoft.graph.event"
}-->

```json
{
  "allowNewTimeProposals": "Boolean",
  "attendees": [{"@odata.type": "microsoft.graph.attendee"}],
  "body": {"@odata.type": "microsoft.graph.itemBody"},
  "bodyPreview": "string",
  "cancelledOccurrences":["string"],
  "categories": ["string"],
  "changeKey": "string",
  "createdDateTime": "String (timestamp)",
  "end": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "exceptionOccurrences":["string"],
  "hasAttachments": true,
  "hideAttendees": false,
  "uid": "string",
  "id": "string (identifier)",
  "importance": "String",
  "isAllDay": true,
  "isCancelled": true,
  "isDraft": false,
  "isOnlineMeeting": true,
  "isOrganizer": true,
  "isReminderOn": true,
  "lastModifiedDateTime": "String (timestamp)",
  "location": {"@odata.type": "microsoft.graph.location"},
  "locations": [{"@odata.type": "microsoft.graph.location"}],
  "occurrenceId":"string",
  "onlineMeeting": {"@odata.type": "microsoft.graph.onlineMeetingInfo"},
  "onlineMeetingProvider": "string",
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
  "singleValueExtendedProperties": [ { "@odata.type": "microsoft.graph.singleValueLegacyExtendedProperty" }],
  "multiValueExtendedProperties": [ { "@odata.type": "microsoft.graph.multiValueLegacyExtendedProperty" }]
}
```
## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|allowNewTimeProposals| 布尔值 | 如果会议组织者允许被邀请者在响应时建议新时间，则为`True`；否则为 `false`。 可选。 默认值为 `true`。 |
|attendees|[Attendee](attendee.md) 集合|事件的与会者集合。|
|body|[ItemBody](itembody.md)|与事件相关联的邮件正文。可以是 HTML 格式或文本格式。|
|bodyPreview|字符串|与事件相关联的邮件预览。文本格式。|
|cancelledOccurrences|字符串集合|包含定期系列中已取消实例的 **occurrenceId** 属性值（如果该事件为系列母版事件）。 定期系列中已取消的实例称为 cancelledOccurences。<br><br>仅在 [Get](../api/event-get.md) 操作的 $select 中返回，该操作指定系列母版事件（即 seriesMasterId 属性值）的 ID。|
|categories|String collection|与事件相关联的类别。 每个类别对应于为用户定义的 [outlookCategory](outlookcategory.md) 的 **displayName** 属性。|
|changeKey|String|标识 event 对象的版本。每次事件更改时，ChangeKey 也将更改。这样，Exchange 可以将更改应用于该对象的正确版本。|
|createdDateTime|DateTimeOffset|时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`2014-01-01T00:00:00Z`|
|end|[DateTimeTimeZone](datetimetimezone.md)|事件结束的日期、时间和时区。 默认情况下，结束时间为 UTC 时间。|
|exceptionOccurrences|字符串集合|包含定期系列中的例外事件实例的 **id** 属性值。<br>异常可能不同于定期系列中的其他事件，例如主题、开始或结束时间或与会者。异常不包括已取消的事件。<br><br>仅在 [Get](../api/event-get.md) 操作的 $select 和 $expand 中返回，该操作指定系列母版事件（即 seriesMasterId 属性值）的 ID。|
|hasAttachments|Boolean|如果事件包含附件，则设置为 true。|
|hideAttendees|布尔值|如果设置为 `true`，则每个与会者仅会在会议请求和会议 **跟踪** 列表中看到自己。 默认为 false。|
|id|String| 事件的唯一标识符。 [!INCLUDE [outlook-beta-id](../../includes/outlook-beta-id.md)] 只读。 |
|importance|String|事件的重要性。 可取值为：`low`、`normal`、`high`。|
|isAllDay|Boolean|如果事件持续整天则设为 true。如果为 true，则无论是单天事件还是多天事件，都必须将开始和结束时间设置为午夜，并且必须处于同一时区。|
|isCancelled|Boolean|如果事件已取消，则设置为 true。|
|isDraft|Boolean|如果用户在 Outlook 中更新了会议，但尚未将更新发送给与会者，则设置为 true。 如果所有更改均已发送，或者如果事件是不带任何与会者的约会，则设置为 false。|
|isOnlineMeeting|Boolean| 若此事件包含联机会议信息（即 **onlineMeeting** 指向 [onlineMeetingInfo](onlinemeetinginfo.md) 资源）则为 `True`，反之则为 `false`。 默认值为 `false`（**onlineMeeting** 为 `null`）。 可选。 <br> 将 **isOnlineMeeting** 设置为 `true` 后，Microsoft Graph 将初始化 **onlineMeeting**。 随后，Outlook 将忽略对 **isOnlineMeeting** 的任何进一步更改，并且会议仍保持联机。 |
|isOrganizer|Boolean|如果日历所有者（通过“[日历](calendar.md)”的“**所有者**”属性指定）是事件的组织者（通过“**事件**”的“**组织者**”属性指定），设定为 true。 这也适用于代理人代表所有者组织事件。|
|isReminderOn|Boolean|如果设置警报以提醒用户有事件，则设置为 true。|
|lastModifiedDateTime|DateTimeOffset|时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`2014-01-01T00:00:00Z`|
|位置|[位置](location.md)|事件的位置。|
|位置|[location](location.md) 集合|举办或参加活动的地点。 **location** 和 **locations** 属性总是相互对应。 如果更新 **location** 属性，**locations** 集合中所有以前的位置都将被删除并替换为新的 **location** 值。 |
|occurrenceId|字符串|定期事件系列中的事件的标识符。 如果该事件不属于定期系列，则为 Null。<br><br>属性值的格式为 OID.{seriesMasterId-value}.{occurrence-start-date}。 {occurrence-start-date} 的时区是为相应 [recurrenceRange](recurrencerange.md) 定义的 recurrenceTimeZone 属性。<br><br>此属性可以识别定期系列中的任何事件，包括已修改或已取消的事件。 可使用此属性执行定期系列中的事件所支持的所有操作。|
|onlineMeeting|[OnlineMeetingInfo](onlinemeetinginfo.md)| 与会者联机加入会议的详细信息。默认值为 null。只读。 <br>设置 **isOnlineMeeting** 和 **onlineMeetingProvider** 属性以启用联机会议后，Microsoft Graph 将初始化 **onlineMeeting**。 设置后，会议仍保持联机，并且不能再次更改 **isOnlineMeeting**、**onlineMeetingProvider** 和 **onlneMeeting** 属性。|
|onlineMeetingProvider|onlineMeetingProviderType| 表示联机会议服务提供商。 默认情况下，**onlineMeetingProvider** 为 `unknown`。 可取值为：`unknown`、`teamsForBusiness`、`skypeForBusiness` 和 `skypeForConsumer`。 可选。 <br> 设置 **isOnlineMeeting** 后，Microsoft Graph 将初始化 **onlineMeeting**。 随后，你不能再次更改 **onlineMeetingProvider**，并且会议仍保持联机。 |
|onlineMeetingUrl|String|联机会议的 URL。仅当组织者在 Outlook 中将事件指定为联机会议（如 Skype）时才会设置此属性。只读。<br>若要访问 URL 参加联机会议，请使用通过 **event** 的 **onlineMeeting** 属性公开的 **joinUrl**。 未来即将弃用 **onlineMeetingUrl** 属性。 |
|组织者|[收件人](recipient.md)|事件的组织者。|
|originalEndTimeZone|String|创建事件时设置的结束时区。`tzone://Microsoft/Custom` 值表示旧的自定义时区在桌面版 Outlook 中设置。|
|originalStart|DateTimeOffset|时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`2014-01-01T00:00:00Z`|
|originalStartTimeZone|字符串|创建事件时设置的开始时区。`tzone://Microsoft/Custom` 值表示旧的自定义时区在桌面版 Outlook 中设置。|
|recurrence|[PatternedRecurrence](patternedrecurrence.md)|事件的定期模式。|
|reminderMinutesBeforeStart|Int32|事件开始时间（即提醒警报发生时间）之前的分钟数。|
|responseRequested|布尔值|默认值为 true，表示组织者愿意被邀请者发送事件响应。|
|responseStatus|[ResponseStatus](responsestatus.md)|指示在事件消息的响应中发送的响应类型。|
|sensitivity|String| 可能的值是：`normal`、`personal`、`private`、`confidential`。|
|seriesMasterId|String|定期系列主项的 ID（如果此事件是定期系列的一部分）。|
|showAs|String|要显示的状态。 可取值为：`free`、`tentative`、`busy`、`oof`、`workingElsewhere`、`unknown`。|
|start|[DateTimeTimeZone](datetimetimezone.md)|事件的开始日期、时间和时区。 默认情况下，开始时间使用 UTC 格式。|
|subject|String|事件的主题行文本。|
|transactionId|字符串|客户端应用为服务器指定的自定义标识符，用于避免因客户端重试创建相同事件而导致冗余的 [POST](../api/calendar-post-events.md) 操作。 当低网络连接性导致客户端在从服务器中收到客户端先前创建事件请求的响应之前超时时，此功能很有用。 你在创建事件时设置 **transactionId**，之后不能在后续更新中更改 **transactionId**。 如果应用已设置此属性，则仅在响应有效负载中返回此属性。 可选。|
|type|String|事件类型。 可取值为：`singleInstance`、`occurrence`、`exception`、`seriesMaster`。 只读|
|uid|字符串|日历事件的唯一标识符。 对于定期事件，Series Master 及其所有事件（包括异常）的此值均相同。 此属性将替换[事件资源](/graph/api/resources/event?view=graph-rest-1.0&preserve-view=true)中定义的当前 iCalUid 属性（对于序列中各个实例而言各不相同）。|
|webLink|String|要在 Web 上的 Outlook 中打开事件的 URL。<br/><br/>如果登录邮件，则 Outlook 网页面会在浏览器中打开事件。 否则，Outlook 网页面会提示你进行登录。<br/><br/>无法从 iFrame 中访问此 URL。|

> [!NOTE]
> **webLink** 属性指定了一个 URL，它仅在 Outlook 网页版早期版本中打开事件。 其 URL 的格式如下所示，其中 _{event-id}_ 是 **id** 属性的 _**URL 编码**_ 值：
>
> * 对于工作或学校帐户：`https://outlook.office365.com/owa/?itemid={event-id}&exvsurl=1&path=/calendar/item`
>
> * 对于 Microsoft 帐户：`https://outlook.live.com/owa/?itemid={event-id}&exvsurl=1&path=/calendar/item`
>
> 要在 Outlook 网页版的当前版本中打开事件，请将 URL 转换为下述格式之一，并使用该 URL 打开事件：
>
> * 对于工作或学校帐户：`https://outlook.office365.com/calendar/item/{event-id}`
>
> * 对于 Microsoft 帐户：`https://outlook.live.com/calendar/item/{event-id}`


## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|attachments|[Attachment](attachment.md) 集合|事件的 [FileAttachment](fileattachment.md)、[ItemAttachment](itemattachment.md) 和 [referenceAttachment](referenceattachment.md) 附件的集合。 导航属性。 只读。 可为 Null。|
|日历|[Calendar](calendar.md)|包含 event. Navigation 属性的日历。只读。|
|extensions|[Extension](extension.md) 集合|为事件定义的开放扩展集合。可为空。|
|实例|[Event](event.md) 集合|定期系列的出现次数（如果该事件是系列母版事件）。 此属性包括定期模式的组成事件和已修改的例外，但不包括已从系列中取消的事件。 导航属性。 只读。 可为空。|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) 集合| 为事件定义的多值扩展属性的集合。只读。可为 Null。|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection| 为事件定义的单值扩展属性的集合。只读。可为空。|

## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[列出事件](../api/user-list-events.md)|[Event](event.md) 集合 |检索用户邮箱中的 [event](../resources/event.md) 对象列表。该列表包含单个实例会议和系列主控形状。|
|[创建事件](../api/user-post-events.md) |[事件](event.md)| 通过发布到实例集合创建新事件。|
|[获取事件](../api/event-get.md) | [事件](event.md) |读取 event 对象的属性和关系。|
|[更新](../api/event-update.md) | [事件](event.md)   |更新事件对象。 |
|[删除](../api/event-delete.md) | 无 |删除 event 对象。 |
|[delta](../api/event-delta.md)|[事件](event.md)集合|获取用户主日历的 **calendarView**（事件范围）中已添加、删除或更新的事件集。|
|[转发](../api/event-forward.md)|无|让会议事件的组织者或与会者可以将会议请求转发给新的收件人。|
|[取消](../api/event-cancel.md) | 无 | 将取消消息从组织者发送至所有与会者，并取消指定会议。 |
|[接受](../api/event-accept.md)|无|接受用户日历中的指定事件。|
|[tentativelyAccept](../api/event-tentativelyaccept.md)|无|暂时接受用户日历中的指定事件。|
|[拒绝](../api/event-decline.md)|无|拒绝用户日历中的指定事件邀请。|
|[dismissReminder](../api/event-dismissreminder.md)|无|消除用户日历中指定事件的提醒。|
|[snoozeReminder](../api/event-snoozereminder.md)|无|将用户日历中指定事件的提醒推迟至新的时间。|
|[列出实例](../api/event-list-instances.md) |[Event](event.md) 集合| 获取 Event 对象集合。|
|**附件**| | |
|[列出附件](../api/event-list-attachments.md) |[Attachment](attachment.md) 集合| 获取事件的所有附件。|
|[Add attachment](../api/event-post-attachments.md) |[附件](attachment.md)| 通过发布到附件集合，向事件添加新附件。|
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
<!--
{
  "type": "#page.annotation",
  "description": "event resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
