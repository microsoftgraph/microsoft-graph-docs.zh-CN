---
title: rubricQualityFeedbackModel 资源类型
description: 与 educationRubric 的特定质量相关的反馈
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 0a7c2b80a2cef18b50157ae9a54c66d35822fa51
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173298"
---
# <a name="rubricqualityfeedbackmodel-resource-type"></a><span data-ttu-id="f774f-103">rubricQualityFeedbackModel 资源类型</span><span class="sxs-lookup"><span data-stu-id="f774f-103">rubricQualityFeedbackModel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f774f-104">与[educationRubric](educationrubric.md)的特定[质量](rubricquality.md)相关的反馈。</span><span class="sxs-lookup"><span data-stu-id="f774f-104">Feedback related to a specific [quality](rubricquality.md) of an [educationRubric](educationrubric.md).</span></span>

## <a name="properties"></a><span data-ttu-id="f774f-105">属性</span><span class="sxs-lookup"><span data-stu-id="f774f-105">Properties</span></span>

| <span data-ttu-id="f774f-106">属性</span><span class="sxs-lookup"><span data-stu-id="f774f-106">Property</span></span>     | <span data-ttu-id="f774f-107">类型</span><span class="sxs-lookup"><span data-stu-id="f774f-107">Type</span></span>        | <span data-ttu-id="f774f-108">说明</span><span class="sxs-lookup"><span data-stu-id="f774f-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f774f-109">反馈</span><span class="sxs-lookup"><span data-stu-id="f774f-109">feedback</span></span>|[<span data-ttu-id="f774f-110">itemBody</span><span class="sxs-lookup"><span data-stu-id="f774f-110">itemBody</span></span>](itembody.md)|<span data-ttu-id="f774f-111">针对此 rubric 的一种质量的特定反馈。</span><span class="sxs-lookup"><span data-stu-id="f774f-111">Specific feedback for one quality of this rubric.</span></span>|
|<span data-ttu-id="f774f-112">qualityId</span><span class="sxs-lookup"><span data-stu-id="f774f-112">qualityId</span></span>|<span data-ttu-id="f774f-113">String</span><span class="sxs-lookup"><span data-stu-id="f774f-113">String</span></span>|<span data-ttu-id="f774f-114">与此反馈相关的[rubricQuality](rubricquality.md)的 ID。</span><span class="sxs-lookup"><span data-stu-id="f774f-114">The ID of the [rubricQuality](rubricquality.md) that this feedback is related to.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f774f-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f774f-115">JSON representation</span></span>

<span data-ttu-id="f774f-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f774f-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rubricQualityFeedbackModel",
  "baseType": null
}-->

```json
{
  "feedback": {"@odata.type": "microsoft.graph.itemBody"},
  "qualityId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "rubricQualityFeedbackModel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->