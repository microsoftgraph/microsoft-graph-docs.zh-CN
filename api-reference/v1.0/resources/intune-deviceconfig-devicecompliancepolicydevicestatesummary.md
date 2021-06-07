---
title: deviceCompliancePolicyDeviceStateSummary 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 973a2d4e9779174ec0e7cecd244e347cf28d24f7
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752124"
---
# <a name="devicecompliancepolicydevicestatesummary-resource-type"></a><span data-ttu-id="f6597-103">deviceCompliancePolicyDeviceStateSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="f6597-103">deviceCompliancePolicyDeviceStateSummary resource type</span></span>

<span data-ttu-id="f6597-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6597-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f6597-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f6597-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f6597-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f6597-106">Not yet documented</span></span>

## <a name="methods"></a><span data-ttu-id="f6597-107">Methods</span><span class="sxs-lookup"><span data-stu-id="f6597-107">Methods</span></span>
|<span data-ttu-id="f6597-108">方法</span><span class="sxs-lookup"><span data-stu-id="f6597-108">Method</span></span>|<span data-ttu-id="f6597-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="f6597-109">Return Type</span></span>|<span data-ttu-id="f6597-110">Description</span><span class="sxs-lookup"><span data-stu-id="f6597-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f6597-111">获取 deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="f6597-111">Get deviceCompliancePolicyDeviceStateSummary</span></span>](../api/intune-deviceconfig-devicecompliancepolicydevicestatesummary-get.md)|[<span data-ttu-id="f6597-112">deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="f6597-112">deviceCompliancePolicyDeviceStateSummary</span></span>](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|<span data-ttu-id="f6597-113">读取 [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f6597-113">Read properties and relationships of the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>|
|[<span data-ttu-id="f6597-114">更新 deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="f6597-114">Update deviceCompliancePolicyDeviceStateSummary</span></span>](../api/intune-deviceconfig-devicecompliancepolicydevicestatesummary-update.md)|[<span data-ttu-id="f6597-115">deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="f6597-115">deviceCompliancePolicyDeviceStateSummary</span></span>](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|<span data-ttu-id="f6597-116">更新 [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f6597-116">Update the properties of a [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f6597-117">属性</span><span class="sxs-lookup"><span data-stu-id="f6597-117">Properties</span></span>
|<span data-ttu-id="f6597-118">属性</span><span class="sxs-lookup"><span data-stu-id="f6597-118">Property</span></span>|<span data-ttu-id="f6597-119">类型</span><span class="sxs-lookup"><span data-stu-id="f6597-119">Type</span></span>|<span data-ttu-id="f6597-120">Description</span><span class="sxs-lookup"><span data-stu-id="f6597-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6597-121">inGracePeriodCount</span><span class="sxs-lookup"><span data-stu-id="f6597-121">inGracePeriodCount</span></span>|<span data-ttu-id="f6597-122">Int32</span><span class="sxs-lookup"><span data-stu-id="f6597-122">Int32</span></span>|<span data-ttu-id="f6597-123">宽限期内的设备数</span><span class="sxs-lookup"><span data-stu-id="f6597-123">Number of devices that are in grace period</span></span>|
|<span data-ttu-id="f6597-124">configManagerCount</span><span class="sxs-lookup"><span data-stu-id="f6597-124">configManagerCount</span></span>|<span data-ttu-id="f6597-125">Int32</span><span class="sxs-lookup"><span data-stu-id="f6597-125">Int32</span></span>|<span data-ttu-id="f6597-126">由 System Center Configuration Manager 管理符合性的设备数</span><span class="sxs-lookup"><span data-stu-id="f6597-126">Number of devices that have compliance managed by System Center Configuration Manager</span></span>|
|<span data-ttu-id="f6597-127">id</span><span class="sxs-lookup"><span data-stu-id="f6597-127">id</span></span>|<span data-ttu-id="f6597-128">String</span><span class="sxs-lookup"><span data-stu-id="f6597-128">String</span></span>|<span data-ttu-id="f6597-129">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f6597-129">Key of the entity.</span></span>|
|<span data-ttu-id="f6597-130">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f6597-130">unknownDeviceCount</span></span>|<span data-ttu-id="f6597-131">Int32</span><span class="sxs-lookup"><span data-stu-id="f6597-131">Int32</span></span>|<span data-ttu-id="f6597-132">未知设备的数量</span><span class="sxs-lookup"><span data-stu-id="f6597-132">Number of unknown devices</span></span>|
|<span data-ttu-id="f6597-133">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f6597-133">notApplicableDeviceCount</span></span>|<span data-ttu-id="f6597-134">Int32</span><span class="sxs-lookup"><span data-stu-id="f6597-134">Int32</span></span>|<span data-ttu-id="f6597-135">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="f6597-135">Number of not applicable devices</span></span>|
|<span data-ttu-id="f6597-136">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f6597-136">compliantDeviceCount</span></span>|<span data-ttu-id="f6597-137">Int32</span><span class="sxs-lookup"><span data-stu-id="f6597-137">Int32</span></span>|<span data-ttu-id="f6597-138">兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="f6597-138">Number of compliant devices</span></span>|
|<span data-ttu-id="f6597-139">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f6597-139">remediatedDeviceCount</span></span>|<span data-ttu-id="f6597-140">Int32</span><span class="sxs-lookup"><span data-stu-id="f6597-140">Int32</span></span>|<span data-ttu-id="f6597-141">已修复设备的数量</span><span class="sxs-lookup"><span data-stu-id="f6597-141">Number of remediated devices</span></span>|
|<span data-ttu-id="f6597-142">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f6597-142">nonCompliantDeviceCount</span></span>|<span data-ttu-id="f6597-143">Int32</span><span class="sxs-lookup"><span data-stu-id="f6597-143">Int32</span></span>|<span data-ttu-id="f6597-144">不兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="f6597-144">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="f6597-145">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f6597-145">errorDeviceCount</span></span>|<span data-ttu-id="f6597-146">Int32</span><span class="sxs-lookup"><span data-stu-id="f6597-146">Int32</span></span>|<span data-ttu-id="f6597-147">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="f6597-147">Number of error devices</span></span>|
|<span data-ttu-id="f6597-148">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f6597-148">conflictDeviceCount</span></span>|<span data-ttu-id="f6597-149">Int32</span><span class="sxs-lookup"><span data-stu-id="f6597-149">Int32</span></span>|<span data-ttu-id="f6597-150">冲突设备的数量</span><span class="sxs-lookup"><span data-stu-id="f6597-150">Number of conflict devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="f6597-151">关系</span><span class="sxs-lookup"><span data-stu-id="f6597-151">Relationships</span></span>
<span data-ttu-id="f6597-152">无</span><span class="sxs-lookup"><span data-stu-id="f6597-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f6597-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f6597-153">JSON Representation</span></span>
<span data-ttu-id="f6597-154">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f6597-154">Here is a JSON representation of the resource.</span></span>
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




