---
title: deviceShellScript 资源类型
description: Intune 将向客户提供在已注册的 Mac OS 设备上运行其命令行管理程序脚本的功能。 脚本可以运行一次，也可以定期运行。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e0583eb6dca38af0e490fc23bf57c852bd195ba5
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42784124"
---
# <a name="deviceshellscript-resource-type"></a><span data-ttu-id="9aa92-104">deviceShellScript 资源类型</span><span class="sxs-lookup"><span data-stu-id="9aa92-104">deviceShellScript resource type</span></span>

> <span data-ttu-id="9aa92-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9aa92-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9aa92-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9aa92-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9aa92-107">Intune 将向客户提供在已注册的 Mac OS 设备上运行其命令行管理程序脚本的功能。</span><span class="sxs-lookup"><span data-stu-id="9aa92-107">Intune will provide customer the ability to run their Shell scripts on the enrolled Mac OS devices.</span></span> <span data-ttu-id="9aa92-108">脚本可以运行一次，也可以定期运行。</span><span class="sxs-lookup"><span data-stu-id="9aa92-108">The script can be run once or periodically.</span></span>

## <a name="methods"></a><span data-ttu-id="9aa92-109">方法</span><span class="sxs-lookup"><span data-stu-id="9aa92-109">Methods</span></span>
|<span data-ttu-id="9aa92-110">方法</span><span class="sxs-lookup"><span data-stu-id="9aa92-110">Method</span></span>|<span data-ttu-id="9aa92-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="9aa92-111">Return Type</span></span>|<span data-ttu-id="9aa92-112">说明</span><span class="sxs-lookup"><span data-stu-id="9aa92-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9aa92-113">列出 deviceShellScripts</span><span class="sxs-lookup"><span data-stu-id="9aa92-113">List deviceShellScripts</span></span>](../api/intune-devices-deviceshellscript-list.md)|<span data-ttu-id="9aa92-114">[deviceShellScript](../resources/intune-devices-deviceshellscript.md)集合</span><span class="sxs-lookup"><span data-stu-id="9aa92-114">[deviceShellScript](../resources/intune-devices-deviceshellscript.md) collection</span></span>|<span data-ttu-id="9aa92-115">列出[deviceShellScript](../resources/intune-devices-deviceshellscript.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9aa92-115">List properties and relationships of the [deviceShellScript](../resources/intune-devices-deviceshellscript.md) objects.</span></span>|
|[<span data-ttu-id="9aa92-116">获取 deviceShellScript</span><span class="sxs-lookup"><span data-stu-id="9aa92-116">Get deviceShellScript</span></span>](../api/intune-devices-deviceshellscript-get.md)|[<span data-ttu-id="9aa92-117">deviceShellScript</span><span class="sxs-lookup"><span data-stu-id="9aa92-117">deviceShellScript</span></span>](../resources/intune-devices-deviceshellscript.md)|<span data-ttu-id="9aa92-118">读取[deviceShellScript](../resources/intune-devices-deviceshellscript.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9aa92-118">Read properties and relationships of the [deviceShellScript](../resources/intune-devices-deviceshellscript.md) object.</span></span>|
|[<span data-ttu-id="9aa92-119">创建 deviceShellScript</span><span class="sxs-lookup"><span data-stu-id="9aa92-119">Create deviceShellScript</span></span>](../api/intune-devices-deviceshellscript-create.md)|[<span data-ttu-id="9aa92-120">deviceShellScript</span><span class="sxs-lookup"><span data-stu-id="9aa92-120">deviceShellScript</span></span>](../resources/intune-devices-deviceshellscript.md)|<span data-ttu-id="9aa92-121">创建新的[deviceShellScript](../resources/intune-devices-deviceshellscript.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9aa92-121">Create a new [deviceShellScript](../resources/intune-devices-deviceshellscript.md) object.</span></span>|
|[<span data-ttu-id="9aa92-122">删除 deviceShellScript</span><span class="sxs-lookup"><span data-stu-id="9aa92-122">Delete deviceShellScript</span></span>](../api/intune-devices-deviceshellscript-delete.md)|<span data-ttu-id="9aa92-123">None</span><span class="sxs-lookup"><span data-stu-id="9aa92-123">None</span></span>|<span data-ttu-id="9aa92-124">删除[deviceShellScript](../resources/intune-devices-deviceshellscript.md)。</span><span class="sxs-lookup"><span data-stu-id="9aa92-124">Deletes a [deviceShellScript](../resources/intune-devices-deviceshellscript.md).</span></span>|
|[<span data-ttu-id="9aa92-125">更新 deviceShellScript</span><span class="sxs-lookup"><span data-stu-id="9aa92-125">Update deviceShellScript</span></span>](../api/intune-devices-deviceshellscript-update.md)|[<span data-ttu-id="9aa92-126">deviceShellScript</span><span class="sxs-lookup"><span data-stu-id="9aa92-126">deviceShellScript</span></span>](../resources/intune-devices-deviceshellscript.md)|<span data-ttu-id="9aa92-127">更新[deviceShellScript](../resources/intune-devices-deviceshellscript.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9aa92-127">Update the properties of a [deviceShellScript](../resources/intune-devices-deviceshellscript.md) object.</span></span>|
|[<span data-ttu-id="9aa92-128">分配操作</span><span class="sxs-lookup"><span data-stu-id="9aa92-128">assign action</span></span>](../api/intune-devices-deviceshellscript-assign.md)|<span data-ttu-id="9aa92-129">无</span><span class="sxs-lookup"><span data-stu-id="9aa92-129">None</span></span>|<span data-ttu-id="9aa92-130">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9aa92-130">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="9aa92-131">属性</span><span class="sxs-lookup"><span data-stu-id="9aa92-131">Properties</span></span>
|<span data-ttu-id="9aa92-132">属性</span><span class="sxs-lookup"><span data-stu-id="9aa92-132">Property</span></span>|<span data-ttu-id="9aa92-133">类型</span><span class="sxs-lookup"><span data-stu-id="9aa92-133">Type</span></span>|<span data-ttu-id="9aa92-134">说明</span><span class="sxs-lookup"><span data-stu-id="9aa92-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9aa92-135">id</span><span class="sxs-lookup"><span data-stu-id="9aa92-135">id</span></span>|<span data-ttu-id="9aa92-136">字符串</span><span class="sxs-lookup"><span data-stu-id="9aa92-136">String</span></span>|<span data-ttu-id="9aa92-137">设备管理脚本的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="9aa92-137">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="9aa92-138">displayName</span><span class="sxs-lookup"><span data-stu-id="9aa92-138">displayName</span></span>|<span data-ttu-id="9aa92-139">字符串</span><span class="sxs-lookup"><span data-stu-id="9aa92-139">String</span></span>|<span data-ttu-id="9aa92-140">设备管理脚本的名称。</span><span class="sxs-lookup"><span data-stu-id="9aa92-140">Name of the device management script.</span></span>|
|<span data-ttu-id="9aa92-141">说明</span><span class="sxs-lookup"><span data-stu-id="9aa92-141">description</span></span>|<span data-ttu-id="9aa92-142">String</span><span class="sxs-lookup"><span data-stu-id="9aa92-142">String</span></span>|<span data-ttu-id="9aa92-143">设备管理脚本的可选说明。</span><span class="sxs-lookup"><span data-stu-id="9aa92-143">Optional description for the device management script.</span></span>|
|<span data-ttu-id="9aa92-144">scriptContent</span><span class="sxs-lookup"><span data-stu-id="9aa92-144">scriptContent</span></span>|<span data-ttu-id="9aa92-145">Binary</span><span class="sxs-lookup"><span data-stu-id="9aa92-145">Binary</span></span>|<span data-ttu-id="9aa92-146">脚本内容。</span><span class="sxs-lookup"><span data-stu-id="9aa92-146">The script content.</span></span>|
|<span data-ttu-id="9aa92-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9aa92-147">createdDateTime</span></span>|<span data-ttu-id="9aa92-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9aa92-148">DateTimeOffset</span></span>|<span data-ttu-id="9aa92-149">设备管理脚本的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="9aa92-149">The date and time the device management script was created.</span></span> <span data-ttu-id="9aa92-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9aa92-150">This property is read-only.</span></span>|
|<span data-ttu-id="9aa92-151">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9aa92-151">lastModifiedDateTime</span></span>|<span data-ttu-id="9aa92-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9aa92-152">DateTimeOffset</span></span>|<span data-ttu-id="9aa92-153">上次修改设备管理脚本的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="9aa92-153">The date and time the device management script was last modified.</span></span> <span data-ttu-id="9aa92-154">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9aa92-154">This property is read-only.</span></span>|
|<span data-ttu-id="9aa92-155">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="9aa92-155">runAsAccount</span></span>|[<span data-ttu-id="9aa92-156">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="9aa92-156">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="9aa92-157">指示执行上下文的类型。</span><span class="sxs-lookup"><span data-stu-id="9aa92-157">Indicates the type of execution context.</span></span> <span data-ttu-id="9aa92-158">可取值为：`system`、`user`。</span><span class="sxs-lookup"><span data-stu-id="9aa92-158">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="9aa92-159">fileName</span><span class="sxs-lookup"><span data-stu-id="9aa92-159">fileName</span></span>|<span data-ttu-id="9aa92-160">String</span><span class="sxs-lookup"><span data-stu-id="9aa92-160">String</span></span>|<span data-ttu-id="9aa92-161">脚本文件名。</span><span class="sxs-lookup"><span data-stu-id="9aa92-161">Script file name.</span></span>|
|<span data-ttu-id="9aa92-162">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9aa92-162">roleScopeTagIds</span></span>|<span data-ttu-id="9aa92-163">String collection</span><span class="sxs-lookup"><span data-stu-id="9aa92-163">String collection</span></span>|<span data-ttu-id="9aa92-164">此 PowerShellScript 实例的范围标记 Id 的列表。</span><span class="sxs-lookup"><span data-stu-id="9aa92-164">List of Scope Tag IDs for this PowerShellScript instance.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9aa92-165">关系</span><span class="sxs-lookup"><span data-stu-id="9aa92-165">Relationships</span></span>
|<span data-ttu-id="9aa92-166">关系</span><span class="sxs-lookup"><span data-stu-id="9aa92-166">Relationship</span></span>|<span data-ttu-id="9aa92-167">类型</span><span class="sxs-lookup"><span data-stu-id="9aa92-167">Type</span></span>|<span data-ttu-id="9aa92-168">说明</span><span class="sxs-lookup"><span data-stu-id="9aa92-168">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9aa92-169">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="9aa92-169">groupAssignments</span></span>|<span data-ttu-id="9aa92-170">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="9aa92-170">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) collection</span></span>|<span data-ttu-id="9aa92-171">设备管理脚本的组分配的列表。</span><span class="sxs-lookup"><span data-stu-id="9aa92-171">The list of group assignments for the device management script.</span></span>|
|<span data-ttu-id="9aa92-172">assignments</span><span class="sxs-lookup"><span data-stu-id="9aa92-172">assignments</span></span>|<span data-ttu-id="9aa92-173">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="9aa92-173">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) collection</span></span>|<span data-ttu-id="9aa92-174">设备管理脚本的组分配的列表。</span><span class="sxs-lookup"><span data-stu-id="9aa92-174">The list of group assignments for the device management script.</span></span>|
|<span data-ttu-id="9aa92-175">runSummary</span><span class="sxs-lookup"><span data-stu-id="9aa92-175">runSummary</span></span>|[<span data-ttu-id="9aa92-176">deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="9aa92-176">deviceManagementScriptRunSummary</span></span>](../resources/intune-devices-devicemanagementscriptrunsummary.md)|<span data-ttu-id="9aa92-177">设备管理脚本的运行摘要。</span><span class="sxs-lookup"><span data-stu-id="9aa92-177">Run summary for device management script.</span></span>|
|<span data-ttu-id="9aa92-178">deviceRunStates</span><span class="sxs-lookup"><span data-stu-id="9aa92-178">deviceRunStates</span></span>|<span data-ttu-id="9aa92-179">[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)集合</span><span class="sxs-lookup"><span data-stu-id="9aa92-179">[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) collection</span></span>|<span data-ttu-id="9aa92-180">此脚本在所有设备上的运行状态列表。</span><span class="sxs-lookup"><span data-stu-id="9aa92-180">List of run states for this script across all devices.</span></span>|
|<span data-ttu-id="9aa92-181">userRunStates</span><span class="sxs-lookup"><span data-stu-id="9aa92-181">userRunStates</span></span>|<span data-ttu-id="9aa92-182">[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)集合</span><span class="sxs-lookup"><span data-stu-id="9aa92-182">[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) collection</span></span>|<span data-ttu-id="9aa92-183">此脚本在所有用户中的运行状态列表。</span><span class="sxs-lookup"><span data-stu-id="9aa92-183">List of run states for this script across all users.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9aa92-184">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9aa92-184">JSON Representation</span></span>
<span data-ttu-id="9aa92-185">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9aa92-185">Here is a JSON representation of the resource.</span></span>
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



