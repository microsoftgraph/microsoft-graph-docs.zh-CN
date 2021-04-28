---
title: 搜索
description: 检索用于执行查询的搜索资源
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 123d57b05950203434ac23fd85e9c29dfa41476d
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067094"
---
# <a name="search-resource-type"></a><span data-ttu-id="5976c-103">搜索资源类型</span><span class="sxs-lookup"><span data-stu-id="5976c-103">search resource type</span></span>

<span data-ttu-id="5976c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5976c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5976c-105">搜索资源是表示搜索终结点的顶级对象。</span><span class="sxs-lookup"><span data-stu-id="5976c-105">The search resource is the top level object representing the search endpoint.</span></span> <span data-ttu-id="5976c-106">它充当查询操作 [锚点](../api/search-query.md) 。</span><span class="sxs-lookup"><span data-stu-id="5976c-106">It serves as an anchor to the [query](../api/search-query.md) action.</span></span>

<span data-ttu-id="5976c-107">不应这样调用此资源。</span><span class="sxs-lookup"><span data-stu-id="5976c-107">This resource is not expected to be called as such.</span></span> <span data-ttu-id="5976c-108">资源上的任何请求都会导致错误的请求。</span><span class="sxs-lookup"><span data-stu-id="5976c-108">Any request on the resource will incur a Bad Request.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="json-representation"></a><span data-ttu-id="5976c-109">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5976c-109">JSON representation</span></span>

<span data-ttu-id="5976c-110">无</span><span class="sxs-lookup"><span data-stu-id="5976c-110">None</span></span>

## <a name="properties"></a><span data-ttu-id="5976c-111">属性</span><span class="sxs-lookup"><span data-stu-id="5976c-111">Properties</span></span>

<span data-ttu-id="5976c-112">无</span><span class="sxs-lookup"><span data-stu-id="5976c-112">None</span></span>

## <a name="relationships"></a><span data-ttu-id="5976c-113">关系</span><span class="sxs-lookup"><span data-stu-id="5976c-113">Relationships</span></span>

<span data-ttu-id="5976c-114">无</span><span class="sxs-lookup"><span data-stu-id="5976c-114">None</span></span>

## <a name="methods"></a><span data-ttu-id="5976c-115">方法</span><span class="sxs-lookup"><span data-stu-id="5976c-115">Methods</span></span>

| <span data-ttu-id="5976c-116">方法</span><span class="sxs-lookup"><span data-stu-id="5976c-116">Method</span></span>       | <span data-ttu-id="5976c-117">返回类型</span><span class="sxs-lookup"><span data-stu-id="5976c-117">Return Type</span></span> | <span data-ttu-id="5976c-118">说明</span><span class="sxs-lookup"><span data-stu-id="5976c-118">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="5976c-119">查询</span><span class="sxs-lookup"><span data-stu-id="5976c-119">query</span></span>](../api/search-query.md) | [<span data-ttu-id="5976c-120">searchResponse</span><span class="sxs-lookup"><span data-stu-id="5976c-120">searchResponse</span></span>](searchresponse.md)| <span data-ttu-id="5976c-121">执行 [searchRequest 中指定的查询](../resources/searchrequest.md)</span><span class="sxs-lookup"><span data-stu-id="5976c-121">Executes the query specified in the [searchRequest](../resources/searchrequest.md)</span></span> |

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get search",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


