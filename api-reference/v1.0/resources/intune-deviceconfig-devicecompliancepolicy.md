---
title: deviceCompliancePolicy 资源类型
description: '这是符合性策略的基类。 符合性策略特定于平台，每个平台的符合性策略相互独立，且继承自此处。 '
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 85a82c981c16370603e3622f6536755bf9146343
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990395"
---
# <a name="devicecompliancepolicy-resource-type"></a><span data-ttu-id="487b6-104">deviceCompliancePolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="487b6-104">deviceCompliancePolicy resource type</span></span>

> <span data-ttu-id="487b6-105">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="487b6-105">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="487b6-106">这是符合性策略的基类。</span><span class="sxs-lookup"><span data-stu-id="487b6-106">This is the base class for Compliance policy.</span></span> <span data-ttu-id="487b6-107">符合性策略特定于平台，每个平台的符合性策略相互独立，且继承自此处。</span><span class="sxs-lookup"><span data-stu-id="487b6-107">Compliance policies are platform specific and individual per-platform compliance policies inherit from here.</span></span> 
## <a name="methods"></a><span data-ttu-id="487b6-108">方法</span><span class="sxs-lookup"><span data-stu-id="487b6-108">Methods</span></span>
|<span data-ttu-id="487b6-109">方法</span><span class="sxs-lookup"><span data-stu-id="487b6-109">Method</span></span>|<span data-ttu-id="487b6-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="487b6-110">Return Type</span></span>|<span data-ttu-id="487b6-111">说明</span><span class="sxs-lookup"><span data-stu-id="487b6-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="487b6-112">List deviceCompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="487b6-112">List deviceCompliancePolicies</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-list.md)|<span data-ttu-id="487b6-113">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="487b6-113">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) collection</span></span>|<span data-ttu-id="487b6-114">列出 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="487b6-114">List properties and relationships of the [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) objects.</span></span>|
|[<span data-ttu-id="487b6-115">Get deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="487b6-115">Get deviceCompliancePolicy</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-get.md)|[<span data-ttu-id="487b6-116">deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="487b6-116">deviceCompliancePolicy</span></span>](../resources/intune-deviceconfig-devicecompliancepolicy.md)|<span data-ttu-id="487b6-117">读取 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="487b6-117">Read properties and relationships of the [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) object.</span></span>|
|[<span data-ttu-id="487b6-118">assign 操作</span><span class="sxs-lookup"><span data-stu-id="487b6-118">assign action</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-assign.md)|<span data-ttu-id="487b6-119">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="487b6-119">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="487b6-120">尚未记录</span><span class="sxs-lookup"><span data-stu-id="487b6-120">Not yet documented</span></span>|
|[<span data-ttu-id="487b6-121">scheduleActionsForRules 操作</span><span class="sxs-lookup"><span data-stu-id="487b6-121">scheduleActionsForRules action</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-scheduleactionsforrules.md)|<span data-ttu-id="487b6-122">无</span><span class="sxs-lookup"><span data-stu-id="487b6-122">None</span></span>|<span data-ttu-id="487b6-123">尚未记录</span><span class="sxs-lookup"><span data-stu-id="487b6-123">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="487b6-124">属性</span><span class="sxs-lookup"><span data-stu-id="487b6-124">Properties</span></span>
|<span data-ttu-id="487b6-125">属性</span><span class="sxs-lookup"><span data-stu-id="487b6-125">Property</span></span>|<span data-ttu-id="487b6-126">类型</span><span class="sxs-lookup"><span data-stu-id="487b6-126">Type</span></span>|<span data-ttu-id="487b6-127">说明</span><span class="sxs-lookup"><span data-stu-id="487b6-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="487b6-128">id</span><span class="sxs-lookup"><span data-stu-id="487b6-128">id</span></span>|<span data-ttu-id="487b6-129">String</span><span class="sxs-lookup"><span data-stu-id="487b6-129">String</span></span>|<span data-ttu-id="487b6-130">实体的键。</span><span class="sxs-lookup"><span data-stu-id="487b6-130">Key of the entity.</span></span>|
|<span data-ttu-id="487b6-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="487b6-131">createdDateTime</span></span>|<span data-ttu-id="487b6-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="487b6-132">DateTimeOffset</span></span>|<span data-ttu-id="487b6-133">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="487b6-133">DateTime the object was created.</span></span>|
|<span data-ttu-id="487b6-134">description</span><span class="sxs-lookup"><span data-stu-id="487b6-134">description</span></span>|<span data-ttu-id="487b6-135">String</span><span class="sxs-lookup"><span data-stu-id="487b6-135">String</span></span>|<span data-ttu-id="487b6-136">管理员提供的设备配置说明。</span><span class="sxs-lookup"><span data-stu-id="487b6-136">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="487b6-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="487b6-137">lastModifiedDateTime</span></span>|<span data-ttu-id="487b6-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="487b6-138">DateTimeOffset</span></span>|<span data-ttu-id="487b6-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="487b6-139">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="487b6-140">displayName</span><span class="sxs-lookup"><span data-stu-id="487b6-140">displayName</span></span>|<span data-ttu-id="487b6-141">String</span><span class="sxs-lookup"><span data-stu-id="487b6-141">String</span></span>|<span data-ttu-id="487b6-142">管理员提供的设备配置名称。</span><span class="sxs-lookup"><span data-stu-id="487b6-142">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="487b6-143">version</span><span class="sxs-lookup"><span data-stu-id="487b6-143">version</span></span>|<span data-ttu-id="487b6-144">Int32</span><span class="sxs-lookup"><span data-stu-id="487b6-144">Int32</span></span>|<span data-ttu-id="487b6-145">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="487b6-145">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="487b6-146">关系</span><span class="sxs-lookup"><span data-stu-id="487b6-146">Relationships</span></span>
|<span data-ttu-id="487b6-147">关系</span><span class="sxs-lookup"><span data-stu-id="487b6-147">Relationship</span></span>|<span data-ttu-id="487b6-148">类型</span><span class="sxs-lookup"><span data-stu-id="487b6-148">Type</span></span>|<span data-ttu-id="487b6-149">说明</span><span class="sxs-lookup"><span data-stu-id="487b6-149">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="487b6-150">scheduledActionsForRule</span><span class="sxs-lookup"><span data-stu-id="487b6-150">scheduledActionsForRule</span></span>|<span data-ttu-id="487b6-151">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="487b6-151">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) collection</span></span>|<span data-ttu-id="487b6-152">此规则的计划操作列表</span><span class="sxs-lookup"><span data-stu-id="487b6-152">The list of scheduled action for this rule</span></span>|
|<span data-ttu-id="487b6-153">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="487b6-153">deviceStatuses</span></span>|<span data-ttu-id="487b6-154">[deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="487b6-154">[deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) collection</span></span>|<span data-ttu-id="487b6-155">DeviceComplianceDeviceStatus 的列表。</span><span class="sxs-lookup"><span data-stu-id="487b6-155">List of DeviceComplianceDeviceStatus.</span></span>|
|<span data-ttu-id="487b6-156">userStatuses</span><span class="sxs-lookup"><span data-stu-id="487b6-156">userStatuses</span></span>|<span data-ttu-id="487b6-157">[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="487b6-157">[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) collection</span></span>|<span data-ttu-id="487b6-158">DeviceComplianceUserStatus 的列表。</span><span class="sxs-lookup"><span data-stu-id="487b6-158">List of DeviceComplianceUserStatus.</span></span>|
|<span data-ttu-id="487b6-159">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="487b6-159">deviceStatusOverview</span></span>|[<span data-ttu-id="487b6-160">deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="487b6-160">deviceComplianceDeviceOverview</span></span>](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md)|<span data-ttu-id="487b6-161">设备符合性设备状态概述</span><span class="sxs-lookup"><span data-stu-id="487b6-161">Device compliance devices status overview</span></span>|
|<span data-ttu-id="487b6-162">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="487b6-162">userStatusOverview</span></span>|[<span data-ttu-id="487b6-163">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="487b6-163">deviceComplianceUserOverview</span></span>](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|<span data-ttu-id="487b6-164">设备符合性用户状态概述</span><span class="sxs-lookup"><span data-stu-id="487b6-164">Device compliance users status overview</span></span>|
|<span data-ttu-id="487b6-165">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="487b6-165">deviceSettingStateSummaries</span></span>|<span data-ttu-id="487b6-166">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="487b6-166">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="487b6-167">符合性设置状态设备摘要</span><span class="sxs-lookup"><span data-stu-id="487b6-167">Compliance Setting State Device Summary</span></span>|
|<span data-ttu-id="487b6-168">assignments</span><span class="sxs-lookup"><span data-stu-id="487b6-168">assignments</span></span>|<span data-ttu-id="487b6-169">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="487b6-169">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="487b6-170">此符合性策略的分配集合。</span><span class="sxs-lookup"><span data-stu-id="487b6-170">The collection of assignments for this compliance policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="487b6-171">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="487b6-171">JSON Representation</span></span>
<span data-ttu-id="487b6-172">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="487b6-172">Here is a JSON representation of the resource.</span></span>
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



