---
title: remove使用markAction 资源类型
description: 表示一个操作，指定要从信息中删除的内容水印的详细信息（如果适用）。
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 2a2365b2c9bc1080db9b6bf58b2035d88832881a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960353"
---
# <a name="removewatermarkaction-resource-type"></a><span data-ttu-id="8e6e5-103">remove使用markAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="8e6e5-103">removeWatermarkAction resource type</span></span>

<span data-ttu-id="8e6e5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8e6e5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8e6e5-105">表示一个操作，指定要从信息中删除的内容水印的详细信息（如果适用）。</span><span class="sxs-lookup"><span data-stu-id="8e6e5-105">Represents an action that specifies the details on the content watermark to be removed from the information, if applicable.</span></span> <span data-ttu-id="8e6e5-106">如果由于更新或删除标签而删除水印，则 evaluateApplication、evaluateClassificationResults 或 [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md) API 可能会返回 [](../api/informationprotectionlabel-evaluateapplication.md)[](../api/informationprotectionlabel-evaluateclassificationresults.md)**removeIngmarkAction。**</span><span class="sxs-lookup"><span data-stu-id="8e6e5-106">The [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md), [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md), or [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md) APIs may return the **removeWatermarkAction** if the watermark is to be removed as a result of updating or removing the label.</span></span> <span data-ttu-id="8e6e5-107">此操作指示使用应用程序删除包含以前适用的内容水印的特定 UI 元素。</span><span class="sxs-lookup"><span data-stu-id="8e6e5-107">The action instructs the consuming application to remove the specific UI element that contains the previously-applicable content watermark.</span></span>

## <a name="properties"></a><span data-ttu-id="8e6e5-108">属性</span><span class="sxs-lookup"><span data-stu-id="8e6e5-108">Properties</span></span>

| <span data-ttu-id="8e6e5-109">属性</span><span class="sxs-lookup"><span data-stu-id="8e6e5-109">Property</span></span>       | <span data-ttu-id="8e6e5-110">类型</span><span class="sxs-lookup"><span data-stu-id="8e6e5-110">Type</span></span>              | <span data-ttu-id="8e6e5-111">说明</span><span class="sxs-lookup"><span data-stu-id="8e6e5-111">Description</span></span>                           |
| :------------- | :---------------- | :------------------------------------ |
| <span data-ttu-id="8e6e5-112">uiElementNames</span><span class="sxs-lookup"><span data-stu-id="8e6e5-112">uiElementNames</span></span> | <span data-ttu-id="8e6e5-113">String collection</span><span class="sxs-lookup"><span data-stu-id="8e6e5-113">String collection</span></span> | <span data-ttu-id="8e6e5-114">要删除的页脚的 UI 元素的名称。</span><span class="sxs-lookup"><span data-stu-id="8e6e5-114">The name of the UI element of footer to be removed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8e6e5-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8e6e5-115">JSON representation</span></span>

<span data-ttu-id="8e6e5-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8e6e5-116">The following is a JSON representation of the resource.</span></span>

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

