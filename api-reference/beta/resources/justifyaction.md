---
title: justifyAction 资源类型
description: 指示指定的操作需要理由。
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9e26cd675ecb1a3a50c505c019244c60eaee88c0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48039354"
---
# <a name="justifyaction-resource-type"></a>justifyAction 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指示指定的操作需要理由。 [EvaluateApplication](../api/informationprotectionlabel-evaluateApplication.md)、 [evaluateClassificationResults](../api/informationprotectionlabel-evaluateClassificationResults.md)或[evaluateRemoval](../api/informationprotectionlabel-evaluateRemoval.md) api 可能返回**justifyAction**。 理由通过 [labelingOptions](../resources/labelingoptions.md)提供。 前一个调用应重复出现，但通过用户输入或应用程序逻辑提供的 **downgradeJustification** 属性为 **labelingOptions** 设置的理由消息。

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

