---
title: deviceCompliancePolicy 资源类型
description: '这是符合性策略的基类。 符合性策略特定于平台，每个平台的符合性策略相互独立，且继承自此处。 '
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d63870ea018261e044aa01129416bb55278d8963
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42771339"
---
# <a name="devicecompliancepolicy-resource-type"></a><span data-ttu-id="a6cc0-104">deviceCompliancePolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="a6cc0-104">deviceCompliancePolicy resource type</span></span>

> <span data-ttu-id="a6cc0-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a6cc0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a6cc0-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a6cc0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6cc0-107">这是符合性策略的基类。</span><span class="sxs-lookup"><span data-stu-id="a6cc0-107">This is the base class for Compliance policy.</span></span> <span data-ttu-id="a6cc0-108">符合性策略特定于平台，每个平台的符合性策略相互独立，且继承自此处。</span><span class="sxs-lookup"><span data-stu-id="a6cc0-108">Compliance policies are platform specific and individual per-platform compliance policies inherit from here.</span></span> 

## <a name="methods"></a><span data-ttu-id="a6cc0-109">方法</span><span class="sxs-lookup"><span data-stu-id="a6cc0-109">Methods</span></span>
|<span data-ttu-id="a6cc0-110">方法</span><span class="sxs-lookup"><span data-stu-id="a6cc0-110">Method</span></span>|<span data-ttu-id="a6cc0-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="a6cc0-111">Return Type</span></span>|<span data-ttu-id="a6cc0-112">说明</span><span class="sxs-lookup"><span data-stu-id="a6cc0-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a6cc0-113">List deviceCompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="a6cc0-113">List deviceCompliancePolicies</span></span>](../api/intune-shared-devicecompliancepolicy-list.md)|<span data-ttu-id="a6cc0-114">[deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a6cc0-114">[deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md) collection</span></span>|<span data-ttu-id="a6cc0-115">列出 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a6cc0-115">List properties and relationships of the [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md) objects.</span></span>|
|[<span data-ttu-id="a6cc0-116">Get deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="a6cc0-116">Get deviceCompliancePolicy</span></span>](../api/intune-shared-devicecompliancepolicy-get.md)|[<span data-ttu-id="a6cc0-117">deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="a6cc0-117">deviceCompliancePolicy</span></span>](../resources/intune-shared-devicecompliancepolicy.md)|<span data-ttu-id="a6cc0-118">读取 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a6cc0-118">Read properties and relationships of the [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md) object.</span></span>|
|<span data-ttu-id="a6cc0-119">**设备配置**</span><span class="sxs-lookup"><span data-stu-id="a6cc0-119">**Device configuration**</span></span>|
|[<span data-ttu-id="a6cc0-120">assign 操作</span><span class="sxs-lookup"><span data-stu-id="a6cc0-120">assign action</span></span>](../api/intune-shared-devicecompliancepolicy-assign.md)|<span data-ttu-id="a6cc0-121">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a6cc0-121">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="a6cc0-122">尚未记录</span><span class="sxs-lookup"><span data-stu-id="a6cc0-122">Not yet documented</span></span>|
|<span data-ttu-id="a6cc0-123">scheduleActionsForRules 操作</span><span class="sxs-lookup"><span data-stu-id="a6cc0-123">scheduleActionsForRules action</span></span>|<span data-ttu-id="a6cc0-124">无</span><span class="sxs-lookup"><span data-stu-id="a6cc0-124">None</span></span>|<span data-ttu-id="a6cc0-125">尚未记录</span><span class="sxs-lookup"><span data-stu-id="a6cc0-125">Not yet documented</span></span>|
|<span data-ttu-id="a6cc0-126">refreshDeviceComplianceReportSummarization 操作] （.。。/api/intune-shared-devicecompliancepolicy-refreshdevicecompliancereportsummarization.md)</span><span class="sxs-lookup"><span data-stu-id="a6cc0-126">refreshDeviceComplianceReportSummarization action](../api/intune-shared-devicecompliancepolicy-refreshdevicecompliancereportsummarization.md)</span></span>|<span data-ttu-id="a6cc0-127">无</span><span class="sxs-lookup"><span data-stu-id="a6cc0-127">None</span></span>|<span data-ttu-id="a6cc0-128">尚未记录</span><span class="sxs-lookup"><span data-stu-id="a6cc0-128">Not yet documented</span></span>|
|<span data-ttu-id="a6cc0-129">**策略集**</span><span class="sxs-lookup"><span data-stu-id="a6cc0-129">**Policy Set**</span></span>|
|[<span data-ttu-id="a6cc0-130">hasPayloadLinks 操作</span><span class="sxs-lookup"><span data-stu-id="a6cc0-130">hasPayloadLinks action</span></span>](../api/intune-shared-devicecompliancepolicy-haspayloadlinks.md)|<span data-ttu-id="a6cc0-131">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="a6cc0-131">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) collection</span></span>|<span data-ttu-id="a6cc0-132">尚未记录</span><span class="sxs-lookup"><span data-stu-id="a6cc0-132">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="a6cc0-133">属性</span><span class="sxs-lookup"><span data-stu-id="a6cc0-133">Properties</span></span>
|<span data-ttu-id="a6cc0-134">属性</span><span class="sxs-lookup"><span data-stu-id="a6cc0-134">Property</span></span>|<span data-ttu-id="a6cc0-135">类型</span><span class="sxs-lookup"><span data-stu-id="a6cc0-135">Type</span></span>|<span data-ttu-id="a6cc0-136">说明</span><span class="sxs-lookup"><span data-stu-id="a6cc0-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6cc0-137">id</span><span class="sxs-lookup"><span data-stu-id="a6cc0-137">id</span></span>|<span data-ttu-id="a6cc0-138">字符串</span><span class="sxs-lookup"><span data-stu-id="a6cc0-138">String</span></span>|<span data-ttu-id="a6cc0-139">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a6cc0-139">Key of the entity.</span></span>|
|<span data-ttu-id="a6cc0-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a6cc0-140">roleScopeTagIds</span></span>|<span data-ttu-id="a6cc0-141">String collection</span><span class="sxs-lookup"><span data-stu-id="a6cc0-141">String collection</span></span>|<span data-ttu-id="a6cc0-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="a6cc0-142">List of Scope Tags for this Entity instance.</span></span>|
|<span data-ttu-id="a6cc0-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a6cc0-143">createdDateTime</span></span>|<span data-ttu-id="a6cc0-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a6cc0-144">DateTimeOffset</span></span>|<span data-ttu-id="a6cc0-145">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="a6cc0-145">DateTime the object was created.</span></span>|
|<span data-ttu-id="a6cc0-146">说明</span><span class="sxs-lookup"><span data-stu-id="a6cc0-146">description</span></span>|<span data-ttu-id="a6cc0-147">String</span><span class="sxs-lookup"><span data-stu-id="a6cc0-147">String</span></span>|<span data-ttu-id="a6cc0-148">管理员提供的设备配置说明。</span><span class="sxs-lookup"><span data-stu-id="a6cc0-148">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="a6cc0-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a6cc0-149">lastModifiedDateTime</span></span>|<span data-ttu-id="a6cc0-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a6cc0-150">DateTimeOffset</span></span>|<span data-ttu-id="a6cc0-151">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="a6cc0-151">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="a6cc0-152">displayName</span><span class="sxs-lookup"><span data-stu-id="a6cc0-152">displayName</span></span>|<span data-ttu-id="a6cc0-153">String</span><span class="sxs-lookup"><span data-stu-id="a6cc0-153">String</span></span>|<span data-ttu-id="a6cc0-154">管理员提供的设备配置名称。</span><span class="sxs-lookup"><span data-stu-id="a6cc0-154">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="a6cc0-155">version</span><span class="sxs-lookup"><span data-stu-id="a6cc0-155">version</span></span>|<span data-ttu-id="a6cc0-156">Int32</span><span class="sxs-lookup"><span data-stu-id="a6cc0-156">Int32</span></span>|<span data-ttu-id="a6cc0-157">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="a6cc0-157">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a6cc0-158">关系</span><span class="sxs-lookup"><span data-stu-id="a6cc0-158">Relationships</span></span>
|<span data-ttu-id="a6cc0-159">关系</span><span class="sxs-lookup"><span data-stu-id="a6cc0-159">Relationship</span></span>|<span data-ttu-id="a6cc0-160">类型</span><span class="sxs-lookup"><span data-stu-id="a6cc0-160">Type</span></span>|<span data-ttu-id="a6cc0-161">说明</span><span class="sxs-lookup"><span data-stu-id="a6cc0-161">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6cc0-162">**设备配置**</span><span class="sxs-lookup"><span data-stu-id="a6cc0-162">**Device configuration**</span></span>|
|<span data-ttu-id="a6cc0-163">scheduledActionsForRule</span><span class="sxs-lookup"><span data-stu-id="a6cc0-163">scheduledActionsForRule</span></span>|<span data-ttu-id="a6cc0-164">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a6cc0-164">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) collection</span></span>|<span data-ttu-id="a6cc0-165">此规则的计划操作列表</span><span class="sxs-lookup"><span data-stu-id="a6cc0-165">The list of scheduled action for this rule</span></span>|
|<span data-ttu-id="a6cc0-166">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="a6cc0-166">deviceStatuses</span></span>|<span data-ttu-id="a6cc0-167">[deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a6cc0-167">[deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) collection</span></span>|<span data-ttu-id="a6cc0-168">DeviceComplianceDeviceStatus 的列表。</span><span class="sxs-lookup"><span data-stu-id="a6cc0-168">List of DeviceComplianceDeviceStatus.</span></span>|
|<span data-ttu-id="a6cc0-169">userStatuses</span><span class="sxs-lookup"><span data-stu-id="a6cc0-169">userStatuses</span></span>|<span data-ttu-id="a6cc0-170">[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a6cc0-170">[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) collection</span></span>|<span data-ttu-id="a6cc0-171">DeviceComplianceUserStatus 的列表。</span><span class="sxs-lookup"><span data-stu-id="a6cc0-171">List of DeviceComplianceUserStatus.</span></span>|
|<span data-ttu-id="a6cc0-172">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="a6cc0-172">deviceStatusOverview</span></span>|[<span data-ttu-id="a6cc0-173">deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="a6cc0-173">deviceComplianceDeviceOverview</span></span>](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md)|<span data-ttu-id="a6cc0-174">设备符合性设备状态概述</span><span class="sxs-lookup"><span data-stu-id="a6cc0-174">Device compliance devices status overview</span></span>|
|<span data-ttu-id="a6cc0-175">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="a6cc0-175">userStatusOverview</span></span>|[<span data-ttu-id="a6cc0-176">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="a6cc0-176">deviceComplianceUserOverview</span></span>](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|<span data-ttu-id="a6cc0-177">设备符合性用户状态概述</span><span class="sxs-lookup"><span data-stu-id="a6cc0-177">Device compliance users status overview</span></span>|
|<span data-ttu-id="a6cc0-178">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="a6cc0-178">deviceSettingStateSummaries</span></span>|<span data-ttu-id="a6cc0-179">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a6cc0-179">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="a6cc0-180">符合性设置状态设备摘要</span><span class="sxs-lookup"><span data-stu-id="a6cc0-180">Compliance Setting State Device Summary</span></span>|
|<span data-ttu-id="a6cc0-181">assignments</span><span class="sxs-lookup"><span data-stu-id="a6cc0-181">assignments</span></span>|<span data-ttu-id="a6cc0-182">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a6cc0-182">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="a6cc0-183">此符合性策略的分配集合。</span><span class="sxs-lookup"><span data-stu-id="a6cc0-183">The collection of assignments for this compliance policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a6cc0-184">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a6cc0-184">JSON Representation</span></span>
<span data-ttu-id="a6cc0-185">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a6cc0-185">Here is a JSON representation of the resource.</span></span>
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



