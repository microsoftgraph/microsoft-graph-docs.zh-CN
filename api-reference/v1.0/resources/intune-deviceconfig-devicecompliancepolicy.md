---
title: deviceCompliancePolicy 资源类型
description: '这是符合性策略的基类。 符合性策略特定于平台，每个平台的符合性策略相互独立，且继承自此处。 '
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e556fd8619ef16b4212711511592de2b26e4772a
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30255610"
---
# <a name="devicecompliancepolicy-resource-type"></a><span data-ttu-id="14e5e-104">deviceCompliancePolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="14e5e-104">deviceCompliancePolicy resource type</span></span>

> <span data-ttu-id="14e5e-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="14e5e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="14e5e-106">这是符合性策略的基类。</span><span class="sxs-lookup"><span data-stu-id="14e5e-106">This is the base class for Compliance policy.</span></span> <span data-ttu-id="14e5e-107">符合性策略特定于平台，每个平台的符合性策略相互独立，且继承自此处。</span><span class="sxs-lookup"><span data-stu-id="14e5e-107">Compliance policies are platform specific and individual per-platform compliance policies inherit from here.</span></span> 

## <a name="methods"></a><span data-ttu-id="14e5e-108">方法</span><span class="sxs-lookup"><span data-stu-id="14e5e-108">Methods</span></span>
|<span data-ttu-id="14e5e-109">方法</span><span class="sxs-lookup"><span data-stu-id="14e5e-109">Method</span></span>|<span data-ttu-id="14e5e-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="14e5e-110">Return Type</span></span>|<span data-ttu-id="14e5e-111">说明</span><span class="sxs-lookup"><span data-stu-id="14e5e-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="14e5e-112">List deviceCompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="14e5e-112">List deviceCompliancePolicies</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-list.md)|<span data-ttu-id="14e5e-113">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="14e5e-113">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) collection</span></span>|<span data-ttu-id="14e5e-114">列出 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="14e5e-114">List properties and relationships of the [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) objects.</span></span>|
|[<span data-ttu-id="14e5e-115">Get deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="14e5e-115">Get deviceCompliancePolicy</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-get.md)|[<span data-ttu-id="14e5e-116">deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="14e5e-116">deviceCompliancePolicy</span></span>](../resources/intune-deviceconfig-devicecompliancepolicy.md)|<span data-ttu-id="14e5e-117">读取 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="14e5e-117">Read properties and relationships of the [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) object.</span></span>|
|[<span data-ttu-id="14e5e-118">assign 操作</span><span class="sxs-lookup"><span data-stu-id="14e5e-118">assign action</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-assign.md)|<span data-ttu-id="14e5e-119">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="14e5e-119">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="14e5e-120">尚未记录</span><span class="sxs-lookup"><span data-stu-id="14e5e-120">Not yet documented</span></span>|
|[<span data-ttu-id="14e5e-121">scheduleActionsForRules 操作</span><span class="sxs-lookup"><span data-stu-id="14e5e-121">scheduleActionsForRules action</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-scheduleactionsforrules.md)|<span data-ttu-id="14e5e-122">无</span><span class="sxs-lookup"><span data-stu-id="14e5e-122">None</span></span>|<span data-ttu-id="14e5e-123">尚未记录</span><span class="sxs-lookup"><span data-stu-id="14e5e-123">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="14e5e-124">属性</span><span class="sxs-lookup"><span data-stu-id="14e5e-124">Properties</span></span>
|<span data-ttu-id="14e5e-125">属性</span><span class="sxs-lookup"><span data-stu-id="14e5e-125">Property</span></span>|<span data-ttu-id="14e5e-126">类型</span><span class="sxs-lookup"><span data-stu-id="14e5e-126">Type</span></span>|<span data-ttu-id="14e5e-127">说明</span><span class="sxs-lookup"><span data-stu-id="14e5e-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14e5e-128">id</span><span class="sxs-lookup"><span data-stu-id="14e5e-128">id</span></span>|<span data-ttu-id="14e5e-129">String</span><span class="sxs-lookup"><span data-stu-id="14e5e-129">String</span></span>|<span data-ttu-id="14e5e-130">实体的键。</span><span class="sxs-lookup"><span data-stu-id="14e5e-130">Key of the entity.</span></span>|
|<span data-ttu-id="14e5e-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="14e5e-131">createdDateTime</span></span>|<span data-ttu-id="14e5e-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="14e5e-132">DateTimeOffset</span></span>|<span data-ttu-id="14e5e-133">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="14e5e-133">DateTime the object was created.</span></span>|
|<span data-ttu-id="14e5e-134">description</span><span class="sxs-lookup"><span data-stu-id="14e5e-134">description</span></span>|<span data-ttu-id="14e5e-135">String</span><span class="sxs-lookup"><span data-stu-id="14e5e-135">String</span></span>|<span data-ttu-id="14e5e-136">管理员提供的设备配置说明。</span><span class="sxs-lookup"><span data-stu-id="14e5e-136">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="14e5e-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="14e5e-137">lastModifiedDateTime</span></span>|<span data-ttu-id="14e5e-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="14e5e-138">DateTimeOffset</span></span>|<span data-ttu-id="14e5e-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="14e5e-139">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="14e5e-140">displayName</span><span class="sxs-lookup"><span data-stu-id="14e5e-140">displayName</span></span>|<span data-ttu-id="14e5e-141">String</span><span class="sxs-lookup"><span data-stu-id="14e5e-141">String</span></span>|<span data-ttu-id="14e5e-142">管理员提供的设备配置名称。</span><span class="sxs-lookup"><span data-stu-id="14e5e-142">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="14e5e-143">version</span><span class="sxs-lookup"><span data-stu-id="14e5e-143">version</span></span>|<span data-ttu-id="14e5e-144">Int32</span><span class="sxs-lookup"><span data-stu-id="14e5e-144">Int32</span></span>|<span data-ttu-id="14e5e-145">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="14e5e-145">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="14e5e-146">关系</span><span class="sxs-lookup"><span data-stu-id="14e5e-146">Relationships</span></span>
|<span data-ttu-id="14e5e-147">关系</span><span class="sxs-lookup"><span data-stu-id="14e5e-147">Relationship</span></span>|<span data-ttu-id="14e5e-148">类型</span><span class="sxs-lookup"><span data-stu-id="14e5e-148">Type</span></span>|<span data-ttu-id="14e5e-149">说明</span><span class="sxs-lookup"><span data-stu-id="14e5e-149">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14e5e-150">scheduledActionsForRule</span><span class="sxs-lookup"><span data-stu-id="14e5e-150">scheduledActionsForRule</span></span>|<span data-ttu-id="14e5e-151">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="14e5e-151">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) collection</span></span>|<span data-ttu-id="14e5e-152">此规则的计划操作列表</span><span class="sxs-lookup"><span data-stu-id="14e5e-152">The list of scheduled action for this rule</span></span>|
|<span data-ttu-id="14e5e-153">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="14e5e-153">deviceStatuses</span></span>|<span data-ttu-id="14e5e-154">[deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="14e5e-154">[deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) collection</span></span>|<span data-ttu-id="14e5e-155">DeviceComplianceDeviceStatus 的列表。</span><span class="sxs-lookup"><span data-stu-id="14e5e-155">List of DeviceComplianceDeviceStatus.</span></span>|
|<span data-ttu-id="14e5e-156">userStatuses</span><span class="sxs-lookup"><span data-stu-id="14e5e-156">userStatuses</span></span>|<span data-ttu-id="14e5e-157">[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="14e5e-157">[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) collection</span></span>|<span data-ttu-id="14e5e-158">DeviceComplianceUserStatus 的列表。</span><span class="sxs-lookup"><span data-stu-id="14e5e-158">List of DeviceComplianceUserStatus.</span></span>|
|<span data-ttu-id="14e5e-159">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="14e5e-159">deviceStatusOverview</span></span>|[<span data-ttu-id="14e5e-160">deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="14e5e-160">deviceComplianceDeviceOverview</span></span>](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md)|<span data-ttu-id="14e5e-161">设备符合性设备状态概述</span><span class="sxs-lookup"><span data-stu-id="14e5e-161">Device compliance devices status overview</span></span>|
|<span data-ttu-id="14e5e-162">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="14e5e-162">userStatusOverview</span></span>|[<span data-ttu-id="14e5e-163">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="14e5e-163">deviceComplianceUserOverview</span></span>](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|<span data-ttu-id="14e5e-164">设备符合性用户状态概述</span><span class="sxs-lookup"><span data-stu-id="14e5e-164">Device compliance users status overview</span></span>|
|<span data-ttu-id="14e5e-165">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="14e5e-165">deviceSettingStateSummaries</span></span>|<span data-ttu-id="14e5e-166">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="14e5e-166">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="14e5e-167">符合性设置状态设备摘要</span><span class="sxs-lookup"><span data-stu-id="14e5e-167">Compliance Setting State Device Summary</span></span>|
|<span data-ttu-id="14e5e-168">assignments</span><span class="sxs-lookup"><span data-stu-id="14e5e-168">assignments</span></span>|<span data-ttu-id="14e5e-169">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="14e5e-169">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="14e5e-170">此符合性策略的分配集合。</span><span class="sxs-lookup"><span data-stu-id="14e5e-170">The collection of assignments for this compliance policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="14e5e-171">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="14e5e-171">JSON Representation</span></span>
<span data-ttu-id="14e5e-172">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="14e5e-172">Here is a JSON representation of the resource.</span></span>
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



