---
title: 列出事例
description: 检索电子数据展示事例列表。
localization_priority: Normal
author: mahage-msft
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: eae0e826451383eb4e3bbd9b2c8089709baf509e
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52044758"
---
# <a name="list-cases"></a><span data-ttu-id="19a6c-103">列出事例</span><span class="sxs-lookup"><span data-stu-id="19a6c-103">List cases</span></span>

<span data-ttu-id="19a6c-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="19a6c-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="19a6c-105">检索 case [对象](../resources/ediscovery-case.md) 的列表。</span><span class="sxs-lookup"><span data-stu-id="19a6c-105">Retrieve a list of [case](../resources/ediscovery-case.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="19a6c-106">权限</span><span class="sxs-lookup"><span data-stu-id="19a6c-106">Permissions</span></span>

<span data-ttu-id="19a6c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="19a6c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19a6c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="19a6c-109">Permission type</span></span>|<span data-ttu-id="19a6c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="19a6c-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="19a6c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="19a6c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="19a6c-112">eDiscovery.Read.All、eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19a6c-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="19a6c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="19a6c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="19a6c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="19a6c-114">Not supported.</span></span>|
|<span data-ttu-id="19a6c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="19a6c-115">Application</span></span>|<span data-ttu-id="19a6c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="19a6c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="19a6c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="19a6c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /compliance/ediscovery/cases
```

## <a name="optional-query-parameters"></a><span data-ttu-id="19a6c-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="19a6c-118">Optional query parameters</span></span>

<span data-ttu-id="19a6c-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="19a6c-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="19a6c-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="19a6c-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="19a6c-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="19a6c-121">Request headers</span></span>

| <span data-ttu-id="19a6c-122">名称</span><span class="sxs-lookup"><span data-stu-id="19a6c-122">Name</span></span>      |<span data-ttu-id="19a6c-123">说明</span><span class="sxs-lookup"><span data-stu-id="19a6c-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="19a6c-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="19a6c-124">Authorization</span></span> | <span data-ttu-id="19a6c-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="19a6c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="19a6c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="19a6c-127">Request body</span></span>

<span data-ttu-id="19a6c-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="19a6c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="19a6c-129">响应</span><span class="sxs-lookup"><span data-stu-id="19a6c-129">Response</span></span>

<span data-ttu-id="19a6c-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [microsoft.graph.ediscovery.case](../resources/ediscovery-case.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="19a6c-130">If successful, this method returns a `200 OK` response code and a collection of [microsoft.graph.ediscovery.case](../resources/ediscovery-case.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="19a6c-131">示例</span><span class="sxs-lookup"><span data-stu-id="19a6c-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="19a6c-132">请求</span><span class="sxs-lookup"><span data-stu-id="19a6c-132">Request</span></span>

<span data-ttu-id="19a6c-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="19a6c-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="19a6c-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="19a6c-134">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "list_case"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases
```

# <a name="c"></a>[<span data-ttu-id="19a6c-135">C#</span><span class="sxs-lookup"><span data-stu-id="19a6c-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-case-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="19a6c-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="19a6c-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-case-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="19a6c-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="19a6c-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-case-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="19a6c-138">Java</span><span class="sxs-lookup"><span data-stu-id="19a6c-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-case-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="19a6c-139">响应</span><span class="sxs-lookup"><span data-stu-id="19a6c-139">Response</span></span>

<span data-ttu-id="19a6c-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="19a6c-140">The following is an example of the response.</span></span>

> <span data-ttu-id="19a6c-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="19a6c-141">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.case",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#cases",
    "odata.nextLink":"https://graph.microsoft.com/beta/compliance/ediscovery/cases?$skipToken=159dc1d7-f84f-439e-9d57-4a4d3af0abe5",
    "value": [
        {
            "id": "061b9a92-8926-4bd9-b41d-abf35edc7583",
            "displayName": "My Case 1",
            "description": "",
            "createdBy": {
                "user": {
                    "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
                    "displayName": "eDiscovery admin"
                }
            },
            "createdDateTime": "2020-02-20T22:42:28.5505500Z",
            "lastModifiedBy": {
                "user": {
                    "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
                    "displayName": "eDiscovery admin"
                }
            },
            "lastModifiedDateTime": "2020-02-20T22:42:28.5505500Z",
            "status": "active",
            "closedBy": null,
            "closedDateTime": null,
            "externalId": ""
        },
        {
            "id": "b956a1b5-6b74-47db-af83-97d1fdad4ddc",
            "displayName": "My Case 2",
            "description": "",
            "createdBy": {
                "user": {
                    "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
                    "displayName": "eDiscovery admin"
                }
            },
            "createdDateTime": "2020-02-18T22:42:28.5505500Z",
            "lastModifiedBy": {
                "user": {
                    "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
                    "displayName": "eDiscovery admin"
                }
            },
            "lastModifiedDateTime": "2020-02-18T22:42:28.5505500Z",
            "status": "active",
            "closedBy": null,
            "closedDateTime": null,
            "externalId": ""
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List cases",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
