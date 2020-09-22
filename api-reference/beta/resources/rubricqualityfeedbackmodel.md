---
title: rubricQualityFeedbackModel 资源类型
description: 与 educationRubric 的特定质量相关的反馈
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 56fea149446c79dd95e50e1b5d152cc8610dc0dd
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016063"
---
# <a name="rubricqualityfeedbackmodel-resource-type"></a><span data-ttu-id="07d81-103">rubricQualityFeedbackModel 资源类型</span><span class="sxs-lookup"><span data-stu-id="07d81-103">rubricQualityFeedbackModel resource type</span></span>

<span data-ttu-id="07d81-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07d81-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="07d81-105">与[educationRubric](educationrubric.md)的特定[质量](rubricquality.md)相关的反馈。</span><span class="sxs-lookup"><span data-stu-id="07d81-105">Feedback related to a specific [quality](rubricquality.md) of an [educationRubric](educationrubric.md).</span></span>

## <a name="properties"></a><span data-ttu-id="07d81-106">属性</span><span class="sxs-lookup"><span data-stu-id="07d81-106">Properties</span></span>

| <span data-ttu-id="07d81-107">属性</span><span class="sxs-lookup"><span data-stu-id="07d81-107">Property</span></span>     | <span data-ttu-id="07d81-108">类型</span><span class="sxs-lookup"><span data-stu-id="07d81-108">Type</span></span>        | <span data-ttu-id="07d81-109">说明</span><span class="sxs-lookup"><span data-stu-id="07d81-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="07d81-110">反馈</span><span class="sxs-lookup"><span data-stu-id="07d81-110">feedback</span></span>|[<span data-ttu-id="07d81-111">itemBody</span><span class="sxs-lookup"><span data-stu-id="07d81-111">itemBody</span></span>](itembody.md)|<span data-ttu-id="07d81-112">针对此 rubric 的一种质量的特定反馈。</span><span class="sxs-lookup"><span data-stu-id="07d81-112">Specific feedback for one quality of this rubric.</span></span>|
|<span data-ttu-id="07d81-113">qualityId</span><span class="sxs-lookup"><span data-stu-id="07d81-113">qualityId</span></span>|<span data-ttu-id="07d81-114">String</span><span class="sxs-lookup"><span data-stu-id="07d81-114">String</span></span>|<span data-ttu-id="07d81-115">与此反馈相关的 [rubricQuality](rubricquality.md) 的 ID。</span><span class="sxs-lookup"><span data-stu-id="07d81-115">The ID of the [rubricQuality](rubricquality.md) that this feedback is related to.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="07d81-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="07d81-116">JSON representation</span></span>

<span data-ttu-id="07d81-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="07d81-117">The following is a JSON representation of the resource.</span></span>

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

