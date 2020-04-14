---
title: deviceCompliancePolicy 资源类型
description: '这是符合性策略的基类。 符合性策略特定于平台，每个平台的符合性策略相互独立，且继承自此处。 '
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c3ae4adc329d09002b0eeb6e8c9d4112fa22d6eb
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43443615"
---
# <a name="devicecompliancepolicy-resource-type"></a><span data-ttu-id="482a5-104">deviceCompliancePolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="482a5-104">deviceCompliancePolicy resource type</span></span>

<span data-ttu-id="482a5-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="482a5-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="482a5-106">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="482a5-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="482a5-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="482a5-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="482a5-108">这是符合性策略的基类。</span><span class="sxs-lookup"><span data-stu-id="482a5-108">This is the base class for Compliance policy.</span></span> <span data-ttu-id="482a5-109">符合性策略特定于平台，每个平台的符合性策略相互独立，且继承自此处。</span><span class="sxs-lookup"><span data-stu-id="482a5-109">Compliance policies are platform specific and individual per-platform compliance policies inherit from here.</span></span> 

## <a name="methods"></a><span data-ttu-id="482a5-110">方法</span><span class="sxs-lookup"><span data-stu-id="482a5-110">Methods</span></span>
|<span data-ttu-id="482a5-111">方法</span><span class="sxs-lookup"><span data-stu-id="482a5-111">Method</span></span>|<span data-ttu-id="482a5-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="482a5-112">Return Type</span></span>|<span data-ttu-id="482a5-113">说明</span><span class="sxs-lookup"><span data-stu-id="482a5-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="482a5-114">List deviceCompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="482a5-114">List deviceCompliancePolicies</span></span>](../api/intune-shared-devicecompliancepolicy-list.md)|<span data-ttu-id="482a5-115">[deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="482a5-115">[deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md) collection</span></span>|<span data-ttu-id="482a5-116">列出 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="482a5-116">List properties and relationships of the [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md) objects.</span></span>|
|[<span data-ttu-id="482a5-117">Get deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="482a5-117">Get deviceCompliancePolicy</span></span>](../api/intune-shared-devicecompliancepolicy-get.md)|[<span data-ttu-id="482a5-118">deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="482a5-118">deviceCompliancePolicy</span></span>](../resources/intune-shared-devicecompliancepolicy.md)|<span data-ttu-id="482a5-119">读取 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="482a5-119">Read properties and relationships of the [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md) object.</span></span>|
|<span data-ttu-id="482a5-120">**设备配置**</span><span class="sxs-lookup"><span data-stu-id="482a5-120">**Device configuration**</span></span>|
|[<span data-ttu-id="482a5-121">assign 操作</span><span class="sxs-lookup"><span data-stu-id="482a5-121">assign action</span></span>](../api/intune-shared-devicecompliancepolicy-assign.md)|<span data-ttu-id="482a5-122">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="482a5-122">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="482a5-123">尚未记录</span><span class="sxs-lookup"><span data-stu-id="482a5-123">Not yet documented</span></span>|
|<span data-ttu-id="482a5-124">scheduleActionsForRules 操作</span><span class="sxs-lookup"><span data-stu-id="482a5-124">scheduleActionsForRules action</span></span>|<span data-ttu-id="482a5-125">无</span><span class="sxs-lookup"><span data-stu-id="482a5-125">None</span></span>|<span data-ttu-id="482a5-126">尚未记录</span><span class="sxs-lookup"><span data-stu-id="482a5-126">Not yet documented</span></span>|
|<span data-ttu-id="482a5-127">refreshDeviceComplianceReportSummarization 操作] （.。。/api/intune-shared-devicecompliancepolicy-refreshdevicecompliancereportsummarization.md)</span><span class="sxs-lookup"><span data-stu-id="482a5-127">refreshDeviceComplianceReportSummarization action](../api/intune-shared-devicecompliancepolicy-refreshdevicecompliancereportsummarization.md)</span></span>|<span data-ttu-id="482a5-128">无</span><span class="sxs-lookup"><span data-stu-id="482a5-128">None</span></span>|<span data-ttu-id="482a5-129">尚未记录</span><span class="sxs-lookup"><span data-stu-id="482a5-129">Not yet documented</span></span>|
|<span data-ttu-id="482a5-130">**策略集**</span><span class="sxs-lookup"><span data-stu-id="482a5-130">**Policy Set**</span></span>|
|[<span data-ttu-id="482a5-131">hasPayloadLinks 操作</span><span class="sxs-lookup"><span data-stu-id="482a5-131">hasPayloadLinks action</span></span>](../api/intune-shared-devicecompliancepolicy-haspayloadlinks.md)|<span data-ttu-id="482a5-132">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="482a5-132">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) collection</span></span>|<span data-ttu-id="482a5-133">尚未记录</span><span class="sxs-lookup"><span data-stu-id="482a5-133">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="482a5-134">属性</span><span class="sxs-lookup"><span data-stu-id="482a5-134">Properties</span></span>
|<span data-ttu-id="482a5-135">属性</span><span class="sxs-lookup"><span data-stu-id="482a5-135">Property</span></span>|<span data-ttu-id="482a5-136">类型</span><span class="sxs-lookup"><span data-stu-id="482a5-136">Type</span></span>|<span data-ttu-id="482a5-137">说明</span><span class="sxs-lookup"><span data-stu-id="482a5-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="482a5-138">id</span><span class="sxs-lookup"><span data-stu-id="482a5-138">id</span></span>|<span data-ttu-id="482a5-139">字符串</span><span class="sxs-lookup"><span data-stu-id="482a5-139">String</span></span>|<span data-ttu-id="482a5-140">实体的键。</span><span class="sxs-lookup"><span data-stu-id="482a5-140">Key of the entity.</span></span>|
|<span data-ttu-id="482a5-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="482a5-141">roleScopeTagIds</span></span>|<span data-ttu-id="482a5-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="482a5-142">String collection</span></span>|<span data-ttu-id="482a5-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="482a5-143">List of Scope Tags for this Entity instance.</span></span>|
|<span data-ttu-id="482a5-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="482a5-144">createdDateTime</span></span>|<span data-ttu-id="482a5-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="482a5-145">DateTimeOffset</span></span>|<span data-ttu-id="482a5-146">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="482a5-146">DateTime the object was created.</span></span>|
|<span data-ttu-id="482a5-147">description</span><span class="sxs-lookup"><span data-stu-id="482a5-147">description</span></span>|<span data-ttu-id="482a5-148">String</span><span class="sxs-lookup"><span data-stu-id="482a5-148">String</span></span>|<span data-ttu-id="482a5-149">管理员提供的设备配置说明。</span><span class="sxs-lookup"><span data-stu-id="482a5-149">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="482a5-150">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="482a5-150">lastModifiedDateTime</span></span>|<span data-ttu-id="482a5-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="482a5-151">DateTimeOffset</span></span>|<span data-ttu-id="482a5-152">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="482a5-152">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="482a5-153">displayName</span><span class="sxs-lookup"><span data-stu-id="482a5-153">displayName</span></span>|<span data-ttu-id="482a5-154">String</span><span class="sxs-lookup"><span data-stu-id="482a5-154">String</span></span>|<span data-ttu-id="482a5-155">管理员提供的设备配置名称。</span><span class="sxs-lookup"><span data-stu-id="482a5-155">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="482a5-156">version</span><span class="sxs-lookup"><span data-stu-id="482a5-156">version</span></span>|<span data-ttu-id="482a5-157">Int32</span><span class="sxs-lookup"><span data-stu-id="482a5-157">Int32</span></span>|<span data-ttu-id="482a5-158">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="482a5-158">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="482a5-159">关系</span><span class="sxs-lookup"><span data-stu-id="482a5-159">Relationships</span></span>
|<span data-ttu-id="482a5-160">关系</span><span class="sxs-lookup"><span data-stu-id="482a5-160">Relationship</span></span>|<span data-ttu-id="482a5-161">类型</span><span class="sxs-lookup"><span data-stu-id="482a5-161">Type</span></span>|<span data-ttu-id="482a5-162">说明</span><span class="sxs-lookup"><span data-stu-id="482a5-162">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="482a5-163">**设备配置**</span><span class="sxs-lookup"><span data-stu-id="482a5-163">**Device configuration**</span></span>|
|<span data-ttu-id="482a5-164">scheduledActionsForRule</span><span class="sxs-lookup"><span data-stu-id="482a5-164">scheduledActionsForRule</span></span>|<span data-ttu-id="482a5-165">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="482a5-165">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) collection</span></span>|<span data-ttu-id="482a5-166">此规则的计划操作列表</span><span class="sxs-lookup"><span data-stu-id="482a5-166">The list of scheduled action for this rule</span></span>|
|<span data-ttu-id="482a5-167">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="482a5-167">deviceStatuses</span></span>|<span data-ttu-id="482a5-168">[deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="482a5-168">[deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) collection</span></span>|<span data-ttu-id="482a5-169">DeviceComplianceDeviceStatus 的列表。</span><span class="sxs-lookup"><span data-stu-id="482a5-169">List of DeviceComplianceDeviceStatus.</span></span>|
|<span data-ttu-id="482a5-170">userStatuses</span><span class="sxs-lookup"><span data-stu-id="482a5-170">userStatuses</span></span>|<span data-ttu-id="482a5-171">[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="482a5-171">[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) collection</span></span>|<span data-ttu-id="482a5-172">DeviceComplianceUserStatus 的列表。</span><span class="sxs-lookup"><span data-stu-id="482a5-172">List of DeviceComplianceUserStatus.</span></span>|
|<span data-ttu-id="482a5-173">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="482a5-173">deviceStatusOverview</span></span>|[<span data-ttu-id="482a5-174">deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="482a5-174">deviceComplianceDeviceOverview</span></span>](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md)|<span data-ttu-id="482a5-175">设备符合性设备状态概述</span><span class="sxs-lookup"><span data-stu-id="482a5-175">Device compliance devices status overview</span></span>|
|<span data-ttu-id="482a5-176">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="482a5-176">userStatusOverview</span></span>|[<span data-ttu-id="482a5-177">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="482a5-177">deviceComplianceUserOverview</span></span>](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|<span data-ttu-id="482a5-178">设备符合性用户状态概述</span><span class="sxs-lookup"><span data-stu-id="482a5-178">Device compliance users status overview</span></span>|
|<span data-ttu-id="482a5-179">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="482a5-179">deviceSettingStateSummaries</span></span>|<span data-ttu-id="482a5-180">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="482a5-180">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="482a5-181">符合性设置状态设备摘要</span><span class="sxs-lookup"><span data-stu-id="482a5-181">Compliance Setting State Device Summary</span></span>|
|<span data-ttu-id="482a5-182">assignments</span><span class="sxs-lookup"><span data-stu-id="482a5-182">assignments</span></span>|<span data-ttu-id="482a5-183">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="482a5-183">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="482a5-184">此符合性策略的分配集合。</span><span class="sxs-lookup"><span data-stu-id="482a5-184">The collection of assignments for this compliance policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="482a5-185">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="482a5-185">JSON Representation</span></span>
<span data-ttu-id="482a5-186">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="482a5-186">Here is a JSON representation of the resource.</span></span>
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



