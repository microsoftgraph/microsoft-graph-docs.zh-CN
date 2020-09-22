---
title: aggregationOption 资源类型
description: 指定 aggregationOption 实体
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: c18cc1801e5eac76d2fa4396f809ff68f59a78fe
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193863"
---
# <a name="aggregationoption-resource-type"></a><span data-ttu-id="6f9b5-103">aggregationOption 资源类型</span><span class="sxs-lookup"><span data-stu-id="6f9b5-103">aggregationOption resource type</span></span>

<span data-ttu-id="6f9b5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6f9b5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6f9b5-105">指定在搜索结果的旁边应返回哪些聚合。</span><span class="sxs-lookup"><span data-stu-id="6f9b5-105">Specifies which aggregations should be returned alongside the search results.</span></span>

## <a name="properties"></a><span data-ttu-id="6f9b5-106">属性</span><span class="sxs-lookup"><span data-stu-id="6f9b5-106">Properties</span></span>

| <span data-ttu-id="6f9b5-107">属性</span><span class="sxs-lookup"><span data-stu-id="6f9b5-107">Property</span></span>     | <span data-ttu-id="6f9b5-108">类型</span><span class="sxs-lookup"><span data-stu-id="6f9b5-108">Type</span></span>        | <span data-ttu-id="6f9b5-109">描述</span><span class="sxs-lookup"><span data-stu-id="6f9b5-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6f9b5-110">字段</span><span class="sxs-lookup"><span data-stu-id="6f9b5-110">field</span></span>|<span data-ttu-id="6f9b5-111">字符串</span><span class="sxs-lookup"><span data-stu-id="6f9b5-111">String</span></span>|<span data-ttu-id="6f9b5-112">指定应在其上计算聚合的指定实体类型的架构中的字段。</span><span class="sxs-lookup"><span data-stu-id="6f9b5-112">Specifies the field in the schema of the specified entity type that aggregation should be computed on.</span></span> <span data-ttu-id="6f9b5-113">必需。</span><span class="sxs-lookup"><span data-stu-id="6f9b5-113">Required.</span></span>|
|<span data-ttu-id="6f9b5-114">大小</span><span class="sxs-lookup"><span data-stu-id="6f9b5-114">size</span></span>|<span data-ttu-id="6f9b5-115">Int32</span><span class="sxs-lookup"><span data-stu-id="6f9b5-115">Int32</span></span>|<span data-ttu-id="6f9b5-116">要返回的 [searchBucket](searchBucket.md) 资源数。</span><span class="sxs-lookup"><span data-stu-id="6f9b5-116">The number of [searchBucket](searchBucket.md) resources to be returned.</span></span> <span data-ttu-id="6f9b5-117">当在搜索请求中手动提供范围时，这不是必需的。</span><span class="sxs-lookup"><span data-stu-id="6f9b5-117">This is not required when the range is provided manually in the search request.</span></span> <span data-ttu-id="6f9b5-118">可选。</span><span class="sxs-lookup"><span data-stu-id="6f9b5-118">Optional.</span></span>|
|<span data-ttu-id="6f9b5-119">bucketDefinition</span><span class="sxs-lookup"><span data-stu-id="6f9b5-119">bucketDefinition</span></span>|[<span data-ttu-id="6f9b5-120">bucketAggregationDefinition</span><span class="sxs-lookup"><span data-stu-id="6f9b5-120">bucketAggregationDefinition</span></span>](bucketaggregationdefinition.md)|<span data-ttu-id="6f9b5-121">指定计算聚合的条件。</span><span class="sxs-lookup"><span data-stu-id="6f9b5-121">Specifies the criteria to compute an aggregation.</span></span> <span data-ttu-id="6f9b5-122">可选。</span><span class="sxs-lookup"><span data-stu-id="6f9b5-122">Optional.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6f9b5-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6f9b5-123">JSON representation</span></span>

<span data-ttu-id="6f9b5-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6f9b5-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.aggregationOption",
  "baseType": null
}-->

```json
{
  "field": "String",
  "size": 1024,
  "bucketDefinition": {"@odata.type": "microsoft.graph.bucketAggregationDefinition"}
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