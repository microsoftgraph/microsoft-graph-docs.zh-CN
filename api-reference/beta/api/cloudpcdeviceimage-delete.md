---
title: 删除 cloudPcDeviceImage
description: 删除 cloudPcDeviceImage 对象。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 6e2e3a3bef480c8b269a57819f32f4a00e3b08f3
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52546859"
---
# <a name="delete-cloudpcdeviceimage"></a><span data-ttu-id="3b0ff-103">删除 cloudPcDeviceImage</span><span class="sxs-lookup"><span data-stu-id="3b0ff-103">Delete cloudPcDeviceImage</span></span>

<span data-ttu-id="3b0ff-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3b0ff-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3b0ff-105">删除 [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3b0ff-105">Delete a [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]
## <a name="permissions"></a><span data-ttu-id="3b0ff-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="3b0ff-106">Permissions</span></span>

<span data-ttu-id="3b0ff-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3b0ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b0ff-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="3b0ff-109">Permission type</span></span>|<span data-ttu-id="3b0ff-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3b0ff-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3b0ff-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3b0ff-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3b0ff-112">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b0ff-112">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="3b0ff-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3b0ff-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3b0ff-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="3b0ff-114">Not supported.</span></span>|
|<span data-ttu-id="3b0ff-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="3b0ff-115">Application</span></span>|<span data-ttu-id="3b0ff-116">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b0ff-116">CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3b0ff-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3b0ff-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /deviceManagement/virtualEndpoint/deviceImages/{id}
```

## <a name="request-headers"></a><span data-ttu-id="3b0ff-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="3b0ff-118">Request headers</span></span>

|<span data-ttu-id="3b0ff-119">名称</span><span class="sxs-lookup"><span data-stu-id="3b0ff-119">Name</span></span>|<span data-ttu-id="3b0ff-120">说明</span><span class="sxs-lookup"><span data-stu-id="3b0ff-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3b0ff-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3b0ff-121">Authorization</span></span>|<span data-ttu-id="3b0ff-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3b0ff-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b0ff-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="3b0ff-124">Request body</span></span>

<span data-ttu-id="3b0ff-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3b0ff-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3b0ff-126">响应</span><span class="sxs-lookup"><span data-stu-id="3b0ff-126">Response</span></span>

<span data-ttu-id="3b0ff-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="3b0ff-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="3b0ff-128">示例</span><span class="sxs-lookup"><span data-stu-id="3b0ff-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3b0ff-129">请求</span><span class="sxs-lookup"><span data-stu-id="3b0ff-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="3b0ff-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="3b0ff-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_deviceimages_from_virtualendpoint"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/deviceImages/{id}
```
# <a name="c"></a>[<span data-ttu-id="3b0ff-131">C#</span><span class="sxs-lookup"><span data-stu-id="3b0ff-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-deviceimages-from-virtualendpoint-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3b0ff-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3b0ff-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-deviceimages-from-virtualendpoint-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3b0ff-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3b0ff-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-deviceimages-from-virtualendpoint-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3b0ff-134">Java</span><span class="sxs-lookup"><span data-stu-id="3b0ff-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-deviceimages-from-virtualendpoint-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3b0ff-135">响应</span><span class="sxs-lookup"><span data-stu-id="3b0ff-135">Response</span></span>

<span data-ttu-id="3b0ff-136">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="3b0ff-136">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
