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
# <a name="justifyaction-resource-type"></a><span data-ttu-id="9d013-103">justifyAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="9d013-103">justifyAction resource type</span></span>

<span data-ttu-id="9d013-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d013-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9d013-105">指示指定的操作需要理由。</span><span class="sxs-lookup"><span data-stu-id="9d013-105">Indicates that a justification is required for the specified operation.</span></span> <span data-ttu-id="9d013-106">[EvaluateApplication](../api/informationprotectionlabel-evaluateApplication.md)、 [evaluateClassificationResults](../api/informationprotectionlabel-evaluateClassificationResults.md)或[evaluateRemoval](../api/informationprotectionlabel-evaluateRemoval.md) api 可能返回**justifyAction**。</span><span class="sxs-lookup"><span data-stu-id="9d013-106">The [evaluateApplication](../api/informationprotectionlabel-evaluateApplication.md), [evaluateClassificationResults](../api/informationprotectionlabel-evaluateClassificationResults.md), or [evaluateRemoval](../api/informationprotectionlabel-evaluateRemoval.md) APIs may return **justifyAction**.</span></span> <span data-ttu-id="9d013-107">理由通过 [labelingOptions](../resources/labelingoptions.md)提供。</span><span class="sxs-lookup"><span data-stu-id="9d013-107">Justification is provided via [labelingOptions](../resources/labelingoptions.md).</span></span> <span data-ttu-id="9d013-108">前一个调用应重复出现，但通过用户输入或应用程序逻辑提供的 **downgradeJustification** 属性为 **labelingOptions** 设置的理由消息。</span><span class="sxs-lookup"><span data-stu-id="9d013-108">The previous call should be repeated, but with the **downgradeJustification** property of **labelingOptions** set with a justification message, provided via user input or application logic.</span></span>

## <a name="properties"></a><span data-ttu-id="9d013-109">属性</span><span class="sxs-lookup"><span data-stu-id="9d013-109">Properties</span></span>

<span data-ttu-id="9d013-110">无</span><span class="sxs-lookup"><span data-stu-id="9d013-110">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9d013-111">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9d013-111">JSON representation</span></span>

<span data-ttu-id="9d013-112">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9d013-112">The following is a JSON representation of the resource.</span></span>

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

