---
title: serviceUpdateMessage 资源类型
description: 表示服务中的更改通知。
author: payiAzure
ms.localizationpriority: medium
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: 81d3524855daf6138baa61388b9d853faefec5f6
ms.sourcegitcommit: 15956da1b4a7d523363ffa8afb5e2059fbf680ce
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/01/2022
ms.locfileid: "62291244"
---
# <a name="serviceupdatemessage-resource-type"></a>serviceUpdateMessage 资源类型

命名空间：microsoft.graph

表示有关服务中更改的公告。

表示公告，如产品的主要更新、新功能;例如，发布新的SharePoint功能。

继承自 [serviceAnnouncementBase](../resources/serviceannouncementbase.md)。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 serviceUpdateMessage](../api/serviceupdatemessage-get.md)|[serviceUpdateMessage](../resources/serviceupdatemessage.md)|检索 [serviceUpdateMessage 对象的属性和](../resources/serviceupdatemessage.md) 关系。 |
|[markRead](../api/serviceupdatemessage-markread.md)|Boolean|将 [serviceUpdateMessages](../resources/serviceupdatemessage.md) 列表标记为 **已** 登录用户的已读。|
|[markUnread](../api/serviceupdatemessage-markunread.md)|Boolean|将 [serviceUpdateMessages](../resources/serviceupdatemessage.md) 列表标记为 **登录** 用户未读。|
|[archive](../api/serviceupdatemessage-archive.md)|Boolean|存档已登录 [用户的 serviceUpdateMessages](../resources/serviceupdatemessage.md) 列表。|
|[unarchive](../api/serviceupdatemessage-unarchive.md)|Boolean|取消存档已登录 [用户的 serviceUpdateMessages](../resources/serviceupdatemessage.md) 列表。|
|[favorite](../api/serviceupdatemessage-favorite.md)|Boolean|将 [serviceUpdateMessages](../resources/serviceupdatemessage.md) 列表的状态更改为为登录用户收藏。|
|[unfavorite](../api/serviceupdatemessage-unfavorite.md)|Boolean|删除已登录 [用户的 serviceUpdateMessages](../resources/serviceupdatemessage.md) 的收藏夹状态。|
|[列出附件](../api/serviceupdatemessage-list-attachments.md)|[serviceAnnouncementAttachment](../resources/serviceannouncementattachment.md) 集合|获取与服务邮件关联的附件列表。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|actionRequiredByDateTime|DateTimeOffset|邮件操作的预期截止时间。|
|attachmentsArchive|Stream|包含邮件的所有附件的 zip 文件。|
|body|[itemBody](../resources/itembody.md)|服务邮件正文的内容类型和内容。|
|“类别”|serviceUpdateCategory|服务邮件类别。 可能的值是：`preventOrFixIssue`、`planForChange`、`stayInformed`、`unknownFutureValue`。|
|详细信息|collection ([keyValuePair](../resources/keyvaluepair.md)) |有关服务邮件的其他详细信息。 此属性不支持筛选器。 继承自 [serviceAnnouncementBase](../resources/serviceannouncementbase.md)。|
|endDateTime|DateTimeOffset|服务消息的结束时间。 继承自 [serviceAnnouncementBase](../resources/serviceannouncementbase.md)。|
|hasAttachments|Boolean|指示邮件是否包含任何附件。|
|id|String|服务消息的 ID。 继承自 [serviceAnnouncementBase](../resources/serviceannouncementbase.md)。|
|isMajorChange|Boolean|指示消息是否描述服务的主要更新。|
|lastModifiedDateTime|DateTimeOffset|服务邮件的上次修改时间。 继承自 [serviceAnnouncementBase](../resources/serviceannouncementbase.md)。|
|服务|集合 (字符串) |服务消息影响的服务。|
|severity|serviceUpdateSeverity|服务邮件的严重性。 可取值为：`normal`、`high`、`critical`、`unknownFutureValue`。|
|startDateTime|DateTimeOffset|服务消息的开始时间。 继承自 [serviceAnnouncementBase](../resources/serviceannouncementbase.md)。|
|标记|集合 (字符串) |服务邮件的标记集合。 标签由发布消息的服务团队/支持团队提供，用于判断此邮件是否包含隐私数据，或此消息是否用于服务新功能更新等。|
|title|String|服务消息的标题。 继承自 [serviceAnnouncementBase](../resources/serviceannouncementbase.md)。|
|viewPoint|[serviceUpdateMessageViewpoint](../resources/serviceupdatemessageviewpoint.md)|表示用户对服务消息的数据进行观察。 此数据包括邮件状态，例如用户是否已存档、阅读或将邮件标记为收藏夹。 使用应用程序权限访问此属性时，此属性为 null。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|attachments|collection ([serviceAnnouncementAttachment](../resources/serviceannouncementattachment.md)) |[serviceAnnouncementAttachments 的集合](../resources/serviceannouncementattachment.md)。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.serviceUpdateMessage",
  "baseType": "microsoft.graph.serviceAnnouncementBase",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.serviceUpdateMessage",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "title": "String",
  "details": [
    {
      "@odata.type": "microsoft.graph.keyValuePair"
    }
  ],
  "id": "String (identifier)",
  "body": {
    "@odata.type": "microsoft.graph.itemBody"
  },
  "category": "String",
  "severity": "String",
  "tags": [
    "String"
  ],
  "isMajorChange": "Boolean",
  "actionRequiredByDateTime": "String (timestamp)",
  "services": [
    "String"
  ],
  "viewPoint": {
    "@odata.type": "microsoft.graph.serviceUpdateMessageViewpoint"
  },
  "hasAttachments": "Boolean",
  "attachmentsArchive": "Stream"
}
```

