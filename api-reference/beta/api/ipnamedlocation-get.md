---
title: 获取 ipNamedLocation
description: 检索 ipnamedlocation 对象的属性和关系。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 77b276877c416aaf4cfc21b9a152ac84f5ac59a0
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938472"
---
# <a name="get-ipnamedlocation"></a><span data-ttu-id="b3174-103">获取 ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="b3174-103">Get ipNamedLocation</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b3174-104">检索[ipNamedLocation](../resources/ipNamedLocation.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b3174-104">Retrieve the properties and relationships of an [ipNamedLocation](../resources/ipNamedLocation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b3174-105">权限</span><span class="sxs-lookup"><span data-stu-id="b3174-105">Permissions</span></span>

<span data-ttu-id="b3174-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b3174-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b3174-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="b3174-108">Permission type</span></span>                        | <span data-ttu-id="b3174-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b3174-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b3174-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b3174-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="b3174-111">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="b3174-111">Policy.Read.All</span></span> |
| <span data-ttu-id="b3174-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b3174-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b3174-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="b3174-113">Not supported.</span></span> |
| <span data-ttu-id="b3174-114">Application</span><span class="sxs-lookup"><span data-stu-id="b3174-114">Application</span></span>                            | <span data-ttu-id="b3174-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b3174-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b3174-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b3174-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /conditionalAccess/namedLocations/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b3174-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b3174-117">Optional query parameters</span></span>

<span data-ttu-id="b3174-118">此方法支持`select` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b3174-118">This method supports the `select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="b3174-119">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="b3174-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="b3174-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b3174-120">Request headers</span></span>

| <span data-ttu-id="b3174-121">名称</span><span class="sxs-lookup"><span data-stu-id="b3174-121">Name</span></span>      |<span data-ttu-id="b3174-122">说明</span><span class="sxs-lookup"><span data-stu-id="b3174-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b3174-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b3174-123">Authorization</span></span> | <span data-ttu-id="b3174-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b3174-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b3174-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="b3174-126">Request body</span></span>

<span data-ttu-id="b3174-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b3174-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b3174-128">响应</span><span class="sxs-lookup"><span data-stu-id="b3174-128">Response</span></span>

<span data-ttu-id="b3174-129">如果成功，此方法在响应`200 OK`正文中返回响应代码和请求的[ipNamedLocation](../resources/ipnamedlocation.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b3174-129">If successful, this method returns a `200 OK` response code and the requested [ipNamedLocation](../resources/ipnamedlocation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b3174-130">示例</span><span class="sxs-lookup"><span data-stu-id="b3174-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b3174-131">请求</span><span class="sxs-lookup"><span data-stu-id="b3174-131">Request</span></span>

<span data-ttu-id="b3174-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b3174-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b3174-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="b3174-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_ipnamedlocation"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/conditionalAccess/namedLocations/0854951d-5fc0-4eb1-b392-9b2c9d7949c2
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b3174-134">C#</span><span class="sxs-lookup"><span data-stu-id="b3174-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-ipnamedlocation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b3174-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b3174-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-ipnamedlocation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b3174-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b3174-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-ipnamedlocation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b3174-137">响应</span><span class="sxs-lookup"><span data-stu-id="b3174-137">Response</span></span>

<span data-ttu-id="b3174-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b3174-138">The following is an example of the response.</span></span>

> <span data-ttu-id="b3174-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b3174-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ipNamedLocation"
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
  "description": "Get ipNamedLocation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
