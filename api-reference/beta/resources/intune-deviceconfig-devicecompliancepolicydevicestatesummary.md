---
title: deviceCompliancePolicyDeviceStateSummary 资源类型
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ae4643cd5cb51091f815e372ad9582fbe6f416ff
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35970568"
---
# <a name="devicecompliancepolicydevicestatesummary-resource-type"></a><span data-ttu-id="ec63c-103">deviceCompliancePolicyDeviceStateSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="ec63c-103">deviceCompliancePolicyDeviceStateSummary resource type</span></span>

> <span data-ttu-id="ec63c-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ec63c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ec63c-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ec63c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ec63c-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="ec63c-106">Not yet documented</span></span>

## <a name="methods"></a><span data-ttu-id="ec63c-107">方法</span><span class="sxs-lookup"><span data-stu-id="ec63c-107">Methods</span></span>
|<span data-ttu-id="ec63c-108">方法</span><span class="sxs-lookup"><span data-stu-id="ec63c-108">Method</span></span>|<span data-ttu-id="ec63c-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="ec63c-109">Return Type</span></span>|<span data-ttu-id="ec63c-110">说明</span><span class="sxs-lookup"><span data-stu-id="ec63c-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ec63c-111">获取 deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="ec63c-111">Get deviceCompliancePolicyDeviceStateSummary</span></span>](../api/intune-deviceconfig-devicecompliancepolicydevicestatesummary-get.md)|[<span data-ttu-id="ec63c-112">deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="ec63c-112">deviceCompliancePolicyDeviceStateSummary</span></span>](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|<span data-ttu-id="ec63c-113">读取 [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ec63c-113">Read properties and relationships of the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>|
|[<span data-ttu-id="ec63c-114">更新 deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="ec63c-114">Update deviceCompliancePolicyDeviceStateSummary</span></span>](../api/intune-deviceconfig-devicecompliancepolicydevicestatesummary-update.md)|[<span data-ttu-id="ec63c-115">deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="ec63c-115">deviceCompliancePolicyDeviceStateSummary</span></span>](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|<span data-ttu-id="ec63c-116">更新 [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ec63c-116">Update the properties of a [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ec63c-117">属性</span><span class="sxs-lookup"><span data-stu-id="ec63c-117">Properties</span></span>
|<span data-ttu-id="ec63c-118">属性</span><span class="sxs-lookup"><span data-stu-id="ec63c-118">Property</span></span>|<span data-ttu-id="ec63c-119">类型</span><span class="sxs-lookup"><span data-stu-id="ec63c-119">Type</span></span>|<span data-ttu-id="ec63c-120">说明</span><span class="sxs-lookup"><span data-stu-id="ec63c-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec63c-121">inGracePeriodCount</span><span class="sxs-lookup"><span data-stu-id="ec63c-121">inGracePeriodCount</span></span>|<span data-ttu-id="ec63c-122">Int32</span><span class="sxs-lookup"><span data-stu-id="ec63c-122">Int32</span></span>|<span data-ttu-id="ec63c-123">宽限期内的设备数</span><span class="sxs-lookup"><span data-stu-id="ec63c-123">Number of devices that are in grace period</span></span>|
|<span data-ttu-id="ec63c-124">configManagerCount</span><span class="sxs-lookup"><span data-stu-id="ec63c-124">configManagerCount</span></span>|<span data-ttu-id="ec63c-125">Int32</span><span class="sxs-lookup"><span data-stu-id="ec63c-125">Int32</span></span>|<span data-ttu-id="ec63c-126">由 System Center Configuration Manager 管理符合性的设备数</span><span class="sxs-lookup"><span data-stu-id="ec63c-126">Number of devices that have compliance managed by System Center Configuration Manager</span></span>|
|<span data-ttu-id="ec63c-127">id</span><span class="sxs-lookup"><span data-stu-id="ec63c-127">id</span></span>|<span data-ttu-id="ec63c-128">String</span><span class="sxs-lookup"><span data-stu-id="ec63c-128">String</span></span>|<span data-ttu-id="ec63c-129">实体的键。</span><span class="sxs-lookup"><span data-stu-id="ec63c-129">Key of the entity.</span></span>|
|<span data-ttu-id="ec63c-130">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ec63c-130">unknownDeviceCount</span></span>|<span data-ttu-id="ec63c-131">Int32</span><span class="sxs-lookup"><span data-stu-id="ec63c-131">Int32</span></span>|<span data-ttu-id="ec63c-132">未知设备的数量</span><span class="sxs-lookup"><span data-stu-id="ec63c-132">Number of unknown devices</span></span>|
|<span data-ttu-id="ec63c-133">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ec63c-133">notApplicableDeviceCount</span></span>|<span data-ttu-id="ec63c-134">Int32</span><span class="sxs-lookup"><span data-stu-id="ec63c-134">Int32</span></span>|<span data-ttu-id="ec63c-135">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="ec63c-135">Number of not applicable devices</span></span>|
|<span data-ttu-id="ec63c-136">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ec63c-136">compliantDeviceCount</span></span>|<span data-ttu-id="ec63c-137">Int32</span><span class="sxs-lookup"><span data-stu-id="ec63c-137">Int32</span></span>|<span data-ttu-id="ec63c-138">兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="ec63c-138">Number of compliant devices</span></span>|
|<span data-ttu-id="ec63c-139">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ec63c-139">remediatedDeviceCount</span></span>|<span data-ttu-id="ec63c-140">Int32</span><span class="sxs-lookup"><span data-stu-id="ec63c-140">Int32</span></span>|<span data-ttu-id="ec63c-141">已修复设备的数量</span><span class="sxs-lookup"><span data-stu-id="ec63c-141">Number of remediated devices</span></span>|
|<span data-ttu-id="ec63c-142">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ec63c-142">nonCompliantDeviceCount</span></span>|<span data-ttu-id="ec63c-143">Int32</span><span class="sxs-lookup"><span data-stu-id="ec63c-143">Int32</span></span>|<span data-ttu-id="ec63c-144">不兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="ec63c-144">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="ec63c-145">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ec63c-145">errorDeviceCount</span></span>|<span data-ttu-id="ec63c-146">Int32</span><span class="sxs-lookup"><span data-stu-id="ec63c-146">Int32</span></span>|<span data-ttu-id="ec63c-147">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="ec63c-147">Number of error devices</span></span>|
|<span data-ttu-id="ec63c-148">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ec63c-148">conflictDeviceCount</span></span>|<span data-ttu-id="ec63c-149">Int32</span><span class="sxs-lookup"><span data-stu-id="ec63c-149">Int32</span></span>|<span data-ttu-id="ec63c-150">冲突设备的数量</span><span class="sxs-lookup"><span data-stu-id="ec63c-150">Number of conflict devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="ec63c-151">关系</span><span class="sxs-lookup"><span data-stu-id="ec63c-151">Relationships</span></span>
<span data-ttu-id="ec63c-152">无</span><span class="sxs-lookup"><span data-stu-id="ec63c-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ec63c-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ec63c-153">JSON Representation</span></span>
<span data-ttu-id="ec63c-154">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ec63c-154">Here is a JSON representation of the resource.</span></span>
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





