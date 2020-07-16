---
title: deviceLogCollectionResponse 资源类型
description: Windows 日志集合请求实体。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1f9b6dcfda30845138c4576b3a100b8fbe3ff26c
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/14/2020
ms.locfileid: "45124185"
---
# <a name="devicelogcollectionresponse-resource-type"></a><span data-ttu-id="cf471-103">deviceLogCollectionResponse 资源类型</span><span class="sxs-lookup"><span data-stu-id="cf471-103">deviceLogCollectionResponse resource type</span></span>

<span data-ttu-id="cf471-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf471-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cf471-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="cf471-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cf471-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cf471-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cf471-107">Windows 日志集合请求实体。</span><span class="sxs-lookup"><span data-stu-id="cf471-107">Windows Log Collection request entity.</span></span>

## <a name="methods"></a><span data-ttu-id="cf471-108">方法</span><span class="sxs-lookup"><span data-stu-id="cf471-108">Methods</span></span>
|<span data-ttu-id="cf471-109">方法</span><span class="sxs-lookup"><span data-stu-id="cf471-109">Method</span></span>|<span data-ttu-id="cf471-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="cf471-110">Return Type</span></span>|<span data-ttu-id="cf471-111">说明</span><span class="sxs-lookup"><span data-stu-id="cf471-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="cf471-112">列出 deviceLogCollectionResponses</span><span class="sxs-lookup"><span data-stu-id="cf471-112">List deviceLogCollectionResponses</span></span>](../api/intune-devices-devicelogcollectionresponse-list.md)|<span data-ttu-id="cf471-113">[deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md)集合</span><span class="sxs-lookup"><span data-stu-id="cf471-113">[deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) collection</span></span>|<span data-ttu-id="cf471-114">列出[deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cf471-114">List properties and relationships of the [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) objects.</span></span>|
|[<span data-ttu-id="cf471-115">获取 deviceLogCollectionResponse</span><span class="sxs-lookup"><span data-stu-id="cf471-115">Get deviceLogCollectionResponse</span></span>](../api/intune-devices-devicelogcollectionresponse-get.md)|[<span data-ttu-id="cf471-116">deviceLogCollectionResponse</span><span class="sxs-lookup"><span data-stu-id="cf471-116">deviceLogCollectionResponse</span></span>](../resources/intune-devices-devicelogcollectionresponse.md)|<span data-ttu-id="cf471-117">读取[deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cf471-117">Read properties and relationships of the [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) object.</span></span>|
|[<span data-ttu-id="cf471-118">createDownloadUrl 操作</span><span class="sxs-lookup"><span data-stu-id="cf471-118">createDownloadUrl action</span></span>](../api/intune-devices-devicelogcollectionresponse-createdownloadurl.md)|<span data-ttu-id="cf471-119">String</span><span class="sxs-lookup"><span data-stu-id="cf471-119">String</span></span>|<span data-ttu-id="cf471-120">尚未记录</span><span class="sxs-lookup"><span data-stu-id="cf471-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="cf471-121">属性</span><span class="sxs-lookup"><span data-stu-id="cf471-121">Properties</span></span>
|<span data-ttu-id="cf471-122">属性</span><span class="sxs-lookup"><span data-stu-id="cf471-122">Property</span></span>|<span data-ttu-id="cf471-123">类型</span><span class="sxs-lookup"><span data-stu-id="cf471-123">Type</span></span>|<span data-ttu-id="cf471-124">说明</span><span class="sxs-lookup"><span data-stu-id="cf471-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf471-125">id</span><span class="sxs-lookup"><span data-stu-id="cf471-125">id</span></span>|<span data-ttu-id="cf471-126">String</span><span class="sxs-lookup"><span data-stu-id="cf471-126">String</span></span>|<span data-ttu-id="cf471-127">TenantId_deviceId_requestId 形式的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="cf471-127">The unique identifier in the form of tenantId_deviceId_requestId</span></span>|
|<span data-ttu-id="cf471-128">status</span><span class="sxs-lookup"><span data-stu-id="cf471-128">status</span></span>|<span data-ttu-id="cf471-129">String</span><span class="sxs-lookup"><span data-stu-id="cf471-129">String</span></span>|<span data-ttu-id="cf471-130">日志集合请求的状态</span><span class="sxs-lookup"><span data-stu-id="cf471-130">The status of the log collection request</span></span>|
|<span data-ttu-id="cf471-131">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="cf471-131">managedDeviceId</span></span>|<span data-ttu-id="cf471-132">Guid</span><span class="sxs-lookup"><span data-stu-id="cf471-132">Guid</span></span>|<span data-ttu-id="cf471-133">设备 Id</span><span class="sxs-lookup"><span data-stu-id="cf471-133">The device Id</span></span>|
|<span data-ttu-id="cf471-134">errorCode</span><span class="sxs-lookup"><span data-stu-id="cf471-134">errorCode</span></span>|<span data-ttu-id="cf471-135">Int64</span><span class="sxs-lookup"><span data-stu-id="cf471-135">Int64</span></span>|<span data-ttu-id="cf471-136">错误代码（如果有）。</span><span class="sxs-lookup"><span data-stu-id="cf471-136">The error code, if any.</span></span> <span data-ttu-id="cf471-137">有效值-9.22337203685478 E + 18 to 9.22337203685478 E + 18</span><span class="sxs-lookup"><span data-stu-id="cf471-137">Valid values -9.22337203685478E+18 to 9.22337203685478E+18</span></span>|
|<span data-ttu-id="cf471-138">requestedDateTimeUTC</span><span class="sxs-lookup"><span data-stu-id="cf471-138">requestedDateTimeUTC</span></span>|<span data-ttu-id="cf471-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf471-139">DateTimeOffset</span></span>|<span data-ttu-id="cf471-140">请求的日期时间</span><span class="sxs-lookup"><span data-stu-id="cf471-140">The DateTime of the request</span></span>|
|<span data-ttu-id="cf471-141">receivedDateTimeUTC</span><span class="sxs-lookup"><span data-stu-id="cf471-141">receivedDateTimeUTC</span></span>|<span data-ttu-id="cf471-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf471-142">DateTimeOffset</span></span>|<span data-ttu-id="cf471-143">收到请求的日期/时间</span><span class="sxs-lookup"><span data-stu-id="cf471-143">The DateTime the request was received</span></span>|
|<span data-ttu-id="cf471-144">initiatedByUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="cf471-144">initiatedByUserPrincipalName</span></span>|<span data-ttu-id="cf471-145">String</span><span class="sxs-lookup"><span data-stu-id="cf471-145">String</span></span>|<span data-ttu-id="cf471-146">为其启动请求的 UPN</span><span class="sxs-lookup"><span data-stu-id="cf471-146">The UPN for who initiated the request</span></span>|
|<span data-ttu-id="cf471-147">expirationDateTimeUTC</span><span class="sxs-lookup"><span data-stu-id="cf471-147">expirationDateTimeUTC</span></span>|<span data-ttu-id="cf471-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf471-148">DateTimeOffset</span></span>|<span data-ttu-id="cf471-149">日志过期日期的日期/时间</span><span class="sxs-lookup"><span data-stu-id="cf471-149">The DateTime of the expiration of the logs</span></span>|
|<span data-ttu-id="cf471-150">大小</span><span class="sxs-lookup"><span data-stu-id="cf471-150">size</span></span>|<span data-ttu-id="cf471-151">双精度</span><span class="sxs-lookup"><span data-stu-id="cf471-151">Double</span></span>|<span data-ttu-id="cf471-152">日志的大小。</span><span class="sxs-lookup"><span data-stu-id="cf471-152">The size of the logs.</span></span> <span data-ttu-id="cf471-153">有效值-1.79769313486232 E + 308 到 1.79769313486232 E + 308</span><span class="sxs-lookup"><span data-stu-id="cf471-153">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|

## <a name="relationships"></a><span data-ttu-id="cf471-154">关系</span><span class="sxs-lookup"><span data-stu-id="cf471-154">Relationships</span></span>
<span data-ttu-id="cf471-155">无</span><span class="sxs-lookup"><span data-stu-id="cf471-155">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cf471-156">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cf471-156">JSON Representation</span></span>
<span data-ttu-id="cf471-157">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cf471-157">Here is a JSON representation of the resource.</span></span>
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



