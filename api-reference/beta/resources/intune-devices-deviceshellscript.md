---
title: deviceShellScript 资源类型
description: Intune 将向客户提供在已注册的 Mac OS 设备上运行其命令行管理程序脚本的功能。 脚本可以运行一次，也可以定期运行。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: de1bd720e244c1b63587a9d63b2dee66a67da0b8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081410"
---
# <a name="deviceshellscript-resource-type"></a><span data-ttu-id="f41af-104">deviceShellScript 资源类型</span><span class="sxs-lookup"><span data-stu-id="f41af-104">deviceShellScript resource type</span></span>

<span data-ttu-id="f41af-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f41af-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f41af-106">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f41af-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f41af-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f41af-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f41af-108">Intune 将向客户提供在已注册的 Mac OS 设备上运行其命令行管理程序脚本的功能。</span><span class="sxs-lookup"><span data-stu-id="f41af-108">Intune will provide customer the ability to run their Shell scripts on the enrolled Mac OS devices.</span></span> <span data-ttu-id="f41af-109">脚本可以运行一次，也可以定期运行。</span><span class="sxs-lookup"><span data-stu-id="f41af-109">The script can be run once or periodically.</span></span>

## <a name="methods"></a><span data-ttu-id="f41af-110">方法</span><span class="sxs-lookup"><span data-stu-id="f41af-110">Methods</span></span>
|<span data-ttu-id="f41af-111">方法</span><span class="sxs-lookup"><span data-stu-id="f41af-111">Method</span></span>|<span data-ttu-id="f41af-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="f41af-112">Return Type</span></span>|<span data-ttu-id="f41af-113">说明</span><span class="sxs-lookup"><span data-stu-id="f41af-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f41af-114">列出 deviceShellScripts</span><span class="sxs-lookup"><span data-stu-id="f41af-114">List deviceShellScripts</span></span>](../api/intune-devices-deviceshellscript-list.md)|<span data-ttu-id="f41af-115">[deviceShellScript](../resources/intune-devices-deviceshellscript.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f41af-115">[deviceShellScript](../resources/intune-devices-deviceshellscript.md) collection</span></span>|<span data-ttu-id="f41af-116">列出 [deviceShellScript](../resources/intune-devices-deviceshellscript.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f41af-116">List properties and relationships of the [deviceShellScript](../resources/intune-devices-deviceshellscript.md) objects.</span></span>|
|[<span data-ttu-id="f41af-117">获取 deviceShellScript</span><span class="sxs-lookup"><span data-stu-id="f41af-117">Get deviceShellScript</span></span>](../api/intune-devices-deviceshellscript-get.md)|[<span data-ttu-id="f41af-118">deviceShellScript</span><span class="sxs-lookup"><span data-stu-id="f41af-118">deviceShellScript</span></span>](../resources/intune-devices-deviceshellscript.md)|<span data-ttu-id="f41af-119">读取 [deviceShellScript](../resources/intune-devices-deviceshellscript.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f41af-119">Read properties and relationships of the [deviceShellScript](../resources/intune-devices-deviceshellscript.md) object.</span></span>|
|[<span data-ttu-id="f41af-120">创建 deviceShellScript</span><span class="sxs-lookup"><span data-stu-id="f41af-120">Create deviceShellScript</span></span>](../api/intune-devices-deviceshellscript-create.md)|[<span data-ttu-id="f41af-121">deviceShellScript</span><span class="sxs-lookup"><span data-stu-id="f41af-121">deviceShellScript</span></span>](../resources/intune-devices-deviceshellscript.md)|<span data-ttu-id="f41af-122">创建新的 [deviceShellScript](../resources/intune-devices-deviceshellscript.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f41af-122">Create a new [deviceShellScript](../resources/intune-devices-deviceshellscript.md) object.</span></span>|
|[<span data-ttu-id="f41af-123">删除 deviceShellScript</span><span class="sxs-lookup"><span data-stu-id="f41af-123">Delete deviceShellScript</span></span>](../api/intune-devices-deviceshellscript-delete.md)|<span data-ttu-id="f41af-124">无</span><span class="sxs-lookup"><span data-stu-id="f41af-124">None</span></span>|<span data-ttu-id="f41af-125">删除 [deviceShellScript](../resources/intune-devices-deviceshellscript.md)。</span><span class="sxs-lookup"><span data-stu-id="f41af-125">Deletes a [deviceShellScript](../resources/intune-devices-deviceshellscript.md).</span></span>|
|[<span data-ttu-id="f41af-126">更新 deviceShellScript</span><span class="sxs-lookup"><span data-stu-id="f41af-126">Update deviceShellScript</span></span>](../api/intune-devices-deviceshellscript-update.md)|[<span data-ttu-id="f41af-127">deviceShellScript</span><span class="sxs-lookup"><span data-stu-id="f41af-127">deviceShellScript</span></span>](../resources/intune-devices-deviceshellscript.md)|<span data-ttu-id="f41af-128">更新 [deviceShellScript](../resources/intune-devices-deviceshellscript.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f41af-128">Update the properties of a [deviceShellScript](../resources/intune-devices-deviceshellscript.md) object.</span></span>|
|[<span data-ttu-id="f41af-129">分配操作</span><span class="sxs-lookup"><span data-stu-id="f41af-129">assign action</span></span>](../api/intune-devices-deviceshellscript-assign.md)|<span data-ttu-id="f41af-130">无</span><span class="sxs-lookup"><span data-stu-id="f41af-130">None</span></span>|<span data-ttu-id="f41af-131">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f41af-131">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="f41af-132">属性</span><span class="sxs-lookup"><span data-stu-id="f41af-132">Properties</span></span>
|<span data-ttu-id="f41af-133">属性</span><span class="sxs-lookup"><span data-stu-id="f41af-133">Property</span></span>|<span data-ttu-id="f41af-134">类型</span><span class="sxs-lookup"><span data-stu-id="f41af-134">Type</span></span>|<span data-ttu-id="f41af-135">说明</span><span class="sxs-lookup"><span data-stu-id="f41af-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f41af-136">executionFrequency</span><span class="sxs-lookup"><span data-stu-id="f41af-136">executionFrequency</span></span>|<span data-ttu-id="f41af-137">持续时间</span><span class="sxs-lookup"><span data-stu-id="f41af-137">Duration</span></span>|<span data-ttu-id="f41af-138">脚本运行的间隔。</span><span class="sxs-lookup"><span data-stu-id="f41af-138">The interval for script to run.</span></span> <span data-ttu-id="f41af-139">如果未定义，脚本将运行一次</span><span class="sxs-lookup"><span data-stu-id="f41af-139">If not defined the script will run once</span></span>|
|<span data-ttu-id="f41af-140">retryCount</span><span class="sxs-lookup"><span data-stu-id="f41af-140">retryCount</span></span>|<span data-ttu-id="f41af-141">Int32</span><span class="sxs-lookup"><span data-stu-id="f41af-141">Int32</span></span>|<span data-ttu-id="f41af-142">脚本失败时将重试脚本的次数</span><span class="sxs-lookup"><span data-stu-id="f41af-142">Number of times for the script to be retried if it fails</span></span>|
|<span data-ttu-id="f41af-143">blockExecutionNotifications</span><span class="sxs-lookup"><span data-stu-id="f41af-143">blockExecutionNotifications</span></span>|<span data-ttu-id="f41af-144">布尔</span><span class="sxs-lookup"><span data-stu-id="f41af-144">Boolean</span></span>|<span data-ttu-id="f41af-145">不通知用户正在执行的脚本</span><span class="sxs-lookup"><span data-stu-id="f41af-145">Does not notify the user a script is being executed</span></span>|
|<span data-ttu-id="f41af-146">id</span><span class="sxs-lookup"><span data-stu-id="f41af-146">id</span></span>|<span data-ttu-id="f41af-147">字符串</span><span class="sxs-lookup"><span data-stu-id="f41af-147">String</span></span>|<span data-ttu-id="f41af-148">设备管理脚本的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="f41af-148">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="f41af-149">displayName</span><span class="sxs-lookup"><span data-stu-id="f41af-149">displayName</span></span>|<span data-ttu-id="f41af-150">字符串</span><span class="sxs-lookup"><span data-stu-id="f41af-150">String</span></span>|<span data-ttu-id="f41af-151">设备管理脚本的名称。</span><span class="sxs-lookup"><span data-stu-id="f41af-151">Name of the device management script.</span></span>|
|<span data-ttu-id="f41af-152">说明</span><span class="sxs-lookup"><span data-stu-id="f41af-152">description</span></span>|<span data-ttu-id="f41af-153">字符串</span><span class="sxs-lookup"><span data-stu-id="f41af-153">String</span></span>|<span data-ttu-id="f41af-154">设备管理脚本的可选说明。</span><span class="sxs-lookup"><span data-stu-id="f41af-154">Optional description for the device management script.</span></span>|
|<span data-ttu-id="f41af-155">scriptContent</span><span class="sxs-lookup"><span data-stu-id="f41af-155">scriptContent</span></span>|<span data-ttu-id="f41af-156">Binary</span><span class="sxs-lookup"><span data-stu-id="f41af-156">Binary</span></span>|<span data-ttu-id="f41af-157">脚本内容。</span><span class="sxs-lookup"><span data-stu-id="f41af-157">The script content.</span></span>|
|<span data-ttu-id="f41af-158">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f41af-158">createdDateTime</span></span>|<span data-ttu-id="f41af-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f41af-159">DateTimeOffset</span></span>|<span data-ttu-id="f41af-160">设备管理脚本的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="f41af-160">The date and time the device management script was created.</span></span> <span data-ttu-id="f41af-161">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="f41af-161">This property is read-only.</span></span>|
|<span data-ttu-id="f41af-162">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f41af-162">lastModifiedDateTime</span></span>|<span data-ttu-id="f41af-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f41af-163">DateTimeOffset</span></span>|<span data-ttu-id="f41af-164">上次修改设备管理脚本的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="f41af-164">The date and time the device management script was last modified.</span></span> <span data-ttu-id="f41af-165">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="f41af-165">This property is read-only.</span></span>|
|<span data-ttu-id="f41af-166">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="f41af-166">runAsAccount</span></span>|[<span data-ttu-id="f41af-167">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="f41af-167">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="f41af-168">指示执行上下文的类型。</span><span class="sxs-lookup"><span data-stu-id="f41af-168">Indicates the type of execution context.</span></span> <span data-ttu-id="f41af-169">可取值为：`system`、`user`。</span><span class="sxs-lookup"><span data-stu-id="f41af-169">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="f41af-170">fileName</span><span class="sxs-lookup"><span data-stu-id="f41af-170">fileName</span></span>|<span data-ttu-id="f41af-171">String</span><span class="sxs-lookup"><span data-stu-id="f41af-171">String</span></span>|<span data-ttu-id="f41af-172">脚本文件名。</span><span class="sxs-lookup"><span data-stu-id="f41af-172">Script file name.</span></span>|
|<span data-ttu-id="f41af-173">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f41af-173">roleScopeTagIds</span></span>|<span data-ttu-id="f41af-174">字符串集合</span><span class="sxs-lookup"><span data-stu-id="f41af-174">String collection</span></span>|<span data-ttu-id="f41af-175">此 PowerShellScript 实例的范围标记 Id 的列表。</span><span class="sxs-lookup"><span data-stu-id="f41af-175">List of Scope Tag IDs for this PowerShellScript instance.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f41af-176">关系</span><span class="sxs-lookup"><span data-stu-id="f41af-176">Relationships</span></span>
|<span data-ttu-id="f41af-177">关系</span><span class="sxs-lookup"><span data-stu-id="f41af-177">Relationship</span></span>|<span data-ttu-id="f41af-178">类型</span><span class="sxs-lookup"><span data-stu-id="f41af-178">Type</span></span>|<span data-ttu-id="f41af-179">说明</span><span class="sxs-lookup"><span data-stu-id="f41af-179">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f41af-180">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="f41af-180">groupAssignments</span></span>|<span data-ttu-id="f41af-181">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f41af-181">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) collection</span></span>|<span data-ttu-id="f41af-182">设备管理脚本的组分配的列表。</span><span class="sxs-lookup"><span data-stu-id="f41af-182">The list of group assignments for the device management script.</span></span>|
|<span data-ttu-id="f41af-183">assignments</span><span class="sxs-lookup"><span data-stu-id="f41af-183">assignments</span></span>|<span data-ttu-id="f41af-184">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f41af-184">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) collection</span></span>|<span data-ttu-id="f41af-185">设备管理脚本的组分配的列表。</span><span class="sxs-lookup"><span data-stu-id="f41af-185">The list of group assignments for the device management script.</span></span>|
|<span data-ttu-id="f41af-186">runSummary</span><span class="sxs-lookup"><span data-stu-id="f41af-186">runSummary</span></span>|[<span data-ttu-id="f41af-187">deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="f41af-187">deviceManagementScriptRunSummary</span></span>](../resources/intune-devices-devicemanagementscriptrunsummary.md)|<span data-ttu-id="f41af-188">设备管理脚本的运行摘要。</span><span class="sxs-lookup"><span data-stu-id="f41af-188">Run summary for device management script.</span></span>|
|<span data-ttu-id="f41af-189">deviceRunStates</span><span class="sxs-lookup"><span data-stu-id="f41af-189">deviceRunStates</span></span>|<span data-ttu-id="f41af-190">[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f41af-190">[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) collection</span></span>|<span data-ttu-id="f41af-191">此脚本在所有设备上的运行状态列表。</span><span class="sxs-lookup"><span data-stu-id="f41af-191">List of run states for this script across all devices.</span></span>|
|<span data-ttu-id="f41af-192">userRunStates</span><span class="sxs-lookup"><span data-stu-id="f41af-192">userRunStates</span></span>|<span data-ttu-id="f41af-193">[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f41af-193">[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) collection</span></span>|<span data-ttu-id="f41af-194">此脚本在所有用户中的运行状态列表。</span><span class="sxs-lookup"><span data-stu-id="f41af-194">List of run states for this script across all users.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f41af-195">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f41af-195">JSON Representation</span></span>
<span data-ttu-id="f41af-196">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f41af-196">Here is a JSON representation of the resource.</span></span>
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






