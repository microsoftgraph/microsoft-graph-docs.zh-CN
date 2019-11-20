---
title: 获取 countryNamedLocation
description: 检索 countryNamedlocation 对象的属性和关系。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: bd6ec395532124daa94dc60f895f22a6c2951a4b
ms.sourcegitcommit: d40d2a9266bd376d713382925323aefab285ed69
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/20/2019
ms.locfileid: "38747758"
---
# <a name="get-countrynamedlocation"></a><span data-ttu-id="cda2f-103">获取 countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="cda2f-103">Get countryNamedLocation</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cda2f-104">检索[countryNamedLocation](../resources/countryNamedLocation.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cda2f-104">Retrieve the properties and relationships of a [countryNamedLocation](../resources/countryNamedLocation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cda2f-105">权限</span><span class="sxs-lookup"><span data-stu-id="cda2f-105">Permissions</span></span>

<span data-ttu-id="cda2f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cda2f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cda2f-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="cda2f-108">Permission type</span></span>                        | <span data-ttu-id="cda2f-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cda2f-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="cda2f-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cda2f-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="cda2f-111">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="cda2f-111">Policy.Read.All</span></span> |
| <span data-ttu-id="cda2f-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cda2f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cda2f-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="cda2f-113">Not supported.</span></span> |
| <span data-ttu-id="cda2f-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="cda2f-114">Application</span></span>                            | <span data-ttu-id="cda2f-115">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="cda2f-115">Policy.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cda2f-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cda2f-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /conditionalAccess/namedLocations/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cda2f-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="cda2f-117">Optional query parameters</span></span>

<span data-ttu-id="cda2f-118">此方法支持`select` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="cda2f-118">This method supports the `select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="cda2f-119">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="cda2f-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="cda2f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="cda2f-120">Request headers</span></span>

| <span data-ttu-id="cda2f-121">名称</span><span class="sxs-lookup"><span data-stu-id="cda2f-121">Name</span></span>      |<span data-ttu-id="cda2f-122">说明</span><span class="sxs-lookup"><span data-stu-id="cda2f-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="cda2f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cda2f-123">Authorization</span></span> | <span data-ttu-id="cda2f-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cda2f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cda2f-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="cda2f-126">Request body</span></span>

<span data-ttu-id="cda2f-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cda2f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cda2f-128">响应</span><span class="sxs-lookup"><span data-stu-id="cda2f-128">Response</span></span>

<span data-ttu-id="cda2f-129">如果成功，此方法在响应`200 OK`正文中返回响应代码和请求的[countryNamedLocation](../resources/countrynamedlocation.md)对象。</span><span class="sxs-lookup"><span data-stu-id="cda2f-129">If successful, this method returns a `200 OK` response code and the requested [countryNamedLocation](../resources/countrynamedlocation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cda2f-130">示例</span><span class="sxs-lookup"><span data-stu-id="cda2f-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cda2f-131">请求</span><span class="sxs-lookup"><span data-stu-id="cda2f-131">Request</span></span>

<span data-ttu-id="cda2f-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="cda2f-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="cda2f-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="cda2f-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_countrynamedlocation"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/conditionalAccess/namedLocations/1c4427fd-0885-4a3d-8b23-09a899ffa959
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="cda2f-134">C#</span><span class="sxs-lookup"><span data-stu-id="cda2f-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-countrynamedlocation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cda2f-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cda2f-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-countrynamedlocation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="cda2f-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cda2f-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-countrynamedlocation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="cda2f-137">响应</span><span class="sxs-lookup"><span data-stu-id="cda2f-137">Response</span></span>

<span data-ttu-id="cda2f-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="cda2f-138">The following is an example of the response.</span></span>

> <span data-ttu-id="cda2f-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="cda2f-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
