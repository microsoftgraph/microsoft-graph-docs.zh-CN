---
title: institutionData 资源类型
description: institutionData 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: a528bf5bc8800b10deed2c45d84613b5ab4bd6b2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47986063"
---
# <a name="institutiondata-resource-type"></a>institutionData 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

代表用户已进行并在 [educationalActivity](educationalActivity.md) 资源中使用的 undergraduate、毕业、postgraduate 学位或其他教学活动的其他详细信息。

## <a name="properties"></a>属性

| 属性     | 类型                                 | 说明                                              |
|:-------------|:-------------------------------------|:---------------------------------------------------------|
|说明   |String                                |用户对其进行研究的机构的简短说明。 |
|displayName   |String                                |用户在其上研究的机构的名称。              |
|位置      |[physicalAddress](physicaladdress.md) |研究院的地址或位置。                     |
|webUrl        |String                                |链接到机构或部门主页。           |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.institutionData",
  "baseType": null
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "location": {"@odata.type": "microsoft.graph.physicalAddress"},
  "webUrl": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "institutionData resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

