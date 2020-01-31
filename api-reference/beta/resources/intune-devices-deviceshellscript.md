---
title: deviceShellScript 资源类型
description: Intune 将向客户提供在已注册的 Mac OS 设备上运行其命令行管理程序脚本的功能。 脚本可以运行一次，也可以定期运行。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 391e911eb32639b9f814e8ad00aa9948e9f9e0e3
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/31/2020
ms.locfileid: "41634954"
---
# <a name="deviceshellscript-resource-type"></a><span data-ttu-id="35d78-104">deviceShellScript 资源类型</span><span class="sxs-lookup"><span data-stu-id="35d78-104">deviceShellScript resource type</span></span>

> <span data-ttu-id="35d78-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="35d78-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="35d78-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="35d78-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="35d78-107">Intune 将向客户提供在已注册的 Mac OS 设备上运行其命令行管理程序脚本的功能。</span><span class="sxs-lookup"><span data-stu-id="35d78-107">Intune will provide customer the ability to run their Shell scripts on the enrolled Mac OS devices.</span></span> <span data-ttu-id="35d78-108">脚本可以运行一次，也可以定期运行。</span><span class="sxs-lookup"><span data-stu-id="35d78-108">The script can be run once or periodically.</span></span>

## <a name="methods"></a><span data-ttu-id="35d78-109">方法</span><span class="sxs-lookup"><span data-stu-id="35d78-109">Methods</span></span>
|<span data-ttu-id="35d78-110">方法</span><span class="sxs-lookup"><span data-stu-id="35d78-110">Method</span></span>|<span data-ttu-id="35d78-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="35d78-111">Return Type</span></span>|<span data-ttu-id="35d78-112">说明</span><span class="sxs-lookup"><span data-stu-id="35d78-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="35d78-113">列出 deviceShellScripts</span><span class="sxs-lookup"><span data-stu-id="35d78-113">List deviceShellScripts</span></span>](../api/intune-devices-deviceshellscript-list.md)|<span data-ttu-id="35d78-114">[deviceShellScript](../resources/intune-devices-deviceshellscript.md)集合</span><span class="sxs-lookup"><span data-stu-id="35d78-114">[deviceShellScript](../resources/intune-devices-deviceshellscript.md) collection</span></span>|<span data-ttu-id="35d78-115">列出[deviceShellScript](../resources/intune-devices-deviceshellscript.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="35d78-115">List properties and relationships of the [deviceShellScript](../resources/intune-devices-deviceshellscript.md) objects.</span></span>|
|[<span data-ttu-id="35d78-116">获取 deviceShellScript</span><span class="sxs-lookup"><span data-stu-id="35d78-116">Get deviceShellScript</span></span>](../api/intune-devices-deviceshellscript-get.md)|[<span data-ttu-id="35d78-117">deviceShellScript</span><span class="sxs-lookup"><span data-stu-id="35d78-117">deviceShellScript</span></span>](../resources/intune-devices-deviceshellscript.md)|<span data-ttu-id="35d78-118">读取[deviceShellScript](../resources/intune-devices-deviceshellscript.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="35d78-118">Read properties and relationships of the [deviceShellScript](../resources/intune-devices-deviceshellscript.md) object.</span></span>|
|[<span data-ttu-id="35d78-119">创建 deviceShellScript</span><span class="sxs-lookup"><span data-stu-id="35d78-119">Create deviceShellScript</span></span>](../api/intune-devices-deviceshellscript-create.md)|[<span data-ttu-id="35d78-120">deviceShellScript</span><span class="sxs-lookup"><span data-stu-id="35d78-120">deviceShellScript</span></span>](../resources/intune-devices-deviceshellscript.md)|<span data-ttu-id="35d78-121">创建新的[deviceShellScript](../resources/intune-devices-deviceshellscript.md)对象。</span><span class="sxs-lookup"><span data-stu-id="35d78-121">Create a new [deviceShellScript](../resources/intune-devices-deviceshellscript.md) object.</span></span>|
|[<span data-ttu-id="35d78-122">删除 deviceShellScript</span><span class="sxs-lookup"><span data-stu-id="35d78-122">Delete deviceShellScript</span></span>](../api/intune-devices-deviceshellscript-delete.md)|<span data-ttu-id="35d78-123">无</span><span class="sxs-lookup"><span data-stu-id="35d78-123">None</span></span>|<span data-ttu-id="35d78-124">删除[deviceShellScript](../resources/intune-devices-deviceshellscript.md)。</span><span class="sxs-lookup"><span data-stu-id="35d78-124">Deletes a [deviceShellScript](../resources/intune-devices-deviceshellscript.md).</span></span>|
|[<span data-ttu-id="35d78-125">更新 deviceShellScript</span><span class="sxs-lookup"><span data-stu-id="35d78-125">Update deviceShellScript</span></span>](../api/intune-devices-deviceshellscript-update.md)|[<span data-ttu-id="35d78-126">deviceShellScript</span><span class="sxs-lookup"><span data-stu-id="35d78-126">deviceShellScript</span></span>](../resources/intune-devices-deviceshellscript.md)|<span data-ttu-id="35d78-127">更新[deviceShellScript](../resources/intune-devices-deviceshellscript.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="35d78-127">Update the properties of a [deviceShellScript](../resources/intune-devices-deviceshellscript.md) object.</span></span>|
|[<span data-ttu-id="35d78-128">分配操作</span><span class="sxs-lookup"><span data-stu-id="35d78-128">assign action</span></span>](../api/intune-devices-deviceshellscript-assign.md)|<span data-ttu-id="35d78-129">无</span><span class="sxs-lookup"><span data-stu-id="35d78-129">None</span></span>|<span data-ttu-id="35d78-130">尚未记录</span><span class="sxs-lookup"><span data-stu-id="35d78-130">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="35d78-131">属性</span><span class="sxs-lookup"><span data-stu-id="35d78-131">Properties</span></span>
|<span data-ttu-id="35d78-132">属性</span><span class="sxs-lookup"><span data-stu-id="35d78-132">Property</span></span>|<span data-ttu-id="35d78-133">类型</span><span class="sxs-lookup"><span data-stu-id="35d78-133">Type</span></span>|<span data-ttu-id="35d78-134">Description</span><span class="sxs-lookup"><span data-stu-id="35d78-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35d78-135">id</span><span class="sxs-lookup"><span data-stu-id="35d78-135">id</span></span>|<span data-ttu-id="35d78-136">字符串</span><span class="sxs-lookup"><span data-stu-id="35d78-136">String</span></span>|<span data-ttu-id="35d78-137">设备管理脚本的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="35d78-137">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="35d78-138">displayName</span><span class="sxs-lookup"><span data-stu-id="35d78-138">displayName</span></span>|<span data-ttu-id="35d78-139">字符串</span><span class="sxs-lookup"><span data-stu-id="35d78-139">String</span></span>|<span data-ttu-id="35d78-140">设备管理脚本的名称。</span><span class="sxs-lookup"><span data-stu-id="35d78-140">Name of the device management script.</span></span>|
|<span data-ttu-id="35d78-141">说明</span><span class="sxs-lookup"><span data-stu-id="35d78-141">description</span></span>|<span data-ttu-id="35d78-142">String</span><span class="sxs-lookup"><span data-stu-id="35d78-142">String</span></span>|<span data-ttu-id="35d78-143">设备管理脚本的可选说明。</span><span class="sxs-lookup"><span data-stu-id="35d78-143">Optional description for the device management script.</span></span>|
|<span data-ttu-id="35d78-144">scriptContent</span><span class="sxs-lookup"><span data-stu-id="35d78-144">scriptContent</span></span>|<span data-ttu-id="35d78-145">Binary</span><span class="sxs-lookup"><span data-stu-id="35d78-145">Binary</span></span>|<span data-ttu-id="35d78-146">脚本内容。</span><span class="sxs-lookup"><span data-stu-id="35d78-146">The script content.</span></span>|
|<span data-ttu-id="35d78-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="35d78-147">createdDateTime</span></span>|<span data-ttu-id="35d78-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="35d78-148">DateTimeOffset</span></span>|<span data-ttu-id="35d78-149">设备管理脚本的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="35d78-149">The date and time the device management script was created.</span></span> <span data-ttu-id="35d78-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="35d78-150">This property is read-only.</span></span>|
|<span data-ttu-id="35d78-151">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="35d78-151">lastModifiedDateTime</span></span>|<span data-ttu-id="35d78-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="35d78-152">DateTimeOffset</span></span>|<span data-ttu-id="35d78-153">上次修改设备管理脚本的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="35d78-153">The date and time the device management script was last modified.</span></span> <span data-ttu-id="35d78-154">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="35d78-154">This property is read-only.</span></span>|
|<span data-ttu-id="35d78-155">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="35d78-155">runAsAccount</span></span>|[<span data-ttu-id="35d78-156">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="35d78-156">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="35d78-157">指示执行上下文的类型。</span><span class="sxs-lookup"><span data-stu-id="35d78-157">Indicates the type of execution context.</span></span> <span data-ttu-id="35d78-158">可取值为：`system`、`user`。</span><span class="sxs-lookup"><span data-stu-id="35d78-158">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="35d78-159">fileName</span><span class="sxs-lookup"><span data-stu-id="35d78-159">fileName</span></span>|<span data-ttu-id="35d78-160">String</span><span class="sxs-lookup"><span data-stu-id="35d78-160">String</span></span>|<span data-ttu-id="35d78-161">脚本文件名。</span><span class="sxs-lookup"><span data-stu-id="35d78-161">Script file name.</span></span>|
|<span data-ttu-id="35d78-162">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="35d78-162">roleScopeTagIds</span></span>|<span data-ttu-id="35d78-163">String 集合</span><span class="sxs-lookup"><span data-stu-id="35d78-163">String collection</span></span>|<span data-ttu-id="35d78-164">此 PowerShellScript 实例的范围标记 Id 的列表。</span><span class="sxs-lookup"><span data-stu-id="35d78-164">List of Scope Tag IDs for this PowerShellScript instance.</span></span>|

## <a name="relationships"></a><span data-ttu-id="35d78-165">关系</span><span class="sxs-lookup"><span data-stu-id="35d78-165">Relationships</span></span>
|<span data-ttu-id="35d78-166">关系</span><span class="sxs-lookup"><span data-stu-id="35d78-166">Relationship</span></span>|<span data-ttu-id="35d78-167">类型</span><span class="sxs-lookup"><span data-stu-id="35d78-167">Type</span></span>|<span data-ttu-id="35d78-168">Description</span><span class="sxs-lookup"><span data-stu-id="35d78-168">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35d78-169">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="35d78-169">groupAssignments</span></span>|<span data-ttu-id="35d78-170">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="35d78-170">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) collection</span></span>|<span data-ttu-id="35d78-171">设备管理脚本的组分配的列表。</span><span class="sxs-lookup"><span data-stu-id="35d78-171">The list of group assignments for the device management script.</span></span>|
|<span data-ttu-id="35d78-172">assignments</span><span class="sxs-lookup"><span data-stu-id="35d78-172">assignments</span></span>|<span data-ttu-id="35d78-173">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="35d78-173">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) collection</span></span>|<span data-ttu-id="35d78-174">设备管理脚本的组分配的列表。</span><span class="sxs-lookup"><span data-stu-id="35d78-174">The list of group assignments for the device management script.</span></span>|
|<span data-ttu-id="35d78-175">runSummary</span><span class="sxs-lookup"><span data-stu-id="35d78-175">runSummary</span></span>|[<span data-ttu-id="35d78-176">deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="35d78-176">deviceManagementScriptRunSummary</span></span>](../resources/intune-devices-devicemanagementscriptrunsummary.md)|<span data-ttu-id="35d78-177">设备管理脚本的运行摘要。</span><span class="sxs-lookup"><span data-stu-id="35d78-177">Run summary for device management script.</span></span>|
|<span data-ttu-id="35d78-178">deviceRunStates</span><span class="sxs-lookup"><span data-stu-id="35d78-178">deviceRunStates</span></span>|<span data-ttu-id="35d78-179">[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)集合</span><span class="sxs-lookup"><span data-stu-id="35d78-179">[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) collection</span></span>|<span data-ttu-id="35d78-180">此脚本在所有设备上的运行状态列表。</span><span class="sxs-lookup"><span data-stu-id="35d78-180">List of run states for this script across all devices.</span></span>|
|<span data-ttu-id="35d78-181">userRunStates</span><span class="sxs-lookup"><span data-stu-id="35d78-181">userRunStates</span></span>|<span data-ttu-id="35d78-182">[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)集合</span><span class="sxs-lookup"><span data-stu-id="35d78-182">[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) collection</span></span>|<span data-ttu-id="35d78-183">此脚本在所有用户中的运行状态列表。</span><span class="sxs-lookup"><span data-stu-id="35d78-183">List of run states for this script across all users.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="35d78-184">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="35d78-184">JSON Representation</span></span>
<span data-ttu-id="35d78-185">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="35d78-185">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceShellScript"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceShellScript",
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



