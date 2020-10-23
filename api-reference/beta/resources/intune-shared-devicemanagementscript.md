---
title: deviceManagementScript 资源类型
description: Intune 将向客户提供在已注册的 windows 10 Azure Active Directory 联接设备上运行其 Powershell 脚本的功能。 脚本可以运行一次，也可以定期运行。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2c855b09674f7d4a62879022257d96a5442a764a
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48730362"
---
# <a name="devicemanagementscript-resource-type"></a><span data-ttu-id="c7046-104">deviceManagementScript 资源类型</span><span class="sxs-lookup"><span data-stu-id="c7046-104">deviceManagementScript resource type</span></span>

<span data-ttu-id="c7046-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7046-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c7046-106">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c7046-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c7046-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c7046-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7046-108">Intune 将向客户提供在已注册的 windows 10 Azure Active Directory 联接设备上运行其 Powershell 脚本的功能。</span><span class="sxs-lookup"><span data-stu-id="c7046-108">Intune will provide customer the ability to run their Powershell scripts on the enrolled windows 10 Azure Active Directory joined devices.</span></span> <span data-ttu-id="c7046-109">脚本可以运行一次，也可以定期运行。</span><span class="sxs-lookup"><span data-stu-id="c7046-109">The script can be run once or periodically.</span></span>

## <a name="methods"></a><span data-ttu-id="c7046-110">Methods</span><span class="sxs-lookup"><span data-stu-id="c7046-110">Methods</span></span>
|<span data-ttu-id="c7046-111">方法</span><span class="sxs-lookup"><span data-stu-id="c7046-111">Method</span></span>|<span data-ttu-id="c7046-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="c7046-112">Return Type</span></span>|<span data-ttu-id="c7046-113">说明</span><span class="sxs-lookup"><span data-stu-id="c7046-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c7046-114">列出 deviceManagementScripts</span><span class="sxs-lookup"><span data-stu-id="c7046-114">List deviceManagementScripts</span></span>](../api/intune-shared-devicemanagementscript-list.md)|<span data-ttu-id="c7046-115">[deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c7046-115">[deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) collection</span></span>|<span data-ttu-id="c7046-116">列出 [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c7046-116">List properties and relationships of the [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) objects.</span></span>|
|[<span data-ttu-id="c7046-117">获取 deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="c7046-117">Get deviceManagementScript</span></span>](../api/intune-shared-devicemanagementscript-get.md)|[<span data-ttu-id="c7046-118">deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="c7046-118">deviceManagementScript</span></span>](../resources/intune-shared-devicemanagementscript.md)|<span data-ttu-id="c7046-119">读取 [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c7046-119">Read properties and relationships of the [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) object.</span></span>|
|[<span data-ttu-id="c7046-120">创建 deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="c7046-120">Create deviceManagementScript</span></span>](../api/intune-shared-devicemanagementscript-create.md)|[<span data-ttu-id="c7046-121">deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="c7046-121">deviceManagementScript</span></span>](../resources/intune-shared-devicemanagementscript.md)|<span data-ttu-id="c7046-122">创建新的 [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c7046-122">Create a new [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) object.</span></span>|
|[<span data-ttu-id="c7046-123">删除 deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="c7046-123">Delete deviceManagementScript</span></span>](../api/intune-shared-devicemanagementscript-delete.md)|<span data-ttu-id="c7046-124">无</span><span class="sxs-lookup"><span data-stu-id="c7046-124">None</span></span>|<span data-ttu-id="c7046-125">删除 [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)。</span><span class="sxs-lookup"><span data-stu-id="c7046-125">Deletes a [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md).</span></span>|
|[<span data-ttu-id="c7046-126">更新 deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="c7046-126">Update deviceManagementScript</span></span>](../api/intune-shared-devicemanagementscript-update.md)|[<span data-ttu-id="c7046-127">deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="c7046-127">deviceManagementScript</span></span>](../resources/intune-shared-devicemanagementscript.md)|<span data-ttu-id="c7046-128">更新 [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c7046-128">Update the properties of a [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) object.</span></span>|
|<span data-ttu-id="c7046-129">**设备管理**</span><span class="sxs-lookup"><span data-stu-id="c7046-129">**Device management**</span></span>|
|[<span data-ttu-id="c7046-130">分配操作</span><span class="sxs-lookup"><span data-stu-id="c7046-130">assign action</span></span>](../api/intune-shared-devicemanagementscript-assign.md)|<span data-ttu-id="c7046-131">无</span><span class="sxs-lookup"><span data-stu-id="c7046-131">None</span></span>|<span data-ttu-id="c7046-132">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c7046-132">Not yet documented</span></span>|
|<span data-ttu-id="c7046-133">**策略集**</span><span class="sxs-lookup"><span data-stu-id="c7046-133">**Policy Set**</span></span>|
|[<span data-ttu-id="c7046-134">hasPayloadLinks 操作</span><span class="sxs-lookup"><span data-stu-id="c7046-134">hasPayloadLinks action</span></span>](../api/intune-shared-devicemanagementscript-haspayloadlinks.md)|<span data-ttu-id="c7046-135">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c7046-135">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) collection</span></span>|<span data-ttu-id="c7046-136">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c7046-136">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="c7046-137">属性</span><span class="sxs-lookup"><span data-stu-id="c7046-137">Properties</span></span>
|<span data-ttu-id="c7046-138">属性</span><span class="sxs-lookup"><span data-stu-id="c7046-138">Property</span></span>|<span data-ttu-id="c7046-139">类型</span><span class="sxs-lookup"><span data-stu-id="c7046-139">Type</span></span>|<span data-ttu-id="c7046-140">说明</span><span class="sxs-lookup"><span data-stu-id="c7046-140">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7046-141">id</span><span class="sxs-lookup"><span data-stu-id="c7046-141">id</span></span>|<span data-ttu-id="c7046-142">String</span><span class="sxs-lookup"><span data-stu-id="c7046-142">String</span></span>|<span data-ttu-id="c7046-143">设备管理脚本的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="c7046-143">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="c7046-144">displayName</span><span class="sxs-lookup"><span data-stu-id="c7046-144">displayName</span></span>|<span data-ttu-id="c7046-145">String</span><span class="sxs-lookup"><span data-stu-id="c7046-145">String</span></span>|<span data-ttu-id="c7046-146">设备管理脚本的名称。</span><span class="sxs-lookup"><span data-stu-id="c7046-146">Name of the device management script.</span></span>|
|<span data-ttu-id="c7046-147">说明</span><span class="sxs-lookup"><span data-stu-id="c7046-147">description</span></span>|<span data-ttu-id="c7046-148">String</span><span class="sxs-lookup"><span data-stu-id="c7046-148">String</span></span>|<span data-ttu-id="c7046-149">设备管理脚本的可选说明。</span><span class="sxs-lookup"><span data-stu-id="c7046-149">Optional description for the device management script.</span></span>|
|<span data-ttu-id="c7046-150">scriptContent</span><span class="sxs-lookup"><span data-stu-id="c7046-150">scriptContent</span></span>|<span data-ttu-id="c7046-151">Binary</span><span class="sxs-lookup"><span data-stu-id="c7046-151">Binary</span></span>|<span data-ttu-id="c7046-152">脚本内容。</span><span class="sxs-lookup"><span data-stu-id="c7046-152">The script content.</span></span>|
|<span data-ttu-id="c7046-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c7046-153">createdDateTime</span></span>|<span data-ttu-id="c7046-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7046-154">DateTimeOffset</span></span>|<span data-ttu-id="c7046-155">设备管理脚本的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="c7046-155">The date and time the device management script was created.</span></span> <span data-ttu-id="c7046-156">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c7046-156">This property is read-only.</span></span>|
|<span data-ttu-id="c7046-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c7046-157">lastModifiedDateTime</span></span>|<span data-ttu-id="c7046-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7046-158">DateTimeOffset</span></span>|<span data-ttu-id="c7046-159">上次修改设备管理脚本的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="c7046-159">The date and time the device management script was last modified.</span></span> <span data-ttu-id="c7046-160">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c7046-160">This property is read-only.</span></span>|
|<span data-ttu-id="c7046-161">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="c7046-161">runAsAccount</span></span>|[<span data-ttu-id="c7046-162">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="c7046-162">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="c7046-163">指示执行上下文的类型。</span><span class="sxs-lookup"><span data-stu-id="c7046-163">Indicates the type of execution context.</span></span> <span data-ttu-id="c7046-164">可取值为：`system`、`user`。</span><span class="sxs-lookup"><span data-stu-id="c7046-164">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="c7046-165">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="c7046-165">enforceSignatureCheck</span></span>|<span data-ttu-id="c7046-166">布尔</span><span class="sxs-lookup"><span data-stu-id="c7046-166">Boolean</span></span>|<span data-ttu-id="c7046-167">指示是否需要检查脚本签名。</span><span class="sxs-lookup"><span data-stu-id="c7046-167">Indicate whether the script signature needs be checked.</span></span>|
|<span data-ttu-id="c7046-168">fileName</span><span class="sxs-lookup"><span data-stu-id="c7046-168">fileName</span></span>|<span data-ttu-id="c7046-169">String</span><span class="sxs-lookup"><span data-stu-id="c7046-169">String</span></span>|<span data-ttu-id="c7046-170">脚本文件名。</span><span class="sxs-lookup"><span data-stu-id="c7046-170">Script file name.</span></span>|
|<span data-ttu-id="c7046-171">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c7046-171">roleScopeTagIds</span></span>|<span data-ttu-id="c7046-172">String collection</span><span class="sxs-lookup"><span data-stu-id="c7046-172">String collection</span></span>|<span data-ttu-id="c7046-173">此 PowerShellScript 实例的范围标记 Id 的列表。</span><span class="sxs-lookup"><span data-stu-id="c7046-173">List of Scope Tag IDs for this PowerShellScript instance.</span></span>|
|<span data-ttu-id="c7046-174">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="c7046-174">runAs32Bit</span></span>|<span data-ttu-id="c7046-175">布尔</span><span class="sxs-lookup"><span data-stu-id="c7046-175">Boolean</span></span>|<span data-ttu-id="c7046-176">一个指示 PowerShell 脚本是否应作为32位运行的值</span><span class="sxs-lookup"><span data-stu-id="c7046-176">A value indicating whether the PowerShell script should run as 32-bit</span></span>|

## <a name="relationships"></a><span data-ttu-id="c7046-177">关系</span><span class="sxs-lookup"><span data-stu-id="c7046-177">Relationships</span></span>
|<span data-ttu-id="c7046-178">关系</span><span class="sxs-lookup"><span data-stu-id="c7046-178">Relationship</span></span>|<span data-ttu-id="c7046-179">类型</span><span class="sxs-lookup"><span data-stu-id="c7046-179">Type</span></span>|<span data-ttu-id="c7046-180">说明</span><span class="sxs-lookup"><span data-stu-id="c7046-180">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7046-181">**设备管理**</span><span class="sxs-lookup"><span data-stu-id="c7046-181">**Device management**</span></span>|
|<span data-ttu-id="c7046-182">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="c7046-182">groupAssignments</span></span>|<span data-ttu-id="c7046-183">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c7046-183">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) collection</span></span>|<span data-ttu-id="c7046-184">设备管理脚本的组分配的列表。</span><span class="sxs-lookup"><span data-stu-id="c7046-184">The list of group assignments for the device management script.</span></span>|
|<span data-ttu-id="c7046-185">assignments</span><span class="sxs-lookup"><span data-stu-id="c7046-185">assignments</span></span>|<span data-ttu-id="c7046-186">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c7046-186">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) collection</span></span>|<span data-ttu-id="c7046-187">设备管理脚本的组分配的列表。</span><span class="sxs-lookup"><span data-stu-id="c7046-187">The list of group assignments for the device management script.</span></span>|
|<span data-ttu-id="c7046-188">runSummary</span><span class="sxs-lookup"><span data-stu-id="c7046-188">runSummary</span></span>|[<span data-ttu-id="c7046-189">deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="c7046-189">deviceManagementScriptRunSummary</span></span>](../resources/intune-devices-devicemanagementscriptrunsummary.md)|<span data-ttu-id="c7046-190">设备管理脚本的运行摘要。</span><span class="sxs-lookup"><span data-stu-id="c7046-190">Run summary for device management script.</span></span>|
|<span data-ttu-id="c7046-191">deviceRunStates</span><span class="sxs-lookup"><span data-stu-id="c7046-191">deviceRunStates</span></span>|<span data-ttu-id="c7046-192">[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c7046-192">[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) collection</span></span>|<span data-ttu-id="c7046-193">此脚本在所有设备上的运行状态列表。</span><span class="sxs-lookup"><span data-stu-id="c7046-193">List of run states for this script across all devices.</span></span>|
|<span data-ttu-id="c7046-194">userRunStates</span><span class="sxs-lookup"><span data-stu-id="c7046-194">userRunStates</span></span>|<span data-ttu-id="c7046-195">[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c7046-195">[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) collection</span></span>|<span data-ttu-id="c7046-196">此脚本在所有用户中的运行状态列表。</span><span class="sxs-lookup"><span data-stu-id="c7046-196">List of run states for this script across all users.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c7046-197">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c7046-197">JSON Representation</span></span>
<span data-ttu-id="c7046-198">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c7046-198">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementScript"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementScript",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "scriptContent": "binary",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "runAsAccount": "String",
  "enforceSignatureCheck": true,
  "fileName": "String",
  "roleScopeTagIds": [
    "String"
  ],
  "runAs32Bit": true
}
```





