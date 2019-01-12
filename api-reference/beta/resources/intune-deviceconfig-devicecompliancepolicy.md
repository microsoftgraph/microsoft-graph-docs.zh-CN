---
title: deviceCompliancePolicy 资源类型
description: '这是符合性策略的基类。 符合性策略特定于平台，每个平台的符合性策略相互独立，且继承自此处。 '
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: dd282f30e36ab659b37306a7793b6d6aae1ddd21
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27965430"
---
# <a name="devicecompliancepolicy-resource-type"></a><span data-ttu-id="16896-104">deviceCompliancePolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="16896-104">deviceCompliancePolicy resource type</span></span>

> <span data-ttu-id="16896-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="16896-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="16896-106">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="16896-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="16896-107">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="16896-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="16896-108">这是符合性策略的基类。</span><span class="sxs-lookup"><span data-stu-id="16896-108">This is the base class for Compliance policy.</span></span> <span data-ttu-id="16896-109">符合性策略特定于平台，每个平台的符合性策略相互独立，且继承自此处。</span><span class="sxs-lookup"><span data-stu-id="16896-109">Compliance policies are platform specific and individual per-platform compliance policies inherit from here.</span></span> 
## <a name="methods"></a><span data-ttu-id="16896-110">方法</span><span class="sxs-lookup"><span data-stu-id="16896-110">Methods</span></span>
|<span data-ttu-id="16896-111">方法</span><span class="sxs-lookup"><span data-stu-id="16896-111">Method</span></span>|<span data-ttu-id="16896-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="16896-112">Return Type</span></span>|<span data-ttu-id="16896-113">说明</span><span class="sxs-lookup"><span data-stu-id="16896-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="16896-114">List deviceCompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="16896-114">List deviceCompliancePolicies</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-list.md)|<span data-ttu-id="16896-115">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="16896-115">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) collection</span></span>|<span data-ttu-id="16896-116">列出 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="16896-116">List properties and relationships of the [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) objects.</span></span>|
|[<span data-ttu-id="16896-117">Get deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="16896-117">Get deviceCompliancePolicy</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-get.md)|[<span data-ttu-id="16896-118">deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="16896-118">deviceCompliancePolicy</span></span>](../resources/intune-deviceconfig-devicecompliancepolicy.md)|<span data-ttu-id="16896-119">读取 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="16896-119">Read properties and relationships of the [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) object.</span></span>|
|[<span data-ttu-id="16896-120">assign 操作</span><span class="sxs-lookup"><span data-stu-id="16896-120">assign action</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-assign.md)|<span data-ttu-id="16896-121">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="16896-121">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="16896-122">尚未记录</span><span class="sxs-lookup"><span data-stu-id="16896-122">Not yet documented</span></span>|
|[<span data-ttu-id="16896-123">scheduleActionsForRules 操作</span><span class="sxs-lookup"><span data-stu-id="16896-123">scheduleActionsForRules action</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-scheduleactionsforrules.md)|<span data-ttu-id="16896-124">无</span><span class="sxs-lookup"><span data-stu-id="16896-124">None</span></span>|<span data-ttu-id="16896-125">尚未记录</span><span class="sxs-lookup"><span data-stu-id="16896-125">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="16896-126">属性</span><span class="sxs-lookup"><span data-stu-id="16896-126">Properties</span></span>
|<span data-ttu-id="16896-127">属性</span><span class="sxs-lookup"><span data-stu-id="16896-127">Property</span></span>|<span data-ttu-id="16896-128">类型</span><span class="sxs-lookup"><span data-stu-id="16896-128">Type</span></span>|<span data-ttu-id="16896-129">Description</span><span class="sxs-lookup"><span data-stu-id="16896-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16896-130">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="16896-130">roleScopeTagIds</span></span>|<span data-ttu-id="16896-131">String 集合</span><span class="sxs-lookup"><span data-stu-id="16896-131">String collection</span></span>|<span data-ttu-id="16896-132">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="16896-132">List of Scope Tags for this Entity instance.</span></span>|
|<span data-ttu-id="16896-133">id</span><span class="sxs-lookup"><span data-stu-id="16896-133">id</span></span>|<span data-ttu-id="16896-134">String</span><span class="sxs-lookup"><span data-stu-id="16896-134">String</span></span>|<span data-ttu-id="16896-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="16896-135">Key of the entity.</span></span>|
|<span data-ttu-id="16896-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="16896-136">createdDateTime</span></span>|<span data-ttu-id="16896-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="16896-137">DateTimeOffset</span></span>|<span data-ttu-id="16896-138">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="16896-138">DateTime the object was created.</span></span>|
|<span data-ttu-id="16896-139">description</span><span class="sxs-lookup"><span data-stu-id="16896-139">description</span></span>|<span data-ttu-id="16896-140">String</span><span class="sxs-lookup"><span data-stu-id="16896-140">String</span></span>|<span data-ttu-id="16896-141">管理员提供的设备配置说明。</span><span class="sxs-lookup"><span data-stu-id="16896-141">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="16896-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="16896-142">lastModifiedDateTime</span></span>|<span data-ttu-id="16896-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="16896-143">DateTimeOffset</span></span>|<span data-ttu-id="16896-144">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="16896-144">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="16896-145">displayName</span><span class="sxs-lookup"><span data-stu-id="16896-145">displayName</span></span>|<span data-ttu-id="16896-146">String</span><span class="sxs-lookup"><span data-stu-id="16896-146">String</span></span>|<span data-ttu-id="16896-147">管理员提供的设备配置名称。</span><span class="sxs-lookup"><span data-stu-id="16896-147">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="16896-148">version</span><span class="sxs-lookup"><span data-stu-id="16896-148">version</span></span>|<span data-ttu-id="16896-149">Int32</span><span class="sxs-lookup"><span data-stu-id="16896-149">Int32</span></span>|<span data-ttu-id="16896-150">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="16896-150">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="16896-151">关系</span><span class="sxs-lookup"><span data-stu-id="16896-151">Relationships</span></span>
|<span data-ttu-id="16896-152">关系</span><span class="sxs-lookup"><span data-stu-id="16896-152">Relationship</span></span>|<span data-ttu-id="16896-153">类型</span><span class="sxs-lookup"><span data-stu-id="16896-153">Type</span></span>|<span data-ttu-id="16896-154">说明</span><span class="sxs-lookup"><span data-stu-id="16896-154">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16896-155">scheduledActionsForRule</span><span class="sxs-lookup"><span data-stu-id="16896-155">scheduledActionsForRule</span></span>|<span data-ttu-id="16896-156">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="16896-156">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) collection</span></span>|<span data-ttu-id="16896-157">此规则的计划操作列表</span><span class="sxs-lookup"><span data-stu-id="16896-157">The list of scheduled action for this rule</span></span>|
|<span data-ttu-id="16896-158">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="16896-158">deviceStatuses</span></span>|<span data-ttu-id="16896-159">[deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="16896-159">[deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) collection</span></span>|<span data-ttu-id="16896-160">DeviceComplianceDeviceStatus 的列表。</span><span class="sxs-lookup"><span data-stu-id="16896-160">List of DeviceComplianceDeviceStatus.</span></span>|
|<span data-ttu-id="16896-161">userStatuses</span><span class="sxs-lookup"><span data-stu-id="16896-161">userStatuses</span></span>|<span data-ttu-id="16896-162">[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="16896-162">[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) collection</span></span>|<span data-ttu-id="16896-163">DeviceComplianceUserStatus 的列表。</span><span class="sxs-lookup"><span data-stu-id="16896-163">List of DeviceComplianceUserStatus.</span></span>|
|<span data-ttu-id="16896-164">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="16896-164">deviceStatusOverview</span></span>|[<span data-ttu-id="16896-165">deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="16896-165">deviceComplianceDeviceOverview</span></span>](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md)|<span data-ttu-id="16896-166">设备符合性设备状态概述</span><span class="sxs-lookup"><span data-stu-id="16896-166">Device compliance devices status overview</span></span>|
|<span data-ttu-id="16896-167">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="16896-167">userStatusOverview</span></span>|[<span data-ttu-id="16896-168">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="16896-168">deviceComplianceUserOverview</span></span>](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|<span data-ttu-id="16896-169">设备符合性用户状态概述</span><span class="sxs-lookup"><span data-stu-id="16896-169">Device compliance users status overview</span></span>|
|<span data-ttu-id="16896-170">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="16896-170">deviceSettingStateSummaries</span></span>|<span data-ttu-id="16896-171">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="16896-171">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="16896-172">符合性设置状态设备摘要</span><span class="sxs-lookup"><span data-stu-id="16896-172">Compliance Setting State Device Summary</span></span>|
|<span data-ttu-id="16896-173">assignments</span><span class="sxs-lookup"><span data-stu-id="16896-173">assignments</span></span>|<span data-ttu-id="16896-174">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="16896-174">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="16896-175">此符合性策略的分配集合。</span><span class="sxs-lookup"><span data-stu-id="16896-175">The collection of assignments for this compliance policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="16896-176">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="16896-176">JSON Representation</span></span>
<span data-ttu-id="16896-177">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="16896-177">Here is a JSON representation of the resource.</span></span>
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





