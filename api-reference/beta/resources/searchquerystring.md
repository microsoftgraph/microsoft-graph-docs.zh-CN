---
title: searchQueryString 资源类型
description: searchQueryString
localization_priority: Normal
author: nmoreau
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 93142dcc672c5fee18a5f98d0988352e6c02cbd0
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37935264"
---
# <a name="searchquerystring-resource-type"></a><span data-ttu-id="fb19b-103">searchQueryString 资源类型</span><span class="sxs-lookup"><span data-stu-id="fb19b-103">searchQueryString resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fb19b-104">查询的搜索词。</span><span class="sxs-lookup"><span data-stu-id="fb19b-104">The search terms for the query.</span></span>

## <a name="properties"></a><span data-ttu-id="fb19b-105">属性</span><span class="sxs-lookup"><span data-stu-id="fb19b-105">Properties</span></span>

| <span data-ttu-id="fb19b-106">属性</span><span class="sxs-lookup"><span data-stu-id="fb19b-106">Property</span></span>     | <span data-ttu-id="fb19b-107">类型</span><span class="sxs-lookup"><span data-stu-id="fb19b-107">Type</span></span>        | <span data-ttu-id="fb19b-108">描述</span><span class="sxs-lookup"><span data-stu-id="fb19b-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="fb19b-109">查询</span><span class="sxs-lookup"><span data-stu-id="fb19b-109">query</span></span>|<span data-ttu-id="fb19b-110">字符串</span><span class="sxs-lookup"><span data-stu-id="fb19b-110">String</span></span>|<span data-ttu-id="fb19b-111">包含请求的实际搜索词。</span><span class="sxs-lookup"><span data-stu-id="fb19b-111">Contains the actual search terms of the request.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fb19b-112">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fb19b-112">JSON representation</span></span>

<span data-ttu-id="fb19b-113">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fb19b-113">The following is a JSON representation of the resource.</span></span>

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