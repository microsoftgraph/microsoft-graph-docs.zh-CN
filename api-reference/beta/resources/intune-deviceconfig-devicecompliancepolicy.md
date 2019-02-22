---
title: deviceCompliancePolicy 资源类型
description: '这是符合性策略的基类。 符合性策略特定于平台，每个平台的符合性策略相互独立，且继承自此处。 '
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 04138e7488925350630f7a36d743292408441bee
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30146737"
---
# <a name="devicecompliancepolicy-resource-type"></a><span data-ttu-id="ab2b7-104">deviceCompliancePolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="ab2b7-104">deviceCompliancePolicy resource type</span></span>

> <span data-ttu-id="ab2b7-105">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ab2b7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ab2b7-106">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ab2b7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ab2b7-107">这是符合性策略的基类。</span><span class="sxs-lookup"><span data-stu-id="ab2b7-107">This is the base class for Compliance policy.</span></span> <span data-ttu-id="ab2b7-108">符合性策略特定于平台，每个平台的符合性策略相互独立，且继承自此处。</span><span class="sxs-lookup"><span data-stu-id="ab2b7-108">Compliance policies are platform specific and individual per-platform compliance policies inherit from here.</span></span> 

## <a name="methods"></a><span data-ttu-id="ab2b7-109">方法</span><span class="sxs-lookup"><span data-stu-id="ab2b7-109">Methods</span></span>
|<span data-ttu-id="ab2b7-110">方法</span><span class="sxs-lookup"><span data-stu-id="ab2b7-110">Method</span></span>|<span data-ttu-id="ab2b7-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="ab2b7-111">Return Type</span></span>|<span data-ttu-id="ab2b7-112">说明</span><span class="sxs-lookup"><span data-stu-id="ab2b7-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ab2b7-113">List deviceCompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="ab2b7-113">List deviceCompliancePolicies</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-list.md)|<span data-ttu-id="ab2b7-114">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ab2b7-114">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) collection</span></span>|<span data-ttu-id="ab2b7-115">列出 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ab2b7-115">List properties and relationships of the [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) objects.</span></span>|
|[<span data-ttu-id="ab2b7-116">Get deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="ab2b7-116">Get deviceCompliancePolicy</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-get.md)|[<span data-ttu-id="ab2b7-117">deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="ab2b7-117">deviceCompliancePolicy</span></span>](../resources/intune-deviceconfig-devicecompliancepolicy.md)|<span data-ttu-id="ab2b7-118">读取 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ab2b7-118">Read properties and relationships of the [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) object.</span></span>|
|[<span data-ttu-id="ab2b7-119">assign 操作</span><span class="sxs-lookup"><span data-stu-id="ab2b7-119">assign action</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-assign.md)|<span data-ttu-id="ab2b7-120">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ab2b7-120">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="ab2b7-121">尚未记录</span><span class="sxs-lookup"><span data-stu-id="ab2b7-121">Not yet documented</span></span>|
|[<span data-ttu-id="ab2b7-122">scheduleActionsForRules 操作</span><span class="sxs-lookup"><span data-stu-id="ab2b7-122">scheduleActionsForRules action</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-scheduleactionsforrules.md)|<span data-ttu-id="ab2b7-123">无</span><span class="sxs-lookup"><span data-stu-id="ab2b7-123">None</span></span>|<span data-ttu-id="ab2b7-124">尚未记录</span><span class="sxs-lookup"><span data-stu-id="ab2b7-124">Not yet documented</span></span>|
|[<span data-ttu-id="ab2b7-125">refreshDeviceComplianceReportSummarization 操作</span><span class="sxs-lookup"><span data-stu-id="ab2b7-125">refreshDeviceComplianceReportSummarization action</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-refreshdevicecompliancereportsummarization.md)|<span data-ttu-id="ab2b7-126">无</span><span class="sxs-lookup"><span data-stu-id="ab2b7-126">None</span></span>|<span data-ttu-id="ab2b7-127">尚未记录</span><span class="sxs-lookup"><span data-stu-id="ab2b7-127">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="ab2b7-128">属性</span><span class="sxs-lookup"><span data-stu-id="ab2b7-128">Properties</span></span>
|<span data-ttu-id="ab2b7-129">属性</span><span class="sxs-lookup"><span data-stu-id="ab2b7-129">Property</span></span>|<span data-ttu-id="ab2b7-130">类型</span><span class="sxs-lookup"><span data-stu-id="ab2b7-130">Type</span></span>|<span data-ttu-id="ab2b7-131">说明</span><span class="sxs-lookup"><span data-stu-id="ab2b7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab2b7-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ab2b7-132">roleScopeTagIds</span></span>|<span data-ttu-id="ab2b7-133">String collection</span><span class="sxs-lookup"><span data-stu-id="ab2b7-133">String collection</span></span>|<span data-ttu-id="ab2b7-134">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="ab2b7-134">List of Scope Tags for this Entity instance.</span></span>|
|<span data-ttu-id="ab2b7-135">id</span><span class="sxs-lookup"><span data-stu-id="ab2b7-135">id</span></span>|<span data-ttu-id="ab2b7-136">String</span><span class="sxs-lookup"><span data-stu-id="ab2b7-136">String</span></span>|<span data-ttu-id="ab2b7-137">实体的键。</span><span class="sxs-lookup"><span data-stu-id="ab2b7-137">Key of the entity.</span></span>|
|<span data-ttu-id="ab2b7-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ab2b7-138">createdDateTime</span></span>|<span data-ttu-id="ab2b7-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ab2b7-139">DateTimeOffset</span></span>|<span data-ttu-id="ab2b7-140">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="ab2b7-140">DateTime the object was created.</span></span>|
|<span data-ttu-id="ab2b7-141">description</span><span class="sxs-lookup"><span data-stu-id="ab2b7-141">description</span></span>|<span data-ttu-id="ab2b7-142">String</span><span class="sxs-lookup"><span data-stu-id="ab2b7-142">String</span></span>|<span data-ttu-id="ab2b7-143">管理员提供的设备配置说明。</span><span class="sxs-lookup"><span data-stu-id="ab2b7-143">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="ab2b7-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ab2b7-144">lastModifiedDateTime</span></span>|<span data-ttu-id="ab2b7-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ab2b7-145">DateTimeOffset</span></span>|<span data-ttu-id="ab2b7-146">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="ab2b7-146">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="ab2b7-147">displayName</span><span class="sxs-lookup"><span data-stu-id="ab2b7-147">displayName</span></span>|<span data-ttu-id="ab2b7-148">String</span><span class="sxs-lookup"><span data-stu-id="ab2b7-148">String</span></span>|<span data-ttu-id="ab2b7-149">管理员提供的设备配置名称。</span><span class="sxs-lookup"><span data-stu-id="ab2b7-149">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="ab2b7-150">version</span><span class="sxs-lookup"><span data-stu-id="ab2b7-150">version</span></span>|<span data-ttu-id="ab2b7-151">Int32</span><span class="sxs-lookup"><span data-stu-id="ab2b7-151">Int32</span></span>|<span data-ttu-id="ab2b7-152">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="ab2b7-152">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ab2b7-153">关系</span><span class="sxs-lookup"><span data-stu-id="ab2b7-153">Relationships</span></span>
|<span data-ttu-id="ab2b7-154">关系</span><span class="sxs-lookup"><span data-stu-id="ab2b7-154">Relationship</span></span>|<span data-ttu-id="ab2b7-155">类型</span><span class="sxs-lookup"><span data-stu-id="ab2b7-155">Type</span></span>|<span data-ttu-id="ab2b7-156">说明</span><span class="sxs-lookup"><span data-stu-id="ab2b7-156">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab2b7-157">scheduledActionsForRule</span><span class="sxs-lookup"><span data-stu-id="ab2b7-157">scheduledActionsForRule</span></span>|<span data-ttu-id="ab2b7-158">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ab2b7-158">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) collection</span></span>|<span data-ttu-id="ab2b7-159">此规则的计划操作列表</span><span class="sxs-lookup"><span data-stu-id="ab2b7-159">The list of scheduled action for this rule</span></span>|
|<span data-ttu-id="ab2b7-160">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="ab2b7-160">deviceStatuses</span></span>|<span data-ttu-id="ab2b7-161">[deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ab2b7-161">[deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) collection</span></span>|<span data-ttu-id="ab2b7-162">DeviceComplianceDeviceStatus 的列表。</span><span class="sxs-lookup"><span data-stu-id="ab2b7-162">List of DeviceComplianceDeviceStatus.</span></span>|
|<span data-ttu-id="ab2b7-163">userStatuses</span><span class="sxs-lookup"><span data-stu-id="ab2b7-163">userStatuses</span></span>|<span data-ttu-id="ab2b7-164">[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ab2b7-164">[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) collection</span></span>|<span data-ttu-id="ab2b7-165">DeviceComplianceUserStatus 的列表。</span><span class="sxs-lookup"><span data-stu-id="ab2b7-165">List of DeviceComplianceUserStatus.</span></span>|
|<span data-ttu-id="ab2b7-166">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="ab2b7-166">deviceStatusOverview</span></span>|[<span data-ttu-id="ab2b7-167">deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="ab2b7-167">deviceComplianceDeviceOverview</span></span>](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md)|<span data-ttu-id="ab2b7-168">设备符合性设备状态概述</span><span class="sxs-lookup"><span data-stu-id="ab2b7-168">Device compliance devices status overview</span></span>|
|<span data-ttu-id="ab2b7-169">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="ab2b7-169">userStatusOverview</span></span>|[<span data-ttu-id="ab2b7-170">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="ab2b7-170">deviceComplianceUserOverview</span></span>](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|<span data-ttu-id="ab2b7-171">设备符合性用户状态概述</span><span class="sxs-lookup"><span data-stu-id="ab2b7-171">Device compliance users status overview</span></span>|
|<span data-ttu-id="ab2b7-172">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="ab2b7-172">deviceSettingStateSummaries</span></span>|<span data-ttu-id="ab2b7-173">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ab2b7-173">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="ab2b7-174">符合性设置状态设备摘要</span><span class="sxs-lookup"><span data-stu-id="ab2b7-174">Compliance Setting State Device Summary</span></span>|
|<span data-ttu-id="ab2b7-175">assignments</span><span class="sxs-lookup"><span data-stu-id="ab2b7-175">assignments</span></span>|<span data-ttu-id="ab2b7-176">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ab2b7-176">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="ab2b7-177">此符合性策略的分配集合。</span><span class="sxs-lookup"><span data-stu-id="ab2b7-177">The collection of assignments for this compliance policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ab2b7-178">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ab2b7-178">JSON Representation</span></span>
<span data-ttu-id="ab2b7-179">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ab2b7-179">Here is a JSON representation of the resource.</span></span>
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




