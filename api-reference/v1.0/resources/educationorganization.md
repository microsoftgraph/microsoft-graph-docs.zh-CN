---
title: educationOrganization 资源类型
description: 用于对教育部门中不同组织类型之间的通用性进行建模的抽象实体。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: b4f00fc4c44b3019dccbded1fd222aa211d78c7a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48032675"
---
# <a name="educationorganization-resource-type"></a>educationOrganization 资源类型

命名空间：microsoft.graph

用于对教育部门中不同组织类型之间的通用性进行建模的抽象实体。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|说明|String| 组织说明。|
|displayName|String| 组织显示名称。|
|externalSource|educationExternalSource| 从中创建此组织的源。 可能的值包括 `sis`、`manual`、`unknownFutureValue`。|

## <a name="relationships"></a>关系
无。


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "abstract": true,
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationOrganization"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "externalSource": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationOrganization resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

