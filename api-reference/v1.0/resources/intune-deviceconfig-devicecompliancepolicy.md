---
title: deviceCompliancePolicy 资源类型
description: '这是符合性策略的基类。 符合性策略特定于平台，每个平台的符合性策略相互独立，且继承自此处。 '
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 16160cc5658d64aca3ba8f50450a2c99fd4c8309
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48009350"
---
# <a name="devicecompliancepolicy-resource-type"></a><span data-ttu-id="55573-104">deviceCompliancePolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="55573-104">deviceCompliancePolicy resource type</span></span>

<span data-ttu-id="55573-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55573-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="55573-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="55573-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55573-107">这是符合性策略的基类。</span><span class="sxs-lookup"><span data-stu-id="55573-107">This is the base class for Compliance policy.</span></span> <span data-ttu-id="55573-108">符合性策略特定于平台，每个平台的符合性策略相互独立，且继承自此处。</span><span class="sxs-lookup"><span data-stu-id="55573-108">Compliance policies are platform specific and individual per-platform compliance policies inherit from here.</span></span> 

## <a name="methods"></a><span data-ttu-id="55573-109">方法</span><span class="sxs-lookup"><span data-stu-id="55573-109">Methods</span></span>
|<span data-ttu-id="55573-110">方法</span><span class="sxs-lookup"><span data-stu-id="55573-110">Method</span></span>|<span data-ttu-id="55573-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="55573-111">Return Type</span></span>|<span data-ttu-id="55573-112">说明</span><span class="sxs-lookup"><span data-stu-id="55573-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="55573-113">List deviceCompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="55573-113">List deviceCompliancePolicies</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-list.md)|<span data-ttu-id="55573-114">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="55573-114">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) collection</span></span>|<span data-ttu-id="55573-115">列出 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="55573-115">List properties and relationships of the [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) objects.</span></span>|
|[<span data-ttu-id="55573-116">Get deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="55573-116">Get deviceCompliancePolicy</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-get.md)|[<span data-ttu-id="55573-117">deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="55573-117">deviceCompliancePolicy</span></span>](../resources/intune-deviceconfig-devicecompliancepolicy.md)|<span data-ttu-id="55573-118">读取 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="55573-118">Read properties and relationships of the [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) object.</span></span>|
|[<span data-ttu-id="55573-119">assign 操作</span><span class="sxs-lookup"><span data-stu-id="55573-119">assign action</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-assign.md)|<span data-ttu-id="55573-120">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="55573-120">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="55573-121">尚未记录</span><span class="sxs-lookup"><span data-stu-id="55573-121">Not yet documented</span></span>|
|[<span data-ttu-id="55573-122">scheduleActionsForRules 操作</span><span class="sxs-lookup"><span data-stu-id="55573-122">scheduleActionsForRules action</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-scheduleactionsforrules.md)|<span data-ttu-id="55573-123">无</span><span class="sxs-lookup"><span data-stu-id="55573-123">None</span></span>|<span data-ttu-id="55573-124">尚未记录</span><span class="sxs-lookup"><span data-stu-id="55573-124">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="55573-125">属性</span><span class="sxs-lookup"><span data-stu-id="55573-125">Properties</span></span>
|<span data-ttu-id="55573-126">属性</span><span class="sxs-lookup"><span data-stu-id="55573-126">Property</span></span>|<span data-ttu-id="55573-127">类型</span><span class="sxs-lookup"><span data-stu-id="55573-127">Type</span></span>|<span data-ttu-id="55573-128">说明</span><span class="sxs-lookup"><span data-stu-id="55573-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55573-129">id</span><span class="sxs-lookup"><span data-stu-id="55573-129">id</span></span>|<span data-ttu-id="55573-130">String</span><span class="sxs-lookup"><span data-stu-id="55573-130">String</span></span>|<span data-ttu-id="55573-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="55573-131">Key of the entity.</span></span>|
|<span data-ttu-id="55573-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="55573-132">createdDateTime</span></span>|<span data-ttu-id="55573-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="55573-133">DateTimeOffset</span></span>|<span data-ttu-id="55573-134">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="55573-134">DateTime the object was created.</span></span>|
|<span data-ttu-id="55573-135">description</span><span class="sxs-lookup"><span data-stu-id="55573-135">description</span></span>|<span data-ttu-id="55573-136">String</span><span class="sxs-lookup"><span data-stu-id="55573-136">String</span></span>|<span data-ttu-id="55573-137">管理员提供的设备配置说明。</span><span class="sxs-lookup"><span data-stu-id="55573-137">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="55573-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="55573-138">lastModifiedDateTime</span></span>|<span data-ttu-id="55573-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="55573-139">DateTimeOffset</span></span>|<span data-ttu-id="55573-140">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="55573-140">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="55573-141">displayName</span><span class="sxs-lookup"><span data-stu-id="55573-141">displayName</span></span>|<span data-ttu-id="55573-142">String</span><span class="sxs-lookup"><span data-stu-id="55573-142">String</span></span>|<span data-ttu-id="55573-143">管理员提供的设备配置名称。</span><span class="sxs-lookup"><span data-stu-id="55573-143">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="55573-144">version</span><span class="sxs-lookup"><span data-stu-id="55573-144">version</span></span>|<span data-ttu-id="55573-145">Int32</span><span class="sxs-lookup"><span data-stu-id="55573-145">Int32</span></span>|<span data-ttu-id="55573-146">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="55573-146">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="55573-147">关系</span><span class="sxs-lookup"><span data-stu-id="55573-147">Relationships</span></span>
|<span data-ttu-id="55573-148">关系</span><span class="sxs-lookup"><span data-stu-id="55573-148">Relationship</span></span>|<span data-ttu-id="55573-149">类型</span><span class="sxs-lookup"><span data-stu-id="55573-149">Type</span></span>|<span data-ttu-id="55573-150">说明</span><span class="sxs-lookup"><span data-stu-id="55573-150">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55573-151">scheduledActionsForRule</span><span class="sxs-lookup"><span data-stu-id="55573-151">scheduledActionsForRule</span></span>|<span data-ttu-id="55573-152">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="55573-152">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) collection</span></span>|<span data-ttu-id="55573-153">此规则的计划操作列表</span><span class="sxs-lookup"><span data-stu-id="55573-153">The list of scheduled action for this rule</span></span>|
|<span data-ttu-id="55573-154">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="55573-154">deviceStatuses</span></span>|<span data-ttu-id="55573-155">[deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="55573-155">[deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) collection</span></span>|<span data-ttu-id="55573-156">DeviceComplianceDeviceStatus 的列表。</span><span class="sxs-lookup"><span data-stu-id="55573-156">List of DeviceComplianceDeviceStatus.</span></span>|
|<span data-ttu-id="55573-157">userStatuses</span><span class="sxs-lookup"><span data-stu-id="55573-157">userStatuses</span></span>|<span data-ttu-id="55573-158">[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="55573-158">[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) collection</span></span>|<span data-ttu-id="55573-159">DeviceComplianceUserStatus 的列表。</span><span class="sxs-lookup"><span data-stu-id="55573-159">List of DeviceComplianceUserStatus.</span></span>|
|<span data-ttu-id="55573-160">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="55573-160">deviceStatusOverview</span></span>|[<span data-ttu-id="55573-161">deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="55573-161">deviceComplianceDeviceOverview</span></span>](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md)|<span data-ttu-id="55573-162">设备符合性设备状态概述</span><span class="sxs-lookup"><span data-stu-id="55573-162">Device compliance devices status overview</span></span>|
|<span data-ttu-id="55573-163">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="55573-163">userStatusOverview</span></span>|[<span data-ttu-id="55573-164">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="55573-164">deviceComplianceUserOverview</span></span>](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|<span data-ttu-id="55573-165">设备符合性用户状态概述</span><span class="sxs-lookup"><span data-stu-id="55573-165">Device compliance users status overview</span></span>|
|<span data-ttu-id="55573-166">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="55573-166">deviceSettingStateSummaries</span></span>|<span data-ttu-id="55573-167">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="55573-167">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="55573-168">符合性设置状态设备摘要</span><span class="sxs-lookup"><span data-stu-id="55573-168">Compliance Setting State Device Summary</span></span>|
|<span data-ttu-id="55573-169">assignments</span><span class="sxs-lookup"><span data-stu-id="55573-169">assignments</span></span>|<span data-ttu-id="55573-170">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="55573-170">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="55573-171">此符合性策略的分配集合。</span><span class="sxs-lookup"><span data-stu-id="55573-171">The collection of assignments for this compliance policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="55573-172">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="55573-172">JSON Representation</span></span>
<span data-ttu-id="55573-173">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="55573-173">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCompliancePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicy",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024
}
```









