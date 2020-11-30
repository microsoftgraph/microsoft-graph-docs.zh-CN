---
title: 删除 cloudPcDeviceImage
description: 删除 cloudPcDeviceImage 对象。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: e6b5ad15ec2bf768a9b02cb49289c8028699f3ea
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378269"
---
# <a name="delete-cloudpcdeviceimage"></a><span data-ttu-id="d49d2-103">删除 cloudPcDeviceImage</span><span class="sxs-lookup"><span data-stu-id="d49d2-103">Delete cloudPcDeviceImage</span></span>

<span data-ttu-id="d49d2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d49d2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d49d2-105">删除 [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d49d2-105">Delete a [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d49d2-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="d49d2-106">Permissions</span></span>

<span data-ttu-id="d49d2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d49d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d49d2-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d49d2-109">Permission type</span></span>|<span data-ttu-id="d49d2-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d49d2-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d49d2-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d49d2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d49d2-112">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d49d2-112">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="d49d2-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d49d2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d49d2-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d49d2-114">Not supported.</span></span>|
|<span data-ttu-id="d49d2-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d49d2-115">Application</span></span>|<span data-ttu-id="d49d2-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d49d2-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d49d2-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d49d2-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /deviceManagement/virtualEndpoint/deviceImages/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d49d2-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="d49d2-118">Request headers</span></span>

|<span data-ttu-id="d49d2-119">名称</span><span class="sxs-lookup"><span data-stu-id="d49d2-119">Name</span></span>|<span data-ttu-id="d49d2-120">说明</span><span class="sxs-lookup"><span data-stu-id="d49d2-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d49d2-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d49d2-121">Authorization</span></span>|<span data-ttu-id="d49d2-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d49d2-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d49d2-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="d49d2-124">Request body</span></span>

<span data-ttu-id="d49d2-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d49d2-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d49d2-126">响应</span><span class="sxs-lookup"><span data-stu-id="d49d2-126">Response</span></span>

<span data-ttu-id="d49d2-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="d49d2-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="d49d2-128">示例</span><span class="sxs-lookup"><span data-stu-id="d49d2-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d49d2-129">请求</span><span class="sxs-lookup"><span data-stu-id="d49d2-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_deviceimages_from_virtualendpoint"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/deviceImages/{id}
```

### <a name="response"></a><span data-ttu-id="d49d2-130">响应</span><span class="sxs-lookup"><span data-stu-id="d49d2-130">Response</span></span>

<span data-ttu-id="d49d2-131">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d49d2-131">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
