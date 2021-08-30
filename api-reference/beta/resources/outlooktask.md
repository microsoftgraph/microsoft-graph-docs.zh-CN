---
title: outlookTask 资源类型
description: '可用于跟踪工作项目的 Outlook 项目。 '
author: mashriv
ms.localizationpriority: high
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: f4cf54ad1420cd18ac8d7665ba8bdf02f4bc0dc2
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/30/2021
ms.locfileid: "58695264"
---
# <a name="outlooktask-resource-type-deprecated"></a>outlookTask 资源类型（不推荐使用）

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]

可用于跟踪工作项目的 Outlook 项目。

你可以使用任务来跟踪开始、截止和实际完成日期及时间、其进度或状态、它是否为定期任务并且需要提醒。

**outlookTask** 资源中与日期相关的属性包括：

- completedDateTime
- createdDateTime
- dueDateTime
- lastModifiedDateTime
- reminderDateTime
- startDateTime

默认情况下，POST、GET、PATCH 和[完成](../api/outlooktask-complete.md)操作会在 UTC 的 REST 响应中返回与日期相关的属性。
你可以使用 `Prefer: outlook.timezone` 标头将响应中的所有与日期相关的属性都表示为与 UTC 不同的时区。 以下示例在对应响应的 EST 中返回与日期相关的属性：

```
Prefer: outlook.timezone="Eastern Standard Time"
```

## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 outlookTask](../api/outlooktask-get.md) | [outlookTask](outlooktask.md) |获取用户邮箱中的 Outlook 任务的属性和关系。|
|[更新](../api/outlooktask-update.md) | [outlookTask](outlooktask.md) |更改 Outlook 任务的可写属性。 |
|[删除](../api/outlooktask-delete.md) | 无 |删除用户邮箱中的指定任务。 |
|[完成](../api/outlooktask-complete.md)|[outlookTask](outlooktask.md) 集合|完成 Outlook 任务，它将 **completedDateTime** 属性设置为当前日期，并将 **status** 属性设置为 `completed`。|
|**附件**| | |
|[列出附件](../api/outlooktask-list-attachments.md) |[attachment](attachment.md) 集合| 获取 Outlook 任务的所有附件。|
|[添加附件](../api/outlooktask-post-attachments.md) |[附件](attachment.md)| 向任务添加作为附件的文件、项目（消息、事件或联系人）或文件链接。|
|**扩展属性**| | |
|[创建单值扩展属性](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[outlookTask](outlooktask.md)  |在新建或现有 Outlook 任务中创建一个或多个单值扩展属性。   |
|[获取具有单值扩展属性的任务](../api/singlevaluelegacyextendedproperty-get.md)  | [outlookTask](outlooktask.md) | 通过使用 `$expand` 或 `$filter` 获取包含单值扩展属性的 Outlook 任务。 |
|[创建多值扩展属性](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [outlookTask](outlooktask.md) | 在新建或现有的 Outlook 任务中创建一个或多个多值扩展属性。  |
|[获取具有多值扩展属性的任务](../api/multivaluelegacyextendedproperty-get.md)  | [outlookTask](outlooktask.md) | 使用 `$expand` 获取包含一个多值扩展属性的 Outlook 任务。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|assignedTo|String|Outlook 中已为其分配任务的人员姓名。只读。|
|body|[itemBody](itembody.md)|通常包含有关任务的信息的任务正文。 请注意，仅支持 HTML 类型。|
|类别|String 集合|与任务关联的类别。 每个类别对应于用户定义的 [outlookCategory](outlookcategory.md) 的 **displayName** 属性。|
|changeKey|String|任务的版本。|
|completedDateTime|[dateTimeTimeZone](datetimetimezone.md)|在指定时区内完成任务的日期。|
|createdDateTime|DateTimeOffset|任务的创建日期和时间。 默认情况下，它采用 UTC 格式。 你可以在请求标头中提供自定义时区。 属性值使用 ISO 8601 格式。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
|dueDateTime|[dateTimeTimeZone](datetimetimezone.md)|要在指定时区内完成任务的日期。|
|hasAttachments|Boolean|如果任务包含附件，则设置为 true。|
|id|String| 任务的唯一标识符。 [!INCLUDE [outlook-beta-id](../../includes/outlook-beta-id.md)] 只读。 |
|importance|importance|事件的重要性。 可取值为：`low`、`normal`、`high`。|
|isReminderOn|Boolean|如果设置警报以提醒用户有任务，则设置为 true。|
|lastModifiedDateTime|DateTimeOffset|上次修改任务的日期和时间。 默认情况下，它采用 UTC 格式。 你可以在请求标头中提供自定义时区。 属性值使用 ISO 8601 格式，并始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
|Owner|String|任务创建者的姓名。|
|parentFolderId|String|任务的父文件夹的唯一标识符。|
|定期|[patternedRecurrence](patternedrecurrence.md)|任务的定期模式。|
|reminderDateTime|[dateTimeTimeZone](datetimetimezone.md)|提醒警报发出任务发生提醒的日期和时间。|
|敏感度|敏感度|指示任务的隐私级别。 可取值为：`normal`、`personal`、`private`、`confidential`。|
|startDateTime|[dateTimeTimeZone](datetimetimezone.md)|要在指定时区内开始执行任务的日期。|
|状态|任务状态|指示任务的状态或进度。 可取值为：`notStarted`、`inProgress`、`completed`、`waitingOnOthers`、`deferred`。|
|主题|String|任务的简要说明或标题。|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|attachments|[attachment](attachment.md) 集合|任务的 [fileAttachment](fileattachment.md)、[itemAttachment](itemattachment.md) 和 [referenceAttachment](referenceattachment.md) 附件的集合。  只读。 可为空。|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) 集合|为任务定义的多值扩展属性的集合。只读。可为 NULL。|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection|为任务定义的单值扩展属性的集合。只读。可为 NULL。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "attachments",
    "singleValueExtendedProperties",
    "multiValueExtendedProperties"
  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
  "@odata.type": "microsoft.graph.outlookTask"
}-->

```json
{
  "assignedTo": "String",
  "body": {"@odata.type": "microsoft.graph.itemBody"},
  "categories": ["String"],
  "changeKey": "String",
  "completedDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "createdDateTime": "String (timestamp)",
  "dueDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "hasAttachments": true,
  "id": "String (identifier)",
  "importance": "string",
  "isReminderOn": true,
  "lastModifiedDateTime": "String (timestamp)",
  "owner": "String",
  "parentFolderId": "String",
  "recurrence": {"@odata.type": "microsoft.graph.patternedRecurrence"},
  "reminderDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "sensitivity": "string",
  "startDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "status": "string",
  "subject": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "outlookTask resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


