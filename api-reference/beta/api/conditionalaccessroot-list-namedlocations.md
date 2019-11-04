---
title: 列出 namedLocations
description: 获取 namedLocation 对象的列表。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8b4af8a750c1264039146254417e6e7de6b34589
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37936682"
---
# <a name="list-namedlocations"></a><span data-ttu-id="c1c2d-103">列出 namedLocations</span><span class="sxs-lookup"><span data-stu-id="c1c2d-103">List namedLocations</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c1c2d-104">获取[namedLocation](../resources/namedlocation.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="c1c2d-104">Get a list of [namedLocation](../resources/namedlocation.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="c1c2d-105">权限</span><span class="sxs-lookup"><span data-stu-id="c1c2d-105">Permissions</span></span>

<span data-ttu-id="c1c2d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c1c2d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c1c2d-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="c1c2d-108">Permission type</span></span>                        | <span data-ttu-id="c1c2d-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c1c2d-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c1c2d-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c1c2d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="c1c2d-111">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1c2d-111">Policy.Read.All</span></span> |
| <span data-ttu-id="c1c2d-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c1c2d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c1c2d-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="c1c2d-113">Not supported.</span></span> |
| <span data-ttu-id="c1c2d-114">Application</span><span class="sxs-lookup"><span data-stu-id="c1c2d-114">Application</span></span>                            | <span data-ttu-id="c1c2d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c1c2d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c1c2d-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c1c2d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /conditionalAccess/namedLocations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c1c2d-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c1c2d-117">Optional query parameters</span></span>

<span data-ttu-id="c1c2d-118">`$count`此方法支持、 `$filter`、 `$orderBy` `$select` `$skip`、、和`$top` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c1c2d-118">This method supports the `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="c1c2d-119">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="c1c2d-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="c1c2d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c1c2d-120">Request headers</span></span>

| <span data-ttu-id="c1c2d-121">名称</span><span class="sxs-lookup"><span data-stu-id="c1c2d-121">Name</span></span>      |<span data-ttu-id="c1c2d-122">说明</span><span class="sxs-lookup"><span data-stu-id="c1c2d-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c1c2d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c1c2d-123">Authorization</span></span> | <span data-ttu-id="c1c2d-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c1c2d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c1c2d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c1c2d-126">Request body</span></span>

<span data-ttu-id="c1c2d-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c1c2d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c1c2d-128">响应</span><span class="sxs-lookup"><span data-stu-id="c1c2d-128">Response</span></span>

<span data-ttu-id="c1c2d-129">如果成功，此方法在响应`200 OK`正文中返回响应代码和[namedLocation](../resources/namedlocation.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="c1c2d-129">If successful, this method returns a `200 OK` response code and a collection of [namedLocation](../resources/namedlocation.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c1c2d-130">示例</span><span class="sxs-lookup"><span data-stu-id="c1c2d-130">Examples</span></span>

### <a name="example-1-list-all-namedlocations"></a><span data-ttu-id="c1c2d-131">示例1：列出所有 namedLocations</span><span class="sxs-lookup"><span data-stu-id="c1c2d-131">Example 1: List all namedLocations</span></span>

#### <a name="request"></a><span data-ttu-id="c1c2d-132">请求</span><span class="sxs-lookup"><span data-stu-id="c1c2d-132">Request</span></span>

<span data-ttu-id="c1c2d-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c1c2d-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c1c2d-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="c1c2d-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_namedlocations"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/conditionalAccess/namedLocations
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c1c2d-135">C#</span><span class="sxs-lookup"><span data-stu-id="c1c2d-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-namedlocations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c1c2d-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c1c2d-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-namedlocations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c1c2d-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c1c2d-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-namedlocations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c1c2d-138">响应</span><span class="sxs-lookup"><span data-stu-id="c1c2d-138">Response</span></span>

<span data-ttu-id="c1c2d-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c1c2d-139">The following is an example of the response.</span></span>

> <span data-ttu-id="c1c2d-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c1c2d-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
### <a name="example-2-list-all-ipnamedlocations"></a><span data-ttu-id="c1c2d-142">示例2：列出所有 ipNamedLocations</span><span class="sxs-lookup"><span data-stu-id="c1c2d-142">Example 2: List all ipNamedLocations</span></span>

#### <a name="request"></a><span data-ttu-id="c1c2d-143">请求</span><span class="sxs-lookup"><span data-stu-id="c1c2d-143">Request</span></span>

<span data-ttu-id="c1c2d-144">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c1c2d-144">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c1c2d-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="c1c2d-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_namedlocations"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/conditionalAccess/namedLocations?$filter=isof('microsoft.graph.ipNamedLocation')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c1c2d-146">C#</span><span class="sxs-lookup"><span data-stu-id="c1c2d-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-namedlocations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c1c2d-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c1c2d-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-namedlocations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c1c2d-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c1c2d-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-namedlocations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c1c2d-149">响应</span><span class="sxs-lookup"><span data-stu-id="c1c2d-149">Response</span></span>

<span data-ttu-id="c1c2d-150">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c1c2d-150">The following is an example of the response.</span></span>

> <span data-ttu-id="c1c2d-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c1c2d-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
### <a name="example-3-list-all-namedlocations-created-after-a-certain-date"></a><span data-ttu-id="c1c2d-153">示例3：列出在特定日期之后创建的所有 namedLocations</span><span class="sxs-lookup"><span data-stu-id="c1c2d-153">Example 3: List all namedLocations created after a certain date</span></span>

#### <a name="request"></a><span data-ttu-id="c1c2d-154">请求</span><span class="sxs-lookup"><span data-stu-id="c1c2d-154">Request</span></span>

<span data-ttu-id="c1c2d-155">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c1c2d-155">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c1c2d-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="c1c2d-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_namedlocations"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/conditionalAccess/namedLocations?$filter=createdDateTime ge 2019-09-01T00:00:00Z
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c1c2d-157">C#</span><span class="sxs-lookup"><span data-stu-id="c1c2d-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-namedlocations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c1c2d-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c1c2d-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-namedlocations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c1c2d-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c1c2d-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-namedlocations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c1c2d-160">响应</span><span class="sxs-lookup"><span data-stu-id="c1c2d-160">Response</span></span>

<span data-ttu-id="c1c2d-161">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c1c2d-161">The following is an example of the response.</span></span>

> <span data-ttu-id="c1c2d-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c1c2d-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
### <a name="example-4-list-all-countrynamedlocations-containing-a-certain-country-or-region"></a><span data-ttu-id="c1c2d-164">示例4：列出包含特定国家或地区的所有 countryNamedLocations</span><span class="sxs-lookup"><span data-stu-id="c1c2d-164">Example 4: List all countryNamedLocations containing a certain country or region</span></span>

#### <a name="request"></a><span data-ttu-id="c1c2d-165">请求</span><span class="sxs-lookup"><span data-stu-id="c1c2d-165">Request</span></span>

<span data-ttu-id="c1c2d-166">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c1c2d-166">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c1c2d-167">HTTP</span><span class="sxs-lookup"><span data-stu-id="c1c2d-167">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_namedlocations"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/conditionalAccess/namedLocations?$filter=microsoft.graph.countryNamedLocation/countriesAndRegions/any(c: c eq 'CA')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c1c2d-168">C#</span><span class="sxs-lookup"><span data-stu-id="c1c2d-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-namedlocations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c1c2d-169">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c1c2d-169">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-namedlocations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c1c2d-170">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c1c2d-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-namedlocations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c1c2d-171">响应</span><span class="sxs-lookup"><span data-stu-id="c1c2d-171">Response</span></span>

<span data-ttu-id="c1c2d-172">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c1c2d-172">The following is an example of the response.</span></span>

> <span data-ttu-id="c1c2d-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c1c2d-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
