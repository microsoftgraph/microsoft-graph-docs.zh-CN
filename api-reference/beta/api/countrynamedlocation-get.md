---
title: 获取 countryNamedLocation
description: 检索 countryNamedlocation 对象的属性和关系。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 14ac09bc9fdcfbecd660d3eea9a09917702ae9e3
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48956581"
---
# <a name="get-countrynamedlocation"></a><span data-ttu-id="80f0a-103">获取 countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="80f0a-103">Get countryNamedLocation</span></span>

<span data-ttu-id="80f0a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="80f0a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="80f0a-105">检索 [countryNamedLocation](../resources/countryNamedLocation.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="80f0a-105">Retrieve the properties and relationships of a [countryNamedLocation](../resources/countryNamedLocation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="80f0a-106">权限</span><span class="sxs-lookup"><span data-stu-id="80f0a-106">Permissions</span></span>

<span data-ttu-id="80f0a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="80f0a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="80f0a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="80f0a-109">Permission type</span></span>                        | <span data-ttu-id="80f0a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="80f0a-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="80f0a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="80f0a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="80f0a-112">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="80f0a-112">Policy.Read.All</span></span> |
| <span data-ttu-id="80f0a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="80f0a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="80f0a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="80f0a-114">Not supported.</span></span> |
| <span data-ttu-id="80f0a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="80f0a-115">Application</span></span>                            | <span data-ttu-id="80f0a-116">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="80f0a-116">Policy.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="80f0a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="80f0a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/conditionalAccess/namedLocations/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="80f0a-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="80f0a-118">Optional query parameters</span></span>

<span data-ttu-id="80f0a-119">此方法支持 `select` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="80f0a-119">This method supports the `select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="80f0a-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="80f0a-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="80f0a-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="80f0a-121">Request headers</span></span>

| <span data-ttu-id="80f0a-122">名称</span><span class="sxs-lookup"><span data-stu-id="80f0a-122">Name</span></span>      |<span data-ttu-id="80f0a-123">说明</span><span class="sxs-lookup"><span data-stu-id="80f0a-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="80f0a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="80f0a-124">Authorization</span></span> | <span data-ttu-id="80f0a-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="80f0a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="80f0a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="80f0a-127">Request body</span></span>

<span data-ttu-id="80f0a-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="80f0a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="80f0a-129">响应</span><span class="sxs-lookup"><span data-stu-id="80f0a-129">Response</span></span>

<span data-ttu-id="80f0a-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和请求的 [countryNamedLocation](../resources/countrynamedlocation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="80f0a-130">If successful, this method returns a `200 OK` response code and the requested [countryNamedLocation](../resources/countrynamedlocation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="80f0a-131">示例</span><span class="sxs-lookup"><span data-stu-id="80f0a-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="80f0a-132">请求</span><span class="sxs-lookup"><span data-stu-id="80f0a-132">Request</span></span>

<span data-ttu-id="80f0a-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="80f0a-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="80f0a-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="80f0a-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_countrynamedlocation"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identity/conditionalAccess/namedLocations/1c4427fd-0885-4a3d-8b23-09a899ffa959
```
# <a name="c"></a>[<span data-ttu-id="80f0a-135">C#</span><span class="sxs-lookup"><span data-stu-id="80f0a-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-countrynamedlocation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="80f0a-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="80f0a-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-countrynamedlocation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="80f0a-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="80f0a-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-countrynamedlocation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="80f0a-138">Java</span><span class="sxs-lookup"><span data-stu-id="80f0a-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-countrynamedlocation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="80f0a-139">响应</span><span class="sxs-lookup"><span data-stu-id="80f0a-139">Response</span></span>

<span data-ttu-id="80f0a-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="80f0a-140">The following is an example of the response.</span></span>

> <span data-ttu-id="80f0a-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="80f0a-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.countryNamedLocation"
} -->

```http
HTTP/1.1 200 OK
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
  "description": "Get countryNamedLocation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


