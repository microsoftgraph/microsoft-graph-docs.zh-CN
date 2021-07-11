---
title: cloudPcDeviceImage 资源类型
description: 表示云电脑上的图像资源。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 50154654835d1137db49f9f5690115c05ea7e0c1
ms.sourcegitcommit: 3873c85f53e026073addca92d31d234af244444c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/10/2021
ms.locfileid: "53367001"
---
# <a name="cloudpcdeviceimage-resource-type"></a><span data-ttu-id="b01e2-103">cloudPcDeviceImage 资源类型</span><span class="sxs-lookup"><span data-stu-id="b01e2-103">cloudPcDeviceImage resource type</span></span>

<span data-ttu-id="b01e2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b01e2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b01e2-105">表示云电脑上的图像资源。</span><span class="sxs-lookup"><span data-stu-id="b01e2-105">Represents the image resource on a cloud PC.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a><span data-ttu-id="b01e2-106">方法</span><span class="sxs-lookup"><span data-stu-id="b01e2-106">Methods</span></span>

|<span data-ttu-id="b01e2-107">方法</span><span class="sxs-lookup"><span data-stu-id="b01e2-107">Method</span></span>|<span data-ttu-id="b01e2-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="b01e2-108">Return type</span></span>|<span data-ttu-id="b01e2-109">说明</span><span class="sxs-lookup"><span data-stu-id="b01e2-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b01e2-110">列出 deviceImages</span><span class="sxs-lookup"><span data-stu-id="b01e2-110">List deviceImages</span></span>](../api/virtualendpoint-list-deviceimages.md)|<span data-ttu-id="b01e2-111">[cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b01e2-111">[cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) collection</span></span>|<span data-ttu-id="b01e2-112">列出 [cloudPcDeviceImage 对象的属性和](../resources/cloudpcdeviceimage.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="b01e2-112">List the properties and relationships of [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) objects.</span></span>|
|[<span data-ttu-id="b01e2-113">获取 cloudPcDeviceImage</span><span class="sxs-lookup"><span data-stu-id="b01e2-113">Get cloudPcDeviceImage</span></span>](../api/cloudpcdeviceimage-get.md)|[<span data-ttu-id="b01e2-114">cloudPcDeviceImage</span><span class="sxs-lookup"><span data-stu-id="b01e2-114">cloudPcDeviceImage</span></span>](../resources/cloudpcdeviceimage.md)|<span data-ttu-id="b01e2-115">读取 [cloudPcDeviceImage 对象的属性和](../resources/cloudpcdeviceimage.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="b01e2-115">Read the properties and relationships of a [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object.</span></span>|
|[<span data-ttu-id="b01e2-116">创建 cloudPcDeviceImage</span><span class="sxs-lookup"><span data-stu-id="b01e2-116">Create cloudPcDeviceImage</span></span>](../api/virtualendpoint-post-deviceimages.md)|[<span data-ttu-id="b01e2-117">cloudPcDeviceImage</span><span class="sxs-lookup"><span data-stu-id="b01e2-117">cloudPcDeviceImage</span></span>](../resources/cloudpcdeviceimage.md)|<span data-ttu-id="b01e2-118">创建新的 [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b01e2-118">Create a new [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object.</span></span>|
|[<span data-ttu-id="b01e2-119">删除 cloudPcDeviceImage</span><span class="sxs-lookup"><span data-stu-id="b01e2-119">Delete cloudPcDeviceImage</span></span>](../api/cloudpcdeviceimage-delete.md)|<span data-ttu-id="b01e2-120">无</span><span class="sxs-lookup"><span data-stu-id="b01e2-120">None</span></span>|<span data-ttu-id="b01e2-121">删除 [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b01e2-121">Delete a [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object.</span></span>|
|[<span data-ttu-id="b01e2-122">getSourceImages</span><span class="sxs-lookup"><span data-stu-id="b01e2-122">getSourceImages</span></span>](../api/cloudpcdeviceimage-getsourceimages.md)|<span data-ttu-id="b01e2-123">[cloudPcSourceDeviceImage](../resources/cloudpcsourcedeviceimage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b01e2-123">[cloudPcSourceDeviceImage](../resources/cloudpcsourcedeviceimage.md) collection</span></span>|<span data-ttu-id="b01e2-124">获取 [cloudPcSourceDeviceImage](../resources/cloudpcsourcedeviceimage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b01e2-124">Get [cloudPcSourceDeviceImage](../resources/cloudpcsourcedeviceimage.md) objects.</span></span>|
|[<span data-ttu-id="b01e2-125">重新加载 cloudPcDeviceImage</span><span class="sxs-lookup"><span data-stu-id="b01e2-125">Reupload cloudPcDeviceImage</span></span>](../api/cloudpcdeviceimage-reupload.md)|<span data-ttu-id="b01e2-126">无</span><span class="sxs-lookup"><span data-stu-id="b01e2-126">None</span></span>|<span data-ttu-id="b01e2-127">重新加载 [无法上载的 cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b01e2-127">Reupload a [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object that failed to upload.</span></span>|

## <a name="properties"></a><span data-ttu-id="b01e2-128">属性</span><span class="sxs-lookup"><span data-stu-id="b01e2-128">Properties</span></span>

|<span data-ttu-id="b01e2-129">属性</span><span class="sxs-lookup"><span data-stu-id="b01e2-129">Property</span></span>|<span data-ttu-id="b01e2-130">类型</span><span class="sxs-lookup"><span data-stu-id="b01e2-130">Type</span></span>|<span data-ttu-id="b01e2-131">说明</span><span class="sxs-lookup"><span data-stu-id="b01e2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b01e2-132">id</span><span class="sxs-lookup"><span data-stu-id="b01e2-132">id</span></span>|<span data-ttu-id="b01e2-133">String</span><span class="sxs-lookup"><span data-stu-id="b01e2-133">String</span></span>|<span data-ttu-id="b01e2-134">云电脑上的图像资源的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="b01e2-134">Unique identifier for the image resource on the cloud PC.</span></span> <span data-ttu-id="b01e2-135">只读。</span><span class="sxs-lookup"><span data-stu-id="b01e2-135">Read-only.</span></span>|
|<span data-ttu-id="b01e2-136">sourceImageResourceId</span><span class="sxs-lookup"><span data-stu-id="b01e2-136">sourceImageResourceId</span></span>|<span data-ttu-id="b01e2-137">String</span><span class="sxs-lookup"><span data-stu-id="b01e2-137">String</span></span>|<span data-ttu-id="b01e2-138">Azure 上的源图像资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="b01e2-138">The ID of the source image resource on Azure.</span></span> <span data-ttu-id="b01e2-139">所需格式："/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Compute/images/{imageName}"。</span><span class="sxs-lookup"><span data-stu-id="b01e2-139">Required format: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Compute/images/{imageName}".</span></span>|
|<span data-ttu-id="b01e2-140">displayName</span><span class="sxs-lookup"><span data-stu-id="b01e2-140">displayName</span></span>|<span data-ttu-id="b01e2-141">String</span><span class="sxs-lookup"><span data-stu-id="b01e2-141">String</span></span>|<span data-ttu-id="b01e2-142">图像的显示名称。</span><span class="sxs-lookup"><span data-stu-id="b01e2-142">The image's display name.</span></span>|
|<span data-ttu-id="b01e2-143">version</span><span class="sxs-lookup"><span data-stu-id="b01e2-143">version</span></span>|<span data-ttu-id="b01e2-144">String</span><span class="sxs-lookup"><span data-stu-id="b01e2-144">String</span></span>|<span data-ttu-id="b01e2-145">图像版本。</span><span class="sxs-lookup"><span data-stu-id="b01e2-145">The image version.</span></span> <span data-ttu-id="b01e2-146">例如：0.0.1、1.5.13。</span><span class="sxs-lookup"><span data-stu-id="b01e2-146">For example: 0.0.1, 1.5.13.</span></span>|
|<span data-ttu-id="b01e2-147">osBuildNumber</span><span class="sxs-lookup"><span data-stu-id="b01e2-147">osBuildNumber</span></span>|<span data-ttu-id="b01e2-148">String</span><span class="sxs-lookup"><span data-stu-id="b01e2-148">String</span></span>|<span data-ttu-id="b01e2-149">映像的操作系统生成版本。</span><span class="sxs-lookup"><span data-stu-id="b01e2-149">The image's OS build version.</span></span> <span data-ttu-id="b01e2-150">例如：1909。</span><span class="sxs-lookup"><span data-stu-id="b01e2-150">For example: 1909.</span></span>|
|<span data-ttu-id="b01e2-151">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="b01e2-151">operatingSystem</span></span>|<span data-ttu-id="b01e2-152">String</span><span class="sxs-lookup"><span data-stu-id="b01e2-152">String</span></span>|<span data-ttu-id="b01e2-153">映像的操作系统。</span><span class="sxs-lookup"><span data-stu-id="b01e2-153">The image's operating system.</span></span> <span data-ttu-id="b01e2-154">例如：Windows 10 企业版。</span><span class="sxs-lookup"><span data-stu-id="b01e2-154">For example: Windows 10 Enterprise.</span></span>|
|<span data-ttu-id="b01e2-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b01e2-155">lastModifiedDateTime</span></span>|<span data-ttu-id="b01e2-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b01e2-156">DateTimeOffset</span></span>|<span data-ttu-id="b01e2-157">上次修改图像的数据和时间。</span><span class="sxs-lookup"><span data-stu-id="b01e2-157">The data and time that the image was last modified.</span></span> <span data-ttu-id="b01e2-158">时间以 ISO 8601 格式显示，协调世界时 (UTC) 时间。</span><span class="sxs-lookup"><span data-stu-id="b01e2-158">The time is shown in ISO 8601 format and  Coordinated Universal Time (UTC) time.</span></span> <span data-ttu-id="b01e2-159">例如，2014 年 1 月 1 日午夜 UTC 显示为"2014-01-01T00：00：00Z"。</span><span class="sxs-lookup"><span data-stu-id="b01e2-159">For example, midnight UTC on Jan 1, 2014 appears as '2014-01-01T00:00:00Z'.</span></span>|
|<span data-ttu-id="b01e2-160">状态</span><span class="sxs-lookup"><span data-stu-id="b01e2-160">status</span></span>|<span data-ttu-id="b01e2-161">cloudPcDeviceImageStatus</span><span class="sxs-lookup"><span data-stu-id="b01e2-161">cloudPcDeviceImageStatus</span></span>|<span data-ttu-id="b01e2-162">云电脑上映像的状态。</span><span class="sxs-lookup"><span data-stu-id="b01e2-162">The status of the image on cloud PC.</span></span> <span data-ttu-id="b01e2-163">可取值为：`pending`、`ready`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="b01e2-163">Possible values are: `pending`, `ready`, `failed`.</span></span>|
|<span data-ttu-id="b01e2-164">statusDetails</span><span class="sxs-lookup"><span data-stu-id="b01e2-164">statusDetails</span></span>|<span data-ttu-id="b01e2-165">cloudPcDeviceImageStatusDetails</span><span class="sxs-lookup"><span data-stu-id="b01e2-165">cloudPcDeviceImageStatusDetails</span></span>|<span data-ttu-id="b01e2-166">图像状态的详细信息，指示上传失败的原因（如果适用）。</span><span class="sxs-lookup"><span data-stu-id="b01e2-166">The details of the image's status, which indicates why the upload failed, if applicable.</span></span> <span data-ttu-id="b01e2-167">可能的值为： `internalServerError`、 `sourceImageNotFound`、 `osVersionNotSupported`和 `sourceImageInvalid`。</span><span class="sxs-lookup"><span data-stu-id="b01e2-167">Possible values are: `internalServerError`, `sourceImageNotFound`, `osVersionNotSupported`, and `sourceImageInvalid`.</span></span>|

### <a name="cloudpcdeviceimagestatus-values"></a><span data-ttu-id="b01e2-168">cloudPcDeviceImageStatus 值</span><span class="sxs-lookup"><span data-stu-id="b01e2-168">cloudPcDeviceImageStatus values</span></span>

|<span data-ttu-id="b01e2-169">成员</span><span class="sxs-lookup"><span data-stu-id="b01e2-169">Member</span></span>|<span data-ttu-id="b01e2-170">说明</span><span class="sxs-lookup"><span data-stu-id="b01e2-170">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b01e2-171">pending</span><span class="sxs-lookup"><span data-stu-id="b01e2-171">pending</span></span>|<span data-ttu-id="b01e2-172">图像上载正在进行中。</span><span class="sxs-lookup"><span data-stu-id="b01e2-172">The image upload is in progress.</span></span>|
|<span data-ttu-id="b01e2-173">ready</span><span class="sxs-lookup"><span data-stu-id="b01e2-173">ready</span></span>|<span data-ttu-id="b01e2-174">该映像已准备好在云 PC 上使用。</span><span class="sxs-lookup"><span data-stu-id="b01e2-174">The image is ready for use on cloud PCs.</span></span>|
|<span data-ttu-id="b01e2-175">failed</span><span class="sxs-lookup"><span data-stu-id="b01e2-175">failed</span></span>|<span data-ttu-id="b01e2-176">无法上载图像。</span><span class="sxs-lookup"><span data-stu-id="b01e2-176">The image couldn’t be uploaded.</span></span> |

### <a name="cloudpcdeviceimagestatusdetails-values"></a><span data-ttu-id="b01e2-177">cloudPcDeviceImageStatusDetails 值</span><span class="sxs-lookup"><span data-stu-id="b01e2-177">cloudPcDeviceImageStatusDetails values</span></span>

|<span data-ttu-id="b01e2-178">成员</span><span class="sxs-lookup"><span data-stu-id="b01e2-178">Member</span></span>|<span data-ttu-id="b01e2-179">说明</span><span class="sxs-lookup"><span data-stu-id="b01e2-179">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b01e2-180">internalServerError</span><span class="sxs-lookup"><span data-stu-id="b01e2-180">internalServerError</span></span>|<span data-ttu-id="b01e2-181">处理映像时出现内部服务器错误。</span><span class="sxs-lookup"><span data-stu-id="b01e2-181">There was an internal server error while processing the image.</span></span>|
|<span data-ttu-id="b01e2-182">sourceImageNotFound</span><span class="sxs-lookup"><span data-stu-id="b01e2-182">sourceImageNotFound</span></span>|<span data-ttu-id="b01e2-183">无法访问或找不到源图像。</span><span class="sxs-lookup"><span data-stu-id="b01e2-183">Source image is inaccessible or not found.</span></span>|
|<span data-ttu-id="b01e2-184">osVersionNotSupported</span><span class="sxs-lookup"><span data-stu-id="b01e2-184">osVersionNotSupported</span></span>| <span data-ttu-id="b01e2-185">不支持操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="b01e2-185">OS version is not supported.</span></span>|
|<span data-ttu-id="b01e2-186">sourceImageInvalid</span><span class="sxs-lookup"><span data-stu-id="b01e2-186">sourceImageInvalid</span></span>|<span data-ttu-id="b01e2-187">源映像用于无效一个Windows VM。</span><span class="sxs-lookup"><span data-stu-id="b01e2-187">The source image is not valid for provisioning a Windows VM with it.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b01e2-188">关系</span><span class="sxs-lookup"><span data-stu-id="b01e2-188">Relationships</span></span>

<span data-ttu-id="b01e2-189">无。</span><span class="sxs-lookup"><span data-stu-id="b01e2-189">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b01e2-190">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b01e2-190">JSON representation</span></span>

<span data-ttu-id="b01e2-191">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b01e2-191">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cloudPcDeviceImage",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcDeviceImage",
  "id": "String (identifier)",
  "displayName": "String",
  "operatingSystem": "String",
  "osBuildNumber": "String",
  "version": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "status": "String",
  "statusDetails": "String",
  "sourceImageResourceId": "String"
}
```
