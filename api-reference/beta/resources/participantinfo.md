---
title: participantInfo 资源类型
description: 包含有关参与者标识的其他属性
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 4cffe361b63ddc6d54d2ad16c29d2de8836044fc
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006590"
---
# <a name="participantinfo-resource-type"></a>participantInfo 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含有关参与者标识的其他属性

## <a name="properties"></a>属性

| 属性       | 类型                          | 说明  |
|:---------------|:------------------------------|:-------------|
| 窃取       | [identitySet](identityset.md) | 与此参与者关联的[了解 identityset](identityset.md) 。 |
| languageId     | String                        | 语言区域性字符串。 |
| 范围         | String                        | 参与者的地区。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "languageId", "region"
  ],
  "@odata.type": "microsoft.graph.participantInfo"
}-->
```json
{
  "identity": { "@odata.type": "#microsoft.graph.identitySet" },
  "languageId": "String",
  "region": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "participantInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
