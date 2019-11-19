---
title: searchQuery 资源类型
description: searchQuery
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: e9501831ef2e83d23aa4a5587b9afd8eaa7f5ee8
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/19/2019
ms.locfileid: "38703903"
---
# <a name="searchquery-resource-type"></a><span data-ttu-id="00b8e-103">searchQuery 资源类型</span><span class="sxs-lookup"><span data-stu-id="00b8e-103">searchQuery resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="00b8e-104">表示包含搜索词和可选筛选器的搜索查询。</span><span class="sxs-lookup"><span data-stu-id="00b8e-104">Represents a search query that contains search terms and optional filters.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="00b8e-105">属性</span><span class="sxs-lookup"><span data-stu-id="00b8e-105">Properties</span></span>

| <span data-ttu-id="00b8e-106">属性</span><span class="sxs-lookup"><span data-stu-id="00b8e-106">Property</span></span>     | <span data-ttu-id="00b8e-107">类型</span><span class="sxs-lookup"><span data-stu-id="00b8e-107">Type</span></span>        | <span data-ttu-id="00b8e-108">说明</span><span class="sxs-lookup"><span data-stu-id="00b8e-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="00b8e-109">query_string</span><span class="sxs-lookup"><span data-stu-id="00b8e-109">query_string</span></span>|[<span data-ttu-id="00b8e-110">searchQueryString</span><span class="sxs-lookup"><span data-stu-id="00b8e-110">searchQueryString</span></span>](searchquerystring.md)|<span data-ttu-id="00b8e-111">包含搜索词的搜索查询。</span><span class="sxs-lookup"><span data-stu-id="00b8e-111">The search query containing the search terms.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="00b8e-112">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="00b8e-112">JSON representation</span></span>

<span data-ttu-id="00b8e-113">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="00b8e-113">The following is a JSON representation of the resource.</span></span>

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