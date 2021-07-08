---
title: searchEntity： query
description: 运行请求正文中指定的查询。 响应中提供了搜索结果。
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: f2e3fa1aff81051820fda4444a55d9916e99128b
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334575"
---
# <a name="searchentity-query"></a><span data-ttu-id="a8d86-104">searchEntity： query</span><span class="sxs-lookup"><span data-stu-id="a8d86-104">searchEntity: query</span></span>

<span data-ttu-id="a8d86-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a8d86-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a8d86-106">运行请求正文中指定的查询。</span><span class="sxs-lookup"><span data-stu-id="a8d86-106">Runs the query specified in the request body.</span></span> <span data-ttu-id="a8d86-107">响应中提供了搜索结果。</span><span class="sxs-lookup"><span data-stu-id="a8d86-107">Search results are provided in the response.</span></span>

[!INCLUDE [search-api-deprecation](../../includes/search-api-deprecation.md)]

## <a name="permissions"></a><span data-ttu-id="a8d86-108">权限</span><span class="sxs-lookup"><span data-stu-id="a8d86-108">Permissions</span></span>

<span data-ttu-id="a8d86-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a8d86-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span> 

| <span data-ttu-id="a8d86-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a8d86-111">Permission type</span></span>                        | <span data-ttu-id="a8d86-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a8d86-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a8d86-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a8d86-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="a8d86-114">Mail.Read、Calendars.Read、Files.Read.All、Sites.Read.All、ExternalItem.Read.All</span><span class="sxs-lookup"><span data-stu-id="a8d86-114">Mail.Read, Calendars.Read, Files.Read.All, Sites.Read.All, ExternalItem.Read.All</span></span> |
| <span data-ttu-id="a8d86-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a8d86-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a8d86-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a8d86-116">Not supported.</span></span> |
| <span data-ttu-id="a8d86-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a8d86-117">Application</span></span>                            | <span data-ttu-id="a8d86-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="a8d86-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a8d86-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a8d86-119">HTTP request</span></span>

```HTTP
POST /search/query
```

## <a name="request-headers"></a><span data-ttu-id="a8d86-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a8d86-120">Request headers</span></span>

| <span data-ttu-id="a8d86-121">名称</span><span class="sxs-lookup"><span data-stu-id="a8d86-121">Name</span></span>          | <span data-ttu-id="a8d86-122">说明</span><span class="sxs-lookup"><span data-stu-id="a8d86-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="a8d86-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a8d86-123">Authorization</span></span> | <span data-ttu-id="a8d86-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a8d86-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a8d86-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="a8d86-126">Content-type</span></span> | <span data-ttu-id="a8d86-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="a8d86-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a8d86-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="a8d86-129">Request body</span></span>

<span data-ttu-id="a8d86-130">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="a8d86-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a8d86-131">参数</span><span class="sxs-lookup"><span data-stu-id="a8d86-131">Parameter</span></span>    | <span data-ttu-id="a8d86-132">类型</span><span class="sxs-lookup"><span data-stu-id="a8d86-132">Type</span></span>        | <span data-ttu-id="a8d86-133">说明</span><span class="sxs-lookup"><span data-stu-id="a8d86-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a8d86-134">requests</span><span class="sxs-lookup"><span data-stu-id="a8d86-134">requests</span></span>|<span data-ttu-id="a8d86-135">[searchRequest](../resources/searchrequest.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a8d86-135">[searchRequest](../resources/searchrequest.md) collection</span></span>|<span data-ttu-id="a8d86-136">一个或多个搜索请求的集合，每个搜索请求的格式都为 JSON blob。</span><span class="sxs-lookup"><span data-stu-id="a8d86-136">A collection of one or more search requests each formatted in a JSON blob.</span></span> <span data-ttu-id="a8d86-137">每个 JSON blob 都包含响应中预期的资源类型、基础源、分页参数、请求的字段和实际搜索查询。</span><span class="sxs-lookup"><span data-stu-id="a8d86-137">Each JSON blob contains the types of resources expected in the response, the underlying sources, paging parameters, requested fields, and actual search query.</span></span> <br> <span data-ttu-id="a8d86-138">请注意搜索 [实体](../resources/search-api-overview.md#known-limitations) 类型的特定组合以及排序或聚合搜索结果的已知限制。</span><span class="sxs-lookup"><span data-stu-id="a8d86-138">Be aware of [known limitations](../resources/search-api-overview.md#known-limitations) on searching specific combinations of entity types, and sorting or aggregating search results.</span></span> |
|<span data-ttu-id="a8d86-139">queryAlterationOptions</span><span class="sxs-lookup"><span data-stu-id="a8d86-139">queryAlterationOptions</span></span>|[<span data-ttu-id="a8d86-140">searchAlterationOptions</span><span class="sxs-lookup"><span data-stu-id="a8d86-140">searchAlterationOptions</span></span>](../resources/searchalterationoptions.md)|<span data-ttu-id="a8d86-141">JSON blob 中格式化的查询更改选项，其中包含用于拼写更正的两个可选标志。</span><span class="sxs-lookup"><span data-stu-id="a8d86-141">Query alteration options formatted in a JSON blob that contains two optional flags to for spelling correction.</span></span> <span data-ttu-id="a8d86-142">可选。</span><span class="sxs-lookup"><span data-stu-id="a8d86-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="a8d86-143">响应</span><span class="sxs-lookup"><span data-stu-id="a8d86-143">Response</span></span>

<span data-ttu-id="a8d86-144">如果成功，此方法在响应正文中返回 响应代码和 `HTTP 200 OK` [searchResponse](../resources/searchresponse.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a8d86-144">If successful, this method returns a `HTTP 200 OK` response code and a [searchResponse](../resources/searchresponse.md) object in the response body.</span></span>
 

## <a name="examples"></a><span data-ttu-id="a8d86-145">示例</span><span class="sxs-lookup"><span data-stu-id="a8d86-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a8d86-146">请求</span><span class="sxs-lookup"><span data-stu-id="a8d86-146">Request</span></span>

<span data-ttu-id="a8d86-147">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a8d86-147">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a8d86-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="a8d86-148">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="a8d86-149">C#</span><span class="sxs-lookup"><span data-stu-id="a8d86-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/search-query-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a8d86-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a8d86-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/search-query-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a8d86-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a8d86-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/search-query-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a8d86-152">Java</span><span class="sxs-lookup"><span data-stu-id="a8d86-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/search-query-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a8d86-153">响应</span><span class="sxs-lookup"><span data-stu-id="a8d86-153">Response</span></span>

<span data-ttu-id="a8d86-154">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a8d86-154">The following is an example of the response.</span></span>

> <span data-ttu-id="a8d86-155">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a8d86-155">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.searchResponse",
  "isCollection": true
} -->

```HTTP
HTTP/1.1 200 OK
Content-type: application/json

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

## <a name="see-also"></a><span data-ttu-id="a8d86-156">另请参阅</span><span class="sxs-lookup"><span data-stu-id="a8d86-156">See also</span></span>

- <span data-ttu-id="a8d86-157">搜索 [邮件](/graph/search-concept-messages)</span><span class="sxs-lookup"><span data-stu-id="a8d86-157">Search [mail messages](/graph/search-concept-messages)</span></span>
- <span data-ttu-id="a8d86-158">搜索 [日历事件](/graph/search-concept-events)</span><span class="sxs-lookup"><span data-stu-id="a8d86-158">Search [calendar events](/graph/search-concept-events)</span></span>
- <span data-ttu-id="a8d86-159">搜索 [人员](/graph/search-concept-person)</span><span class="sxs-lookup"><span data-stu-id="a8d86-159">Search [person](/graph/search-concept-person)</span></span>
- <span data-ttu-id="a8d86-160">搜索网站[SharePoint OneDrive (、列表和网站) ](/graph/search-concept-files)</span><span class="sxs-lookup"><span data-stu-id="a8d86-160">Search content in SharePoint and OneDrive ([files, lists and sites](/graph/search-concept-files))</span></span>
- <span data-ttu-id="a8d86-161">搜索[连接器 (Graph自定义) ](/graph/search-concept-custom-types)数据</span><span class="sxs-lookup"><span data-stu-id="a8d86-161">Search [custom types (Graph Connectors)](/graph/search-concept-custom-types) data</span></span>
- <span data-ttu-id="a8d86-162">[对](/graph/search-concept-sort) 搜索结果进行排序</span><span class="sxs-lookup"><span data-stu-id="a8d86-162">[Sort](/graph/search-concept-sort) search results</span></span>
- <span data-ttu-id="a8d86-163">使用 [聚合](/graph/search-concept-aggregations) 优化搜索结果</span><span class="sxs-lookup"><span data-stu-id="a8d86-163">Use [aggregations](/graph/search-concept-aggregations) to refine search results</span></span>
- <span data-ttu-id="a8d86-164">在 [搜索结果中启用](/graph/search-concept-speller) 拼写更正</span><span class="sxs-lookup"><span data-stu-id="a8d86-164">Enable [spell corrections](/graph/search-concept-speller) in search results</span></span>

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "search: query",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
