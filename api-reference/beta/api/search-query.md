---
title: 搜索：查询
description: 运行请求正文中指定的查询。 搜索结果在响应中提供。
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: ff5d67dc749ce60797ec6c6387d79795718409c5
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40868847"
---
# <a name="search-query"></a><span data-ttu-id="40e4e-104">搜索：查询</span><span class="sxs-lookup"><span data-stu-id="40e4e-104">search: query</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="40e4e-105">运行请求正文中指定的查询。</span><span class="sxs-lookup"><span data-stu-id="40e4e-105">Runs the query specified in the request body.</span></span> <span data-ttu-id="40e4e-106">搜索结果在响应中提供。</span><span class="sxs-lookup"><span data-stu-id="40e4e-106">Search results are provided in the response.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="40e4e-107">权限</span><span class="sxs-lookup"><span data-stu-id="40e4e-107">Permissions</span></span>

<span data-ttu-id="40e4e-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="40e4e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="40e4e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="40e4e-110">Permission type</span></span>                        | <span data-ttu-id="40e4e-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="40e4e-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="40e4e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="40e4e-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="40e4e-113">阅读文章、文件、读取、ExternalItem、阅读、全部</span><span class="sxs-lookup"><span data-stu-id="40e4e-113">Mail.Read, Files.Read.All, Calendars.Read, ExternalItem.Read.All</span></span> |
| <span data-ttu-id="40e4e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="40e4e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="40e4e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="40e4e-115">Not supported.</span></span> |
| <span data-ttu-id="40e4e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="40e4e-116">Application</span></span>                            | <span data-ttu-id="40e4e-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="40e4e-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="40e4e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="40e4e-118">HTTP request</span></span>

```HTTP
POST /search/query
```

## <a name="request-headers"></a><span data-ttu-id="40e4e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="40e4e-119">Request headers</span></span>

| <span data-ttu-id="40e4e-120">名称</span><span class="sxs-lookup"><span data-stu-id="40e4e-120">Name</span></span>          | <span data-ttu-id="40e4e-121">说明</span><span class="sxs-lookup"><span data-stu-id="40e4e-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="40e4e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="40e4e-122">Authorization</span></span> | <span data-ttu-id="40e4e-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="40e4e-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="40e4e-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="40e4e-125">Content-type</span></span> | <span data-ttu-id="40e4e-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="40e4e-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="40e4e-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="40e4e-128">Request body</span></span>

<span data-ttu-id="40e4e-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="40e4e-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="40e4e-130">参数</span><span class="sxs-lookup"><span data-stu-id="40e4e-130">Parameter</span></span>    | <span data-ttu-id="40e4e-131">类型</span><span class="sxs-lookup"><span data-stu-id="40e4e-131">Type</span></span>        | <span data-ttu-id="40e4e-132">说明</span><span class="sxs-lookup"><span data-stu-id="40e4e-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="40e4e-133">requests</span><span class="sxs-lookup"><span data-stu-id="40e4e-133">requests</span></span>|<span data-ttu-id="40e4e-134">[searchRequest](../resources/searchrequest.md)集合</span><span class="sxs-lookup"><span data-stu-id="40e4e-134">[searchRequest](../resources/searchrequest.md) collection</span></span>|<span data-ttu-id="40e4e-135">要发送到 JSON blob 中格式化的查询终结点的搜索请求。</span><span class="sxs-lookup"><span data-stu-id="40e4e-135">The search request to be sent to the query endpoint formatted in a JSON blob.</span></span> <span data-ttu-id="40e4e-136">它包含响应中的预期实体类型、基础源、分页参数、请求的字段和实际搜索查询。</span><span class="sxs-lookup"><span data-stu-id="40e4e-136">It contains the type of entities expected in the response, the underlying sources, the paging parameters, the requested fields, and the actual search query.</span></span>|

## <a name="response"></a><span data-ttu-id="40e4e-137">响应</span><span class="sxs-lookup"><span data-stu-id="40e4e-137">Response</span></span>

<span data-ttu-id="40e4e-138">如果成功，此方法在`HTTP 200 OK`响应正文中返回响应代码和[searchResponse](../resources/searchresponse.md)集合对象。</span><span class="sxs-lookup"><span data-stu-id="40e4e-138">If successful, this method returns `HTTP 200 OK` response code and a [searchResponse](../resources/searchresponse.md) collection object in the response body.</span></span>

## <a name="common-use-cases"></a><span data-ttu-id="40e4e-139">常见用例</span><span class="sxs-lookup"><span data-stu-id="40e4e-139">Common use cases</span></span>

- <span data-ttu-id="40e4e-140">搜索[邮件消息](/graph/search-concept-messages)</span><span class="sxs-lookup"><span data-stu-id="40e4e-140">Search [mail messages](/graph/search-concept-messages)</span></span>
- <span data-ttu-id="40e4e-141">搜索[日历事件](/graph/search-concept-events)</span><span class="sxs-lookup"><span data-stu-id="40e4e-141">Search [calendar events](/graph/search-concept-events)</span></span>
- <span data-ttu-id="40e4e-142">搜索[文件](/graph/search-concept-files)</span><span class="sxs-lookup"><span data-stu-id="40e4e-142">Search [files](/graph/search-concept-files)</span></span>
- <span data-ttu-id="40e4e-143">搜索[自定义类型（连接器）](/graph/search-concept-custom-types)数据</span><span class="sxs-lookup"><span data-stu-id="40e4e-143">Search [custom types (Connectors)](/graph/search-concept-custom-types) data</span></span>

## <a name="examples"></a><span data-ttu-id="40e4e-144">示例</span><span class="sxs-lookup"><span data-stu-id="40e4e-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="40e4e-145">请求</span><span class="sxs-lookup"><span data-stu-id="40e4e-145">Request</span></span>

<span data-ttu-id="40e4e-146">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="40e4e-146">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="40e4e-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="40e4e-147">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="40e4e-148">C#</span><span class="sxs-lookup"><span data-stu-id="40e4e-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/search-query-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="40e4e-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="40e4e-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/search-query-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="40e4e-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="40e4e-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/search-query-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="40e4e-151">响应</span><span class="sxs-lookup"><span data-stu-id="40e4e-151">Response</span></span>

<span data-ttu-id="40e4e-152">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="40e4e-152">The following is an example of the response.</span></span>

> <span data-ttu-id="40e4e-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="40e4e-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
