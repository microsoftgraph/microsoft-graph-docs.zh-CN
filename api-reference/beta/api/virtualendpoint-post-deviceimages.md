---
title: 创建 cloudPcDeviceImage
description: Upload自定义操作系统映像，稍后可以在云电脑中预配该映像。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: e7da8717b9dcbf34d40de5bbcb08247d80d04514
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547090"
---
# <a name="create-cloudpcdeviceimage"></a><span data-ttu-id="2217f-103">创建 cloudPcDeviceImage</span><span class="sxs-lookup"><span data-stu-id="2217f-103">Create cloudPcDeviceImage</span></span>

<span data-ttu-id="2217f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2217f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2217f-105">创建新的 [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2217f-105">Create a new [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object.</span></span> <span data-ttu-id="2217f-106">Upload自定义操作系统映像，稍后可以在云电脑中预配该映像。</span><span class="sxs-lookup"><span data-stu-id="2217f-106">Upload a custom OS image that you can later provision on cloud PCs.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="2217f-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="2217f-107">Permissions</span></span>

<span data-ttu-id="2217f-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2217f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2217f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="2217f-110">Permission type</span></span>|<span data-ttu-id="2217f-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2217f-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2217f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2217f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2217f-113">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2217f-113">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="2217f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2217f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2217f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="2217f-115">Not supported.</span></span>|
|<span data-ttu-id="2217f-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="2217f-116">Application</span></span>|<span data-ttu-id="2217f-117">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2217f-117">CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2217f-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2217f-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/virtualEndpoint/deviceImages
```

## <a name="request-headers"></a><span data-ttu-id="2217f-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="2217f-119">Request headers</span></span>

| <span data-ttu-id="2217f-120">名称</span><span class="sxs-lookup"><span data-stu-id="2217f-120">Name</span></span>          | <span data-ttu-id="2217f-121">说明</span><span class="sxs-lookup"><span data-stu-id="2217f-121">Description</span></span>                |
| :------------ | :------------------------  |
| <span data-ttu-id="2217f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2217f-122">Authorization</span></span> | <span data-ttu-id="2217f-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2217f-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2217f-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2217f-125">Content-Type</span></span>  | <span data-ttu-id="2217f-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="2217f-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2217f-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="2217f-128">Request body</span></span>

<span data-ttu-id="2217f-129">在请求正文中，提供 [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2217f-129">In the request body, supply a JSON representation of the [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object.</span></span>

<span data-ttu-id="2217f-130">下表显示创建 [cloudPcDeviceImage 时所需的属性](../resources/cloudpcdeviceimage.md)。</span><span class="sxs-lookup"><span data-stu-id="2217f-130">The following table shows the properties that are required when you create the [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md).</span></span>

|<span data-ttu-id="2217f-131">属性</span><span class="sxs-lookup"><span data-stu-id="2217f-131">Property</span></span>|<span data-ttu-id="2217f-132">类型</span><span class="sxs-lookup"><span data-stu-id="2217f-132">Type</span></span>|<span data-ttu-id="2217f-133">说明</span><span class="sxs-lookup"><span data-stu-id="2217f-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2217f-134">displayName</span><span class="sxs-lookup"><span data-stu-id="2217f-134">displayName</span></span>|<span data-ttu-id="2217f-135">String</span><span class="sxs-lookup"><span data-stu-id="2217f-135">String</span></span>|<span data-ttu-id="2217f-136">图像的显示名称。</span><span class="sxs-lookup"><span data-stu-id="2217f-136">The image's display name.</span></span>|
|<span data-ttu-id="2217f-137">sourceImageResourceId</span><span class="sxs-lookup"><span data-stu-id="2217f-137">sourceImageResourceId</span></span>|<span data-ttu-id="2217f-138">String</span><span class="sxs-lookup"><span data-stu-id="2217f-138">String</span></span>|<span data-ttu-id="2217f-139">Azure 上的源图像资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="2217f-139">The ID of the source image resource on Azure.</span></span> <span data-ttu-id="2217f-140">所需格式："/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Compute/images/{imageName}"。</span><span class="sxs-lookup"><span data-stu-id="2217f-140">Required format: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Compute/images/{imageName}".</span></span>|
|<span data-ttu-id="2217f-141">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="2217f-141">operatingSystem</span></span>|<span data-ttu-id="2217f-142">String</span><span class="sxs-lookup"><span data-stu-id="2217f-142">String</span></span>|<span data-ttu-id="2217f-143">映像的操作系统。</span><span class="sxs-lookup"><span data-stu-id="2217f-143">The image's operating system.</span></span> <span data-ttu-id="2217f-144">例如：Windows 10 企业版。</span><span class="sxs-lookup"><span data-stu-id="2217f-144">For example: Windows 10 Enterprise.</span></span>|
|<span data-ttu-id="2217f-145">osBuildNumber</span><span class="sxs-lookup"><span data-stu-id="2217f-145">osBuildNumber</span></span>|<span data-ttu-id="2217f-146">String</span><span class="sxs-lookup"><span data-stu-id="2217f-146">String</span></span>|<span data-ttu-id="2217f-147">映像的操作系统生成版本。</span><span class="sxs-lookup"><span data-stu-id="2217f-147">The image's OS build version.</span></span> <span data-ttu-id="2217f-148">例如：1909。</span><span class="sxs-lookup"><span data-stu-id="2217f-148">For example: 1909.</span></span>|
|<span data-ttu-id="2217f-149">version</span><span class="sxs-lookup"><span data-stu-id="2217f-149">version</span></span>|<span data-ttu-id="2217f-150">String</span><span class="sxs-lookup"><span data-stu-id="2217f-150">String</span></span>|<span data-ttu-id="2217f-151">图像版本。</span><span class="sxs-lookup"><span data-stu-id="2217f-151">The image version.</span></span> <span data-ttu-id="2217f-152">例如：0.0.1、1.5.13。</span><span class="sxs-lookup"><span data-stu-id="2217f-152">For example: 0.0.1, 1.5.13.</span></span>|

## <a name="response"></a><span data-ttu-id="2217f-153">响应</span><span class="sxs-lookup"><span data-stu-id="2217f-153">Response</span></span>

<span data-ttu-id="2217f-154">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2217f-154">If successful, this method returns a `201 Created` response code and a [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2217f-155">示例</span><span class="sxs-lookup"><span data-stu-id="2217f-155">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2217f-156">请求</span><span class="sxs-lookup"><span data-stu-id="2217f-156">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="2217f-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="2217f-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_cloudpcdeviceimage_from_cloudpcdeviceimage"
}
-->

``` http
POST https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/deviceImages
Content-Type: application/json
Content-length: 363

{
  "@odata.type": "#microsoft.graph.cloudPcDeviceImage",
  "displayName": "Display Name value",
  "osBuildNumber": "OS Build Number value",
  "operatingSystem": "Operating System value",
  "version": "Version value",
  "sourceImageResourceId": "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c58ffff/resourceGroups/Example/providers/Microsoft.Compute/images/exampleImage"
}
```
# <a name="c"></a>[<span data-ttu-id="2217f-158">C#</span><span class="sxs-lookup"><span data-stu-id="2217f-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-cloudpcdeviceimage-from-cloudpcdeviceimage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2217f-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2217f-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-cloudpcdeviceimage-from-cloudpcdeviceimage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2217f-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2217f-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-cloudpcdeviceimage-from-cloudpcdeviceimage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2217f-161">Java</span><span class="sxs-lookup"><span data-stu-id="2217f-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-cloudpcdeviceimage-from-cloudpcdeviceimage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2217f-162">响应</span><span class="sxs-lookup"><span data-stu-id="2217f-162">Response</span></span>

<span data-ttu-id="2217f-163">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="2217f-163">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cloudPcDeviceImage"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-length: 508

{
  "@odata.type": "#microsoft.graph.cloudPcDeviceImage",
  "id": "eda7ed64-7705-4079-9d08-c2bd883fffff",
  "displayName": "Display Name value",
  "osBuildNumber": "OS Build Number value",
  "operatingSystem": "Operating System value",
  "version": "Version value",
  "sourceImageResourceId": "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c58ffff/resourceGroups/Example/providers/Microsoft.Compute/images/exampleImage",
  "lastModifiedDateTime": "2020-11-03T07:03:44.97Z",
  "status": "pending",
  "statusDetails": null
}
```
