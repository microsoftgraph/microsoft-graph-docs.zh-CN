---
title: 获取 cloudPcDeviceImages
description: 读取 cloudPcDeviceImage 对象的属性和关系。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 1db3504d2915723d950ab6f52706429cedbd4765
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52546852"
---
# <a name="get-cloudpcdeviceimage"></a><span data-ttu-id="320e6-103">获取 cloudPcDeviceImage</span><span class="sxs-lookup"><span data-stu-id="320e6-103">Get cloudPcDeviceImage</span></span>

<span data-ttu-id="320e6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="320e6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="320e6-105">读取特定 [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="320e6-105">Read the properties and relationships of a specific [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]
## <a name="permissions"></a><span data-ttu-id="320e6-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="320e6-106">Permissions</span></span>

<span data-ttu-id="320e6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="320e6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="320e6-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="320e6-109">Permission type</span></span>|<span data-ttu-id="320e6-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="320e6-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="320e6-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="320e6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="320e6-112">CloudPC.Read.All、CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="320e6-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="320e6-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="320e6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="320e6-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="320e6-114">Not supported.</span></span>|
|<span data-ttu-id="320e6-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="320e6-115">Application</span></span>|<span data-ttu-id="320e6-116">CloudPC.Read.All、CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="320e6-116">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="320e6-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="320e6-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/deviceImages/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="320e6-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="320e6-118">Optional query parameters</span></span>

<span data-ttu-id="320e6-119">此方法支持 `$select` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="320e6-119">This method supports `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="320e6-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="320e6-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="320e6-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="320e6-121">Request headers</span></span>

| <span data-ttu-id="320e6-122">名称</span><span class="sxs-lookup"><span data-stu-id="320e6-122">Name</span></span>          | <span data-ttu-id="320e6-123">说明</span><span class="sxs-lookup"><span data-stu-id="320e6-123">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="320e6-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="320e6-124">Authorization</span></span> | <span data-ttu-id="320e6-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="320e6-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="320e6-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="320e6-127">Request body</span></span>

<span data-ttu-id="320e6-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="320e6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="320e6-129">响应</span><span class="sxs-lookup"><span data-stu-id="320e6-129">Response</span></span>

<span data-ttu-id="320e6-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="320e6-130">If successful, this method returns a `200 OK` response code and a [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="320e6-131">示例</span><span class="sxs-lookup"><span data-stu-id="320e6-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="320e6-132">请求</span><span class="sxs-lookup"><span data-stu-id="320e6-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="320e6-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="320e6-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_cloudpcdeviceimage"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/deviceImages/{id}
```
# <a name="c"></a>[<span data-ttu-id="320e6-134">C#</span><span class="sxs-lookup"><span data-stu-id="320e6-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-cloudpcdeviceimage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="320e6-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="320e6-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-cloudpcdeviceimage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="320e6-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="320e6-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-cloudpcdeviceimage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="320e6-137">Java</span><span class="sxs-lookup"><span data-stu-id="320e6-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-cloudpcdeviceimage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="320e6-138">响应</span><span class="sxs-lookup"><span data-stu-id="320e6-138">Response</span></span>

<span data-ttu-id="320e6-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="320e6-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cloudPcDeviceImage"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.cloudPcDeviceImage",
    "id": "eda7ed64-7705-4079-9d08-c2bd883f4fff",
    "displayName": "Display Name value",
    "osBuildNumber": "OS Build Number value",
    "operatingSystem": "Operating System value",
    "version": "Version value",
    "sourceImageResourceId": "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c58ffff/resourceGroups/Example/providers/Microsoft.Compute/images/exampleImage",
    "lastModifiedDateTime": "2020-11-03T07:03:44.97Z",
    "status": "pending",
    "statusDetails": null
  }
}
```
