---
title: deviceManagementScript 资源类型
description: Intune 将向客户提供在已注册的 windows 10 Azure Active Directory 联接设备上运行其 Powershell 脚本的功能。 脚本可以运行一次，也可以定期运行。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4e0a3a4bebaa36ef1f2818b6ced6a9836d6ceb8a
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538733"
---
# <a name="devicemanagementscript-resource-type"></a><span data-ttu-id="75875-104">deviceManagementScript 资源类型</span><span class="sxs-lookup"><span data-stu-id="75875-104">deviceManagementScript resource type</span></span>

> <span data-ttu-id="75875-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="75875-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="75875-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="75875-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="75875-107">Intune 将向客户提供在已注册的 windows 10 Azure Active Directory 联接设备上运行其 Powershell 脚本的功能。</span><span class="sxs-lookup"><span data-stu-id="75875-107">Intune will provide customer the ability to run their Powershell scripts on the enrolled windows 10 Azure Active Directory joined devices.</span></span> <span data-ttu-id="75875-108">脚本可以运行一次，也可以定期运行。</span><span class="sxs-lookup"><span data-stu-id="75875-108">The script can be run once or periodically.</span></span>

## <a name="methods"></a><span data-ttu-id="75875-109">方法</span><span class="sxs-lookup"><span data-stu-id="75875-109">Methods</span></span>
|<span data-ttu-id="75875-110">方法</span><span class="sxs-lookup"><span data-stu-id="75875-110">Method</span></span>|<span data-ttu-id="75875-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="75875-111">Return Type</span></span>|<span data-ttu-id="75875-112">说明</span><span class="sxs-lookup"><span data-stu-id="75875-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="75875-113">列出 deviceManagementScripts</span><span class="sxs-lookup"><span data-stu-id="75875-113">List deviceManagementScripts</span></span>](../api/intune-shared-devicemanagementscript-list.md)|<span data-ttu-id="75875-114">[deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)集合</span><span class="sxs-lookup"><span data-stu-id="75875-114">[deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) collection</span></span>|<span data-ttu-id="75875-115">列出[deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="75875-115">List properties and relationships of the [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) objects.</span></span>|
|[<span data-ttu-id="75875-116">获取 deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="75875-116">Get deviceManagementScript</span></span>](../api/intune-shared-devicemanagementscript-get.md)|[<span data-ttu-id="75875-117">deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="75875-117">deviceManagementScript</span></span>](../resources/intune-shared-devicemanagementscript.md)|<span data-ttu-id="75875-118">读取[deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="75875-118">Read properties and relationships of the [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) object.</span></span>|
|[<span data-ttu-id="75875-119">创建 deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="75875-119">Create deviceManagementScript</span></span>](../api/intune-shared-devicemanagementscript-create.md)|[<span data-ttu-id="75875-120">deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="75875-120">deviceManagementScript</span></span>](../resources/intune-shared-devicemanagementscript.md)|<span data-ttu-id="75875-121">创建新的[deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)对象。</span><span class="sxs-lookup"><span data-stu-id="75875-121">Create a new [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) object.</span></span>|
|[<span data-ttu-id="75875-122">删除 deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="75875-122">Delete deviceManagementScript</span></span>](../api/intune-shared-devicemanagementscript-delete.md)|<span data-ttu-id="75875-123">无</span><span class="sxs-lookup"><span data-stu-id="75875-123">None</span></span>|<span data-ttu-id="75875-124">删除[deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)。</span><span class="sxs-lookup"><span data-stu-id="75875-124">Deletes a [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md).</span></span>|
|[<span data-ttu-id="75875-125">更新 deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="75875-125">Update deviceManagementScript</span></span>](../api/intune-shared-devicemanagementscript-update.md)|[<span data-ttu-id="75875-126">deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="75875-126">deviceManagementScript</span></span>](../resources/intune-shared-devicemanagementscript.md)|<span data-ttu-id="75875-127">更新[deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="75875-127">Update the properties of a [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) object.</span></span>|
|<span data-ttu-id="75875-128">**设备管理**</span><span class="sxs-lookup"><span data-stu-id="75875-128">**Device management**</span></span>|
|[<span data-ttu-id="75875-129">分配操作</span><span class="sxs-lookup"><span data-stu-id="75875-129">assign action</span></span>](../api/intune-shared-devicemanagementscript-assign.md)|<span data-ttu-id="75875-130">无</span><span class="sxs-lookup"><span data-stu-id="75875-130">None</span></span>|<span data-ttu-id="75875-131">尚未记录</span><span class="sxs-lookup"><span data-stu-id="75875-131">Not yet documented</span></span>|
|<span data-ttu-id="75875-132">**策略集**</span><span class="sxs-lookup"><span data-stu-id="75875-132">**Policy Set**</span></span>|
|[<span data-ttu-id="75875-133">hasPayloadLinks 操作</span><span class="sxs-lookup"><span data-stu-id="75875-133">hasPayloadLinks action</span></span>](../api/intune-shared-devicemanagementscript-haspayloadlinks.md)|<span data-ttu-id="75875-134">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="75875-134">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) collection</span></span>|<span data-ttu-id="75875-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="75875-135">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="75875-136">属性</span><span class="sxs-lookup"><span data-stu-id="75875-136">Properties</span></span>
|<span data-ttu-id="75875-137">属性</span><span class="sxs-lookup"><span data-stu-id="75875-137">Property</span></span>|<span data-ttu-id="75875-138">类型</span><span class="sxs-lookup"><span data-stu-id="75875-138">Type</span></span>|<span data-ttu-id="75875-139">说明</span><span class="sxs-lookup"><span data-stu-id="75875-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75875-140">id</span><span class="sxs-lookup"><span data-stu-id="75875-140">id</span></span>|<span data-ttu-id="75875-141">字符串</span><span class="sxs-lookup"><span data-stu-id="75875-141">String</span></span>|<span data-ttu-id="75875-142">设备管理脚本的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="75875-142">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="75875-143">displayName</span><span class="sxs-lookup"><span data-stu-id="75875-143">displayName</span></span>|<span data-ttu-id="75875-144">字符串</span><span class="sxs-lookup"><span data-stu-id="75875-144">String</span></span>|<span data-ttu-id="75875-145">设备管理脚本的名称。</span><span class="sxs-lookup"><span data-stu-id="75875-145">Name of the device management script.</span></span>|
|<span data-ttu-id="75875-146">说明</span><span class="sxs-lookup"><span data-stu-id="75875-146">description</span></span>|<span data-ttu-id="75875-147">String</span><span class="sxs-lookup"><span data-stu-id="75875-147">String</span></span>|<span data-ttu-id="75875-148">设备管理脚本的可选说明。</span><span class="sxs-lookup"><span data-stu-id="75875-148">Optional description for the device management script.</span></span>|
|<span data-ttu-id="75875-149">scriptContent</span><span class="sxs-lookup"><span data-stu-id="75875-149">scriptContent</span></span>|<span data-ttu-id="75875-150">Binary</span><span class="sxs-lookup"><span data-stu-id="75875-150">Binary</span></span>|<span data-ttu-id="75875-151">脚本内容。</span><span class="sxs-lookup"><span data-stu-id="75875-151">The script content.</span></span>|
|<span data-ttu-id="75875-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="75875-152">createdDateTime</span></span>|<span data-ttu-id="75875-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75875-153">DateTimeOffset</span></span>|<span data-ttu-id="75875-154">设备管理脚本的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="75875-154">The date and time the device management script was created.</span></span> <span data-ttu-id="75875-155">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="75875-155">This property is read-only.</span></span>|
|<span data-ttu-id="75875-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="75875-156">lastModifiedDateTime</span></span>|<span data-ttu-id="75875-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75875-157">DateTimeOffset</span></span>|<span data-ttu-id="75875-158">上次修改设备管理脚本的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="75875-158">The date and time the device management script was last modified.</span></span> <span data-ttu-id="75875-159">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="75875-159">This property is read-only.</span></span>|
|<span data-ttu-id="75875-160">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="75875-160">runAsAccount</span></span>|[<span data-ttu-id="75875-161">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="75875-161">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="75875-162">指示执行上下文的类型。</span><span class="sxs-lookup"><span data-stu-id="75875-162">Indicates the type of execution context.</span></span> <span data-ttu-id="75875-163">可取值为：`system`、`user`。</span><span class="sxs-lookup"><span data-stu-id="75875-163">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="75875-164">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="75875-164">enforceSignatureCheck</span></span>|<span data-ttu-id="75875-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="75875-165">Boolean</span></span>|<span data-ttu-id="75875-166">指示是否需要检查脚本签名。</span><span class="sxs-lookup"><span data-stu-id="75875-166">Indicate whether the script signature needs be checked.</span></span>|
|<span data-ttu-id="75875-167">fileName</span><span class="sxs-lookup"><span data-stu-id="75875-167">fileName</span></span>|<span data-ttu-id="75875-168">String</span><span class="sxs-lookup"><span data-stu-id="75875-168">String</span></span>|<span data-ttu-id="75875-169">脚本文件名。</span><span class="sxs-lookup"><span data-stu-id="75875-169">Script file name.</span></span>|
|<span data-ttu-id="75875-170">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="75875-170">roleScopeTagIds</span></span>|<span data-ttu-id="75875-171">String 集合</span><span class="sxs-lookup"><span data-stu-id="75875-171">String collection</span></span>|<span data-ttu-id="75875-172">此 PowerShellScript 实例的范围标记 Id 的列表。</span><span class="sxs-lookup"><span data-stu-id="75875-172">List of Scope Tag IDs for this PowerShellScript instance.</span></span>|
|<span data-ttu-id="75875-173">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="75875-173">runAs32Bit</span></span>|<span data-ttu-id="75875-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="75875-174">Boolean</span></span>|<span data-ttu-id="75875-175">一个指示 PowerShell 脚本是否应作为32位运行的值</span><span class="sxs-lookup"><span data-stu-id="75875-175">A value indicating whether the PowerShell script should run as 32-bit</span></span>|

## <a name="relationships"></a><span data-ttu-id="75875-176">关系</span><span class="sxs-lookup"><span data-stu-id="75875-176">Relationships</span></span>
|<span data-ttu-id="75875-177">关系</span><span class="sxs-lookup"><span data-stu-id="75875-177">Relationship</span></span>|<span data-ttu-id="75875-178">类型</span><span class="sxs-lookup"><span data-stu-id="75875-178">Type</span></span>|<span data-ttu-id="75875-179">说明</span><span class="sxs-lookup"><span data-stu-id="75875-179">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75875-180">**设备管理**</span><span class="sxs-lookup"><span data-stu-id="75875-180">**Device management**</span></span>|
|<span data-ttu-id="75875-181">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="75875-181">groupAssignments</span></span>|<span data-ttu-id="75875-182">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="75875-182">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) collection</span></span>|<span data-ttu-id="75875-183">设备管理脚本的组分配的列表。</span><span class="sxs-lookup"><span data-stu-id="75875-183">The list of group assignments for the device management script.</span></span>|
|<span data-ttu-id="75875-184">assignments</span><span class="sxs-lookup"><span data-stu-id="75875-184">assignments</span></span>|<span data-ttu-id="75875-185">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="75875-185">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) collection</span></span>|<span data-ttu-id="75875-186">设备管理脚本的组分配的列表。</span><span class="sxs-lookup"><span data-stu-id="75875-186">The list of group assignments for the device management script.</span></span>|
|<span data-ttu-id="75875-187">runSummary</span><span class="sxs-lookup"><span data-stu-id="75875-187">runSummary</span></span>|[<span data-ttu-id="75875-188">deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="75875-188">deviceManagementScriptRunSummary</span></span>](../resources/intune-devices-devicemanagementscriptrunsummary.md)|<span data-ttu-id="75875-189">设备管理脚本的运行摘要。</span><span class="sxs-lookup"><span data-stu-id="75875-189">Run summary for device management script.</span></span>|
|<span data-ttu-id="75875-190">deviceRunStates</span><span class="sxs-lookup"><span data-stu-id="75875-190">deviceRunStates</span></span>|<span data-ttu-id="75875-191">[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)集合</span><span class="sxs-lookup"><span data-stu-id="75875-191">[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) collection</span></span>|<span data-ttu-id="75875-192">此脚本在所有设备上的运行状态列表。</span><span class="sxs-lookup"><span data-stu-id="75875-192">List of run states for this script across all devices.</span></span>|
|<span data-ttu-id="75875-193">userRunStates</span><span class="sxs-lookup"><span data-stu-id="75875-193">userRunStates</span></span>|<span data-ttu-id="75875-194">[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)集合</span><span class="sxs-lookup"><span data-stu-id="75875-194">[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) collection</span></span>|<span data-ttu-id="75875-195">此脚本在所有用户中的运行状态列表。</span><span class="sxs-lookup"><span data-stu-id="75875-195">List of run states for this script across all users.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="75875-196">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="75875-196">JSON Representation</span></span>
<span data-ttu-id="75875-197">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="75875-197">Here is a JSON representation of the resource.</span></span>
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
  "runSchedule": {
    "@odata.type": "microsoft.graph.runSchedule"
  },
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



