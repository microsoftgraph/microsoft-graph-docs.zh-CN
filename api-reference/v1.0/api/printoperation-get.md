---
title: 获取 printOperation
description: 检索 printOperation。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: ccd4960f4b8da00b2352feda7bb6106523958dcc
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771363"
---
# <a name="get-printoperation"></a><span data-ttu-id="38756-103">获取 printOperation</span><span class="sxs-lookup"><span data-stu-id="38756-103">Get printOperation</span></span>
<span data-ttu-id="38756-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="38756-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="38756-105">检索 [printOperation 对象的属性和](../resources/printoperation.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="38756-105">Retrieve the properties and relationships of a [printOperation](../resources/printoperation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="38756-106">权限</span><span class="sxs-lookup"><span data-stu-id="38756-106">Permissions</span></span>
<span data-ttu-id="38756-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="38756-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="38756-109">登录的用户必须是打印机 [管理员](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)。</span><span class="sxs-lookup"><span data-stu-id="38756-109">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="38756-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="38756-110">Permission type</span></span> | <span data-ttu-id="38756-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="38756-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="38756-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="38756-112">Delegated (work or school account)</span></span>| <span data-ttu-id="38756-113">Printer.Create、Printer.ReadWrite.All、Printer.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="38756-113">Printer.Create, Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="38756-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="38756-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="38756-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="38756-115">Not Supported.</span></span>|
|<span data-ttu-id="38756-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="38756-116">Application</span></span>| <span data-ttu-id="38756-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="38756-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="38756-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="38756-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/operations/{printOperationId}
```

## <a name="request-headers"></a><span data-ttu-id="38756-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="38756-119">Request headers</span></span>
|<span data-ttu-id="38756-120">名称</span><span class="sxs-lookup"><span data-stu-id="38756-120">Name</span></span>|<span data-ttu-id="38756-121">说明</span><span class="sxs-lookup"><span data-stu-id="38756-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="38756-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="38756-122">Authorization</span></span>|<span data-ttu-id="38756-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="38756-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="38756-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="38756-125">Request body</span></span>
<span data-ttu-id="38756-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="38756-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="38756-127">响应</span><span class="sxs-lookup"><span data-stu-id="38756-127">Response</span></span>
<span data-ttu-id="38756-128">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [printOperation](../resources/printOperation.md) (**printOperation**) 派生对象。</span><span class="sxs-lookup"><span data-stu-id="38756-128">If successful, this method returns a `200 OK` response code and a [printOperation](../resources/printOperation.md) object (or a derivative of **printOperation**) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="38756-129">示例</span><span class="sxs-lookup"><span data-stu-id="38756-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="38756-130">请求</span><span class="sxs-lookup"><span data-stu-id="38756-130">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="38756-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="38756-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printoperation"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/operations/{printOperationId}
```
# <a name="c"></a>[<span data-ttu-id="38756-132">C#</span><span class="sxs-lookup"><span data-stu-id="38756-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printoperation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="38756-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="38756-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printoperation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="38756-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="38756-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printoperation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="38756-135">Java</span><span class="sxs-lookup"><span data-stu-id="38756-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-printoperation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="38756-136">响应</span><span class="sxs-lookup"><span data-stu-id="38756-136">Response</span></span>
<span data-ttu-id="38756-137">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="38756-137">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printOperation"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/operations/$entity",
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
        "isShared": false,
        "id": "e56f9cdd-acec-486f-a05e-b622ff0bcc7d",
        "displayName": "Test Printer",
        "manufacturer": "Test Printer Manufacturer",
        "model": "Test Printer Model",
        "isAcceptingJobs": null,
        "status": {
            "state": "unknown",
            "details": [],
            "description": ""
        },
        "location": {
            "latitude": null,
            "longitude": null
        }
    }
}
```

