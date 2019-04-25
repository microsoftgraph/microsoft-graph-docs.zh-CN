---
title: deviceCompliancePolicyDeviceStateSummary 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1c434009d1f34014a36e6871963051773aa2aab5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32572442"
---
# <a name="devicecompliancepolicydevicestatesummary-resource-type"></a><span data-ttu-id="14e72-103">deviceCompliancePolicyDeviceStateSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="14e72-103">deviceCompliancePolicyDeviceStateSummary resource type</span></span>

> <span data-ttu-id="14e72-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="14e72-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="14e72-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="14e72-105">Not yet documented</span></span>

## <a name="methods"></a><span data-ttu-id="14e72-106">方法</span><span class="sxs-lookup"><span data-stu-id="14e72-106">Methods</span></span>
|<span data-ttu-id="14e72-107">方法</span><span class="sxs-lookup"><span data-stu-id="14e72-107">Method</span></span>|<span data-ttu-id="14e72-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="14e72-108">Return Type</span></span>|<span data-ttu-id="14e72-109">说明</span><span class="sxs-lookup"><span data-stu-id="14e72-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="14e72-110">获取 deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="14e72-110">Get deviceCompliancePolicyDeviceStateSummary</span></span>](../api/intune-deviceconfig-devicecompliancepolicydevicestatesummary-get.md)|[<span data-ttu-id="14e72-111">deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="14e72-111">deviceCompliancePolicyDeviceStateSummary</span></span>](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|<span data-ttu-id="14e72-112">读取 [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="14e72-112">Read properties and relationships of the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>|
|[<span data-ttu-id="14e72-113">更新 deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="14e72-113">Update deviceCompliancePolicyDeviceStateSummary</span></span>](../api/intune-deviceconfig-devicecompliancepolicydevicestatesummary-update.md)|[<span data-ttu-id="14e72-114">deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="14e72-114">deviceCompliancePolicyDeviceStateSummary</span></span>](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|<span data-ttu-id="14e72-115">更新 [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="14e72-115">Update the properties of a [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="14e72-116">属性</span><span class="sxs-lookup"><span data-stu-id="14e72-116">Properties</span></span>
|<span data-ttu-id="14e72-117">属性</span><span class="sxs-lookup"><span data-stu-id="14e72-117">Property</span></span>|<span data-ttu-id="14e72-118">类型</span><span class="sxs-lookup"><span data-stu-id="14e72-118">Type</span></span>|<span data-ttu-id="14e72-119">说明</span><span class="sxs-lookup"><span data-stu-id="14e72-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14e72-120">inGracePeriodCount</span><span class="sxs-lookup"><span data-stu-id="14e72-120">inGracePeriodCount</span></span>|<span data-ttu-id="14e72-121">Int32</span><span class="sxs-lookup"><span data-stu-id="14e72-121">Int32</span></span>|<span data-ttu-id="14e72-122">宽限期内的设备数</span><span class="sxs-lookup"><span data-stu-id="14e72-122">Number of devices that are in grace period</span></span>|
|<span data-ttu-id="14e72-123">configManagerCount</span><span class="sxs-lookup"><span data-stu-id="14e72-123">configManagerCount</span></span>|<span data-ttu-id="14e72-124">Int32</span><span class="sxs-lookup"><span data-stu-id="14e72-124">Int32</span></span>|<span data-ttu-id="14e72-125">由 System Center Configuration Manager 管理符合性的设备数</span><span class="sxs-lookup"><span data-stu-id="14e72-125">Number of devices that have compliance managed by System Center Configuration Manager</span></span>|
|<span data-ttu-id="14e72-126">id</span><span class="sxs-lookup"><span data-stu-id="14e72-126">id</span></span>|<span data-ttu-id="14e72-127">String</span><span class="sxs-lookup"><span data-stu-id="14e72-127">String</span></span>|<span data-ttu-id="14e72-128">实体的键。</span><span class="sxs-lookup"><span data-stu-id="14e72-128">Key of the entity.</span></span>|
|<span data-ttu-id="14e72-129">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="14e72-129">unknownDeviceCount</span></span>|<span data-ttu-id="14e72-130">Int32</span><span class="sxs-lookup"><span data-stu-id="14e72-130">Int32</span></span>|<span data-ttu-id="14e72-131">未知设备的数量</span><span class="sxs-lookup"><span data-stu-id="14e72-131">Number of unknown devices</span></span>|
|<span data-ttu-id="14e72-132">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="14e72-132">notApplicableDeviceCount</span></span>|<span data-ttu-id="14e72-133">Int32</span><span class="sxs-lookup"><span data-stu-id="14e72-133">Int32</span></span>|<span data-ttu-id="14e72-134">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="14e72-134">Number of not applicable devices</span></span>|
|<span data-ttu-id="14e72-135">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="14e72-135">compliantDeviceCount</span></span>|<span data-ttu-id="14e72-136">Int32</span><span class="sxs-lookup"><span data-stu-id="14e72-136">Int32</span></span>|<span data-ttu-id="14e72-137">兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="14e72-137">Number of compliant devices</span></span>|
|<span data-ttu-id="14e72-138">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="14e72-138">remediatedDeviceCount</span></span>|<span data-ttu-id="14e72-139">Int32</span><span class="sxs-lookup"><span data-stu-id="14e72-139">Int32</span></span>|<span data-ttu-id="14e72-140">已修复设备的数量</span><span class="sxs-lookup"><span data-stu-id="14e72-140">Number of remediated devices</span></span>|
|<span data-ttu-id="14e72-141">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="14e72-141">nonCompliantDeviceCount</span></span>|<span data-ttu-id="14e72-142">Int32</span><span class="sxs-lookup"><span data-stu-id="14e72-142">Int32</span></span>|<span data-ttu-id="14e72-143">不兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="14e72-143">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="14e72-144">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="14e72-144">errorDeviceCount</span></span>|<span data-ttu-id="14e72-145">Int32</span><span class="sxs-lookup"><span data-stu-id="14e72-145">Int32</span></span>|<span data-ttu-id="14e72-146">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="14e72-146">Number of error devices</span></span>|
|<span data-ttu-id="14e72-147">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="14e72-147">conflictDeviceCount</span></span>|<span data-ttu-id="14e72-148">Int32</span><span class="sxs-lookup"><span data-stu-id="14e72-148">Int32</span></span>|<span data-ttu-id="14e72-149">冲突设备的数量</span><span class="sxs-lookup"><span data-stu-id="14e72-149">Number of conflict devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="14e72-150">关系</span><span class="sxs-lookup"><span data-stu-id="14e72-150">Relationships</span></span>
<span data-ttu-id="14e72-151">无</span><span class="sxs-lookup"><span data-stu-id="14e72-151">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="14e72-152">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="14e72-152">JSON Representation</span></span>
<span data-ttu-id="14e72-153">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="14e72-153">Here is a JSON representation of the resource.</span></span>
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



