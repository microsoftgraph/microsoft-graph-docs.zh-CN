---
title: searchBucket 资源类型
description: 在响应中提供特定聚合，即特定存储桶的值。
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: a6b26c01133f519b0308ffee430d85c9df6d868b
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/07/2020
ms.locfileid: "48373851"
---
# <a name="searchbucket-resource-type"></a><span data-ttu-id="bfa21-103">searchBucket 资源类型</span><span class="sxs-lookup"><span data-stu-id="bfa21-103">searchBucket resource type</span></span>

<span data-ttu-id="bfa21-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bfa21-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bfa21-105">表示一个或多个搜索结果的容器，这些搜索结果共享聚合它们的实体字段的相同值。</span><span class="sxs-lookup"><span data-stu-id="bfa21-105">Represents a container for one or more search results that share the same value for the entity field that aggregates them.</span></span> 

## <a name="properties"></a><span data-ttu-id="bfa21-106">属性</span><span class="sxs-lookup"><span data-stu-id="bfa21-106">Properties</span></span>

| <span data-ttu-id="bfa21-107">属性</span><span class="sxs-lookup"><span data-stu-id="bfa21-107">Property</span></span>     | <span data-ttu-id="bfa21-108">类型</span><span class="sxs-lookup"><span data-stu-id="bfa21-108">Type</span></span>        | <span data-ttu-id="bfa21-109">说明</span><span class="sxs-lookup"><span data-stu-id="bfa21-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="bfa21-110">Key</span><span class="sxs-lookup"><span data-stu-id="bfa21-110">key</span></span>|<span data-ttu-id="bfa21-111">String</span><span class="sxs-lookup"><span data-stu-id="bfa21-111">String</span></span>| <span data-ttu-id="bfa21-112">计算聚合所依据的字段的离散值。</span><span class="sxs-lookup"><span data-stu-id="bfa21-112">The discrete value of the field that an aggregation was computed on.</span></span>|
|<span data-ttu-id="bfa21-113">count</span><span class="sxs-lookup"><span data-stu-id="bfa21-113">count</span></span>|<span data-ttu-id="bfa21-114">Int32</span><span class="sxs-lookup"><span data-stu-id="bfa21-114">Int32</span></span>| <span data-ttu-id="bfa21-115">与在 **key** 属性中指定的相同值共享的近似搜索匹配数。</span><span class="sxs-lookup"><span data-stu-id="bfa21-115">The approximate number of search matches that share the same value specified in the **key** property.</span></span> <span data-ttu-id="bfa21-116">请注意，此数字不是精确的匹配数。</span><span class="sxs-lookup"><span data-stu-id="bfa21-116">Note that this number is not the exact number of matches.</span></span>|
|<span data-ttu-id="bfa21-117">aggregationFilterToken</span><span class="sxs-lookup"><span data-stu-id="bfa21-117">aggregationFilterToken</span></span>|<span data-ttu-id="bfa21-118">String</span><span class="sxs-lookup"><span data-stu-id="bfa21-118">String</span></span>| <span data-ttu-id="bfa21-119">包含编码的筛选器的令牌，以聚合搜索匹配项的特定 **键值** 。</span><span class="sxs-lookup"><span data-stu-id="bfa21-119">A token containing the encoded filter to aggregate search matches by the specific **key** value.</span></span> <span data-ttu-id="bfa21-120">若要使用筛选器，请将令牌作为**searchRequest**对象中的**aggregationFilter**属性的一部分进行传递，格式为 **"{field}： \\ " {aggregationFilterToken} \\ ""**。</span><span class="sxs-lookup"><span data-stu-id="bfa21-120">To use the filter, pass the token as part of the **aggregationFilter** property in a **searchRequest** object, in the format **"{field}:\\"{aggregationFilterToken}\\""**.</span></span> <span data-ttu-id="bfa21-121">请参阅[示例](/graph/search-concept-aggregation#example-2-apply-an-aggregation-filter-based-on-a-previous-request)。</span><span class="sxs-lookup"><span data-stu-id="bfa21-121">See an [example](/graph/search-concept-aggregation#example-2-apply-an-aggregation-filter-based-on-a-previous-request).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bfa21-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bfa21-122">JSON representation</span></span>

<span data-ttu-id="bfa21-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bfa21-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchBucket",
  "baseType": null
}-->

```json
{
  "key": "String",
  "count": "10",  
  "aggregationFilterToken": "String"
}
```
