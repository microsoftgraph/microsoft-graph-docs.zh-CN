---
title: 获取 namedLocation
description: 检索 namedlocation 对象的属性和关系。
localization_priority: Normal
author: dkershaw10
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 23c24915da7e269b647ffee8ac1c39dabccebc8f
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052101"
---
# <a name="get-namedlocation"></a><span data-ttu-id="72598-103">获取 namedLocation</span><span class="sxs-lookup"><span data-stu-id="72598-103">Get namedLocation</span></span>

<span data-ttu-id="72598-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72598-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72598-105">检索 [namedLocation](../resources/namedlocation.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="72598-105">Retrieve the properties and relationships of a [namedLocation](../resources/namedlocation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="72598-106">权限</span><span class="sxs-lookup"><span data-stu-id="72598-106">Permissions</span></span>

<span data-ttu-id="72598-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="72598-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="72598-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="72598-109">Permission type</span></span>                        | <span data-ttu-id="72598-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="72598-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="72598-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="72598-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="72598-112">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="72598-112">Policy.Read.All</span></span> |
| <span data-ttu-id="72598-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="72598-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="72598-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="72598-114">Not supported.</span></span> |
| <span data-ttu-id="72598-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="72598-115">Application</span></span>                            | <span data-ttu-id="72598-116">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="72598-116">Policy.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="72598-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="72598-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/conditionalAccess/namedLocations/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="72598-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="72598-118">Optional query parameters</span></span>

<span data-ttu-id="72598-119">此方法支持 `select` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="72598-119">This method supports the `select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="72598-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="72598-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="72598-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="72598-121">Request headers</span></span>

| <span data-ttu-id="72598-122">名称</span><span class="sxs-lookup"><span data-stu-id="72598-122">Name</span></span>      |<span data-ttu-id="72598-123">说明</span><span class="sxs-lookup"><span data-stu-id="72598-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="72598-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="72598-124">Authorization</span></span> | <span data-ttu-id="72598-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="72598-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="72598-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="72598-127">Request body</span></span>

<span data-ttu-id="72598-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="72598-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="72598-129">响应</span><span class="sxs-lookup"><span data-stu-id="72598-129">Response</span></span>

<span data-ttu-id="72598-130">如果成功，此方法在响应正文中返回 响应代码和请求 `200 OK` 的 [namedLocation](../resources/namedlocation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="72598-130">If successful, this method returns a `200 OK` response code and the requested [namedLocation](../resources/namedlocation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="72598-131">示例</span><span class="sxs-lookup"><span data-stu-id="72598-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="72598-132">请求</span><span class="sxs-lookup"><span data-stu-id="72598-132">Request</span></span>

<span data-ttu-id="72598-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="72598-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="72598-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="72598-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_namedlocation"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identity/conditionalAccess/namedLocations/0854951d-5fc0-4eb1-b392-9b2c9d7949c2
```
# <a name="c"></a>[<span data-ttu-id="72598-135">C#</span><span class="sxs-lookup"><span data-stu-id="72598-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-namedlocation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="72598-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="72598-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-namedlocation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="72598-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="72598-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-namedlocation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="72598-138">Java</span><span class="sxs-lookup"><span data-stu-id="72598-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-namedlocation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="72598-139">响应</span><span class="sxs-lookup"><span data-stu-id="72598-139">Response</span></span>

<span data-ttu-id="72598-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="72598-140">The following is an example of the response.</span></span>

> <span data-ttu-id="72598-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="72598-141">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.namedLocation"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#namedLocations/$entity",
    "@odata.type": "#microsoft.graph.ipNamedLocation",
    "id": "0854951d-5fc0-4eb1-b392-9b2c9d7949c2",
    "displayName": "Untrusted IP named location",
    "modifiedDateTime": "2019-09-04T01:11:34.9387578Z",
    "createdDateTime": "2019-09-04T01:11:34.9387578Z",
    "isTrusted": false,
    "ipRanges": [
        {
            "@odata.type": "#microsoft.graph.iPv4CidrRange",
            "cidrAddress": "12.34.221.11/22"
        },
        {
            "@odata.type": "#microsoft.graph.iPv6CidrRange",
            "cidrAddress": "2001:0:9d38:90d6:0:0:0:0/63"
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get namedLocation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


