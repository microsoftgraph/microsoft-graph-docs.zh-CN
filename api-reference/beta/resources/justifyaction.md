---
title: justifyAction 资源类型
description: 指示指定的操作需要理由。
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: bc96062febc15310de6a3b2ed04f96a8cf1e69e5
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939311"
---
# <a name="justifyaction-resource-type"></a>justifyAction 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指示指定的操作需要理由。 [EvaluateApplication](../api/informationprotectionlabel-evaluateApplication.md)、 [evaluateClassificationResults](../api/informationprotectionlabel-evaluateClassificationResults.md)或[evaluateRemoval](../api/informationprotectionlabel-evaluateRemoval.md) api 可能返回**justifyAction**。 理由通过[labelingOptions](../resources/labelingoptions.md)提供。 前一个调用应重复出现，但通过用户输入或应用程序逻辑提供的**downgradeJustification**属性为**labelingOptions**设置的理由消息。

## <a name="properties"></a>属性

无

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.justifyAction",
  "baseType": "microsoft.graph.informationProtectionAction"
}-->

```json
{
  
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "justifyAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->