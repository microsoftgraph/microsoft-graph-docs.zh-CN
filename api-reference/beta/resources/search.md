---
title: 搜索
description: 检索用于执行查询的搜索资源
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: a30a1fe5891a0f8a58f08d742ef2aac645006156
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47985784"
---
# <a name="search-resource-type"></a><span data-ttu-id="bb096-103">搜索资源类型</span><span class="sxs-lookup"><span data-stu-id="bb096-103">search resource type</span></span>

<span data-ttu-id="bb096-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb096-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bb096-105">搜索资源是表示搜索终结点的顶级对象。</span><span class="sxs-lookup"><span data-stu-id="bb096-105">The search resource is the top level object representing the search endpoint.</span></span> <span data-ttu-id="bb096-106">它充当 [查询](../api/search-query.md) 操作的定位。</span><span class="sxs-lookup"><span data-stu-id="bb096-106">It serves as an anchor to the [query](../api/search-query.md) action.</span></span>

<span data-ttu-id="bb096-107">此资源不应按此方式调用。</span><span class="sxs-lookup"><span data-stu-id="bb096-107">This resource is not expected to be called as such.</span></span> <span data-ttu-id="bb096-108">对资源的任何请求都将导致错误请求。</span><span class="sxs-lookup"><span data-stu-id="bb096-108">Any request on the resource will incur a Bad Request.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="json-representation"></a><span data-ttu-id="bb096-109">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bb096-109">JSON representation</span></span>

<span data-ttu-id="bb096-110">无</span><span class="sxs-lookup"><span data-stu-id="bb096-110">None</span></span>

## <a name="properties"></a><span data-ttu-id="bb096-111">属性</span><span class="sxs-lookup"><span data-stu-id="bb096-111">Properties</span></span>

<span data-ttu-id="bb096-112">无</span><span class="sxs-lookup"><span data-stu-id="bb096-112">None</span></span>

## <a name="relationships"></a><span data-ttu-id="bb096-113">关系</span><span class="sxs-lookup"><span data-stu-id="bb096-113">Relationships</span></span>

<span data-ttu-id="bb096-114">无</span><span class="sxs-lookup"><span data-stu-id="bb096-114">None</span></span>

## <a name="methods"></a><span data-ttu-id="bb096-115">方法</span><span class="sxs-lookup"><span data-stu-id="bb096-115">Methods</span></span>

| <span data-ttu-id="bb096-116">方法</span><span class="sxs-lookup"><span data-stu-id="bb096-116">Method</span></span>       | <span data-ttu-id="bb096-117">返回类型</span><span class="sxs-lookup"><span data-stu-id="bb096-117">Return Type</span></span> | <span data-ttu-id="bb096-118">说明</span><span class="sxs-lookup"><span data-stu-id="bb096-118">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="bb096-119">查询</span><span class="sxs-lookup"><span data-stu-id="bb096-119">query</span></span>](../api/search-query.md) | <span data-ttu-id="bb096-120">[searchResponse](searchresponse.md) 组</span><span class="sxs-lookup"><span data-stu-id="bb096-120">[searchResponse](searchresponse.md) Collection</span></span>| <span data-ttu-id="bb096-121">执行[searchRequest](../resources/searchrequest.md)中指定的查询</span><span class="sxs-lookup"><span data-stu-id="bb096-121">Executes the query specified in the [searchRequest](../resources/searchrequest.md)</span></span> |

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get search",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


