---
title: searchResponse 资源类型
description: 在此处提供说明
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: a2bdd013cb755d37664c89aca81a8ae89c63b4f9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47973737"
---
# <a name="searchresponse-resource-type"></a><span data-ttu-id="bb771-103">searchResponse 资源类型</span><span class="sxs-lookup"><span data-stu-id="bb771-103">searchResponse resource type</span></span>

<span data-ttu-id="bb771-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb771-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bb771-105">SearchResponse 包含搜索查询中的结果。</span><span class="sxs-lookup"><span data-stu-id="bb771-105">The searchResponse contains the results from the search query.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="bb771-106">属性</span><span class="sxs-lookup"><span data-stu-id="bb771-106">Properties</span></span>

| <span data-ttu-id="bb771-107">属性</span><span class="sxs-lookup"><span data-stu-id="bb771-107">Property</span></span>     | <span data-ttu-id="bb771-108">类型</span><span class="sxs-lookup"><span data-stu-id="bb771-108">Type</span></span>        | <span data-ttu-id="bb771-109">说明</span><span class="sxs-lookup"><span data-stu-id="bb771-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="bb771-110">hitsContainers</span><span class="sxs-lookup"><span data-stu-id="bb771-110">hitsContainers</span></span>|<span data-ttu-id="bb771-111">[searchHitsContainer](searchhitscontainer.md) 集合</span><span class="sxs-lookup"><span data-stu-id="bb771-111">[searchHitsContainer](searchhitscontainer.md) collection</span></span>|<span data-ttu-id="bb771-112">搜索结果的集合。</span><span class="sxs-lookup"><span data-stu-id="bb771-112">A collection of search results.</span></span>|
|<span data-ttu-id="bb771-113">searchTerms</span><span class="sxs-lookup"><span data-stu-id="bb771-113">searchTerms</span></span>|<span data-ttu-id="bb771-114">String collection</span><span class="sxs-lookup"><span data-stu-id="bb771-114">String collection</span></span>|<span data-ttu-id="bb771-115">包含在初始搜索查询中发送的搜索词。</span><span class="sxs-lookup"><span data-stu-id="bb771-115">Contains the search terms sent in the initial search query.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bb771-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bb771-116">JSON representation</span></span>

<span data-ttu-id="bb771-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bb771-117">The following is a JSON representation of the resource.</span></span>

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

