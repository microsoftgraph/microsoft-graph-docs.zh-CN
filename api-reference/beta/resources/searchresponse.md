---
title: searchResponse 资源类型
description: searchResponse 的说明
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 5778d82c0c4718b9f34c686a613270eebfcc56e1
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067087"
---
# <a name="searchresponse-resource-type"></a><span data-ttu-id="39b23-103">searchResponse 资源类型</span><span class="sxs-lookup"><span data-stu-id="39b23-103">searchResponse resource type</span></span>

<span data-ttu-id="39b23-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="39b23-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="39b23-105">表示来自搜索查询的响应。</span><span class="sxs-lookup"><span data-stu-id="39b23-105">Represents the response from a search query.</span></span> 

## <a name="properties"></a><span data-ttu-id="39b23-106">属性</span><span class="sxs-lookup"><span data-stu-id="39b23-106">Properties</span></span>

| <span data-ttu-id="39b23-107">属性</span><span class="sxs-lookup"><span data-stu-id="39b23-107">Property</span></span>     | <span data-ttu-id="39b23-108">类型</span><span class="sxs-lookup"><span data-stu-id="39b23-108">Type</span></span>        | <span data-ttu-id="39b23-109">说明</span><span class="sxs-lookup"><span data-stu-id="39b23-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="39b23-110">queryAlterationResponse</span><span class="sxs-lookup"><span data-stu-id="39b23-110">queryAlterationResponse</span></span>|[<span data-ttu-id="39b23-111">更改response</span><span class="sxs-lookup"><span data-stu-id="39b23-111">alterationResponse</span></span>](alterationResponse.md)|<span data-ttu-id="39b23-112">提供用于拼写更正的查询更改响应的详细信息。</span><span class="sxs-lookup"><span data-stu-id="39b23-112">Provides details of query alteration response for spelling correction.</span></span>|
|<span data-ttu-id="39b23-113">值</span><span class="sxs-lookup"><span data-stu-id="39b23-113">value</span></span>|<span data-ttu-id="39b23-114">[searchResultSet](searchResultSet.md) 集合</span><span class="sxs-lookup"><span data-stu-id="39b23-114">[searchResultSet](searchResultSet.md) collection</span></span>|<span data-ttu-id="39b23-115">表示来自搜索查询的结果，以及用于查询的术语。</span><span class="sxs-lookup"><span data-stu-id="39b23-115">Represents results from a search query, and the terms used for the query.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="39b23-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="39b23-116">JSON representation</span></span>

<span data-ttu-id="39b23-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="39b23-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchResponse",
  "baseType": null
}-->

```json
{
  "queryAlterationResponse": {"@odata.type": "microsoft.graph.alterationResponse"},
  "value": [{"@odata.type": "microsoft.graph.searchResultSet"}]
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

