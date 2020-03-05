---
title: labelingOptions 资源类型
description: 表示可提供给评估 Api 的标记选项。
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 97557ad6e233506e5e074c408ffb04f83297f0af
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523000"
---
# <a name="labelingoptions-resource-type"></a>labelingOptions 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示可提供给评估 Api 的标记选项。 **labelingOptions**必须传递到[evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md) API，以指定要应用的标签的详细信息。 

## <a name="properties"></a>属性

| 属性               | 类型                                                | 说明                                                                                                                   |
| :--------------------- | :-------------------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------- |
| assignmentMethod       | String                                              | 可取值为：`standard`、`privileged`、`auto`。                                                                        |
| downgradeJustification | [downgradeJustification](downgradejustification.md) | 降级理由对象，该对象指示降级是否已两端对齐，如果是，则指示原因。                          |
| extendedProperties     | [keyValuePair](keyvaluepair.md) 集合          | 扩展属性将在作为标签信息一部分的标准 MIP 标记元数据格式中进行分析和返回。 |
| labelId                | Guid                                                | 应应用于信息的标签的 GUID。                                                              |

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