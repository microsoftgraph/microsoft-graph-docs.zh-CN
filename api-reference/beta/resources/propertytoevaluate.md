---
title: propertyToEvaluate 资源类型
description: 定义属性的名称和值。
localization_priority: Normal
author: yyuank
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7f6c08adc311c343699667ea3179b0b2d09a5a34
ms.sourcegitcommit: 62c900af626e46439d949462f09061cc5c41d6ff
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/16/2020
ms.locfileid: "44272846"
---
# <a name="propertytoevaluate-resource-type"></a>propertyToEvaluate 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

定义属性的名称和值。

## <a name="properties"></a>属性

| 属性 | 类型 | Description |
|:-------- |:---- |:----------- |
| propertyName | String | 提供属性名称。 |
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