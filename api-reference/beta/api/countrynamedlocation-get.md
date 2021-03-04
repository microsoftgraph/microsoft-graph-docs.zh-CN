---
title: 获取 countryNamedLocation
description: 检索 countryNamedlocation 对象的属性和关系。
localization_priority: Normal
author: dkershaw10
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 16e8a3e27eb0858cff682b2f28fb1179aaf05f0c
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50437252"
---
# <a name="get-countrynamedlocation"></a><span data-ttu-id="4b767-103">获取 countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="4b767-103">Get countryNamedLocation</span></span>

<span data-ttu-id="4b767-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4b767-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4b767-105">检索 [countryNamedLocation 对象的属性和](../resources/countryNamedLocation.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="4b767-105">Retrieve the properties and relationships of a [countryNamedLocation](../resources/countryNamedLocation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4b767-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="4b767-106">Permissions</span></span>

<span data-ttu-id="4b767-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4b767-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4b767-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4b767-109">Permission type</span></span>                        | <span data-ttu-id="4b767-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4b767-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4b767-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4b767-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4b767-112">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="4b767-112">Policy.Read.All</span></span> |
| <span data-ttu-id="4b767-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4b767-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4b767-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4b767-114">Not supported.</span></span> |
| <span data-ttu-id="4b767-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4b767-115">Application</span></span>                            | <span data-ttu-id="4b767-116">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="4b767-116">Policy.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4b767-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4b767-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/conditionalAccess/namedLocations/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4b767-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="4b767-118">Optional query parameters</span></span>

<span data-ttu-id="4b767-119">此方法支持 `select` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="4b767-119">This method supports the `select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="4b767-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="4b767-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="4b767-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="4b767-121">Request headers</span></span>

| <span data-ttu-id="4b767-122">名称</span><span class="sxs-lookup"><span data-stu-id="4b767-122">Name</span></span>      |<span data-ttu-id="4b767-123">说明</span><span class="sxs-lookup"><span data-stu-id="4b767-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4b767-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="4b767-124">Authorization</span></span> | <span data-ttu-id="4b767-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4b767-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4b767-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="4b767-127">Request body</span></span>

<span data-ttu-id="4b767-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4b767-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4b767-129">响应</span><span class="sxs-lookup"><span data-stu-id="4b767-129">Response</span></span>

<span data-ttu-id="4b767-130">如果成功，此方法在响应正文中返回响应代码和请求的 `200 OK` [countryNamedLocation](../resources/countrynamedlocation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4b767-130">If successful, this method returns a `200 OK` response code and the requested [countryNamedLocation](../resources/countrynamedlocation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4b767-131">示例</span><span class="sxs-lookup"><span data-stu-id="4b767-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4b767-132">请求</span><span class="sxs-lookup"><span data-stu-id="4b767-132">Request</span></span>

<span data-ttu-id="4b767-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4b767-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4b767-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="4b767-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_countrynamedlocation"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identity/conditionalAccess/namedLocations/1c4427fd-0885-4a3d-8b23-09a899ffa959
```
# <a name="c"></a>[<span data-ttu-id="4b767-135">C#</span><span class="sxs-lookup"><span data-stu-id="4b767-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-countrynamedlocation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4b767-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4b767-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-countrynamedlocation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4b767-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4b767-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-countrynamedlocation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4b767-138">Java</span><span class="sxs-lookup"><span data-stu-id="4b767-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-countrynamedlocation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4b767-139">响应</span><span class="sxs-lookup"><span data-stu-id="4b767-139">Response</span></span>

<span data-ttu-id="4b767-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4b767-140">The following is an example of the response.</span></span>

> <span data-ttu-id="4b767-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="4b767-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


