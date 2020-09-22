---
title: 搜索：查询
description: 运行请求正文中指定的查询。 搜索结果在响应中提供。
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 781517d686ad0c01d2d1b7bd235bdf3dbb009f03
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48074144"
---
# <a name="search-query"></a><span data-ttu-id="f1a41-104">搜索：查询</span><span class="sxs-lookup"><span data-stu-id="f1a41-104">search: query</span></span>

<span data-ttu-id="f1a41-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1a41-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1a41-106">运行请求正文中指定的查询。</span><span class="sxs-lookup"><span data-stu-id="f1a41-106">Runs the query specified in the request body.</span></span> <span data-ttu-id="f1a41-107">搜索结果在响应中提供。</span><span class="sxs-lookup"><span data-stu-id="f1a41-107">Search results are provided in the response.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="f1a41-108">权限</span><span class="sxs-lookup"><span data-stu-id="f1a41-108">Permissions</span></span>

<span data-ttu-id="f1a41-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f1a41-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f1a41-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f1a41-111">Permission type</span></span>                        | <span data-ttu-id="f1a41-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f1a41-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f1a41-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f1a41-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="f1a41-114">阅读文章、文件、读取、ExternalItem、阅读、全部</span><span class="sxs-lookup"><span data-stu-id="f1a41-114">Mail.Read, Files.Read.All, Calendars.Read, ExternalItem.Read.All</span></span> |
| <span data-ttu-id="f1a41-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f1a41-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f1a41-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f1a41-116">Not supported.</span></span> |
| <span data-ttu-id="f1a41-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f1a41-117">Application</span></span>                            | <span data-ttu-id="f1a41-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="f1a41-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f1a41-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f1a41-119">HTTP request</span></span>

```HTTP
POST /search/query
```

## <a name="request-headers"></a><span data-ttu-id="f1a41-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f1a41-120">Request headers</span></span>

| <span data-ttu-id="f1a41-121">名称</span><span class="sxs-lookup"><span data-stu-id="f1a41-121">Name</span></span>          | <span data-ttu-id="f1a41-122">说明</span><span class="sxs-lookup"><span data-stu-id="f1a41-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="f1a41-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f1a41-123">Authorization</span></span> | <span data-ttu-id="f1a41-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f1a41-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f1a41-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="f1a41-126">Content-type</span></span> | <span data-ttu-id="f1a41-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="f1a41-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f1a41-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="f1a41-129">Request body</span></span>

<span data-ttu-id="f1a41-130">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="f1a41-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f1a41-131">参数</span><span class="sxs-lookup"><span data-stu-id="f1a41-131">Parameter</span></span>    | <span data-ttu-id="f1a41-132">类型</span><span class="sxs-lookup"><span data-stu-id="f1a41-132">Type</span></span>        | <span data-ttu-id="f1a41-133">说明</span><span class="sxs-lookup"><span data-stu-id="f1a41-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f1a41-134">requests</span><span class="sxs-lookup"><span data-stu-id="f1a41-134">requests</span></span>|<span data-ttu-id="f1a41-135">[searchRequest](../resources/searchrequest.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f1a41-135">[searchRequest](../resources/searchrequest.md) collection</span></span>|<span data-ttu-id="f1a41-136">要发送到 JSON blob 中格式化的查询终结点的搜索请求。</span><span class="sxs-lookup"><span data-stu-id="f1a41-136">The search request to be sent to the query endpoint formatted in a JSON blob.</span></span> <span data-ttu-id="f1a41-137">它包含响应中的预期实体类型、基础源、分页参数、请求的字段和实际搜索查询。</span><span class="sxs-lookup"><span data-stu-id="f1a41-137">It contains the type of entities expected in the response, the underlying sources, the paging parameters, the requested fields, and the actual search query.</span></span>|

## <a name="response"></a><span data-ttu-id="f1a41-138">响应</span><span class="sxs-lookup"><span data-stu-id="f1a41-138">Response</span></span>

<span data-ttu-id="f1a41-139">如果成功，此方法 `HTTP 200 OK` 在响应正文中返回响应代码和 [searchResponse](../resources/searchresponse.md) 集合对象。</span><span class="sxs-lookup"><span data-stu-id="f1a41-139">If successful, this method returns `HTTP 200 OK` response code and a [searchResponse](../resources/searchresponse.md) collection object in the response body.</span></span>

## <a name="common-use-cases"></a><span data-ttu-id="f1a41-140">常见用例</span><span class="sxs-lookup"><span data-stu-id="f1a41-140">Common use cases</span></span>

- <span data-ttu-id="f1a41-141">搜索 [邮件消息](/graph/search-concept-messages)</span><span class="sxs-lookup"><span data-stu-id="f1a41-141">Search [mail messages](/graph/search-concept-messages)</span></span>
- <span data-ttu-id="f1a41-142">搜索 [日历事件](/graph/search-concept-events)</span><span class="sxs-lookup"><span data-stu-id="f1a41-142">Search [calendar events](/graph/search-concept-events)</span></span>
- <span data-ttu-id="f1a41-143">搜索 [文件](/graph/search-concept-files)</span><span class="sxs-lookup"><span data-stu-id="f1a41-143">Search [files](/graph/search-concept-files)</span></span>
- <span data-ttu-id="f1a41-144">搜索 [自定义类型 (连接器) ](/graph/search-concept-custom-types) 数据</span><span class="sxs-lookup"><span data-stu-id="f1a41-144">Search [custom types (Connectors)](/graph/search-concept-custom-types) data</span></span>

## <a name="examples"></a><span data-ttu-id="f1a41-145">示例</span><span class="sxs-lookup"><span data-stu-id="f1a41-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f1a41-146">请求</span><span class="sxs-lookup"><span data-stu-id="f1a41-146">Request</span></span>

<span data-ttu-id="f1a41-147">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f1a41-147">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f1a41-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="f1a41-148">HTTP</span></span>](#tab/http)
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
        "query_string": {
          "query": "contoso product"
        }
      },
      "from": 0,
      "size": 25,
      "stored_fields": [
        "title",
        "description"
      ]
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="f1a41-149">C#</span><span class="sxs-lookup"><span data-stu-id="f1a41-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/search-query-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f1a41-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f1a41-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/search-query-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f1a41-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f1a41-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/search-query-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f1a41-152">响应</span><span class="sxs-lookup"><span data-stu-id="f1a41-152">Response</span></span>

<span data-ttu-id="f1a41-153">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f1a41-153">The following is an example of the response.</span></span>

> <span data-ttu-id="f1a41-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="f1a41-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
              "_id": "1",
              "_score": 1,
              "_sortField": "Relevance",
              "_summary": "_summary-value",
              "_source": "The source field will contain the underlying graph entity part of the response"
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

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "search: query",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


