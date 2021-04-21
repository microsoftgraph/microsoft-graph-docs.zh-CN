---
title: searchEntity： query
description: 运行请求正文中指定的查询。 响应中提供了搜索结果。
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 346f6941d23387fce06f99ec4e7fcdf2907d0c0e
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921838"
---
# <a name="searchentity-query"></a><span data-ttu-id="0dda2-104">searchEntity： query</span><span class="sxs-lookup"><span data-stu-id="0dda2-104">searchEntity: query</span></span>

<span data-ttu-id="0dda2-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0dda2-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0dda2-106">运行请求正文中指定的查询。</span><span class="sxs-lookup"><span data-stu-id="0dda2-106">Runs the query specified in the request body.</span></span> <span data-ttu-id="0dda2-107">响应中提供了搜索结果。</span><span class="sxs-lookup"><span data-stu-id="0dda2-107">Search results are provided in the response.</span></span>

[!INCLUDE [search-api-deprecation](../../includes/search-api-deprecation.md)]

## <a name="permissions"></a><span data-ttu-id="0dda2-108">权限</span><span class="sxs-lookup"><span data-stu-id="0dda2-108">Permissions</span></span>

<span data-ttu-id="0dda2-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0dda2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span> 

| <span data-ttu-id="0dda2-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="0dda2-111">Permission type</span></span>                        | <span data-ttu-id="0dda2-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0dda2-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0dda2-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0dda2-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="0dda2-114">Mail.Read、Calendars.Read、Files.Read.All、Sites.Read.All、ExternalItem.Read.All</span><span class="sxs-lookup"><span data-stu-id="0dda2-114">Mail.Read, Calendars.Read, Files.Read.All, Sites.Read.All, ExternalItem.Read.All</span></span> |
| <span data-ttu-id="0dda2-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0dda2-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0dda2-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0dda2-116">Not supported.</span></span> |
| <span data-ttu-id="0dda2-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="0dda2-117">Application</span></span>                            | <span data-ttu-id="0dda2-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="0dda2-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0dda2-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0dda2-119">HTTP request</span></span>

```HTTP
POST /search/query
```

## <a name="request-headers"></a><span data-ttu-id="0dda2-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="0dda2-120">Request headers</span></span>

| <span data-ttu-id="0dda2-121">名称</span><span class="sxs-lookup"><span data-stu-id="0dda2-121">Name</span></span>          | <span data-ttu-id="0dda2-122">说明</span><span class="sxs-lookup"><span data-stu-id="0dda2-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="0dda2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0dda2-123">Authorization</span></span> | <span data-ttu-id="0dda2-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0dda2-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0dda2-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="0dda2-126">Content-type</span></span> | <span data-ttu-id="0dda2-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="0dda2-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0dda2-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="0dda2-129">Request body</span></span>

<span data-ttu-id="0dda2-130">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="0dda2-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0dda2-131">参数</span><span class="sxs-lookup"><span data-stu-id="0dda2-131">Parameter</span></span>    | <span data-ttu-id="0dda2-132">类型</span><span class="sxs-lookup"><span data-stu-id="0dda2-132">Type</span></span>        | <span data-ttu-id="0dda2-133">说明</span><span class="sxs-lookup"><span data-stu-id="0dda2-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0dda2-134">requests</span><span class="sxs-lookup"><span data-stu-id="0dda2-134">requests</span></span>|<span data-ttu-id="0dda2-135">[searchRequest](../resources/searchrequest.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0dda2-135">[searchRequest](../resources/searchrequest.md) collection</span></span>|<span data-ttu-id="0dda2-136">一个或多个搜索请求的集合，每个搜索请求的格式都为 JSON blob。</span><span class="sxs-lookup"><span data-stu-id="0dda2-136">A collection of one or more search requests each formatted in a JSON blob.</span></span> <span data-ttu-id="0dda2-137">每个 JSON blob 都包含响应中预期的资源类型、基础源、分页参数、请求的字段和实际搜索查询。</span><span class="sxs-lookup"><span data-stu-id="0dda2-137">Each JSON blob contains the types of resources expected in the response, the underlying sources, paging parameters, requested fields, and actual search query.</span></span> <br> <span data-ttu-id="0dda2-138">请注意搜索 [实体](../resources/search-api-overview.md#known-limitations) 类型的特定组合以及排序或聚合搜索结果的已知限制。</span><span class="sxs-lookup"><span data-stu-id="0dda2-138">Be aware of [known limitations](../resources/search-api-overview.md#known-limitations) on searching specific combinations of entity types, and sorting or aggregating search results.</span></span> |

## <a name="response"></a><span data-ttu-id="0dda2-139">响应</span><span class="sxs-lookup"><span data-stu-id="0dda2-139">Response</span></span>

<span data-ttu-id="0dda2-140">如果成功，此方法在响应正文中返回 响应代码和 `HTTP 200 OK` [searchResponse](../resources/searchresponse.md) 集合对象。</span><span class="sxs-lookup"><span data-stu-id="0dda2-140">If successful, this method returns `HTTP 200 OK` response code and a [searchResponse](../resources/searchresponse.md) collection object in the response body.</span></span>
 

## <a name="examples"></a><span data-ttu-id="0dda2-141">示例</span><span class="sxs-lookup"><span data-stu-id="0dda2-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0dda2-142">请求</span><span class="sxs-lookup"><span data-stu-id="0dda2-142">Request</span></span>

<span data-ttu-id="0dda2-143">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0dda2-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0dda2-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="0dda2-144">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="0dda2-145">C#</span><span class="sxs-lookup"><span data-stu-id="0dda2-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/search-query-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0dda2-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0dda2-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/search-query-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0dda2-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0dda2-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/search-query-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0dda2-148">Java</span><span class="sxs-lookup"><span data-stu-id="0dda2-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/search-query-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0dda2-149">响应</span><span class="sxs-lookup"><span data-stu-id="0dda2-149">Response</span></span>

<span data-ttu-id="0dda2-150">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0dda2-150">The following is an example of the response.</span></span>

> <span data-ttu-id="0dda2-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="0dda2-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="0dda2-153">另请参阅</span><span class="sxs-lookup"><span data-stu-id="0dda2-153">See also</span></span>
- <span data-ttu-id="0dda2-154">搜索 [邮件](/graph/search-concept-messages)</span><span class="sxs-lookup"><span data-stu-id="0dda2-154">Search [mail messages](/graph/search-concept-messages)</span></span>
- <span data-ttu-id="0dda2-155">搜索 [日历事件](/graph/search-concept-events)</span><span class="sxs-lookup"><span data-stu-id="0dda2-155">Search [calendar events](/graph/search-concept-events)</span></span>
- <span data-ttu-id="0dda2-156">在 SharePoint 和 OneDrive 中搜索 ([文件、列表和网站) ](/graph/search-concept-files)</span><span class="sxs-lookup"><span data-stu-id="0dda2-156">Search content in SharePoint and OneDrive ([files, lists and sites](/graph/search-concept-files))</span></span>
- <span data-ttu-id="0dda2-157">使用 [Graph 连接器 (搜索) ](/graph/search-concept-custom-types) 类型</span><span class="sxs-lookup"><span data-stu-id="0dda2-157">Search [custom types (Graph Connectors)](/graph/search-concept-custom-types) data</span></span>
- <span data-ttu-id="0dda2-158">[对](/graph/search-concept-sort) 搜索结果进行排序</span><span class="sxs-lookup"><span data-stu-id="0dda2-158">[Sort](/graph/search-concept-sort) search results</span></span>
- <span data-ttu-id="0dda2-159">使用 [聚合](/graph/search-concept-aggregations) 优化搜索结果</span><span class="sxs-lookup"><span data-stu-id="0dda2-159">Use [aggregations](/graph/search-concept-aggregations) to refine search results</span></span>


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "search: query",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


