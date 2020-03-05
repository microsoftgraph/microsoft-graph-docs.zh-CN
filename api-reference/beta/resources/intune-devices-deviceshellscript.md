---
title: deviceShellScript 资源类型
description: Intune 将向客户提供在已注册的 Mac OS 设备上运行其命令行管理程序脚本的功能。 脚本可以运行一次，也可以定期运行。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6dddb69c9559fbf7472615216c4498e5db65d69a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528587"
---
# <a name="deviceshellscript-resource-type"></a><span data-ttu-id="904bf-104">deviceShellScript 资源类型</span><span class="sxs-lookup"><span data-stu-id="904bf-104">deviceShellScript resource type</span></span>

<span data-ttu-id="904bf-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="904bf-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="904bf-106">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="904bf-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="904bf-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="904bf-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="904bf-108">Intune 将向客户提供在已注册的 Mac OS 设备上运行其命令行管理程序脚本的功能。</span><span class="sxs-lookup"><span data-stu-id="904bf-108">Intune will provide customer the ability to run their Shell scripts on the enrolled Mac OS devices.</span></span> <span data-ttu-id="904bf-109">脚本可以运行一次，也可以定期运行。</span><span class="sxs-lookup"><span data-stu-id="904bf-109">The script can be run once or periodically.</span></span>

## <a name="methods"></a><span data-ttu-id="904bf-110">方法</span><span class="sxs-lookup"><span data-stu-id="904bf-110">Methods</span></span>
|<span data-ttu-id="904bf-111">方法</span><span class="sxs-lookup"><span data-stu-id="904bf-111">Method</span></span>|<span data-ttu-id="904bf-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="904bf-112">Return Type</span></span>|<span data-ttu-id="904bf-113">说明</span><span class="sxs-lookup"><span data-stu-id="904bf-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="904bf-114">列出 deviceShellScripts</span><span class="sxs-lookup"><span data-stu-id="904bf-114">List deviceShellScripts</span></span>](../api/intune-devices-deviceshellscript-list.md)|<span data-ttu-id="904bf-115">[deviceShellScript](../resources/intune-devices-deviceshellscript.md)集合</span><span class="sxs-lookup"><span data-stu-id="904bf-115">[deviceShellScript](../resources/intune-devices-deviceshellscript.md) collection</span></span>|<span data-ttu-id="904bf-116">列出[deviceShellScript](../resources/intune-devices-deviceshellscript.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="904bf-116">List properties and relationships of the [deviceShellScript](../resources/intune-devices-deviceshellscript.md) objects.</span></span>|
|[<span data-ttu-id="904bf-117">获取 deviceShellScript</span><span class="sxs-lookup"><span data-stu-id="904bf-117">Get deviceShellScript</span></span>](../api/intune-devices-deviceshellscript-get.md)|[<span data-ttu-id="904bf-118">deviceShellScript</span><span class="sxs-lookup"><span data-stu-id="904bf-118">deviceShellScript</span></span>](../resources/intune-devices-deviceshellscript.md)|<span data-ttu-id="904bf-119">读取[deviceShellScript](../resources/intune-devices-deviceshellscript.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="904bf-119">Read properties and relationships of the [deviceShellScript](../resources/intune-devices-deviceshellscript.md) object.</span></span>|
|[<span data-ttu-id="904bf-120">创建 deviceShellScript</span><span class="sxs-lookup"><span data-stu-id="904bf-120">Create deviceShellScript</span></span>](../api/intune-devices-deviceshellscript-create.md)|[<span data-ttu-id="904bf-121">deviceShellScript</span><span class="sxs-lookup"><span data-stu-id="904bf-121">deviceShellScript</span></span>](../resources/intune-devices-deviceshellscript.md)|<span data-ttu-id="904bf-122">创建新的[deviceShellScript](../resources/intune-devices-deviceshellscript.md)对象。</span><span class="sxs-lookup"><span data-stu-id="904bf-122">Create a new [deviceShellScript](../resources/intune-devices-deviceshellscript.md) object.</span></span>|
|[<span data-ttu-id="904bf-123">删除 deviceShellScript</span><span class="sxs-lookup"><span data-stu-id="904bf-123">Delete deviceShellScript</span></span>](../api/intune-devices-deviceshellscript-delete.md)|<span data-ttu-id="904bf-124">无</span><span class="sxs-lookup"><span data-stu-id="904bf-124">None</span></span>|<span data-ttu-id="904bf-125">删除[deviceShellScript](../resources/intune-devices-deviceshellscript.md)。</span><span class="sxs-lookup"><span data-stu-id="904bf-125">Deletes a [deviceShellScript](../resources/intune-devices-deviceshellscript.md).</span></span>|
|[<span data-ttu-id="904bf-126">更新 deviceShellScript</span><span class="sxs-lookup"><span data-stu-id="904bf-126">Update deviceShellScript</span></span>](../api/intune-devices-deviceshellscript-update.md)|[<span data-ttu-id="904bf-127">deviceShellScript</span><span class="sxs-lookup"><span data-stu-id="904bf-127">deviceShellScript</span></span>](../resources/intune-devices-deviceshellscript.md)|<span data-ttu-id="904bf-128">更新[deviceShellScript](../resources/intune-devices-deviceshellscript.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="904bf-128">Update the properties of a [deviceShellScript](../resources/intune-devices-deviceshellscript.md) object.</span></span>|
|[<span data-ttu-id="904bf-129">分配操作</span><span class="sxs-lookup"><span data-stu-id="904bf-129">assign action</span></span>](../api/intune-devices-deviceshellscript-assign.md)|<span data-ttu-id="904bf-130">无</span><span class="sxs-lookup"><span data-stu-id="904bf-130">None</span></span>|<span data-ttu-id="904bf-131">尚未记录</span><span class="sxs-lookup"><span data-stu-id="904bf-131">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="904bf-132">属性</span><span class="sxs-lookup"><span data-stu-id="904bf-132">Properties</span></span>
|<span data-ttu-id="904bf-133">属性</span><span class="sxs-lookup"><span data-stu-id="904bf-133">Property</span></span>|<span data-ttu-id="904bf-134">类型</span><span class="sxs-lookup"><span data-stu-id="904bf-134">Type</span></span>|<span data-ttu-id="904bf-135">说明</span><span class="sxs-lookup"><span data-stu-id="904bf-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="904bf-136">id</span><span class="sxs-lookup"><span data-stu-id="904bf-136">id</span></span>|<span data-ttu-id="904bf-137">字符串</span><span class="sxs-lookup"><span data-stu-id="904bf-137">String</span></span>|<span data-ttu-id="904bf-138">设备管理脚本的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="904bf-138">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="904bf-139">displayName</span><span class="sxs-lookup"><span data-stu-id="904bf-139">displayName</span></span>|<span data-ttu-id="904bf-140">字符串</span><span class="sxs-lookup"><span data-stu-id="904bf-140">String</span></span>|<span data-ttu-id="904bf-141">设备管理脚本的名称。</span><span class="sxs-lookup"><span data-stu-id="904bf-141">Name of the device management script.</span></span>|
|<span data-ttu-id="904bf-142">说明</span><span class="sxs-lookup"><span data-stu-id="904bf-142">description</span></span>|<span data-ttu-id="904bf-143">String</span><span class="sxs-lookup"><span data-stu-id="904bf-143">String</span></span>|<span data-ttu-id="904bf-144">设备管理脚本的可选说明。</span><span class="sxs-lookup"><span data-stu-id="904bf-144">Optional description for the device management script.</span></span>|
|<span data-ttu-id="904bf-145">scriptContent</span><span class="sxs-lookup"><span data-stu-id="904bf-145">scriptContent</span></span>|<span data-ttu-id="904bf-146">Binary</span><span class="sxs-lookup"><span data-stu-id="904bf-146">Binary</span></span>|<span data-ttu-id="904bf-147">脚本内容。</span><span class="sxs-lookup"><span data-stu-id="904bf-147">The script content.</span></span>|
|<span data-ttu-id="904bf-148">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="904bf-148">createdDateTime</span></span>|<span data-ttu-id="904bf-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="904bf-149">DateTimeOffset</span></span>|<span data-ttu-id="904bf-150">设备管理脚本的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="904bf-150">The date and time the device management script was created.</span></span> <span data-ttu-id="904bf-151">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="904bf-151">This property is read-only.</span></span>|
|<span data-ttu-id="904bf-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="904bf-152">lastModifiedDateTime</span></span>|<span data-ttu-id="904bf-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="904bf-153">DateTimeOffset</span></span>|<span data-ttu-id="904bf-154">上次修改设备管理脚本的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="904bf-154">The date and time the device management script was last modified.</span></span> <span data-ttu-id="904bf-155">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="904bf-155">This property is read-only.</span></span>|
|<span data-ttu-id="904bf-156">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="904bf-156">runAsAccount</span></span>|[<span data-ttu-id="904bf-157">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="904bf-157">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="904bf-158">指示执行上下文的类型。</span><span class="sxs-lookup"><span data-stu-id="904bf-158">Indicates the type of execution context.</span></span> <span data-ttu-id="904bf-159">可取值为：`system`、`user`。</span><span class="sxs-lookup"><span data-stu-id="904bf-159">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="904bf-160">fileName</span><span class="sxs-lookup"><span data-stu-id="904bf-160">fileName</span></span>|<span data-ttu-id="904bf-161">String</span><span class="sxs-lookup"><span data-stu-id="904bf-161">String</span></span>|<span data-ttu-id="904bf-162">脚本文件名。</span><span class="sxs-lookup"><span data-stu-id="904bf-162">Script file name.</span></span>|
|<span data-ttu-id="904bf-163">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="904bf-163">roleScopeTagIds</span></span>|<span data-ttu-id="904bf-164">String 集合</span><span class="sxs-lookup"><span data-stu-id="904bf-164">String collection</span></span>|<span data-ttu-id="904bf-165">此 PowerShellScript 实例的范围标记 Id 的列表。</span><span class="sxs-lookup"><span data-stu-id="904bf-165">List of Scope Tag IDs for this PowerShellScript instance.</span></span>|

## <a name="relationships"></a><span data-ttu-id="904bf-166">关系</span><span class="sxs-lookup"><span data-stu-id="904bf-166">Relationships</span></span>
|<span data-ttu-id="904bf-167">关系</span><span class="sxs-lookup"><span data-stu-id="904bf-167">Relationship</span></span>|<span data-ttu-id="904bf-168">类型</span><span class="sxs-lookup"><span data-stu-id="904bf-168">Type</span></span>|<span data-ttu-id="904bf-169">说明</span><span class="sxs-lookup"><span data-stu-id="904bf-169">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="904bf-170">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="904bf-170">groupAssignments</span></span>|<span data-ttu-id="904bf-171">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="904bf-171">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) collection</span></span>|<span data-ttu-id="904bf-172">设备管理脚本的组分配的列表。</span><span class="sxs-lookup"><span data-stu-id="904bf-172">The list of group assignments for the device management script.</span></span>|
|<span data-ttu-id="904bf-173">assignments</span><span class="sxs-lookup"><span data-stu-id="904bf-173">assignments</span></span>|<span data-ttu-id="904bf-174">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="904bf-174">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) collection</span></span>|<span data-ttu-id="904bf-175">设备管理脚本的组分配的列表。</span><span class="sxs-lookup"><span data-stu-id="904bf-175">The list of group assignments for the device management script.</span></span>|
|<span data-ttu-id="904bf-176">runSummary</span><span class="sxs-lookup"><span data-stu-id="904bf-176">runSummary</span></span>|[<span data-ttu-id="904bf-177">deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="904bf-177">deviceManagementScriptRunSummary</span></span>](../resources/intune-devices-devicemanagementscriptrunsummary.md)|<span data-ttu-id="904bf-178">设备管理脚本的运行摘要。</span><span class="sxs-lookup"><span data-stu-id="904bf-178">Run summary for device management script.</span></span>|
|<span data-ttu-id="904bf-179">deviceRunStates</span><span class="sxs-lookup"><span data-stu-id="904bf-179">deviceRunStates</span></span>|<span data-ttu-id="904bf-180">[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)集合</span><span class="sxs-lookup"><span data-stu-id="904bf-180">[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) collection</span></span>|<span data-ttu-id="904bf-181">此脚本在所有设备上的运行状态列表。</span><span class="sxs-lookup"><span data-stu-id="904bf-181">List of run states for this script across all devices.</span></span>|
|<span data-ttu-id="904bf-182">userRunStates</span><span class="sxs-lookup"><span data-stu-id="904bf-182">userRunStates</span></span>|<span data-ttu-id="904bf-183">[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)集合</span><span class="sxs-lookup"><span data-stu-id="904bf-183">[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) collection</span></span>|<span data-ttu-id="904bf-184">此脚本在所有用户中的运行状态列表。</span><span class="sxs-lookup"><span data-stu-id="904bf-184">List of run states for this script across all users.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="904bf-185">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="904bf-185">JSON Representation</span></span>
<span data-ttu-id="904bf-186">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="904bf-186">Here is a JSON representation of the resource.</span></span>
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



