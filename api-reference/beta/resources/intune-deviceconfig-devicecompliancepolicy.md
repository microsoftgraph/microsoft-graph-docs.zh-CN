---
title: deviceCompliancePolicy 资源类型
description: '这是符合性策略的基类。 符合性策略特定于平台，每个平台的符合性策略相互独立，且继承自此处。 '
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1a02fc8ab612011edf1ff6f2d1e281d8aeb8f8e6
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407569"
---
# <a name="devicecompliancepolicy-resource-type"></a><span data-ttu-id="e54ca-104">deviceCompliancePolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="e54ca-104">deviceCompliancePolicy resource type</span></span>

> <span data-ttu-id="e54ca-105">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="e54ca-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e54ca-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e54ca-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e54ca-107">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e54ca-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e54ca-108">这是符合性策略的基类。</span><span class="sxs-lookup"><span data-stu-id="e54ca-108">This is the base class for Compliance policy.</span></span> <span data-ttu-id="e54ca-109">符合性策略特定于平台，每个平台的符合性策略相互独立，且继承自此处。</span><span class="sxs-lookup"><span data-stu-id="e54ca-109">Compliance policies are platform specific and individual per-platform compliance policies inherit from here.</span></span> 

## <a name="methods"></a><span data-ttu-id="e54ca-110">方法</span><span class="sxs-lookup"><span data-stu-id="e54ca-110">Methods</span></span>
|<span data-ttu-id="e54ca-111">方法</span><span class="sxs-lookup"><span data-stu-id="e54ca-111">Method</span></span>|<span data-ttu-id="e54ca-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="e54ca-112">Return Type</span></span>|<span data-ttu-id="e54ca-113">说明</span><span class="sxs-lookup"><span data-stu-id="e54ca-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e54ca-114">List deviceCompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="e54ca-114">List deviceCompliancePolicies</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-list.md)|<span data-ttu-id="e54ca-115">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e54ca-115">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) collection</span></span>|<span data-ttu-id="e54ca-116">列出 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e54ca-116">List properties and relationships of the [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) objects.</span></span>|
|[<span data-ttu-id="e54ca-117">Get deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="e54ca-117">Get deviceCompliancePolicy</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-get.md)|[<span data-ttu-id="e54ca-118">deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="e54ca-118">deviceCompliancePolicy</span></span>](../resources/intune-deviceconfig-devicecompliancepolicy.md)|<span data-ttu-id="e54ca-119">读取 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e54ca-119">Read properties and relationships of the [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) object.</span></span>|
|[<span data-ttu-id="e54ca-120">assign 操作</span><span class="sxs-lookup"><span data-stu-id="e54ca-120">assign action</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-assign.md)|<span data-ttu-id="e54ca-121">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e54ca-121">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="e54ca-122">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e54ca-122">Not yet documented</span></span>|
|[<span data-ttu-id="e54ca-123">scheduleActionsForRules 操作</span><span class="sxs-lookup"><span data-stu-id="e54ca-123">scheduleActionsForRules action</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-scheduleactionsforrules.md)|<span data-ttu-id="e54ca-124">无</span><span class="sxs-lookup"><span data-stu-id="e54ca-124">None</span></span>|<span data-ttu-id="e54ca-125">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e54ca-125">Not yet documented</span></span>|
|[<span data-ttu-id="e54ca-126">refreshDeviceComplianceReportSummarization 操作</span><span class="sxs-lookup"><span data-stu-id="e54ca-126">refreshDeviceComplianceReportSummarization action</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-refreshdevicecompliancereportsummarization.md)|<span data-ttu-id="e54ca-127">无</span><span class="sxs-lookup"><span data-stu-id="e54ca-127">None</span></span>|<span data-ttu-id="e54ca-128">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e54ca-128">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="e54ca-129">属性</span><span class="sxs-lookup"><span data-stu-id="e54ca-129">Properties</span></span>
|<span data-ttu-id="e54ca-130">属性</span><span class="sxs-lookup"><span data-stu-id="e54ca-130">Property</span></span>|<span data-ttu-id="e54ca-131">类型</span><span class="sxs-lookup"><span data-stu-id="e54ca-131">Type</span></span>|<span data-ttu-id="e54ca-132">说明</span><span class="sxs-lookup"><span data-stu-id="e54ca-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e54ca-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e54ca-133">roleScopeTagIds</span></span>|<span data-ttu-id="e54ca-134">String 集合</span><span class="sxs-lookup"><span data-stu-id="e54ca-134">String collection</span></span>|<span data-ttu-id="e54ca-135">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="e54ca-135">List of Scope Tags for this Entity instance.</span></span>|
|<span data-ttu-id="e54ca-136">id</span><span class="sxs-lookup"><span data-stu-id="e54ca-136">id</span></span>|<span data-ttu-id="e54ca-137">String</span><span class="sxs-lookup"><span data-stu-id="e54ca-137">String</span></span>|<span data-ttu-id="e54ca-138">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e54ca-138">Key of the entity.</span></span>|
|<span data-ttu-id="e54ca-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e54ca-139">createdDateTime</span></span>|<span data-ttu-id="e54ca-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e54ca-140">DateTimeOffset</span></span>|<span data-ttu-id="e54ca-141">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="e54ca-141">DateTime the object was created.</span></span>|
|<span data-ttu-id="e54ca-142">description</span><span class="sxs-lookup"><span data-stu-id="e54ca-142">description</span></span>|<span data-ttu-id="e54ca-143">String</span><span class="sxs-lookup"><span data-stu-id="e54ca-143">String</span></span>|<span data-ttu-id="e54ca-144">管理员提供的设备配置说明。</span><span class="sxs-lookup"><span data-stu-id="e54ca-144">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="e54ca-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e54ca-145">lastModifiedDateTime</span></span>|<span data-ttu-id="e54ca-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e54ca-146">DateTimeOffset</span></span>|<span data-ttu-id="e54ca-147">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="e54ca-147">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="e54ca-148">displayName</span><span class="sxs-lookup"><span data-stu-id="e54ca-148">displayName</span></span>|<span data-ttu-id="e54ca-149">String</span><span class="sxs-lookup"><span data-stu-id="e54ca-149">String</span></span>|<span data-ttu-id="e54ca-150">管理员提供的设备配置名称。</span><span class="sxs-lookup"><span data-stu-id="e54ca-150">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="e54ca-151">version</span><span class="sxs-lookup"><span data-stu-id="e54ca-151">version</span></span>|<span data-ttu-id="e54ca-152">Int32</span><span class="sxs-lookup"><span data-stu-id="e54ca-152">Int32</span></span>|<span data-ttu-id="e54ca-153">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="e54ca-153">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e54ca-154">关系</span><span class="sxs-lookup"><span data-stu-id="e54ca-154">Relationships</span></span>
|<span data-ttu-id="e54ca-155">关系</span><span class="sxs-lookup"><span data-stu-id="e54ca-155">Relationship</span></span>|<span data-ttu-id="e54ca-156">类型</span><span class="sxs-lookup"><span data-stu-id="e54ca-156">Type</span></span>|<span data-ttu-id="e54ca-157">说明</span><span class="sxs-lookup"><span data-stu-id="e54ca-157">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e54ca-158">scheduledActionsForRule</span><span class="sxs-lookup"><span data-stu-id="e54ca-158">scheduledActionsForRule</span></span>|<span data-ttu-id="e54ca-159">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e54ca-159">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) collection</span></span>|<span data-ttu-id="e54ca-160">此规则的计划操作列表</span><span class="sxs-lookup"><span data-stu-id="e54ca-160">The list of scheduled action for this rule</span></span>|
|<span data-ttu-id="e54ca-161">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="e54ca-161">deviceStatuses</span></span>|<span data-ttu-id="e54ca-162">[deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e54ca-162">[deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) collection</span></span>|<span data-ttu-id="e54ca-163">DeviceComplianceDeviceStatus 的列表。</span><span class="sxs-lookup"><span data-stu-id="e54ca-163">List of DeviceComplianceDeviceStatus.</span></span>|
|<span data-ttu-id="e54ca-164">userStatuses</span><span class="sxs-lookup"><span data-stu-id="e54ca-164">userStatuses</span></span>|<span data-ttu-id="e54ca-165">[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e54ca-165">[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) collection</span></span>|<span data-ttu-id="e54ca-166">DeviceComplianceUserStatus 的列表。</span><span class="sxs-lookup"><span data-stu-id="e54ca-166">List of DeviceComplianceUserStatus.</span></span>|
|<span data-ttu-id="e54ca-167">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="e54ca-167">deviceStatusOverview</span></span>|[<span data-ttu-id="e54ca-168">deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="e54ca-168">deviceComplianceDeviceOverview</span></span>](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md)|<span data-ttu-id="e54ca-169">设备符合性设备状态概述</span><span class="sxs-lookup"><span data-stu-id="e54ca-169">Device compliance devices status overview</span></span>|
|<span data-ttu-id="e54ca-170">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="e54ca-170">userStatusOverview</span></span>|[<span data-ttu-id="e54ca-171">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="e54ca-171">deviceComplianceUserOverview</span></span>](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|<span data-ttu-id="e54ca-172">设备符合性用户状态概述</span><span class="sxs-lookup"><span data-stu-id="e54ca-172">Device compliance users status overview</span></span>|
|<span data-ttu-id="e54ca-173">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="e54ca-173">deviceSettingStateSummaries</span></span>|<span data-ttu-id="e54ca-174">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e54ca-174">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="e54ca-175">符合性设置状态设备摘要</span><span class="sxs-lookup"><span data-stu-id="e54ca-175">Compliance Setting State Device Summary</span></span>|
|<span data-ttu-id="e54ca-176">assignments</span><span class="sxs-lookup"><span data-stu-id="e54ca-176">assignments</span></span>|<span data-ttu-id="e54ca-177">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e54ca-177">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="e54ca-178">此符合性策略的分配集合。</span><span class="sxs-lookup"><span data-stu-id="e54ca-178">The collection of assignments for this compliance policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e54ca-179">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e54ca-179">JSON Representation</span></span>
<span data-ttu-id="e54ca-180">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e54ca-180">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCompliancePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicy",
  "roleScopeTagIds": [
    "String"
  ],
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024
}
```




