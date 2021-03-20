---
title: justifyAction 资源类型
description: 指示指定操作需要理由。
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 1db6a91987fd1345ca6a1503dfbd51e3178e9b89
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50950315"
---
# <a name="justifyaction-resource-type"></a>justifyAction 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指示指定操作需要理由。 [evaluateApplication](../api/informationprotectionlabel-evaluateApplication.md) [、evaluateClassificationResults](../api/informationprotectionlabel-evaluateClassificationResults.md)或 [evaluateRemoval](../api/informationprotectionlabel-evaluateRemoval.md) API 可能会返回 **justifyAction**。 理由通过 [labelingOptions 提供](../resources/labelingoptions.md)。 上一个调用应重复，但 **labelingOptions** 的 **downgradeJustification** 属性设置有理由消息（通过用户输入或应用程序逻辑提供）。

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

