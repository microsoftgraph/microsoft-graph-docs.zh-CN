---
title: cloudPcDeviceImage 资源类型
description: 表示云电脑上的图像资源。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: d4a88bb4d826ead30d1d739e696dec76df5cbb2f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50957063"
---
# <a name="cloudpcdeviceimage-resource-type"></a><span data-ttu-id="052c2-103">cloudPcDeviceImage 资源类型</span><span class="sxs-lookup"><span data-stu-id="052c2-103">cloudPcDeviceImage resource type</span></span>

<span data-ttu-id="052c2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="052c2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="052c2-105">表示云电脑上的图像资源。</span><span class="sxs-lookup"><span data-stu-id="052c2-105">Represents the image resource on cloud PC.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a><span data-ttu-id="052c2-106">Methods</span><span class="sxs-lookup"><span data-stu-id="052c2-106">Methods</span></span>

|<span data-ttu-id="052c2-107">方法</span><span class="sxs-lookup"><span data-stu-id="052c2-107">Method</span></span>|<span data-ttu-id="052c2-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="052c2-108">Return type</span></span>|<span data-ttu-id="052c2-109">说明</span><span class="sxs-lookup"><span data-stu-id="052c2-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="052c2-110">列出 deviceImages</span><span class="sxs-lookup"><span data-stu-id="052c2-110">List deviceImages</span></span>](../api/virtualendpoint-list-deviceimages.md)|<span data-ttu-id="052c2-111">[cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="052c2-111">[cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) collection</span></span>|<span data-ttu-id="052c2-112">列出 [cloudPcDeviceImage 对象的属性和](../resources/cloudpcdeviceimage.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="052c2-112">List the properties and relationships of [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) objects.</span></span>|
|[<span data-ttu-id="052c2-113">获取 cloudPcDeviceImage</span><span class="sxs-lookup"><span data-stu-id="052c2-113">Get cloudPcDeviceImage</span></span>](../api/cloudpcdeviceimage-get.md)|[<span data-ttu-id="052c2-114">cloudPcDeviceImage</span><span class="sxs-lookup"><span data-stu-id="052c2-114">cloudPcDeviceImage</span></span>](../resources/cloudpcdeviceimage.md)|<span data-ttu-id="052c2-115">读取 [cloudPcDeviceImage 对象的属性和](../resources/cloudpcdeviceimage.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="052c2-115">Read the properties and relationships of a [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object.</span></span>|
|[<span data-ttu-id="052c2-116">创建 cloudPcDeviceImage</span><span class="sxs-lookup"><span data-stu-id="052c2-116">Create cloudPcDeviceImage</span></span>](../api/virtualendpoint-post-deviceimages.md)|[<span data-ttu-id="052c2-117">cloudPcDeviceImage</span><span class="sxs-lookup"><span data-stu-id="052c2-117">cloudPcDeviceImage</span></span>](../resources/cloudpcdeviceimage.md)|<span data-ttu-id="052c2-118">创建新的 [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="052c2-118">Create a new [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object.</span></span>|
|[<span data-ttu-id="052c2-119">删除 cloudPcDeviceImage</span><span class="sxs-lookup"><span data-stu-id="052c2-119">Delete cloudPcDeviceImage</span></span>](../api/cloudpcdeviceimage-delete.md)|<span data-ttu-id="052c2-120">无</span><span class="sxs-lookup"><span data-stu-id="052c2-120">None</span></span>|<span data-ttu-id="052c2-121">删除 [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="052c2-121">Delete a [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object.</span></span>|
|[<span data-ttu-id="052c2-122">getSourceImages</span><span class="sxs-lookup"><span data-stu-id="052c2-122">getSourceImages</span></span>](../api/cloudpcdeviceimage-getsourceimages.md)|<span data-ttu-id="052c2-123">[cloudPcSourceDeviceImage](../resources/cloudpcsourcedeviceimage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="052c2-123">[cloudPcSourceDeviceImage](../resources/cloudpcsourcedeviceimage.md) collection</span></span>|<span data-ttu-id="052c2-124">获取 [cloudPcSourceDeviceImage](../resources/cloudpcsourcedeviceimage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="052c2-124">Get [cloudPcSourceDeviceImage](../resources/cloudpcsourcedeviceimage.md) objects.</span></span>|

## <a name="properties"></a><span data-ttu-id="052c2-125">属性</span><span class="sxs-lookup"><span data-stu-id="052c2-125">Properties</span></span>

|<span data-ttu-id="052c2-126">属性</span><span class="sxs-lookup"><span data-stu-id="052c2-126">Property</span></span>|<span data-ttu-id="052c2-127">类型</span><span class="sxs-lookup"><span data-stu-id="052c2-127">Type</span></span>|<span data-ttu-id="052c2-128">说明</span><span class="sxs-lookup"><span data-stu-id="052c2-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="052c2-129">id</span><span class="sxs-lookup"><span data-stu-id="052c2-129">id</span></span>|<span data-ttu-id="052c2-130">String</span><span class="sxs-lookup"><span data-stu-id="052c2-130">String</span></span>|<span data-ttu-id="052c2-131">云电脑上的图像资源的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="052c2-131">Unique identifier for the image resource on cloud PC.</span></span> <span data-ttu-id="052c2-132">只读。</span><span class="sxs-lookup"><span data-stu-id="052c2-132">Read-only.</span></span>|
|<span data-ttu-id="052c2-133">sourceImageResourceId</span><span class="sxs-lookup"><span data-stu-id="052c2-133">sourceImageResourceId</span></span>|<span data-ttu-id="052c2-134">String</span><span class="sxs-lookup"><span data-stu-id="052c2-134">String</span></span>|<span data-ttu-id="052c2-135">Azure 上的源图像资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="052c2-135">The ID of the source image resource on Azure.</span></span> <span data-ttu-id="052c2-136">所需格式："/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Compute/images/{imageName}"。</span><span class="sxs-lookup"><span data-stu-id="052c2-136">Required format: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Compute/images/{imageName}".</span></span>|
|<span data-ttu-id="052c2-137">displayName</span><span class="sxs-lookup"><span data-stu-id="052c2-137">displayName</span></span>|<span data-ttu-id="052c2-138">String</span><span class="sxs-lookup"><span data-stu-id="052c2-138">String</span></span>|<span data-ttu-id="052c2-139">图像的显示名称。</span><span class="sxs-lookup"><span data-stu-id="052c2-139">The image's display name.</span></span>|
|<span data-ttu-id="052c2-140">version</span><span class="sxs-lookup"><span data-stu-id="052c2-140">version</span></span>|<span data-ttu-id="052c2-141">String</span><span class="sxs-lookup"><span data-stu-id="052c2-141">String</span></span>|<span data-ttu-id="052c2-142">图像版本。</span><span class="sxs-lookup"><span data-stu-id="052c2-142">The image version.</span></span> <span data-ttu-id="052c2-143">例如：0.0.1、1.5.13。</span><span class="sxs-lookup"><span data-stu-id="052c2-143">For example: 0.0.1, 1.5.13.</span></span>|
|<span data-ttu-id="052c2-144">osBuildNumber</span><span class="sxs-lookup"><span data-stu-id="052c2-144">osBuildNumber</span></span>|<span data-ttu-id="052c2-145">String</span><span class="sxs-lookup"><span data-stu-id="052c2-145">String</span></span>|<span data-ttu-id="052c2-146">映像的操作系统生成版本。</span><span class="sxs-lookup"><span data-stu-id="052c2-146">The image's OS build version.</span></span> <span data-ttu-id="052c2-147">例如：1909。</span><span class="sxs-lookup"><span data-stu-id="052c2-147">For example: 1909.</span></span>|
|<span data-ttu-id="052c2-148">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="052c2-148">operatingSystem</span></span>|<span data-ttu-id="052c2-149">String</span><span class="sxs-lookup"><span data-stu-id="052c2-149">String</span></span>|<span data-ttu-id="052c2-150">映像的操作系统。</span><span class="sxs-lookup"><span data-stu-id="052c2-150">The image's operating system.</span></span> <span data-ttu-id="052c2-151">例如：Windows 10 企业版。</span><span class="sxs-lookup"><span data-stu-id="052c2-151">For example: Windows 10 Enterprise.</span></span>|
|<span data-ttu-id="052c2-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="052c2-152">lastModifiedDateTime</span></span>|<span data-ttu-id="052c2-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="052c2-153">DateTimeOffset</span></span>|<span data-ttu-id="052c2-154">上次修改图像的数据和时间。</span><span class="sxs-lookup"><span data-stu-id="052c2-154">The data and time that the image was last modified.</span></span> <span data-ttu-id="052c2-155">时间以 ISO 8601 格式显示，协调世界时 (UTC) 时间。</span><span class="sxs-lookup"><span data-stu-id="052c2-155">The time is shown in ISO 8601 format and  Coordinated Universal Time (UTC) time.</span></span> <span data-ttu-id="052c2-156">例如，2014 年 1 月 1 日午夜 UTC 显示为"2014-01-01T00：00：00Z"。</span><span class="sxs-lookup"><span data-stu-id="052c2-156">For example, midnight UTC on Jan 1, 2014 appears as '2014-01-01T00:00:00Z'.</span></span>|
|<span data-ttu-id="052c2-157">状态</span><span class="sxs-lookup"><span data-stu-id="052c2-157">status</span></span>|<span data-ttu-id="052c2-158">cloudPcDeviceImageStatus</span><span class="sxs-lookup"><span data-stu-id="052c2-158">cloudPcDeviceImageStatus</span></span>|<span data-ttu-id="052c2-159">云电脑上映像的状态。</span><span class="sxs-lookup"><span data-stu-id="052c2-159">The status of the image on cloud PC.</span></span> <span data-ttu-id="052c2-160">可取值为：`pending`、`ready`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="052c2-160">Possible values are: `pending`, `ready`, `failed`.</span></span>|
|<span data-ttu-id="052c2-161">statusDetails</span><span class="sxs-lookup"><span data-stu-id="052c2-161">statusDetails</span></span>|<span data-ttu-id="052c2-162">cloudPcDeviceImageStatusDetails</span><span class="sxs-lookup"><span data-stu-id="052c2-162">cloudPcDeviceImageStatusDetails</span></span>|<span data-ttu-id="052c2-163">图像状态的详细信息，指示上传失败的原因（如果适用）。</span><span class="sxs-lookup"><span data-stu-id="052c2-163">The details of the image's status, which indicates why the upload failed, if applicable.</span></span> <span data-ttu-id="052c2-164">可取值为：`internalServerError`、`sourceImageNotFound`。</span><span class="sxs-lookup"><span data-stu-id="052c2-164">Possible values are: `internalServerError`, `sourceImageNotFound`.</span></span>|

### <a name="cloudpcdeviceimagestatus-values"></a><span data-ttu-id="052c2-165">cloudPcDeviceImageStatus 值</span><span class="sxs-lookup"><span data-stu-id="052c2-165">cloudPcDeviceImageStatus values</span></span>

|<span data-ttu-id="052c2-166">成员</span><span class="sxs-lookup"><span data-stu-id="052c2-166">Member</span></span>|<span data-ttu-id="052c2-167">说明</span><span class="sxs-lookup"><span data-stu-id="052c2-167">Description</span></span>|
|:---|:---|
|<span data-ttu-id="052c2-168">pending</span><span class="sxs-lookup"><span data-stu-id="052c2-168">pending</span></span>|<span data-ttu-id="052c2-169">图像上载正在进行中。</span><span class="sxs-lookup"><span data-stu-id="052c2-169">The image upload is in progress.</span></span>|
|<span data-ttu-id="052c2-170">ready</span><span class="sxs-lookup"><span data-stu-id="052c2-170">ready</span></span>|<span data-ttu-id="052c2-171">该映像已准备好在云电脑使用。</span><span class="sxs-lookup"><span data-stu-id="052c2-171">The image is ready for use on Cloud PCs.</span></span>|
|<span data-ttu-id="052c2-172">failed</span><span class="sxs-lookup"><span data-stu-id="052c2-172">failed</span></span>|<span data-ttu-id="052c2-173">无法上载图像。</span><span class="sxs-lookup"><span data-stu-id="052c2-173">The image couldn’t be uploaded.</span></span> |

### <a name="cloudpcdeviceimagestatusdetails-values"></a><span data-ttu-id="052c2-174">cloudPcDeviceImageStatusDetails 值</span><span class="sxs-lookup"><span data-stu-id="052c2-174">cloudPcDeviceImageStatusDetails values</span></span>

|<span data-ttu-id="052c2-175">成员</span><span class="sxs-lookup"><span data-stu-id="052c2-175">Member</span></span>|<span data-ttu-id="052c2-176">说明</span><span class="sxs-lookup"><span data-stu-id="052c2-176">Description</span></span>|
|:---|:---|
|<span data-ttu-id="052c2-177">internalServerError</span><span class="sxs-lookup"><span data-stu-id="052c2-177">internalServerError</span></span>|<span data-ttu-id="052c2-178">处理映像时出现内部服务器错误。</span><span class="sxs-lookup"><span data-stu-id="052c2-178">There was an internal server error while processing the image.</span></span>|
|<span data-ttu-id="052c2-179">sourceImageNotFound</span><span class="sxs-lookup"><span data-stu-id="052c2-179">sourceImageNotFound</span></span>|<span data-ttu-id="052c2-180">无法访问或找不到源图像。</span><span class="sxs-lookup"><span data-stu-id="052c2-180">Source image is inaccessible or not found.</span></span>|
|<span data-ttu-id="052c2-181">osVersionNotSupported</span><span class="sxs-lookup"><span data-stu-id="052c2-181">osVersionNotSupported</span></span>| <span data-ttu-id="052c2-182">不支持操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="052c2-182">OS version is not supported.</span></span>|
|<span data-ttu-id="052c2-183">sourceImageInvalid</span><span class="sxs-lookup"><span data-stu-id="052c2-183">sourceImageInvalid</span></span>|<span data-ttu-id="052c2-184">源映像用于无效 Windows VM。</span><span class="sxs-lookup"><span data-stu-id="052c2-184">The source image is not valid for provisioning a windows VM with it.</span></span>|

## <a name="relationships"></a><span data-ttu-id="052c2-185">关系</span><span class="sxs-lookup"><span data-stu-id="052c2-185">Relationships</span></span>

<span data-ttu-id="052c2-186">无。</span><span class="sxs-lookup"><span data-stu-id="052c2-186">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="052c2-187">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="052c2-187">JSON representation</span></span>

<span data-ttu-id="052c2-188">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="052c2-188">The following is a JSON representation of the resource.</span></span>
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
