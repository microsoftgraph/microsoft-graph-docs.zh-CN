---
title: bucketAggregationDefinition 资源类型
description: 提供有关如何在结果中生成 agregations 的详细信息
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 1f9fdadefc43b99b8772217db9a9b101357a1c9c
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193869"
---
# <a name="bucketaggregationdefinition-resource-type"></a><span data-ttu-id="a0e13-103">bucketAggregationDefinition 资源类型</span><span class="sxs-lookup"><span data-stu-id="a0e13-103">bucketAggregationDefinition resource type</span></span>

<span data-ttu-id="a0e13-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a0e13-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a0e13-105">指定聚合搜索结果的详细信息。</span><span class="sxs-lookup"><span data-stu-id="a0e13-105">Specifies details to aggregate search results.</span></span>

## <a name="properties"></a><span data-ttu-id="a0e13-106">属性</span><span class="sxs-lookup"><span data-stu-id="a0e13-106">Properties</span></span>

| <span data-ttu-id="a0e13-107">属性</span><span class="sxs-lookup"><span data-stu-id="a0e13-107">Property</span></span>     | <span data-ttu-id="a0e13-108">类型</span><span class="sxs-lookup"><span data-stu-id="a0e13-108">Type</span></span>        | <span data-ttu-id="a0e13-109">描述</span><span class="sxs-lookup"><span data-stu-id="a0e13-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a0e13-110">sortBy</span><span class="sxs-lookup"><span data-stu-id="a0e13-110">sortBy</span></span>|<span data-ttu-id="a0e13-111">bucketAggregationSortProperty</span><span class="sxs-lookup"><span data-stu-id="a0e13-111">bucketAggregationSortProperty</span></span>| <span data-ttu-id="a0e13-112">可能的值是 `count` 按聚合中的匹配项数进行排序，基于聚合中的键对 `keyAsString` alphabeticaly 进行排序，以 `keyAsNumber` 实现基于聚合中键的数值排序。</span><span class="sxs-lookup"><span data-stu-id="a0e13-112">The possible values are `count` to sort by the number of matches in the aggregation, `keyAsString`to sort alphabeticaly based on the key in the aggregation, `keyAsNumber` for numerical sorting based on the key in the aggregation.</span></span> <span data-ttu-id="a0e13-113">必需。</span><span class="sxs-lookup"><span data-stu-id="a0e13-113">Required.</span></span>
|<span data-ttu-id="a0e13-114">isDescending</span><span class="sxs-lookup"><span data-stu-id="a0e13-114">isDescending</span></span>|<span data-ttu-id="a0e13-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="a0e13-115">Boolean</span></span>|<span data-ttu-id="a0e13-116">`True` 指定排序次序为降序。</span><span class="sxs-lookup"><span data-stu-id="a0e13-116">`True` to specify the sort order as descending.</span></span> <span data-ttu-id="a0e13-117">默认值为 `false` ，排序次序为升序。</span><span class="sxs-lookup"><span data-stu-id="a0e13-117">The default is `false`, with the sort order as ascending.</span></span> <span data-ttu-id="a0e13-118">可选。</span><span class="sxs-lookup"><span data-stu-id="a0e13-118">Optional.</span></span>|
|<span data-ttu-id="a0e13-119">prefixFilter</span><span class="sxs-lookup"><span data-stu-id="a0e13-119">prefixFilter</span></span>|<span data-ttu-id="a0e13-120">字符串</span><span class="sxs-lookup"><span data-stu-id="a0e13-120">String</span></span>|<span data-ttu-id="a0e13-121">用于定义匹配条件的筛选器。</span><span class="sxs-lookup"><span data-stu-id="a0e13-121">A filter to define a matching criteria.</span></span> <span data-ttu-id="a0e13-122">该密钥应以指定的前缀开头，以在响应中返回。</span><span class="sxs-lookup"><span data-stu-id="a0e13-122">The key should start with the specified prefix to be returned in the response.</span></span> <span data-ttu-id="a0e13-123">可选。</span><span class="sxs-lookup"><span data-stu-id="a0e13-123">Optional.</span></span>|
|<span data-ttu-id="a0e13-124">minimumCount</span><span class="sxs-lookup"><span data-stu-id="a0e13-124">minimumCount</span></span>|<span data-ttu-id="a0e13-125">Int32</span><span class="sxs-lookup"><span data-stu-id="a0e13-125">Int32</span></span>|<span data-ttu-id="a0e13-126">应在存储桶中返回的聚合中应存在的最小项目数。</span><span class="sxs-lookup"><span data-stu-id="a0e13-126">The minimum number of items that should be present in the aggregation to be returned in a bucket.</span></span> <span data-ttu-id="a0e13-127">可选。</span><span class="sxs-lookup"><span data-stu-id="a0e13-127">Optional.</span></span>|
|<span data-ttu-id="a0e13-128">ranges</span><span class="sxs-lookup"><span data-stu-id="a0e13-128">ranges</span></span>|<span data-ttu-id="a0e13-129">[bucketAggregationRange](bucketaggregationrange.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a0e13-129">[bucketAggregationRange](bucketaggregationrange.md) collection</span></span>|<span data-ttu-id="a0e13-130">指定用于计算聚合的手动范围。</span><span class="sxs-lookup"><span data-stu-id="a0e13-130">Specifies the manual ranges to compute the aggregations.</span></span> <span data-ttu-id="a0e13-131">这仅对日期或数值类型的非字符串精简程序有效。</span><span class="sxs-lookup"><span data-stu-id="a0e13-131">This is only valid for non-string refiners of date or numeric type.</span></span> <span data-ttu-id="a0e13-132">可选。</span><span class="sxs-lookup"><span data-stu-id="a0e13-132">Optional.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a0e13-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a0e13-133">JSON representation</span></span>

<span data-ttu-id="a0e13-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a0e13-134">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bucketAggregationDefinition",
  "baseType": null
}-->

```json
{
  "sortBy": "String",
  "isDescending": true,
  "prefixFilter": "String",
  "minimumCount": 1024,
  "ranges": [{"@odata.type": "microsoft.graph.bucketAggregationRange"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sortProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->