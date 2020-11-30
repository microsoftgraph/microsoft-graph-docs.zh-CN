---
title: 搜索
description: 检索用于执行查询的搜索资源
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 8e9d8bc133a050701543f2a978e56b662bafcc33
ms.sourcegitcommit: 5345c2f3265ede107fa0faaff7a3f1c2afee3810
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/21/2020
ms.locfileid: "49377976"
---
# <a name="search-resource-type"></a><span data-ttu-id="46444-103">搜索资源类型</span><span class="sxs-lookup"><span data-stu-id="46444-103">search resource type</span></span>

<span data-ttu-id="46444-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="46444-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="46444-105">搜索资源是表示搜索终结点的顶级对象。</span><span class="sxs-lookup"><span data-stu-id="46444-105">The search resource is the top level object representing the search endpoint.</span></span> <span data-ttu-id="46444-106">它充当 [查询](../api/search-query.md) 操作的定位。</span><span class="sxs-lookup"><span data-stu-id="46444-106">It serves as an anchor to the [query](../api/search-query.md) action.</span></span>

<span data-ttu-id="46444-107">此资源不应按此方式调用。</span><span class="sxs-lookup"><span data-stu-id="46444-107">This resource is not expected to be called as such.</span></span> <span data-ttu-id="46444-108">对资源的任何请求都将导致错误请求。</span><span class="sxs-lookup"><span data-stu-id="46444-108">Any request on the resource will incur a Bad Request.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="json-representation"></a><span data-ttu-id="46444-109">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="46444-109">JSON representation</span></span>

<span data-ttu-id="46444-110">无</span><span class="sxs-lookup"><span data-stu-id="46444-110">None</span></span>

## <a name="properties"></a><span data-ttu-id="46444-111">属性</span><span class="sxs-lookup"><span data-stu-id="46444-111">Properties</span></span>

<span data-ttu-id="46444-112">无</span><span class="sxs-lookup"><span data-stu-id="46444-112">None</span></span>

## <a name="relationships"></a><span data-ttu-id="46444-113">关系</span><span class="sxs-lookup"><span data-stu-id="46444-113">Relationships</span></span>

<span data-ttu-id="46444-114">无</span><span class="sxs-lookup"><span data-stu-id="46444-114">None</span></span>

## <a name="methods"></a><span data-ttu-id="46444-115">方法</span><span class="sxs-lookup"><span data-stu-id="46444-115">Methods</span></span>

| <span data-ttu-id="46444-116">方法</span><span class="sxs-lookup"><span data-stu-id="46444-116">Method</span></span>       | <span data-ttu-id="46444-117">返回类型</span><span class="sxs-lookup"><span data-stu-id="46444-117">Return Type</span></span> | <span data-ttu-id="46444-118">说明</span><span class="sxs-lookup"><span data-stu-id="46444-118">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="46444-119">查询</span><span class="sxs-lookup"><span data-stu-id="46444-119">query</span></span>](../api/search-query.md) | <span data-ttu-id="46444-120">[searchResponse](searchresponse.md) 组</span><span class="sxs-lookup"><span data-stu-id="46444-120">[searchResponse](searchresponse.md) Collection</span></span>| <span data-ttu-id="46444-121">执行[searchRequest](../resources/searchrequest.md)中指定的查询</span><span class="sxs-lookup"><span data-stu-id="46444-121">Executes the query specified in the [searchRequest](../resources/searchrequest.md)</span></span> |

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get search",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


