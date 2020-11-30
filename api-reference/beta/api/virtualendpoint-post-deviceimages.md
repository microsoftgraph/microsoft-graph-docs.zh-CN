---
title: 创建 cloudPcDeviceImage
description: 上载稍后可在云电脑上预配的自定义 OS 映像。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 7b2e60355bfe4db8eee014ac2290c83d146eea37
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378310"
---
# <a name="create-cloudpcdeviceimage"></a><span data-ttu-id="51e21-103">创建 cloudPcDeviceImage</span><span class="sxs-lookup"><span data-stu-id="51e21-103">Create cloudPcDeviceImage</span></span>

<span data-ttu-id="51e21-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="51e21-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="51e21-105">创建新的 [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="51e21-105">Create a new [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object.</span></span> <span data-ttu-id="51e21-106">上载稍后可在云电脑上预配的自定义 OS 映像。</span><span class="sxs-lookup"><span data-stu-id="51e21-106">Upload a custom OS image that you can later provision on cloud PCs.</span></span>

## <a name="permissions"></a><span data-ttu-id="51e21-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="51e21-107">Permissions</span></span>

<span data-ttu-id="51e21-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="51e21-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51e21-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="51e21-110">Permission type</span></span>|<span data-ttu-id="51e21-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="51e21-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51e21-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="51e21-112">Delegated (work or school account)</span></span>|<span data-ttu-id="51e21-113">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51e21-113">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="51e21-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="51e21-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51e21-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="51e21-115">Not supported.</span></span>|
|<span data-ttu-id="51e21-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="51e21-116">Application</span></span>|<span data-ttu-id="51e21-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="51e21-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="51e21-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="51e21-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/virtualEndpoint/deviceImages
```

## <a name="request-headers"></a><span data-ttu-id="51e21-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="51e21-119">Request headers</span></span>

| <span data-ttu-id="51e21-120">名称</span><span class="sxs-lookup"><span data-stu-id="51e21-120">Name</span></span>          | <span data-ttu-id="51e21-121">说明</span><span class="sxs-lookup"><span data-stu-id="51e21-121">Description</span></span>                |
| :------------ | :------------------------  |
| <span data-ttu-id="51e21-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="51e21-122">Authorization</span></span> | <span data-ttu-id="51e21-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="51e21-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="51e21-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="51e21-125">Content-Type</span></span>  | <span data-ttu-id="51e21-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="51e21-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="51e21-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="51e21-128">Request body</span></span>

<span data-ttu-id="51e21-129">在请求正文中，提供 [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="51e21-129">In the request body, supply a JSON representation of the [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object.</span></span>

<span data-ttu-id="51e21-130">下表显示创建 [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="51e21-130">The following table shows the properties that are required when you create the [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md).</span></span>

|<span data-ttu-id="51e21-131">属性</span><span class="sxs-lookup"><span data-stu-id="51e21-131">Property</span></span>|<span data-ttu-id="51e21-132">类型</span><span class="sxs-lookup"><span data-stu-id="51e21-132">Type</span></span>|<span data-ttu-id="51e21-133">说明</span><span class="sxs-lookup"><span data-stu-id="51e21-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51e21-134">displayName</span><span class="sxs-lookup"><span data-stu-id="51e21-134">displayName</span></span>|<span data-ttu-id="51e21-135">字符串</span><span class="sxs-lookup"><span data-stu-id="51e21-135">String</span></span>|<span data-ttu-id="51e21-136">图像的显示名称。</span><span class="sxs-lookup"><span data-stu-id="51e21-136">The image's display name.</span></span>|
|<span data-ttu-id="51e21-137">sourceImageResourceId</span><span class="sxs-lookup"><span data-stu-id="51e21-137">sourceImageResourceId</span></span>|<span data-ttu-id="51e21-138">字符串</span><span class="sxs-lookup"><span data-stu-id="51e21-138">String</span></span>|<span data-ttu-id="51e21-139">Azure 上的源图像资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="51e21-139">The ID of the source image resource on Azure.</span></span> <span data-ttu-id="51e21-140">必需的格式： "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Compute/images/{imageName}"。</span><span class="sxs-lookup"><span data-stu-id="51e21-140">Required format: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Compute/images/{imageName}".</span></span>|
|<span data-ttu-id="51e21-141">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="51e21-141">operatingSystem</span></span>|<span data-ttu-id="51e21-142">String</span><span class="sxs-lookup"><span data-stu-id="51e21-142">String</span></span>|<span data-ttu-id="51e21-143">图像的操作系统。</span><span class="sxs-lookup"><span data-stu-id="51e21-143">The image's operating system.</span></span> <span data-ttu-id="51e21-144">例如： Windows 10 企业版。</span><span class="sxs-lookup"><span data-stu-id="51e21-144">For example: Windows 10 Enterprise.</span></span>|
|<span data-ttu-id="51e21-145">osBuildNumber</span><span class="sxs-lookup"><span data-stu-id="51e21-145">osBuildNumber</span></span>|<span data-ttu-id="51e21-146">字符串</span><span class="sxs-lookup"><span data-stu-id="51e21-146">String</span></span>|<span data-ttu-id="51e21-147">图像的 OS 内部版本。</span><span class="sxs-lookup"><span data-stu-id="51e21-147">The image's OS build version.</span></span> <span data-ttu-id="51e21-148">例如：1909。</span><span class="sxs-lookup"><span data-stu-id="51e21-148">For example: 1909.</span></span>|
|<span data-ttu-id="51e21-149">version</span><span class="sxs-lookup"><span data-stu-id="51e21-149">version</span></span>|<span data-ttu-id="51e21-150">String</span><span class="sxs-lookup"><span data-stu-id="51e21-150">String</span></span>|<span data-ttu-id="51e21-151">图像版本。</span><span class="sxs-lookup"><span data-stu-id="51e21-151">The image version.</span></span> <span data-ttu-id="51e21-152">例如：0.0.1、1.5.13。</span><span class="sxs-lookup"><span data-stu-id="51e21-152">For example: 0.0.1, 1.5.13.</span></span>|

## <a name="response"></a><span data-ttu-id="51e21-153">响应</span><span class="sxs-lookup"><span data-stu-id="51e21-153">Response</span></span>

<span data-ttu-id="51e21-154">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="51e21-154">If successful, this method returns a `201 Created` response code and a [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="51e21-155">示例</span><span class="sxs-lookup"><span data-stu-id="51e21-155">Examples</span></span>

### <a name="request"></a><span data-ttu-id="51e21-156">请求</span><span class="sxs-lookup"><span data-stu-id="51e21-156">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="51e21-157">响应</span><span class="sxs-lookup"><span data-stu-id="51e21-157">Response</span></span>

<span data-ttu-id="51e21-158">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="51e21-158">**Note:** The response object shown here might be shortened for readability.</span></span>
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
