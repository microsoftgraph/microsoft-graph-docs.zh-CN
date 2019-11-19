---
title: 搜索：查询
description: 在此处提供说明
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: b5da13640d2c62eb8258ca1a154ddcb8c2e1b353
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/19/2019
ms.locfileid: "38703705"
---
# <a name="search-query"></a><span data-ttu-id="9a958-103">搜索：查询</span><span class="sxs-lookup"><span data-stu-id="9a958-103">search: query</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a958-104">执行请求正文中指定的查询。</span><span class="sxs-lookup"><span data-stu-id="9a958-104">Executes the query specified in the request body.</span></span> <span data-ttu-id="9a958-105">搜索结果在响应中提供。</span><span class="sxs-lookup"><span data-stu-id="9a958-105">Search results are provided in the response.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="9a958-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="9a958-106">Permissions</span></span>

<span data-ttu-id="9a958-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9a958-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9a958-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9a958-109">Permission type</span></span>                        | <span data-ttu-id="9a958-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9a958-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9a958-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9a958-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9a958-112">阅读文章、文件、读取、ExternalItem、阅读、全部</span><span class="sxs-lookup"><span data-stu-id="9a958-112">Mail.Read, Files.Read.All, Calendars.Read, ExternalItem.Read.All</span></span> |
| <span data-ttu-id="9a958-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9a958-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a958-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9a958-114">Not supported.</span></span> |
| <span data-ttu-id="9a958-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9a958-115">Application</span></span>                            | <span data-ttu-id="9a958-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9a958-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9a958-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9a958-117">HTTP request</span></span>

```HTTP
POST /search/query
```

## <a name="request-headers"></a><span data-ttu-id="9a958-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="9a958-118">Request headers</span></span>

| <span data-ttu-id="9a958-119">名称</span><span class="sxs-lookup"><span data-stu-id="9a958-119">Name</span></span>          | <span data-ttu-id="9a958-120">说明</span><span class="sxs-lookup"><span data-stu-id="9a958-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="9a958-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9a958-121">Authorization</span></span> | <span data-ttu-id="9a958-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="9a958-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="9a958-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="9a958-123">Request body</span></span>

<span data-ttu-id="9a958-124">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="9a958-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9a958-125">参数</span><span class="sxs-lookup"><span data-stu-id="9a958-125">Parameter</span></span>    | <span data-ttu-id="9a958-126">类型</span><span class="sxs-lookup"><span data-stu-id="9a958-126">Type</span></span>        | <span data-ttu-id="9a958-127">说明</span><span class="sxs-lookup"><span data-stu-id="9a958-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9a958-128">requests</span><span class="sxs-lookup"><span data-stu-id="9a958-128">requests</span></span>|<span data-ttu-id="9a958-129">[searchRequest](../resources/searchrequest.md)集合</span><span class="sxs-lookup"><span data-stu-id="9a958-129">[searchRequest](../resources/searchrequest.md) collection</span></span>|<span data-ttu-id="9a958-130">要发送到 JSON blob 中格式化的查询终结点的搜索请求。</span><span class="sxs-lookup"><span data-stu-id="9a958-130">The search request to be sent to the query endpoint formatted in a JSON blob.</span></span> <span data-ttu-id="9a958-131">它包含响应中的预期实体类型、基础源、分页参数、请求的字段和实际搜索查询。</span><span class="sxs-lookup"><span data-stu-id="9a958-131">It contains the type of entities expected in the response, the underlying sources, the paging parameters, the requested fields, and the actual search query.</span></span>|

## <a name="response"></a><span data-ttu-id="9a958-132">响应</span><span class="sxs-lookup"><span data-stu-id="9a958-132">Response</span></span>

<span data-ttu-id="9a958-133">如果成功，此方法在`HTTP 200 OK`响应正文中返回响应代码和[searchResponse](../resources/searchresponse.md)集合对象。</span><span class="sxs-lookup"><span data-stu-id="9a958-133">If successful, this method returns `HTTP 200 OK` response code and a [searchResponse](../resources/searchresponse.md) collection object in the response body.</span></span>

## <a name="common-use-cases"></a><span data-ttu-id="9a958-134">常见用例</span><span class="sxs-lookup"><span data-stu-id="9a958-134">Common use cases</span></span>

- <span data-ttu-id="9a958-135">搜索[邮件消息](/graph/search-concept-messages)</span><span class="sxs-lookup"><span data-stu-id="9a958-135">Search [mail messages](/graph/search-concept-messages)</span></span>
- <span data-ttu-id="9a958-136">搜索[日历事件](/graph/search-concept-events)</span><span class="sxs-lookup"><span data-stu-id="9a958-136">Search [calendar events](/graph/search-concept-events)</span></span>
- <span data-ttu-id="9a958-137">搜索[文件](/graph/search-concept-files)</span><span class="sxs-lookup"><span data-stu-id="9a958-137">Search [files](/graph/search-concept-files)</span></span>
- <span data-ttu-id="9a958-138">搜索[自定义类型（连接器）](/graph/search-concept-custom-types)数据</span><span class="sxs-lookup"><span data-stu-id="9a958-138">Search [custom types (Connectors)](/graph/search-concept-custom-types) data</span></span>

## <a name="examples"></a><span data-ttu-id="9a958-139">示例</span><span class="sxs-lookup"><span data-stu-id="9a958-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9a958-140">请求</span><span class="sxs-lookup"><span data-stu-id="9a958-140">Request</span></span>

<span data-ttu-id="9a958-141">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9a958-141">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9a958-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="9a958-142">HTTP</span></span>](#tab/http)
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
        "microsoft.graph.externalItem"
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="9a958-143">C#</span><span class="sxs-lookup"><span data-stu-id="9a958-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/search-query-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9a958-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9a958-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/search-query-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9a958-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9a958-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/search-query-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9a958-146">响应</span><span class="sxs-lookup"><span data-stu-id="9a958-146">Response</span></span>

<span data-ttu-id="9a958-147">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9a958-147">The following is an example of the response.</span></span>

> <span data-ttu-id="9a958-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="9a958-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
