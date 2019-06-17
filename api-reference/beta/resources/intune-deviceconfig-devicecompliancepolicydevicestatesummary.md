---
title: deviceCompliancePolicyDeviceStateSummary 资源类型
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6a1343abb5c460dab504e1f56b21b1b0d1185186
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34979450"
---
# <a name="devicecompliancepolicydevicestatesummary-resource-type"></a><span data-ttu-id="27379-103">deviceCompliancePolicyDeviceStateSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="27379-103">deviceCompliancePolicyDeviceStateSummary resource type</span></span>

> <span data-ttu-id="27379-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="27379-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="27379-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="27379-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="27379-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="27379-106">Not yet documented</span></span>

## <a name="methods"></a><span data-ttu-id="27379-107">方法</span><span class="sxs-lookup"><span data-stu-id="27379-107">Methods</span></span>
|<span data-ttu-id="27379-108">方法</span><span class="sxs-lookup"><span data-stu-id="27379-108">Method</span></span>|<span data-ttu-id="27379-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="27379-109">Return Type</span></span>|<span data-ttu-id="27379-110">说明</span><span class="sxs-lookup"><span data-stu-id="27379-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="27379-111">获取 deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="27379-111">Get deviceCompliancePolicyDeviceStateSummary</span></span>](../api/intune-deviceconfig-devicecompliancepolicydevicestatesummary-get.md)|[<span data-ttu-id="27379-112">deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="27379-112">deviceCompliancePolicyDeviceStateSummary</span></span>](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|<span data-ttu-id="27379-113">读取 [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="27379-113">Read properties and relationships of the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>|
|[<span data-ttu-id="27379-114">更新 deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="27379-114">Update deviceCompliancePolicyDeviceStateSummary</span></span>](../api/intune-deviceconfig-devicecompliancepolicydevicestatesummary-update.md)|[<span data-ttu-id="27379-115">deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="27379-115">deviceCompliancePolicyDeviceStateSummary</span></span>](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|<span data-ttu-id="27379-116">更新 [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="27379-116">Update the properties of a [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="27379-117">属性</span><span class="sxs-lookup"><span data-stu-id="27379-117">Properties</span></span>
|<span data-ttu-id="27379-118">属性</span><span class="sxs-lookup"><span data-stu-id="27379-118">Property</span></span>|<span data-ttu-id="27379-119">类型</span><span class="sxs-lookup"><span data-stu-id="27379-119">Type</span></span>|<span data-ttu-id="27379-120">说明</span><span class="sxs-lookup"><span data-stu-id="27379-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27379-121">inGracePeriodCount</span><span class="sxs-lookup"><span data-stu-id="27379-121">inGracePeriodCount</span></span>|<span data-ttu-id="27379-122">Int32</span><span class="sxs-lookup"><span data-stu-id="27379-122">Int32</span></span>|<span data-ttu-id="27379-123">宽限期内的设备数</span><span class="sxs-lookup"><span data-stu-id="27379-123">Number of devices that are in grace period</span></span>|
|<span data-ttu-id="27379-124">configManagerCount</span><span class="sxs-lookup"><span data-stu-id="27379-124">configManagerCount</span></span>|<span data-ttu-id="27379-125">Int32</span><span class="sxs-lookup"><span data-stu-id="27379-125">Int32</span></span>|<span data-ttu-id="27379-126">由 System Center Configuration Manager 管理符合性的设备数</span><span class="sxs-lookup"><span data-stu-id="27379-126">Number of devices that have compliance managed by System Center Configuration Manager</span></span>|
|<span data-ttu-id="27379-127">id</span><span class="sxs-lookup"><span data-stu-id="27379-127">id</span></span>|<span data-ttu-id="27379-128">String</span><span class="sxs-lookup"><span data-stu-id="27379-128">String</span></span>|<span data-ttu-id="27379-129">实体的键。</span><span class="sxs-lookup"><span data-stu-id="27379-129">Key of the entity.</span></span>|
|<span data-ttu-id="27379-130">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="27379-130">unknownDeviceCount</span></span>|<span data-ttu-id="27379-131">Int32</span><span class="sxs-lookup"><span data-stu-id="27379-131">Int32</span></span>|<span data-ttu-id="27379-132">未知设备的数量</span><span class="sxs-lookup"><span data-stu-id="27379-132">Number of unknown devices</span></span>|
|<span data-ttu-id="27379-133">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="27379-133">notApplicableDeviceCount</span></span>|<span data-ttu-id="27379-134">Int32</span><span class="sxs-lookup"><span data-stu-id="27379-134">Int32</span></span>|<span data-ttu-id="27379-135">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="27379-135">Number of not applicable devices</span></span>|
|<span data-ttu-id="27379-136">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="27379-136">compliantDeviceCount</span></span>|<span data-ttu-id="27379-137">Int32</span><span class="sxs-lookup"><span data-stu-id="27379-137">Int32</span></span>|<span data-ttu-id="27379-138">兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="27379-138">Number of compliant devices</span></span>|
|<span data-ttu-id="27379-139">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="27379-139">remediatedDeviceCount</span></span>|<span data-ttu-id="27379-140">Int32</span><span class="sxs-lookup"><span data-stu-id="27379-140">Int32</span></span>|<span data-ttu-id="27379-141">已修复设备的数量</span><span class="sxs-lookup"><span data-stu-id="27379-141">Number of remediated devices</span></span>|
|<span data-ttu-id="27379-142">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="27379-142">nonCompliantDeviceCount</span></span>|<span data-ttu-id="27379-143">Int32</span><span class="sxs-lookup"><span data-stu-id="27379-143">Int32</span></span>|<span data-ttu-id="27379-144">不兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="27379-144">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="27379-145">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="27379-145">errorDeviceCount</span></span>|<span data-ttu-id="27379-146">Int32</span><span class="sxs-lookup"><span data-stu-id="27379-146">Int32</span></span>|<span data-ttu-id="27379-147">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="27379-147">Number of error devices</span></span>|
|<span data-ttu-id="27379-148">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="27379-148">conflictDeviceCount</span></span>|<span data-ttu-id="27379-149">Int32</span><span class="sxs-lookup"><span data-stu-id="27379-149">Int32</span></span>|<span data-ttu-id="27379-150">冲突设备的数量</span><span class="sxs-lookup"><span data-stu-id="27379-150">Number of conflict devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="27379-151">关系</span><span class="sxs-lookup"><span data-stu-id="27379-151">Relationships</span></span>
<span data-ttu-id="27379-152">无</span><span class="sxs-lookup"><span data-stu-id="27379-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="27379-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="27379-153">JSON Representation</span></span>
<span data-ttu-id="27379-154">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="27379-154">Here is a JSON representation of the resource.</span></span>
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





