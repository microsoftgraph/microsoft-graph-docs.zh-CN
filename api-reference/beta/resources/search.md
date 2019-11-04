---
title: 搜索
description: 检索用于执行查询的搜索资源
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 65a099ea0ae57b116bcf6a251170e507945226c9
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938770"
---
# <a name="search-resource-type"></a><span data-ttu-id="be180-103">搜索资源类型</span><span class="sxs-lookup"><span data-stu-id="be180-103">search resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="be180-104">搜索资源是表示搜索终结点的顶级对象。</span><span class="sxs-lookup"><span data-stu-id="be180-104">The search resource is the top level object representing the search endpoint.</span></span> <span data-ttu-id="be180-105">它充当[查询](../api/search-query.md)操作的定位。</span><span class="sxs-lookup"><span data-stu-id="be180-105">It serves as an anchor to the [query](../api/search-query.md) action.</span></span>

<span data-ttu-id="be180-106">此资源不应按此方式调用。</span><span class="sxs-lookup"><span data-stu-id="be180-106">This resource is not expected to be called as such.</span></span> <span data-ttu-id="be180-107">对资源的任何请求都将导致错误请求。</span><span class="sxs-lookup"><span data-stu-id="be180-107">Any request on the resource will incur a Bad Request.</span></span>

## <a name="json-representation"></a><span data-ttu-id="be180-108">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="be180-108">JSON representation</span></span>

<span data-ttu-id="be180-109">无</span><span class="sxs-lookup"><span data-stu-id="be180-109">None</span></span>

## <a name="properties"></a><span data-ttu-id="be180-110">属性</span><span class="sxs-lookup"><span data-stu-id="be180-110">Properties</span></span>

<span data-ttu-id="be180-111">无</span><span class="sxs-lookup"><span data-stu-id="be180-111">None</span></span>

## <a name="relationships"></a><span data-ttu-id="be180-112">关系</span><span class="sxs-lookup"><span data-stu-id="be180-112">Relationships</span></span>

<span data-ttu-id="be180-113">无</span><span class="sxs-lookup"><span data-stu-id="be180-113">None</span></span>

## <a name="methods"></a><span data-ttu-id="be180-114">方法</span><span class="sxs-lookup"><span data-stu-id="be180-114">Methods</span></span>

| <span data-ttu-id="be180-115">方法</span><span class="sxs-lookup"><span data-stu-id="be180-115">Method</span></span>       | <span data-ttu-id="be180-116">返回类型</span><span class="sxs-lookup"><span data-stu-id="be180-116">Return Type</span></span> | <span data-ttu-id="be180-117">说明</span><span class="sxs-lookup"><span data-stu-id="be180-117">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="be180-118">query</span><span class="sxs-lookup"><span data-stu-id="be180-118">query</span></span>](../api/search-query.md) | <span data-ttu-id="be180-119">[searchResponse](searchresponse.md)组</span><span class="sxs-lookup"><span data-stu-id="be180-119">[searchResponse](searchresponse.md) Collection</span></span>| <span data-ttu-id="be180-120">执行[searchRequest](../resources/searchrequest.md)中指定的查询</span><span class="sxs-lookup"><span data-stu-id="be180-120">Executes the query specified in the [searchRequest](../resources/searchrequest.md)</span></span> |

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get search",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
