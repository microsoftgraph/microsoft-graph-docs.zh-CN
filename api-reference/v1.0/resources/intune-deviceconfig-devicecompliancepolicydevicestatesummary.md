---
title: deviceCompliancePolicyDeviceStateSummary 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 01aaeb851a8a7be9f07e49c140e151f438bb9978
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47967609"
---
# <a name="devicecompliancepolicydevicestatesummary-resource-type"></a><span data-ttu-id="e26ea-103">deviceCompliancePolicyDeviceStateSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="e26ea-103">deviceCompliancePolicyDeviceStateSummary resource type</span></span>

<span data-ttu-id="e26ea-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e26ea-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e26ea-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e26ea-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e26ea-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e26ea-106">Not yet documented</span></span>

## <a name="methods"></a><span data-ttu-id="e26ea-107">方法</span><span class="sxs-lookup"><span data-stu-id="e26ea-107">Methods</span></span>
|<span data-ttu-id="e26ea-108">方法</span><span class="sxs-lookup"><span data-stu-id="e26ea-108">Method</span></span>|<span data-ttu-id="e26ea-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="e26ea-109">Return Type</span></span>|<span data-ttu-id="e26ea-110">说明</span><span class="sxs-lookup"><span data-stu-id="e26ea-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e26ea-111">获取 deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="e26ea-111">Get deviceCompliancePolicyDeviceStateSummary</span></span>](../api/intune-deviceconfig-devicecompliancepolicydevicestatesummary-get.md)|[<span data-ttu-id="e26ea-112">deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="e26ea-112">deviceCompliancePolicyDeviceStateSummary</span></span>](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|<span data-ttu-id="e26ea-113">读取 [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e26ea-113">Read properties and relationships of the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>|
|[<span data-ttu-id="e26ea-114">更新 deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="e26ea-114">Update deviceCompliancePolicyDeviceStateSummary</span></span>](../api/intune-deviceconfig-devicecompliancepolicydevicestatesummary-update.md)|[<span data-ttu-id="e26ea-115">deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="e26ea-115">deviceCompliancePolicyDeviceStateSummary</span></span>](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|<span data-ttu-id="e26ea-116">更新 [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e26ea-116">Update the properties of a [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e26ea-117">属性</span><span class="sxs-lookup"><span data-stu-id="e26ea-117">Properties</span></span>
|<span data-ttu-id="e26ea-118">属性</span><span class="sxs-lookup"><span data-stu-id="e26ea-118">Property</span></span>|<span data-ttu-id="e26ea-119">类型</span><span class="sxs-lookup"><span data-stu-id="e26ea-119">Type</span></span>|<span data-ttu-id="e26ea-120">说明</span><span class="sxs-lookup"><span data-stu-id="e26ea-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e26ea-121">inGracePeriodCount</span><span class="sxs-lookup"><span data-stu-id="e26ea-121">inGracePeriodCount</span></span>|<span data-ttu-id="e26ea-122">Int32</span><span class="sxs-lookup"><span data-stu-id="e26ea-122">Int32</span></span>|<span data-ttu-id="e26ea-123">宽限期内的设备数</span><span class="sxs-lookup"><span data-stu-id="e26ea-123">Number of devices that are in grace period</span></span>|
|<span data-ttu-id="e26ea-124">configManagerCount</span><span class="sxs-lookup"><span data-stu-id="e26ea-124">configManagerCount</span></span>|<span data-ttu-id="e26ea-125">Int32</span><span class="sxs-lookup"><span data-stu-id="e26ea-125">Int32</span></span>|<span data-ttu-id="e26ea-126">由 System Center Configuration Manager 管理符合性的设备数</span><span class="sxs-lookup"><span data-stu-id="e26ea-126">Number of devices that have compliance managed by System Center Configuration Manager</span></span>|
|<span data-ttu-id="e26ea-127">id</span><span class="sxs-lookup"><span data-stu-id="e26ea-127">id</span></span>|<span data-ttu-id="e26ea-128">String</span><span class="sxs-lookup"><span data-stu-id="e26ea-128">String</span></span>|<span data-ttu-id="e26ea-129">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e26ea-129">Key of the entity.</span></span>|
|<span data-ttu-id="e26ea-130">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e26ea-130">unknownDeviceCount</span></span>|<span data-ttu-id="e26ea-131">Int32</span><span class="sxs-lookup"><span data-stu-id="e26ea-131">Int32</span></span>|<span data-ttu-id="e26ea-132">未知设备的数量</span><span class="sxs-lookup"><span data-stu-id="e26ea-132">Number of unknown devices</span></span>|
|<span data-ttu-id="e26ea-133">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e26ea-133">notApplicableDeviceCount</span></span>|<span data-ttu-id="e26ea-134">Int32</span><span class="sxs-lookup"><span data-stu-id="e26ea-134">Int32</span></span>|<span data-ttu-id="e26ea-135">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="e26ea-135">Number of not applicable devices</span></span>|
|<span data-ttu-id="e26ea-136">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e26ea-136">compliantDeviceCount</span></span>|<span data-ttu-id="e26ea-137">Int32</span><span class="sxs-lookup"><span data-stu-id="e26ea-137">Int32</span></span>|<span data-ttu-id="e26ea-138">兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="e26ea-138">Number of compliant devices</span></span>|
|<span data-ttu-id="e26ea-139">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e26ea-139">remediatedDeviceCount</span></span>|<span data-ttu-id="e26ea-140">Int32</span><span class="sxs-lookup"><span data-stu-id="e26ea-140">Int32</span></span>|<span data-ttu-id="e26ea-141">已修复设备的数量</span><span class="sxs-lookup"><span data-stu-id="e26ea-141">Number of remediated devices</span></span>|
|<span data-ttu-id="e26ea-142">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e26ea-142">nonCompliantDeviceCount</span></span>|<span data-ttu-id="e26ea-143">Int32</span><span class="sxs-lookup"><span data-stu-id="e26ea-143">Int32</span></span>|<span data-ttu-id="e26ea-144">不兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="e26ea-144">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="e26ea-145">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e26ea-145">errorDeviceCount</span></span>|<span data-ttu-id="e26ea-146">Int32</span><span class="sxs-lookup"><span data-stu-id="e26ea-146">Int32</span></span>|<span data-ttu-id="e26ea-147">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="e26ea-147">Number of error devices</span></span>|
|<span data-ttu-id="e26ea-148">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e26ea-148">conflictDeviceCount</span></span>|<span data-ttu-id="e26ea-149">Int32</span><span class="sxs-lookup"><span data-stu-id="e26ea-149">Int32</span></span>|<span data-ttu-id="e26ea-150">冲突设备的数量</span><span class="sxs-lookup"><span data-stu-id="e26ea-150">Number of conflict devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="e26ea-151">关系</span><span class="sxs-lookup"><span data-stu-id="e26ea-151">Relationships</span></span>
<span data-ttu-id="e26ea-152">无</span><span class="sxs-lookup"><span data-stu-id="e26ea-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e26ea-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e26ea-153">JSON Representation</span></span>
<span data-ttu-id="e26ea-154">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e26ea-154">Here is a JSON representation of the resource.</span></span>
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









