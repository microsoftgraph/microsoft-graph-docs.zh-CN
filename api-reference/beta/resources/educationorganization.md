---
title: educationOrganization 资源类型
description: '用于对教育部门中不同组织类型之间的通用性进行建模的抽象实体。  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: ae3add0c3541e1617fec6bb71f0e05bb8fdc1b3f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016679"
---
# <a name="educationorganization-resource-type"></a>educationOrganization 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

用于对教育部门中不同组织类型之间的通用性进行建模的抽象实体。

## <a name="properties"></a>属性

| 属性       | 类型   | 说明                                                                       |
| :------------- | :----- | :-------------------------------------------------------------------------------- |
| 说明    | String | 组织说明。                                                         |
| displayName    | String | 组织显示名称。                                                        |
| externalSource | String | 创建此用户的位置。 可能的值包括： `sis` 、 `lms` 或 `manual` 。 |

## <a name="relationships"></a>关系

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


