---
title: 列出 namedLocations
description: 获取 namedLocation 对象的列表。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: da3de62116941946a52ab0b8ba32d44b4f8c5dad
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43382342"
---
# <a name="list-namedlocations"></a><span data-ttu-id="92697-103">列出 namedLocations</span><span class="sxs-lookup"><span data-stu-id="92697-103">List namedLocations</span></span>

<span data-ttu-id="92697-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92697-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="92697-105">获取[namedLocation](../resources/namedlocation.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="92697-105">Get a list of [namedLocation](../resources/namedlocation.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="92697-106">权限</span><span class="sxs-lookup"><span data-stu-id="92697-106">Permissions</span></span>

<span data-ttu-id="92697-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="92697-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="92697-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="92697-109">Permission type</span></span>                        | <span data-ttu-id="92697-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="92697-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="92697-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="92697-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="92697-112">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="92697-112">Policy.Read.All</span></span> |
| <span data-ttu-id="92697-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="92697-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="92697-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="92697-114">Not supported.</span></span> |
| <span data-ttu-id="92697-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="92697-115">Application</span></span>                            | <span data-ttu-id="92697-116">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="92697-116">Policy.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="92697-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="92697-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/conditionalAccess/namedLocations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="92697-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="92697-118">Optional query parameters</span></span>

<span data-ttu-id="92697-119">`$count`此方法支持、 `$filter`、 `$orderBy` `$select` `$skip`、、和`$top` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="92697-119">This method supports the `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="92697-120">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="92697-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="92697-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="92697-121">Request headers</span></span>

| <span data-ttu-id="92697-122">名称</span><span class="sxs-lookup"><span data-stu-id="92697-122">Name</span></span>      |<span data-ttu-id="92697-123">说明</span><span class="sxs-lookup"><span data-stu-id="92697-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="92697-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="92697-124">Authorization</span></span> | <span data-ttu-id="92697-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="92697-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="92697-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="92697-127">Request body</span></span>

<span data-ttu-id="92697-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="92697-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="92697-129">响应</span><span class="sxs-lookup"><span data-stu-id="92697-129">Response</span></span>

<span data-ttu-id="92697-130">如果成功，此方法在响应`200 OK`正文中返回响应代码和[namedLocation](../resources/namedlocation.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="92697-130">If successful, this method returns a `200 OK` response code and a collection of [namedLocation](../resources/namedlocation.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="92697-131">示例</span><span class="sxs-lookup"><span data-stu-id="92697-131">Examples</span></span>

### <a name="example-1-list-all-namedlocations"></a><span data-ttu-id="92697-132">示例1：列出所有 namedLocations</span><span class="sxs-lookup"><span data-stu-id="92697-132">Example 1: List all namedLocations</span></span>

#### <a name="request"></a><span data-ttu-id="92697-133">请求</span><span class="sxs-lookup"><span data-stu-id="92697-133">Request</span></span>

<span data-ttu-id="92697-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="92697-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="92697-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="92697-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_namedlocations"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identity/conditionalAccess/namedLocations
```
# <a name="c"></a>[<span data-ttu-id="92697-136">C#</span><span class="sxs-lookup"><span data-stu-id="92697-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-namedlocations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="92697-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="92697-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-namedlocations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="92697-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="92697-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-namedlocations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="92697-139">响应</span><span class="sxs-lookup"><span data-stu-id="92697-139">Response</span></span>

<span data-ttu-id="92697-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="92697-140">The following is an example of the response.</span></span>

> <span data-ttu-id="92697-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="92697-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.namedLocation",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json


{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#conditionalAccess/namedLocations",
    "value": [
        {
            "@odata.type": "#microsoft.graph.ipNamedLocation",
            "id": "06e4ff15-ca6b-4843-9c34-3fdd1ce8f739",
            "displayName": "IPv4 named location",
            "modifiedDateTime": "2019-07-26T18:00:43.5796446Z",
            "createdDateTime": "2018-06-22T11:56:12Z",
            "isTrusted": false,
            "ipRanges": [
                {
                    "@odata.type": "#microsoft.graph.iPv4CidrRange",
                    "cidrAddress": "6.5.4.3/32"
                },
                {
                    "@odata.type": "#microsoft.graph.iPv4CidrRange",
                    "cidrAddress": "127.126.125.0/24"
                }
            ]
        },
        {
            "@odata.type": "#microsoft.graph.countryNamedLocation",
            "id": "1b7f0916-7677-40d8-97a1-d606f4ed8fcf",
            "displayName": "Country named location",
            "modifiedDateTime": "2018-09-10T16:54:53.7238848Z",
            "createdDateTime": "2018-09-10T16:54:53.7238848Z",
            "countriesAndRegions": [
                "US",
                "CA"
            ],
            "includeUnknownCountriesAndRegions": false
        },
        {
            "@odata.type": "#microsoft.graph.ipNamedLocation",
            "id": "05239353-9117-4d29-a6a1-89724cb61b8c",
            "displayName": "Trusted IPv6 named location",
            "modifiedDateTime": "2019-09-16T00:47:36.4967092Z",
            "createdDateTime": "2019-09-15T21:53:34.5001162Z",
            "isTrusted": true,
            "ipRanges": [
                {
                    "@odata.type": "#microsoft.graph.iPv6CidrRange",
                    "cidrAddress": "2001:4898:80e8:7:d92a:7695:fda1:9d62/48"
                },
                {
                    "@odata.type": "#microsoft.graph.iPv6CidrRange",
                    "cidrAddress": "2001:4898:80d8:7:d92a:7695:fda1:9d62/48"
                }
            ]
        }
    ]
}
```
### <a name="example-2-list-all-ipnamedlocations"></a><span data-ttu-id="92697-143">示例2：列出所有 ipNamedLocations</span><span class="sxs-lookup"><span data-stu-id="92697-143">Example 2: List all ipNamedLocations</span></span>

#### <a name="request"></a><span data-ttu-id="92697-144">请求</span><span class="sxs-lookup"><span data-stu-id="92697-144">Request</span></span>

<span data-ttu-id="92697-145">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="92697-145">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="92697-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="92697-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_namedlocations"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identity/conditionalAccess/namedLocations?$filter=isof('microsoft.graph.ipNamedLocation')
```
# <a name="c"></a>[<span data-ttu-id="92697-147">C#</span><span class="sxs-lookup"><span data-stu-id="92697-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-namedlocations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="92697-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="92697-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-namedlocations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="92697-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="92697-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-namedlocations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="92697-150">响应</span><span class="sxs-lookup"><span data-stu-id="92697-150">Response</span></span>

<span data-ttu-id="92697-151">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="92697-151">The following is an example of the response.</span></span>

> <span data-ttu-id="92697-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="92697-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.namedLocation",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json


{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#conditionalAccess/namedLocations",
    "value": [
        {
            "@odata.type": "#microsoft.graph.ipNamedLocation",
            "id": "06e4ff15-ca6b-4843-9c34-3fdd1ce8f739",
            "displayName": "IPv4 named location",
            "modifiedDateTime": "2019-07-26T18:00:43.5796446Z",
            "createdDateTime": "2018-06-22T11:56:12Z",
            "isTrusted": false,
            "ipRanges": [
                {
                    "@odata.type": "#microsoft.graph.iPv4CidrRange",
                    "cidrAddress": "6.5.4.3/32"
                },
                {
                    "@odata.type": "#microsoft.graph.iPv4CidrRange",
                    "cidrAddress": "127.126.125.0/24"
                }
            ]
        },
        {
            "@odata.type": "#microsoft.graph.ipNamedLocation",
            "id": "05239353-9117-4d29-a6a1-89724cb61b8c",
            "displayName": "Trusted IPv6 named location",
            "modifiedDateTime": "2019-09-16T00:47:36.4967092Z",
            "createdDateTime": "2019-09-15T21:53:34.5001162Z",
            "isTrusted": true,
            "ipRanges": [
                {
                    "@odata.type": "#microsoft.graph.iPv6CidrRange",
                    "cidrAddress": "2001:4898:80e8:7:d92a:7695:fda1:9d62/48"
                },
                {
                    "@odata.type": "#microsoft.graph.iPv6CidrRange",
                    "cidrAddress": "2001:4898:80d8:7:d92a:7695:fda1:9d62/48"
                }
            ]
        }
    ]
}
```
### <a name="example-3-list-all-namedlocations-created-after-a-certain-date"></a><span data-ttu-id="92697-154">示例3：列出在特定日期之后创建的所有 namedLocations</span><span class="sxs-lookup"><span data-stu-id="92697-154">Example 3: List all namedLocations created after a certain date</span></span>

#### <a name="request"></a><span data-ttu-id="92697-155">请求</span><span class="sxs-lookup"><span data-stu-id="92697-155">Request</span></span>

<span data-ttu-id="92697-156">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="92697-156">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="92697-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="92697-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_namedlocations"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identity/conditionalAccess/namedLocations?$filter=createdDateTime ge 2019-09-01T00:00:00Z
```
# <a name="c"></a>[<span data-ttu-id="92697-158">C#</span><span class="sxs-lookup"><span data-stu-id="92697-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-namedlocations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="92697-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="92697-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-namedlocations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="92697-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="92697-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-namedlocations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="92697-161">响应</span><span class="sxs-lookup"><span data-stu-id="92697-161">Response</span></span>

<span data-ttu-id="92697-162">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="92697-162">The following is an example of the response.</span></span>

> <span data-ttu-id="92697-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="92697-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.namedLocation",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json


{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#conditionalAccess/namedLocations",
    "value": [
        {
            "@odata.type": "#microsoft.graph.ipNamedLocation",
            "id": "05239353-9117-4d29-a6a1-89724cb61b8c",
            "displayName": "Trusted IPv6 named location",
            "modifiedDateTime": "2019-09-16T00:47:36.4967092Z",
            "createdDateTime": "2019-09-15T21:53:34.5001162Z",
            "isTrusted": true,
            "ipRanges": [
                {
                    "@odata.type": "#microsoft.graph.iPv6CidrRange",
                    "cidrAddress": "2001:4898:80e8:7:d92a:7695:fda1:9d62/48"
                },
                {
                    "@odata.type": "#microsoft.graph.iPv6CidrRange",
                    "cidrAddress": "2001:4898:80d8:7:d92a:7695:fda1:9d62/48"
                }
            ]
        }
    ]
}
```
### <a name="example-4-list-all-countrynamedlocations-containing-a-certain-country-or-region"></a><span data-ttu-id="92697-165">示例4：列出包含特定国家或地区的所有 countryNamedLocations</span><span class="sxs-lookup"><span data-stu-id="92697-165">Example 4: List all countryNamedLocations containing a certain country or region</span></span>

#### <a name="request"></a><span data-ttu-id="92697-166">请求</span><span class="sxs-lookup"><span data-stu-id="92697-166">Request</span></span>

<span data-ttu-id="92697-167">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="92697-167">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="92697-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="92697-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_namedlocations"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identity/conditionalAccess/namedLocations?$filter=microsoft.graph.countryNamedLocation/countriesAndRegions/any(c: c eq 'CA')
```
# <a name="c"></a>[<span data-ttu-id="92697-169">C#</span><span class="sxs-lookup"><span data-stu-id="92697-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-namedlocations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="92697-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="92697-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-namedlocations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="92697-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="92697-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-namedlocations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="92697-172">响应</span><span class="sxs-lookup"><span data-stu-id="92697-172">Response</span></span>

<span data-ttu-id="92697-173">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="92697-173">The following is an example of the response.</span></span>

> <span data-ttu-id="92697-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="92697-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.namedLocation",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json


{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#conditionalAccess/namedLocations",
    "value": [
        {
            "@odata.type": "#microsoft.graph.countryNamedLocation",
            "id": "1b7f0916-7677-40d8-97a1-d606f4ed8fcf",
            "displayName": "Country named location",
            "modifiedDateTime": "2018-09-10T16:54:53.7238848Z",
            "createdDateTime": "2018-09-10T16:54:53.7238848Z",
            "countriesAndRegions": [
                "US",
                "CA"
            ],
            "includeUnknownCountriesAndRegions": false
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List namedLocations",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
