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
# <a name="justifyaction-resource-type"></a><span data-ttu-id="89320-103">justifyAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="89320-103">justifyAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="89320-104">指示指定的操作需要理由。</span><span class="sxs-lookup"><span data-stu-id="89320-104">Indicates that a justification is required for the specified operation.</span></span> <span data-ttu-id="89320-105">[EvaluateApplication](../api/informationprotectionlabel-evaluateApplication.md)、 [evaluateClassificationResults](../api/informationprotectionlabel-evaluateClassificationResults.md)或[evaluateRemoval](../api/informationprotectionlabel-evaluateRemoval.md) api 可能返回**justifyAction**。</span><span class="sxs-lookup"><span data-stu-id="89320-105">The [evaluateApplication](../api/informationprotectionlabel-evaluateApplication.md), [evaluateClassificationResults](../api/informationprotectionlabel-evaluateClassificationResults.md), or [evaluateRemoval](../api/informationprotectionlabel-evaluateRemoval.md) APIs may return **justifyAction**.</span></span> <span data-ttu-id="89320-106">理由通过[labelingOptions](../resources/labelingoptions.md)提供。</span><span class="sxs-lookup"><span data-stu-id="89320-106">Justification is provided via [labelingOptions](../resources/labelingoptions.md).</span></span> <span data-ttu-id="89320-107">前一个调用应重复出现，但通过用户输入或应用程序逻辑提供的**downgradeJustification**属性为**labelingOptions**设置的理由消息。</span><span class="sxs-lookup"><span data-stu-id="89320-107">The previous call should be repeated, but with the **downgradeJustification** property of **labelingOptions** set with a justification message, provided via user input or application logic.</span></span>

## <a name="properties"></a><span data-ttu-id="89320-108">属性</span><span class="sxs-lookup"><span data-stu-id="89320-108">Properties</span></span>

<span data-ttu-id="89320-109">无</span><span class="sxs-lookup"><span data-stu-id="89320-109">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="89320-110">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="89320-110">JSON representation</span></span>

<span data-ttu-id="89320-111">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="89320-111">The following is a JSON representation of the resource.</span></span>

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