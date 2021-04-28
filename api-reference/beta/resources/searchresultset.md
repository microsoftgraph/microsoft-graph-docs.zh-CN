---
title: searchResultSet 资源类型
description: searchResultSet 的说明
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 5d17791a618f1d587520f23524da9ce19241d3b1
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067864"
---
# <a name="searchresultset-resource-type"></a><span data-ttu-id="d3d19-103">searchResultSet 资源类型</span><span class="sxs-lookup"><span data-stu-id="d3d19-103">searchResultSet resource type</span></span>

<span data-ttu-id="d3d19-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3d19-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d3d19-105">表示来自搜索查询的结果，以及用于查询的术语。</span><span class="sxs-lookup"><span data-stu-id="d3d19-105">Represents results from a search query, and the terms used for the query.</span></span> 

## <a name="properties"></a><span data-ttu-id="d3d19-106">属性</span><span class="sxs-lookup"><span data-stu-id="d3d19-106">Properties</span></span>

| <span data-ttu-id="d3d19-107">属性</span><span class="sxs-lookup"><span data-stu-id="d3d19-107">Property</span></span>     | <span data-ttu-id="d3d19-108">类型</span><span class="sxs-lookup"><span data-stu-id="d3d19-108">Type</span></span>        | <span data-ttu-id="d3d19-109">说明</span><span class="sxs-lookup"><span data-stu-id="d3d19-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d3d19-110">hitsContainers</span><span class="sxs-lookup"><span data-stu-id="d3d19-110">hitsContainers</span></span>|<span data-ttu-id="d3d19-111">[searchHitsContainer](searchhitscontainer.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d3d19-111">[searchHitsContainer](searchhitscontainer.md) collection</span></span>|<span data-ttu-id="d3d19-112">搜索结果的集合。</span><span class="sxs-lookup"><span data-stu-id="d3d19-112">A collection of search results.</span></span>|
|<span data-ttu-id="d3d19-113">searchTerms</span><span class="sxs-lookup"><span data-stu-id="d3d19-113">searchTerms</span></span>|<span data-ttu-id="d3d19-114">字符串集合</span><span class="sxs-lookup"><span data-stu-id="d3d19-114">String collection</span></span>|<span data-ttu-id="d3d19-115">包含初始搜索查询中发送的搜索词。</span><span class="sxs-lookup"><span data-stu-id="d3d19-115">Contains the search terms sent in the initial search query.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d3d19-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d3d19-116">JSON representation</span></span>

<span data-ttu-id="d3d19-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d3d19-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchResultSet",
  "baseType": null
}-->

```json
{
  "hitsContainers": [{"@odata.type": "microsoft.graph.searchHitsContainer"}],
  "searchTerms": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchResultSet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

