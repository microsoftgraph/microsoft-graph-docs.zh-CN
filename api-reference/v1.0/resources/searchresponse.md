---
title: searchResponse 资源类型
description: SearchResponse 的说明
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 8582da8daf604952807e05376d98dabf16267052
ms.sourcegitcommit: 5345c2f3265ede107fa0faaff7a3f1c2afee3810
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/21/2020
ms.locfileid: "49377774"
---
# <a name="searchresponse-resource-type"></a><span data-ttu-id="3a5da-103">searchResponse 资源类型</span><span class="sxs-lookup"><span data-stu-id="3a5da-103">searchResponse resource type</span></span>

<span data-ttu-id="3a5da-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3a5da-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3a5da-105">表示搜索查询中的结果和用于查询的术语。</span><span class="sxs-lookup"><span data-stu-id="3a5da-105">Represents results from a search query, and the terms used for the query.</span></span> 

## <a name="properties"></a><span data-ttu-id="3a5da-106">属性</span><span class="sxs-lookup"><span data-stu-id="3a5da-106">Properties</span></span>

| <span data-ttu-id="3a5da-107">属性</span><span class="sxs-lookup"><span data-stu-id="3a5da-107">Property</span></span>     | <span data-ttu-id="3a5da-108">类型</span><span class="sxs-lookup"><span data-stu-id="3a5da-108">Type</span></span>        | <span data-ttu-id="3a5da-109">说明</span><span class="sxs-lookup"><span data-stu-id="3a5da-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3a5da-110">hitsContainers</span><span class="sxs-lookup"><span data-stu-id="3a5da-110">hitsContainers</span></span>|<span data-ttu-id="3a5da-111">[searchHitsContainer](searchhitscontainer.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3a5da-111">[searchHitsContainer](searchhitscontainer.md) collection</span></span>|<span data-ttu-id="3a5da-112">搜索结果的集合。</span><span class="sxs-lookup"><span data-stu-id="3a5da-112">A collection of search results.</span></span>|
|<span data-ttu-id="3a5da-113">searchTerms</span><span class="sxs-lookup"><span data-stu-id="3a5da-113">searchTerms</span></span>|<span data-ttu-id="3a5da-114">String collection</span><span class="sxs-lookup"><span data-stu-id="3a5da-114">String collection</span></span>|<span data-ttu-id="3a5da-115">包含在初始搜索查询中发送的搜索词。</span><span class="sxs-lookup"><span data-stu-id="3a5da-115">Contains the search terms sent in the initial search query.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3a5da-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3a5da-116">JSON representation</span></span>

<span data-ttu-id="3a5da-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3a5da-117">The following is a JSON representation of the resource.</span></span>

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

