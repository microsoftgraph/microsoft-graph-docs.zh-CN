---
title: 'cloudPcDeviceImage: getSourceImages'
description: 查看来自你的 Azure 订阅的所有托管图像资源的列表。 可以在云电脑上上传和使用这些源映像。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 244531c8dc1f54d7af3c901b45711431afc1992b
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378272"
---
# <a name="cloudpcdeviceimage-getsourceimages"></a><span data-ttu-id="3170d-104">cloudPcDeviceImage: getSourceImages</span><span class="sxs-lookup"><span data-stu-id="3170d-104">cloudPcDeviceImage: getSourceImages</span></span>

<span data-ttu-id="3170d-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3170d-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3170d-106">获取 [cloudPcSourceDeviceImage](../resources/cloudpcsourcedeviceimage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3170d-106">Get [cloudPcSourceDeviceImage](../resources/cloudpcsourcedeviceimage.md) objects.</span></span> <span data-ttu-id="3170d-107">查看 Azure Active Directory 订阅中所有托管图像资源的列表。</span><span class="sxs-lookup"><span data-stu-id="3170d-107">View a list of all the managed image resources from your Azure Active Directory subscriptions.</span></span>

## <a name="permissions"></a><span data-ttu-id="3170d-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="3170d-108">Permissions</span></span>

<span data-ttu-id="3170d-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3170d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3170d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="3170d-111">Permission type</span></span>|<span data-ttu-id="3170d-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3170d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3170d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3170d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3170d-114">CloudPC、CloudPC 和全部读。</span><span class="sxs-lookup"><span data-stu-id="3170d-114">CloudPC.ReadWrite.All, CloudPC.Read.All</span></span>|
|<span data-ttu-id="3170d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3170d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3170d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3170d-116">Not supported.</span></span>|
|<span data-ttu-id="3170d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="3170d-117">Application</span></span>|<span data-ttu-id="3170d-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="3170d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3170d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3170d-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/deviceImages/getSourceImages
```

## <a name="request-headers"></a><span data-ttu-id="3170d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="3170d-120">Request headers</span></span>

|<span data-ttu-id="3170d-121">名称</span><span class="sxs-lookup"><span data-stu-id="3170d-121">Name</span></span>|<span data-ttu-id="3170d-122">说明</span><span class="sxs-lookup"><span data-stu-id="3170d-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3170d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3170d-123">Authorization</span></span>|<span data-ttu-id="3170d-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3170d-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3170d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="3170d-126">Request body</span></span>

<span data-ttu-id="3170d-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3170d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3170d-128">响应</span><span class="sxs-lookup"><span data-stu-id="3170d-128">Response</span></span>

<span data-ttu-id="3170d-129">如果成功，此函数会 `200 OK` 在响应正文中返回响应代码和 [cloudPcSourceDeviceImage](../resources/cloudpcsourcedeviceimage.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="3170d-129">If successful, this function returns a `200 OK` response code and a [cloudPcSourceDeviceImage](../resources/cloudpcsourcedeviceimage.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3170d-130">示例</span><span class="sxs-lookup"><span data-stu-id="3170d-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3170d-131">请求</span><span class="sxs-lookup"><span data-stu-id="3170d-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "cloudpcdeviceimage_getsourceimages"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/deviceImages/getSourceImages
```

### <a name="response"></a><span data-ttu-id="3170d-132">响应</span><span class="sxs-lookup"><span data-stu-id="3170d-132">Response</span></span>

<span data-ttu-id="3170d-133">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="3170d-133">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.cloudPcSourceDeviceImage)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.cloudPcSourceDeviceImage",
      "id": "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ffff/resourceGroups/ExampleRG/providers/Microsoft.Compute/images/ExampleImage",
      "displayName": "Display Name value"
    }
  ]
}
```
