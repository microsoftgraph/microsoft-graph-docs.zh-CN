---
title: deviceComplianceDeviceOverview 资源类型
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5466b179e98bc4aed6d8d4bdf366db6d9cb0e656
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34979492"
---
# <a name="devicecompliancedeviceoverview-resource-type"></a><span data-ttu-id="438f9-103">deviceComplianceDeviceOverview 资源类型</span><span class="sxs-lookup"><span data-stu-id="438f9-103">deviceComplianceDeviceOverview resource type</span></span>

> <span data-ttu-id="438f9-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="438f9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="438f9-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="438f9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="438f9-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="438f9-106">Not yet documented</span></span>

## <a name="methods"></a><span data-ttu-id="438f9-107">方法</span><span class="sxs-lookup"><span data-stu-id="438f9-107">Methods</span></span>
|<span data-ttu-id="438f9-108">方法</span><span class="sxs-lookup"><span data-stu-id="438f9-108">Method</span></span>|<span data-ttu-id="438f9-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="438f9-109">Return Type</span></span>|<span data-ttu-id="438f9-110">说明</span><span class="sxs-lookup"><span data-stu-id="438f9-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="438f9-111">获取 deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="438f9-111">Get deviceComplianceDeviceOverview</span></span>](../api/intune-deviceconfig-devicecompliancedeviceoverview-get.md)|[<span data-ttu-id="438f9-112">deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="438f9-112">deviceComplianceDeviceOverview</span></span>](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md)|<span data-ttu-id="438f9-113">读取 [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="438f9-113">Read properties and relationships of the [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="438f9-114">更新 deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="438f9-114">Update deviceComplianceDeviceOverview</span></span>](../api/intune-deviceconfig-devicecompliancedeviceoverview-update.md)|[<span data-ttu-id="438f9-115">deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="438f9-115">deviceComplianceDeviceOverview</span></span>](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md)|<span data-ttu-id="438f9-116">更新 [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="438f9-116">Update the properties of a [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="438f9-117">属性</span><span class="sxs-lookup"><span data-stu-id="438f9-117">Properties</span></span>
|<span data-ttu-id="438f9-118">属性</span><span class="sxs-lookup"><span data-stu-id="438f9-118">Property</span></span>|<span data-ttu-id="438f9-119">类型</span><span class="sxs-lookup"><span data-stu-id="438f9-119">Type</span></span>|<span data-ttu-id="438f9-120">说明</span><span class="sxs-lookup"><span data-stu-id="438f9-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="438f9-121">id</span><span class="sxs-lookup"><span data-stu-id="438f9-121">id</span></span>|<span data-ttu-id="438f9-122">String</span><span class="sxs-lookup"><span data-stu-id="438f9-122">String</span></span>|<span data-ttu-id="438f9-123">实体的键。</span><span class="sxs-lookup"><span data-stu-id="438f9-123">Key of the entity.</span></span>|
|<span data-ttu-id="438f9-124">pendingCount</span><span class="sxs-lookup"><span data-stu-id="438f9-124">pendingCount</span></span>|<span data-ttu-id="438f9-125">Int32</span><span class="sxs-lookup"><span data-stu-id="438f9-125">Int32</span></span>|<span data-ttu-id="438f9-126">挂起设备的数量</span><span class="sxs-lookup"><span data-stu-id="438f9-126">Number of pending devices</span></span>|
|<span data-ttu-id="438f9-127">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="438f9-127">notApplicableCount</span></span>|<span data-ttu-id="438f9-128">Int32</span><span class="sxs-lookup"><span data-stu-id="438f9-128">Int32</span></span>|<span data-ttu-id="438f9-129">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="438f9-129">Number of not applicable devices</span></span>|
|<span data-ttu-id="438f9-130">notApplicablePlatformCount</span><span class="sxs-lookup"><span data-stu-id="438f9-130">notApplicablePlatformCount</span></span>|<span data-ttu-id="438f9-131">Int32</span><span class="sxs-lookup"><span data-stu-id="438f9-131">Int32</span></span>|<span data-ttu-id="438f9-132">由于平台和策略不匹配而导致不适用的设备数量</span><span class="sxs-lookup"><span data-stu-id="438f9-132">Number of not applicable devices due to mismatch platform and policy</span></span>|
|<span data-ttu-id="438f9-133">successCount</span><span class="sxs-lookup"><span data-stu-id="438f9-133">successCount</span></span>|<span data-ttu-id="438f9-134">Int32</span><span class="sxs-lookup"><span data-stu-id="438f9-134">Int32</span></span>|<span data-ttu-id="438f9-135">成功设备的数量</span><span class="sxs-lookup"><span data-stu-id="438f9-135">Number of succeeded devices</span></span>|
|<span data-ttu-id="438f9-136">errorCount</span><span class="sxs-lookup"><span data-stu-id="438f9-136">errorCount</span></span>|<span data-ttu-id="438f9-137">Int32</span><span class="sxs-lookup"><span data-stu-id="438f9-137">Int32</span></span>|<span data-ttu-id="438f9-138">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="438f9-138">Number of error devices</span></span>|
|<span data-ttu-id="438f9-139">failedCount</span><span class="sxs-lookup"><span data-stu-id="438f9-139">failedCount</span></span>|<span data-ttu-id="438f9-140">Int32</span><span class="sxs-lookup"><span data-stu-id="438f9-140">Int32</span></span>|<span data-ttu-id="438f9-141">失败设备的数量</span><span class="sxs-lookup"><span data-stu-id="438f9-141">Number of failed devices</span></span>|
|<span data-ttu-id="438f9-142">conflictCount</span><span class="sxs-lookup"><span data-stu-id="438f9-142">conflictCount</span></span>|<span data-ttu-id="438f9-143">Int32</span><span class="sxs-lookup"><span data-stu-id="438f9-143">Int32</span></span>|<span data-ttu-id="438f9-144">发生冲突的设备数</span><span class="sxs-lookup"><span data-stu-id="438f9-144">Number of devices in conflict</span></span>|
|<span data-ttu-id="438f9-145">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="438f9-145">lastUpdateDateTime</span></span>|<span data-ttu-id="438f9-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="438f9-146">DateTimeOffset</span></span>|<span data-ttu-id="438f9-147">上次更新时间</span><span class="sxs-lookup"><span data-stu-id="438f9-147">Last update time</span></span>|
|<span data-ttu-id="438f9-148">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="438f9-148">configurationVersion</span></span>|<span data-ttu-id="438f9-149">Int32</span><span class="sxs-lookup"><span data-stu-id="438f9-149">Int32</span></span>|<span data-ttu-id="438f9-150">用于此概述的策略版本</span><span class="sxs-lookup"><span data-stu-id="438f9-150">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="438f9-151">关系</span><span class="sxs-lookup"><span data-stu-id="438f9-151">Relationships</span></span>
<span data-ttu-id="438f9-152">无</span><span class="sxs-lookup"><span data-stu-id="438f9-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="438f9-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="438f9-153">JSON Representation</span></span>
<span data-ttu-id="438f9-154">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="438f9-154">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceDeviceOverview"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceOverview",
  "id": "String (identifier)",
  "pendingCount": 1024,
  "notApplicableCount": 1024,
  "notApplicablePlatformCount": 1024,
  "successCount": 1024,
  "errorCount": 1024,
  "failedCount": 1024,
  "conflictCount": 1024,
  "lastUpdateDateTime": "String (timestamp)",
  "configurationVersion": 1024
}
```





