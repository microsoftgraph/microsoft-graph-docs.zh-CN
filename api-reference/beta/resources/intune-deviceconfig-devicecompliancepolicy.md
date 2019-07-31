---
title: deviceCompliancePolicy 资源类型
description: '这是符合性策略的基类。 符合性策略特定于平台，每个平台的符合性策略相互独立，且继承自此处。 '
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ffce3853157f5852c7ebf984ff0dfeea18fc2aef
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35970575"
---
# <a name="devicecompliancepolicy-resource-type"></a><span data-ttu-id="3c122-104">deviceCompliancePolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="3c122-104">deviceCompliancePolicy resource type</span></span>

> <span data-ttu-id="3c122-105">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3c122-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3c122-106">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3c122-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3c122-107">这是符合性策略的基类。</span><span class="sxs-lookup"><span data-stu-id="3c122-107">This is the base class for Compliance policy.</span></span> <span data-ttu-id="3c122-108">符合性策略特定于平台，每个平台的符合性策略相互独立，且继承自此处。</span><span class="sxs-lookup"><span data-stu-id="3c122-108">Compliance policies are platform specific and individual per-platform compliance policies inherit from here.</span></span> 

## <a name="methods"></a><span data-ttu-id="3c122-109">方法</span><span class="sxs-lookup"><span data-stu-id="3c122-109">Methods</span></span>
|<span data-ttu-id="3c122-110">方法</span><span class="sxs-lookup"><span data-stu-id="3c122-110">Method</span></span>|<span data-ttu-id="3c122-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="3c122-111">Return Type</span></span>|<span data-ttu-id="3c122-112">说明</span><span class="sxs-lookup"><span data-stu-id="3c122-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3c122-113">List deviceCompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="3c122-113">List deviceCompliancePolicies</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-list.md)|<span data-ttu-id="3c122-114">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3c122-114">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) collection</span></span>|<span data-ttu-id="3c122-115">列出 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3c122-115">List properties and relationships of the [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) objects.</span></span>|
|[<span data-ttu-id="3c122-116">Get deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="3c122-116">Get deviceCompliancePolicy</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-get.md)|[<span data-ttu-id="3c122-117">deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="3c122-117">deviceCompliancePolicy</span></span>](../resources/intune-deviceconfig-devicecompliancepolicy.md)|<span data-ttu-id="3c122-118">读取 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3c122-118">Read properties and relationships of the [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) object.</span></span>|
|[<span data-ttu-id="3c122-119">assign 操作</span><span class="sxs-lookup"><span data-stu-id="3c122-119">assign action</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-assign.md)|<span data-ttu-id="3c122-120">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3c122-120">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="3c122-121">尚未记录</span><span class="sxs-lookup"><span data-stu-id="3c122-121">Not yet documented</span></span>|
|[<span data-ttu-id="3c122-122">scheduleActionsForRules 操作</span><span class="sxs-lookup"><span data-stu-id="3c122-122">scheduleActionsForRules action</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-scheduleactionsforrules.md)|<span data-ttu-id="3c122-123">无</span><span class="sxs-lookup"><span data-stu-id="3c122-123">None</span></span>|<span data-ttu-id="3c122-124">尚未记录</span><span class="sxs-lookup"><span data-stu-id="3c122-124">Not yet documented</span></span>|
|[<span data-ttu-id="3c122-125">refreshDeviceComplianceReportSummarization 操作</span><span class="sxs-lookup"><span data-stu-id="3c122-125">refreshDeviceComplianceReportSummarization action</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-refreshdevicecompliancereportsummarization.md)|<span data-ttu-id="3c122-126">无</span><span class="sxs-lookup"><span data-stu-id="3c122-126">None</span></span>|<span data-ttu-id="3c122-127">尚未记录</span><span class="sxs-lookup"><span data-stu-id="3c122-127">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="3c122-128">属性</span><span class="sxs-lookup"><span data-stu-id="3c122-128">Properties</span></span>
|<span data-ttu-id="3c122-129">属性</span><span class="sxs-lookup"><span data-stu-id="3c122-129">Property</span></span>|<span data-ttu-id="3c122-130">类型</span><span class="sxs-lookup"><span data-stu-id="3c122-130">Type</span></span>|<span data-ttu-id="3c122-131">说明</span><span class="sxs-lookup"><span data-stu-id="3c122-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c122-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3c122-132">roleScopeTagIds</span></span>|<span data-ttu-id="3c122-133">String collection</span><span class="sxs-lookup"><span data-stu-id="3c122-133">String collection</span></span>|<span data-ttu-id="3c122-134">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="3c122-134">List of Scope Tags for this Entity instance.</span></span>|
|<span data-ttu-id="3c122-135">id</span><span class="sxs-lookup"><span data-stu-id="3c122-135">id</span></span>|<span data-ttu-id="3c122-136">字符串</span><span class="sxs-lookup"><span data-stu-id="3c122-136">String</span></span>|<span data-ttu-id="3c122-137">实体的键。</span><span class="sxs-lookup"><span data-stu-id="3c122-137">Key of the entity.</span></span>|
|<span data-ttu-id="3c122-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3c122-138">createdDateTime</span></span>|<span data-ttu-id="3c122-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c122-139">DateTimeOffset</span></span>|<span data-ttu-id="3c122-140">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="3c122-140">DateTime the object was created.</span></span>|
|<span data-ttu-id="3c122-141">说明</span><span class="sxs-lookup"><span data-stu-id="3c122-141">description</span></span>|<span data-ttu-id="3c122-142">String</span><span class="sxs-lookup"><span data-stu-id="3c122-142">String</span></span>|<span data-ttu-id="3c122-143">管理员提供的设备配置说明。</span><span class="sxs-lookup"><span data-stu-id="3c122-143">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="3c122-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3c122-144">lastModifiedDateTime</span></span>|<span data-ttu-id="3c122-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c122-145">DateTimeOffset</span></span>|<span data-ttu-id="3c122-146">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="3c122-146">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="3c122-147">displayName</span><span class="sxs-lookup"><span data-stu-id="3c122-147">displayName</span></span>|<span data-ttu-id="3c122-148">String</span><span class="sxs-lookup"><span data-stu-id="3c122-148">String</span></span>|<span data-ttu-id="3c122-149">管理员提供的设备配置名称。</span><span class="sxs-lookup"><span data-stu-id="3c122-149">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="3c122-150">version</span><span class="sxs-lookup"><span data-stu-id="3c122-150">version</span></span>|<span data-ttu-id="3c122-151">Int32</span><span class="sxs-lookup"><span data-stu-id="3c122-151">Int32</span></span>|<span data-ttu-id="3c122-152">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="3c122-152">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3c122-153">关系</span><span class="sxs-lookup"><span data-stu-id="3c122-153">Relationships</span></span>
|<span data-ttu-id="3c122-154">关系</span><span class="sxs-lookup"><span data-stu-id="3c122-154">Relationship</span></span>|<span data-ttu-id="3c122-155">类型</span><span class="sxs-lookup"><span data-stu-id="3c122-155">Type</span></span>|<span data-ttu-id="3c122-156">说明</span><span class="sxs-lookup"><span data-stu-id="3c122-156">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c122-157">scheduledActionsForRule</span><span class="sxs-lookup"><span data-stu-id="3c122-157">scheduledActionsForRule</span></span>|<span data-ttu-id="3c122-158">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3c122-158">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) collection</span></span>|<span data-ttu-id="3c122-159">此规则的计划操作列表</span><span class="sxs-lookup"><span data-stu-id="3c122-159">The list of scheduled action for this rule</span></span>|
|<span data-ttu-id="3c122-160">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="3c122-160">deviceStatuses</span></span>|<span data-ttu-id="3c122-161">[deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3c122-161">[deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) collection</span></span>|<span data-ttu-id="3c122-162">DeviceComplianceDeviceStatus 的列表。</span><span class="sxs-lookup"><span data-stu-id="3c122-162">List of DeviceComplianceDeviceStatus.</span></span>|
|<span data-ttu-id="3c122-163">userStatuses</span><span class="sxs-lookup"><span data-stu-id="3c122-163">userStatuses</span></span>|<span data-ttu-id="3c122-164">[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3c122-164">[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) collection</span></span>|<span data-ttu-id="3c122-165">DeviceComplianceUserStatus 的列表。</span><span class="sxs-lookup"><span data-stu-id="3c122-165">List of DeviceComplianceUserStatus.</span></span>|
|<span data-ttu-id="3c122-166">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="3c122-166">deviceStatusOverview</span></span>|[<span data-ttu-id="3c122-167">deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="3c122-167">deviceComplianceDeviceOverview</span></span>](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md)|<span data-ttu-id="3c122-168">设备符合性设备状态概述</span><span class="sxs-lookup"><span data-stu-id="3c122-168">Device compliance devices status overview</span></span>|
|<span data-ttu-id="3c122-169">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="3c122-169">userStatusOverview</span></span>|[<span data-ttu-id="3c122-170">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="3c122-170">deviceComplianceUserOverview</span></span>](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|<span data-ttu-id="3c122-171">设备符合性用户状态概述</span><span class="sxs-lookup"><span data-stu-id="3c122-171">Device compliance users status overview</span></span>|
|<span data-ttu-id="3c122-172">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="3c122-172">deviceSettingStateSummaries</span></span>|<span data-ttu-id="3c122-173">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3c122-173">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="3c122-174">符合性设置状态设备摘要</span><span class="sxs-lookup"><span data-stu-id="3c122-174">Compliance Setting State Device Summary</span></span>|
|<span data-ttu-id="3c122-175">assignments</span><span class="sxs-lookup"><span data-stu-id="3c122-175">assignments</span></span>|<span data-ttu-id="3c122-176">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3c122-176">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="3c122-177">此符合性策略的分配集合。</span><span class="sxs-lookup"><span data-stu-id="3c122-177">The collection of assignments for this compliance policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3c122-178">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3c122-178">JSON Representation</span></span>
<span data-ttu-id="3c122-179">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3c122-179">Here is a JSON representation of the resource.</span></span>
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





