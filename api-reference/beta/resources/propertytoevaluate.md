---
title: propertyToEvaluate 资源类型
description: 定义属性的名称和值。
ms.localizationpriority: medium
author: psaffaie
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 84481eeff8ed1367e85d4000ffe1b60fb5116ad2
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2022
ms.locfileid: "64587061"
---
# <a name="propertytoevaluate-resource-type"></a>propertyToEvaluate 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

定义属性的名称和值。

## <a name="properties"></a>属性

| 属性      | 类型   | 说明                  |
| :------------ | :----- | :--------------------------- |
| PropertyName  | String | 提供属性名称。  |
| propertyValue | String | 提供属性值。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.propertyToEvaluate",
  "baseType": null
}-->

```json
{
  "propertyName": "String",
  "propertyValue": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "propertyToEvaluate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
