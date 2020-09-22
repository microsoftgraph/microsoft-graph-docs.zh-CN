---
title: inferenceData 资源类型
description: inferenceData 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: profile
doc_type: resourcePageType
ms.openlocfilehash: 412d96d3eb497681e65dacd2f7a0576b4071a9aa
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016492"
---
# <a name="inferencedata-resource-type"></a>inferenceData 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[InferenceData](inferencedata.md)资源类型提供了有关通过推断用户信息创建的实体的附加详细信息。 只要特定实体中的数据是由机器学习或其他系统进程对数据进行迭代时，就会出现此信息。

## <a name="properties"></a>属性

| 属性              | 类型        | 说明                                                                     |
|:----------------------|:------------|:--------------------------------------------------------------------------------|
|confidenceScore        |双精度       | 反映有关用户推断的数据准确性的置信度分数。   |
|userHasVerifiedAccuracy|Boolean      | 如果用户已确认此推理为 True 或 False，则为记录。        |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.inferenceData",
  "baseType": null
}-->

```json
{
  "confidenceScore": 1024,
  "userHasVerifiedAccuracy": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "inferenceData resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

