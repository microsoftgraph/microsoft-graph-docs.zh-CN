---
title: deviceCompliancePolicyDeviceStateSummary 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3f1234fba81943d984758cd96a6b9f54480e813b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031743"
---
# <a name="devicecompliancepolicydevicestatesummary-resource-type"></a><span data-ttu-id="03e06-103">deviceCompliancePolicyDeviceStateSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="03e06-103">deviceCompliancePolicyDeviceStateSummary resource type</span></span>

> <span data-ttu-id="03e06-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="03e06-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="03e06-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="03e06-105">Not yet documented</span></span>

## <a name="methods"></a><span data-ttu-id="03e06-106">方法</span><span class="sxs-lookup"><span data-stu-id="03e06-106">Methods</span></span>
|<span data-ttu-id="03e06-107">方法</span><span class="sxs-lookup"><span data-stu-id="03e06-107">Method</span></span>|<span data-ttu-id="03e06-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="03e06-108">Return Type</span></span>|<span data-ttu-id="03e06-109">说明</span><span class="sxs-lookup"><span data-stu-id="03e06-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="03e06-110">获取 deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="03e06-110">Get deviceCompliancePolicyDeviceStateSummary</span></span>](../api/intune-deviceconfig-devicecompliancepolicydevicestatesummary-get.md)|[<span data-ttu-id="03e06-111">deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="03e06-111">deviceCompliancePolicyDeviceStateSummary</span></span>](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|<span data-ttu-id="03e06-112">读取 [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="03e06-112">Read properties and relationships of the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>|
|[<span data-ttu-id="03e06-113">更新 deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="03e06-113">Update deviceCompliancePolicyDeviceStateSummary</span></span>](../api/intune-deviceconfig-devicecompliancepolicydevicestatesummary-update.md)|[<span data-ttu-id="03e06-114">deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="03e06-114">deviceCompliancePolicyDeviceStateSummary</span></span>](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|<span data-ttu-id="03e06-115">更新 [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="03e06-115">Update the properties of a [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="03e06-116">属性</span><span class="sxs-lookup"><span data-stu-id="03e06-116">Properties</span></span>
|<span data-ttu-id="03e06-117">属性</span><span class="sxs-lookup"><span data-stu-id="03e06-117">Property</span></span>|<span data-ttu-id="03e06-118">类型</span><span class="sxs-lookup"><span data-stu-id="03e06-118">Type</span></span>|<span data-ttu-id="03e06-119">说明</span><span class="sxs-lookup"><span data-stu-id="03e06-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03e06-120">inGracePeriodCount</span><span class="sxs-lookup"><span data-stu-id="03e06-120">inGracePeriodCount</span></span>|<span data-ttu-id="03e06-121">Int32</span><span class="sxs-lookup"><span data-stu-id="03e06-121">Int32</span></span>|<span data-ttu-id="03e06-122">宽限期内的设备数</span><span class="sxs-lookup"><span data-stu-id="03e06-122">Number of devices that are in grace period</span></span>|
|<span data-ttu-id="03e06-123">configManagerCount</span><span class="sxs-lookup"><span data-stu-id="03e06-123">configManagerCount</span></span>|<span data-ttu-id="03e06-124">Int32</span><span class="sxs-lookup"><span data-stu-id="03e06-124">Int32</span></span>|<span data-ttu-id="03e06-125">由 System Center Configuration Manager 管理符合性的设备数</span><span class="sxs-lookup"><span data-stu-id="03e06-125">Number of devices that have compliance managed by System Center Configuration Manager</span></span>|
|<span data-ttu-id="03e06-126">id</span><span class="sxs-lookup"><span data-stu-id="03e06-126">id</span></span>|<span data-ttu-id="03e06-127">String</span><span class="sxs-lookup"><span data-stu-id="03e06-127">String</span></span>|<span data-ttu-id="03e06-128">实体的键。</span><span class="sxs-lookup"><span data-stu-id="03e06-128">Key of the entity.</span></span>|
|<span data-ttu-id="03e06-129">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="03e06-129">unknownDeviceCount</span></span>|<span data-ttu-id="03e06-130">Int32</span><span class="sxs-lookup"><span data-stu-id="03e06-130">Int32</span></span>|<span data-ttu-id="03e06-131">未知设备的数量</span><span class="sxs-lookup"><span data-stu-id="03e06-131">Number of unknown devices</span></span>|
|<span data-ttu-id="03e06-132">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="03e06-132">notApplicableDeviceCount</span></span>|<span data-ttu-id="03e06-133">Int32</span><span class="sxs-lookup"><span data-stu-id="03e06-133">Int32</span></span>|<span data-ttu-id="03e06-134">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="03e06-134">Number of not applicable devices</span></span>|
|<span data-ttu-id="03e06-135">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="03e06-135">compliantDeviceCount</span></span>|<span data-ttu-id="03e06-136">Int32</span><span class="sxs-lookup"><span data-stu-id="03e06-136">Int32</span></span>|<span data-ttu-id="03e06-137">兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="03e06-137">Number of compliant devices</span></span>|
|<span data-ttu-id="03e06-138">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="03e06-138">remediatedDeviceCount</span></span>|<span data-ttu-id="03e06-139">Int32</span><span class="sxs-lookup"><span data-stu-id="03e06-139">Int32</span></span>|<span data-ttu-id="03e06-140">已修复设备的数量</span><span class="sxs-lookup"><span data-stu-id="03e06-140">Number of remediated devices</span></span>|
|<span data-ttu-id="03e06-141">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="03e06-141">nonCompliantDeviceCount</span></span>|<span data-ttu-id="03e06-142">Int32</span><span class="sxs-lookup"><span data-stu-id="03e06-142">Int32</span></span>|<span data-ttu-id="03e06-143">不兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="03e06-143">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="03e06-144">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="03e06-144">errorDeviceCount</span></span>|<span data-ttu-id="03e06-145">Int32</span><span class="sxs-lookup"><span data-stu-id="03e06-145">Int32</span></span>|<span data-ttu-id="03e06-146">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="03e06-146">Number of error devices</span></span>|
|<span data-ttu-id="03e06-147">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="03e06-147">conflictDeviceCount</span></span>|<span data-ttu-id="03e06-148">Int32</span><span class="sxs-lookup"><span data-stu-id="03e06-148">Int32</span></span>|<span data-ttu-id="03e06-149">冲突设备的数量</span><span class="sxs-lookup"><span data-stu-id="03e06-149">Number of conflict devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="03e06-150">关系</span><span class="sxs-lookup"><span data-stu-id="03e06-150">Relationships</span></span>
<span data-ttu-id="03e06-151">无</span><span class="sxs-lookup"><span data-stu-id="03e06-151">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="03e06-152">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="03e06-152">JSON Representation</span></span>
<span data-ttu-id="03e06-153">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="03e06-153">Here is a JSON representation of the resource.</span></span>
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



