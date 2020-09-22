---
title: searchAggregation 资源类型
description: 提供搜索响应中的搜索聚合的详细信息。
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 480a6f70a2815a174697ff22fc217057053e1f4b
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193860"
---
# <a name="searchaggregation-resource-type"></a><span data-ttu-id="14379-103">searchAggregation 资源类型</span><span class="sxs-lookup"><span data-stu-id="14379-103">searchAggregation resource type</span></span>

<span data-ttu-id="14379-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14379-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="14379-105">提供搜索响应中的搜索聚合的详细信息。</span><span class="sxs-lookup"><span data-stu-id="14379-105">Provides the details of the search aggregation in the search response.</span></span>

## <a name="properties"></a><span data-ttu-id="14379-106">属性</span><span class="sxs-lookup"><span data-stu-id="14379-106">Properties</span></span>

| <span data-ttu-id="14379-107">属性</span><span class="sxs-lookup"><span data-stu-id="14379-107">Property</span></span>     | <span data-ttu-id="14379-108">类型</span><span class="sxs-lookup"><span data-stu-id="14379-108">Type</span></span>        | <span data-ttu-id="14379-109">说明</span><span class="sxs-lookup"><span data-stu-id="14379-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="14379-110">displayName</span><span class="sxs-lookup"><span data-stu-id="14379-110">displayName</span></span>|<span data-ttu-id="14379-111">字符串</span><span class="sxs-lookup"><span data-stu-id="14379-111">String</span></span>| <span data-ttu-id="14379-112">聚合的友好名称。</span><span class="sxs-lookup"><span data-stu-id="14379-112">The friendly name of the aggregation.</span></span> <span data-ttu-id="14379-113">输入中提供了此值。</span><span class="sxs-lookup"><span data-stu-id="14379-113">This value was provided in the input.</span></span>|
|<span data-ttu-id="14379-114">字段</span><span class="sxs-lookup"><span data-stu-id="14379-114">field</span></span>|<span data-ttu-id="14379-115">字符串</span><span class="sxs-lookup"><span data-stu-id="14379-115">String</span></span>| <span data-ttu-id="14379-116">定义在哪一字段上计算聚合。</span><span class="sxs-lookup"><span data-stu-id="14379-116">Defines on which field the aggregation was computed on.</span></span>|
|<span data-ttu-id="14379-117">buckets</span><span class="sxs-lookup"><span data-stu-id="14379-117">buckets</span></span>|<span data-ttu-id="14379-118">[searchBucket](searchbucket.md) 集合</span><span class="sxs-lookup"><span data-stu-id="14379-118">[searchBucket](searchbucket.md) collection</span></span>| <span data-ttu-id="14379-119">定义计算出的聚合的实际存储桶。</span><span class="sxs-lookup"><span data-stu-id="14379-119">Defines the actual buckets of the computed aggregation.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="14379-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="14379-120">JSON representation</span></span>

<span data-ttu-id="14379-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="14379-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchAggregation",
  "baseType": null
}-->

```json
{
  "displayName": "String",
  "field": "String",  
  "buckets": [{"@odata.type": "microsoft.graph.searchBucket"}]
}
```