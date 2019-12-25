---
title: participantInfo 资源类型
description: 包含有关参与者标识的其他属性
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 1dcc164769c2e8168be5f593c35cd62218254add
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871065"
---
# <a name="participantinfo-resource-type"></a>participantInfo 资源类型

包含有关参与者标识的其他属性

## <a name="properties"></a>属性

| 属性       | 类型                          | 说明                                                                                                                                                |
|:---------------|:------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------|
| 窃取       | [identitySet](identityset.md) | 与此参与者关联的[了解 identityset](identityset.md) 。 只读。                                                                             |
| languageId     | String                        | 语言区域性字符串。 只读。                                                                                                                    |
| 范围         | String                        | 参与者的家乡区域。 它可以是国家/地区、一个洲或更大的地理区域。 这不会根据参与者的当前物理位置而更改。 只读。 |


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "languageId",
    "region"
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
