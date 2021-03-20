---
title: labelingOptions 资源类型
description: 表示可提供给评估 API 的标签选项。
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 7d2409bf538de3d37ca32cdf2fd1afb78a659817
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50950297"
---
# <a name="labelingoptions-resource-type"></a>labelingOptions 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示可提供给评估 API 的标签选项。 **labelingOptions** 必须传递到 [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md) API，以指定有关要应用的标签的详细信息。 

## <a name="properties"></a>属性

| 属性               | 类型                                                | 说明                                                                                                                   |
| :--------------------- | :-------------------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------- |
| assignmentMethod       | String                                              | 可取值为：`standard`、`privileged`、`auto`。                                                                        |
| downgradeJustification | [downgradeJustification](downgradejustification.md) | 用于指示降级是否合理以及原因（如果有）的降级理由对象。                          |
| extendedProperties     | [keyValuePair](keyvaluepair.md) 集合          | 扩展属性将在标签信息中以标准 MIP 标记元数据格式进行分析和返回。 |
| labelId                | Guid                                                | 应用于信息的标签的 GUID。                                                              |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.labelingOptions",
  "baseType": null
}-->

```json
{
  "assignmentMethod": "String",
  "downgradeJustification": {"@odata.type": "microsoft.graph.downgradeJustification"},
  "extendedProperties": [{"@odata.type": "microsoft.graph.keyValuePair"}],
  "labelId": "Guid"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "labelingOptions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

