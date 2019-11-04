---
title: removeWatermarkAction 资源类型
description: 表示一个操作，该操作指定要从信息中删除的内容水印的详细信息（如果适用）。
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 34859dedd5e5e740aa776cdf78bb742399523fa2
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939269"
---
# <a name="removewatermarkaction-resource-type"></a><span data-ttu-id="70c38-103">removeWatermarkAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="70c38-103">removeWatermarkAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="70c38-104">表示一个操作，该操作指定要从信息中删除的内容水印的详细信息（如果适用）。</span><span class="sxs-lookup"><span data-stu-id="70c38-104">Represents an action that specifies the details on the content watermark to be removed from the information, if applicable.</span></span> <span data-ttu-id="70c38-105">如果由于更新或删除标签而要删除水印， [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md)、 [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md)或[EvaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md) api 可能会返回**removeWatermarkAction** 。</span><span class="sxs-lookup"><span data-stu-id="70c38-105">The [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md), [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md), or [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md) APIs may return the **removeWatermarkAction** if the watermark is to be removed as a result of updating or removing the label.</span></span> <span data-ttu-id="70c38-106">该操作指示使用应用程序移除包含之前适用的内容水印的特定 UI 元素。</span><span class="sxs-lookup"><span data-stu-id="70c38-106">The action instructs the consuming application to remove the specific UI element that contains the previously-applicable content watermark.</span></span>

## <a name="properties"></a><span data-ttu-id="70c38-107">属性</span><span class="sxs-lookup"><span data-stu-id="70c38-107">Properties</span></span>

| <span data-ttu-id="70c38-108">属性</span><span class="sxs-lookup"><span data-stu-id="70c38-108">Property</span></span>       | <span data-ttu-id="70c38-109">类型</span><span class="sxs-lookup"><span data-stu-id="70c38-109">Type</span></span>              | <span data-ttu-id="70c38-110">描述</span><span class="sxs-lookup"><span data-stu-id="70c38-110">Description</span></span>                           |
| :------------- | :---------------- | :------------------------------------ |
| <span data-ttu-id="70c38-111">uiElementNames</span><span class="sxs-lookup"><span data-stu-id="70c38-111">uiElementNames</span></span> | <span data-ttu-id="70c38-112">String collection</span><span class="sxs-lookup"><span data-stu-id="70c38-112">String collection</span></span> | <span data-ttu-id="70c38-113">要删除的页脚的 UI 元素的名称。</span><span class="sxs-lookup"><span data-stu-id="70c38-113">The name of the UI element of footer to be removed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="70c38-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="70c38-114">JSON representation</span></span>

<span data-ttu-id="70c38-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="70c38-115">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.removeWatermarkAction",
  "baseType": "microsoft.graph.informationProtectionAction"
}-->

```json
{
  "uiElementNames": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "removeWatermarkAction resource",
  "keywords": "",  
  "section": "documentation",
  "tocPath": ""
}-->