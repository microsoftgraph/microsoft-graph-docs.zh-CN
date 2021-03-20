---
title: protectDoNotForwardAction 资源类型
description: 通知应用程序应用"不要转发"保护。
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: a68771ea278ba8a904c032a86732b2b190eeeb43
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50941769"
---
# <a name="protectdonotforwardaction-resource-type"></a>protectDoNotForwardAction 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

通知应用程序应用"不要转发"保护。 **protectionDoNotForwardAction** 可能由 [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md) 或 [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md) 返回（如果结果标签已配置为应用 Do [Not Forward 保护](/azure/information-protection/configure-usage-rights#do-not-forward-option-for-emails)）。 使用应用程序必须使用客户端库通过 Azure 信息保护应用保护。

## <a name="properties"></a>属性

无

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.protectDoNotForwardAction",
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
  "description": "protectDoNotForwardAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->