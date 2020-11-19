---
title: deviceManagementConfigurationPolicy 资源类型
description: 设备管理配置策略
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b00db0b46c03726561cff31a6a7f9a52b165a55b
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49241287"
---
# <a name="devicemanagementconfigurationpolicy-resource-type"></a><span data-ttu-id="f108c-103">deviceManagementConfigurationPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="f108c-103">deviceManagementConfigurationPolicy resource type</span></span>

<span data-ttu-id="f108c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f108c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f108c-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f108c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f108c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f108c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f108c-107">设备管理配置策略</span><span class="sxs-lookup"><span data-stu-id="f108c-107">Device Management Configuration Policy</span></span>

## <a name="methods"></a><span data-ttu-id="f108c-108">方法</span><span class="sxs-lookup"><span data-stu-id="f108c-108">Methods</span></span>
|<span data-ttu-id="f108c-109">方法</span><span class="sxs-lookup"><span data-stu-id="f108c-109">Method</span></span>|<span data-ttu-id="f108c-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="f108c-110">Return Type</span></span>|<span data-ttu-id="f108c-111">说明</span><span class="sxs-lookup"><span data-stu-id="f108c-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f108c-112">列出 deviceManagementConfigurationPolicies</span><span class="sxs-lookup"><span data-stu-id="f108c-112">List deviceManagementConfigurationPolicies</span></span>](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicy-list.md)|<span data-ttu-id="f108c-113">[deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f108c-113">[deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) collection</span></span>|<span data-ttu-id="f108c-114">列出 [deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f108c-114">List properties and relationships of the [deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) objects.</span></span>|
|[<span data-ttu-id="f108c-115">获取 deviceManagementConfigurationPolicy</span><span class="sxs-lookup"><span data-stu-id="f108c-115">Get deviceManagementConfigurationPolicy</span></span>](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicy-get.md)|[<span data-ttu-id="f108c-116">deviceManagementConfigurationPolicy</span><span class="sxs-lookup"><span data-stu-id="f108c-116">deviceManagementConfigurationPolicy</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md)|<span data-ttu-id="f108c-117">读取 [deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f108c-117">Read properties and relationships of the [deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) object.</span></span>|
|[<span data-ttu-id="f108c-118">创建 deviceManagementConfigurationPolicy</span><span class="sxs-lookup"><span data-stu-id="f108c-118">Create deviceManagementConfigurationPolicy</span></span>](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicy-create.md)|[<span data-ttu-id="f108c-119">deviceManagementConfigurationPolicy</span><span class="sxs-lookup"><span data-stu-id="f108c-119">deviceManagementConfigurationPolicy</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md)|<span data-ttu-id="f108c-120">创建新的 [deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f108c-120">Create a new [deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) object.</span></span>|
|[<span data-ttu-id="f108c-121">删除 deviceManagementConfigurationPolicy</span><span class="sxs-lookup"><span data-stu-id="f108c-121">Delete deviceManagementConfigurationPolicy</span></span>](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicy-delete.md)|<span data-ttu-id="f108c-122">无</span><span class="sxs-lookup"><span data-stu-id="f108c-122">None</span></span>|<span data-ttu-id="f108c-123">删除 [deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="f108c-123">Deletes a [deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md).</span></span>|
|[<span data-ttu-id="f108c-124">更新 deviceManagementConfigurationPolicy</span><span class="sxs-lookup"><span data-stu-id="f108c-124">Update deviceManagementConfigurationPolicy</span></span>](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicy-update.md)|[<span data-ttu-id="f108c-125">deviceManagementConfigurationPolicy</span><span class="sxs-lookup"><span data-stu-id="f108c-125">deviceManagementConfigurationPolicy</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md)|<span data-ttu-id="f108c-126">更新 [deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f108c-126">Update the properties of a [deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) object.</span></span>|
|[<span data-ttu-id="f108c-127">分配操作</span><span class="sxs-lookup"><span data-stu-id="f108c-127">assign action</span></span>](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicy-assign.md)|<span data-ttu-id="f108c-128">[deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f108c-128">[deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) collection</span></span>|<span data-ttu-id="f108c-129">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f108c-129">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="f108c-130">属性</span><span class="sxs-lookup"><span data-stu-id="f108c-130">Properties</span></span>
|<span data-ttu-id="f108c-131">属性</span><span class="sxs-lookup"><span data-stu-id="f108c-131">Property</span></span>|<span data-ttu-id="f108c-132">类型</span><span class="sxs-lookup"><span data-stu-id="f108c-132">Type</span></span>|<span data-ttu-id="f108c-133">说明</span><span class="sxs-lookup"><span data-stu-id="f108c-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f108c-134">id</span><span class="sxs-lookup"><span data-stu-id="f108c-134">id</span></span>|<span data-ttu-id="f108c-135">String</span><span class="sxs-lookup"><span data-stu-id="f108c-135">String</span></span>|<span data-ttu-id="f108c-136">策略文档的键。</span><span class="sxs-lookup"><span data-stu-id="f108c-136">Key of the policy document.</span></span> <span data-ttu-id="f108c-137">自动生成。</span><span class="sxs-lookup"><span data-stu-id="f108c-137">Automatically generated.</span></span>|
|<span data-ttu-id="f108c-138">name</span><span class="sxs-lookup"><span data-stu-id="f108c-138">name</span></span>|<span data-ttu-id="f108c-139">String</span><span class="sxs-lookup"><span data-stu-id="f108c-139">String</span></span>|<span data-ttu-id="f108c-140">策略名称</span><span class="sxs-lookup"><span data-stu-id="f108c-140">Policy name</span></span>|
|<span data-ttu-id="f108c-141">description</span><span class="sxs-lookup"><span data-stu-id="f108c-141">description</span></span>|<span data-ttu-id="f108c-142">String</span><span class="sxs-lookup"><span data-stu-id="f108c-142">String</span></span>|<span data-ttu-id="f108c-143">策略说明</span><span class="sxs-lookup"><span data-stu-id="f108c-143">Policy description</span></span>|
|<span data-ttu-id="f108c-144">平台</span><span class="sxs-lookup"><span data-stu-id="f108c-144">platforms</span></span>|[<span data-ttu-id="f108c-145">deviceManagementConfigurationPlatforms</span><span class="sxs-lookup"><span data-stu-id="f108c-145">deviceManagementConfigurationPlatforms</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationplatforms.md)|<span data-ttu-id="f108c-146">此策略的平台。</span><span class="sxs-lookup"><span data-stu-id="f108c-146">Platforms for this policy.</span></span> <span data-ttu-id="f108c-147">可取值为：`none`、`macOS`、`windows10X`、`windows10`。</span><span class="sxs-lookup"><span data-stu-id="f108c-147">Possible values are: `none`, `macOS`, `windows10X`, `windows10`.</span></span>|
|<span data-ttu-id="f108c-148">技术</span><span class="sxs-lookup"><span data-stu-id="f108c-148">technologies</span></span>|[<span data-ttu-id="f108c-149">deviceManagementConfigurationTechnologies</span><span class="sxs-lookup"><span data-stu-id="f108c-149">deviceManagementConfigurationTechnologies</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationtechnologies.md)|<span data-ttu-id="f108c-150">适用于此策略的技术。</span><span class="sxs-lookup"><span data-stu-id="f108c-150">Technologies for this policy.</span></span> <span data-ttu-id="f108c-151">可取值为：`none`、`mdm`、`windows10XManagement`、`configManager`。</span><span class="sxs-lookup"><span data-stu-id="f108c-151">Possible values are: `none`, `mdm`, `windows10XManagement`, `configManager`.</span></span>|
|<span data-ttu-id="f108c-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f108c-152">createdDateTime</span></span>|<span data-ttu-id="f108c-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f108c-153">DateTimeOffset</span></span>|<span data-ttu-id="f108c-154">策略创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="f108c-154">Policy creation date and time.</span></span> <span data-ttu-id="f108c-155">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="f108c-155">This property is read-only.</span></span>|
|<span data-ttu-id="f108c-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f108c-156">lastModifiedDateTime</span></span>|<span data-ttu-id="f108c-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f108c-157">DateTimeOffset</span></span>|<span data-ttu-id="f108c-158">策略上次修改日期和时间。</span><span class="sxs-lookup"><span data-stu-id="f108c-158">Policy last modification date and time.</span></span> <span data-ttu-id="f108c-159">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="f108c-159">This property is read-only.</span></span>|
|<span data-ttu-id="f108c-160">settingCount</span><span class="sxs-lookup"><span data-stu-id="f108c-160">settingCount</span></span>|<span data-ttu-id="f108c-161">Int32</span><span class="sxs-lookup"><span data-stu-id="f108c-161">Int32</span></span>|<span data-ttu-id="f108c-162">设置的数目。</span><span class="sxs-lookup"><span data-stu-id="f108c-162">Number of settings.</span></span> <span data-ttu-id="f108c-163">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="f108c-163">This property is read-only.</span></span>|
|<span data-ttu-id="f108c-164">creationSource</span><span class="sxs-lookup"><span data-stu-id="f108c-164">creationSource</span></span>|<span data-ttu-id="f108c-165">String</span><span class="sxs-lookup"><span data-stu-id="f108c-165">String</span></span>|<span data-ttu-id="f108c-166">策略创建源</span><span class="sxs-lookup"><span data-stu-id="f108c-166">Policy creation source</span></span>|
|<span data-ttu-id="f108c-167">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f108c-167">roleScopeTagIds</span></span>|<span data-ttu-id="f108c-168">String 集合</span><span class="sxs-lookup"><span data-stu-id="f108c-168">String collection</span></span>|<span data-ttu-id="f108c-169">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="f108c-169">List of Scope Tags for this Entity instance.</span></span>|
|<span data-ttu-id="f108c-170">isAssigned</span><span class="sxs-lookup"><span data-stu-id="f108c-170">isAssigned</span></span>|<span data-ttu-id="f108c-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="f108c-171">Boolean</span></span>|<span data-ttu-id="f108c-172">策略分配状态。</span><span class="sxs-lookup"><span data-stu-id="f108c-172">Policy assignment status.</span></span> <span data-ttu-id="f108c-173">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="f108c-173">This property is read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f108c-174">关系</span><span class="sxs-lookup"><span data-stu-id="f108c-174">Relationships</span></span>
|<span data-ttu-id="f108c-175">关系</span><span class="sxs-lookup"><span data-stu-id="f108c-175">Relationship</span></span>|<span data-ttu-id="f108c-176">类型</span><span class="sxs-lookup"><span data-stu-id="f108c-176">Type</span></span>|<span data-ttu-id="f108c-177">说明</span><span class="sxs-lookup"><span data-stu-id="f108c-177">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f108c-178">settings</span><span class="sxs-lookup"><span data-stu-id="f108c-178">settings</span></span>|<span data-ttu-id="f108c-179">[deviceManagementConfigurationSetting](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f108c-179">[deviceManagementConfigurationSetting](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md) collection</span></span>|<span data-ttu-id="f108c-180">策略设置</span><span class="sxs-lookup"><span data-stu-id="f108c-180">Policy settings</span></span>|
|<span data-ttu-id="f108c-181">assignments</span><span class="sxs-lookup"><span data-stu-id="f108c-181">assignments</span></span>|<span data-ttu-id="f108c-182">[deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f108c-182">[deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) collection</span></span>|<span data-ttu-id="f108c-183">策略分配</span><span class="sxs-lookup"><span data-stu-id="f108c-183">Policy assignments</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f108c-184">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f108c-184">JSON Representation</span></span>
<span data-ttu-id="f108c-185">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f108c-185">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationPolicy",
  "id": "String (identifier)",
  "name": "String",
  "description": "String",
  "platforms": "String",
  "technologies": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "settingCount": 1024,
  "creationSource": "String",
  "roleScopeTagIds": [
    "String"
  ],
  "isAssigned": true
}
```




