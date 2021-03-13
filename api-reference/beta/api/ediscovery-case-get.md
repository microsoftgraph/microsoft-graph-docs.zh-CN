---
title: 获取案例
description: 检索 case 对象的属性和关系。
localization_priority: Normal
author: mahage-msft
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: d4785ba534ddbb334b87da5c0ddac3f8b32cb071
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776730"
---
# <a name="get-case"></a><span data-ttu-id="a44a5-103">获取案例</span><span class="sxs-lookup"><span data-stu-id="a44a5-103">Get case</span></span>

<span data-ttu-id="a44a5-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="a44a5-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a44a5-105">检索 case [对象的属性和](../resources/ediscovery-case.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="a44a5-105">Retrieve the properties and relationships of a [case](../resources/ediscovery-case.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a44a5-106">权限</span><span class="sxs-lookup"><span data-stu-id="a44a5-106">Permissions</span></span>

<span data-ttu-id="a44a5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a44a5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a44a5-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a44a5-109">Permission type</span></span>|<span data-ttu-id="a44a5-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a44a5-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a44a5-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a44a5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a44a5-112">eDiscovery.Read.All、eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a44a5-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="a44a5-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a44a5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a44a5-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a44a5-114">Not supported.</span></span>|
|<span data-ttu-id="a44a5-115">Application</span><span class="sxs-lookup"><span data-stu-id="a44a5-115">Application</span></span>|<span data-ttu-id="a44a5-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a44a5-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a44a5-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a44a5-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /compliance/ediscovery/cases/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a44a5-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a44a5-118">Optional query parameters</span></span>

<span data-ttu-id="a44a5-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a44a5-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="a44a5-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="a44a5-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="a44a5-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="a44a5-121">Request headers</span></span>

| <span data-ttu-id="a44a5-122">名称</span><span class="sxs-lookup"><span data-stu-id="a44a5-122">Name</span></span>      |<span data-ttu-id="a44a5-123">说明</span><span class="sxs-lookup"><span data-stu-id="a44a5-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a44a5-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a44a5-124">Authorization</span></span> | <span data-ttu-id="a44a5-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a44a5-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a44a5-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a44a5-127">Request body</span></span>

<span data-ttu-id="a44a5-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a44a5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a44a5-129">响应</span><span class="sxs-lookup"><span data-stu-id="a44a5-129">Response</span></span>

<span data-ttu-id="a44a5-130">如果成功，此方法在响应正文中返回 响应代码和请求的 `200 OK` [microsoft.graph.ediscovery.case](../resources/ediscovery-case.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a44a5-130">If successful, this method returns a `200 OK` response code and the requested [microsoft.graph.ediscovery.case](../resources/ediscovery-case.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a44a5-131">示例</span><span class="sxs-lookup"><span data-stu-id="a44a5-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a44a5-132">请求</span><span class="sxs-lookup"><span data-stu-id="a44a5-132">Request</span></span>

<span data-ttu-id="a44a5-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a44a5-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a44a5-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="a44a5-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_case"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/061b9a92-8926-4bd9-b41d-abf35edc7583
```
# <a name="c"></a>[<span data-ttu-id="a44a5-135">C#</span><span class="sxs-lookup"><span data-stu-id="a44a5-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-case-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a44a5-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a44a5-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-case-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a44a5-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a44a5-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-case-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a44a5-138">Java</span><span class="sxs-lookup"><span data-stu-id="a44a5-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-case-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a44a5-139">响应</span><span class="sxs-lookup"><span data-stu-id="a44a5-139">Response</span></span>

<span data-ttu-id="a44a5-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a44a5-140">The following is an example of the response.</span></span>

> <span data-ttu-id="a44a5-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a44a5-141">**Note:** The response object shown here might be shortened for readability.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.case"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

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
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get Case",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
