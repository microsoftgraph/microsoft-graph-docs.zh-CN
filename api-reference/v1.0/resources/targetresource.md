---
title: targetResource 资源类型
description: 表示与审核活动相关联的目标资源类型。
localization_priority: Normal
author: dhanyahk
ms.prod: azure-ad
doc_type: resourcePageType
ms.openlocfilehash: 641097b6e8b4646d878182ba1763fd62ab75b080
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48094055"
---
# <a name="targetresource-resource-type"></a>targetResource 资源类型

命名空间：microsoft.graph

表示与审核活动相关联的目标资源类型。 

## <a name="properties"></a>属性

| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|String|指示资源的唯一 ID。|
|displayName|String|指示为资源定义的可见名称。 通常是在创建资源时指定的。|
|type|String|描述资源类型。  示例值包括 `Application` 、 `Group` 、 `ServicePrincipal` 和 `User` 。|
|userPrincipalName|String|当 " **类型** " 设置为时 `User` ，其中包括启动操作的用户名; `null` 针对其他类型。|
|groupType|String|当 " **类型** " 设置为时 `Group` ，这表示组类型。|
|ModifiedProperties|[modifiedProperty](modifiedproperty.md) 集合|指示已更改的每个属性的名称、旧值和新值。 属性值取决于操作 **类型**。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.targetResource"
}-->

```json
{
  "id": "String",
  "displayName": "String",
  "type": "String",
  "userPrincipalName": "String",
  "groupType": "String",
  "modifiedProperties": [{"@odata.type": "microsoft.graph.modifiedProperty"}]
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "targetResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

