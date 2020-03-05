---
title: searchQuery 资源类型
description: searchQuery
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: b5c46353d0533fb2c032765527ed5ccf7107e1b3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520912"
---
# <a name="searchquery-resource-type"></a><span data-ttu-id="39f2f-103">searchQuery 资源类型</span><span class="sxs-lookup"><span data-stu-id="39f2f-103">searchQuery resource type</span></span>

<span data-ttu-id="39f2f-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="39f2f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="39f2f-105">表示包含搜索词和可选筛选器的搜索查询。</span><span class="sxs-lookup"><span data-stu-id="39f2f-105">Represents a search query that contains search terms and optional filters.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="39f2f-106">属性</span><span class="sxs-lookup"><span data-stu-id="39f2f-106">Properties</span></span>

| <span data-ttu-id="39f2f-107">属性</span><span class="sxs-lookup"><span data-stu-id="39f2f-107">Property</span></span>     | <span data-ttu-id="39f2f-108">类型</span><span class="sxs-lookup"><span data-stu-id="39f2f-108">Type</span></span>        | <span data-ttu-id="39f2f-109">说明</span><span class="sxs-lookup"><span data-stu-id="39f2f-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="39f2f-110">query_string</span><span class="sxs-lookup"><span data-stu-id="39f2f-110">query_string</span></span>|[<span data-ttu-id="39f2f-111">searchQueryString</span><span class="sxs-lookup"><span data-stu-id="39f2f-111">searchQueryString</span></span>](searchquerystring.md)|<span data-ttu-id="39f2f-112">包含搜索词的搜索查询。</span><span class="sxs-lookup"><span data-stu-id="39f2f-112">The search query containing the search terms.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="39f2f-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="39f2f-113">JSON representation</span></span>

<span data-ttu-id="39f2f-114">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="39f2f-114">The following is a JSON representation of the resource.</span></span>

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