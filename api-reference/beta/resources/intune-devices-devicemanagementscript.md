---
title: deviceManagementScript 资源类型
description: Intune 将向客户提供在已注册的 windows 10 Azure Active Directory 联接设备上运行其 Powershell 脚本的功能。 脚本可以运行一次, 也可以定期运行。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6599f0dbc083859bef4f7a334d36fdcdfa63ee86
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31801594"
---
# <a name="devicemanagementscript-resource-type"></a><span data-ttu-id="43cf7-104">deviceManagementScript 资源类型</span><span class="sxs-lookup"><span data-stu-id="43cf7-104">deviceManagementScript resource type</span></span>

> <span data-ttu-id="43cf7-105">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="43cf7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="43cf7-106">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="43cf7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="43cf7-107">Intune 将向客户提供在已注册的 windows 10 Azure Active Directory 联接设备上运行其 Powershell 脚本的功能。</span><span class="sxs-lookup"><span data-stu-id="43cf7-107">Intune will provide customer the ability to run their Powershell scripts on the enrolled windows 10 Azure Active Directory joined devices.</span></span> <span data-ttu-id="43cf7-108">脚本可以运行一次, 也可以定期运行。</span><span class="sxs-lookup"><span data-stu-id="43cf7-108">The script can be run once or periodically.</span></span>

## <a name="methods"></a><span data-ttu-id="43cf7-109">方法</span><span class="sxs-lookup"><span data-stu-id="43cf7-109">Methods</span></span>
|<span data-ttu-id="43cf7-110">方法</span><span class="sxs-lookup"><span data-stu-id="43cf7-110">Method</span></span>|<span data-ttu-id="43cf7-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="43cf7-111">Return Type</span></span>|<span data-ttu-id="43cf7-112">说明</span><span class="sxs-lookup"><span data-stu-id="43cf7-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="43cf7-113">列出 deviceManagementScripts</span><span class="sxs-lookup"><span data-stu-id="43cf7-113">List deviceManagementScripts</span></span>](../api/intune-devices-devicemanagementscript-list.md)|<span data-ttu-id="43cf7-114">[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)集合</span><span class="sxs-lookup"><span data-stu-id="43cf7-114">[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) collection</span></span>|<span data-ttu-id="43cf7-115">列出[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="43cf7-115">List properties and relationships of the [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) objects.</span></span>|
|[<span data-ttu-id="43cf7-116">获取 deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="43cf7-116">Get deviceManagementScript</span></span>](../api/intune-devices-devicemanagementscript-get.md)|[<span data-ttu-id="43cf7-117">deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="43cf7-117">deviceManagementScript</span></span>](../resources/intune-devices-devicemanagementscript.md)|<span data-ttu-id="43cf7-118">读取[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="43cf7-118">Read properties and relationships of the [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object.</span></span>|
|[<span data-ttu-id="43cf7-119">创建 deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="43cf7-119">Create deviceManagementScript</span></span>](../api/intune-devices-devicemanagementscript-create.md)|[<span data-ttu-id="43cf7-120">deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="43cf7-120">deviceManagementScript</span></span>](../resources/intune-devices-devicemanagementscript.md)|<span data-ttu-id="43cf7-121">创建新的[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)对象。</span><span class="sxs-lookup"><span data-stu-id="43cf7-121">Create a new [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object.</span></span>|
|[<span data-ttu-id="43cf7-122">删除 deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="43cf7-122">Delete deviceManagementScript</span></span>](../api/intune-devices-devicemanagementscript-delete.md)|<span data-ttu-id="43cf7-123">无</span><span class="sxs-lookup"><span data-stu-id="43cf7-123">None</span></span>|<span data-ttu-id="43cf7-124">删除[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)。</span><span class="sxs-lookup"><span data-stu-id="43cf7-124">Deletes a [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md).</span></span>|
|[<span data-ttu-id="43cf7-125">更新 deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="43cf7-125">Update deviceManagementScript</span></span>](../api/intune-devices-devicemanagementscript-update.md)|[<span data-ttu-id="43cf7-126">deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="43cf7-126">deviceManagementScript</span></span>](../resources/intune-devices-devicemanagementscript.md)|<span data-ttu-id="43cf7-127">更新[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="43cf7-127">Update the properties of a [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object.</span></span>|
|[<span data-ttu-id="43cf7-128">分配操作</span><span class="sxs-lookup"><span data-stu-id="43cf7-128">assign action</span></span>](../api/intune-devices-devicemanagementscript-assign.md)|<span data-ttu-id="43cf7-129">无</span><span class="sxs-lookup"><span data-stu-id="43cf7-129">None</span></span>|<span data-ttu-id="43cf7-130">尚未记录</span><span class="sxs-lookup"><span data-stu-id="43cf7-130">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="43cf7-131">属性</span><span class="sxs-lookup"><span data-stu-id="43cf7-131">Properties</span></span>
|<span data-ttu-id="43cf7-132">属性</span><span class="sxs-lookup"><span data-stu-id="43cf7-132">Property</span></span>|<span data-ttu-id="43cf7-133">类型</span><span class="sxs-lookup"><span data-stu-id="43cf7-133">Type</span></span>|<span data-ttu-id="43cf7-134">说明</span><span class="sxs-lookup"><span data-stu-id="43cf7-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43cf7-135">id</span><span class="sxs-lookup"><span data-stu-id="43cf7-135">id</span></span>|<span data-ttu-id="43cf7-136">String</span><span class="sxs-lookup"><span data-stu-id="43cf7-136">String</span></span>|<span data-ttu-id="43cf7-137">设备管理脚本的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="43cf7-137">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="43cf7-138">displayName</span><span class="sxs-lookup"><span data-stu-id="43cf7-138">displayName</span></span>|<span data-ttu-id="43cf7-139">String</span><span class="sxs-lookup"><span data-stu-id="43cf7-139">String</span></span>|<span data-ttu-id="43cf7-140">设备管理脚本的名称。</span><span class="sxs-lookup"><span data-stu-id="43cf7-140">Name of the device management script.</span></span>|
|<span data-ttu-id="43cf7-141">description</span><span class="sxs-lookup"><span data-stu-id="43cf7-141">description</span></span>|<span data-ttu-id="43cf7-142">String</span><span class="sxs-lookup"><span data-stu-id="43cf7-142">String</span></span>|<span data-ttu-id="43cf7-143">设备管理脚本的可选说明。</span><span class="sxs-lookup"><span data-stu-id="43cf7-143">Optional description for the device management script.</span></span>|
|<span data-ttu-id="43cf7-144">runSchedule</span><span class="sxs-lookup"><span data-stu-id="43cf7-144">runSchedule</span></span>|[<span data-ttu-id="43cf7-145">runSchedule</span><span class="sxs-lookup"><span data-stu-id="43cf7-145">runSchedule</span></span>](../resources/intune-devices-runschedule.md)|<span data-ttu-id="43cf7-146">脚本运行的间隔。</span><span class="sxs-lookup"><span data-stu-id="43cf7-146">The interval for script to run.</span></span> <span data-ttu-id="43cf7-147">如果未定义, 脚本将运行一次</span><span class="sxs-lookup"><span data-stu-id="43cf7-147">If not defined the script will run once</span></span>|
|<span data-ttu-id="43cf7-148">scriptContent</span><span class="sxs-lookup"><span data-stu-id="43cf7-148">scriptContent</span></span>|<span data-ttu-id="43cf7-149">Binary</span><span class="sxs-lookup"><span data-stu-id="43cf7-149">Binary</span></span>|<span data-ttu-id="43cf7-150">脚本内容。</span><span class="sxs-lookup"><span data-stu-id="43cf7-150">The script content.</span></span>|
|<span data-ttu-id="43cf7-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="43cf7-151">createdDateTime</span></span>|<span data-ttu-id="43cf7-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="43cf7-152">DateTimeOffset</span></span>|<span data-ttu-id="43cf7-153">设备管理脚本的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="43cf7-153">The date and time the device management script was created.</span></span>|
|<span data-ttu-id="43cf7-154">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="43cf7-154">lastModifiedDateTime</span></span>|<span data-ttu-id="43cf7-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="43cf7-155">DateTimeOffset</span></span>|<span data-ttu-id="43cf7-156">上次修改设备管理脚本的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="43cf7-156">The date and time the device management script was last modified.</span></span>|
|<span data-ttu-id="43cf7-157">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="43cf7-157">runAsAccount</span></span>|[<span data-ttu-id="43cf7-158">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="43cf7-158">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="43cf7-159">指示执行上下文的类型。</span><span class="sxs-lookup"><span data-stu-id="43cf7-159">Indicates the type of execution context.</span></span> <span data-ttu-id="43cf7-160">可取值为：`system`、`user`。</span><span class="sxs-lookup"><span data-stu-id="43cf7-160">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="43cf7-161">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="43cf7-161">enforceSignatureCheck</span></span>|<span data-ttu-id="43cf7-162">布尔值</span><span class="sxs-lookup"><span data-stu-id="43cf7-162">Boolean</span></span>|<span data-ttu-id="43cf7-163">指示是否需要检查脚本签名。</span><span class="sxs-lookup"><span data-stu-id="43cf7-163">Indicate whether the script signature needs be checked.</span></span>|
|<span data-ttu-id="43cf7-164">fileName</span><span class="sxs-lookup"><span data-stu-id="43cf7-164">fileName</span></span>|<span data-ttu-id="43cf7-165">String</span><span class="sxs-lookup"><span data-stu-id="43cf7-165">String</span></span>|<span data-ttu-id="43cf7-166">脚本文件名。</span><span class="sxs-lookup"><span data-stu-id="43cf7-166">Script file name.</span></span>|
|<span data-ttu-id="43cf7-167">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="43cf7-167">roleScopeTagIds</span></span>|<span data-ttu-id="43cf7-168">String 集合</span><span class="sxs-lookup"><span data-stu-id="43cf7-168">String collection</span></span>|<span data-ttu-id="43cf7-169">此 PowerShellScript 实例的范围标记 id 的列表。</span><span class="sxs-lookup"><span data-stu-id="43cf7-169">List of Scope Tag IDs for this PowerShellScript instance.</span></span>|
|<span data-ttu-id="43cf7-170">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="43cf7-170">runAs32Bit</span></span>|<span data-ttu-id="43cf7-171">布尔值</span><span class="sxs-lookup"><span data-stu-id="43cf7-171">Boolean</span></span>|<span data-ttu-id="43cf7-172">一个指示 PowerShell 脚本是否应作为32位运行的值</span><span class="sxs-lookup"><span data-stu-id="43cf7-172">A value indicating whether the PowerShell script should run as 32-bit</span></span>|

## <a name="relationships"></a><span data-ttu-id="43cf7-173">关系</span><span class="sxs-lookup"><span data-stu-id="43cf7-173">Relationships</span></span>
|<span data-ttu-id="43cf7-174">关系</span><span class="sxs-lookup"><span data-stu-id="43cf7-174">Relationship</span></span>|<span data-ttu-id="43cf7-175">类型</span><span class="sxs-lookup"><span data-stu-id="43cf7-175">Type</span></span>|<span data-ttu-id="43cf7-176">说明</span><span class="sxs-lookup"><span data-stu-id="43cf7-176">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43cf7-177">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="43cf7-177">groupAssignments</span></span>|<span data-ttu-id="43cf7-178">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="43cf7-178">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) collection</span></span>|<span data-ttu-id="43cf7-179">设备管理脚本的组分配的列表。</span><span class="sxs-lookup"><span data-stu-id="43cf7-179">The list of group assignments for the device management script.</span></span>|
|<span data-ttu-id="43cf7-180">assignments</span><span class="sxs-lookup"><span data-stu-id="43cf7-180">assignments</span></span>|<span data-ttu-id="43cf7-181">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="43cf7-181">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) collection</span></span>|<span data-ttu-id="43cf7-182">设备管理脚本的组分配的列表。</span><span class="sxs-lookup"><span data-stu-id="43cf7-182">The list of group assignments for the device management script.</span></span>|
|<span data-ttu-id="43cf7-183">runSummary</span><span class="sxs-lookup"><span data-stu-id="43cf7-183">runSummary</span></span>|[<span data-ttu-id="43cf7-184">deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="43cf7-184">deviceManagementScriptRunSummary</span></span>](../resources/intune-devices-devicemanagementscriptrunsummary.md)|<span data-ttu-id="43cf7-185">设备管理脚本的运行摘要。</span><span class="sxs-lookup"><span data-stu-id="43cf7-185">Run summary for device management script.</span></span>|
|<span data-ttu-id="43cf7-186">deviceRunStates</span><span class="sxs-lookup"><span data-stu-id="43cf7-186">deviceRunStates</span></span>|<span data-ttu-id="43cf7-187">[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)集合</span><span class="sxs-lookup"><span data-stu-id="43cf7-187">[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) collection</span></span>|<span data-ttu-id="43cf7-188">此脚本在所有设备上的运行状态列表。</span><span class="sxs-lookup"><span data-stu-id="43cf7-188">List of run states for this script across all devices.</span></span>|
|<span data-ttu-id="43cf7-189">userRunStates</span><span class="sxs-lookup"><span data-stu-id="43cf7-189">userRunStates</span></span>|<span data-ttu-id="43cf7-190">[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)集合</span><span class="sxs-lookup"><span data-stu-id="43cf7-190">[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) collection</span></span>|<span data-ttu-id="43cf7-191">此脚本在所有用户中的运行状态列表。</span><span class="sxs-lookup"><span data-stu-id="43cf7-191">List of run states for this script across all users.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="43cf7-192">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="43cf7-192">JSON Representation</span></span>
<span data-ttu-id="43cf7-193">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="43cf7-193">Here is a JSON representation of the resource.</span></span>
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





