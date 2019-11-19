---
title: searchQueryString 资源类型
description: searchQueryString
localization_priority: Normal
author: nmoreau
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 59809860bd2d0954ee8323f9c8e4fe982fb4faa7
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/19/2019
ms.locfileid: "38703824"
---
# <a name="searchquerystring-resource-type"></a><span data-ttu-id="324cc-103">searchQueryString 资源类型</span><span class="sxs-lookup"><span data-stu-id="324cc-103">searchQueryString resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="324cc-104">查询的搜索词。</span><span class="sxs-lookup"><span data-stu-id="324cc-104">The search terms for the query.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="324cc-105">属性</span><span class="sxs-lookup"><span data-stu-id="324cc-105">Properties</span></span>

| <span data-ttu-id="324cc-106">属性</span><span class="sxs-lookup"><span data-stu-id="324cc-106">Property</span></span>     | <span data-ttu-id="324cc-107">类型</span><span class="sxs-lookup"><span data-stu-id="324cc-107">Type</span></span>        | <span data-ttu-id="324cc-108">说明</span><span class="sxs-lookup"><span data-stu-id="324cc-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="324cc-109">查询</span><span class="sxs-lookup"><span data-stu-id="324cc-109">query</span></span>|<span data-ttu-id="324cc-110">String</span><span class="sxs-lookup"><span data-stu-id="324cc-110">String</span></span>|<span data-ttu-id="324cc-111">包含请求的实际搜索词。</span><span class="sxs-lookup"><span data-stu-id="324cc-111">Contains the actual search terms of the request.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="324cc-112">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="324cc-112">JSON representation</span></span>

<span data-ttu-id="324cc-113">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="324cc-113">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchQueryString",
  "baseType": null
}-->

```json
{
  "query": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchQueryString resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->