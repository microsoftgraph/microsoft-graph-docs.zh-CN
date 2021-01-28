---
title: cloudPcDeviceImage 资源类型
description: 表示云电脑上的图像资源。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 14e3f28d9e7d91df953405bc36afff4d3405c886
ms.sourcegitcommit: 9a03b719d1316729dd022bf4d268894e91515475
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/28/2021
ms.locfileid: "50033891"
---
# <a name="cloudpcdeviceimage-resource-type"></a><span data-ttu-id="abcc7-103">cloudPcDeviceImage 资源类型</span><span class="sxs-lookup"><span data-stu-id="abcc7-103">cloudPcDeviceImage resource type</span></span>

<span data-ttu-id="abcc7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="abcc7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="abcc7-105">表示云电脑上的图像资源。</span><span class="sxs-lookup"><span data-stu-id="abcc7-105">Represents the image resource on cloud PC.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a><span data-ttu-id="abcc7-106">方法</span><span class="sxs-lookup"><span data-stu-id="abcc7-106">Methods</span></span>

|<span data-ttu-id="abcc7-107">方法</span><span class="sxs-lookup"><span data-stu-id="abcc7-107">Method</span></span>|<span data-ttu-id="abcc7-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="abcc7-108">Return type</span></span>|<span data-ttu-id="abcc7-109">说明</span><span class="sxs-lookup"><span data-stu-id="abcc7-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="abcc7-110">列出 deviceImages</span><span class="sxs-lookup"><span data-stu-id="abcc7-110">List deviceImages</span></span>](../api/virtualendpoint-list-deviceimages.md)|<span data-ttu-id="abcc7-111">[cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="abcc7-111">[cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) collection</span></span>|<span data-ttu-id="abcc7-112">列出 [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="abcc7-112">List the properties and relationships of [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) objects.</span></span>|
|[<span data-ttu-id="abcc7-113">获取 cloudPcDeviceImage</span><span class="sxs-lookup"><span data-stu-id="abcc7-113">Get cloudPcDeviceImage</span></span>](../api/cloudpcdeviceimage-get.md)|[<span data-ttu-id="abcc7-114">cloudPcDeviceImage</span><span class="sxs-lookup"><span data-stu-id="abcc7-114">cloudPcDeviceImage</span></span>](../resources/cloudpcdeviceimage.md)|<span data-ttu-id="abcc7-115">读取 [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="abcc7-115">Read the properties and relationships of a [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object.</span></span>|
|[<span data-ttu-id="abcc7-116">创建 cloudPcDeviceImage</span><span class="sxs-lookup"><span data-stu-id="abcc7-116">Create cloudPcDeviceImage</span></span>](../api/virtualendpoint-post-deviceimages.md)|[<span data-ttu-id="abcc7-117">cloudPcDeviceImage</span><span class="sxs-lookup"><span data-stu-id="abcc7-117">cloudPcDeviceImage</span></span>](../resources/cloudpcdeviceimage.md)|<span data-ttu-id="abcc7-118">创建新的 [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="abcc7-118">Create a new [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object.</span></span>|
|[<span data-ttu-id="abcc7-119">删除 cloudPcDeviceImage</span><span class="sxs-lookup"><span data-stu-id="abcc7-119">Delete cloudPcDeviceImage</span></span>](../api/cloudpcdeviceimage-delete.md)|<span data-ttu-id="abcc7-120">无</span><span class="sxs-lookup"><span data-stu-id="abcc7-120">None</span></span>|<span data-ttu-id="abcc7-121">删除 [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="abcc7-121">Delete a [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object.</span></span>|
|[<span data-ttu-id="abcc7-122">getSourceImages</span><span class="sxs-lookup"><span data-stu-id="abcc7-122">getSourceImages</span></span>](../api/cloudpcdeviceimage-getsourceimages.md)|<span data-ttu-id="abcc7-123">[cloudPcSourceDeviceImage](../resources/cloudpcsourcedeviceimage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="abcc7-123">[cloudPcSourceDeviceImage](../resources/cloudpcsourcedeviceimage.md) collection</span></span>|<span data-ttu-id="abcc7-124">获取 [cloudPcSourceDeviceImage](../resources/cloudpcsourcedeviceimage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="abcc7-124">Get [cloudPcSourceDeviceImage](../resources/cloudpcsourcedeviceimage.md) objects.</span></span>|

## <a name="properties"></a><span data-ttu-id="abcc7-125">属性</span><span class="sxs-lookup"><span data-stu-id="abcc7-125">Properties</span></span>

|<span data-ttu-id="abcc7-126">属性</span><span class="sxs-lookup"><span data-stu-id="abcc7-126">Property</span></span>|<span data-ttu-id="abcc7-127">类型</span><span class="sxs-lookup"><span data-stu-id="abcc7-127">Type</span></span>|<span data-ttu-id="abcc7-128">说明</span><span class="sxs-lookup"><span data-stu-id="abcc7-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="abcc7-129">id</span><span class="sxs-lookup"><span data-stu-id="abcc7-129">id</span></span>|<span data-ttu-id="abcc7-130">String</span><span class="sxs-lookup"><span data-stu-id="abcc7-130">String</span></span>|<span data-ttu-id="abcc7-131">云电脑上的图像资源的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="abcc7-131">Unique identifier for the image resource on cloud PC.</span></span> <span data-ttu-id="abcc7-132">只读。</span><span class="sxs-lookup"><span data-stu-id="abcc7-132">Read-only.</span></span>|
|<span data-ttu-id="abcc7-133">sourceImageResourceId</span><span class="sxs-lookup"><span data-stu-id="abcc7-133">sourceImageResourceId</span></span>|<span data-ttu-id="abcc7-134">String</span><span class="sxs-lookup"><span data-stu-id="abcc7-134">String</span></span>|<span data-ttu-id="abcc7-135">Azure 上的源映像资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="abcc7-135">The ID of the source image resource on Azure.</span></span> <span data-ttu-id="abcc7-136">必需格式："/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Compute/images/{imageName}"。</span><span class="sxs-lookup"><span data-stu-id="abcc7-136">Required format: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Compute/images/{imageName}".</span></span>|
|<span data-ttu-id="abcc7-137">displayName</span><span class="sxs-lookup"><span data-stu-id="abcc7-137">displayName</span></span>|<span data-ttu-id="abcc7-138">String</span><span class="sxs-lookup"><span data-stu-id="abcc7-138">String</span></span>|<span data-ttu-id="abcc7-139">图像显示名称。</span><span class="sxs-lookup"><span data-stu-id="abcc7-139">The image's display name.</span></span>|
|<span data-ttu-id="abcc7-140">version</span><span class="sxs-lookup"><span data-stu-id="abcc7-140">version</span></span>|<span data-ttu-id="abcc7-141">String</span><span class="sxs-lookup"><span data-stu-id="abcc7-141">String</span></span>|<span data-ttu-id="abcc7-142">图像版本。</span><span class="sxs-lookup"><span data-stu-id="abcc7-142">The image version.</span></span> <span data-ttu-id="abcc7-143">例如：0.0.1、1.5.13。</span><span class="sxs-lookup"><span data-stu-id="abcc7-143">For example: 0.0.1, 1.5.13.</span></span>|
|<span data-ttu-id="abcc7-144">osBuildNumber</span><span class="sxs-lookup"><span data-stu-id="abcc7-144">osBuildNumber</span></span>|<span data-ttu-id="abcc7-145">String</span><span class="sxs-lookup"><span data-stu-id="abcc7-145">String</span></span>|<span data-ttu-id="abcc7-146">映像的操作系统生成版本。</span><span class="sxs-lookup"><span data-stu-id="abcc7-146">The image's OS build version.</span></span> <span data-ttu-id="abcc7-147">例如：1909。</span><span class="sxs-lookup"><span data-stu-id="abcc7-147">For example: 1909.</span></span>|
|<span data-ttu-id="abcc7-148">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="abcc7-148">operatingSystem</span></span>|<span data-ttu-id="abcc7-149">String</span><span class="sxs-lookup"><span data-stu-id="abcc7-149">String</span></span>|<span data-ttu-id="abcc7-150">映像的操作系统。</span><span class="sxs-lookup"><span data-stu-id="abcc7-150">The image's operating system.</span></span> <span data-ttu-id="abcc7-151">例如：Windows 10 企业版。</span><span class="sxs-lookup"><span data-stu-id="abcc7-151">For example: Windows 10 Enterprise.</span></span>|
|<span data-ttu-id="abcc7-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="abcc7-152">lastModifiedDateTime</span></span>|<span data-ttu-id="abcc7-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="abcc7-153">DateTimeOffset</span></span>|<span data-ttu-id="abcc7-154">上次修改图像的数据和时间。</span><span class="sxs-lookup"><span data-stu-id="abcc7-154">The data and time that the image was last modified.</span></span> <span data-ttu-id="abcc7-155">时间以 ISO 8601 格式显示，协调世界时 (UTC) 时间。</span><span class="sxs-lookup"><span data-stu-id="abcc7-155">The time is shown in ISO 8601 format and  Coordinated Universal Time (UTC) time.</span></span> <span data-ttu-id="abcc7-156">例如，2014 年 1 月 1 日午夜 UTC 显示为"2014-01-01T00：00：00Z"。</span><span class="sxs-lookup"><span data-stu-id="abcc7-156">For example, midnight UTC on Jan 1, 2014 appears as '2014-01-01T00:00:00Z'.</span></span>|
|<span data-ttu-id="abcc7-157">状态</span><span class="sxs-lookup"><span data-stu-id="abcc7-157">status</span></span>|<span data-ttu-id="abcc7-158">cloudPcDeviceImageStatus</span><span class="sxs-lookup"><span data-stu-id="abcc7-158">cloudPcDeviceImageStatus</span></span>|<span data-ttu-id="abcc7-159">云电脑上的图像状态。</span><span class="sxs-lookup"><span data-stu-id="abcc7-159">The status of the image on cloud PC.</span></span> <span data-ttu-id="abcc7-160">可取值为：`pending`、`ready`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="abcc7-160">Possible values are: `pending`, `ready`, `failed`.</span></span>|
|<span data-ttu-id="abcc7-161">statusDetails</span><span class="sxs-lookup"><span data-stu-id="abcc7-161">statusDetails</span></span>|<span data-ttu-id="abcc7-162">cloudPcDeviceImageStatusDetails</span><span class="sxs-lookup"><span data-stu-id="abcc7-162">cloudPcDeviceImageStatusDetails</span></span>|<span data-ttu-id="abcc7-163">图像状态的详细信息，指示上传失败的原因（如果适用）。</span><span class="sxs-lookup"><span data-stu-id="abcc7-163">The details of the image's status, which indicates why the upload failed, if applicable.</span></span> <span data-ttu-id="abcc7-164">可取值为：`internalServerError`、`sourceImageNotFound`。</span><span class="sxs-lookup"><span data-stu-id="abcc7-164">Possible values are: `internalServerError`, `sourceImageNotFound`.</span></span>|

### <a name="cloudpcdeviceimagestatus-values"></a><span data-ttu-id="abcc7-165">cloudPcDeviceImageStatus 值</span><span class="sxs-lookup"><span data-stu-id="abcc7-165">cloudPcDeviceImageStatus values</span></span>

|<span data-ttu-id="abcc7-166">成员</span><span class="sxs-lookup"><span data-stu-id="abcc7-166">Member</span></span>|<span data-ttu-id="abcc7-167">说明</span><span class="sxs-lookup"><span data-stu-id="abcc7-167">Description</span></span>|
|:---|:---|
|<span data-ttu-id="abcc7-168">挂起</span><span class="sxs-lookup"><span data-stu-id="abcc7-168">pending</span></span>|<span data-ttu-id="abcc7-169">图像上传正在进行中。</span><span class="sxs-lookup"><span data-stu-id="abcc7-169">The image upload is in progress.</span></span>|
|<span data-ttu-id="abcc7-170">ready</span><span class="sxs-lookup"><span data-stu-id="abcc7-170">ready</span></span>|<span data-ttu-id="abcc7-171">该映像已准备好在云电脑中使用。</span><span class="sxs-lookup"><span data-stu-id="abcc7-171">The image is ready for use on Cloud PCs.</span></span>|
|<span data-ttu-id="abcc7-172">failed</span><span class="sxs-lookup"><span data-stu-id="abcc7-172">failed</span></span>|<span data-ttu-id="abcc7-173">无法上载图像。</span><span class="sxs-lookup"><span data-stu-id="abcc7-173">The image couldn’t be uploaded.</span></span> |

### <a name="cloudpcdeviceimagestatusdetails-values"></a><span data-ttu-id="abcc7-174">cloudPcDeviceImageStatusDetails 值</span><span class="sxs-lookup"><span data-stu-id="abcc7-174">cloudPcDeviceImageStatusDetails values</span></span>

|<span data-ttu-id="abcc7-175">成员</span><span class="sxs-lookup"><span data-stu-id="abcc7-175">Member</span></span>|<span data-ttu-id="abcc7-176">说明</span><span class="sxs-lookup"><span data-stu-id="abcc7-176">Description</span></span>|
|:---|:---|
|<span data-ttu-id="abcc7-177">internalServerError</span><span class="sxs-lookup"><span data-stu-id="abcc7-177">internalServerError</span></span>|<span data-ttu-id="abcc7-178">处理映像时出现内部服务器错误。</span><span class="sxs-lookup"><span data-stu-id="abcc7-178">There was an internal server error while processing the image.</span></span>|
|<span data-ttu-id="abcc7-179">sourceImageNotFound</span><span class="sxs-lookup"><span data-stu-id="abcc7-179">sourceImageNotFound</span></span>|<span data-ttu-id="abcc7-180">源映像无效预配 Windows VM。</span><span class="sxs-lookup"><span data-stu-id="abcc7-180">The source image is not valid for provisioning a Windows VM with it.</span></span>|

## <a name="relationships"></a><span data-ttu-id="abcc7-181">关系</span><span class="sxs-lookup"><span data-stu-id="abcc7-181">Relationships</span></span>

<span data-ttu-id="abcc7-182">无。</span><span class="sxs-lookup"><span data-stu-id="abcc7-182">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="abcc7-183">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="abcc7-183">JSON representation</span></span>

<span data-ttu-id="abcc7-184">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="abcc7-184">The following is a JSON representation of the resource.</span></span>
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
