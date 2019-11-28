---
title: 创建 namedLocation
description: 创建新的 namedLocation。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 21927e1cc85048603217a1067d40274c5d6c80b7
ms.sourcegitcommit: fce7ce328f0c88c6310af9cc85d12bcebc88a6c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/28/2019
ms.locfileid: "39636776"
---
# <a name="create-namedlocation"></a><span data-ttu-id="c2d0f-103">创建 namedLocation</span><span class="sxs-lookup"><span data-stu-id="c2d0f-103">Create namedLocation</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c2d0f-104">创建新的[namedLocation](../resources/namedlocation.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c2d0f-104">Create a new [namedLocation](../resources/namedlocation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c2d0f-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="c2d0f-105">Permissions</span></span>

<span data-ttu-id="c2d0f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c2d0f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c2d0f-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="c2d0f-108">Permission type</span></span>                        | <span data-ttu-id="c2d0f-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c2d0f-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c2d0f-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c2d0f-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="c2d0f-111">Policy.ReadWrite.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="c2d0f-111">Policy.ReadWrite.ConditionalAccess</span></span> |
| <span data-ttu-id="c2d0f-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c2d0f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c2d0f-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="c2d0f-113">Not supported.</span></span> |
| <span data-ttu-id="c2d0f-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="c2d0f-114">Application</span></span>                            | <span data-ttu-id="c2d0f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c2d0f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c2d0f-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c2d0f-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /conditionalAccess/namedLocations
```

## <a name="request-headers"></a><span data-ttu-id="c2d0f-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="c2d0f-117">Request headers</span></span>

| <span data-ttu-id="c2d0f-118">名称</span><span class="sxs-lookup"><span data-stu-id="c2d0f-118">Name</span></span>          | <span data-ttu-id="c2d0f-119">说明</span><span class="sxs-lookup"><span data-stu-id="c2d0f-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="c2d0f-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="c2d0f-120">Authorization</span></span> | <span data-ttu-id="c2d0f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c2d0f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c2d0f-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c2d0f-123">Content-Type</span></span>  | <span data-ttu-id="c2d0f-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="c2d0f-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c2d0f-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c2d0f-126">Request body</span></span>

<span data-ttu-id="c2d0f-127">在请求正文中，提供[ipNamedLocation](../resources/ipnamedlocation.md)或[COUNTRYNAMEDLOCATION](../resources/countrynamedlocation.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c2d0f-127">In the request body, supply a JSON representation of an [ipNamedLocation](../resources/ipnamedlocation.md) or [countryNamedLocation](../resources/countrynamedlocation.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="c2d0f-128">响应</span><span class="sxs-lookup"><span data-stu-id="c2d0f-128">Response</span></span>

<span data-ttu-id="c2d0f-129">如果成功，此方法在响应`201 Created`正文中返回响应代码和新的[ipNamedLocation](../resources/ipnamedlocation.md)或[countryNamedLocation](../resources/countrynamedlocation.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c2d0f-129">If successful, this method returns a `201 Created`response code and a new [ipNamedLocation](../resources/ipnamedlocation.md) or [countryNamedLocation](../resources/countrynamedlocation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c2d0f-130">示例</span><span class="sxs-lookup"><span data-stu-id="c2d0f-130">Examples</span></span>

### <a name="example-1-create-an-ipnamedlocation"></a><span data-ttu-id="c2d0f-131">示例1：创建 ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="c2d0f-131">Example 1: Create an ipNamedLocation</span></span>

#### <a name="request"></a><span data-ttu-id="c2d0f-132">请求</span><span class="sxs-lookup"><span data-stu-id="c2d0f-132">Request</span></span>

<span data-ttu-id="c2d0f-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c2d0f-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c2d0f-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="c2d0f-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_namedlocation_from_conditionalaccessroot"
}-->

```http
POST https://graph.microsoft.com/beta/conditionalAccess/namedLocations
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.ipNamedLocation",
    "displayName": "Untrusted IP named location",
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
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c2d0f-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c2d0f-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-namedlocation-from-conditionalaccessroot-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c2d0f-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c2d0f-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-namedlocation-from-conditionalaccessroot-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c2d0f-137">响应</span><span class="sxs-lookup"><span data-stu-id="c2d0f-137">Response</span></span>

<span data-ttu-id="c2d0f-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c2d0f-138">The following is an example of the response.</span></span>

> <span data-ttu-id="c2d0f-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c2d0f-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.namedLocation"
} -->

```http
HTTP/1.1 201 Created
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
### <a name="example-2-create-a-countrynamedlocation"></a><span data-ttu-id="c2d0f-141">示例2：创建 countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="c2d0f-141">Example 2: Create a countryNamedLocation</span></span>

#### <a name="request"></a><span data-ttu-id="c2d0f-142">请求</span><span class="sxs-lookup"><span data-stu-id="c2d0f-142">Request</span></span>

<span data-ttu-id="c2d0f-143">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c2d0f-143">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_namedlocation_from_conditionalaccessroot"
}-->

```http
POST https://graph.microsoft.com/beta/conditionalAccess/namedLocations
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.countryNamedLocation",
    "displayName": "Named location with unknown countries and regions",
    "countriesAndRegions": [
        "US",
        "GB"
    ],
    "includeUnknownCountriesAndRegions": true
}
```

#### <a name="response"></a><span data-ttu-id="c2d0f-144">响应</span><span class="sxs-lookup"><span data-stu-id="c2d0f-144">Response</span></span>

<span data-ttu-id="c2d0f-145">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c2d0f-145">The following is an example of the response.</span></span>

> <span data-ttu-id="c2d0f-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c2d0f-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.namedLocation"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#namedLocations/$entity",
    "@odata.type": "#microsoft.graph.countryNamedLocation",
    "id": "1c4427fd-0885-4a3d-8b23-09a899ffa959",
    "displayName": "Named location with unknown countries and regions",
    "modifiedDateTime": "2019-09-04T01:08:02.5249255Z",
    "createdDateTime": "2019-09-04T01:08:02.5249255Z",
    "countriesAndRegions": [
        "US",
        "GB"
    ],
    "includeUnknownCountriesAndRegions": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create namedLocation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
