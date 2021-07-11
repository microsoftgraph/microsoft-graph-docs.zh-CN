---
title: cloudPcDeviceImage：重新加载
description: 重新加载 cloudPcDeviceImage 对象。
author: RuiHou105
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: ab636894279317ef18b4f41eb86081ac159ded59
ms.sourcegitcommit: 3873c85f53e026073addca92d31d234af244444c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/10/2021
ms.locfileid: "53367044"
---
# <a name="cloudpcdeviceimage-reupload"></a><span data-ttu-id="76c66-103">cloudPcDeviceImage：重新加载</span><span class="sxs-lookup"><span data-stu-id="76c66-103">cloudPcDeviceImage: reupload</span></span>

<span data-ttu-id="76c66-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="76c66-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="76c66-105">重新加载 [无法上载的 cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="76c66-105">Reupload a [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object that failed to upload.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]
## <a name="permissions"></a><span data-ttu-id="76c66-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="76c66-106">Permissions</span></span>

<span data-ttu-id="76c66-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="76c66-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76c66-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="76c66-109">Permission type</span></span>|<span data-ttu-id="76c66-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="76c66-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="76c66-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="76c66-111">Delegated (work or school account)</span></span>|<span data-ttu-id="76c66-112">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76c66-112">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="76c66-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="76c66-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="76c66-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="76c66-114">Not supported.</span></span>|
|<span data-ttu-id="76c66-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="76c66-115">Application</span></span>|<span data-ttu-id="76c66-116">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76c66-116">CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="76c66-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="76c66-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/virtualEndpoint/deviceImages/{cloudPcDeviceImageId}/reupload
```

## <a name="request-headers"></a><span data-ttu-id="76c66-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="76c66-118">Request headers</span></span>

|<span data-ttu-id="76c66-119">名称</span><span class="sxs-lookup"><span data-stu-id="76c66-119">Name</span></span>|<span data-ttu-id="76c66-120">说明</span><span class="sxs-lookup"><span data-stu-id="76c66-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="76c66-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="76c66-121">Authorization</span></span>|<span data-ttu-id="76c66-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="76c66-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="76c66-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="76c66-124">Request body</span></span>

<span data-ttu-id="76c66-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="76c66-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="76c66-126">响应</span><span class="sxs-lookup"><span data-stu-id="76c66-126">Response</span></span>

<span data-ttu-id="76c66-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="76c66-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="76c66-128">示例</span><span class="sxs-lookup"><span data-stu-id="76c66-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="76c66-129">请求</span><span class="sxs-lookup"><span data-stu-id="76c66-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "reupload_deviceimages_from_virtualendpoint"
}
-->

``` http
POST https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/deviceImages/{cloudPcDeviceImageId}/reupload
```

### <a name="response"></a><span data-ttu-id="76c66-130">响应</span><span class="sxs-lookup"><span data-stu-id="76c66-130">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
