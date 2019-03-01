---
title: targetResource 资源复杂类型-Microsoft Graph API
description: 定义支持审核日志报告组织 (租户) 活动的 Microsoft Graph API 的 targetResource 实体资源复杂类型。
author: lleonard-msft
localization_priority: Normal
ms.prod: azure-ad
ms.openlocfilehash: a03ca03e0b7105c8f07347f6ed52aa322a6fd090
ms.sourcegitcommit: e8b488f8068845522b869bf97475da7b078bee3d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/01/2019
ms.locfileid: "30342287"
---
# <a name="targetresource-resource-type"></a>targetResource 资源类型

表示与审核活动相关联的目标资源类型。 


## <a name="properties"></a>属性

| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|字符串|指示资源的唯一 ID。|
|displayName|String|指示为资源定义的可见名称。 通常是在创建资源时指定的。|
|type|字符串|描述资源类型。  示例值包括`Application`、 `Group`、 `ServicePrincipal`和`User`。|
|userPrincipalName|String|当 "**类型**" 设置`User`为时, 这包括启动操作的用户名;`null`对于其他类型。|
|groupType|String|当 "**类型**" 设置`Group`为时, 这表示组类型。|
|ModifiedProperties|[modifiedProperty](modifiedproperty.md)集合|指示已更改的每个属性的名称、旧值和新值。 属性值取决于操作**类型**。|

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
