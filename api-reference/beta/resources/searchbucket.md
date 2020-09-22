---
title: searchBucket 资源类型
description: 在响应中提供特定聚合，即特定存储桶的值。
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 3fe375ca2e9695a237b60e30cdd9e98a9e545d35
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193858"
---
# <a name="searchbucket-resource-type"></a><span data-ttu-id="a5986-103">searchBucket 资源类型</span><span class="sxs-lookup"><span data-stu-id="a5986-103">searchBucket resource type</span></span>

<span data-ttu-id="a5986-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a5986-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a5986-105">表示一个或多个搜索结果的容器，这些搜索结果共享聚合它们的实体字段的相同值。</span><span class="sxs-lookup"><span data-stu-id="a5986-105">Represents a container for one or more search results that share the same value for the entity field that aggregates them.</span></span> 



## <a name="properties"></a><span data-ttu-id="a5986-106">属性</span><span class="sxs-lookup"><span data-stu-id="a5986-106">Properties</span></span>

| <span data-ttu-id="a5986-107">属性</span><span class="sxs-lookup"><span data-stu-id="a5986-107">Property</span></span>     | <span data-ttu-id="a5986-108">类型</span><span class="sxs-lookup"><span data-stu-id="a5986-108">Type</span></span>        | <span data-ttu-id="a5986-109">描述</span><span class="sxs-lookup"><span data-stu-id="a5986-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a5986-110">Key</span><span class="sxs-lookup"><span data-stu-id="a5986-110">key</span></span>|<span data-ttu-id="a5986-111">字符串</span><span class="sxs-lookup"><span data-stu-id="a5986-111">String</span></span>| <span data-ttu-id="a5986-112">计算聚合所依据的字段的离散值。</span><span class="sxs-lookup"><span data-stu-id="a5986-112">The discrete value of the field that an aggregation was computed on.</span></span>|
|<span data-ttu-id="a5986-113">count</span><span class="sxs-lookup"><span data-stu-id="a5986-113">count</span></span>|<span data-ttu-id="a5986-114">Int32</span><span class="sxs-lookup"><span data-stu-id="a5986-114">Int32</span></span>| <span data-ttu-id="a5986-115">与 **key** 属性中指定的值相同的搜索匹配项的数量。</span><span class="sxs-lookup"><span data-stu-id="a5986-115">The number of search matches that share the same value specified in the **key** property.</span></span> |
|<span data-ttu-id="a5986-116">aggregationFilterToken</span><span class="sxs-lookup"><span data-stu-id="a5986-116">aggregationFilterToken</span></span>|<span data-ttu-id="a5986-117">字符串</span><span class="sxs-lookup"><span data-stu-id="a5986-117">String</span></span>| <span data-ttu-id="a5986-118">包含编码的筛选器的令牌，以聚合搜索匹配项的特定 **键值** 。</span><span class="sxs-lookup"><span data-stu-id="a5986-118">A token containing the encoded filter to aggregate search matches by the specific **key** value.</span></span> <span data-ttu-id="a5986-119">若要使用筛选器，请将令牌作为**searchRequest**对象中的**aggregationFilter**属性的一部分进行传递，格式为 **"{field}： \\ " {aggregationFilterToken} \\ ""**。</span><span class="sxs-lookup"><span data-stu-id="a5986-119">To use the filter, pass the token as part of the **aggregationFilter** property in a **searchRequest** object, in the format **"{field}:\\"{aggregationFilterToken}\\""**.</span></span> <span data-ttu-id="a5986-120">请参阅[示例](/graph/search-concept-aggregation#example-2-apply-an-aggregation-filter-based-on-a-previous-request)。</span><span class="sxs-lookup"><span data-stu-id="a5986-120">See an [example](/graph/search-concept-aggregation#example-2-apply-an-aggregation-filter-based-on-a-previous-request).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a5986-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a5986-121">JSON representation</span></span>

<span data-ttu-id="a5986-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a5986-122">The following is a JSON representation of the resource.</span></span>

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
