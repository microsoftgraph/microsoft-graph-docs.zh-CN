---
title: deviceCompliancePolicyDeviceStateSummary 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b21b34506c9ef763751a32a4e83b9c7f5e363a19
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815818"
---
# <a name="devicecompliancepolicydevicestatesummary-resource-type"></a><span data-ttu-id="e6061-103">deviceCompliancePolicyDeviceStateSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="e6061-103">deviceCompliancePolicyDeviceStateSummary resource type</span></span>

> <span data-ttu-id="e6061-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e6061-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e6061-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e6061-105">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="e6061-106">方法</span><span class="sxs-lookup"><span data-stu-id="e6061-106">Methods</span></span>
|<span data-ttu-id="e6061-107">方法</span><span class="sxs-lookup"><span data-stu-id="e6061-107">Method</span></span>|<span data-ttu-id="e6061-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="e6061-108">Return Type</span></span>|<span data-ttu-id="e6061-109">说明</span><span class="sxs-lookup"><span data-stu-id="e6061-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e6061-110">获取 deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="e6061-110">Get deviceCompliancePolicyDeviceStateSummary</span></span>](../api/intune-deviceconfig-devicecompliancepolicydevicestatesummary-get.md)|[<span data-ttu-id="e6061-111">deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="e6061-111">deviceCompliancePolicyDeviceStateSummary</span></span>](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|<span data-ttu-id="e6061-112">读取 [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e6061-112">Read properties and relationships of the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>|
|[<span data-ttu-id="e6061-113">更新 deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="e6061-113">Update deviceCompliancePolicyDeviceStateSummary</span></span>](../api/intune-deviceconfig-devicecompliancepolicydevicestatesummary-update.md)|[<span data-ttu-id="e6061-114">deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="e6061-114">deviceCompliancePolicyDeviceStateSummary</span></span>](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|<span data-ttu-id="e6061-115">更新 [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e6061-115">Update the properties of a [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e6061-116">属性</span><span class="sxs-lookup"><span data-stu-id="e6061-116">Properties</span></span>
|<span data-ttu-id="e6061-117">属性</span><span class="sxs-lookup"><span data-stu-id="e6061-117">Property</span></span>|<span data-ttu-id="e6061-118">类型</span><span class="sxs-lookup"><span data-stu-id="e6061-118">Type</span></span>|<span data-ttu-id="e6061-119">说明</span><span class="sxs-lookup"><span data-stu-id="e6061-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6061-120">inGracePeriodCount</span><span class="sxs-lookup"><span data-stu-id="e6061-120">inGracePeriodCount</span></span>|<span data-ttu-id="e6061-121">Int32</span><span class="sxs-lookup"><span data-stu-id="e6061-121">Int32</span></span>|<span data-ttu-id="e6061-122">宽限期内的设备数</span><span class="sxs-lookup"><span data-stu-id="e6061-122">Number of devices that are in grace period</span></span>|
|<span data-ttu-id="e6061-123">configManagerCount</span><span class="sxs-lookup"><span data-stu-id="e6061-123">configManagerCount</span></span>|<span data-ttu-id="e6061-124">Int32</span><span class="sxs-lookup"><span data-stu-id="e6061-124">Int32</span></span>|<span data-ttu-id="e6061-125">由 System Center Configuration Manager 管理符合性的设备数</span><span class="sxs-lookup"><span data-stu-id="e6061-125">Number of devices that have compliance managed by System Center Configuration Manager</span></span>|
|<span data-ttu-id="e6061-126">id</span><span class="sxs-lookup"><span data-stu-id="e6061-126">id</span></span>|<span data-ttu-id="e6061-127">String</span><span class="sxs-lookup"><span data-stu-id="e6061-127">String</span></span>|<span data-ttu-id="e6061-128">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e6061-128">Key of the entity.</span></span>|
|<span data-ttu-id="e6061-129">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e6061-129">unknownDeviceCount</span></span>|<span data-ttu-id="e6061-130">Int32</span><span class="sxs-lookup"><span data-stu-id="e6061-130">Int32</span></span>|<span data-ttu-id="e6061-131">未知设备的数量</span><span class="sxs-lookup"><span data-stu-id="e6061-131">Number of unknown devices</span></span>|
|<span data-ttu-id="e6061-132">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e6061-132">notApplicableDeviceCount</span></span>|<span data-ttu-id="e6061-133">Int32</span><span class="sxs-lookup"><span data-stu-id="e6061-133">Int32</span></span>|<span data-ttu-id="e6061-134">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="e6061-134">Number of not applicable devices</span></span>|
|<span data-ttu-id="e6061-135">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e6061-135">compliantDeviceCount</span></span>|<span data-ttu-id="e6061-136">Int32</span><span class="sxs-lookup"><span data-stu-id="e6061-136">Int32</span></span>|<span data-ttu-id="e6061-137">兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="e6061-137">Number of compliant devices</span></span>|
|<span data-ttu-id="e6061-138">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e6061-138">remediatedDeviceCount</span></span>|<span data-ttu-id="e6061-139">Int32</span><span class="sxs-lookup"><span data-stu-id="e6061-139">Int32</span></span>|<span data-ttu-id="e6061-140">已修复设备的数量</span><span class="sxs-lookup"><span data-stu-id="e6061-140">Number of remediated devices</span></span>|
|<span data-ttu-id="e6061-141">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e6061-141">nonCompliantDeviceCount</span></span>|<span data-ttu-id="e6061-142">Int32</span><span class="sxs-lookup"><span data-stu-id="e6061-142">Int32</span></span>|<span data-ttu-id="e6061-143">不兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="e6061-143">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="e6061-144">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e6061-144">errorDeviceCount</span></span>|<span data-ttu-id="e6061-145">Int32</span><span class="sxs-lookup"><span data-stu-id="e6061-145">Int32</span></span>|<span data-ttu-id="e6061-146">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="e6061-146">Number of error devices</span></span>|
|<span data-ttu-id="e6061-147">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e6061-147">conflictDeviceCount</span></span>|<span data-ttu-id="e6061-148">Int32</span><span class="sxs-lookup"><span data-stu-id="e6061-148">Int32</span></span>|<span data-ttu-id="e6061-149">冲突设备的数量</span><span class="sxs-lookup"><span data-stu-id="e6061-149">Number of conflict devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="e6061-150">关系</span><span class="sxs-lookup"><span data-stu-id="e6061-150">Relationships</span></span>
<span data-ttu-id="e6061-151">无</span><span class="sxs-lookup"><span data-stu-id="e6061-151">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e6061-152">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e6061-152">JSON Representation</span></span>
<span data-ttu-id="e6061-153">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e6061-153">Here is a JSON representation of the resource.</span></span>
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



