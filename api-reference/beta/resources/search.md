---
title: 搜索
description: 检索用于执行查询的搜索资源
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: bb38d281895ac11d97a026a4352f68b93e8ba801
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/19/2019
ms.locfileid: "38704060"
---
# <a name="search-resource-type"></a><span data-ttu-id="d1d37-103">搜索资源类型</span><span class="sxs-lookup"><span data-stu-id="d1d37-103">search resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d1d37-104">搜索资源是表示搜索终结点的顶级对象。</span><span class="sxs-lookup"><span data-stu-id="d1d37-104">The search resource is the top level object representing the search endpoint.</span></span> <span data-ttu-id="d1d37-105">它充当[查询](../api/search-query.md)操作的定位。</span><span class="sxs-lookup"><span data-stu-id="d1d37-105">It serves as an anchor to the [query](../api/search-query.md) action.</span></span>

<span data-ttu-id="d1d37-106">此资源不应按此方式调用。</span><span class="sxs-lookup"><span data-stu-id="d1d37-106">This resource is not expected to be called as such.</span></span> <span data-ttu-id="d1d37-107">对资源的任何请求都将导致错误请求。</span><span class="sxs-lookup"><span data-stu-id="d1d37-107">Any request on the resource will incur a Bad Request.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="json-representation"></a><span data-ttu-id="d1d37-108">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d1d37-108">JSON representation</span></span>

<span data-ttu-id="d1d37-109">无</span><span class="sxs-lookup"><span data-stu-id="d1d37-109">None</span></span>

## <a name="properties"></a><span data-ttu-id="d1d37-110">属性</span><span class="sxs-lookup"><span data-stu-id="d1d37-110">Properties</span></span>

<span data-ttu-id="d1d37-111">无</span><span class="sxs-lookup"><span data-stu-id="d1d37-111">None</span></span>

## <a name="relationships"></a><span data-ttu-id="d1d37-112">关系</span><span class="sxs-lookup"><span data-stu-id="d1d37-112">Relationships</span></span>

<span data-ttu-id="d1d37-113">无</span><span class="sxs-lookup"><span data-stu-id="d1d37-113">None</span></span>

## <a name="methods"></a><span data-ttu-id="d1d37-114">方法</span><span class="sxs-lookup"><span data-stu-id="d1d37-114">Methods</span></span>

| <span data-ttu-id="d1d37-115">方法</span><span class="sxs-lookup"><span data-stu-id="d1d37-115">Method</span></span>       | <span data-ttu-id="d1d37-116">返回类型</span><span class="sxs-lookup"><span data-stu-id="d1d37-116">Return Type</span></span> | <span data-ttu-id="d1d37-117">说明</span><span class="sxs-lookup"><span data-stu-id="d1d37-117">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="d1d37-118">查询</span><span class="sxs-lookup"><span data-stu-id="d1d37-118">query</span></span>](../api/search-query.md) | <span data-ttu-id="d1d37-119">[searchResponse](searchresponse.md)组</span><span class="sxs-lookup"><span data-stu-id="d1d37-119">[searchResponse](searchresponse.md) Collection</span></span>| <span data-ttu-id="d1d37-120">执行[searchRequest](../resources/searchrequest.md)中指定的查询</span><span class="sxs-lookup"><span data-stu-id="d1d37-120">Executes the query specified in the [searchRequest](../resources/searchrequest.md)</span></span> |

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get search",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
