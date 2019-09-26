---
title: deviceManagementScriptRunSummary 资源类型
description: 包含设备管理脚本的运行摘要的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 28337464b731c2d5bd833451574b591fd955a41b
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37196964"
---
# <a name="devicemanagementscriptrunsummary-resource-type"></a><span data-ttu-id="4e446-103">deviceManagementScriptRunSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="4e446-103">deviceManagementScriptRunSummary resource type</span></span>

> <span data-ttu-id="4e446-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4e446-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4e446-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4e446-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4e446-106">包含设备管理脚本的运行摘要的属性。</span><span class="sxs-lookup"><span data-stu-id="4e446-106">Contains properties for the run summary of a device management script.</span></span>

## <a name="methods"></a><span data-ttu-id="4e446-107">方法</span><span class="sxs-lookup"><span data-stu-id="4e446-107">Methods</span></span>
|<span data-ttu-id="4e446-108">方法</span><span class="sxs-lookup"><span data-stu-id="4e446-108">Method</span></span>|<span data-ttu-id="4e446-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="4e446-109">Return Type</span></span>|<span data-ttu-id="4e446-110">说明</span><span class="sxs-lookup"><span data-stu-id="4e446-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4e446-111">获取 deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="4e446-111">Get deviceManagementScriptRunSummary</span></span>](../api/intune-devices-devicemanagementscriptrunsummary-get.md)|[<span data-ttu-id="4e446-112">deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="4e446-112">deviceManagementScriptRunSummary</span></span>](../resources/intune-devices-devicemanagementscriptrunsummary.md)|<span data-ttu-id="4e446-113">读取[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4e446-113">Read properties and relationships of the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>|
|[<span data-ttu-id="4e446-114">更新 deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="4e446-114">Update deviceManagementScriptRunSummary</span></span>](../api/intune-devices-devicemanagementscriptrunsummary-update.md)|[<span data-ttu-id="4e446-115">deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="4e446-115">deviceManagementScriptRunSummary</span></span>](../resources/intune-devices-devicemanagementscriptrunsummary.md)|<span data-ttu-id="4e446-116">更新[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4e446-116">Update the properties of a [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="4e446-117">属性</span><span class="sxs-lookup"><span data-stu-id="4e446-117">Properties</span></span>
|<span data-ttu-id="4e446-118">属性</span><span class="sxs-lookup"><span data-stu-id="4e446-118">Property</span></span>|<span data-ttu-id="4e446-119">类型</span><span class="sxs-lookup"><span data-stu-id="4e446-119">Type</span></span>|<span data-ttu-id="4e446-120">说明</span><span class="sxs-lookup"><span data-stu-id="4e446-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e446-121">id</span><span class="sxs-lookup"><span data-stu-id="4e446-121">id</span></span>|<span data-ttu-id="4e446-122">String</span><span class="sxs-lookup"><span data-stu-id="4e446-122">String</span></span>|<span data-ttu-id="4e446-123">设备管理脚本运行摘要实体的键。</span><span class="sxs-lookup"><span data-stu-id="4e446-123">Key of the device management script run summary entity.</span></span> <span data-ttu-id="4e446-124">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4e446-124">This property is read-only.</span></span>|
|<span data-ttu-id="4e446-125">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4e446-125">successDeviceCount</span></span>|<span data-ttu-id="4e446-126">Int32</span><span class="sxs-lookup"><span data-stu-id="4e446-126">Int32</span></span>|<span data-ttu-id="4e446-127">成功设备计数。</span><span class="sxs-lookup"><span data-stu-id="4e446-127">Success device count.</span></span>|
|<span data-ttu-id="4e446-128">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4e446-128">errorDeviceCount</span></span>|<span data-ttu-id="4e446-129">Int32</span><span class="sxs-lookup"><span data-stu-id="4e446-129">Int32</span></span>|<span data-ttu-id="4e446-130">错误设备计数。</span><span class="sxs-lookup"><span data-stu-id="4e446-130">Error device count.</span></span>|
|<span data-ttu-id="4e446-131">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4e446-131">compliantDeviceCount</span></span>|<span data-ttu-id="4e446-132">Int32</span><span class="sxs-lookup"><span data-stu-id="4e446-132">Int32</span></span>|<span data-ttu-id="4e446-133">合规设备计数。</span><span class="sxs-lookup"><span data-stu-id="4e446-133">Compliant device count.</span></span>|
|<span data-ttu-id="4e446-134">notCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4e446-134">notCompliantDeviceCount</span></span>|<span data-ttu-id="4e446-135">Int32</span><span class="sxs-lookup"><span data-stu-id="4e446-135">Int32</span></span>|<span data-ttu-id="4e446-136">不符合的设备计数。</span><span class="sxs-lookup"><span data-stu-id="4e446-136">Not Compliant device count.</span></span>|
|<span data-ttu-id="4e446-137">pendingDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4e446-137">pendingDeviceCount</span></span>|<span data-ttu-id="4e446-138">Int32</span><span class="sxs-lookup"><span data-stu-id="4e446-138">Int32</span></span>|<span data-ttu-id="4e446-139">挂起的设备计数。</span><span class="sxs-lookup"><span data-stu-id="4e446-139">Pending device count.</span></span>|
|<span data-ttu-id="4e446-140">successUserCount</span><span class="sxs-lookup"><span data-stu-id="4e446-140">successUserCount</span></span>|<span data-ttu-id="4e446-141">Int32</span><span class="sxs-lookup"><span data-stu-id="4e446-141">Int32</span></span>|<span data-ttu-id="4e446-142">成功的用户计数。</span><span class="sxs-lookup"><span data-stu-id="4e446-142">Success user count.</span></span>|
|<span data-ttu-id="4e446-143">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="4e446-143">errorUserCount</span></span>|<span data-ttu-id="4e446-144">Int32</span><span class="sxs-lookup"><span data-stu-id="4e446-144">Int32</span></span>|<span data-ttu-id="4e446-145">错误用户计数。</span><span class="sxs-lookup"><span data-stu-id="4e446-145">Error user count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4e446-146">关系</span><span class="sxs-lookup"><span data-stu-id="4e446-146">Relationships</span></span>
<span data-ttu-id="4e446-147">无</span><span class="sxs-lookup"><span data-stu-id="4e446-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4e446-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4e446-148">JSON Representation</span></span>
<span data-ttu-id="4e446-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4e446-149">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementScriptRunSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementScriptRunSummary",
  "id": "String (identifier)",
  "successDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "compliantDeviceCount": 1024,
  "notCompliantDeviceCount": 1024,
  "pendingDeviceCount": 1024,
  "successUserCount": 1024,
  "errorUserCount": 1024
}
```



