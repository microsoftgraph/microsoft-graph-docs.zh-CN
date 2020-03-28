---
title: deviceShellScript 资源类型
description: Intune 将向客户提供在已注册的 Mac OS 设备上运行其命令行管理程序脚本的功能。 脚本可以运行一次，也可以定期运行。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f6f1fd1f5a543a3caa3e0fcbf53272ea12d4c572
ms.sourcegitcommit: d93fcc2212491567f8322b1cc0c02d37829b6051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/28/2020
ms.locfileid: "43034788"
---
# <a name="deviceshellscript-resource-type"></a><span data-ttu-id="2b6d9-104">deviceShellScript 资源类型</span><span class="sxs-lookup"><span data-stu-id="2b6d9-104">deviceShellScript resource type</span></span>

> <span data-ttu-id="2b6d9-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2b6d9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2b6d9-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2b6d9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2b6d9-107">Intune 将向客户提供在已注册的 Mac OS 设备上运行其命令行管理程序脚本的功能。</span><span class="sxs-lookup"><span data-stu-id="2b6d9-107">Intune will provide customer the ability to run their Shell scripts on the enrolled Mac OS devices.</span></span> <span data-ttu-id="2b6d9-108">脚本可以运行一次，也可以定期运行。</span><span class="sxs-lookup"><span data-stu-id="2b6d9-108">The script can be run once or periodically.</span></span>

## <a name="methods"></a><span data-ttu-id="2b6d9-109">Methods</span><span class="sxs-lookup"><span data-stu-id="2b6d9-109">Methods</span></span>
|<span data-ttu-id="2b6d9-110">方法</span><span class="sxs-lookup"><span data-stu-id="2b6d9-110">Method</span></span>|<span data-ttu-id="2b6d9-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="2b6d9-111">Return Type</span></span>|<span data-ttu-id="2b6d9-112">说明</span><span class="sxs-lookup"><span data-stu-id="2b6d9-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2b6d9-113">列出 deviceShellScripts</span><span class="sxs-lookup"><span data-stu-id="2b6d9-113">List deviceShellScripts</span></span>](../api/intune-devices-deviceshellscript-list.md)|<span data-ttu-id="2b6d9-114">[deviceShellScript](../resources/intune-devices-deviceshellscript.md)集合</span><span class="sxs-lookup"><span data-stu-id="2b6d9-114">[deviceShellScript](../resources/intune-devices-deviceshellscript.md) collection</span></span>|<span data-ttu-id="2b6d9-115">列出[deviceShellScript](../resources/intune-devices-deviceshellscript.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2b6d9-115">List properties and relationships of the [deviceShellScript](../resources/intune-devices-deviceshellscript.md) objects.</span></span>|
|[<span data-ttu-id="2b6d9-116">获取 deviceShellScript</span><span class="sxs-lookup"><span data-stu-id="2b6d9-116">Get deviceShellScript</span></span>](../api/intune-devices-deviceshellscript-get.md)|[<span data-ttu-id="2b6d9-117">deviceShellScript</span><span class="sxs-lookup"><span data-stu-id="2b6d9-117">deviceShellScript</span></span>](../resources/intune-devices-deviceshellscript.md)|<span data-ttu-id="2b6d9-118">读取[deviceShellScript](../resources/intune-devices-deviceshellscript.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2b6d9-118">Read properties and relationships of the [deviceShellScript](../resources/intune-devices-deviceshellscript.md) object.</span></span>|
|[<span data-ttu-id="2b6d9-119">创建 deviceShellScript</span><span class="sxs-lookup"><span data-stu-id="2b6d9-119">Create deviceShellScript</span></span>](../api/intune-devices-deviceshellscript-create.md)|[<span data-ttu-id="2b6d9-120">deviceShellScript</span><span class="sxs-lookup"><span data-stu-id="2b6d9-120">deviceShellScript</span></span>](../resources/intune-devices-deviceshellscript.md)|<span data-ttu-id="2b6d9-121">创建新的[deviceShellScript](../resources/intune-devices-deviceshellscript.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2b6d9-121">Create a new [deviceShellScript](../resources/intune-devices-deviceshellscript.md) object.</span></span>|
|[<span data-ttu-id="2b6d9-122">删除 deviceShellScript</span><span class="sxs-lookup"><span data-stu-id="2b6d9-122">Delete deviceShellScript</span></span>](../api/intune-devices-deviceshellscript-delete.md)|<span data-ttu-id="2b6d9-123">无</span><span class="sxs-lookup"><span data-stu-id="2b6d9-123">None</span></span>|<span data-ttu-id="2b6d9-124">删除[deviceShellScript](../resources/intune-devices-deviceshellscript.md)。</span><span class="sxs-lookup"><span data-stu-id="2b6d9-124">Deletes a [deviceShellScript](../resources/intune-devices-deviceshellscript.md).</span></span>|
|[<span data-ttu-id="2b6d9-125">更新 deviceShellScript</span><span class="sxs-lookup"><span data-stu-id="2b6d9-125">Update deviceShellScript</span></span>](../api/intune-devices-deviceshellscript-update.md)|[<span data-ttu-id="2b6d9-126">deviceShellScript</span><span class="sxs-lookup"><span data-stu-id="2b6d9-126">deviceShellScript</span></span>](../resources/intune-devices-deviceshellscript.md)|<span data-ttu-id="2b6d9-127">更新[deviceShellScript](../resources/intune-devices-deviceshellscript.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="2b6d9-127">Update the properties of a [deviceShellScript](../resources/intune-devices-deviceshellscript.md) object.</span></span>|
|[<span data-ttu-id="2b6d9-128">分配操作</span><span class="sxs-lookup"><span data-stu-id="2b6d9-128">assign action</span></span>](../api/intune-devices-deviceshellscript-assign.md)|<span data-ttu-id="2b6d9-129">无</span><span class="sxs-lookup"><span data-stu-id="2b6d9-129">None</span></span>|<span data-ttu-id="2b6d9-130">尚未记录</span><span class="sxs-lookup"><span data-stu-id="2b6d9-130">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="2b6d9-131">属性</span><span class="sxs-lookup"><span data-stu-id="2b6d9-131">Properties</span></span>
|<span data-ttu-id="2b6d9-132">属性</span><span class="sxs-lookup"><span data-stu-id="2b6d9-132">Property</span></span>|<span data-ttu-id="2b6d9-133">类型</span><span class="sxs-lookup"><span data-stu-id="2b6d9-133">Type</span></span>|<span data-ttu-id="2b6d9-134">Description</span><span class="sxs-lookup"><span data-stu-id="2b6d9-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b6d9-135">executionFrequency</span><span class="sxs-lookup"><span data-stu-id="2b6d9-135">executionFrequency</span></span>|<span data-ttu-id="2b6d9-136">持续时间</span><span class="sxs-lookup"><span data-stu-id="2b6d9-136">Duration</span></span>|<span data-ttu-id="2b6d9-137">脚本运行的间隔。</span><span class="sxs-lookup"><span data-stu-id="2b6d9-137">The interval for script to run.</span></span> <span data-ttu-id="2b6d9-138">如果未定义，脚本将运行一次。</span><span class="sxs-lookup"><span data-stu-id="2b6d9-138">If not defined the script runs once.</span></span>|
|<span data-ttu-id="2b6d9-139">retryCount</span><span class="sxs-lookup"><span data-stu-id="2b6d9-139">retryCount</span></span>|<span data-ttu-id="2b6d9-140">Int32</span><span class="sxs-lookup"><span data-stu-id="2b6d9-140">Int32</span></span>|<span data-ttu-id="2b6d9-141">脚本失败时重试脚本的次数。</span><span class="sxs-lookup"><span data-stu-id="2b6d9-141">The number of times for the script to be retried if it fails.</span></span>|
|<span data-ttu-id="2b6d9-142">blockExecutionNotifications</span><span class="sxs-lookup"><span data-stu-id="2b6d9-142">blockExecutionNotifications</span></span>|<span data-ttu-id="2b6d9-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b6d9-143">Boolean</span></span>|<span data-ttu-id="2b6d9-144">指示在脚本运行时是否通知用户。</span><span class="sxs-lookup"><span data-stu-id="2b6d9-144">Indicates whether the user is notified when a script runs.</span></span>|
|<span data-ttu-id="2b6d9-145">id</span><span class="sxs-lookup"><span data-stu-id="2b6d9-145">id</span></span>|<span data-ttu-id="2b6d9-146">字符串</span><span class="sxs-lookup"><span data-stu-id="2b6d9-146">String</span></span>|<span data-ttu-id="2b6d9-147">设备管理脚本的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="2b6d9-147">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="2b6d9-148">displayName</span><span class="sxs-lookup"><span data-stu-id="2b6d9-148">displayName</span></span>|<span data-ttu-id="2b6d9-149">字符串</span><span class="sxs-lookup"><span data-stu-id="2b6d9-149">String</span></span>|<span data-ttu-id="2b6d9-150">设备管理脚本的名称。</span><span class="sxs-lookup"><span data-stu-id="2b6d9-150">The name of the device management script.</span></span>|
|<span data-ttu-id="2b6d9-151">description</span><span class="sxs-lookup"><span data-stu-id="2b6d9-151">description</span></span>|<span data-ttu-id="2b6d9-152">String</span><span class="sxs-lookup"><span data-stu-id="2b6d9-152">String</span></span>|<span data-ttu-id="2b6d9-153">设备管理脚本的可选说明。</span><span class="sxs-lookup"><span data-stu-id="2b6d9-153">Optional description for the device management script.</span></span>|
|<span data-ttu-id="2b6d9-154">scriptContent</span><span class="sxs-lookup"><span data-stu-id="2b6d9-154">scriptContent</span></span>|<span data-ttu-id="2b6d9-155">Binary</span><span class="sxs-lookup"><span data-stu-id="2b6d9-155">Binary</span></span>|<span data-ttu-id="2b6d9-156">脚本内容。</span><span class="sxs-lookup"><span data-stu-id="2b6d9-156">The script content.</span></span>|
|<span data-ttu-id="2b6d9-157">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2b6d9-157">createdDateTime</span></span>|<span data-ttu-id="2b6d9-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2b6d9-158">DateTimeOffset</span></span>|<span data-ttu-id="2b6d9-159">设备管理脚本的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="2b6d9-159">The date and time the device management script was created.</span></span> <span data-ttu-id="2b6d9-160">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="2b6d9-160">This property is read-only.</span></span>|
|<span data-ttu-id="2b6d9-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2b6d9-161">lastModifiedDateTime</span></span>|<span data-ttu-id="2b6d9-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2b6d9-162">DateTimeOffset</span></span>|<span data-ttu-id="2b6d9-163">上次修改设备管理脚本的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="2b6d9-163">The date and time the device management script was last modified.</span></span> <span data-ttu-id="2b6d9-164">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="2b6d9-164">This property is read-only.</span></span>|
|<span data-ttu-id="2b6d9-165">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="2b6d9-165">runAsAccount</span></span>|[<span data-ttu-id="2b6d9-166">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="2b6d9-166">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="2b6d9-167">指示执行上下文的类型。</span><span class="sxs-lookup"><span data-stu-id="2b6d9-167">Indicates the type of execution context.</span></span> <span data-ttu-id="2b6d9-168">可取值为：`system`、`user`。</span><span class="sxs-lookup"><span data-stu-id="2b6d9-168">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="2b6d9-169">fileName</span><span class="sxs-lookup"><span data-stu-id="2b6d9-169">fileName</span></span>|<span data-ttu-id="2b6d9-170">String</span><span class="sxs-lookup"><span data-stu-id="2b6d9-170">String</span></span>|<span data-ttu-id="2b6d9-171">脚本文件名。</span><span class="sxs-lookup"><span data-stu-id="2b6d9-171">The script file name.</span></span>|
|<span data-ttu-id="2b6d9-172">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2b6d9-172">roleScopeTagIds</span></span>|<span data-ttu-id="2b6d9-173">String 集合</span><span class="sxs-lookup"><span data-stu-id="2b6d9-173">String collection</span></span>|<span data-ttu-id="2b6d9-174">此 PowerShellScript 实例的范围标记 Id 的列表。</span><span class="sxs-lookup"><span data-stu-id="2b6d9-174">The list of Scope Tag IDs for this PowerShellScript instance.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2b6d9-175">关系</span><span class="sxs-lookup"><span data-stu-id="2b6d9-175">Relationships</span></span>
|<span data-ttu-id="2b6d9-176">关系</span><span class="sxs-lookup"><span data-stu-id="2b6d9-176">Relationship</span></span>|<span data-ttu-id="2b6d9-177">类型</span><span class="sxs-lookup"><span data-stu-id="2b6d9-177">Type</span></span>|<span data-ttu-id="2b6d9-178">Description</span><span class="sxs-lookup"><span data-stu-id="2b6d9-178">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b6d9-179">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="2b6d9-179">groupAssignments</span></span>|<span data-ttu-id="2b6d9-180">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="2b6d9-180">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) collection</span></span>|<span data-ttu-id="2b6d9-181">设备管理脚本的组分配的列表。</span><span class="sxs-lookup"><span data-stu-id="2b6d9-181">The list of group assignments for the device management script.</span></span>|
|<span data-ttu-id="2b6d9-182">assignments</span><span class="sxs-lookup"><span data-stu-id="2b6d9-182">assignments</span></span>|<span data-ttu-id="2b6d9-183">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="2b6d9-183">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) collection</span></span>|<span data-ttu-id="2b6d9-184">设备管理脚本的组分配的列表。</span><span class="sxs-lookup"><span data-stu-id="2b6d9-184">The list of group assignments for the device management script.</span></span>|
|<span data-ttu-id="2b6d9-185">runSummary</span><span class="sxs-lookup"><span data-stu-id="2b6d9-185">runSummary</span></span>|[<span data-ttu-id="2b6d9-186">deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="2b6d9-186">deviceManagementScriptRunSummary</span></span>](../resources/intune-devices-devicemanagementscriptrunsummary.md)|<span data-ttu-id="2b6d9-187">设备管理脚本的运行摘要。</span><span class="sxs-lookup"><span data-stu-id="2b6d9-187">Run summary for device management script.</span></span>|
|<span data-ttu-id="2b6d9-188">deviceRunStates</span><span class="sxs-lookup"><span data-stu-id="2b6d9-188">deviceRunStates</span></span>|<span data-ttu-id="2b6d9-189">[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)集合</span><span class="sxs-lookup"><span data-stu-id="2b6d9-189">[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) collection</span></span>|<span data-ttu-id="2b6d9-190">此脚本在所有设备上的运行状态列表。</span><span class="sxs-lookup"><span data-stu-id="2b6d9-190">List of run states for this script across all devices.</span></span>|
|<span data-ttu-id="2b6d9-191">userRunStates</span><span class="sxs-lookup"><span data-stu-id="2b6d9-191">userRunStates</span></span>|<span data-ttu-id="2b6d9-192">[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)集合</span><span class="sxs-lookup"><span data-stu-id="2b6d9-192">[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) collection</span></span>|<span data-ttu-id="2b6d9-193">此脚本在所有用户中的运行状态列表。</span><span class="sxs-lookup"><span data-stu-id="2b6d9-193">List of run states for this script across all users.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2b6d9-194">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2b6d9-194">JSON Representation</span></span>
<span data-ttu-id="2b6d9-195">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2b6d9-195">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceShellScript"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceShellScript",
  "executionFrequency": "String (duration)",
  "retryCount": 1024,
  "blockExecutionNotifications": true,
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "scriptContent": "binary",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "runAsAccount": "String",
  "fileName": "String",
  "roleScopeTagIds": [
    "String"
  ]
}
```



