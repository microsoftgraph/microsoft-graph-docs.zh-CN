---
title: 搜索
description: 检索用于执行查询的搜索资源
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: d7b84fdad96530f88f09c7da7b00a6013b19017e
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938384"
---
# <a name="search"></a><span data-ttu-id="e3b8b-103">搜索</span><span class="sxs-lookup"><span data-stu-id="e3b8b-103">Search</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e3b8b-104">搜索资源是表示搜索终结点的顶级对象。</span><span class="sxs-lookup"><span data-stu-id="e3b8b-104">The search resource is the top level object representing the search endpoint.</span></span> <span data-ttu-id="e3b8b-105">它不像 Graph 中的任何其他资源一样工作，而是用作搜索操作（查询）的定位。</span><span class="sxs-lookup"><span data-stu-id="e3b8b-105">It does not behave as any other resource in Graph, but serves as an anchor to Search actions (Query).</span></span> <span data-ttu-id="e3b8b-106">图表中没有资源表示形式。</span><span class="sxs-lookup"><span data-stu-id="e3b8b-106">It has no resource representation in graph.</span></span>

## <a name="permissions"></a><span data-ttu-id="e3b8b-107">权限</span><span class="sxs-lookup"><span data-stu-id="e3b8b-107">Permissions</span></span>

<span data-ttu-id="e3b8b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e3b8b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e3b8b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e3b8b-110">Permission type</span></span>                        | <span data-ttu-id="e3b8b-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e3b8b-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e3b8b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e3b8b-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="e3b8b-113">阅读文章、文件、读取、ExternalItem、阅读、全部</span><span class="sxs-lookup"><span data-stu-id="e3b8b-113">Mail.Read, Files.Read.All, Calendars.Read, ExternalItem.Read.All</span></span> |
| <span data-ttu-id="e3b8b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e3b8b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e3b8b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e3b8b-115">Not supported.</span></span> |
| <span data-ttu-id="e3b8b-116">Application</span><span class="sxs-lookup"><span data-stu-id="e3b8b-116">Application</span></span>                            | <span data-ttu-id="e3b8b-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="e3b8b-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e3b8b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e3b8b-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /search
```

## <a name="request-headers"></a><span data-ttu-id="e3b8b-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="e3b8b-119">Request headers</span></span>

| <span data-ttu-id="e3b8b-120">名称</span><span class="sxs-lookup"><span data-stu-id="e3b8b-120">Name</span></span>      |<span data-ttu-id="e3b8b-121">说明</span><span class="sxs-lookup"><span data-stu-id="e3b8b-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e3b8b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3b8b-122">Authorization</span></span> | <span data-ttu-id="e3b8b-123">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="e3b8b-123">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="e3b8b-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="e3b8b-124">Request body</span></span>

<span data-ttu-id="e3b8b-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e3b8b-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e3b8b-126">响应</span><span class="sxs-lookup"><span data-stu-id="e3b8b-126">Response</span></span>

<span data-ttu-id="e3b8b-127">此资源不应按此方式调用。</span><span class="sxs-lookup"><span data-stu-id="e3b8b-127">This resource is not expected to be called as such.</span></span> <span data-ttu-id="e3b8b-128">对资源的任何请求都将导致错误请求。</span><span class="sxs-lookup"><span data-stu-id="e3b8b-128">Any request on the resource will incur a Bad Request.</span></span>

## <a name="next-steps"></a><span data-ttu-id="e3b8b-129">后续步骤</span><span class="sxs-lookup"><span data-stu-id="e3b8b-129">Next steps</span></span>

- <span data-ttu-id="e3b8b-130">在搜索时浏览[/query](search-query.md)操作。</span><span class="sxs-lookup"><span data-stu-id="e3b8b-130">Explore the [/query](search-query.md) action on Search.</span></span>


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get search",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
