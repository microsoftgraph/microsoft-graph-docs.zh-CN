---
title: retentionEventType 资源类型
description: 表示相同类型的保留事件的单个组。 事件类型是类似事件的泛型反序列化，可与任何带有基于事件的保留的标签一起使用。
author: sseth
ms.localizationpriority: medium
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 38b9ee622663d249c5f6c117b376767eb29ae232
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447583"
---
# <a name="retentioneventtype-resource-type"></a>retentionEventType 资源类型

命名空间：microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示相同类型的保留事件的单个组。

创建 [保留事件](../resources/security-retentionevent.md) 时，它与特定事件类型相关联，而该事件类型又与 [保留标签](../resources/security-retentionlabel.md)相关联。 只有应用了该保留标签的内容才会保留指定的保留期。
有关详细信息，请参阅 [事件发生时开始保留](/microsoft-365/compliance/event-driven-retention)。


## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 retentionEventTypes](../api/security-retentioneventtype-list.md)|[microsoft.graph.security.retentionEventType](../resources/security-retentioneventtype.md) 集合|获取 [retentionEventType](../resources/security-retentioneventtype.md) 对象及其属性的列表。|
|[创建 retentionEventType](../api/security-retentioneventtype-post.md)|[microsoft.graph.security.retentionEventType](../resources/security-retentioneventtype.md)|创建新的 [retentionEventType](../resources/security-retentioneventtype.md) 对象。|
|[获取 retentionEventType](../api/security-retentioneventtype-get.md)|[microsoft.graph.security.retentionEventType](../resources/security-retentioneventtype.md)|读取 [retentionEventType](../resources/security-retentioneventtype.md) 对象的属性和关系。|
|[更新 retentionEventType](../api/security-retentioneventtype-update.md)|[microsoft.graph.security.retentionEventType](../resources/security-retentioneventtype.md)|更新 [retentionEventType](../resources/security-retentioneventtype.md) 对象的属性。|
|[删除 retentionEventType](../api/security-retentioneventtype-delete.md)|无|删除 [retentionEventType](../resources/security-retentioneventtype.md) 对象。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|createdBy|[microsoft.graph.identitySet](/graph/api/resources/identityset)|创建 retentionEventType 的用户。|
|createdDateTime|DateTimeOffset|创建 retentionEventType 的日期时间。|
|description|String|有关事件类型的可选信息。|
|displayName|String|事件类型的名称。|
|id|String|表示创建 retentionEventType 的用户的唯一 ID。 [entity](/graph/api/resources/entity).|
|lastModifiedBy|[microsoft.graph.identitySet](/graph/api/resources/identityset)|上次修改 retentionEventType 的用户。|
|lastModifiedDateTime|DateTimeOffset|修改 retentionEventType 的最新日期时间。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.retentionEventType",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.retentionEventType",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)"
}
```

