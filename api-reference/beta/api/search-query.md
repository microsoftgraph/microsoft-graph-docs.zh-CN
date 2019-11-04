---
title: 搜索：查询
description: 在此处提供说明
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: cc0e750f34af4bc6013d5e4bfbae4b007347b270
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937621"
---
# <a name="search-query"></a><span data-ttu-id="0160c-103">搜索：查询</span><span class="sxs-lookup"><span data-stu-id="0160c-103">search: query</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0160c-104">执行请求正文中指定的查询。</span><span class="sxs-lookup"><span data-stu-id="0160c-104">Executes the query specified in the request body.</span></span> <span data-ttu-id="0160c-105">搜索结果在响应中提供。</span><span class="sxs-lookup"><span data-stu-id="0160c-105">Search results are provided in the response.</span></span>

## <a name="permissions"></a><span data-ttu-id="0160c-106">权限</span><span class="sxs-lookup"><span data-stu-id="0160c-106">Permissions</span></span>

<span data-ttu-id="0160c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0160c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0160c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0160c-109">Permission type</span></span>                        | <span data-ttu-id="0160c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0160c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0160c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0160c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0160c-112">阅读文章、文件、读取、ExternalItem、阅读、全部</span><span class="sxs-lookup"><span data-stu-id="0160c-112">Mail.Read, Files.Read.All, Calendars.Read, ExternalItem.Read.All</span></span> |
| <span data-ttu-id="0160c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0160c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0160c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0160c-114">Not supported.</span></span> |
| <span data-ttu-id="0160c-115">Application</span><span class="sxs-lookup"><span data-stu-id="0160c-115">Application</span></span>                            | <span data-ttu-id="0160c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0160c-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0160c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0160c-117">HTTP request</span></span>

```HTTP
POST /search/query
```

## <a name="request-headers"></a><span data-ttu-id="0160c-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="0160c-118">Request headers</span></span>

| <span data-ttu-id="0160c-119">名称</span><span class="sxs-lookup"><span data-stu-id="0160c-119">Name</span></span>          | <span data-ttu-id="0160c-120">说明</span><span class="sxs-lookup"><span data-stu-id="0160c-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="0160c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0160c-121">Authorization</span></span> | <span data-ttu-id="0160c-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="0160c-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="0160c-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="0160c-123">Request body</span></span>

<span data-ttu-id="0160c-124">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="0160c-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0160c-125">参数</span><span class="sxs-lookup"><span data-stu-id="0160c-125">Parameter</span></span>    | <span data-ttu-id="0160c-126">类型</span><span class="sxs-lookup"><span data-stu-id="0160c-126">Type</span></span>        | <span data-ttu-id="0160c-127">描述</span><span class="sxs-lookup"><span data-stu-id="0160c-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0160c-128">requests</span><span class="sxs-lookup"><span data-stu-id="0160c-128">requests</span></span>|<span data-ttu-id="0160c-129">[searchRequest](../resources/searchrequest.md)集合</span><span class="sxs-lookup"><span data-stu-id="0160c-129">[searchRequest](../resources/searchrequest.md) collection</span></span>|<span data-ttu-id="0160c-130">要发送到 JSON blob 中格式化的查询终结点的搜索请求。</span><span class="sxs-lookup"><span data-stu-id="0160c-130">The search request to be sent to the query endpoint formatted in a JSON blob.</span></span> <span data-ttu-id="0160c-131">它包含响应中的预期实体类型、基础源、分页参数、请求的字段和实际搜索查询。</span><span class="sxs-lookup"><span data-stu-id="0160c-131">It contains the type of entities expected in the response, the underlying sources, the paging parameters, the requested fields, and the actual search query.</span></span>|

## <a name="response"></a><span data-ttu-id="0160c-132">响应</span><span class="sxs-lookup"><span data-stu-id="0160c-132">Response</span></span>

<span data-ttu-id="0160c-133">如果成功，此方法在`HTTP 200 OK`响应正文中返回响应代码和[searchResponse](../resources/searchresponse.md)集合对象。</span><span class="sxs-lookup"><span data-stu-id="0160c-133">If successful, this method returns `HTTP 200 OK` response code and a [searchResponse](../resources/searchresponse.md) collection object in the response body.</span></span>

## <a name="common-use-cases"></a><span data-ttu-id="0160c-134">常见用例</span><span class="sxs-lookup"><span data-stu-id="0160c-134">Common use cases</span></span>

- <span data-ttu-id="0160c-135">搜索[邮件消息](/graph/search-concept-messages)</span><span class="sxs-lookup"><span data-stu-id="0160c-135">Search [mail messages](/graph/search-concept-messages)</span></span>
- <span data-ttu-id="0160c-136">搜索[日历事件](/graph/search-concept-events)</span><span class="sxs-lookup"><span data-stu-id="0160c-136">Search [calendar events](/graph/search-concept-events)</span></span>
- <span data-ttu-id="0160c-137">搜索[文件](/graph/search-concept-files)</span><span class="sxs-lookup"><span data-stu-id="0160c-137">Search [files](/graph/search-concept-files)</span></span>
- <span data-ttu-id="0160c-138">搜索[自定义类型（连接器）](/graph/search-concept-custom-types)数据</span><span class="sxs-lookup"><span data-stu-id="0160c-138">Search [custom types (Connectors)](/graph/search-concept-custom-types) data</span></span>

## <a name="examples"></a><span data-ttu-id="0160c-139">示例</span><span class="sxs-lookup"><span data-stu-id="0160c-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0160c-140">请求</span><span class="sxs-lookup"><span data-stu-id="0160c-140">Request</span></span>

<span data-ttu-id="0160c-141">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0160c-141">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0160c-142">响应</span><span class="sxs-lookup"><span data-stu-id="0160c-142">Response</span></span>

<span data-ttu-id="0160c-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0160c-143">The following is an example of the response.</span></span>

> <span data-ttu-id="0160c-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="0160c-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
