---
title: deviceCompliancePolicy 资源类型
description: '这是符合性策略的基类。 符合性策略特定于平台，每个平台的符合性策略相互独立，且继承自此处。 '
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e556fd8619ef16b4212711511592de2b26e4772a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534771"
---
# <a name="devicecompliancepolicy-resource-type"></a><span data-ttu-id="5c7fd-104">deviceCompliancePolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="5c7fd-104">deviceCompliancePolicy resource type</span></span>

> <span data-ttu-id="5c7fd-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5c7fd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5c7fd-106">这是符合性策略的基类。</span><span class="sxs-lookup"><span data-stu-id="5c7fd-106">This is the base class for Compliance policy.</span></span> <span data-ttu-id="5c7fd-107">符合性策略特定于平台，每个平台的符合性策略相互独立，且继承自此处。</span><span class="sxs-lookup"><span data-stu-id="5c7fd-107">Compliance policies are platform specific and individual per-platform compliance policies inherit from here.</span></span> 

## <a name="methods"></a><span data-ttu-id="5c7fd-108">方法</span><span class="sxs-lookup"><span data-stu-id="5c7fd-108">Methods</span></span>
|<span data-ttu-id="5c7fd-109">方法</span><span class="sxs-lookup"><span data-stu-id="5c7fd-109">Method</span></span>|<span data-ttu-id="5c7fd-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="5c7fd-110">Return Type</span></span>|<span data-ttu-id="5c7fd-111">说明</span><span class="sxs-lookup"><span data-stu-id="5c7fd-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5c7fd-112">List deviceCompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="5c7fd-112">List deviceCompliancePolicies</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-list.md)|<span data-ttu-id="5c7fd-113">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5c7fd-113">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) collection</span></span>|<span data-ttu-id="5c7fd-114">列出 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5c7fd-114">List properties and relationships of the [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) objects.</span></span>|
|[<span data-ttu-id="5c7fd-115">Get deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="5c7fd-115">Get deviceCompliancePolicy</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-get.md)|[<span data-ttu-id="5c7fd-116">deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="5c7fd-116">deviceCompliancePolicy</span></span>](../resources/intune-deviceconfig-devicecompliancepolicy.md)|<span data-ttu-id="5c7fd-117">读取 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5c7fd-117">Read properties and relationships of the [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) object.</span></span>|
|[<span data-ttu-id="5c7fd-118">assign 操作</span><span class="sxs-lookup"><span data-stu-id="5c7fd-118">assign action</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-assign.md)|<span data-ttu-id="5c7fd-119">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5c7fd-119">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="5c7fd-120">尚未记录</span><span class="sxs-lookup"><span data-stu-id="5c7fd-120">Not yet documented</span></span>|
|[<span data-ttu-id="5c7fd-121">scheduleActionsForRules 操作</span><span class="sxs-lookup"><span data-stu-id="5c7fd-121">scheduleActionsForRules action</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-scheduleactionsforrules.md)|<span data-ttu-id="5c7fd-122">无</span><span class="sxs-lookup"><span data-stu-id="5c7fd-122">None</span></span>|<span data-ttu-id="5c7fd-123">尚未记录</span><span class="sxs-lookup"><span data-stu-id="5c7fd-123">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="5c7fd-124">属性</span><span class="sxs-lookup"><span data-stu-id="5c7fd-124">Properties</span></span>
|<span data-ttu-id="5c7fd-125">属性</span><span class="sxs-lookup"><span data-stu-id="5c7fd-125">Property</span></span>|<span data-ttu-id="5c7fd-126">类型</span><span class="sxs-lookup"><span data-stu-id="5c7fd-126">Type</span></span>|<span data-ttu-id="5c7fd-127">说明</span><span class="sxs-lookup"><span data-stu-id="5c7fd-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c7fd-128">id</span><span class="sxs-lookup"><span data-stu-id="5c7fd-128">id</span></span>|<span data-ttu-id="5c7fd-129">字符串</span><span class="sxs-lookup"><span data-stu-id="5c7fd-129">String</span></span>|<span data-ttu-id="5c7fd-130">实体的键。</span><span class="sxs-lookup"><span data-stu-id="5c7fd-130">Key of the entity.</span></span>|
|<span data-ttu-id="5c7fd-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5c7fd-131">createdDateTime</span></span>|<span data-ttu-id="5c7fd-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c7fd-132">DateTimeOffset</span></span>|<span data-ttu-id="5c7fd-133">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="5c7fd-133">DateTime the object was created.</span></span>|
|<span data-ttu-id="5c7fd-134">description</span><span class="sxs-lookup"><span data-stu-id="5c7fd-134">description</span></span>|<span data-ttu-id="5c7fd-135">String</span><span class="sxs-lookup"><span data-stu-id="5c7fd-135">String</span></span>|<span data-ttu-id="5c7fd-136">管理员提供的设备配置说明。</span><span class="sxs-lookup"><span data-stu-id="5c7fd-136">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="5c7fd-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5c7fd-137">lastModifiedDateTime</span></span>|<span data-ttu-id="5c7fd-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c7fd-138">DateTimeOffset</span></span>|<span data-ttu-id="5c7fd-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="5c7fd-139">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="5c7fd-140">displayName</span><span class="sxs-lookup"><span data-stu-id="5c7fd-140">displayName</span></span>|<span data-ttu-id="5c7fd-141">String</span><span class="sxs-lookup"><span data-stu-id="5c7fd-141">String</span></span>|<span data-ttu-id="5c7fd-142">管理员提供的设备配置名称。</span><span class="sxs-lookup"><span data-stu-id="5c7fd-142">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="5c7fd-143">version</span><span class="sxs-lookup"><span data-stu-id="5c7fd-143">version</span></span>|<span data-ttu-id="5c7fd-144">Int32</span><span class="sxs-lookup"><span data-stu-id="5c7fd-144">Int32</span></span>|<span data-ttu-id="5c7fd-145">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="5c7fd-145">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5c7fd-146">关系</span><span class="sxs-lookup"><span data-stu-id="5c7fd-146">Relationships</span></span>
|<span data-ttu-id="5c7fd-147">关系</span><span class="sxs-lookup"><span data-stu-id="5c7fd-147">Relationship</span></span>|<span data-ttu-id="5c7fd-148">类型</span><span class="sxs-lookup"><span data-stu-id="5c7fd-148">Type</span></span>|<span data-ttu-id="5c7fd-149">说明</span><span class="sxs-lookup"><span data-stu-id="5c7fd-149">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c7fd-150">scheduledActionsForRule</span><span class="sxs-lookup"><span data-stu-id="5c7fd-150">scheduledActionsForRule</span></span>|<span data-ttu-id="5c7fd-151">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5c7fd-151">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) collection</span></span>|<span data-ttu-id="5c7fd-152">此规则的计划操作列表</span><span class="sxs-lookup"><span data-stu-id="5c7fd-152">The list of scheduled action for this rule</span></span>|
|<span data-ttu-id="5c7fd-153">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="5c7fd-153">deviceStatuses</span></span>|<span data-ttu-id="5c7fd-154">[deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5c7fd-154">[deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) collection</span></span>|<span data-ttu-id="5c7fd-155">DeviceComplianceDeviceStatus 的列表。</span><span class="sxs-lookup"><span data-stu-id="5c7fd-155">List of DeviceComplianceDeviceStatus.</span></span>|
|<span data-ttu-id="5c7fd-156">userStatuses</span><span class="sxs-lookup"><span data-stu-id="5c7fd-156">userStatuses</span></span>|<span data-ttu-id="5c7fd-157">[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5c7fd-157">[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) collection</span></span>|<span data-ttu-id="5c7fd-158">DeviceComplianceUserStatus 的列表。</span><span class="sxs-lookup"><span data-stu-id="5c7fd-158">List of DeviceComplianceUserStatus.</span></span>|
|<span data-ttu-id="5c7fd-159">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="5c7fd-159">deviceStatusOverview</span></span>|[<span data-ttu-id="5c7fd-160">deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="5c7fd-160">deviceComplianceDeviceOverview</span></span>](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md)|<span data-ttu-id="5c7fd-161">设备符合性设备状态概述</span><span class="sxs-lookup"><span data-stu-id="5c7fd-161">Device compliance devices status overview</span></span>|
|<span data-ttu-id="5c7fd-162">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="5c7fd-162">userStatusOverview</span></span>|[<span data-ttu-id="5c7fd-163">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="5c7fd-163">deviceComplianceUserOverview</span></span>](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|<span data-ttu-id="5c7fd-164">设备符合性用户状态概述</span><span class="sxs-lookup"><span data-stu-id="5c7fd-164">Device compliance users status overview</span></span>|
|<span data-ttu-id="5c7fd-165">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="5c7fd-165">deviceSettingStateSummaries</span></span>|<span data-ttu-id="5c7fd-166">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5c7fd-166">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="5c7fd-167">符合性设置状态设备摘要</span><span class="sxs-lookup"><span data-stu-id="5c7fd-167">Compliance Setting State Device Summary</span></span>|
|<span data-ttu-id="5c7fd-168">assignments</span><span class="sxs-lookup"><span data-stu-id="5c7fd-168">assignments</span></span>|<span data-ttu-id="5c7fd-169">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5c7fd-169">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="5c7fd-170">此符合性策略的分配集合。</span><span class="sxs-lookup"><span data-stu-id="5c7fd-170">The collection of assignments for this compliance policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5c7fd-171">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5c7fd-171">JSON Representation</span></span>
<span data-ttu-id="5c7fd-172">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5c7fd-172">Here is a JSON representation of the resource.</span></span>
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



