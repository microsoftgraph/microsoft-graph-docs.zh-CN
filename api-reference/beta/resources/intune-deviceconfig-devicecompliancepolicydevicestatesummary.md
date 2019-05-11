---
title: deviceCompliancePolicyDeviceStateSummary 资源类型
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6643fbcb7abe0dab5c7a72b8f78e7e7282aee4b6
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33947132"
---
# <a name="devicecompliancepolicydevicestatesummary-resource-type"></a><span data-ttu-id="e6484-103">deviceCompliancePolicyDeviceStateSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="e6484-103">deviceCompliancePolicyDeviceStateSummary resource type</span></span>

> <span data-ttu-id="e6484-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e6484-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e6484-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e6484-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e6484-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e6484-106">Not yet documented</span></span>

## <a name="methods"></a><span data-ttu-id="e6484-107">方法</span><span class="sxs-lookup"><span data-stu-id="e6484-107">Methods</span></span>
|<span data-ttu-id="e6484-108">方法</span><span class="sxs-lookup"><span data-stu-id="e6484-108">Method</span></span>|<span data-ttu-id="e6484-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="e6484-109">Return Type</span></span>|<span data-ttu-id="e6484-110">说明</span><span class="sxs-lookup"><span data-stu-id="e6484-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e6484-111">获取 deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="e6484-111">Get deviceCompliancePolicyDeviceStateSummary</span></span>](../api/intune-deviceconfig-devicecompliancepolicydevicestatesummary-get.md)|[<span data-ttu-id="e6484-112">deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="e6484-112">deviceCompliancePolicyDeviceStateSummary</span></span>](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|<span data-ttu-id="e6484-113">读取 [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e6484-113">Read properties and relationships of the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>|
|[<span data-ttu-id="e6484-114">更新 deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="e6484-114">Update deviceCompliancePolicyDeviceStateSummary</span></span>](../api/intune-deviceconfig-devicecompliancepolicydevicestatesummary-update.md)|[<span data-ttu-id="e6484-115">deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="e6484-115">deviceCompliancePolicyDeviceStateSummary</span></span>](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|<span data-ttu-id="e6484-116">更新 [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e6484-116">Update the properties of a [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e6484-117">属性</span><span class="sxs-lookup"><span data-stu-id="e6484-117">Properties</span></span>
|<span data-ttu-id="e6484-118">属性</span><span class="sxs-lookup"><span data-stu-id="e6484-118">Property</span></span>|<span data-ttu-id="e6484-119">类型</span><span class="sxs-lookup"><span data-stu-id="e6484-119">Type</span></span>|<span data-ttu-id="e6484-120">说明</span><span class="sxs-lookup"><span data-stu-id="e6484-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6484-121">inGracePeriodCount</span><span class="sxs-lookup"><span data-stu-id="e6484-121">inGracePeriodCount</span></span>|<span data-ttu-id="e6484-122">Int32</span><span class="sxs-lookup"><span data-stu-id="e6484-122">Int32</span></span>|<span data-ttu-id="e6484-123">宽限期内的设备数</span><span class="sxs-lookup"><span data-stu-id="e6484-123">Number of devices that are in grace period</span></span>|
|<span data-ttu-id="e6484-124">configManagerCount</span><span class="sxs-lookup"><span data-stu-id="e6484-124">configManagerCount</span></span>|<span data-ttu-id="e6484-125">Int32</span><span class="sxs-lookup"><span data-stu-id="e6484-125">Int32</span></span>|<span data-ttu-id="e6484-126">由 System Center Configuration Manager 管理符合性的设备数</span><span class="sxs-lookup"><span data-stu-id="e6484-126">Number of devices that have compliance managed by System Center Configuration Manager</span></span>|
|<span data-ttu-id="e6484-127">id</span><span class="sxs-lookup"><span data-stu-id="e6484-127">id</span></span>|<span data-ttu-id="e6484-128">String</span><span class="sxs-lookup"><span data-stu-id="e6484-128">String</span></span>|<span data-ttu-id="e6484-129">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e6484-129">Key of the entity.</span></span>|
|<span data-ttu-id="e6484-130">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e6484-130">unknownDeviceCount</span></span>|<span data-ttu-id="e6484-131">Int32</span><span class="sxs-lookup"><span data-stu-id="e6484-131">Int32</span></span>|<span data-ttu-id="e6484-132">未知设备的数量</span><span class="sxs-lookup"><span data-stu-id="e6484-132">Number of unknown devices</span></span>|
|<span data-ttu-id="e6484-133">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e6484-133">notApplicableDeviceCount</span></span>|<span data-ttu-id="e6484-134">Int32</span><span class="sxs-lookup"><span data-stu-id="e6484-134">Int32</span></span>|<span data-ttu-id="e6484-135">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="e6484-135">Number of not applicable devices</span></span>|
|<span data-ttu-id="e6484-136">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e6484-136">compliantDeviceCount</span></span>|<span data-ttu-id="e6484-137">Int32</span><span class="sxs-lookup"><span data-stu-id="e6484-137">Int32</span></span>|<span data-ttu-id="e6484-138">兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="e6484-138">Number of compliant devices</span></span>|
|<span data-ttu-id="e6484-139">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e6484-139">remediatedDeviceCount</span></span>|<span data-ttu-id="e6484-140">Int32</span><span class="sxs-lookup"><span data-stu-id="e6484-140">Int32</span></span>|<span data-ttu-id="e6484-141">已修复设备的数量</span><span class="sxs-lookup"><span data-stu-id="e6484-141">Number of remediated devices</span></span>|
|<span data-ttu-id="e6484-142">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e6484-142">nonCompliantDeviceCount</span></span>|<span data-ttu-id="e6484-143">Int32</span><span class="sxs-lookup"><span data-stu-id="e6484-143">Int32</span></span>|<span data-ttu-id="e6484-144">不兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="e6484-144">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="e6484-145">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e6484-145">errorDeviceCount</span></span>|<span data-ttu-id="e6484-146">Int32</span><span class="sxs-lookup"><span data-stu-id="e6484-146">Int32</span></span>|<span data-ttu-id="e6484-147">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="e6484-147">Number of error devices</span></span>|
|<span data-ttu-id="e6484-148">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e6484-148">conflictDeviceCount</span></span>|<span data-ttu-id="e6484-149">Int32</span><span class="sxs-lookup"><span data-stu-id="e6484-149">Int32</span></span>|<span data-ttu-id="e6484-150">冲突设备的数量</span><span class="sxs-lookup"><span data-stu-id="e6484-150">Number of conflict devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="e6484-151">关系</span><span class="sxs-lookup"><span data-stu-id="e6484-151">Relationships</span></span>
<span data-ttu-id="e6484-152">无</span><span class="sxs-lookup"><span data-stu-id="e6484-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e6484-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e6484-153">JSON Representation</span></span>
<span data-ttu-id="e6484-154">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e6484-154">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCompliancePolicyDeviceStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyDeviceStateSummary",
  "inGracePeriodCount": 1024,
  "configManagerCount": 1024,
  "id": "String (identifier)",
  "unknownDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "compliantDeviceCount": 1024,
  "remediatedDeviceCount": 1024,
  "nonCompliantDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "conflictDeviceCount": 1024
}
```




