---
title: cloudPcDeviceImage 资源类型
description: 表示云电脑上的图像资源。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 782704beabce8131beb1f5c096d0e35a5a44ca3e
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563842"
---
# <a name="cloudpcdeviceimage-resource-type"></a><span data-ttu-id="71596-103">cloudPcDeviceImage 资源类型</span><span class="sxs-lookup"><span data-stu-id="71596-103">cloudPcDeviceImage resource type</span></span>

<span data-ttu-id="71596-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71596-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="71596-105">表示云电脑上的图像资源。</span><span class="sxs-lookup"><span data-stu-id="71596-105">Represents the image resource on cloud PC.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a><span data-ttu-id="71596-106">方法</span><span class="sxs-lookup"><span data-stu-id="71596-106">Methods</span></span>

|<span data-ttu-id="71596-107">方法</span><span class="sxs-lookup"><span data-stu-id="71596-107">Method</span></span>|<span data-ttu-id="71596-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="71596-108">Return type</span></span>|<span data-ttu-id="71596-109">说明</span><span class="sxs-lookup"><span data-stu-id="71596-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="71596-110">列出 deviceImages</span><span class="sxs-lookup"><span data-stu-id="71596-110">List deviceImages</span></span>](../api/virtualendpoint-list-deviceimages.md)|<span data-ttu-id="71596-111">[cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="71596-111">[cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) collection</span></span>|<span data-ttu-id="71596-112">列出 [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="71596-112">List the properties and relationships of [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) objects.</span></span>|
|[<span data-ttu-id="71596-113">获取 cloudPcDeviceImage</span><span class="sxs-lookup"><span data-stu-id="71596-113">Get cloudPcDeviceImage</span></span>](../api/cloudpcdeviceimage-get.md)|[<span data-ttu-id="71596-114">cloudPcDeviceImage</span><span class="sxs-lookup"><span data-stu-id="71596-114">cloudPcDeviceImage</span></span>](../resources/cloudpcdeviceimage.md)|<span data-ttu-id="71596-115">读取 [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="71596-115">Read the properties and relationships of a [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object.</span></span>|
|[<span data-ttu-id="71596-116">创建 cloudPcDeviceImage</span><span class="sxs-lookup"><span data-stu-id="71596-116">Create cloudPcDeviceImage</span></span>](../api/virtualendpoint-post-deviceimages.md)|[<span data-ttu-id="71596-117">cloudPcDeviceImage</span><span class="sxs-lookup"><span data-stu-id="71596-117">cloudPcDeviceImage</span></span>](../resources/cloudpcdeviceimage.md)|<span data-ttu-id="71596-118">创建新的 [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="71596-118">Create a new [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object.</span></span>|
|[<span data-ttu-id="71596-119">删除 cloudPcDeviceImage</span><span class="sxs-lookup"><span data-stu-id="71596-119">Delete cloudPcDeviceImage</span></span>](../api/cloudpcdeviceimage-delete.md)|<span data-ttu-id="71596-120">无</span><span class="sxs-lookup"><span data-stu-id="71596-120">None</span></span>|<span data-ttu-id="71596-121">删除 [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="71596-121">Delete a [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object.</span></span>|
|[<span data-ttu-id="71596-122">getSourceImages</span><span class="sxs-lookup"><span data-stu-id="71596-122">getSourceImages</span></span>](../api/cloudpcdeviceimage-getsourceimages.md)|<span data-ttu-id="71596-123">[cloudPcSourceDeviceImage](../resources/cloudpcsourcedeviceimage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="71596-123">[cloudPcSourceDeviceImage](../resources/cloudpcsourcedeviceimage.md) collection</span></span>|<span data-ttu-id="71596-124">获取 [cloudPcSourceDeviceImage](../resources/cloudpcsourcedeviceimage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="71596-124">Get [cloudPcSourceDeviceImage](../resources/cloudpcsourcedeviceimage.md) objects.</span></span>|

## <a name="properties"></a><span data-ttu-id="71596-125">属性</span><span class="sxs-lookup"><span data-stu-id="71596-125">Properties</span></span>

|<span data-ttu-id="71596-126">属性</span><span class="sxs-lookup"><span data-stu-id="71596-126">Property</span></span>|<span data-ttu-id="71596-127">类型</span><span class="sxs-lookup"><span data-stu-id="71596-127">Type</span></span>|<span data-ttu-id="71596-128">说明</span><span class="sxs-lookup"><span data-stu-id="71596-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71596-129">id</span><span class="sxs-lookup"><span data-stu-id="71596-129">id</span></span>|<span data-ttu-id="71596-130">String</span><span class="sxs-lookup"><span data-stu-id="71596-130">String</span></span>|<span data-ttu-id="71596-131">云电脑上的图像资源的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="71596-131">Unique identifier for the image resource on cloud PC.</span></span> <span data-ttu-id="71596-132">只读。</span><span class="sxs-lookup"><span data-stu-id="71596-132">Read-only.</span></span>|
|<span data-ttu-id="71596-133">sourceImageResourceId</span><span class="sxs-lookup"><span data-stu-id="71596-133">sourceImageResourceId</span></span>|<span data-ttu-id="71596-134">String</span><span class="sxs-lookup"><span data-stu-id="71596-134">String</span></span>|<span data-ttu-id="71596-135">Azure 上的源图像资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="71596-135">The ID of the source image resource on Azure.</span></span> <span data-ttu-id="71596-136">必需的格式： "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Compute/images/{imageName}"。</span><span class="sxs-lookup"><span data-stu-id="71596-136">Required format: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Compute/images/{imageName}".</span></span>|
|<span data-ttu-id="71596-137">displayName</span><span class="sxs-lookup"><span data-stu-id="71596-137">displayName</span></span>|<span data-ttu-id="71596-138">String</span><span class="sxs-lookup"><span data-stu-id="71596-138">String</span></span>|<span data-ttu-id="71596-139">图像的显示名称。</span><span class="sxs-lookup"><span data-stu-id="71596-139">The image's display name.</span></span>|
|<span data-ttu-id="71596-140">version</span><span class="sxs-lookup"><span data-stu-id="71596-140">version</span></span>|<span data-ttu-id="71596-141">String</span><span class="sxs-lookup"><span data-stu-id="71596-141">String</span></span>|<span data-ttu-id="71596-142">图像版本。</span><span class="sxs-lookup"><span data-stu-id="71596-142">The image version.</span></span> <span data-ttu-id="71596-143">例如：0.0.1、1.5.13。</span><span class="sxs-lookup"><span data-stu-id="71596-143">For example: 0.0.1, 1.5.13.</span></span>|
|<span data-ttu-id="71596-144">osBuildNumber</span><span class="sxs-lookup"><span data-stu-id="71596-144">osBuildNumber</span></span>|<span data-ttu-id="71596-145">String</span><span class="sxs-lookup"><span data-stu-id="71596-145">String</span></span>|<span data-ttu-id="71596-146">图像的 OS 内部版本。</span><span class="sxs-lookup"><span data-stu-id="71596-146">The image's OS build version.</span></span> <span data-ttu-id="71596-147">例如：1909。</span><span class="sxs-lookup"><span data-stu-id="71596-147">For example: 1909.</span></span>|
|<span data-ttu-id="71596-148">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="71596-148">operatingSystem</span></span>|<span data-ttu-id="71596-149">String</span><span class="sxs-lookup"><span data-stu-id="71596-149">String</span></span>|<span data-ttu-id="71596-150">图像的操作系统。</span><span class="sxs-lookup"><span data-stu-id="71596-150">The image's operating system.</span></span> <span data-ttu-id="71596-151">例如： Windows 10 企业版。</span><span class="sxs-lookup"><span data-stu-id="71596-151">For example: Windows 10 Enterprise.</span></span>|
|<span data-ttu-id="71596-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="71596-152">lastModifiedDateTime</span></span>|<span data-ttu-id="71596-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71596-153">DateTimeOffset</span></span>|<span data-ttu-id="71596-154">上次修改图像的数据和时间。</span><span class="sxs-lookup"><span data-stu-id="71596-154">The data and time that the image was last modified.</span></span> <span data-ttu-id="71596-155">时间以 ISO 8601 格式和协调世界时 (UTC) 时间显示。</span><span class="sxs-lookup"><span data-stu-id="71596-155">The time is shown in ISO 8601 format and  Coordinated Universal Time (UTC) time.</span></span> <span data-ttu-id="71596-156">例如，2014年1月1日午夜 UTC 显示为 "2014-01-01T00：00： 00Z"。</span><span class="sxs-lookup"><span data-stu-id="71596-156">For example, midnight UTC on Jan 1, 2014 appears as '2014-01-01T00:00:00Z'.</span></span>|
|<span data-ttu-id="71596-157">status</span><span class="sxs-lookup"><span data-stu-id="71596-157">status</span></span>|<span data-ttu-id="71596-158">cloudPcDeviceImageStatus</span><span class="sxs-lookup"><span data-stu-id="71596-158">cloudPcDeviceImageStatus</span></span>|<span data-ttu-id="71596-159">云电脑上的映像的状态。</span><span class="sxs-lookup"><span data-stu-id="71596-159">The status of the image on cloud PC.</span></span> <span data-ttu-id="71596-160">可能的状态包括 "上载挂起"、"上载时失败" 或 "就绪" 可供使用。</span><span class="sxs-lookup"><span data-stu-id="71596-160">Possible status include upload pending, failed to upload, or ready to use.</span></span> <span data-ttu-id="71596-161">可取值为：`pending`、`ready`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="71596-161">Possible values are: `pending`, `ready`, `failed`.</span></span>|
|<span data-ttu-id="71596-162">statusDetails</span><span class="sxs-lookup"><span data-stu-id="71596-162">statusDetails</span></span>|<span data-ttu-id="71596-163">cloudPcDeviceImageStatusDetails</span><span class="sxs-lookup"><span data-stu-id="71596-163">cloudPcDeviceImageStatusDetails</span></span>|<span data-ttu-id="71596-164">图像状态的详细信息，用于指示上载失败的原因（如果适用）。</span><span class="sxs-lookup"><span data-stu-id="71596-164">The details of the image's status, which indicates why the upload failed, if applicable.</span></span> <span data-ttu-id="71596-165">可取值为：`internalServerError`、`sourceImageNotFound`。</span><span class="sxs-lookup"><span data-stu-id="71596-165">Possible values are: `internalServerError`, `sourceImageNotFound`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="71596-166">关系</span><span class="sxs-lookup"><span data-stu-id="71596-166">Relationships</span></span>

<span data-ttu-id="71596-167">无。</span><span class="sxs-lookup"><span data-stu-id="71596-167">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="71596-168">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="71596-168">JSON representation</span></span>

<span data-ttu-id="71596-169">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="71596-169">The following is a JSON representation of the resource.</span></span>
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
