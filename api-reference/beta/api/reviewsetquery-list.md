---
title: 列出 reviewSetQueries
description: 检索 reviewSetQuery 对象的列表。
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 84f26d18a6f4c53299503fb21d6e36e0337d53d7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48085333"
---
# <a name="list-reviewsetqueries"></a><span data-ttu-id="8c9a5-103">列出 reviewSetQueries</span><span class="sxs-lookup"><span data-stu-id="8c9a5-103">List reviewSetQueries</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c9a5-104">检索电子数据展示 [reviewSetQuery](../resources/reviewsetquery.md) 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="8c9a5-104">Retrieve a list of eDiscovery [reviewSetQuery](../resources/reviewsetquery.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="8c9a5-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="8c9a5-105">Permissions</span></span>

<span data-ttu-id="8c9a5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8c9a5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8c9a5-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="8c9a5-108">Permission type</span></span>                        | <span data-ttu-id="8c9a5-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8c9a5-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8c9a5-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8c9a5-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="8c9a5-111">User.Read</span><span class="sxs-lookup"><span data-stu-id="8c9a5-111">User.Read</span></span> |
| <span data-ttu-id="8c9a5-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8c9a5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c9a5-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="8c9a5-113">Not supported.</span></span> |
| <span data-ttu-id="8c9a5-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="8c9a5-114">Application</span></span>                            | <span data-ttu-id="8c9a5-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8c9a5-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8c9a5-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8c9a5-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /compliance/ediscovery/cases/{id}/reviewSets/{id}/queries
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8c9a5-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="8c9a5-117">Optional query parameters</span></span>

<span data-ttu-id="8c9a5-118">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="8c9a5-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="8c9a5-119">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="8c9a5-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="8c9a5-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="8c9a5-120">Request headers</span></span>

| <span data-ttu-id="8c9a5-121">名称</span><span class="sxs-lookup"><span data-stu-id="8c9a5-121">Name</span></span>      |<span data-ttu-id="8c9a5-122">说明</span><span class="sxs-lookup"><span data-stu-id="8c9a5-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8c9a5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8c9a5-123">Authorization</span></span> | <span data-ttu-id="8c9a5-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8c9a5-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8c9a5-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="8c9a5-126">Request body</span></span>

<span data-ttu-id="8c9a5-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8c9a5-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8c9a5-128">响应</span><span class="sxs-lookup"><span data-stu-id="8c9a5-128">Response</span></span>

<span data-ttu-id="8c9a5-129">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [reviewSetQuery](../resources/reviewsetquery.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="8c9a5-129">If successful, this method returns a `200 OK` response code and a collection of [reviewSetQuery](../resources/reviewsetquery.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8c9a5-130">示例</span><span class="sxs-lookup"><span data-stu-id="8c9a5-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8c9a5-131">请求</span><span class="sxs-lookup"><span data-stu-id="8c9a5-131">Request</span></span>

<span data-ttu-id="8c9a5-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8c9a5-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8c9a5-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="8c9a5-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_reviewsetquery"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/2eef613a-ca2d-42f4-89fe-84d5198ddedf/reviewSets/b26888b3-e1f5-47c5-bdf2-33d1b90cb2e8/queries
```
# <a name="c"></a>[<span data-ttu-id="8c9a5-134">C#</span><span class="sxs-lookup"><span data-stu-id="8c9a5-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-reviewsetquery-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8c9a5-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8c9a5-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-reviewsetquery-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8c9a5-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8c9a5-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-reviewsetquery-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8c9a5-137">响应</span><span class="sxs-lookup"><span data-stu-id="8c9a5-137">Response</span></span>

<span data-ttu-id="8c9a5-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8c9a5-138">The following is an example of the response.</span></span>

> <span data-ttu-id="8c9a5-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="8c9a5-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.reviewSetQuery",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/compliance/ediscovery/$metadata#cases('2eef613a-ca2d-42f4-89fe-84d5198ddedf')/reviewSets('b26888b3-e1f5-47c5-bdf2-33d1b90cb2e8')/queries",
    "@odata.nextLink": "https://graph.microsoft.com/beta/compliance/ediscovery/cases('2eef613a-ca2d-42f4-89fe-84d5198ddedf')/reviewSets('b26888b3-e1f5-47c5-bdf2-33d1b90cb2e8')/queries?$skipToken=<encodedPageToken>",
    "value": [
        {
            "id": "f7859ebb-5546-4f96-937a-9cf5723e9809",
            "displayName": "Query 1",
            "createdBy": {
                "user": {
                    "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
                    "displayName": "eDiscovery admin"
                }
            },
            "createdDateTime": "2020-03-02T12:07:52.6520503Z",
            "lastModifiedBy": {
                "user": {
                    "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
                    "displayName": "eDiscovery admin"
                }
            },
            "lastModifiedDateTime": "2020-03-02T12:07:52.6520503Z",
            "query": "(Cc:aa)"
        },
        {
            "id": "7c4b98e1-fe18-4887-be81-79f7a24b15c8",
            "displayName": "New query1",
            "description": null,
            "createdBy": {
                "user": {
                    "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
                    "displayName": "eDiscovery admin"
                }
            },
            "createdDateTime": "2020-03-02T16:17:19.3564678Z",
            "lastModifiedBy": {
                "user": {
                    "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
                    "displayName": "eDiscovery admin"
                }
            },
            "lastModifiedDateTime": "2020-03-02T16:17:19.3564678Z",
            "query": "subject:\"Quarterly Financials\""
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List queries",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


