---
title: 创建 namedLocation
description: 创建新的 namedLocation。
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5e2188ddeeffbba37e72e2d74f9ccd930ee379d4
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46565986"
---
# <a name="create-namedlocation"></a><span data-ttu-id="24f66-103">创建 namedLocation</span><span class="sxs-lookup"><span data-stu-id="24f66-103">Create namedLocation</span></span>

<span data-ttu-id="24f66-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="24f66-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="24f66-105">创建新的[namedLocation](../resources/namedlocation.md)对象。</span><span class="sxs-lookup"><span data-stu-id="24f66-105">Create a new [namedLocation](../resources/namedlocation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="24f66-106">权限</span><span class="sxs-lookup"><span data-stu-id="24f66-106">Permissions</span></span>

<span data-ttu-id="24f66-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="24f66-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="24f66-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="24f66-109">Permission type</span></span>                        | <span data-ttu-id="24f66-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="24f66-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="24f66-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="24f66-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="24f66-112">Policy。 Read. All 和 ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="24f66-112">Policy.Read.All and Policy.ReadWrite.ConditionalAccess</span></span> |
| <span data-ttu-id="24f66-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="24f66-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="24f66-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="24f66-114">Not supported.</span></span> |
| <span data-ttu-id="24f66-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="24f66-115">Application</span></span>                            | <span data-ttu-id="24f66-116">Policy。 Read. All 和 ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="24f66-116">Policy.Read.All and Policy.ReadWrite.ConditionalAccess</span></span> |

## <a name="http-request"></a><span data-ttu-id="24f66-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="24f66-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identity/conditionalAccess/namedLocations
```

## <a name="request-headers"></a><span data-ttu-id="24f66-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="24f66-118">Request headers</span></span>

| <span data-ttu-id="24f66-119">名称</span><span class="sxs-lookup"><span data-stu-id="24f66-119">Name</span></span>          | <span data-ttu-id="24f66-120">说明</span><span class="sxs-lookup"><span data-stu-id="24f66-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="24f66-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="24f66-121">Authorization</span></span> | <span data-ttu-id="24f66-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="24f66-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="24f66-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="24f66-124">Content-Type</span></span>  | <span data-ttu-id="24f66-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="24f66-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="24f66-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="24f66-127">Request body</span></span>

<span data-ttu-id="24f66-128">在请求正文中，提供[ipNamedLocation](../resources/ipnamedlocation.md)或[COUNTRYNAMEDLOCATION](../resources/countrynamedlocation.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="24f66-128">In the request body, supply a JSON representation of an [ipNamedLocation](../resources/ipnamedlocation.md) or [countryNamedLocation](../resources/countrynamedlocation.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="24f66-129">响应</span><span class="sxs-lookup"><span data-stu-id="24f66-129">Response</span></span>

<span data-ttu-id="24f66-130">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和新的[IpNamedLocation](../resources/ipnamedlocation.md)或[countryNamedLocation](../resources/countrynamedlocation.md)对象。</span><span class="sxs-lookup"><span data-stu-id="24f66-130">If successful, this method returns a `201 Created`response code and a new [ipNamedLocation](../resources/ipnamedlocation.md) or [countryNamedLocation](../resources/countrynamedlocation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="24f66-131">示例</span><span class="sxs-lookup"><span data-stu-id="24f66-131">Examples</span></span>

### <a name="example-1-create-an-ipnamedlocation"></a><span data-ttu-id="24f66-132">示例1：创建 ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="24f66-132">Example 1: Create an ipNamedLocation</span></span>

#### <a name="request"></a><span data-ttu-id="24f66-133">请求</span><span class="sxs-lookup"><span data-stu-id="24f66-133">Request</span></span>

<span data-ttu-id="24f66-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="24f66-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="24f66-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="24f66-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_namedlocation_from_conditionalaccessroot"
}-->

```http
POST https://graph.microsoft.com/v1.0/identity/conditionalAccess/namedLocations
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
# <a name="c"></a>[<span data-ttu-id="24f66-136">C#</span><span class="sxs-lookup"><span data-stu-id="24f66-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-namedlocation-from-conditionalaccessroot-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="24f66-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="24f66-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-namedlocation-from-conditionalaccessroot-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="24f66-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="24f66-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-namedlocation-from-conditionalaccessroot-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="24f66-139">Java</span><span class="sxs-lookup"><span data-stu-id="24f66-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-namedlocation-from-conditionalaccessroot-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="24f66-140">响应</span><span class="sxs-lookup"><span data-stu-id="24f66-140">Response</span></span>

<span data-ttu-id="24f66-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="24f66-141">The following is an example of the response.</span></span>

> <span data-ttu-id="24f66-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="24f66-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.namedLocation"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#namedLocations/$entity",
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
### <a name="example-2-create-a-countrynamedlocation"></a><span data-ttu-id="24f66-144">示例2：创建 countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="24f66-144">Example 2: Create a countryNamedLocation</span></span>

#### <a name="request"></a><span data-ttu-id="24f66-145">请求</span><span class="sxs-lookup"><span data-stu-id="24f66-145">Request</span></span>

<span data-ttu-id="24f66-146">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="24f66-146">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_namedlocation_from_conditionalaccessroot"
}-->

```http
POST https://graph.microsoft.com/v1.0/identity/conditionalAccess/namedLocations
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

#### <a name="response"></a><span data-ttu-id="24f66-147">响应</span><span class="sxs-lookup"><span data-stu-id="24f66-147">Response</span></span>

<span data-ttu-id="24f66-148">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="24f66-148">The following is an example of the response.</span></span>

> <span data-ttu-id="24f66-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="24f66-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.namedLocation"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#namedLocations/$entity",
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
