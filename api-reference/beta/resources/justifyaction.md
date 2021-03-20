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
# <a name="justifyaction-resource-type"></a><span data-ttu-id="4b785-103">justifyAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="4b785-103">justifyAction resource type</span></span>

<span data-ttu-id="4b785-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4b785-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4b785-105">指示指定操作需要理由。</span><span class="sxs-lookup"><span data-stu-id="4b785-105">Indicates that a justification is required for the specified operation.</span></span> <span data-ttu-id="4b785-106">[evaluateApplication](../api/informationprotectionlabel-evaluateApplication.md) [、evaluateClassificationResults](../api/informationprotectionlabel-evaluateClassificationResults.md)或 [evaluateRemoval](../api/informationprotectionlabel-evaluateRemoval.md) API 可能会返回 **justifyAction**。</span><span class="sxs-lookup"><span data-stu-id="4b785-106">The [evaluateApplication](../api/informationprotectionlabel-evaluateApplication.md), [evaluateClassificationResults](../api/informationprotectionlabel-evaluateClassificationResults.md), or [evaluateRemoval](../api/informationprotectionlabel-evaluateRemoval.md) APIs may return **justifyAction**.</span></span> <span data-ttu-id="4b785-107">理由通过 [labelingOptions 提供](../resources/labelingoptions.md)。</span><span class="sxs-lookup"><span data-stu-id="4b785-107">Justification is provided via [labelingOptions](../resources/labelingoptions.md).</span></span> <span data-ttu-id="4b785-108">上一个调用应重复，但 **labelingOptions** 的 **downgradeJustification** 属性设置有理由消息（通过用户输入或应用程序逻辑提供）。</span><span class="sxs-lookup"><span data-stu-id="4b785-108">The previous call should be repeated, but with the **downgradeJustification** property of **labelingOptions** set with a justification message, provided via user input or application logic.</span></span>

## <a name="properties"></a><span data-ttu-id="4b785-109">属性</span><span class="sxs-lookup"><span data-stu-id="4b785-109">Properties</span></span>

<span data-ttu-id="4b785-110">无</span><span class="sxs-lookup"><span data-stu-id="4b785-110">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4b785-111">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4b785-111">JSON representation</span></span>

<span data-ttu-id="4b785-112">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4b785-112">The following is a JSON representation of the resource.</span></span>

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

