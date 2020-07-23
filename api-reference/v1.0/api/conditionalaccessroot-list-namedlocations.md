---
title: 列出 namedLocations
description: 获取 namedLocation 对象的列表。
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f329c79b1c8a092f53daa22f2c1228f77d810278
ms.sourcegitcommit: fec7d5002dbeb8d58587c89f1b678d4a54645422
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/23/2020
ms.locfileid: "45384477"
---
# <a name="list-namedlocations"></a><span data-ttu-id="835ac-103">列出 namedLocations</span><span class="sxs-lookup"><span data-stu-id="835ac-103">List namedLocations</span></span>

<span data-ttu-id="835ac-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="835ac-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="835ac-105">获取[namedLocation](../resources/namedlocation.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="835ac-105">Get a list of [namedLocation](../resources/namedlocation.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="835ac-106">权限</span><span class="sxs-lookup"><span data-stu-id="835ac-106">Permissions</span></span>

<span data-ttu-id="835ac-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="835ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="835ac-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="835ac-109">Permission type</span></span>                        | <span data-ttu-id="835ac-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="835ac-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="835ac-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="835ac-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="835ac-112">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="835ac-112">Policy.Read.All</span></span> |
| <span data-ttu-id="835ac-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="835ac-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="835ac-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="835ac-114">Not supported.</span></span> |
| <span data-ttu-id="835ac-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="835ac-115">Application</span></span>                            | <span data-ttu-id="835ac-116">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="835ac-116">Policy.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="835ac-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="835ac-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/conditionalAccess/namedLocations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="835ac-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="835ac-118">Optional query parameters</span></span>

<span data-ttu-id="835ac-119">此方法支持 `$count` 、、、、 `$filter` `$orderBy` `$select` `$skip` 和 `$top` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="835ac-119">This method supports the `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="835ac-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="835ac-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="835ac-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="835ac-121">Request headers</span></span>

| <span data-ttu-id="835ac-122">名称</span><span class="sxs-lookup"><span data-stu-id="835ac-122">Name</span></span>      |<span data-ttu-id="835ac-123">说明</span><span class="sxs-lookup"><span data-stu-id="835ac-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="835ac-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="835ac-124">Authorization</span></span> | <span data-ttu-id="835ac-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="835ac-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="835ac-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="835ac-127">Request body</span></span>

<span data-ttu-id="835ac-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="835ac-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="835ac-129">响应</span><span class="sxs-lookup"><span data-stu-id="835ac-129">Response</span></span>

<span data-ttu-id="835ac-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[namedLocation](../resources/namedlocation.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="835ac-130">If successful, this method returns a `200 OK` response code and a collection of [namedLocation](../resources/namedlocation.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="835ac-131">示例</span><span class="sxs-lookup"><span data-stu-id="835ac-131">Examples</span></span>

### <a name="example-1-list-all-namedlocations"></a><span data-ttu-id="835ac-132">示例1：列出所有 namedLocations</span><span class="sxs-lookup"><span data-stu-id="835ac-132">Example 1: List all namedLocations</span></span>

#### <a name="request"></a><span data-ttu-id="835ac-133">请求</span><span class="sxs-lookup"><span data-stu-id="835ac-133">Request</span></span>

<span data-ttu-id="835ac-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="835ac-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_namedlocations"
}-->

```http
GET https://graph.microsoft.com/v1.0/identity/conditionalAccess/namedLocations
```

#### <a name="response"></a><span data-ttu-id="835ac-135">响应</span><span class="sxs-lookup"><span data-stu-id="835ac-135">Response</span></span>

<span data-ttu-id="835ac-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="835ac-136">The following is an example of the response.</span></span>

> <span data-ttu-id="835ac-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="835ac-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
### <a name="example-2-list-all-ipnamedlocations"></a><span data-ttu-id="835ac-139">示例2：列出所有 ipNamedLocations</span><span class="sxs-lookup"><span data-stu-id="835ac-139">Example 2: List all ipNamedLocations</span></span>

#### <a name="request"></a><span data-ttu-id="835ac-140">请求</span><span class="sxs-lookup"><span data-stu-id="835ac-140">Request</span></span>

<span data-ttu-id="835ac-141">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="835ac-141">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_namedlocations"
}-->

```http
GET https://graph.microsoft.com/v1.0/identity/conditionalAccess/namedLocations?$filter=isof('microsoft.graph.ipNamedLocation')
```

#### <a name="response"></a><span data-ttu-id="835ac-142">响应</span><span class="sxs-lookup"><span data-stu-id="835ac-142">Response</span></span>

<span data-ttu-id="835ac-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="835ac-143">The following is an example of the response.</span></span>

> <span data-ttu-id="835ac-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="835ac-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
### <a name="example-3-list-all-namedlocations-created-after-a-certain-date"></a><span data-ttu-id="835ac-146">示例3：列出在特定日期之后创建的所有 namedLocations</span><span class="sxs-lookup"><span data-stu-id="835ac-146">Example 3: List all namedLocations created after a certain date</span></span>

#### <a name="request"></a><span data-ttu-id="835ac-147">请求</span><span class="sxs-lookup"><span data-stu-id="835ac-147">Request</span></span>

<span data-ttu-id="835ac-148">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="835ac-148">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_namedlocations"
}-->

```http
GET https://graph.microsoft.com/v1.0/identity/conditionalAccess/namedLocations?$filter=createdDateTime ge 2019-09-01T00:00:00Z
```

#### <a name="response"></a><span data-ttu-id="835ac-149">响应</span><span class="sxs-lookup"><span data-stu-id="835ac-149">Response</span></span>

<span data-ttu-id="835ac-150">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="835ac-150">The following is an example of the response.</span></span>

> <span data-ttu-id="835ac-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="835ac-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
### <a name="example-4-list-all-countrynamedlocations-containing-a-certain-country-or-region"></a><span data-ttu-id="835ac-153">示例4：列出包含特定国家或地区的所有 countryNamedLocations</span><span class="sxs-lookup"><span data-stu-id="835ac-153">Example 4: List all countryNamedLocations containing a certain country or region</span></span>

#### <a name="request"></a><span data-ttu-id="835ac-154">请求</span><span class="sxs-lookup"><span data-stu-id="835ac-154">Request</span></span>

<span data-ttu-id="835ac-155">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="835ac-155">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_namedlocations"
}-->

```http
GET https://graph.microsoft.com/v1.0/identity/conditionalAccess/namedLocations?$filter=microsoft.graph.countryNamedLocation/countriesAndRegions/any(c: c eq 'CA')
```

#### <a name="response"></a><span data-ttu-id="835ac-156">响应</span><span class="sxs-lookup"><span data-stu-id="835ac-156">Response</span></span>

<span data-ttu-id="835ac-157">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="835ac-157">The following is an example of the response.</span></span>

> <span data-ttu-id="835ac-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="835ac-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
