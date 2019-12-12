---
title: deviceShellScript 资源类型
description: Intune 将向客户提供在已注册的 Mac OS 设备上运行其命令行管理程序脚本的功能。 脚本可以运行一次，也可以定期运行。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 065c8b1976a4b51e4ce1b764ad13923a284077e6
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39955678"
---
# <a name="deviceshellscript-resource-type"></a><span data-ttu-id="88eef-104">deviceShellScript 资源类型</span><span class="sxs-lookup"><span data-stu-id="88eef-104">deviceShellScript resource type</span></span>

> <span data-ttu-id="88eef-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="88eef-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="88eef-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="88eef-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88eef-107">Intune 将向客户提供在已注册的 Mac OS 设备上运行其命令行管理程序脚本的功能。</span><span class="sxs-lookup"><span data-stu-id="88eef-107">Intune will provide customer the ability to run their Shell scripts on the enrolled Mac OS devices.</span></span> <span data-ttu-id="88eef-108">脚本可以运行一次，也可以定期运行。</span><span class="sxs-lookup"><span data-stu-id="88eef-108">The script can be run once or periodically.</span></span>

## <a name="methods"></a><span data-ttu-id="88eef-109">方法</span><span class="sxs-lookup"><span data-stu-id="88eef-109">Methods</span></span>
|<span data-ttu-id="88eef-110">方法</span><span class="sxs-lookup"><span data-stu-id="88eef-110">Method</span></span>|<span data-ttu-id="88eef-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="88eef-111">Return Type</span></span>|<span data-ttu-id="88eef-112">说明</span><span class="sxs-lookup"><span data-stu-id="88eef-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="88eef-113">列出 deviceShellScripts</span><span class="sxs-lookup"><span data-stu-id="88eef-113">List deviceShellScripts</span></span>](../api/intune-devices-deviceshellscript-list.md)|<span data-ttu-id="88eef-114">[deviceShellScript](../resources/intune-devices-deviceshellscript.md)集合</span><span class="sxs-lookup"><span data-stu-id="88eef-114">[deviceShellScript](../resources/intune-devices-deviceshellscript.md) collection</span></span>|<span data-ttu-id="88eef-115">列出[deviceShellScript](../resources/intune-devices-deviceshellscript.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="88eef-115">List properties and relationships of the [deviceShellScript](../resources/intune-devices-deviceshellscript.md) objects.</span></span>|
|[<span data-ttu-id="88eef-116">获取 deviceShellScript</span><span class="sxs-lookup"><span data-stu-id="88eef-116">Get deviceShellScript</span></span>](../api/intune-devices-deviceshellscript-get.md)|[<span data-ttu-id="88eef-117">deviceShellScript</span><span class="sxs-lookup"><span data-stu-id="88eef-117">deviceShellScript</span></span>](../resources/intune-devices-deviceshellscript.md)|<span data-ttu-id="88eef-118">读取[deviceShellScript](../resources/intune-devices-deviceshellscript.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="88eef-118">Read properties and relationships of the [deviceShellScript](../resources/intune-devices-deviceshellscript.md) object.</span></span>|
|[<span data-ttu-id="88eef-119">创建 deviceShellScript</span><span class="sxs-lookup"><span data-stu-id="88eef-119">Create deviceShellScript</span></span>](../api/intune-devices-deviceshellscript-create.md)|[<span data-ttu-id="88eef-120">deviceShellScript</span><span class="sxs-lookup"><span data-stu-id="88eef-120">deviceShellScript</span></span>](../resources/intune-devices-deviceshellscript.md)|<span data-ttu-id="88eef-121">创建新的[deviceShellScript](../resources/intune-devices-deviceshellscript.md)对象。</span><span class="sxs-lookup"><span data-stu-id="88eef-121">Create a new [deviceShellScript](../resources/intune-devices-deviceshellscript.md) object.</span></span>|
|[<span data-ttu-id="88eef-122">删除 deviceShellScript</span><span class="sxs-lookup"><span data-stu-id="88eef-122">Delete deviceShellScript</span></span>](../api/intune-devices-deviceshellscript-delete.md)|<span data-ttu-id="88eef-123">None</span><span class="sxs-lookup"><span data-stu-id="88eef-123">None</span></span>|<span data-ttu-id="88eef-124">删除[deviceShellScript](../resources/intune-devices-deviceshellscript.md)。</span><span class="sxs-lookup"><span data-stu-id="88eef-124">Deletes a [deviceShellScript](../resources/intune-devices-deviceshellscript.md).</span></span>|
|[<span data-ttu-id="88eef-125">更新 deviceShellScript</span><span class="sxs-lookup"><span data-stu-id="88eef-125">Update deviceShellScript</span></span>](../api/intune-devices-deviceshellscript-update.md)|[<span data-ttu-id="88eef-126">deviceShellScript</span><span class="sxs-lookup"><span data-stu-id="88eef-126">deviceShellScript</span></span>](../resources/intune-devices-deviceshellscript.md)|<span data-ttu-id="88eef-127">更新[deviceShellScript](../resources/intune-devices-deviceshellscript.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="88eef-127">Update the properties of a [deviceShellScript](../resources/intune-devices-deviceshellscript.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="88eef-128">属性</span><span class="sxs-lookup"><span data-stu-id="88eef-128">Properties</span></span>
|<span data-ttu-id="88eef-129">属性</span><span class="sxs-lookup"><span data-stu-id="88eef-129">Property</span></span>|<span data-ttu-id="88eef-130">类型</span><span class="sxs-lookup"><span data-stu-id="88eef-130">Type</span></span>|<span data-ttu-id="88eef-131">说明</span><span class="sxs-lookup"><span data-stu-id="88eef-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88eef-132">id</span><span class="sxs-lookup"><span data-stu-id="88eef-132">id</span></span>|<span data-ttu-id="88eef-133">字符串</span><span class="sxs-lookup"><span data-stu-id="88eef-133">String</span></span>|<span data-ttu-id="88eef-134">设备管理脚本的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="88eef-134">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="88eef-135">displayName</span><span class="sxs-lookup"><span data-stu-id="88eef-135">displayName</span></span>|<span data-ttu-id="88eef-136">字符串</span><span class="sxs-lookup"><span data-stu-id="88eef-136">String</span></span>|<span data-ttu-id="88eef-137">设备管理脚本的名称。</span><span class="sxs-lookup"><span data-stu-id="88eef-137">Name of the device management script.</span></span>|
|<span data-ttu-id="88eef-138">说明</span><span class="sxs-lookup"><span data-stu-id="88eef-138">description</span></span>|<span data-ttu-id="88eef-139">String</span><span class="sxs-lookup"><span data-stu-id="88eef-139">String</span></span>|<span data-ttu-id="88eef-140">设备管理脚本的可选说明。</span><span class="sxs-lookup"><span data-stu-id="88eef-140">Optional description for the device management script.</span></span>|
|<span data-ttu-id="88eef-141">scriptContent</span><span class="sxs-lookup"><span data-stu-id="88eef-141">scriptContent</span></span>|<span data-ttu-id="88eef-142">Binary</span><span class="sxs-lookup"><span data-stu-id="88eef-142">Binary</span></span>|<span data-ttu-id="88eef-143">脚本内容。</span><span class="sxs-lookup"><span data-stu-id="88eef-143">The script content.</span></span>|
|<span data-ttu-id="88eef-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="88eef-144">createdDateTime</span></span>|<span data-ttu-id="88eef-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88eef-145">DateTimeOffset</span></span>|<span data-ttu-id="88eef-146">设备管理脚本的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="88eef-146">The date and time the device management script was created.</span></span> <span data-ttu-id="88eef-147">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="88eef-147">This property is read-only.</span></span>|
|<span data-ttu-id="88eef-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="88eef-148">lastModifiedDateTime</span></span>|<span data-ttu-id="88eef-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88eef-149">DateTimeOffset</span></span>|<span data-ttu-id="88eef-150">上次修改设备管理脚本的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="88eef-150">The date and time the device management script was last modified.</span></span> <span data-ttu-id="88eef-151">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="88eef-151">This property is read-only.</span></span>|
|<span data-ttu-id="88eef-152">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="88eef-152">runAsAccount</span></span>|[<span data-ttu-id="88eef-153">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="88eef-153">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="88eef-154">指示执行上下文的类型。</span><span class="sxs-lookup"><span data-stu-id="88eef-154">Indicates the type of execution context.</span></span> <span data-ttu-id="88eef-155">可取值为：`system`、`user`。</span><span class="sxs-lookup"><span data-stu-id="88eef-155">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="88eef-156">fileName</span><span class="sxs-lookup"><span data-stu-id="88eef-156">fileName</span></span>|<span data-ttu-id="88eef-157">String</span><span class="sxs-lookup"><span data-stu-id="88eef-157">String</span></span>|<span data-ttu-id="88eef-158">脚本文件名。</span><span class="sxs-lookup"><span data-stu-id="88eef-158">Script file name.</span></span>|
|<span data-ttu-id="88eef-159">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="88eef-159">roleScopeTagIds</span></span>|<span data-ttu-id="88eef-160">String collection</span><span class="sxs-lookup"><span data-stu-id="88eef-160">String collection</span></span>|<span data-ttu-id="88eef-161">此 PowerShellScript 实例的范围标记 Id 的列表。</span><span class="sxs-lookup"><span data-stu-id="88eef-161">List of Scope Tag IDs for this PowerShellScript instance.</span></span>|

## <a name="relationships"></a><span data-ttu-id="88eef-162">关系</span><span class="sxs-lookup"><span data-stu-id="88eef-162">Relationships</span></span>
|<span data-ttu-id="88eef-163">关系</span><span class="sxs-lookup"><span data-stu-id="88eef-163">Relationship</span></span>|<span data-ttu-id="88eef-164">类型</span><span class="sxs-lookup"><span data-stu-id="88eef-164">Type</span></span>|<span data-ttu-id="88eef-165">说明</span><span class="sxs-lookup"><span data-stu-id="88eef-165">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88eef-166">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="88eef-166">groupAssignments</span></span>|<span data-ttu-id="88eef-167">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="88eef-167">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) collection</span></span>|<span data-ttu-id="88eef-168">设备管理脚本的组分配的列表。</span><span class="sxs-lookup"><span data-stu-id="88eef-168">The list of group assignments for the device management script.</span></span>|
|<span data-ttu-id="88eef-169">assignments</span><span class="sxs-lookup"><span data-stu-id="88eef-169">assignments</span></span>|<span data-ttu-id="88eef-170">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="88eef-170">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) collection</span></span>|<span data-ttu-id="88eef-171">设备管理脚本的组分配的列表。</span><span class="sxs-lookup"><span data-stu-id="88eef-171">The list of group assignments for the device management script.</span></span>|
|<span data-ttu-id="88eef-172">runSummary</span><span class="sxs-lookup"><span data-stu-id="88eef-172">runSummary</span></span>|[<span data-ttu-id="88eef-173">deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="88eef-173">deviceManagementScriptRunSummary</span></span>](../resources/intune-devices-devicemanagementscriptrunsummary.md)|<span data-ttu-id="88eef-174">设备管理脚本的运行摘要。</span><span class="sxs-lookup"><span data-stu-id="88eef-174">Run summary for device management script.</span></span>|
|<span data-ttu-id="88eef-175">deviceRunStates</span><span class="sxs-lookup"><span data-stu-id="88eef-175">deviceRunStates</span></span>|<span data-ttu-id="88eef-176">[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)集合</span><span class="sxs-lookup"><span data-stu-id="88eef-176">[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) collection</span></span>|<span data-ttu-id="88eef-177">此脚本在所有设备上的运行状态列表。</span><span class="sxs-lookup"><span data-stu-id="88eef-177">List of run states for this script across all devices.</span></span>|
|<span data-ttu-id="88eef-178">userRunStates</span><span class="sxs-lookup"><span data-stu-id="88eef-178">userRunStates</span></span>|<span data-ttu-id="88eef-179">[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)集合</span><span class="sxs-lookup"><span data-stu-id="88eef-179">[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) collection</span></span>|<span data-ttu-id="88eef-180">此脚本在所有用户中的运行状态列表。</span><span class="sxs-lookup"><span data-stu-id="88eef-180">List of run states for this script across all users.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="88eef-181">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="88eef-181">JSON Representation</span></span>
<span data-ttu-id="88eef-182">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="88eef-182">Here is a JSON representation of the resource.</span></span>
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



