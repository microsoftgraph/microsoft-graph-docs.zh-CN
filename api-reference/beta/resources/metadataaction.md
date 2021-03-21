---
title: metadataAction 资源类型
description: 表示要写入或删除文件的元数据。
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 23305d8a3e1e89d198b4700e794dd264eabf003b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960395"
---
# <a name="metadataaction-resource-type"></a>metadataAction 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示要写入或删除文件的元数据。 **metadataAction** 可能由 [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md) [、evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md)和 [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md) API 返回。 此操作会通知使用应用程序应添加到文件的特定键/值对，或应从文件中删除的特定元数据键。 此元数据描述了要标记的文件或 *信息*。

## <a name="properties"></a>属性

| 属性         | 类型                                       | 说明                                                                        |
| :--------------- | :----------------------------------------- | :--------------------------------------------------------------------------------- |
| metadataToAdd    | [keyValuePair](keyvaluepair.md) 集合 | 应添加到文件的键值对的集合。                  |
| metadataToRemove | String collection                          | 字符串的集合，用于指示要从文件元数据中删除哪些键。 |

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

