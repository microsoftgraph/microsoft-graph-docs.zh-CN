---
title: deviceLogCollectionResponse 资源类型
description: Windows 日志集合请求实体。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3a4316655cc7ca10205165bac1b96579eb135713
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060158"
---
# <a name="devicelogcollectionresponse-resource-type"></a><span data-ttu-id="0acac-103">deviceLogCollectionResponse 资源类型</span><span class="sxs-lookup"><span data-stu-id="0acac-103">deviceLogCollectionResponse resource type</span></span>

<span data-ttu-id="0acac-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0acac-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0acac-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0acac-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0acac-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0acac-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0acac-107">Windows 日志集合请求实体。</span><span class="sxs-lookup"><span data-stu-id="0acac-107">Windows Log Collection request entity.</span></span>

## <a name="methods"></a><span data-ttu-id="0acac-108">方法</span><span class="sxs-lookup"><span data-stu-id="0acac-108">Methods</span></span>
|<span data-ttu-id="0acac-109">方法</span><span class="sxs-lookup"><span data-stu-id="0acac-109">Method</span></span>|<span data-ttu-id="0acac-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="0acac-110">Return Type</span></span>|<span data-ttu-id="0acac-111">说明</span><span class="sxs-lookup"><span data-stu-id="0acac-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0acac-112">列出 deviceLogCollectionResponses</span><span class="sxs-lookup"><span data-stu-id="0acac-112">List deviceLogCollectionResponses</span></span>](../api/intune-devices-devicelogcollectionresponse-list.md)|<span data-ttu-id="0acac-113">[deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0acac-113">[deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) collection</span></span>|<span data-ttu-id="0acac-114">列出 [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0acac-114">List properties and relationships of the [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) objects.</span></span>|
|[<span data-ttu-id="0acac-115">获取 deviceLogCollectionResponse</span><span class="sxs-lookup"><span data-stu-id="0acac-115">Get deviceLogCollectionResponse</span></span>](../api/intune-devices-devicelogcollectionresponse-get.md)|[<span data-ttu-id="0acac-116">deviceLogCollectionResponse</span><span class="sxs-lookup"><span data-stu-id="0acac-116">deviceLogCollectionResponse</span></span>](../resources/intune-devices-devicelogcollectionresponse.md)|<span data-ttu-id="0acac-117">读取 [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0acac-117">Read properties and relationships of the [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) object.</span></span>|
|[<span data-ttu-id="0acac-118">创建 deviceLogCollectionResponse</span><span class="sxs-lookup"><span data-stu-id="0acac-118">Create deviceLogCollectionResponse</span></span>](../api/intune-devices-devicelogcollectionresponse-create.md)|[<span data-ttu-id="0acac-119">deviceLogCollectionResponse</span><span class="sxs-lookup"><span data-stu-id="0acac-119">deviceLogCollectionResponse</span></span>](../resources/intune-devices-devicelogcollectionresponse.md)|<span data-ttu-id="0acac-120">创建新的 [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0acac-120">Create a new [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) object.</span></span>|
|[<span data-ttu-id="0acac-121">删除 deviceLogCollectionResponse</span><span class="sxs-lookup"><span data-stu-id="0acac-121">Delete deviceLogCollectionResponse</span></span>](../api/intune-devices-devicelogcollectionresponse-delete.md)|<span data-ttu-id="0acac-122">无</span><span class="sxs-lookup"><span data-stu-id="0acac-122">None</span></span>|<span data-ttu-id="0acac-123">删除 [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md)。</span><span class="sxs-lookup"><span data-stu-id="0acac-123">Deletes a [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md).</span></span>|
|[<span data-ttu-id="0acac-124">更新 deviceLogCollectionResponse</span><span class="sxs-lookup"><span data-stu-id="0acac-124">Update deviceLogCollectionResponse</span></span>](../api/intune-devices-devicelogcollectionresponse-update.md)|[<span data-ttu-id="0acac-125">deviceLogCollectionResponse</span><span class="sxs-lookup"><span data-stu-id="0acac-125">deviceLogCollectionResponse</span></span>](../resources/intune-devices-devicelogcollectionresponse.md)|<span data-ttu-id="0acac-126">更新 [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0acac-126">Update the properties of a [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) object.</span></span>|
|[<span data-ttu-id="0acac-127">createDownloadUrl 操作</span><span class="sxs-lookup"><span data-stu-id="0acac-127">createDownloadUrl action</span></span>](../api/intune-devices-devicelogcollectionresponse-createdownloadurl.md)|<span data-ttu-id="0acac-128">String</span><span class="sxs-lookup"><span data-stu-id="0acac-128">String</span></span>|<span data-ttu-id="0acac-129">尚未记录</span><span class="sxs-lookup"><span data-stu-id="0acac-129">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="0acac-130">属性</span><span class="sxs-lookup"><span data-stu-id="0acac-130">Properties</span></span>
|<span data-ttu-id="0acac-131">属性</span><span class="sxs-lookup"><span data-stu-id="0acac-131">Property</span></span>|<span data-ttu-id="0acac-132">类型</span><span class="sxs-lookup"><span data-stu-id="0acac-132">Type</span></span>|<span data-ttu-id="0acac-133">说明</span><span class="sxs-lookup"><span data-stu-id="0acac-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0acac-134">id</span><span class="sxs-lookup"><span data-stu-id="0acac-134">id</span></span>|<span data-ttu-id="0acac-135">String</span><span class="sxs-lookup"><span data-stu-id="0acac-135">String</span></span>|<span data-ttu-id="0acac-136">TenantId_deviceId_requestId 形式的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="0acac-136">The unique identifier in the form of tenantId_deviceId_requestId</span></span>|
|<span data-ttu-id="0acac-137">状态</span><span class="sxs-lookup"><span data-stu-id="0acac-137">status</span></span>|<span data-ttu-id="0acac-138">String</span><span class="sxs-lookup"><span data-stu-id="0acac-138">String</span></span>|<span data-ttu-id="0acac-139">日志集合请求的状态</span><span class="sxs-lookup"><span data-stu-id="0acac-139">The status of the log collection request</span></span>|
|<span data-ttu-id="0acac-140">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="0acac-140">managedDeviceId</span></span>|<span data-ttu-id="0acac-141">Guid</span><span class="sxs-lookup"><span data-stu-id="0acac-141">Guid</span></span>|<span data-ttu-id="0acac-142">设备 Id</span><span class="sxs-lookup"><span data-stu-id="0acac-142">The device Id</span></span>|
|<span data-ttu-id="0acac-143">errorCode</span><span class="sxs-lookup"><span data-stu-id="0acac-143">errorCode</span></span>|<span data-ttu-id="0acac-144">Int64</span><span class="sxs-lookup"><span data-stu-id="0acac-144">Int64</span></span>|<span data-ttu-id="0acac-145">错误代码（如果有）。</span><span class="sxs-lookup"><span data-stu-id="0acac-145">The error code, if any.</span></span> <span data-ttu-id="0acac-146">有效值-9.22337203685478 E + 18 to 9.22337203685478 E + 18</span><span class="sxs-lookup"><span data-stu-id="0acac-146">Valid values -9.22337203685478E+18 to 9.22337203685478E+18</span></span>|
|<span data-ttu-id="0acac-147">requestedDateTimeUTC</span><span class="sxs-lookup"><span data-stu-id="0acac-147">requestedDateTimeUTC</span></span>|<span data-ttu-id="0acac-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0acac-148">DateTimeOffset</span></span>|<span data-ttu-id="0acac-149">请求的日期时间</span><span class="sxs-lookup"><span data-stu-id="0acac-149">The DateTime of the request</span></span>|
|<span data-ttu-id="0acac-150">receivedDateTimeUTC</span><span class="sxs-lookup"><span data-stu-id="0acac-150">receivedDateTimeUTC</span></span>|<span data-ttu-id="0acac-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0acac-151">DateTimeOffset</span></span>|<span data-ttu-id="0acac-152">收到请求的日期/时间</span><span class="sxs-lookup"><span data-stu-id="0acac-152">The DateTime the request was received</span></span>|
|<span data-ttu-id="0acac-153">initiatedByUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0acac-153">initiatedByUserPrincipalName</span></span>|<span data-ttu-id="0acac-154">String</span><span class="sxs-lookup"><span data-stu-id="0acac-154">String</span></span>|<span data-ttu-id="0acac-155">为其启动请求的 UPN</span><span class="sxs-lookup"><span data-stu-id="0acac-155">The UPN for who initiated the request</span></span>|
|<span data-ttu-id="0acac-156">expirationDateTimeUTC</span><span class="sxs-lookup"><span data-stu-id="0acac-156">expirationDateTimeUTC</span></span>|<span data-ttu-id="0acac-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0acac-157">DateTimeOffset</span></span>|<span data-ttu-id="0acac-158">日志过期日期的日期/时间</span><span class="sxs-lookup"><span data-stu-id="0acac-158">The DateTime of the expiration of the logs</span></span>|
|<span data-ttu-id="0acac-159">size</span><span class="sxs-lookup"><span data-stu-id="0acac-159">size</span></span>|<span data-ttu-id="0acac-160">双精度</span><span class="sxs-lookup"><span data-stu-id="0acac-160">Double</span></span>|<span data-ttu-id="0acac-161">日志的大小。</span><span class="sxs-lookup"><span data-stu-id="0acac-161">The size of the logs.</span></span> <span data-ttu-id="0acac-162">有效值-1.79769313486232 E + 308 到 1.79769313486232 E + 308</span><span class="sxs-lookup"><span data-stu-id="0acac-162">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|

## <a name="relationships"></a><span data-ttu-id="0acac-163">关系</span><span class="sxs-lookup"><span data-stu-id="0acac-163">Relationships</span></span>
<span data-ttu-id="0acac-164">无</span><span class="sxs-lookup"><span data-stu-id="0acac-164">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0acac-165">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0acac-165">JSON Representation</span></span>
<span data-ttu-id="0acac-166">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0acac-166">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceLogCollectionResponse"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceLogCollectionResponse",
  "id": "String (identifier)",
  "status": "String",
  "managedDeviceId": "Guid",
  "errorCode": 1024,
  "requestedDateTimeUTC": "String (timestamp)",
  "receivedDateTimeUTC": "String (timestamp)",
  "initiatedByUserPrincipalName": "String",
  "expirationDateTimeUTC": "String (timestamp)",
  "size": "4.2"
}
```






