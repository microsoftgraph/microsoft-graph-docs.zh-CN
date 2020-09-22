---
title: searchEntity 资源类型
description: 一个顶级对象，表示 Microsoft 搜索 API 终结点。
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: cb6d5bdd5288a3f6098f33d3432a0e4f0d7ac8bd
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193862"
---
# <a name="searchentity-resource-type"></a><span data-ttu-id="d7ca9-103">searchEntity 资源类型</span><span class="sxs-lookup"><span data-stu-id="d7ca9-103">searchEntity resource type</span></span>

<span data-ttu-id="d7ca9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d7ca9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d7ca9-105">一个顶级对象，表示 Microsoft 搜索 API 终结点。</span><span class="sxs-lookup"><span data-stu-id="d7ca9-105">A top level object representing the Microsoft Search API endpoint.</span></span> <span data-ttu-id="d7ca9-106">它不像 Graph 中的任何其他资源一样工作，而是用作 [查询](../api/search-query.md) 操作的定位。</span><span class="sxs-lookup"><span data-stu-id="d7ca9-106">It does not behave as any other resource in Graph, but serves as an anchor to the [query](../api/search-query.md) action.</span></span> 

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a><span data-ttu-id="d7ca9-107">方法</span><span class="sxs-lookup"><span data-stu-id="d7ca9-107">Methods</span></span>
|<span data-ttu-id="d7ca9-108">方法</span><span class="sxs-lookup"><span data-stu-id="d7ca9-108">Method</span></span>|<span data-ttu-id="d7ca9-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="d7ca9-109">Return type</span></span>|<span data-ttu-id="d7ca9-110">说明</span><span class="sxs-lookup"><span data-stu-id="d7ca9-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d7ca9-111">查询</span><span class="sxs-lookup"><span data-stu-id="d7ca9-111">query</span></span>](../api/search-query.md) |<span data-ttu-id="d7ca9-112">[searchResponse](searchresponse.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d7ca9-112">[searchResponse](searchresponse.md) collection</span></span> | <span data-ttu-id="d7ca9-113">运行请求正文中指定的查询。</span><span class="sxs-lookup"><span data-stu-id="d7ca9-113">Runs the query specified in the request body.</span></span>  |

## <a name="properties"></a><span data-ttu-id="d7ca9-114">属性</span><span class="sxs-lookup"><span data-stu-id="d7ca9-114">Properties</span></span>
<span data-ttu-id="d7ca9-115">无。</span><span class="sxs-lookup"><span data-stu-id="d7ca9-115">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="d7ca9-116">关系</span><span class="sxs-lookup"><span data-stu-id="d7ca9-116">Relationships</span></span>
<span data-ttu-id="d7ca9-117">无。</span><span class="sxs-lookup"><span data-stu-id="d7ca9-117">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d7ca9-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d7ca9-118">JSON representation</span></span>
<span data-ttu-id="d7ca9-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d7ca9-119">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.searchEntity",
  "baseType": "microsoft.graph.entity"
}
-->
``` json
{
  
}
```


## <a name="next-steps"></a><span data-ttu-id="d7ca9-120">后续步骤</span><span class="sxs-lookup"><span data-stu-id="d7ca9-120">Next steps</span></span>

<span data-ttu-id="d7ca9-121">探索 [查询](../api/search-query.md) 操作。</span><span class="sxs-lookup"><span data-stu-id="d7ca9-121">Explore the [query](../api/search-query.md) action.</span></span>


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "A top level object representing the Microsoft Search API endpoint.",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


