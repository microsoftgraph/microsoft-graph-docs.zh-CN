---
title: innerErrorDetail 资源类型
description: 包含在 errorDetail 对象中的内部错误。
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 5a5b85f17b87343766a4edb00c6d620c185ecaf5
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939654"
---
# <a name="innererrordetail-resource-type"></a>innerErrorDetail 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含在[errorDetail](errordetail.md)对象中的内部错误。

## <a name="properties"></a>属性

| 属性 | 类型   | 描述                                  |
|:---------|:-------|:---------------------------------------------|
| message  | String | 人类可读错误消息。 只读。 |
| source   | 字符串 | 错误的来源。 只读。          |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.innerErrorDetail",
  "baseType": null
}-->

```json
{
  "message": "String",
  "source": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "innerErrorDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
