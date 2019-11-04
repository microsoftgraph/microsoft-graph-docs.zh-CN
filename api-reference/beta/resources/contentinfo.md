---
title: contentInfo 资源类型
description: 表示要标记的某些信息的当前状态。
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5191be0533810f0a9da3b0ea83f209d69cc67297
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938875"
---
# <a name="contentinfo-resource-type"></a>contentInfo 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示要标记的某些信息的当前状态。 **contentInfo**将传递到[evaluateRemoval](../api/informationprotectionlabel-evaluateRemoval.md)、 [evaluateApplication](../api/informationprotectionlabel-evaluateApplication.md)和[evaluateClassificationResults](../api/informationprotectionlabel-evaluateClassificationResults.md) api，以向 API 描述信息的当前状态。 此**contentInfo**详细说明了如何在应用、更新或删除标签时添加或删除要添加或删除的元数据、内容标记和保护的结果。 

## <a name="properties"></a>属性

| 属性   | 类型                                       | 说明                                                                                                                     |
| :--------- | :----------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------ |
| format     | String                                     | 可取值为：`default`、`email`。                                                                                        |
| 标识符 | 字符串                                     | 用于 Azure 信息保护分析的标识符。                                                                     |
| metadata   | [keyValuePair](keyvaluepair.md) 集合 | 现有的 Microsoft 信息保护元数据作为键/值对进行传递，其中的键是 MSIP_Label_GUID_PropName。 |
| state      | String                                     | 可取值为：`rest`、`motion`、`use`。                                                                                   |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.contentInfo",
  "baseType": null
}-->

```json
{
  "format": "String",
  "identifier": "String",
  "metadata": [{"@odata.type": "microsoft.graph.keyValuePair"}],
  "state": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "contentInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->