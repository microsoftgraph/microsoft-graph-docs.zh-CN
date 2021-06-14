---
title: rubricQualityFeedbackModel 资源类型
description: 与 educationRubric 的特定质量相关的反馈。
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 8f96a1fd0ce0d007c138928c316316349a7b302e
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/12/2021
ms.locfileid: "52911404"
---
# <a name="rubricqualityfeedbackmodel-resource-type"></a><span data-ttu-id="3e187-103">rubricQualityFeedbackModel 资源类型</span><span class="sxs-lookup"><span data-stu-id="3e187-103">rubricQualityFeedbackModel resource type</span></span>

<span data-ttu-id="3e187-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e187-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3e187-105">与[educationRubric](educationrubric.md)的特定[质量](rubricquality.md)相关的反馈。</span><span class="sxs-lookup"><span data-stu-id="3e187-105">Feedback related to a specific [quality](rubricquality.md) of an [educationRubric](educationrubric.md).</span></span>

## <a name="properties"></a><span data-ttu-id="3e187-106">属性</span><span class="sxs-lookup"><span data-stu-id="3e187-106">Properties</span></span>

| <span data-ttu-id="3e187-107">属性</span><span class="sxs-lookup"><span data-stu-id="3e187-107">Property</span></span>     | <span data-ttu-id="3e187-108">类型</span><span class="sxs-lookup"><span data-stu-id="3e187-108">Type</span></span>        | <span data-ttu-id="3e187-109">说明</span><span class="sxs-lookup"><span data-stu-id="3e187-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3e187-110">反馈</span><span class="sxs-lookup"><span data-stu-id="3e187-110">feedback</span></span>|[<span data-ttu-id="3e187-111">itemBody</span><span class="sxs-lookup"><span data-stu-id="3e187-111">itemBody</span></span>](itembody.md)|<span data-ttu-id="3e187-112">有关此标准一个质量的具体反馈。</span><span class="sxs-lookup"><span data-stu-id="3e187-112">Specific feedback for one quality of this rubric.</span></span>|
|<span data-ttu-id="3e187-113">qualityId</span><span class="sxs-lookup"><span data-stu-id="3e187-113">qualityId</span></span>|<span data-ttu-id="3e187-114">String</span><span class="sxs-lookup"><span data-stu-id="3e187-114">String</span></span>|<span data-ttu-id="3e187-115">此反馈相关的 [rubricQuality](rubricquality.md) 的 ID。</span><span class="sxs-lookup"><span data-stu-id="3e187-115">The ID of the [rubricQuality](rubricquality.md) that this feedback is related to.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3e187-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3e187-116">JSON representation</span></span>

<span data-ttu-id="3e187-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3e187-117">The following is a JSON representation of the resource.</span></span>

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

