---
title: searchEntity： query
description: 运行请求正文中指定的查询。 搜索结果在响应中提供。
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: e877b1e126a353aae04a90500fdfe99cd4ec8342
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193316"
---
# <a name="searchentity-query"></a><span data-ttu-id="1c863-104">searchEntity： query</span><span class="sxs-lookup"><span data-stu-id="1c863-104">searchEntity: query</span></span>

<span data-ttu-id="1c863-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c863-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1c863-106">运行请求正文中指定的查询。</span><span class="sxs-lookup"><span data-stu-id="1c863-106">Runs the query specified in the request body.</span></span> <span data-ttu-id="1c863-107">搜索结果在响应中提供。</span><span class="sxs-lookup"><span data-stu-id="1c863-107">Search results are provided in the response.</span></span>

[!INCLUDE [search-api-deprecation](../../includes/search-api-deprecation.md)]

## <a name="permissions"></a><span data-ttu-id="1c863-108">权限</span><span class="sxs-lookup"><span data-stu-id="1c863-108">Permissions</span></span>

<span data-ttu-id="1c863-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1c863-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span> 

| <span data-ttu-id="1c863-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="1c863-111">Permission type</span></span>                        | <span data-ttu-id="1c863-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1c863-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1c863-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1c863-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="1c863-114">已读取的邮件。读取、读取、读取、ExternalItem、文件、读取、全部、读取、全部、全部、全部、读取、全部、全部、</span><span class="sxs-lookup"><span data-stu-id="1c863-114">Mail.Read, Mail.ReadWrite, Calendars.Read, Calendars.ReadWrite,Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All, ExternalItem.Read.All</span></span> |
| <span data-ttu-id="1c863-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1c863-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1c863-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1c863-116">Not supported.</span></span> |
| <span data-ttu-id="1c863-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="1c863-117">Application</span></span>                            | <span data-ttu-id="1c863-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="1c863-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1c863-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1c863-119">HTTP request</span></span>

```HTTP
POST /search/query
```

## <a name="request-headers"></a><span data-ttu-id="1c863-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="1c863-120">Request headers</span></span>

| <span data-ttu-id="1c863-121">名称</span><span class="sxs-lookup"><span data-stu-id="1c863-121">Name</span></span>          | <span data-ttu-id="1c863-122">说明</span><span class="sxs-lookup"><span data-stu-id="1c863-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="1c863-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1c863-123">Authorization</span></span> | <span data-ttu-id="1c863-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1c863-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1c863-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="1c863-126">Content-type</span></span> | <span data-ttu-id="1c863-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="1c863-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1c863-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="1c863-129">Request body</span></span>

<span data-ttu-id="1c863-130">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="1c863-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1c863-131">参数</span><span class="sxs-lookup"><span data-stu-id="1c863-131">Parameter</span></span>    | <span data-ttu-id="1c863-132">类型</span><span class="sxs-lookup"><span data-stu-id="1c863-132">Type</span></span>        | <span data-ttu-id="1c863-133">描述</span><span class="sxs-lookup"><span data-stu-id="1c863-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1c863-134">requests</span><span class="sxs-lookup"><span data-stu-id="1c863-134">requests</span></span>|<span data-ttu-id="1c863-135">[searchRequest](../resources/searchrequest.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1c863-135">[searchRequest](../resources/searchrequest.md) collection</span></span>|<span data-ttu-id="1c863-136">一个或多个在 JSON blob 中格式化的搜索请求的集合。</span><span class="sxs-lookup"><span data-stu-id="1c863-136">A collection of one or more search requests each formatted in a JSON blob.</span></span> <span data-ttu-id="1c863-137">每个 JSON blob 都包含响应中预期的资源类型、基础源、分页参数、请求的字段和实际搜索查询。</span><span class="sxs-lookup"><span data-stu-id="1c863-137">Each JSON blob contains the types of resources expected in the response, the underlying sources, paging parameters, requested fields, and actual search query.</span></span> <br> <span data-ttu-id="1c863-138">了解有关搜索实体类型的特定组合以及对搜索结果进行排序或聚合的 [已知限制](../resources/search-api-overview.md#known-limitations) 。</span><span class="sxs-lookup"><span data-stu-id="1c863-138">Be aware of [known limitations](../resources/search-api-overview.md#known-limitations) on searching specific combinations of entity types, and sorting or aggregating search results.</span></span> |

## <a name="response"></a><span data-ttu-id="1c863-139">响应</span><span class="sxs-lookup"><span data-stu-id="1c863-139">Response</span></span>

<span data-ttu-id="1c863-140">如果成功，此方法 `HTTP 200 OK` 在响应正文中返回响应代码和 [searchResponse](../resources/searchresponse.md) 集合对象。</span><span class="sxs-lookup"><span data-stu-id="1c863-140">If successful, this method returns `HTTP 200 OK` response code and a [searchResponse](../resources/searchresponse.md) collection object in the response body.</span></span>
 

## <a name="examples"></a><span data-ttu-id="1c863-141">示例</span><span class="sxs-lookup"><span data-stu-id="1c863-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1c863-142">请求</span><span class="sxs-lookup"><span data-stu-id="1c863-142">Request</span></span>

<span data-ttu-id="1c863-143">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1c863-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1c863-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="1c863-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "search_query"
}-->

```HTTP
POST https://graph.microsoft.com/beta/search/query
Content-type: application/json

{
  "requests": [
    {
      "entityTypes": [
        "externalItem"
      ],
      "contentSources": [
        "/external/connections/connectionfriendlyname"
      ],
      "query": {
        "queryString": "contoso product"
      },
      "from": 0,
      "size": 25,
      "fields": [
        "title",
        "description"
      ]
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="1c863-145">C#</span><span class="sxs-lookup"><span data-stu-id="1c863-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/search-query-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1c863-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1c863-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/search-query-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1c863-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1c863-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/search-query-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1c863-148">响应</span><span class="sxs-lookup"><span data-stu-id="1c863-148">Response</span></span>

<span data-ttu-id="1c863-149">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1c863-149">The following is an example of the response.</span></span>

> <span data-ttu-id="1c863-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="1c863-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.searchResponse",
  "isCollection": true
} -->

```HTTP
HTTP/1.1 200 OK
Content-type: application/json
```

```json
{
  "value": [
    {
      "searchTerms": [
        "searchTerms-value"
      ],
      "hitsContainers": [
        {
          "hits": [
            {
              "hitId": "1",
              "rank": 1,
              "summary": "_summary-value",
              "resource": "The source field will contain the underlying graph entity part of the response"
            }
          ],
          "total": 47,
          "moreResultsAvailable": true
        }
      ]
    }
  ]
}
```

## <a name="see-also"></a><span data-ttu-id="1c863-152">另请参阅</span><span class="sxs-lookup"><span data-stu-id="1c863-152">See also</span></span>
- <span data-ttu-id="1c863-153">搜索 [邮件消息](/graph/search-concept-messages)</span><span class="sxs-lookup"><span data-stu-id="1c863-153">Search [mail messages](/graph/search-concept-messages)</span></span>
- <span data-ttu-id="1c863-154">搜索 [日历事件](/graph/search-concept-events)</span><span class="sxs-lookup"><span data-stu-id="1c863-154">Search [calendar events](/graph/search-concept-events)</span></span>
- <span data-ttu-id="1c863-155">在 SharePoint 和 OneDrive 中搜索内容 ([文件、列表和网站](/graph/search-concept-files)) </span><span class="sxs-lookup"><span data-stu-id="1c863-155">Search content in SharePoint and OneDrive ([files, lists and sites](/graph/search-concept-files))</span></span>
- <span data-ttu-id="1c863-156">搜索 [自定义类型 (Graph 连接器) ](/graph/search-concept-custom-types) 数据</span><span class="sxs-lookup"><span data-stu-id="1c863-156">Search [custom types (Graph Connectors)](/graph/search-concept-custom-types) data</span></span>
- <span data-ttu-id="1c863-157">[对搜索结果进行排序](/graph/search-concept-sort)</span><span class="sxs-lookup"><span data-stu-id="1c863-157">[Sort](/graph/search-concept-sort) search results</span></span>
- <span data-ttu-id="1c863-158">使用 [聚合](/graph/search-concept-aggregations) 优化搜索结果</span><span class="sxs-lookup"><span data-stu-id="1c863-158">Use [aggregations](/graph/search-concept-aggregations) to refine search results</span></span>


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "search: query",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


