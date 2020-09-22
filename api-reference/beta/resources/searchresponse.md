---
title: searchResponse 资源类型
description: SearchResponse 的说明
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: deb5450017b4ae9db534c30f71dd6da4f1a9b812
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/22/2020
ms.locfileid: "48192747"
---
# <a name="searchresponse-resource-type"></a><span data-ttu-id="c0170-103">searchResponse 资源类型</span><span class="sxs-lookup"><span data-stu-id="c0170-103">searchResponse resource type</span></span>

<span data-ttu-id="c0170-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0170-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c0170-105">表示搜索查询中的结果和用于查询的术语。</span><span class="sxs-lookup"><span data-stu-id="c0170-105">Represents results from a search query, and the terms used for the query.</span></span> 

## <a name="properties"></a><span data-ttu-id="c0170-106">属性</span><span class="sxs-lookup"><span data-stu-id="c0170-106">Properties</span></span>

| <span data-ttu-id="c0170-107">属性</span><span class="sxs-lookup"><span data-stu-id="c0170-107">Property</span></span>     | <span data-ttu-id="c0170-108">类型</span><span class="sxs-lookup"><span data-stu-id="c0170-108">Type</span></span>        | <span data-ttu-id="c0170-109">描述</span><span class="sxs-lookup"><span data-stu-id="c0170-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c0170-110">hitsContainers</span><span class="sxs-lookup"><span data-stu-id="c0170-110">hitsContainers</span></span>|<span data-ttu-id="c0170-111">[searchHitsContainer](searchhitscontainer.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c0170-111">[searchHitsContainer](searchhitscontainer.md) collection</span></span>|<span data-ttu-id="c0170-112">搜索结果的集合。</span><span class="sxs-lookup"><span data-stu-id="c0170-112">A collection of search results.</span></span>|
|<span data-ttu-id="c0170-113">searchTerms</span><span class="sxs-lookup"><span data-stu-id="c0170-113">searchTerms</span></span>|<span data-ttu-id="c0170-114">String collection</span><span class="sxs-lookup"><span data-stu-id="c0170-114">String collection</span></span>|<span data-ttu-id="c0170-115">包含在初始搜索查询中发送的搜索词。</span><span class="sxs-lookup"><span data-stu-id="c0170-115">Contains the search terms sent in the initial search query.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c0170-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c0170-116">JSON representation</span></span>

<span data-ttu-id="c0170-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c0170-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchResponse",
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
  "description": "searchResponse resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

