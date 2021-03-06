---
title: serviceUpdateMessage 资源类型
description: 表示服务中的更改通知。
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: e8bea9b3c44f99d5be0d87b01d47db4505873681
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2021
ms.locfileid: "53109093"
---
# <a name="serviceupdatemessage-resource-type"></a>serviceUpdateMessage 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示有关服务中更改的公告。

表示公告，如产品的主要更新、新功能;例如，发布新的Windows功能。

继承自 [serviceAnnouncementBase](../resources/serviceannouncementbase.md)。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 serviceUpdateMessage](../api/serviceupdatemessage-get.md)|[serviceUpdateMessage](../resources/serviceupdatemessage.md)|检索 [serviceUpdateMessage 对象的属性和](../resources/serviceupdatemessage.md) 关系。 |
|[markRead](../api/serviceupdatemessage-markread.md)|布尔值|将 [serviceUpdateMessage](../resources/serviceupdatemessage.md)的列表标记为 **已** 登录用户的已读。|
|[markUnread](../api/serviceupdatemessage-markunread.md)|布尔值|对于登录用户，将 [serviceUpdateMessage](../resources/serviceupdatemessage.md)**列表标记为未** 读。|
|[archive](../api/serviceupdatemessage-archive.md)|布尔值|存档已登录 [用户的 serviceUpdateMessage](../resources/serviceupdatemessage.md)列表。|
|[unarchive](../api/serviceupdatemessage-unarchive.md)|布尔值|取消存档已登录用户的 [serviceUpdateMessage](../resources/serviceupdatemessage.md)列表。|
|[favorite](../api/serviceupdatemessage-favorite.md)|布尔值|将 [serviceUpdateMessage](../resources/serviceupdatemessage.md)列表的状态更改为为登录用户收藏。|
|[unfavorite](../api/serviceupdatemessage-unfavorite.md)|布尔值|删除已登录用户的 [serviceUpdateMessage](../resources/serviceupdatemessage.md)的收藏夹状态。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|actionRequiredByDateTime|DateTimeOffset|邮件操作的预期截止时间。|
|body|[itemBody](../resources/itembody.md)|服务邮件正文的内容类型和内容。|
|“类别”|serviceUpdateCategory|服务邮件类别。 可取值为：`preventOrFixIssue`、`planForChange`、`stayInformed`、`unknownFutureValue`。|
|详细信息|collection ([keyValuePair](../resources/keyvaluepair.md)) |有关服务邮件的其他详细信息。 此属性不支持筛选器。 继承自 [serviceAnnouncementBase](../resources/serviceannouncementbase.md)。|
|endDateTime|DateTimeOffset|服务消息的结束时间。 继承自 [serviceAnnouncementBase](../resources/serviceannouncementbase.md)。|
|id|字符串|服务消息的 ID。 继承自 [serviceAnnouncementBase](../resources/serviceannouncementbase.md)。|
|isMajorChange|布尔值|指示消息是否描述服务的主要更新。|
|lastModifiedDateTime|DateTimeOffset|服务邮件的上次修改时间。 继承自 [serviceAnnouncementBase](../resources/serviceannouncementbase.md)。|
|服务|集合 (字符串) |服务消息影响的服务。|
|severity|serviceUpdateSeverity|服务邮件的严重性。 可取值为：`normal`、`high`、`critical`、`unknownFutureValue`。|
|startDateTime|DateTimeOffset|服务消息的开始时间。 继承自 [serviceAnnouncementBase](../resources/serviceannouncementbase.md)。|
|标记|集合 (字符串) |服务邮件的标记集合。|
|title|String|服务消息的标题。 继承自 [serviceAnnouncementBase](../resources/serviceannouncementbase.md)。|
|viewPoint|[serviceUpdateMessageViewpoint](../resources/serviceupdatemessageviewpoint.md)|表示服务消息的用户视图点数据。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.serviceUpdateMessage",
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
  }
}
```

