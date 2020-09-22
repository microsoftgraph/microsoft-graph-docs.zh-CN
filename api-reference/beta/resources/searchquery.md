---
title: searchQuery 资源类型
description: searchQuery
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 1d2d643fed135f97f1ccf2c6346d8fdd6e22f8b5
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193363"
---
# <a name="searchquery-resource-type"></a><span data-ttu-id="8b108-103">searchQuery 资源类型</span><span class="sxs-lookup"><span data-stu-id="8b108-103">searchQuery resource type</span></span>

<span data-ttu-id="8b108-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8b108-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [search-api-deprecation](../../includes/search-api-deprecation.md)]

<span data-ttu-id="8b108-105">表示包含搜索词和可选筛选器的搜索查询。</span><span class="sxs-lookup"><span data-stu-id="8b108-105">Represents a search query that contains search terms and optional filters.</span></span>

## <a name="properties"></a><span data-ttu-id="8b108-106">属性</span><span class="sxs-lookup"><span data-stu-id="8b108-106">Properties</span></span>

| <span data-ttu-id="8b108-107">属性</span><span class="sxs-lookup"><span data-stu-id="8b108-107">Property</span></span>     | <span data-ttu-id="8b108-108">类型</span><span class="sxs-lookup"><span data-stu-id="8b108-108">Type</span></span>        | <span data-ttu-id="8b108-109">描述</span><span class="sxs-lookup"><span data-stu-id="8b108-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8b108-110">queryString</span><span class="sxs-lookup"><span data-stu-id="8b108-110">queryString</span></span>|<span data-ttu-id="8b108-111">字符串</span><span class="sxs-lookup"><span data-stu-id="8b108-111">String</span></span>|<span data-ttu-id="8b108-112">包含搜索词的搜索查询。</span><span class="sxs-lookup"><span data-stu-id="8b108-112">The search query containing the search terms.</span></span> <span data-ttu-id="8b108-113">必需。</span><span class="sxs-lookup"><span data-stu-id="8b108-113">Required.</span></span>|
|<span data-ttu-id="8b108-114">query_string (已弃用) </span><span class="sxs-lookup"><span data-stu-id="8b108-114">query_string (deprecated)</span></span>|[<span data-ttu-id="8b108-115">searchQueryString</span><span class="sxs-lookup"><span data-stu-id="8b108-115">searchQueryString</span></span>](searchquerystring.md)|<span data-ttu-id="8b108-116">现在，它将替换为 **queryString** 属性。</span><span class="sxs-lookup"><span data-stu-id="8b108-116">This is now replaced by the **queryString** property.</span></span> <span data-ttu-id="8b108-117">包含搜索词的搜索查询。</span><span class="sxs-lookup"><span data-stu-id="8b108-117">The search query containing the search terms.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="8b108-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8b108-118">JSON representation</span></span>

<span data-ttu-id="8b108-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8b108-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchQuery",
  "baseType": null
}-->

```json
{
  "queryString": "String",
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

