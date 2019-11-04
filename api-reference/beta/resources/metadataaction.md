---
title: metadataAction 资源类型
description: 表示要写入或从文件中移除的元数据。
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8652a33de04d0a28a34c3738dd1706d6aff5e5b9
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938903"
---
# <a name="metadataaction-resource-type"></a>metadataAction 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示要写入或从文件中移除的元数据。 **metadataAction**可能由[evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md)、 [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md)和[evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md) api 返回。 该操作通知使用应用程序应添加到文件中的特定键/值对，或应从文件中删除的特定元数据密钥。 此元数据是描述要*标记*的文件或信息的内容。

## <a name="properties"></a>属性

| 属性         | 类型                                       | 描述                                                                        |
| :--------------- | :----------------------------------------- | :--------------------------------------------------------------------------------- |
| metadataToAdd    | [keyValuePair](keyvaluepair.md) 集合 | 应添加到文件中的键值对的集合。                  |
| metadataToRemove | String collection                          | 字符串的集合，用于指示要从文件元数据中删除的键。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.metadataAction",
  "baseType": "microsoft.graph.informationProtectionAction"
}-->

```json
{
  "metadataToAdd": [{"@odata.type": "microsoft.graph.keyValuePair"}],
  "metadataToRemove": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "metadataAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->