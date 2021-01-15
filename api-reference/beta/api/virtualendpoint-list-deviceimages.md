---
title: 列出 cloudPcDeviceImages
description: 列出上载到云电脑的操作系统映像的属性和关系。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: c1e278ac26e86417432159e6a191a6bf0606813b
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2021
ms.locfileid: "49873974"
---
# <a name="list-deviceimages"></a><span data-ttu-id="22d3c-103">列出 deviceImages</span><span class="sxs-lookup"><span data-stu-id="22d3c-103">List deviceImages</span></span>

<span data-ttu-id="22d3c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22d3c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="22d3c-105">列出已上载到云电脑 (操作系统映像) [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="22d3c-105">List the properties and relationships of the [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) objects (OS images) uploaded to cloud PC.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="22d3c-106">权限</span><span class="sxs-lookup"><span data-stu-id="22d3c-106">Permissions</span></span>

<span data-ttu-id="22d3c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="22d3c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22d3c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="22d3c-109">Permission type</span></span>|<span data-ttu-id="22d3c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="22d3c-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22d3c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="22d3c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="22d3c-112">CloudPC.Read.All、CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22d3c-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="22d3c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="22d3c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22d3c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="22d3c-114">Not supported.</span></span>|
|<span data-ttu-id="22d3c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="22d3c-115">Application</span></span>|<span data-ttu-id="22d3c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="22d3c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="22d3c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="22d3c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/deviceImages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="22d3c-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="22d3c-118">Optional query parameters</span></span>

<span data-ttu-id="22d3c-119">此方法支持 `$select` `$filter` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="22d3c-119">This method supports `$select` and `$filter` OData query parameters to help customize the response.</span></span> <span data-ttu-id="22d3c-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="22d3c-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="22d3c-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="22d3c-121">Request headers</span></span>

| <span data-ttu-id="22d3c-122">名称</span><span class="sxs-lookup"><span data-stu-id="22d3c-122">Name</span></span>          | <span data-ttu-id="22d3c-123">说明</span><span class="sxs-lookup"><span data-stu-id="22d3c-123">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="22d3c-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="22d3c-124">Authorization</span></span> | <span data-ttu-id="22d3c-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="22d3c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="22d3c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="22d3c-127">Request body</span></span>

<span data-ttu-id="22d3c-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="22d3c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="22d3c-129">响应</span><span class="sxs-lookup"><span data-stu-id="22d3c-129">Response</span></span>

<span data-ttu-id="22d3c-130">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="22d3c-130">If successful, this method returns a `200 OK` response code and a collection of [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="22d3c-131">示例</span><span class="sxs-lookup"><span data-stu-id="22d3c-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="22d3c-132">请求</span><span class="sxs-lookup"><span data-stu-id="22d3c-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="22d3c-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="22d3c-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_cloudpcdeviceimages"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/deviceImages
```
# <a name="c"></a>[<span data-ttu-id="22d3c-134">C#</span><span class="sxs-lookup"><span data-stu-id="22d3c-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-cloudpcdeviceimages-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="22d3c-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="22d3c-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-cloudpcdeviceimages-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="22d3c-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="22d3c-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-cloudpcdeviceimages-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="22d3c-137">Java</span><span class="sxs-lookup"><span data-stu-id="22d3c-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-cloudpcdeviceimages-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="22d3c-138">响应</span><span class="sxs-lookup"><span data-stu-id="22d3c-138">Response</span></span>

<span data-ttu-id="22d3c-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="22d3c-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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
