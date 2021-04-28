---
title: 列出 namedLocations
description: 获取 namedLocation 对象的列表。
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 757a71f17aa2d42cbbe40c664fd4a30a3b308875
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054082"
---
# <a name="list-namedlocations"></a><span data-ttu-id="36313-103">列出 namedLocations</span><span class="sxs-lookup"><span data-stu-id="36313-103">List namedLocations</span></span>

<span data-ttu-id="36313-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="36313-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="36313-105">获取 [namedLocation 对象](../resources/namedlocation.md) 的列表。</span><span class="sxs-lookup"><span data-stu-id="36313-105">Get a list of [namedLocation](../resources/namedlocation.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="36313-106">权限</span><span class="sxs-lookup"><span data-stu-id="36313-106">Permissions</span></span>

<span data-ttu-id="36313-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="36313-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="36313-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="36313-109">Permission type</span></span>                        | <span data-ttu-id="36313-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="36313-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="36313-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="36313-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="36313-112">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="36313-112">Policy.Read.All</span></span> |
| <span data-ttu-id="36313-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="36313-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="36313-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="36313-114">Not supported.</span></span> |
| <span data-ttu-id="36313-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="36313-115">Application</span></span>                            | <span data-ttu-id="36313-116">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="36313-116">Policy.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="36313-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="36313-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/conditionalAccess/namedLocations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="36313-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="36313-118">Optional query parameters</span></span>

<span data-ttu-id="36313-119">此方法支持使用 `$count` 、 、 、 、 和 OData 查询参数 `$filter` `$orderBy` `$select` `$skip` `$top` 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="36313-119">This method supports the `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="36313-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="36313-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="36313-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="36313-121">Request headers</span></span>

| <span data-ttu-id="36313-122">名称</span><span class="sxs-lookup"><span data-stu-id="36313-122">Name</span></span>      |<span data-ttu-id="36313-123">说明</span><span class="sxs-lookup"><span data-stu-id="36313-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="36313-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="36313-124">Authorization</span></span> | <span data-ttu-id="36313-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="36313-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="36313-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="36313-127">Request body</span></span>

<span data-ttu-id="36313-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="36313-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="36313-129">响应</span><span class="sxs-lookup"><span data-stu-id="36313-129">Response</span></span>

<span data-ttu-id="36313-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [namedLocation](../resources/namedlocation.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="36313-130">If successful, this method returns a `200 OK` response code and a collection of [namedLocation](../resources/namedlocation.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="36313-131">示例</span><span class="sxs-lookup"><span data-stu-id="36313-131">Examples</span></span>

### <a name="example-1-list-all-namedlocations"></a><span data-ttu-id="36313-132">示例 1：列出所有 namedLocations</span><span class="sxs-lookup"><span data-stu-id="36313-132">Example 1: List all namedLocations</span></span>

#### <a name="request"></a><span data-ttu-id="36313-133">请求</span><span class="sxs-lookup"><span data-stu-id="36313-133">Request</span></span>

<span data-ttu-id="36313-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="36313-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="36313-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="36313-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_namedlocations_1"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/identity/conditionalAccess/namedLocations
```
# <a name="c"></a>[<span data-ttu-id="36313-136">C#</span><span class="sxs-lookup"><span data-stu-id="36313-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-namedlocations-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="36313-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="36313-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-namedlocations-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="36313-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="36313-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-namedlocations-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="36313-139">Java</span><span class="sxs-lookup"><span data-stu-id="36313-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-namedlocations-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="36313-140">响应</span><span class="sxs-lookup"><span data-stu-id="36313-140">Response</span></span>

<span data-ttu-id="36313-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="36313-141">The following is an example of the response.</span></span>

> <span data-ttu-id="36313-142">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="36313-142">**Note:** The response object shown here might be shortened for readability.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#conditionalAccess/namedLocations",
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
### <a name="example-2-list-all-ipnamedlocations"></a><span data-ttu-id="36313-143">示例 2：列出所有 ipNamedLocations</span><span class="sxs-lookup"><span data-stu-id="36313-143">Example 2: List all ipNamedLocations</span></span>

#### <a name="request"></a><span data-ttu-id="36313-144">请求</span><span class="sxs-lookup"><span data-stu-id="36313-144">Request</span></span>

<span data-ttu-id="36313-145">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="36313-145">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="36313-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="36313-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_namedlocations_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/identity/conditionalAccess/namedLocations?$filter=isof('microsoft.graph.ipNamedLocation')
```
# <a name="c"></a>[<span data-ttu-id="36313-147">C#</span><span class="sxs-lookup"><span data-stu-id="36313-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-namedlocations-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="36313-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="36313-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-namedlocations-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="36313-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="36313-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-namedlocations-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="36313-150">Java</span><span class="sxs-lookup"><span data-stu-id="36313-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-namedlocations-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="36313-151">响应</span><span class="sxs-lookup"><span data-stu-id="36313-151">Response</span></span>

<span data-ttu-id="36313-152">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="36313-152">The following is an example of the response.</span></span>

> <span data-ttu-id="36313-153">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="36313-153">**Note:** The response object shown here might be shortened for readability.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#conditionalAccess/namedLocations",
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
### <a name="example-3-list-all-namedlocations-created-after-a-certain-date"></a><span data-ttu-id="36313-154">示例 3：列出在特定日期之后创建的所有 namedLocation</span><span class="sxs-lookup"><span data-stu-id="36313-154">Example 3: List all namedLocations created after a certain date</span></span>

#### <a name="request"></a><span data-ttu-id="36313-155">请求</span><span class="sxs-lookup"><span data-stu-id="36313-155">Request</span></span>

<span data-ttu-id="36313-156">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="36313-156">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="36313-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="36313-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_namedlocations_3"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/identity/conditionalAccess/namedLocations?$filter=createdDateTime ge 2019-09-01T00:00:00Z
```
# <a name="c"></a>[<span data-ttu-id="36313-158">C#</span><span class="sxs-lookup"><span data-stu-id="36313-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-namedlocations-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="36313-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="36313-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-namedlocations-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="36313-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="36313-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-namedlocations-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="36313-161">Java</span><span class="sxs-lookup"><span data-stu-id="36313-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-namedlocations-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="36313-162">响应</span><span class="sxs-lookup"><span data-stu-id="36313-162">Response</span></span>

<span data-ttu-id="36313-163">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="36313-163">The following is an example of the response.</span></span>

> <span data-ttu-id="36313-164">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="36313-164">**Note:** The response object shown here might be shortened for readability.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#conditionalAccess/namedLocations",
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
### <a name="example-4-list-all-countrynamedlocations-containing-a-certain-country-or-region"></a><span data-ttu-id="36313-165">示例 4：列出包含特定国家/地区的所有 countryNamedLocations</span><span class="sxs-lookup"><span data-stu-id="36313-165">Example 4: List all countryNamedLocations containing a certain country or region</span></span>

#### <a name="request"></a><span data-ttu-id="36313-166">请求</span><span class="sxs-lookup"><span data-stu-id="36313-166">Request</span></span>

<span data-ttu-id="36313-167">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="36313-167">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="36313-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="36313-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_namedlocations_4"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/identity/conditionalAccess/namedLocations?$filter=microsoft.graph.countryNamedLocation/countriesAndRegions/any(c: c eq 'CA')
```
# <a name="c"></a>[<span data-ttu-id="36313-169">C#</span><span class="sxs-lookup"><span data-stu-id="36313-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-namedlocations-4-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="36313-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="36313-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-namedlocations-4-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="36313-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="36313-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-namedlocations-4-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="36313-172">Java</span><span class="sxs-lookup"><span data-stu-id="36313-172">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-namedlocations-4-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="36313-173">响应</span><span class="sxs-lookup"><span data-stu-id="36313-173">Response</span></span>

<span data-ttu-id="36313-174">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="36313-174">The following is an example of the response.</span></span>

> <span data-ttu-id="36313-175">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="36313-175">**Note:** The response object shown here might be shortened for readability.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#conditionalAccess/namedLocations",
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

