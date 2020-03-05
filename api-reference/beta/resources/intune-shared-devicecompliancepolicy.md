---
title: deviceCompliancePolicy 资源类型
description: '这是符合性策略的基类。 符合性策略特定于平台，每个平台的符合性策略相互独立，且继承自此处。 '
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ad5d7a521dfd9daa698af96d0b61921f09a4034a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523728"
---
# <a name="devicecompliancepolicy-resource-type"></a><span data-ttu-id="97a0a-104">deviceCompliancePolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="97a0a-104">deviceCompliancePolicy resource type</span></span>

<span data-ttu-id="97a0a-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="97a0a-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="97a0a-106">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="97a0a-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="97a0a-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="97a0a-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="97a0a-108">这是符合性策略的基类。</span><span class="sxs-lookup"><span data-stu-id="97a0a-108">This is the base class for Compliance policy.</span></span> <span data-ttu-id="97a0a-109">符合性策略特定于平台，每个平台的符合性策略相互独立，且继承自此处。</span><span class="sxs-lookup"><span data-stu-id="97a0a-109">Compliance policies are platform specific and individual per-platform compliance policies inherit from here.</span></span> 

## <a name="methods"></a><span data-ttu-id="97a0a-110">方法</span><span class="sxs-lookup"><span data-stu-id="97a0a-110">Methods</span></span>
|<span data-ttu-id="97a0a-111">方法</span><span class="sxs-lookup"><span data-stu-id="97a0a-111">Method</span></span>|<span data-ttu-id="97a0a-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="97a0a-112">Return Type</span></span>|<span data-ttu-id="97a0a-113">说明</span><span class="sxs-lookup"><span data-stu-id="97a0a-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="97a0a-114">List deviceCompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="97a0a-114">List deviceCompliancePolicies</span></span>](../api/intune-shared-devicecompliancepolicy-list.md)|<span data-ttu-id="97a0a-115">[deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="97a0a-115">[deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md) collection</span></span>|<span data-ttu-id="97a0a-116">列出 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="97a0a-116">List properties and relationships of the [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md) objects.</span></span>|
|[<span data-ttu-id="97a0a-117">Get deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="97a0a-117">Get deviceCompliancePolicy</span></span>](../api/intune-shared-devicecompliancepolicy-get.md)|[<span data-ttu-id="97a0a-118">deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="97a0a-118">deviceCompliancePolicy</span></span>](../resources/intune-shared-devicecompliancepolicy.md)|<span data-ttu-id="97a0a-119">读取 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="97a0a-119">Read properties and relationships of the [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md) object.</span></span>|
|<span data-ttu-id="97a0a-120">**设备配置**</span><span class="sxs-lookup"><span data-stu-id="97a0a-120">**Device configuration**</span></span>|
|[<span data-ttu-id="97a0a-121">assign 操作</span><span class="sxs-lookup"><span data-stu-id="97a0a-121">assign action</span></span>](../api/intune-shared-devicecompliancepolicy-assign.md)|<span data-ttu-id="97a0a-122">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="97a0a-122">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="97a0a-123">尚未记录</span><span class="sxs-lookup"><span data-stu-id="97a0a-123">Not yet documented</span></span>|
|<span data-ttu-id="97a0a-124">scheduleActionsForRules 操作</span><span class="sxs-lookup"><span data-stu-id="97a0a-124">scheduleActionsForRules action</span></span>|<span data-ttu-id="97a0a-125">无</span><span class="sxs-lookup"><span data-stu-id="97a0a-125">None</span></span>|<span data-ttu-id="97a0a-126">尚未记录</span><span class="sxs-lookup"><span data-stu-id="97a0a-126">Not yet documented</span></span>|
|<span data-ttu-id="97a0a-127">refreshDeviceComplianceReportSummarization 操作] （.。。/api/intune-shared-devicecompliancepolicy-refreshdevicecompliancereportsummarization.md)</span><span class="sxs-lookup"><span data-stu-id="97a0a-127">refreshDeviceComplianceReportSummarization action](../api/intune-shared-devicecompliancepolicy-refreshdevicecompliancereportsummarization.md)</span></span>|<span data-ttu-id="97a0a-128">无</span><span class="sxs-lookup"><span data-stu-id="97a0a-128">None</span></span>|<span data-ttu-id="97a0a-129">尚未记录</span><span class="sxs-lookup"><span data-stu-id="97a0a-129">Not yet documented</span></span>|
|<span data-ttu-id="97a0a-130">**策略集**</span><span class="sxs-lookup"><span data-stu-id="97a0a-130">**Policy Set**</span></span>|
|[<span data-ttu-id="97a0a-131">hasPayloadLinks 操作</span><span class="sxs-lookup"><span data-stu-id="97a0a-131">hasPayloadLinks action</span></span>](../api/intune-shared-devicecompliancepolicy-haspayloadlinks.md)|<span data-ttu-id="97a0a-132">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="97a0a-132">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) collection</span></span>|<span data-ttu-id="97a0a-133">尚未记录</span><span class="sxs-lookup"><span data-stu-id="97a0a-133">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="97a0a-134">属性</span><span class="sxs-lookup"><span data-stu-id="97a0a-134">Properties</span></span>
|<span data-ttu-id="97a0a-135">属性</span><span class="sxs-lookup"><span data-stu-id="97a0a-135">Property</span></span>|<span data-ttu-id="97a0a-136">类型</span><span class="sxs-lookup"><span data-stu-id="97a0a-136">Type</span></span>|<span data-ttu-id="97a0a-137">说明</span><span class="sxs-lookup"><span data-stu-id="97a0a-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97a0a-138">id</span><span class="sxs-lookup"><span data-stu-id="97a0a-138">id</span></span>|<span data-ttu-id="97a0a-139">字符串</span><span class="sxs-lookup"><span data-stu-id="97a0a-139">String</span></span>|<span data-ttu-id="97a0a-140">实体的键。</span><span class="sxs-lookup"><span data-stu-id="97a0a-140">Key of the entity.</span></span>|
|<span data-ttu-id="97a0a-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="97a0a-141">roleScopeTagIds</span></span>|<span data-ttu-id="97a0a-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="97a0a-142">String collection</span></span>|<span data-ttu-id="97a0a-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="97a0a-143">List of Scope Tags for this Entity instance.</span></span>|
|<span data-ttu-id="97a0a-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="97a0a-144">createdDateTime</span></span>|<span data-ttu-id="97a0a-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97a0a-145">DateTimeOffset</span></span>|<span data-ttu-id="97a0a-146">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="97a0a-146">DateTime the object was created.</span></span>|
|<span data-ttu-id="97a0a-147">说明</span><span class="sxs-lookup"><span data-stu-id="97a0a-147">description</span></span>|<span data-ttu-id="97a0a-148">String</span><span class="sxs-lookup"><span data-stu-id="97a0a-148">String</span></span>|<span data-ttu-id="97a0a-149">管理员提供的设备配置说明。</span><span class="sxs-lookup"><span data-stu-id="97a0a-149">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="97a0a-150">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="97a0a-150">lastModifiedDateTime</span></span>|<span data-ttu-id="97a0a-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97a0a-151">DateTimeOffset</span></span>|<span data-ttu-id="97a0a-152">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="97a0a-152">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="97a0a-153">displayName</span><span class="sxs-lookup"><span data-stu-id="97a0a-153">displayName</span></span>|<span data-ttu-id="97a0a-154">String</span><span class="sxs-lookup"><span data-stu-id="97a0a-154">String</span></span>|<span data-ttu-id="97a0a-155">管理员提供的设备配置名称。</span><span class="sxs-lookup"><span data-stu-id="97a0a-155">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="97a0a-156">version</span><span class="sxs-lookup"><span data-stu-id="97a0a-156">version</span></span>|<span data-ttu-id="97a0a-157">Int32</span><span class="sxs-lookup"><span data-stu-id="97a0a-157">Int32</span></span>|<span data-ttu-id="97a0a-158">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="97a0a-158">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="97a0a-159">关系</span><span class="sxs-lookup"><span data-stu-id="97a0a-159">Relationships</span></span>
|<span data-ttu-id="97a0a-160">关系</span><span class="sxs-lookup"><span data-stu-id="97a0a-160">Relationship</span></span>|<span data-ttu-id="97a0a-161">类型</span><span class="sxs-lookup"><span data-stu-id="97a0a-161">Type</span></span>|<span data-ttu-id="97a0a-162">说明</span><span class="sxs-lookup"><span data-stu-id="97a0a-162">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97a0a-163">**设备配置**</span><span class="sxs-lookup"><span data-stu-id="97a0a-163">**Device configuration**</span></span>|
|<span data-ttu-id="97a0a-164">scheduledActionsForRule</span><span class="sxs-lookup"><span data-stu-id="97a0a-164">scheduledActionsForRule</span></span>|<span data-ttu-id="97a0a-165">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="97a0a-165">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) collection</span></span>|<span data-ttu-id="97a0a-166">此规则的计划操作列表</span><span class="sxs-lookup"><span data-stu-id="97a0a-166">The list of scheduled action for this rule</span></span>|
|<span data-ttu-id="97a0a-167">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="97a0a-167">deviceStatuses</span></span>|<span data-ttu-id="97a0a-168">[deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="97a0a-168">[deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) collection</span></span>|<span data-ttu-id="97a0a-169">DeviceComplianceDeviceStatus 的列表。</span><span class="sxs-lookup"><span data-stu-id="97a0a-169">List of DeviceComplianceDeviceStatus.</span></span>|
|<span data-ttu-id="97a0a-170">userStatuses</span><span class="sxs-lookup"><span data-stu-id="97a0a-170">userStatuses</span></span>|<span data-ttu-id="97a0a-171">[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="97a0a-171">[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) collection</span></span>|<span data-ttu-id="97a0a-172">DeviceComplianceUserStatus 的列表。</span><span class="sxs-lookup"><span data-stu-id="97a0a-172">List of DeviceComplianceUserStatus.</span></span>|
|<span data-ttu-id="97a0a-173">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="97a0a-173">deviceStatusOverview</span></span>|[<span data-ttu-id="97a0a-174">deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="97a0a-174">deviceComplianceDeviceOverview</span></span>](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md)|<span data-ttu-id="97a0a-175">设备符合性设备状态概述</span><span class="sxs-lookup"><span data-stu-id="97a0a-175">Device compliance devices status overview</span></span>|
|<span data-ttu-id="97a0a-176">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="97a0a-176">userStatusOverview</span></span>|[<span data-ttu-id="97a0a-177">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="97a0a-177">deviceComplianceUserOverview</span></span>](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|<span data-ttu-id="97a0a-178">设备符合性用户状态概述</span><span class="sxs-lookup"><span data-stu-id="97a0a-178">Device compliance users status overview</span></span>|
|<span data-ttu-id="97a0a-179">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="97a0a-179">deviceSettingStateSummaries</span></span>|<span data-ttu-id="97a0a-180">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="97a0a-180">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="97a0a-181">符合性设置状态设备摘要</span><span class="sxs-lookup"><span data-stu-id="97a0a-181">Compliance Setting State Device Summary</span></span>|
|<span data-ttu-id="97a0a-182">assignments</span><span class="sxs-lookup"><span data-stu-id="97a0a-182">assignments</span></span>|<span data-ttu-id="97a0a-183">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="97a0a-183">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="97a0a-184">此符合性策略的分配集合。</span><span class="sxs-lookup"><span data-stu-id="97a0a-184">The collection of assignments for this compliance policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="97a0a-185">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="97a0a-185">JSON Representation</span></span>
<span data-ttu-id="97a0a-186">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="97a0a-186">Here is a JSON representation of the resource.</span></span>
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



