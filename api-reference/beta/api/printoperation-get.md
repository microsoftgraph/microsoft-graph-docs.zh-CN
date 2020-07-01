---
title: 获取 printOperation
description: 检索 printOperation。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 85b0031d0bf4949a0309fbbe148c8f8119f0b032
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/01/2020
ms.locfileid: "45007149"
---
# <a name="get-printoperation"></a><span data-ttu-id="2fe3e-103">获取 printOperation</span><span class="sxs-lookup"><span data-stu-id="2fe3e-103">Get printOperation</span></span>

<span data-ttu-id="2fe3e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2fe3e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2fe3e-105">检索[printOperation](../resources/printoperation.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2fe3e-105">Retrieve the properties and relationships of a [printOperation](../resources/printoperation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2fe3e-106">权限</span><span class="sxs-lookup"><span data-stu-id="2fe3e-106">Permissions</span></span>
<span data-ttu-id="2fe3e-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="2fe3e-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="2fe3e-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2fe3e-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2fe3e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2fe3e-109">Permission type</span></span> | <span data-ttu-id="2fe3e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2fe3e-110">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="2fe3e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2fe3e-111">Delegated (work or school account)</span></span>| <span data-ttu-id="2fe3e-112">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="2fe3e-112">User.Read.All</span></span> |
|<span data-ttu-id="2fe3e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2fe3e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2fe3e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="2fe3e-114">Not Supported.</span></span>|
|<span data-ttu-id="2fe3e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="2fe3e-115">Application</span></span>|<span data-ttu-id="2fe3e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2fe3e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2fe3e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2fe3e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/operations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="2fe3e-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="2fe3e-118">Request headers</span></span>
| <span data-ttu-id="2fe3e-119">名称</span><span class="sxs-lookup"><span data-stu-id="2fe3e-119">Name</span></span>      |<span data-ttu-id="2fe3e-120">说明</span><span class="sxs-lookup"><span data-stu-id="2fe3e-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2fe3e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2fe3e-121">Authorization</span></span> | <span data-ttu-id="2fe3e-122">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="2fe3e-122">Bearer {token}.</span></span> <span data-ttu-id="2fe3e-123">Required.</span><span class="sxs-lookup"><span data-stu-id="2fe3e-123">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2fe3e-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="2fe3e-124">Request body</span></span>
<span data-ttu-id="2fe3e-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2fe3e-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="2fe3e-126">响应</span><span class="sxs-lookup"><span data-stu-id="2fe3e-126">Response</span></span>
<span data-ttu-id="2fe3e-127">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[printOperation](../resources/printOperation.md)对象（或**printOperation**的导数）。</span><span class="sxs-lookup"><span data-stu-id="2fe3e-127">If successful, this method returns a `200 OK` response code and a [printOperation](../resources/printOperation.md) object (or a derivative of **printOperation**) in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2fe3e-128">示例</span><span class="sxs-lookup"><span data-stu-id="2fe3e-128">Example</span></span>
### <a name="request"></a><span data-ttu-id="2fe3e-129">请求</span><span class="sxs-lookup"><span data-stu-id="2fe3e-129">Request</span></span>
<span data-ttu-id="2fe3e-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2fe3e-130">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_printoperation"
}-->
```http
GET https://graph.microsoft.com/beta/print/operations/{id}
```

### <a name="response"></a><span data-ttu-id="2fe3e-131">响应</span><span class="sxs-lookup"><span data-stu-id="2fe3e-131">Response</span></span>
<span data-ttu-id="2fe3e-132">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2fe3e-132">The following is an example of the response.</span></span>
><span data-ttu-id="2fe3e-133">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="2fe3e-133">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="2fe3e-134">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="2fe3e-134">All the properties will be returned from an actual call.</span></span>
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
