---
title: 获取 printOperation
description: 检索 printOperation。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: dd03367e71a9c5273e294ac022d4ac9d8a5e2760
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46565627"
---
# <a name="get-printoperation"></a><span data-ttu-id="b01f4-103">获取 printOperation</span><span class="sxs-lookup"><span data-stu-id="b01f4-103">Get printOperation</span></span>

<span data-ttu-id="b01f4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b01f4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b01f4-105">检索[printOperation](../resources/printoperation.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b01f4-105">Retrieve the properties and relationships of a [printOperation](../resources/printoperation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b01f4-106">权限</span><span class="sxs-lookup"><span data-stu-id="b01f4-106">Permissions</span></span>
<span data-ttu-id="b01f4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b01f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b01f4-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b01f4-109">Permission type</span></span> | <span data-ttu-id="b01f4-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b01f4-110">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="b01f4-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b01f4-111">Delegated (work or school account)</span></span>| <span data-ttu-id="b01f4-112">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="b01f4-112">User.Read.All</span></span> |
|<span data-ttu-id="b01f4-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b01f4-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b01f4-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b01f4-114">Not Supported.</span></span>|
|<span data-ttu-id="b01f4-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b01f4-115">Application</span></span>|<span data-ttu-id="b01f4-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b01f4-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b01f4-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b01f4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/operations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b01f4-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="b01f4-118">Request headers</span></span>
| <span data-ttu-id="b01f4-119">名称</span><span class="sxs-lookup"><span data-stu-id="b01f4-119">Name</span></span>      |<span data-ttu-id="b01f4-120">说明</span><span class="sxs-lookup"><span data-stu-id="b01f4-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b01f4-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b01f4-121">Authorization</span></span> | <span data-ttu-id="b01f4-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b01f4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b01f4-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="b01f4-124">Request body</span></span>
<span data-ttu-id="b01f4-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b01f4-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="b01f4-126">响应</span><span class="sxs-lookup"><span data-stu-id="b01f4-126">Response</span></span>
<span data-ttu-id="b01f4-127">如果成功，此方法在 `200 OK` 响应正文中返回响应代码和[printOperation](../resources/printOperation.md)对象 (或**printOperation**) 的导数。</span><span class="sxs-lookup"><span data-stu-id="b01f4-127">If successful, this method returns a `200 OK` response code and a [printOperation](../resources/printOperation.md) object (or a derivative of **printOperation**) in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b01f4-128">示例</span><span class="sxs-lookup"><span data-stu-id="b01f4-128">Example</span></span>
### <a name="request"></a><span data-ttu-id="b01f4-129">请求</span><span class="sxs-lookup"><span data-stu-id="b01f4-129">Request</span></span>
<span data-ttu-id="b01f4-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b01f4-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="b01f4-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="b01f4-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printoperation"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/operations/{id}
```
# <a name="c"></a>[<span data-ttu-id="b01f4-132">C#</span><span class="sxs-lookup"><span data-stu-id="b01f4-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printoperation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b01f4-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b01f4-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printoperation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b01f4-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b01f4-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printoperation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b01f4-135">响应</span><span class="sxs-lookup"><span data-stu-id="b01f4-135">Response</span></span>
<span data-ttu-id="b01f4-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b01f4-136">The following is an example of the response.</span></span>
><span data-ttu-id="b01f4-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b01f4-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printOperation"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1199

{
    "@odata.context": "https://graph.microsoft-ppe.com/beta/$metadata#print/operations/$entity",
    "@odata.type": "#microsoft.graph.printerCreateOperation",
    "id": "81f4cca3-b3b7-47ea-9f88-7ddbf7208ef4",
    "createdDateTime": "2020-06-15T22:27:03.031849Z",
    "certificate": "{ceritificate}",
    "status": {
        "state": "succeeded",
        "description": "The operation has completed successfully."
    },
    "printer": {
        "registeredDateTime": "2020-06-15T22:27:12.0920077Z",
        "acceptingJobs": null,
        "isShared": false,
        "id": "e56f9cdd-acec-486f-a05e-b622ff0bcc7d",
        "name": "Test Printer",
        "manufacturer": "Test Printer Manufacturer",
        "model": "Test Printer Model",
        "isAcceptingJobs": null,
        "capabilities": null,
        "status": {
            "processingState": "unknown",
            "processingStateReasons": [],
            "processingStateDescription": ""
        },
        "location": {
            "latitude": null,
            "longitude": null
        },
        "defaults": {
            "copiesPerJob": 1,
            "finishings": []
        }
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get printOperation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
