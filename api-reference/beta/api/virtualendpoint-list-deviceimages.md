---
title: 列出 cloudPcDeviceImages
description: 列出上载到云电脑的 OS 映像的属性和关系。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 4d392331b2cb07446374275d0ffb8e606fe7d99d
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378313"
---
# <a name="list-deviceimages"></a><span data-ttu-id="461b3-103">列出 deviceImages</span><span class="sxs-lookup"><span data-stu-id="461b3-103">List deviceImages</span></span>

<span data-ttu-id="461b3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="461b3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="461b3-105">列出 (OS 映像) 上载到云电脑的 [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="461b3-105">List the properties and relationships of the [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) objects (OS images) uploaded to cloud PC.</span></span>

## <a name="permissions"></a><span data-ttu-id="461b3-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="461b3-106">Permissions</span></span>

<span data-ttu-id="461b3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="461b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="461b3-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="461b3-109">Permission type</span></span>|<span data-ttu-id="461b3-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="461b3-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="461b3-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="461b3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="461b3-112">CloudPC、CloudPC 和全部读。</span><span class="sxs-lookup"><span data-stu-id="461b3-112">CloudPC.ReadWrite.All, CloudPC.Read.All</span></span>|
|<span data-ttu-id="461b3-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="461b3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="461b3-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="461b3-114">Not supported.</span></span>|
|<span data-ttu-id="461b3-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="461b3-115">Application</span></span>|<span data-ttu-id="461b3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="461b3-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="461b3-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="461b3-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/deviceImages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="461b3-118">可选查询参数</span><span class="sxs-lookup"><span data-stu-id="461b3-118">Optional query parameters</span></span>

<span data-ttu-id="461b3-119">此方法支持 `$select` 和 `$filter` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="461b3-119">This method supports `$select` and `$filter` OData query parameters to help customize the response.</span></span> <span data-ttu-id="461b3-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="461b3-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="461b3-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="461b3-121">Request headers</span></span>

| <span data-ttu-id="461b3-122">名称</span><span class="sxs-lookup"><span data-stu-id="461b3-122">Name</span></span>          | <span data-ttu-id="461b3-123">说明</span><span class="sxs-lookup"><span data-stu-id="461b3-123">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="461b3-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="461b3-124">Authorization</span></span> | <span data-ttu-id="461b3-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="461b3-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="461b3-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="461b3-127">Request body</span></span>

<span data-ttu-id="461b3-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="461b3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="461b3-129">响应</span><span class="sxs-lookup"><span data-stu-id="461b3-129">Response</span></span>

<span data-ttu-id="461b3-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="461b3-130">If successful, this method returns a `200 OK` response code and a collection of [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="461b3-131">示例</span><span class="sxs-lookup"><span data-stu-id="461b3-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="461b3-132">请求</span><span class="sxs-lookup"><span data-stu-id="461b3-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_cloudpcdeviceimages"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/deviceImages
```

### <a name="response"></a><span data-ttu-id="461b3-133">响应</span><span class="sxs-lookup"><span data-stu-id="461b3-133">Response</span></span>

<span data-ttu-id="461b3-134">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="461b3-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.cloudPcDeviceImage)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.cloudPcDeviceImage",
      "id": "eda7ed64-7705-4079-9d08-c2bd883fffff",
      "displayName": "Display Name value",
      "osBuildNumber": "OS Build Number value",
      "operatingSystem": "Operating System value",
      "version": "Version value",
      "sourceImageResourceId": "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ffff/resourceGroups/ExampleRG/providers/Microsoft.Compute/images/ExampleImage",
      "lastModifiedDateTime": "2020-11-03T07:03:44Z",
      "status": "pending",
      "statusDetails": null
    }
  ]
}
```
