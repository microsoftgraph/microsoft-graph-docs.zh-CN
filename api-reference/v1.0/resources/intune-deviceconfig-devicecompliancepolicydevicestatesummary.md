---
title: deviceCompliancePolicyDeviceStateSummary 资源类型
description: 尚未记录
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 73609ae16400dbb36b14cedd6eb07646530c7a45
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532604"
---
# <a name="devicecompliancepolicydevicestatesummary-resource-type"></a><span data-ttu-id="96038-103">deviceCompliancePolicyDeviceStateSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="96038-103">deviceCompliancePolicyDeviceStateSummary resource type</span></span>

<span data-ttu-id="96038-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96038-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="96038-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="96038-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="96038-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="96038-106">Not yet documented</span></span>

## <a name="methods"></a><span data-ttu-id="96038-107">Methods</span><span class="sxs-lookup"><span data-stu-id="96038-107">Methods</span></span>
|<span data-ttu-id="96038-108">方法</span><span class="sxs-lookup"><span data-stu-id="96038-108">Method</span></span>|<span data-ttu-id="96038-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="96038-109">Return Type</span></span>|<span data-ttu-id="96038-110">说明</span><span class="sxs-lookup"><span data-stu-id="96038-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="96038-111">获取 deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="96038-111">Get deviceCompliancePolicyDeviceStateSummary</span></span>](../api/intune-deviceconfig-devicecompliancepolicydevicestatesummary-get.md)|[<span data-ttu-id="96038-112">deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="96038-112">deviceCompliancePolicyDeviceStateSummary</span></span>](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|<span data-ttu-id="96038-113">读取 [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="96038-113">Read properties and relationships of the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>|
|[<span data-ttu-id="96038-114">更新 deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="96038-114">Update deviceCompliancePolicyDeviceStateSummary</span></span>](../api/intune-deviceconfig-devicecompliancepolicydevicestatesummary-update.md)|[<span data-ttu-id="96038-115">deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="96038-115">deviceCompliancePolicyDeviceStateSummary</span></span>](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|<span data-ttu-id="96038-116">更新 [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="96038-116">Update the properties of a [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="96038-117">属性</span><span class="sxs-lookup"><span data-stu-id="96038-117">Properties</span></span>
|<span data-ttu-id="96038-118">属性</span><span class="sxs-lookup"><span data-stu-id="96038-118">Property</span></span>|<span data-ttu-id="96038-119">类型</span><span class="sxs-lookup"><span data-stu-id="96038-119">Type</span></span>|<span data-ttu-id="96038-120">说明</span><span class="sxs-lookup"><span data-stu-id="96038-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96038-121">inGracePeriodCount</span><span class="sxs-lookup"><span data-stu-id="96038-121">inGracePeriodCount</span></span>|<span data-ttu-id="96038-122">Int32</span><span class="sxs-lookup"><span data-stu-id="96038-122">Int32</span></span>|<span data-ttu-id="96038-123">宽限期内的设备数</span><span class="sxs-lookup"><span data-stu-id="96038-123">Number of devices that are in grace period</span></span>|
|<span data-ttu-id="96038-124">configManagerCount</span><span class="sxs-lookup"><span data-stu-id="96038-124">configManagerCount</span></span>|<span data-ttu-id="96038-125">Int32</span><span class="sxs-lookup"><span data-stu-id="96038-125">Int32</span></span>|<span data-ttu-id="96038-126">由 System Center Configuration Manager 管理符合性的设备数</span><span class="sxs-lookup"><span data-stu-id="96038-126">Number of devices that have compliance managed by System Center Configuration Manager</span></span>|
|<span data-ttu-id="96038-127">id</span><span class="sxs-lookup"><span data-stu-id="96038-127">id</span></span>|<span data-ttu-id="96038-128">字符串</span><span class="sxs-lookup"><span data-stu-id="96038-128">String</span></span>|<span data-ttu-id="96038-129">实体的键。</span><span class="sxs-lookup"><span data-stu-id="96038-129">Key of the entity.</span></span>|
|<span data-ttu-id="96038-130">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="96038-130">unknownDeviceCount</span></span>|<span data-ttu-id="96038-131">Int32</span><span class="sxs-lookup"><span data-stu-id="96038-131">Int32</span></span>|<span data-ttu-id="96038-132">未知设备的数量</span><span class="sxs-lookup"><span data-stu-id="96038-132">Number of unknown devices</span></span>|
|<span data-ttu-id="96038-133">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="96038-133">notApplicableDeviceCount</span></span>|<span data-ttu-id="96038-134">Int32</span><span class="sxs-lookup"><span data-stu-id="96038-134">Int32</span></span>|<span data-ttu-id="96038-135">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="96038-135">Number of not applicable devices</span></span>|
|<span data-ttu-id="96038-136">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="96038-136">compliantDeviceCount</span></span>|<span data-ttu-id="96038-137">Int32</span><span class="sxs-lookup"><span data-stu-id="96038-137">Int32</span></span>|<span data-ttu-id="96038-138">兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="96038-138">Number of compliant devices</span></span>|
|<span data-ttu-id="96038-139">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="96038-139">remediatedDeviceCount</span></span>|<span data-ttu-id="96038-140">Int32</span><span class="sxs-lookup"><span data-stu-id="96038-140">Int32</span></span>|<span data-ttu-id="96038-141">已修复设备的数量</span><span class="sxs-lookup"><span data-stu-id="96038-141">Number of remediated devices</span></span>|
|<span data-ttu-id="96038-142">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="96038-142">nonCompliantDeviceCount</span></span>|<span data-ttu-id="96038-143">Int32</span><span class="sxs-lookup"><span data-stu-id="96038-143">Int32</span></span>|<span data-ttu-id="96038-144">不兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="96038-144">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="96038-145">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="96038-145">errorDeviceCount</span></span>|<span data-ttu-id="96038-146">Int32</span><span class="sxs-lookup"><span data-stu-id="96038-146">Int32</span></span>|<span data-ttu-id="96038-147">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="96038-147">Number of error devices</span></span>|
|<span data-ttu-id="96038-148">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="96038-148">conflictDeviceCount</span></span>|<span data-ttu-id="96038-149">Int32</span><span class="sxs-lookup"><span data-stu-id="96038-149">Int32</span></span>|<span data-ttu-id="96038-150">冲突设备的数量</span><span class="sxs-lookup"><span data-stu-id="96038-150">Number of conflict devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="96038-151">关系</span><span class="sxs-lookup"><span data-stu-id="96038-151">Relationships</span></span>
<span data-ttu-id="96038-152">无</span><span class="sxs-lookup"><span data-stu-id="96038-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="96038-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="96038-153">JSON Representation</span></span>
<span data-ttu-id="96038-154">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="96038-154">Here is a JSON representation of the resource.</span></span>
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




