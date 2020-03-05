---
title: participantInfo 资源类型
description: 包含有关参与者标识的其他属性
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 0316cb1bbe474f8265ed384774183759d29aca0f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447246"
---
# <a name="participantinfo-resource-type"></a>participantInfo 资源类型

命名空间： microsoft. graph

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
