---
title: searchResponse 资源类型
description: 在此处提供说明
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 7e68eae7c31486646c4b3d135881fd04fa8c7222
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938756"
---
# <a name="searchresponse-resource-type"></a><span data-ttu-id="23261-103">searchResponse 资源类型</span><span class="sxs-lookup"><span data-stu-id="23261-103">searchResponse resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="23261-104">SearchResponse 包含搜索查询中的结果。</span><span class="sxs-lookup"><span data-stu-id="23261-104">The searchResponse contains the results from the search query.</span></span>

## <a name="properties"></a><span data-ttu-id="23261-105">属性</span><span class="sxs-lookup"><span data-stu-id="23261-105">Properties</span></span>

| <span data-ttu-id="23261-106">属性</span><span class="sxs-lookup"><span data-stu-id="23261-106">Property</span></span>     | <span data-ttu-id="23261-107">类型</span><span class="sxs-lookup"><span data-stu-id="23261-107">Type</span></span>        | <span data-ttu-id="23261-108">描述</span><span class="sxs-lookup"><span data-stu-id="23261-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="23261-109">hitsContainers</span><span class="sxs-lookup"><span data-stu-id="23261-109">hitsContainers</span></span>|<span data-ttu-id="23261-110">[searchHitsContainer](searchhitscontainer.md)集合</span><span class="sxs-lookup"><span data-stu-id="23261-110">[searchHitsContainer](searchhitscontainer.md) collection</span></span>|<span data-ttu-id="23261-111">搜索结果的集合。</span><span class="sxs-lookup"><span data-stu-id="23261-111">A collection of search results.</span></span>|
|<span data-ttu-id="23261-112">searchTerms</span><span class="sxs-lookup"><span data-stu-id="23261-112">searchTerms</span></span>|<span data-ttu-id="23261-113">String collection</span><span class="sxs-lookup"><span data-stu-id="23261-113">String collection</span></span>|<span data-ttu-id="23261-114">包含在初始搜索查询中发送的搜索词。</span><span class="sxs-lookup"><span data-stu-id="23261-114">Contains the search terms sent in the initial search query.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="23261-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="23261-115">JSON representation</span></span>

<span data-ttu-id="23261-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="23261-116">The following is a JSON representation of the resource.</span></span>

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