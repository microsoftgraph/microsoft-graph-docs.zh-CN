---
title: educationOrganization 资源类型
description: 用于模型之间的教育扇区中的不同组织类型通用性抽象实体。
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: b0b65978b3b415af407c886095c4b31c7aaffab9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27831931"
---
# <a name="educationorganization-resource-type"></a>educationOrganization 资源类型

用于模型之间的教育扇区中的不同组织类型通用性抽象实体。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|说明|字符串| 组织说明。|
|displayName|字符串| 组织的显示名称。|
|externalSource|educationExternalSource| 从在其中创建此组织的源。 可能的值为： `sis`， `manual`， `unknownFutureValue`。|

## <a name="relationships"></a>Relationships
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
