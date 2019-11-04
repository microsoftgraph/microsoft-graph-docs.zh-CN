---
title: inferenceData 资源类型
description: inferenceData 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: profile
doc_type: resourcePageType
ms.openlocfilehash: 43d6585243eed560a6a8f77268305b7d7f5824a8
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938847"
---
# <a name="inferencedata-resource-type"></a><span data-ttu-id="06d2e-103">inferenceData 资源类型</span><span class="sxs-lookup"><span data-stu-id="06d2e-103">inferenceData resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="06d2e-104">[InferenceData](inferencedata.md)资源类型提供了有关通过推断用户信息创建的实体的附加详细信息。</span><span class="sxs-lookup"><span data-stu-id="06d2e-104">The [inferenceData](inferencedata.md) resource type provides additional detail about an entity which has been created through inferring information about the user.</span></span> <span data-ttu-id="06d2e-105">只要特定实体中的数据是由机器学习或其他系统进程对数据进行迭代时，就会出现此信息。</span><span class="sxs-lookup"><span data-stu-id="06d2e-105">This information will be present whenever the data within a particular entity was derived from a machine learning or other system process iterating over data.</span></span>

## <a name="properties"></a><span data-ttu-id="06d2e-106">属性</span><span class="sxs-lookup"><span data-stu-id="06d2e-106">Properties</span></span>

| <span data-ttu-id="06d2e-107">属性</span><span class="sxs-lookup"><span data-stu-id="06d2e-107">Property</span></span>              | <span data-ttu-id="06d2e-108">类型</span><span class="sxs-lookup"><span data-stu-id="06d2e-108">Type</span></span>        | <span data-ttu-id="06d2e-109">描述</span><span class="sxs-lookup"><span data-stu-id="06d2e-109">Description</span></span>                                                                     |
|:----------------------|:------------|:--------------------------------------------------------------------------------|
|<span data-ttu-id="06d2e-110">confidenceScore</span><span class="sxs-lookup"><span data-stu-id="06d2e-110">confidenceScore</span></span>        |<span data-ttu-id="06d2e-111">双精度</span><span class="sxs-lookup"><span data-stu-id="06d2e-111">Double</span></span>       | <span data-ttu-id="06d2e-112">反映有关用户推断的数据准确性的置信度分数。</span><span class="sxs-lookup"><span data-stu-id="06d2e-112">Confidence score reflecting the accuracy of the data inferred about the user.</span></span>   |
|<span data-ttu-id="06d2e-113">userHasVerifiedAccuracy</span><span class="sxs-lookup"><span data-stu-id="06d2e-113">userHasVerifiedAccuracy</span></span>|<span data-ttu-id="06d2e-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="06d2e-114">Boolean</span></span>      | <span data-ttu-id="06d2e-115">如果用户已确认此推理为 True 或 False，则为记录。</span><span class="sxs-lookup"><span data-stu-id="06d2e-115">Records if the user has confirmed this inference as being True or False.</span></span>        |

## <a name="json-representation"></a><span data-ttu-id="06d2e-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="06d2e-116">JSON representation</span></span>

<span data-ttu-id="06d2e-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="06d2e-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.inferenceData",
  "baseType": null
}-->

```json
{
  "confidenceScore": 1024,
  "userHasVerifiedAccuracy": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "inferenceData resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->