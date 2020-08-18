---
title: deviceLogCollectionResponse 资源类型
description: Windows 日志集合请求实体。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4c3a7725f0f02c0ba2b8588c57179fa80316c595
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/18/2020
ms.locfileid: "46792973"
---
# <a name="devicelogcollectionresponse-resource-type"></a><span data-ttu-id="bea38-103">deviceLogCollectionResponse 资源类型</span><span class="sxs-lookup"><span data-stu-id="bea38-103">deviceLogCollectionResponse resource type</span></span>

<span data-ttu-id="bea38-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bea38-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bea38-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bea38-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bea38-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bea38-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bea38-107">Windows 日志集合请求实体。</span><span class="sxs-lookup"><span data-stu-id="bea38-107">Windows Log Collection request entity.</span></span>

## <a name="methods"></a><span data-ttu-id="bea38-108">方法</span><span class="sxs-lookup"><span data-stu-id="bea38-108">Methods</span></span>
|<span data-ttu-id="bea38-109">方法</span><span class="sxs-lookup"><span data-stu-id="bea38-109">Method</span></span>|<span data-ttu-id="bea38-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="bea38-110">Return Type</span></span>|<span data-ttu-id="bea38-111">说明</span><span class="sxs-lookup"><span data-stu-id="bea38-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="bea38-112">列出 deviceLogCollectionResponses</span><span class="sxs-lookup"><span data-stu-id="bea38-112">List deviceLogCollectionResponses</span></span>](../api/intune-devices-devicelogcollectionresponse-list.md)|<span data-ttu-id="bea38-113">[deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) 集合</span><span class="sxs-lookup"><span data-stu-id="bea38-113">[deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) collection</span></span>|<span data-ttu-id="bea38-114">列出 [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="bea38-114">List properties and relationships of the [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) objects.</span></span>|
|[<span data-ttu-id="bea38-115">获取 deviceLogCollectionResponse</span><span class="sxs-lookup"><span data-stu-id="bea38-115">Get deviceLogCollectionResponse</span></span>](../api/intune-devices-devicelogcollectionresponse-get.md)|[<span data-ttu-id="bea38-116">deviceLogCollectionResponse</span><span class="sxs-lookup"><span data-stu-id="bea38-116">deviceLogCollectionResponse</span></span>](../resources/intune-devices-devicelogcollectionresponse.md)|<span data-ttu-id="bea38-117">读取 [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="bea38-117">Read properties and relationships of the [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) object.</span></span>|
|[<span data-ttu-id="bea38-118">创建 deviceLogCollectionResponse</span><span class="sxs-lookup"><span data-stu-id="bea38-118">Create deviceLogCollectionResponse</span></span>](../api/intune-devices-devicelogcollectionresponse-create.md)|[<span data-ttu-id="bea38-119">deviceLogCollectionResponse</span><span class="sxs-lookup"><span data-stu-id="bea38-119">deviceLogCollectionResponse</span></span>](../resources/intune-devices-devicelogcollectionresponse.md)|<span data-ttu-id="bea38-120">创建新的 [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bea38-120">Create a new [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) object.</span></span>|
|[<span data-ttu-id="bea38-121">删除 deviceLogCollectionResponse</span><span class="sxs-lookup"><span data-stu-id="bea38-121">Delete deviceLogCollectionResponse</span></span>](../api/intune-devices-devicelogcollectionresponse-delete.md)|<span data-ttu-id="bea38-122">无</span><span class="sxs-lookup"><span data-stu-id="bea38-122">None</span></span>|<span data-ttu-id="bea38-123">删除 [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md)。</span><span class="sxs-lookup"><span data-stu-id="bea38-123">Deletes a [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md).</span></span>|
|[<span data-ttu-id="bea38-124">更新 deviceLogCollectionResponse</span><span class="sxs-lookup"><span data-stu-id="bea38-124">Update deviceLogCollectionResponse</span></span>](../api/intune-devices-devicelogcollectionresponse-update.md)|[<span data-ttu-id="bea38-125">deviceLogCollectionResponse</span><span class="sxs-lookup"><span data-stu-id="bea38-125">deviceLogCollectionResponse</span></span>](../resources/intune-devices-devicelogcollectionresponse.md)|<span data-ttu-id="bea38-126">更新 [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="bea38-126">Update the properties of a [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) object.</span></span>|
|[<span data-ttu-id="bea38-127">createDownloadUrl 操作</span><span class="sxs-lookup"><span data-stu-id="bea38-127">createDownloadUrl action</span></span>](../api/intune-devices-devicelogcollectionresponse-createdownloadurl.md)|<span data-ttu-id="bea38-128">String</span><span class="sxs-lookup"><span data-stu-id="bea38-128">String</span></span>|<span data-ttu-id="bea38-129">尚未记录</span><span class="sxs-lookup"><span data-stu-id="bea38-129">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="bea38-130">属性</span><span class="sxs-lookup"><span data-stu-id="bea38-130">Properties</span></span>
|<span data-ttu-id="bea38-131">属性</span><span class="sxs-lookup"><span data-stu-id="bea38-131">Property</span></span>|<span data-ttu-id="bea38-132">类型</span><span class="sxs-lookup"><span data-stu-id="bea38-132">Type</span></span>|<span data-ttu-id="bea38-133">说明</span><span class="sxs-lookup"><span data-stu-id="bea38-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bea38-134">id</span><span class="sxs-lookup"><span data-stu-id="bea38-134">id</span></span>|<span data-ttu-id="bea38-135">String</span><span class="sxs-lookup"><span data-stu-id="bea38-135">String</span></span>|<span data-ttu-id="bea38-136">TenantId_deviceId_requestId 形式的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="bea38-136">The unique identifier in the form of tenantId_deviceId_requestId</span></span>|
|<span data-ttu-id="bea38-137">status</span><span class="sxs-lookup"><span data-stu-id="bea38-137">status</span></span>|<span data-ttu-id="bea38-138">String</span><span class="sxs-lookup"><span data-stu-id="bea38-138">String</span></span>|<span data-ttu-id="bea38-139">日志集合请求的状态</span><span class="sxs-lookup"><span data-stu-id="bea38-139">The status of the log collection request</span></span>|
|<span data-ttu-id="bea38-140">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="bea38-140">managedDeviceId</span></span>|<span data-ttu-id="bea38-141">Guid</span><span class="sxs-lookup"><span data-stu-id="bea38-141">Guid</span></span>|<span data-ttu-id="bea38-142">设备 Id</span><span class="sxs-lookup"><span data-stu-id="bea38-142">The device Id</span></span>|
|<span data-ttu-id="bea38-143">errorCode</span><span class="sxs-lookup"><span data-stu-id="bea38-143">errorCode</span></span>|<span data-ttu-id="bea38-144">Int64</span><span class="sxs-lookup"><span data-stu-id="bea38-144">Int64</span></span>|<span data-ttu-id="bea38-145">错误代码（如果有）。</span><span class="sxs-lookup"><span data-stu-id="bea38-145">The error code, if any.</span></span> <span data-ttu-id="bea38-146">有效值-9.22337203685478 E + 18 to 9.22337203685478 E + 18</span><span class="sxs-lookup"><span data-stu-id="bea38-146">Valid values -9.22337203685478E+18 to 9.22337203685478E+18</span></span>|
|<span data-ttu-id="bea38-147">requestedDateTimeUTC</span><span class="sxs-lookup"><span data-stu-id="bea38-147">requestedDateTimeUTC</span></span>|<span data-ttu-id="bea38-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bea38-148">DateTimeOffset</span></span>|<span data-ttu-id="bea38-149">请求的日期时间</span><span class="sxs-lookup"><span data-stu-id="bea38-149">The DateTime of the request</span></span>|
|<span data-ttu-id="bea38-150">receivedDateTimeUTC</span><span class="sxs-lookup"><span data-stu-id="bea38-150">receivedDateTimeUTC</span></span>|<span data-ttu-id="bea38-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bea38-151">DateTimeOffset</span></span>|<span data-ttu-id="bea38-152">收到请求的日期/时间</span><span class="sxs-lookup"><span data-stu-id="bea38-152">The DateTime the request was received</span></span>|
|<span data-ttu-id="bea38-153">initiatedByUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="bea38-153">initiatedByUserPrincipalName</span></span>|<span data-ttu-id="bea38-154">String</span><span class="sxs-lookup"><span data-stu-id="bea38-154">String</span></span>|<span data-ttu-id="bea38-155">为其启动请求的 UPN</span><span class="sxs-lookup"><span data-stu-id="bea38-155">The UPN for who initiated the request</span></span>|
|<span data-ttu-id="bea38-156">expirationDateTimeUTC</span><span class="sxs-lookup"><span data-stu-id="bea38-156">expirationDateTimeUTC</span></span>|<span data-ttu-id="bea38-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bea38-157">DateTimeOffset</span></span>|<span data-ttu-id="bea38-158">日志过期日期的日期/时间</span><span class="sxs-lookup"><span data-stu-id="bea38-158">The DateTime of the expiration of the logs</span></span>|
|<span data-ttu-id="bea38-159">size</span><span class="sxs-lookup"><span data-stu-id="bea38-159">size</span></span>|<span data-ttu-id="bea38-160">双精度</span><span class="sxs-lookup"><span data-stu-id="bea38-160">Double</span></span>|<span data-ttu-id="bea38-161">日志的大小。</span><span class="sxs-lookup"><span data-stu-id="bea38-161">The size of the logs.</span></span> <span data-ttu-id="bea38-162">有效值-1.79769313486232 E + 308 到 1.79769313486232 E + 308</span><span class="sxs-lookup"><span data-stu-id="bea38-162">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|

## <a name="relationships"></a><span data-ttu-id="bea38-163">关系</span><span class="sxs-lookup"><span data-stu-id="bea38-163">Relationships</span></span>
<span data-ttu-id="bea38-164">无</span><span class="sxs-lookup"><span data-stu-id="bea38-164">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bea38-165">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bea38-165">JSON Representation</span></span>
<span data-ttu-id="bea38-166">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bea38-166">Here is a JSON representation of the resource.</span></span>
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



