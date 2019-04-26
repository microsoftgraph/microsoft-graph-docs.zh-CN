---
title: educationOrganization 资源类型
description: '用于对教育部门中不同组织类型之间的通用性进行建模的抽象实体。  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 49afe12f4897df80ce78ba28a024883cefeb0a96
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340476"
---
# <a name="educationorganization-resource-type"></a>educationOrganization 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

用于对教育部门中不同组织类型之间的通用性进行建模的抽象实体。  

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|说明|String| 组织说明。|
|displayName|String| 组织显示名称。|
|externalSource|string| 从中创建此组织的源。 可取值为：`sis`、`manual`、`unknownFutureValue`。|

## <a name="relationships"></a>Relationships
无。


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
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
<!--
{
  "type": "#page.annotation",
  "description": "educationOrganization resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
