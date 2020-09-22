---
title: targetResource 资源复杂类型-Microsoft Graph API
description: 定义支持 (租户) 活动的审核日志报告组织的 Microsoft Graph API 的 targetResource 实体资源复杂类型。
author: cloudhandler
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
ms.openlocfilehash: bec25af7e0f39a4adf15577c21d4141e1a3c431a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47985648"
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


