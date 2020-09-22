---
title: deviceCompliancePolicyDeviceStateSummary 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 97c04f9f518d45baab24468ff842968dd54a7572
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48010260"
---
# <a name="devicecompliancepolicydevicestatesummary-resource-type"></a><span data-ttu-id="98313-103">deviceCompliancePolicyDeviceStateSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="98313-103">deviceCompliancePolicyDeviceStateSummary resource type</span></span>

<span data-ttu-id="98313-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="98313-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="98313-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="98313-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="98313-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="98313-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="98313-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="98313-107">Not yet documented</span></span>

## <a name="methods"></a><span data-ttu-id="98313-108">方法</span><span class="sxs-lookup"><span data-stu-id="98313-108">Methods</span></span>
|<span data-ttu-id="98313-109">方法</span><span class="sxs-lookup"><span data-stu-id="98313-109">Method</span></span>|<span data-ttu-id="98313-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="98313-110">Return Type</span></span>|<span data-ttu-id="98313-111">说明</span><span class="sxs-lookup"><span data-stu-id="98313-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="98313-112">获取 deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="98313-112">Get deviceCompliancePolicyDeviceStateSummary</span></span>](../api/intune-deviceconfig-devicecompliancepolicydevicestatesummary-get.md)|[<span data-ttu-id="98313-113">deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="98313-113">deviceCompliancePolicyDeviceStateSummary</span></span>](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|<span data-ttu-id="98313-114">读取 [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="98313-114">Read properties and relationships of the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>|
|[<span data-ttu-id="98313-115">更新 deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="98313-115">Update deviceCompliancePolicyDeviceStateSummary</span></span>](../api/intune-deviceconfig-devicecompliancepolicydevicestatesummary-update.md)|[<span data-ttu-id="98313-116">deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="98313-116">deviceCompliancePolicyDeviceStateSummary</span></span>](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|<span data-ttu-id="98313-117">更新 [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="98313-117">Update the properties of a [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="98313-118">属性</span><span class="sxs-lookup"><span data-stu-id="98313-118">Properties</span></span>
|<span data-ttu-id="98313-119">属性</span><span class="sxs-lookup"><span data-stu-id="98313-119">Property</span></span>|<span data-ttu-id="98313-120">类型</span><span class="sxs-lookup"><span data-stu-id="98313-120">Type</span></span>|<span data-ttu-id="98313-121">说明</span><span class="sxs-lookup"><span data-stu-id="98313-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98313-122">inGracePeriodCount</span><span class="sxs-lookup"><span data-stu-id="98313-122">inGracePeriodCount</span></span>|<span data-ttu-id="98313-123">Int32</span><span class="sxs-lookup"><span data-stu-id="98313-123">Int32</span></span>|<span data-ttu-id="98313-124">宽限期内的设备数</span><span class="sxs-lookup"><span data-stu-id="98313-124">Number of devices that are in grace period</span></span>|
|<span data-ttu-id="98313-125">configManagerCount</span><span class="sxs-lookup"><span data-stu-id="98313-125">configManagerCount</span></span>|<span data-ttu-id="98313-126">Int32</span><span class="sxs-lookup"><span data-stu-id="98313-126">Int32</span></span>|<span data-ttu-id="98313-127">由 System Center Configuration Manager 管理符合性的设备数</span><span class="sxs-lookup"><span data-stu-id="98313-127">Number of devices that have compliance managed by System Center Configuration Manager</span></span>|
|<span data-ttu-id="98313-128">id</span><span class="sxs-lookup"><span data-stu-id="98313-128">id</span></span>|<span data-ttu-id="98313-129">String</span><span class="sxs-lookup"><span data-stu-id="98313-129">String</span></span>|<span data-ttu-id="98313-130">实体的键。</span><span class="sxs-lookup"><span data-stu-id="98313-130">Key of the entity.</span></span>|
|<span data-ttu-id="98313-131">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="98313-131">unknownDeviceCount</span></span>|<span data-ttu-id="98313-132">Int32</span><span class="sxs-lookup"><span data-stu-id="98313-132">Int32</span></span>|<span data-ttu-id="98313-133">未知设备的数量</span><span class="sxs-lookup"><span data-stu-id="98313-133">Number of unknown devices</span></span>|
|<span data-ttu-id="98313-134">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="98313-134">notApplicableDeviceCount</span></span>|<span data-ttu-id="98313-135">Int32</span><span class="sxs-lookup"><span data-stu-id="98313-135">Int32</span></span>|<span data-ttu-id="98313-136">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="98313-136">Number of not applicable devices</span></span>|
|<span data-ttu-id="98313-137">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="98313-137">compliantDeviceCount</span></span>|<span data-ttu-id="98313-138">Int32</span><span class="sxs-lookup"><span data-stu-id="98313-138">Int32</span></span>|<span data-ttu-id="98313-139">兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="98313-139">Number of compliant devices</span></span>|
|<span data-ttu-id="98313-140">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="98313-140">remediatedDeviceCount</span></span>|<span data-ttu-id="98313-141">Int32</span><span class="sxs-lookup"><span data-stu-id="98313-141">Int32</span></span>|<span data-ttu-id="98313-142">已修复设备的数量</span><span class="sxs-lookup"><span data-stu-id="98313-142">Number of remediated devices</span></span>|
|<span data-ttu-id="98313-143">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="98313-143">nonCompliantDeviceCount</span></span>|<span data-ttu-id="98313-144">Int32</span><span class="sxs-lookup"><span data-stu-id="98313-144">Int32</span></span>|<span data-ttu-id="98313-145">不兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="98313-145">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="98313-146">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="98313-146">errorDeviceCount</span></span>|<span data-ttu-id="98313-147">Int32</span><span class="sxs-lookup"><span data-stu-id="98313-147">Int32</span></span>|<span data-ttu-id="98313-148">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="98313-148">Number of error devices</span></span>|
|<span data-ttu-id="98313-149">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="98313-149">conflictDeviceCount</span></span>|<span data-ttu-id="98313-150">Int32</span><span class="sxs-lookup"><span data-stu-id="98313-150">Int32</span></span>|<span data-ttu-id="98313-151">冲突设备的数量</span><span class="sxs-lookup"><span data-stu-id="98313-151">Number of conflict devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="98313-152">关系</span><span class="sxs-lookup"><span data-stu-id="98313-152">Relationships</span></span>
<span data-ttu-id="98313-153">无</span><span class="sxs-lookup"><span data-stu-id="98313-153">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="98313-154">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="98313-154">JSON Representation</span></span>
<span data-ttu-id="98313-155">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="98313-155">Here is a JSON representation of the resource.</span></span>
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






