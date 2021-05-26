---
title: deviceManagementConfigurationPolicy 资源类型
description: 设备管理配置策略
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bd23889586ea110bb663b41d89556996e87340e2
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666504"
---
# <a name="devicemanagementconfigurationpolicy-resource-type"></a><span data-ttu-id="0df50-103">deviceManagementConfigurationPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="0df50-103">deviceManagementConfigurationPolicy resource type</span></span>

<span data-ttu-id="0df50-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0df50-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0df50-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0df50-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0df50-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0df50-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0df50-107">设备管理配置策略</span><span class="sxs-lookup"><span data-stu-id="0df50-107">Device Management Configuration Policy</span></span>

## <a name="methods"></a><span data-ttu-id="0df50-108">方法</span><span class="sxs-lookup"><span data-stu-id="0df50-108">Methods</span></span>
|<span data-ttu-id="0df50-109">方法</span><span class="sxs-lookup"><span data-stu-id="0df50-109">Method</span></span>|<span data-ttu-id="0df50-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="0df50-110">Return Type</span></span>|<span data-ttu-id="0df50-111">说明</span><span class="sxs-lookup"><span data-stu-id="0df50-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0df50-112">列出 deviceManagementConfigurationPolicies</span><span class="sxs-lookup"><span data-stu-id="0df50-112">List deviceManagementConfigurationPolicies</span></span>](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicy-list.md)|<span data-ttu-id="0df50-113">[deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0df50-113">[deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) collection</span></span>|<span data-ttu-id="0df50-114">列出 [deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0df50-114">List properties and relationships of the [deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) objects.</span></span>|
|[<span data-ttu-id="0df50-115">获取 deviceManagementConfigurationPolicy</span><span class="sxs-lookup"><span data-stu-id="0df50-115">Get deviceManagementConfigurationPolicy</span></span>](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicy-get.md)|[<span data-ttu-id="0df50-116">deviceManagementConfigurationPolicy</span><span class="sxs-lookup"><span data-stu-id="0df50-116">deviceManagementConfigurationPolicy</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md)|<span data-ttu-id="0df50-117">读取 [deviceManagementConfigurationPolicy 对象的属性和](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="0df50-117">Read properties and relationships of the [deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) object.</span></span>|
|[<span data-ttu-id="0df50-118">创建 deviceManagementConfigurationPolicy</span><span class="sxs-lookup"><span data-stu-id="0df50-118">Create deviceManagementConfigurationPolicy</span></span>](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicy-create.md)|[<span data-ttu-id="0df50-119">deviceManagementConfigurationPolicy</span><span class="sxs-lookup"><span data-stu-id="0df50-119">deviceManagementConfigurationPolicy</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md)|<span data-ttu-id="0df50-120">创建新的 [deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0df50-120">Create a new [deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) object.</span></span>|
|[<span data-ttu-id="0df50-121">删除 deviceManagementConfigurationPolicy</span><span class="sxs-lookup"><span data-stu-id="0df50-121">Delete deviceManagementConfigurationPolicy</span></span>](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicy-delete.md)|<span data-ttu-id="0df50-122">无</span><span class="sxs-lookup"><span data-stu-id="0df50-122">None</span></span>|<span data-ttu-id="0df50-123">删除 [deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="0df50-123">Deletes a [deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md).</span></span>|
|[<span data-ttu-id="0df50-124">更新 deviceManagementConfigurationPolicy</span><span class="sxs-lookup"><span data-stu-id="0df50-124">Update deviceManagementConfigurationPolicy</span></span>](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicy-update.md)|[<span data-ttu-id="0df50-125">deviceManagementConfigurationPolicy</span><span class="sxs-lookup"><span data-stu-id="0df50-125">deviceManagementConfigurationPolicy</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md)|<span data-ttu-id="0df50-126">更新 [deviceManagementConfigurationPolicy 对象](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="0df50-126">Update the properties of a [deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) object.</span></span>|
|[<span data-ttu-id="0df50-127">分配操作</span><span class="sxs-lookup"><span data-stu-id="0df50-127">assign action</span></span>](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicy-assign.md)|<span data-ttu-id="0df50-128">[deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0df50-128">[deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) collection</span></span>|<span data-ttu-id="0df50-129">尚未记录</span><span class="sxs-lookup"><span data-stu-id="0df50-129">Not yet documented</span></span>|
|[<span data-ttu-id="0df50-130">createCopy 操作</span><span class="sxs-lookup"><span data-stu-id="0df50-130">createCopy action</span></span>](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicy-createcopy.md)|[<span data-ttu-id="0df50-131">deviceManagementConfigurationPolicy</span><span class="sxs-lookup"><span data-stu-id="0df50-131">deviceManagementConfigurationPolicy</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md)|<span data-ttu-id="0df50-132">尚未记录</span><span class="sxs-lookup"><span data-stu-id="0df50-132">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="0df50-133">属性</span><span class="sxs-lookup"><span data-stu-id="0df50-133">Properties</span></span>
|<span data-ttu-id="0df50-134">属性</span><span class="sxs-lookup"><span data-stu-id="0df50-134">Property</span></span>|<span data-ttu-id="0df50-135">类型</span><span class="sxs-lookup"><span data-stu-id="0df50-135">Type</span></span>|<span data-ttu-id="0df50-136">说明</span><span class="sxs-lookup"><span data-stu-id="0df50-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0df50-137">id</span><span class="sxs-lookup"><span data-stu-id="0df50-137">id</span></span>|<span data-ttu-id="0df50-138">String</span><span class="sxs-lookup"><span data-stu-id="0df50-138">String</span></span>|<span data-ttu-id="0df50-139">策略文档的键。</span><span class="sxs-lookup"><span data-stu-id="0df50-139">Key of the policy document.</span></span> <span data-ttu-id="0df50-140">自动生成。</span><span class="sxs-lookup"><span data-stu-id="0df50-140">Automatically generated.</span></span>|
|<span data-ttu-id="0df50-141">name</span><span class="sxs-lookup"><span data-stu-id="0df50-141">name</span></span>|<span data-ttu-id="0df50-142">String</span><span class="sxs-lookup"><span data-stu-id="0df50-142">String</span></span>|<span data-ttu-id="0df50-143">策略名称</span><span class="sxs-lookup"><span data-stu-id="0df50-143">Policy name</span></span>|
|<span data-ttu-id="0df50-144">说明</span><span class="sxs-lookup"><span data-stu-id="0df50-144">description</span></span>|<span data-ttu-id="0df50-145">String</span><span class="sxs-lookup"><span data-stu-id="0df50-145">String</span></span>|<span data-ttu-id="0df50-146">策略说明</span><span class="sxs-lookup"><span data-stu-id="0df50-146">Policy description</span></span>|
|<span data-ttu-id="0df50-147">平台</span><span class="sxs-lookup"><span data-stu-id="0df50-147">platforms</span></span>|[<span data-ttu-id="0df50-148">deviceManagementConfigurationPlatforms</span><span class="sxs-lookup"><span data-stu-id="0df50-148">deviceManagementConfigurationPlatforms</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationplatforms.md)|<span data-ttu-id="0df50-149">此策略的平台。</span><span class="sxs-lookup"><span data-stu-id="0df50-149">Platforms for this policy.</span></span> <span data-ttu-id="0df50-150">可取值为：`none`、`macOS`、`windows10X`、`windows10`。</span><span class="sxs-lookup"><span data-stu-id="0df50-150">Possible values are: `none`, `macOS`, `windows10X`, `windows10`.</span></span>|
|<span data-ttu-id="0df50-151">technologies</span><span class="sxs-lookup"><span data-stu-id="0df50-151">technologies</span></span>|[<span data-ttu-id="0df50-152">deviceManagementConfigurationTechnologies</span><span class="sxs-lookup"><span data-stu-id="0df50-152">deviceManagementConfigurationTechnologies</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationtechnologies.md)|<span data-ttu-id="0df50-153">此策略的技术。</span><span class="sxs-lookup"><span data-stu-id="0df50-153">Technologies for this policy.</span></span> <span data-ttu-id="0df50-154">可取值为：`none`、`mdm`、`windows10XManagement`、`configManager`、`microsoftSense`。</span><span class="sxs-lookup"><span data-stu-id="0df50-154">Possible values are: `none`, `mdm`, `windows10XManagement`, `configManager`, `microsoftSense`.</span></span>|
|<span data-ttu-id="0df50-155">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0df50-155">createdDateTime</span></span>|<span data-ttu-id="0df50-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0df50-156">DateTimeOffset</span></span>|<span data-ttu-id="0df50-157">策略创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="0df50-157">Policy creation date and time.</span></span> <span data-ttu-id="0df50-158">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="0df50-158">This property is read-only.</span></span>|
|<span data-ttu-id="0df50-159">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0df50-159">lastModifiedDateTime</span></span>|<span data-ttu-id="0df50-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0df50-160">DateTimeOffset</span></span>|<span data-ttu-id="0df50-161">策略上次修改日期和时间。</span><span class="sxs-lookup"><span data-stu-id="0df50-161">Policy last modification date and time.</span></span> <span data-ttu-id="0df50-162">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="0df50-162">This property is read-only.</span></span>|
|<span data-ttu-id="0df50-163">settingCount</span><span class="sxs-lookup"><span data-stu-id="0df50-163">settingCount</span></span>|<span data-ttu-id="0df50-164">Int32</span><span class="sxs-lookup"><span data-stu-id="0df50-164">Int32</span></span>|<span data-ttu-id="0df50-165">设置数。</span><span class="sxs-lookup"><span data-stu-id="0df50-165">Number of settings.</span></span> <span data-ttu-id="0df50-166">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="0df50-166">This property is read-only.</span></span>|
|<span data-ttu-id="0df50-167">creationSource</span><span class="sxs-lookup"><span data-stu-id="0df50-167">creationSource</span></span>|<span data-ttu-id="0df50-168">String</span><span class="sxs-lookup"><span data-stu-id="0df50-168">String</span></span>|<span data-ttu-id="0df50-169">策略创建源</span><span class="sxs-lookup"><span data-stu-id="0df50-169">Policy creation source</span></span>|
|<span data-ttu-id="0df50-170">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0df50-170">roleScopeTagIds</span></span>|<span data-ttu-id="0df50-171">String collection</span><span class="sxs-lookup"><span data-stu-id="0df50-171">String collection</span></span>|<span data-ttu-id="0df50-172">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="0df50-172">List of Scope Tags for this Entity instance.</span></span>|
|<span data-ttu-id="0df50-173">isAssigned</span><span class="sxs-lookup"><span data-stu-id="0df50-173">isAssigned</span></span>|<span data-ttu-id="0df50-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="0df50-174">Boolean</span></span>|<span data-ttu-id="0df50-175">策略分配状态。</span><span class="sxs-lookup"><span data-stu-id="0df50-175">Policy assignment status.</span></span> <span data-ttu-id="0df50-176">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="0df50-176">This property is read-only.</span></span>|
|<span data-ttu-id="0df50-177">templateReference</span><span class="sxs-lookup"><span data-stu-id="0df50-177">templateReference</span></span>|[<span data-ttu-id="0df50-178">deviceManagementConfigurationPolicyTemplateReference</span><span class="sxs-lookup"><span data-stu-id="0df50-178">deviceManagementConfigurationPolicyTemplateReference</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplatereference.md)|<span data-ttu-id="0df50-179">模板参考信息</span><span class="sxs-lookup"><span data-stu-id="0df50-179">Template reference information</span></span>|

## <a name="relationships"></a><span data-ttu-id="0df50-180">关系</span><span class="sxs-lookup"><span data-stu-id="0df50-180">Relationships</span></span>
|<span data-ttu-id="0df50-181">关系</span><span class="sxs-lookup"><span data-stu-id="0df50-181">Relationship</span></span>|<span data-ttu-id="0df50-182">类型</span><span class="sxs-lookup"><span data-stu-id="0df50-182">Type</span></span>|<span data-ttu-id="0df50-183">说明</span><span class="sxs-lookup"><span data-stu-id="0df50-183">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0df50-184">settings</span><span class="sxs-lookup"><span data-stu-id="0df50-184">settings</span></span>|<span data-ttu-id="0df50-185">[deviceManagementConfigurationSetting](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0df50-185">[deviceManagementConfigurationSetting](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md) collection</span></span>|<span data-ttu-id="0df50-186">策略设置</span><span class="sxs-lookup"><span data-stu-id="0df50-186">Policy settings</span></span>|
|<span data-ttu-id="0df50-187">assignments</span><span class="sxs-lookup"><span data-stu-id="0df50-187">assignments</span></span>|<span data-ttu-id="0df50-188">[deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0df50-188">[deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) collection</span></span>|<span data-ttu-id="0df50-189">策略分配</span><span class="sxs-lookup"><span data-stu-id="0df50-189">Policy assignments</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0df50-190">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0df50-190">JSON Representation</span></span>
<span data-ttu-id="0df50-191">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0df50-191">Here is a JSON representation of the resource.</span></span>
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
  "isAssigned": true,
  "templateReference": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationPolicyTemplateReference",
    "templateId": "String",
    "templateFamily": "String",
    "templateDisplayName": "String",
    "templateDisplayVersion": "String"
  }
}
```




