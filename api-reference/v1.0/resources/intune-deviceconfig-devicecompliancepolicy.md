---
title: deviceCompliancePolicy 资源类型
description: '这是符合性策略的基类。 符合性策略特定于平台，每个平台的符合性策略相互独立，且继承自此处。 '
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 68fdc729baae64790e19b6956653c45e64137332
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532611"
---
# <a name="devicecompliancepolicy-resource-type"></a><span data-ttu-id="f2229-104">deviceCompliancePolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="f2229-104">deviceCompliancePolicy resource type</span></span>

<span data-ttu-id="f2229-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2229-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f2229-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f2229-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f2229-107">这是符合性策略的基类。</span><span class="sxs-lookup"><span data-stu-id="f2229-107">This is the base class for Compliance policy.</span></span> <span data-ttu-id="f2229-108">符合性策略特定于平台，每个平台的符合性策略相互独立，且继承自此处。</span><span class="sxs-lookup"><span data-stu-id="f2229-108">Compliance policies are platform specific and individual per-platform compliance policies inherit from here.</span></span> 

## <a name="methods"></a><span data-ttu-id="f2229-109">Methods</span><span class="sxs-lookup"><span data-stu-id="f2229-109">Methods</span></span>
|<span data-ttu-id="f2229-110">方法</span><span class="sxs-lookup"><span data-stu-id="f2229-110">Method</span></span>|<span data-ttu-id="f2229-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="f2229-111">Return Type</span></span>|<span data-ttu-id="f2229-112">说明</span><span class="sxs-lookup"><span data-stu-id="f2229-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f2229-113">List deviceCompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="f2229-113">List deviceCompliancePolicies</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-list.md)|<span data-ttu-id="f2229-114">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f2229-114">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) collection</span></span>|<span data-ttu-id="f2229-115">列出 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f2229-115">List properties and relationships of the [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) objects.</span></span>|
|[<span data-ttu-id="f2229-116">Get deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="f2229-116">Get deviceCompliancePolicy</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-get.md)|[<span data-ttu-id="f2229-117">deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="f2229-117">deviceCompliancePolicy</span></span>](../resources/intune-deviceconfig-devicecompliancepolicy.md)|<span data-ttu-id="f2229-118">读取 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f2229-118">Read properties and relationships of the [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) object.</span></span>|
|[<span data-ttu-id="f2229-119">assign 操作</span><span class="sxs-lookup"><span data-stu-id="f2229-119">assign action</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-assign.md)|<span data-ttu-id="f2229-120">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f2229-120">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="f2229-121">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f2229-121">Not yet documented</span></span>|
|[<span data-ttu-id="f2229-122">scheduleActionsForRules 操作</span><span class="sxs-lookup"><span data-stu-id="f2229-122">scheduleActionsForRules action</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-scheduleactionsforrules.md)|<span data-ttu-id="f2229-123">无</span><span class="sxs-lookup"><span data-stu-id="f2229-123">None</span></span>|<span data-ttu-id="f2229-124">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f2229-124">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="f2229-125">属性</span><span class="sxs-lookup"><span data-stu-id="f2229-125">Properties</span></span>
|<span data-ttu-id="f2229-126">属性</span><span class="sxs-lookup"><span data-stu-id="f2229-126">Property</span></span>|<span data-ttu-id="f2229-127">类型</span><span class="sxs-lookup"><span data-stu-id="f2229-127">Type</span></span>|<span data-ttu-id="f2229-128">说明</span><span class="sxs-lookup"><span data-stu-id="f2229-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2229-129">id</span><span class="sxs-lookup"><span data-stu-id="f2229-129">id</span></span>|<span data-ttu-id="f2229-130">字符串</span><span class="sxs-lookup"><span data-stu-id="f2229-130">String</span></span>|<span data-ttu-id="f2229-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f2229-131">Key of the entity.</span></span>|
|<span data-ttu-id="f2229-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f2229-132">createdDateTime</span></span>|<span data-ttu-id="f2229-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2229-133">DateTimeOffset</span></span>|<span data-ttu-id="f2229-134">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f2229-134">DateTime the object was created.</span></span>|
|<span data-ttu-id="f2229-135">说明</span><span class="sxs-lookup"><span data-stu-id="f2229-135">description</span></span>|<span data-ttu-id="f2229-136">String</span><span class="sxs-lookup"><span data-stu-id="f2229-136">String</span></span>|<span data-ttu-id="f2229-137">管理员提供的设备配置说明。</span><span class="sxs-lookup"><span data-stu-id="f2229-137">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="f2229-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f2229-138">lastModifiedDateTime</span></span>|<span data-ttu-id="f2229-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2229-139">DateTimeOffset</span></span>|<span data-ttu-id="f2229-140">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f2229-140">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="f2229-141">displayName</span><span class="sxs-lookup"><span data-stu-id="f2229-141">displayName</span></span>|<span data-ttu-id="f2229-142">String</span><span class="sxs-lookup"><span data-stu-id="f2229-142">String</span></span>|<span data-ttu-id="f2229-143">管理员提供的设备配置名称。</span><span class="sxs-lookup"><span data-stu-id="f2229-143">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="f2229-144">version</span><span class="sxs-lookup"><span data-stu-id="f2229-144">version</span></span>|<span data-ttu-id="f2229-145">Int32</span><span class="sxs-lookup"><span data-stu-id="f2229-145">Int32</span></span>|<span data-ttu-id="f2229-146">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="f2229-146">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f2229-147">关系</span><span class="sxs-lookup"><span data-stu-id="f2229-147">Relationships</span></span>
|<span data-ttu-id="f2229-148">关系</span><span class="sxs-lookup"><span data-stu-id="f2229-148">Relationship</span></span>|<span data-ttu-id="f2229-149">类型</span><span class="sxs-lookup"><span data-stu-id="f2229-149">Type</span></span>|<span data-ttu-id="f2229-150">说明</span><span class="sxs-lookup"><span data-stu-id="f2229-150">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2229-151">scheduledActionsForRule</span><span class="sxs-lookup"><span data-stu-id="f2229-151">scheduledActionsForRule</span></span>|<span data-ttu-id="f2229-152">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f2229-152">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) collection</span></span>|<span data-ttu-id="f2229-153">此规则的计划操作列表</span><span class="sxs-lookup"><span data-stu-id="f2229-153">The list of scheduled action for this rule</span></span>|
|<span data-ttu-id="f2229-154">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="f2229-154">deviceStatuses</span></span>|<span data-ttu-id="f2229-155">[deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f2229-155">[deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) collection</span></span>|<span data-ttu-id="f2229-156">DeviceComplianceDeviceStatus 的列表。</span><span class="sxs-lookup"><span data-stu-id="f2229-156">List of DeviceComplianceDeviceStatus.</span></span>|
|<span data-ttu-id="f2229-157">userStatuses</span><span class="sxs-lookup"><span data-stu-id="f2229-157">userStatuses</span></span>|<span data-ttu-id="f2229-158">[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f2229-158">[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) collection</span></span>|<span data-ttu-id="f2229-159">DeviceComplianceUserStatus 的列表。</span><span class="sxs-lookup"><span data-stu-id="f2229-159">List of DeviceComplianceUserStatus.</span></span>|
|<span data-ttu-id="f2229-160">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="f2229-160">deviceStatusOverview</span></span>|[<span data-ttu-id="f2229-161">deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="f2229-161">deviceComplianceDeviceOverview</span></span>](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md)|<span data-ttu-id="f2229-162">设备符合性设备状态概述</span><span class="sxs-lookup"><span data-stu-id="f2229-162">Device compliance devices status overview</span></span>|
|<span data-ttu-id="f2229-163">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="f2229-163">userStatusOverview</span></span>|[<span data-ttu-id="f2229-164">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="f2229-164">deviceComplianceUserOverview</span></span>](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|<span data-ttu-id="f2229-165">设备符合性用户状态概述</span><span class="sxs-lookup"><span data-stu-id="f2229-165">Device compliance users status overview</span></span>|
|<span data-ttu-id="f2229-166">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="f2229-166">deviceSettingStateSummaries</span></span>|<span data-ttu-id="f2229-167">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f2229-167">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="f2229-168">符合性设置状态设备摘要</span><span class="sxs-lookup"><span data-stu-id="f2229-168">Compliance Setting State Device Summary</span></span>|
|<span data-ttu-id="f2229-169">assignments</span><span class="sxs-lookup"><span data-stu-id="f2229-169">assignments</span></span>|<span data-ttu-id="f2229-170">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f2229-170">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="f2229-171">此符合性策略的分配集合。</span><span class="sxs-lookup"><span data-stu-id="f2229-171">The collection of assignments for this compliance policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f2229-172">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f2229-172">JSON Representation</span></span>
<span data-ttu-id="f2229-173">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f2229-173">Here is a JSON representation of the resource.</span></span>
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




