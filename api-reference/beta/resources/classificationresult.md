---
title: classificationResult 资源类型
description: 表示分类请求的结果。
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 5ecc16197ef4671c6e83883bc69aed45b3ffa200
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50941818"
---
# <a name="classificationresult-resource-type"></a>classificationResult 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示来自 Microsoft 分类引擎的分类操作的结果。 来自 Azure 信息保护、Office 和其他 Microsoft 服务的数据分类结果可能会返回一组明确定义的 [分类类型](/office365/securitycompliance/what-the-sensitive-information-types-look-for)。 可以将这些类型提供给 [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md) API，以将敏感信息解析为 Microsoft 信息保护标签。 

## <a name="properties"></a>属性

| 属性        | 类型  | 说明                                                            |
| :-------------- | :---- | :--------------------------------------------------------------------- |
| confidenceLevel | Int32 | 结果的可信度 0 到 100。                         |
| count           | Int32 | 输入中特定信息类型的实例数。 |
| sensitiveTypeId | GUID  | 发现的敏感信息类型的 GUID。                 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.classificationResult",
  "baseType": null
}-->

```json
{
  "confidenceLevel": 1024,
  "count": 1024,
  "sensitiveTypeId": "Guid"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "classificationResult resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->