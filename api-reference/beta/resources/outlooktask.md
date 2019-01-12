---
title: outlookTask 资源类型
description: '可以跟踪工作项的 Outlook 项目。 '
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: f49c74af92037f430b72d7b9fffa4a85aba00942
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27943270"
---
# <a name="outlooktask-resource-type"></a>outlookTask 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

可以跟踪工作项的 Outlook 项目。 

任务可用于跟踪开始、 截止日期和实际完成日期和时间，它的进度或状态，无论它定期约会，并要求提醒。

日期相关**outlookTask**资源中的属性包括以下项：

- completedDateTime
- createdDateTime
- dueDateTime
- lastModifiedDateTime
- reminderDateTime
- startDateTime

默认情况下，POST、 获取、 PATCH 和[完成](../api/outlooktask-complete.md)操作 UTC 他们 REST 的响应中返回与日期相关的属性。 您可以使用`Prefer: outlook.timezone`标头，使其具有不同于 UTC 时区中表示的响应中的所有日期相关的属性。 下面的示例返回在东部时间与日期相关的属性的相应的响应中：

```
Prefer: outlook.timezone="Eastern Standard Time"
```

## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 outlookTask](../api/outlooktask-get.md) | [outlookTask](outlooktask.md) |获取用户的邮箱中的属性和 Outlook 任务的关系。|
|[Update](../api/outlooktask-update.md) | [outlookTask](outlooktask.md) |更改 Outlook 任务的可写属性。 |
|[删除](../api/outlooktask-delete.md) | 无 |删除用户的邮箱中指定的任务。 |
|[Complete](../api/outlooktask-complete.md)|[outlookTask](outlooktask.md)集合|完成 Outlook 任务，这将**completedDateTime**属性设置为当前日期，并**状态**属性设为`completed`。|
|**附件**| | |
|[列出附件](../api/outlooktask-list-attachments.md) |[attachment](attachment.md) 集合| 获取有关 Outlook 任务的所有附件。|
|[Add attachment](../api/outlooktask-post-attachments.md) |[attachment](attachment.md)| 添加的文件、 项 （邮件、 事件或联系人） 或链接到文件作为附件到一个任务。|
|**扩展属性**| | |
|[创建单值扩展属性](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[outlookTask](outlooktask.md)  |创建新的或现有 Outlook 任务中的一个或多个单值扩展的属性。   |
|[获取与扩展的单值属性的任务](../api/singlevaluelegacyextendedproperty-get.md)  | [outlookTask](outlooktask.md) | 获取包含一个单值使用扩展属性的 Outlook 任务`$expand`或`$filter`。 |
|[创建多值扩展属性](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [outlookTask](outlooktask.md) | 创建新的或现有 Outlook 任务中的一个或多个多值扩展的属性。  |
|[获取与多值扩展属性的任务](../api/multivaluelegacyextendedproperty-get.md)  | [outlookTask](outlooktask.md) | 获取包含多值扩展的属性，通过使用 Outlook 任务`$expand`。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|assignedTo|字符串|已分配任务的人员的名称。|
|body|[itemBody](itembody.md)|任务正文通常包含有关任务的信息。 请注意，仅 HTML 支持类型。|
|categories|String collection|类别与任务关联。 每个类别对应于用户已定义[outlookCategory](outlookcategory.md)的**displayName**属性。|
|changeKey|字符串|任务的版本。|
|completedDateTime|[dateTimeTimeZone](datetimetimezone.md)|中指定的时区任务已完成的日期。|
|createdDateTime|DateTimeOffset|日期和时间创建任务时。 默认情况下，它是采用 UTC。 您可以提供请求标头中自定义时区。 该属性值使用 ISO 8601 格式。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。|
|dueDateTime|[dateTimeTimeZone](datetimetimezone.md)|在指定时区的任务完成日期。|
|hasAttachments|布尔|设置为 true 如果任务的附件。|
|id|字符串|任务的唯一标识符。 只读。|
|importance|string|事件的重要性。 可取值为：`low`、`normal`、`high`。|
|isReminderOn|布尔|如果，设置为 true 设置通知提醒的用户的任务。|
|lastModifiedDateTime|DateTimeOffset|日期和上次修改任务的时间。 默认情况下，它是采用 UTC。 您可以提供请求标头中自定义时区。 该属性值使用 ISO 8601 格式，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。|
|owner|字符串|创建任务的人员的名称。|
|parentFolderId|String|任务的父文件夹的唯一标识符。|
|recurrence|[patternedRecurrence](patternedrecurrence.md)|定期模式的任务。|
|reminderDateTime|[dateTimeTimeZone](datetimetimezone.md)|发生的日期和时间的任务的提醒通知。|
|sensitivity|string|指示任务的隐私级别。 可取值为：`normal`、`personal`、`private`、`confidential`。|
|startDateTime|[dateTimeTimeZone](datetimetimezone.md)|在指定时区时的任务是开始日期。|
|status|string|指示的状态或任务进度。 可取值为：`notStarted`、`inProgress`、`completed`、`waitingOnOthers`、`deferred`。|
|subject|字符串|简要说明或任务的标题。|

## <a name="relationships"></a>Relationships
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|attachments|[附件](attachment.md) 集合|[FileAttachment](fileattachment.md)和[itemAttachment](itemattachment.md)， [referenceAttachment](referenceattachment.md)附件任务的集合。  只读。 可为 Null。|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) 集合|多值定义任务的扩展属性的集合。 只读。 可为 Null。|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection|定义任务的单值扩展属性的集合。 只读。 可为 Null。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "attachments",
    "singleValueExtendedProperties",
    "multiValueExtendedProperties"
  ],
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
<!-- {
  "type": "#page.annotation",
  "description": "outlookTask resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
