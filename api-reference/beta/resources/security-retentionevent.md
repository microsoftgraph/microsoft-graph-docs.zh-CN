---
title: retentionEvent 资源类型
description: 表示基于事件的保留标签的触发器，其中保留期的开始基于发生特定类型的事件的时间。
author: sseth
ms.localizationpriority: medium
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: f44ac532720497888a151776b823884a11782009
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447509"
---
# <a name="retentionevent-resource-type"></a>retentionEvent 资源类型

命名空间：microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示基于事件的保留标签的触发器，其中保留期的开始基于发生特定类型的事件的时间。
若要了解有关它的详细信息，请参阅 [事件发生时开始保留](/microsoft-365/compliance/event-driven-retention)。


## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 retentionEvents](../api/security-retentionevent-list.md)|[microsoft.graph.security.retentionEvent](../resources/security-retentionevent.md) 集合|获取 [retentionEvent](../resources/security-retentionevent.md) 对象及其属性的列表。|
|[创建 retentionEvent](../api/security-retentionevent-post.md)|[microsoft.graph.security.retentionEvent](../resources/security-retentionevent.md)|创建新的 [retentionEvent](../resources/security-retentionevent.md) 对象。|
|[获取 retentionEvent](../api/security-retentionevent-get.md)|[microsoft.graph.security.retentionEvent](../resources/security-retentionevent.md)|读取 [retentionEvent](../resources/security-retentionevent.md) 对象的属性和关系。|
|[删除 retentionEvent](../api/security-retentionevent-delete.md)|无|删除 [retentionEvent](../resources/security-retentionevent.md) 对象。|
|[列出 retentionEventType](../api/security-retentioneventtype-list.md)|[microsoft.graph.security.retentionEventType](../resources/security-retentioneventtype.md) 集合|从 exapnd eventType 导航属性获取 retentionEventType 资源。|
|[创建 retentionEventType](../api/security-retentioneventtype-post.md)|[microsoft.graph.security.retentionEventType](../resources/security-retentioneventtype.md)|通过在创建事件时添加相关的 odata 属性来添加 eventType。|


## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|createdBy|[microsoft.graph.identitySet](/graph/api/resources/identityset)|创建 retentionEvent 的用户。|
|createdDateTime|DateTimeOffset|创建 retentionEvent 的日期时间。|
|description|String|有关事件的可选信息。|
|displayName|String|事件的名称。|
|eventPropagationResult|[microsoft.graph.security.eventPropagationResult](../resources/security-eventpropagationresult.md)|表示已创建事件的成功状态和其他信息。|
|eventQueries|[microsoft.graph.security.eventQueries](../resources/security-eventqueries.md) 集合| 表示与保留事件关联的工作负荷 (SharePoint Online、OneDrive for Business、Exchange Online) 和标识信息。|
|retentionEventStatus|[microsoft.graph.security.retentionEventStatus](../resources/security-retentioneventstatus.md) 集合|创建事件后，向作用域内位置显示事件的状态。|
|eventTriggerDateTime|DateTimeOffset|应触发事件的可选时间。|
|id|String|表示创建 retentionEvent 的用户的唯一 ID。 [entity](/graph/api/resources/entity).|
|lastModifiedBy|[microsoft.graph.identitySet](/graph/api/resources/identityset)|上次修改 retentionEvent 的用户。|
|lastModifiedDateTime|DateTimeOffset|修改 retentionEvent 的最新日期时间。|
|lastStatusUpdateDateTime|DateTimeOffset|上次更新事件状态时。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|retentionEventType|[microsoft.graph.security.retentionEventType](../resources/security-retentioneventtype.md)|指定将在创建事件时为使用此事件类型的标签启动保留期的事件。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.retentionEvent",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.retentionEvent",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "eventQueries": [
    {
      "@odata.type": "microsoft.graph.security.eventQueries"
    }
  ],
  "eventTriggerDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "eventPropagationResults": [
    {
      "@odata.type": "microsoft.graph.security.eventPropagationResult"
    }
  ],
  "eventStatus": {
    "@odata.type": "microsoft.graph.security.retentionEventStatus"
  },
  "lastStatusUpdateDateTime": "String (timestamp)"
}
```