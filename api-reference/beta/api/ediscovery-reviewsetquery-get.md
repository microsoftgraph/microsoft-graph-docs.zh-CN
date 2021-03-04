---
title: 获取 reviewSetQuery
description: 检索电子数据展示 reviewsetquery 对象的属性和关系。
localization_priority: Normal
author: mahage-msft
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 3ddc2c3e3c7231d0bdf8ec81a12e49b4c016a83a
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446022"
---
# <a name="get-reviewsetquery"></a><span data-ttu-id="d746b-103">获取 reviewSetQuery</span><span class="sxs-lookup"><span data-stu-id="d746b-103">Get reviewSetQuery</span></span>

<span data-ttu-id="d746b-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="d746b-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d746b-105">检索电子数据展示 [reviewSetQuery 对象的属性和](../resources/ediscovery-reviewsetquery.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="d746b-105">Retrieve the properties and relationships of an eDiscovery [reviewSetQuery](../resources/ediscovery-reviewsetquery.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d746b-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="d746b-106">Permissions</span></span>

<span data-ttu-id="d746b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d746b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d746b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d746b-109">Permission type</span></span>|<span data-ttu-id="d746b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d746b-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d746b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d746b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d746b-112">eDiscovery.Read.All、eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d746b-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="d746b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d746b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d746b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d746b-114">Not supported.</span></span>|
|<span data-ttu-id="d746b-115">Application</span><span class="sxs-lookup"><span data-stu-id="d746b-115">Application</span></span>|<span data-ttu-id="d746b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d746b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d746b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d746b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /compliance/ediscovery/cases/{id}/reviewSets/{id}/queries/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d746b-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d746b-118">Optional query parameters</span></span>

<span data-ttu-id="d746b-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d746b-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="d746b-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="d746b-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="d746b-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="d746b-121">Request headers</span></span>

| <span data-ttu-id="d746b-122">名称</span><span class="sxs-lookup"><span data-stu-id="d746b-122">Name</span></span>      |<span data-ttu-id="d746b-123">说明</span><span class="sxs-lookup"><span data-stu-id="d746b-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d746b-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="d746b-124">Authorization</span></span> | <span data-ttu-id="d746b-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d746b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d746b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d746b-127">Request body</span></span>

<span data-ttu-id="d746b-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d746b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d746b-129">响应</span><span class="sxs-lookup"><span data-stu-id="d746b-129">Response</span></span>

<span data-ttu-id="d746b-130">如果成功，此方法在响应正文中返回响应代码和请求的 `200 OK` [microsoft.graph.ediscovery.reviewSetQuery](../resources/ediscovery-reviewsetquery.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d746b-130">If successful, this method returns a `200 OK` response code and the requested [microsoft.graph.ediscovery.reviewSetQuery](../resources/ediscovery-reviewsetquery.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d746b-131">示例</span><span class="sxs-lookup"><span data-stu-id="d746b-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d746b-132">请求</span><span class="sxs-lookup"><span data-stu-id="d746b-132">Request</span></span>

<span data-ttu-id="d746b-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d746b-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d746b-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="d746b-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_reviewsetquery"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/2eef613a-ca2d-42f4-89fe-84d5198ddedf/reviewSets/b26888b3-e1f5-47c5-bdf2-33d1b90cb2e8/queries/6b5358b0-2ce2-4369-b9cf-65392fe56807
```
# <a name="c"></a>[<span data-ttu-id="d746b-135">C#</span><span class="sxs-lookup"><span data-stu-id="d746b-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-reviewsetquery-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d746b-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d746b-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-reviewsetquery-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d746b-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d746b-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-reviewsetquery-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d746b-138">Java</span><span class="sxs-lookup"><span data-stu-id="d746b-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-reviewsetquery-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d746b-139">响应</span><span class="sxs-lookup"><span data-stu-id="d746b-139">Response</span></span>

<span data-ttu-id="d746b-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d746b-140">The following is an example of the response.</span></span>

> <span data-ttu-id="d746b-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d746b-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.reviewSetQuery"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/compliance/ediscovery/$metadata#cases('2eef613a-ca2d-42f4-89fe-84d5198ddedf')/reviewSets('b26888b3-e1f5-47c5-bdf2-33d1b90cb2e8')/queries/$entity",
    "id": "6b5358b0-2ce2-4369-b9cf-65392fe56807",
    "displayName": "My Query 1",
    "createdBy": {
        "user": {
            "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
            "displayName": "eDiscovery admin"
        }
    },
    "createdDateTime": "2020-03-09T09:05:12.3756813Z",
    "lastModifiedBy": {
        "user": {
            "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
            "displayName": "eDiscovery admin"
        }
    },
    "lastModifiedDateTime": "2020-03-09T09:05:12.3756813Z",
    "query": "subject:\"Quarterly Financials\""
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get reviewSetQuery",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


