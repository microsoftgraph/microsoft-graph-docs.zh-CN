---
title: searchQuery 资源类型
description: searchQuery
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 3cb46a41b0c46fe5f70d94a64a91489c9c2e7d43
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37936585"
---
# <a name="searchquery-resource-type"></a><span data-ttu-id="d4f2e-103">searchQuery 资源类型</span><span class="sxs-lookup"><span data-stu-id="d4f2e-103">searchQuery resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4f2e-104">表示包含搜索词和可选筛选器的搜索查询。</span><span class="sxs-lookup"><span data-stu-id="d4f2e-104">Represents a search query that contains search terms and optional filters.</span></span>

## <a name="properties"></a><span data-ttu-id="d4f2e-105">属性</span><span class="sxs-lookup"><span data-stu-id="d4f2e-105">Properties</span></span>

| <span data-ttu-id="d4f2e-106">属性</span><span class="sxs-lookup"><span data-stu-id="d4f2e-106">Property</span></span>     | <span data-ttu-id="d4f2e-107">类型</span><span class="sxs-lookup"><span data-stu-id="d4f2e-107">Type</span></span>        | <span data-ttu-id="d4f2e-108">描述</span><span class="sxs-lookup"><span data-stu-id="d4f2e-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d4f2e-109">query_string</span><span class="sxs-lookup"><span data-stu-id="d4f2e-109">query_string</span></span>|[<span data-ttu-id="d4f2e-110">searchQueryString</span><span class="sxs-lookup"><span data-stu-id="d4f2e-110">searchQueryString</span></span>](searchquerystring.md)|<span data-ttu-id="d4f2e-111">包含搜索词的搜索查询。</span><span class="sxs-lookup"><span data-stu-id="d4f2e-111">The search query containing the search terms.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d4f2e-112">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d4f2e-112">JSON representation</span></span>

<span data-ttu-id="d4f2e-113">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d4f2e-113">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchQuery",
  "baseType": null
}-->

```json
{
  "query_string": {"@odata.type": "microsoft.graph.searchQueryString"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchQuery resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->