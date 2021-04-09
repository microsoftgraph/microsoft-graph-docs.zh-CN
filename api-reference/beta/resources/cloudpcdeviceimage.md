---
title: cloudPcDeviceImage 资源类型
description: 表示云电脑上的图像资源。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 2c38895059461f814a3ad0f8e663082972cc8663
ms.sourcegitcommit: e96b98849cfc3aa915df63696a0b9f30c0a52cfd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/09/2021
ms.locfileid: "51654126"
---
# <a name="cloudpcdeviceimage-resource-type"></a><span data-ttu-id="37ce5-103">cloudPcDeviceImage 资源类型</span><span class="sxs-lookup"><span data-stu-id="37ce5-103">cloudPcDeviceImage resource type</span></span>

<span data-ttu-id="37ce5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37ce5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37ce5-105">表示云电脑上的图像资源。</span><span class="sxs-lookup"><span data-stu-id="37ce5-105">Represents the image resource on cloud PC.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a><span data-ttu-id="37ce5-106">方法</span><span class="sxs-lookup"><span data-stu-id="37ce5-106">Methods</span></span>

|<span data-ttu-id="37ce5-107">方法</span><span class="sxs-lookup"><span data-stu-id="37ce5-107">Method</span></span>|<span data-ttu-id="37ce5-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="37ce5-108">Return type</span></span>|<span data-ttu-id="37ce5-109">说明</span><span class="sxs-lookup"><span data-stu-id="37ce5-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="37ce5-110">列出 deviceImages</span><span class="sxs-lookup"><span data-stu-id="37ce5-110">List deviceImages</span></span>](../api/virtualendpoint-list-deviceimages.md)|<span data-ttu-id="37ce5-111">[cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="37ce5-111">[cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) collection</span></span>|<span data-ttu-id="37ce5-112">列出 [cloudPcDeviceImage 对象的属性和](../resources/cloudpcdeviceimage.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="37ce5-112">List the properties and relationships of [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) objects.</span></span>|
|[<span data-ttu-id="37ce5-113">获取 cloudPcDeviceImage</span><span class="sxs-lookup"><span data-stu-id="37ce5-113">Get cloudPcDeviceImage</span></span>](../api/cloudpcdeviceimage-get.md)|[<span data-ttu-id="37ce5-114">cloudPcDeviceImage</span><span class="sxs-lookup"><span data-stu-id="37ce5-114">cloudPcDeviceImage</span></span>](../resources/cloudpcdeviceimage.md)|<span data-ttu-id="37ce5-115">读取 [cloudPcDeviceImage 对象的属性和](../resources/cloudpcdeviceimage.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="37ce5-115">Read the properties and relationships of a [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object.</span></span>|
|[<span data-ttu-id="37ce5-116">创建 cloudPcDeviceImage</span><span class="sxs-lookup"><span data-stu-id="37ce5-116">Create cloudPcDeviceImage</span></span>](../api/virtualendpoint-post-deviceimages.md)|[<span data-ttu-id="37ce5-117">cloudPcDeviceImage</span><span class="sxs-lookup"><span data-stu-id="37ce5-117">cloudPcDeviceImage</span></span>](../resources/cloudpcdeviceimage.md)|<span data-ttu-id="37ce5-118">创建新的 [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="37ce5-118">Create a new [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object.</span></span>|
|[<span data-ttu-id="37ce5-119">删除 cloudPcDeviceImage</span><span class="sxs-lookup"><span data-stu-id="37ce5-119">Delete cloudPcDeviceImage</span></span>](../api/cloudpcdeviceimage-delete.md)|<span data-ttu-id="37ce5-120">无</span><span class="sxs-lookup"><span data-stu-id="37ce5-120">None</span></span>|<span data-ttu-id="37ce5-121">删除 [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="37ce5-121">Delete a [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object.</span></span>|
|[<span data-ttu-id="37ce5-122">getSourceImages</span><span class="sxs-lookup"><span data-stu-id="37ce5-122">getSourceImages</span></span>](../api/cloudpcdeviceimage-getsourceimages.md)|<span data-ttu-id="37ce5-123">[cloudPcSourceDeviceImage](../resources/cloudpcsourcedeviceimage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="37ce5-123">[cloudPcSourceDeviceImage](../resources/cloudpcsourcedeviceimage.md) collection</span></span>|<span data-ttu-id="37ce5-124">获取 [cloudPcSourceDeviceImage](../resources/cloudpcsourcedeviceimage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="37ce5-124">Get [cloudPcSourceDeviceImage](../resources/cloudpcsourcedeviceimage.md) objects.</span></span>|

## <a name="properties"></a><span data-ttu-id="37ce5-125">属性</span><span class="sxs-lookup"><span data-stu-id="37ce5-125">Properties</span></span>

|<span data-ttu-id="37ce5-126">属性</span><span class="sxs-lookup"><span data-stu-id="37ce5-126">Property</span></span>|<span data-ttu-id="37ce5-127">类型</span><span class="sxs-lookup"><span data-stu-id="37ce5-127">Type</span></span>|<span data-ttu-id="37ce5-128">说明</span><span class="sxs-lookup"><span data-stu-id="37ce5-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37ce5-129">id</span><span class="sxs-lookup"><span data-stu-id="37ce5-129">id</span></span>|<span data-ttu-id="37ce5-130">String</span><span class="sxs-lookup"><span data-stu-id="37ce5-130">String</span></span>|<span data-ttu-id="37ce5-131">云电脑上的图像资源的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="37ce5-131">Unique identifier for the image resource on cloud PC.</span></span> <span data-ttu-id="37ce5-132">只读。</span><span class="sxs-lookup"><span data-stu-id="37ce5-132">Read-only.</span></span>|
|<span data-ttu-id="37ce5-133">sourceImageResourceId</span><span class="sxs-lookup"><span data-stu-id="37ce5-133">sourceImageResourceId</span></span>|<span data-ttu-id="37ce5-134">String</span><span class="sxs-lookup"><span data-stu-id="37ce5-134">String</span></span>|<span data-ttu-id="37ce5-135">Azure 上的源图像资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="37ce5-135">The ID of the source image resource on Azure.</span></span> <span data-ttu-id="37ce5-136">所需格式："/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Compute/images/{imageName}"。</span><span class="sxs-lookup"><span data-stu-id="37ce5-136">Required format: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Compute/images/{imageName}".</span></span>|
|<span data-ttu-id="37ce5-137">displayName</span><span class="sxs-lookup"><span data-stu-id="37ce5-137">displayName</span></span>|<span data-ttu-id="37ce5-138">String</span><span class="sxs-lookup"><span data-stu-id="37ce5-138">String</span></span>|<span data-ttu-id="37ce5-139">图像的显示名称。</span><span class="sxs-lookup"><span data-stu-id="37ce5-139">The image's display name.</span></span>|
|<span data-ttu-id="37ce5-140">version</span><span class="sxs-lookup"><span data-stu-id="37ce5-140">version</span></span>|<span data-ttu-id="37ce5-141">String</span><span class="sxs-lookup"><span data-stu-id="37ce5-141">String</span></span>|<span data-ttu-id="37ce5-142">图像版本。</span><span class="sxs-lookup"><span data-stu-id="37ce5-142">The image version.</span></span> <span data-ttu-id="37ce5-143">例如：0.0.1、1.5.13。</span><span class="sxs-lookup"><span data-stu-id="37ce5-143">For example: 0.0.1, 1.5.13.</span></span>|
|<span data-ttu-id="37ce5-144">osBuildNumber</span><span class="sxs-lookup"><span data-stu-id="37ce5-144">osBuildNumber</span></span>|<span data-ttu-id="37ce5-145">String</span><span class="sxs-lookup"><span data-stu-id="37ce5-145">String</span></span>|<span data-ttu-id="37ce5-146">映像的操作系统生成版本。</span><span class="sxs-lookup"><span data-stu-id="37ce5-146">The image's OS build version.</span></span> <span data-ttu-id="37ce5-147">例如：1909。</span><span class="sxs-lookup"><span data-stu-id="37ce5-147">For example: 1909.</span></span>|
|<span data-ttu-id="37ce5-148">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="37ce5-148">operatingSystem</span></span>|<span data-ttu-id="37ce5-149">String</span><span class="sxs-lookup"><span data-stu-id="37ce5-149">String</span></span>|<span data-ttu-id="37ce5-150">映像的操作系统。</span><span class="sxs-lookup"><span data-stu-id="37ce5-150">The image's operating system.</span></span> <span data-ttu-id="37ce5-151">例如：Windows 10 企业版。</span><span class="sxs-lookup"><span data-stu-id="37ce5-151">For example: Windows 10 Enterprise.</span></span>|
|<span data-ttu-id="37ce5-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="37ce5-152">lastModifiedDateTime</span></span>|<span data-ttu-id="37ce5-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="37ce5-153">DateTimeOffset</span></span>|<span data-ttu-id="37ce5-154">上次修改图像的数据和时间。</span><span class="sxs-lookup"><span data-stu-id="37ce5-154">The data and time that the image was last modified.</span></span> <span data-ttu-id="37ce5-155">时间以 ISO 8601 格式显示，协调世界时 (UTC) 时间。</span><span class="sxs-lookup"><span data-stu-id="37ce5-155">The time is shown in ISO 8601 format and  Coordinated Universal Time (UTC) time.</span></span> <span data-ttu-id="37ce5-156">例如，2014 年 1 月 1 日午夜 UTC 显示为"2014-01-01T00：00：00Z"。</span><span class="sxs-lookup"><span data-stu-id="37ce5-156">For example, midnight UTC on Jan 1, 2014 appears as '2014-01-01T00:00:00Z'.</span></span>|
|<span data-ttu-id="37ce5-157">状态</span><span class="sxs-lookup"><span data-stu-id="37ce5-157">status</span></span>|<span data-ttu-id="37ce5-158">cloudPcDeviceImageStatus</span><span class="sxs-lookup"><span data-stu-id="37ce5-158">cloudPcDeviceImageStatus</span></span>|<span data-ttu-id="37ce5-159">云电脑上映像的状态。</span><span class="sxs-lookup"><span data-stu-id="37ce5-159">The status of the image on cloud PC.</span></span> <span data-ttu-id="37ce5-160">可取值为：`pending`、`ready`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="37ce5-160">Possible values are: `pending`, `ready`, `failed`.</span></span>|
|<span data-ttu-id="37ce5-161">statusDetails</span><span class="sxs-lookup"><span data-stu-id="37ce5-161">statusDetails</span></span>|<span data-ttu-id="37ce5-162">cloudPcDeviceImageStatusDetails</span><span class="sxs-lookup"><span data-stu-id="37ce5-162">cloudPcDeviceImageStatusDetails</span></span>|<span data-ttu-id="37ce5-163">图像状态的详细信息，指示上传失败的原因（如果适用）。</span><span class="sxs-lookup"><span data-stu-id="37ce5-163">The details of the image's status, which indicates why the upload failed, if applicable.</span></span> <span data-ttu-id="37ce5-164">可能的值是 `internalServerError` `sourceImageNotFound` ：、、 `osVersionNotSupported` 和 `sourceImageInvalid` 。</span><span class="sxs-lookup"><span data-stu-id="37ce5-164">Possible values are: `internalServerError`, `sourceImageNotFound`, `osVersionNotSupported`, and `sourceImageInvalid`.</span></span>|

### <a name="cloudpcdeviceimagestatus-values"></a><span data-ttu-id="37ce5-165">cloudPcDeviceImageStatus 值</span><span class="sxs-lookup"><span data-stu-id="37ce5-165">cloudPcDeviceImageStatus values</span></span>

|<span data-ttu-id="37ce5-166">成员</span><span class="sxs-lookup"><span data-stu-id="37ce5-166">Member</span></span>|<span data-ttu-id="37ce5-167">说明</span><span class="sxs-lookup"><span data-stu-id="37ce5-167">Description</span></span>|
|:---|:---|
|<span data-ttu-id="37ce5-168">pending</span><span class="sxs-lookup"><span data-stu-id="37ce5-168">pending</span></span>|<span data-ttu-id="37ce5-169">图像上载正在进行中。</span><span class="sxs-lookup"><span data-stu-id="37ce5-169">The image upload is in progress.</span></span>|
|<span data-ttu-id="37ce5-170">ready</span><span class="sxs-lookup"><span data-stu-id="37ce5-170">ready</span></span>|<span data-ttu-id="37ce5-171">该映像已准备好在云电脑使用。</span><span class="sxs-lookup"><span data-stu-id="37ce5-171">The image is ready for use on Cloud PCs.</span></span>|
|<span data-ttu-id="37ce5-172">failed</span><span class="sxs-lookup"><span data-stu-id="37ce5-172">failed</span></span>|<span data-ttu-id="37ce5-173">无法上载图像。</span><span class="sxs-lookup"><span data-stu-id="37ce5-173">The image couldn’t be uploaded.</span></span> |

### <a name="cloudpcdeviceimagestatusdetails-values"></a><span data-ttu-id="37ce5-174">cloudPcDeviceImageStatusDetails 值</span><span class="sxs-lookup"><span data-stu-id="37ce5-174">cloudPcDeviceImageStatusDetails values</span></span>

|<span data-ttu-id="37ce5-175">成员</span><span class="sxs-lookup"><span data-stu-id="37ce5-175">Member</span></span>|<span data-ttu-id="37ce5-176">说明</span><span class="sxs-lookup"><span data-stu-id="37ce5-176">Description</span></span>|
|:---|:---|
|<span data-ttu-id="37ce5-177">internalServerError</span><span class="sxs-lookup"><span data-stu-id="37ce5-177">internalServerError</span></span>|<span data-ttu-id="37ce5-178">处理映像时出现内部服务器错误。</span><span class="sxs-lookup"><span data-stu-id="37ce5-178">There was an internal server error while processing the image.</span></span>|
|<span data-ttu-id="37ce5-179">sourceImageNotFound</span><span class="sxs-lookup"><span data-stu-id="37ce5-179">sourceImageNotFound</span></span>|<span data-ttu-id="37ce5-180">无法访问或找不到源图像。</span><span class="sxs-lookup"><span data-stu-id="37ce5-180">Source image is inaccessible or not found.</span></span>|
|<span data-ttu-id="37ce5-181">osVersionNotSupported</span><span class="sxs-lookup"><span data-stu-id="37ce5-181">osVersionNotSupported</span></span>| <span data-ttu-id="37ce5-182">不支持操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="37ce5-182">OS version is not supported.</span></span>|
|<span data-ttu-id="37ce5-183">sourceImageInvalid</span><span class="sxs-lookup"><span data-stu-id="37ce5-183">sourceImageInvalid</span></span>|<span data-ttu-id="37ce5-184">源映像用于无效 Windows VM。</span><span class="sxs-lookup"><span data-stu-id="37ce5-184">The source image is not valid for provisioning a Windows VM with it.</span></span>|

## <a name="relationships"></a><span data-ttu-id="37ce5-185">关系</span><span class="sxs-lookup"><span data-stu-id="37ce5-185">Relationships</span></span>

<span data-ttu-id="37ce5-186">无。</span><span class="sxs-lookup"><span data-stu-id="37ce5-186">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="37ce5-187">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="37ce5-187">JSON representation</span></span>

<span data-ttu-id="37ce5-188">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="37ce5-188">The following is a JSON representation of the resource.</span></span>
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
