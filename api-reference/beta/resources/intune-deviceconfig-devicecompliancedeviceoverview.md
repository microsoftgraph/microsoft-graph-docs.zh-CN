---
title: deviceComplianceDeviceOverview 资源类型
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 40ab1aba74e316a0fd0a156eac176a0fcddcc6f3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35970631"
---
# <a name="devicecompliancedeviceoverview-resource-type"></a><span data-ttu-id="fc991-103">deviceComplianceDeviceOverview 资源类型</span><span class="sxs-lookup"><span data-stu-id="fc991-103">deviceComplianceDeviceOverview resource type</span></span>

> <span data-ttu-id="fc991-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fc991-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fc991-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fc991-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc991-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="fc991-106">Not yet documented</span></span>

## <a name="methods"></a><span data-ttu-id="fc991-107">方法</span><span class="sxs-lookup"><span data-stu-id="fc991-107">Methods</span></span>
|<span data-ttu-id="fc991-108">方法</span><span class="sxs-lookup"><span data-stu-id="fc991-108">Method</span></span>|<span data-ttu-id="fc991-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="fc991-109">Return Type</span></span>|<span data-ttu-id="fc991-110">说明</span><span class="sxs-lookup"><span data-stu-id="fc991-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="fc991-111">获取 deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="fc991-111">Get deviceComplianceDeviceOverview</span></span>](../api/intune-deviceconfig-devicecompliancedeviceoverview-get.md)|[<span data-ttu-id="fc991-112">deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="fc991-112">deviceComplianceDeviceOverview</span></span>](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md)|<span data-ttu-id="fc991-113">读取 [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="fc991-113">Read properties and relationships of the [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="fc991-114">更新 deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="fc991-114">Update deviceComplianceDeviceOverview</span></span>](../api/intune-deviceconfig-devicecompliancedeviceoverview-update.md)|[<span data-ttu-id="fc991-115">deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="fc991-115">deviceComplianceDeviceOverview</span></span>](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md)|<span data-ttu-id="fc991-116">更新 [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="fc991-116">Update the properties of a [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="fc991-117">属性</span><span class="sxs-lookup"><span data-stu-id="fc991-117">Properties</span></span>
|<span data-ttu-id="fc991-118">属性</span><span class="sxs-lookup"><span data-stu-id="fc991-118">Property</span></span>|<span data-ttu-id="fc991-119">类型</span><span class="sxs-lookup"><span data-stu-id="fc991-119">Type</span></span>|<span data-ttu-id="fc991-120">说明</span><span class="sxs-lookup"><span data-stu-id="fc991-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc991-121">id</span><span class="sxs-lookup"><span data-stu-id="fc991-121">id</span></span>|<span data-ttu-id="fc991-122">String</span><span class="sxs-lookup"><span data-stu-id="fc991-122">String</span></span>|<span data-ttu-id="fc991-123">实体的键。</span><span class="sxs-lookup"><span data-stu-id="fc991-123">Key of the entity.</span></span>|
|<span data-ttu-id="fc991-124">pendingCount</span><span class="sxs-lookup"><span data-stu-id="fc991-124">pendingCount</span></span>|<span data-ttu-id="fc991-125">Int32</span><span class="sxs-lookup"><span data-stu-id="fc991-125">Int32</span></span>|<span data-ttu-id="fc991-126">挂起设备的数量</span><span class="sxs-lookup"><span data-stu-id="fc991-126">Number of pending devices</span></span>|
|<span data-ttu-id="fc991-127">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="fc991-127">notApplicableCount</span></span>|<span data-ttu-id="fc991-128">Int32</span><span class="sxs-lookup"><span data-stu-id="fc991-128">Int32</span></span>|<span data-ttu-id="fc991-129">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="fc991-129">Number of not applicable devices</span></span>|
|<span data-ttu-id="fc991-130">notApplicablePlatformCount</span><span class="sxs-lookup"><span data-stu-id="fc991-130">notApplicablePlatformCount</span></span>|<span data-ttu-id="fc991-131">Int32</span><span class="sxs-lookup"><span data-stu-id="fc991-131">Int32</span></span>|<span data-ttu-id="fc991-132">由于平台和策略不匹配而导致不适用的设备数量</span><span class="sxs-lookup"><span data-stu-id="fc991-132">Number of not applicable devices due to mismatch platform and policy</span></span>|
|<span data-ttu-id="fc991-133">successCount</span><span class="sxs-lookup"><span data-stu-id="fc991-133">successCount</span></span>|<span data-ttu-id="fc991-134">Int32</span><span class="sxs-lookup"><span data-stu-id="fc991-134">Int32</span></span>|<span data-ttu-id="fc991-135">成功设备的数量</span><span class="sxs-lookup"><span data-stu-id="fc991-135">Number of succeeded devices</span></span>|
|<span data-ttu-id="fc991-136">errorCount</span><span class="sxs-lookup"><span data-stu-id="fc991-136">errorCount</span></span>|<span data-ttu-id="fc991-137">Int32</span><span class="sxs-lookup"><span data-stu-id="fc991-137">Int32</span></span>|<span data-ttu-id="fc991-138">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="fc991-138">Number of error devices</span></span>|
|<span data-ttu-id="fc991-139">failedCount</span><span class="sxs-lookup"><span data-stu-id="fc991-139">failedCount</span></span>|<span data-ttu-id="fc991-140">Int32</span><span class="sxs-lookup"><span data-stu-id="fc991-140">Int32</span></span>|<span data-ttu-id="fc991-141">失败设备的数量</span><span class="sxs-lookup"><span data-stu-id="fc991-141">Number of failed devices</span></span>|
|<span data-ttu-id="fc991-142">conflictCount</span><span class="sxs-lookup"><span data-stu-id="fc991-142">conflictCount</span></span>|<span data-ttu-id="fc991-143">Int32</span><span class="sxs-lookup"><span data-stu-id="fc991-143">Int32</span></span>|<span data-ttu-id="fc991-144">发生冲突的设备数</span><span class="sxs-lookup"><span data-stu-id="fc991-144">Number of devices in conflict</span></span>|
|<span data-ttu-id="fc991-145">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="fc991-145">lastUpdateDateTime</span></span>|<span data-ttu-id="fc991-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fc991-146">DateTimeOffset</span></span>|<span data-ttu-id="fc991-147">上次更新时间</span><span class="sxs-lookup"><span data-stu-id="fc991-147">Last update time</span></span>|
|<span data-ttu-id="fc991-148">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="fc991-148">configurationVersion</span></span>|<span data-ttu-id="fc991-149">Int32</span><span class="sxs-lookup"><span data-stu-id="fc991-149">Int32</span></span>|<span data-ttu-id="fc991-150">用于此概述的策略版本</span><span class="sxs-lookup"><span data-stu-id="fc991-150">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="fc991-151">关系</span><span class="sxs-lookup"><span data-stu-id="fc991-151">Relationships</span></span>
<span data-ttu-id="fc991-152">无</span><span class="sxs-lookup"><span data-stu-id="fc991-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fc991-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fc991-153">JSON Representation</span></span>
<span data-ttu-id="fc991-154">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fc991-154">Here is a JSON representation of the resource.</span></span>
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





