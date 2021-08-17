---
title: serviceAnnouncementBase 资源类型
description: 这是 serviceHealthIssue 和 serviceUpdateMessage 的抽象基类型。
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: f5f1beb5918833703fbbff48ba991b850bcd1ceb
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58266903"
---
# <a name="serviceannouncementbase-resource-type"></a>serviceAnnouncementBase 资源类型

命名空间：microsoft.graph

这是 [serviceHealthIssue](../resources/servicehealthissue.md) 和 [serviceUpdateMessage](../resources/serviceupdatemessage.md)的抽象基类型。

继承自 [实体](../resources/entity.md)。

## <a name="methods"></a>方法
无。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|详细信息|集合 ([keyValuePair](../resources/keyvaluepair.md)) |有关服务事件的其他详细信息。 此属性不支持筛选器。|
|endDateTime|DateTimeOffset|服务事件的结束时间。|
|id|String|服务事件的 ID。|
|lastModifiedDateTime|DateTimeOffset|服务事件的上次修改时间。|
|startDateTime|DateTimeOffset|服务事件的开始时间。|
|title|String|服务事件的标题。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.serviceAnnouncementBase",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.serviceAnnouncementBase",
  "id": "String (identifier)",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "title": "String",
  "details": [
    {
      "@odata.type": "microsoft.graph.keyValuePair"
    }
  ]
}
```