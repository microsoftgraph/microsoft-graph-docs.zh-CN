---
title: deviceManagementScript 资源类型
description: Intune 将向客户提供在已注册的 windows 10 Azure Active Directory 联接设备上运行其 Powershell 脚本的功能。 脚本可以运行一次, 也可以定期运行。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e3fffd6bec8866066824725f1477e6de0e71ebf9
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30164062"
---
# <a name="devicemanagementscript-resource-type"></a><span data-ttu-id="ff998-104">deviceManagementScript 资源类型</span><span class="sxs-lookup"><span data-stu-id="ff998-104">deviceManagementScript resource type</span></span>

> <span data-ttu-id="ff998-105">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ff998-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ff998-106">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ff998-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff998-107">Intune 将向客户提供在已注册的 windows 10 Azure Active Directory 联接设备上运行其 Powershell 脚本的功能。</span><span class="sxs-lookup"><span data-stu-id="ff998-107">Intune will provide customer the ability to run their Powershell scripts on the enrolled windows 10 Azure Active Directory joined devices.</span></span> <span data-ttu-id="ff998-108">脚本可以运行一次, 也可以定期运行。</span><span class="sxs-lookup"><span data-stu-id="ff998-108">The script can be run once or periodically.</span></span>

## <a name="methods"></a><span data-ttu-id="ff998-109">方法</span><span class="sxs-lookup"><span data-stu-id="ff998-109">Methods</span></span>
|<span data-ttu-id="ff998-110">方法</span><span class="sxs-lookup"><span data-stu-id="ff998-110">Method</span></span>|<span data-ttu-id="ff998-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="ff998-111">Return Type</span></span>|<span data-ttu-id="ff998-112">说明</span><span class="sxs-lookup"><span data-stu-id="ff998-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ff998-113">列出 deviceManagementScripts</span><span class="sxs-lookup"><span data-stu-id="ff998-113">List deviceManagementScripts</span></span>](../api/intune-devices-devicemanagementscript-list.md)|<span data-ttu-id="ff998-114">[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)集合</span><span class="sxs-lookup"><span data-stu-id="ff998-114">[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) collection</span></span>|<span data-ttu-id="ff998-115">列出[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ff998-115">List properties and relationships of the [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) objects.</span></span>|
|[<span data-ttu-id="ff998-116">获取 deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="ff998-116">Get deviceManagementScript</span></span>](../api/intune-devices-devicemanagementscript-get.md)|[<span data-ttu-id="ff998-117">deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="ff998-117">deviceManagementScript</span></span>](../resources/intune-devices-devicemanagementscript.md)|<span data-ttu-id="ff998-118">读取[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ff998-118">Read properties and relationships of the [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object.</span></span>|
|[<span data-ttu-id="ff998-119">创建 deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="ff998-119">Create deviceManagementScript</span></span>](../api/intune-devices-devicemanagementscript-create.md)|[<span data-ttu-id="ff998-120">deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="ff998-120">deviceManagementScript</span></span>](../resources/intune-devices-devicemanagementscript.md)|<span data-ttu-id="ff998-121">创建新的[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ff998-121">Create a new [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object.</span></span>|
|[<span data-ttu-id="ff998-122">删除 deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="ff998-122">Delete deviceManagementScript</span></span>](../api/intune-devices-devicemanagementscript-delete.md)|<span data-ttu-id="ff998-123">无</span><span class="sxs-lookup"><span data-stu-id="ff998-123">None</span></span>|<span data-ttu-id="ff998-124">删除[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)。</span><span class="sxs-lookup"><span data-stu-id="ff998-124">Deletes a [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md).</span></span>|
|[<span data-ttu-id="ff998-125">更新 deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="ff998-125">Update deviceManagementScript</span></span>](../api/intune-devices-devicemanagementscript-update.md)|[<span data-ttu-id="ff998-126">deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="ff998-126">deviceManagementScript</span></span>](../resources/intune-devices-devicemanagementscript.md)|<span data-ttu-id="ff998-127">更新[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ff998-127">Update the properties of a [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object.</span></span>|
|[<span data-ttu-id="ff998-128">assign 操作</span><span class="sxs-lookup"><span data-stu-id="ff998-128">assign action</span></span>](../api/intune-devices-devicemanagementscript-assign.md)|<span data-ttu-id="ff998-129">无</span><span class="sxs-lookup"><span data-stu-id="ff998-129">None</span></span>|<span data-ttu-id="ff998-130">尚未记录</span><span class="sxs-lookup"><span data-stu-id="ff998-130">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="ff998-131">属性</span><span class="sxs-lookup"><span data-stu-id="ff998-131">Properties</span></span>
|<span data-ttu-id="ff998-132">属性</span><span class="sxs-lookup"><span data-stu-id="ff998-132">Property</span></span>|<span data-ttu-id="ff998-133">类型</span><span class="sxs-lookup"><span data-stu-id="ff998-133">Type</span></span>|<span data-ttu-id="ff998-134">说明</span><span class="sxs-lookup"><span data-stu-id="ff998-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff998-135">id</span><span class="sxs-lookup"><span data-stu-id="ff998-135">id</span></span>|<span data-ttu-id="ff998-136">字串符号</span><span class="sxs-lookup"><span data-stu-id="ff998-136">String</span></span>|<span data-ttu-id="ff998-137">设备管理脚本的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="ff998-137">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="ff998-138">displayName</span><span class="sxs-lookup"><span data-stu-id="ff998-138">displayName</span></span>|<span data-ttu-id="ff998-139">字符串</span><span class="sxs-lookup"><span data-stu-id="ff998-139">String</span></span>|<span data-ttu-id="ff998-140">设备管理脚本的名称。</span><span class="sxs-lookup"><span data-stu-id="ff998-140">Name of the device management script.</span></span>|
|<span data-ttu-id="ff998-141">说明</span><span class="sxs-lookup"><span data-stu-id="ff998-141">description</span></span>|<span data-ttu-id="ff998-142">字符串</span><span class="sxs-lookup"><span data-stu-id="ff998-142">String</span></span>|<span data-ttu-id="ff998-143">设备管理脚本的可选说明。</span><span class="sxs-lookup"><span data-stu-id="ff998-143">Optional description for the device management script.</span></span>|
|<span data-ttu-id="ff998-144">runSchedule</span><span class="sxs-lookup"><span data-stu-id="ff998-144">runSchedule</span></span>|[<span data-ttu-id="ff998-145">runSchedule</span><span class="sxs-lookup"><span data-stu-id="ff998-145">runSchedule</span></span>](../resources/intune-devices-runschedule.md)|<span data-ttu-id="ff998-146">脚本运行的间隔。</span><span class="sxs-lookup"><span data-stu-id="ff998-146">The interval for script to run.</span></span> <span data-ttu-id="ff998-147">如果未定义, 脚本将运行一次</span><span class="sxs-lookup"><span data-stu-id="ff998-147">If not defined the script will run once</span></span>|
|<span data-ttu-id="ff998-148">scriptContent</span><span class="sxs-lookup"><span data-stu-id="ff998-148">scriptContent</span></span>|<span data-ttu-id="ff998-149">Binary</span><span class="sxs-lookup"><span data-stu-id="ff998-149">Binary</span></span>|<span data-ttu-id="ff998-150">脚本内容。</span><span class="sxs-lookup"><span data-stu-id="ff998-150">The script content.</span></span>|
|<span data-ttu-id="ff998-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ff998-151">createdDateTime</span></span>|<span data-ttu-id="ff998-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff998-152">DateTimeOffset</span></span>|<span data-ttu-id="ff998-153">设备管理脚本的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="ff998-153">The date and time the device management script was created.</span></span>|
|<span data-ttu-id="ff998-154">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ff998-154">lastModifiedDateTime</span></span>|<span data-ttu-id="ff998-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff998-155">DateTimeOffset</span></span>|<span data-ttu-id="ff998-156">上次修改设备管理脚本的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="ff998-156">The date and time the device management script was last modified.</span></span>|
|<span data-ttu-id="ff998-157">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="ff998-157">runAsAccount</span></span>|[<span data-ttu-id="ff998-158">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="ff998-158">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="ff998-159">指示设备管理脚本在其中运行的执行上下文的类型。</span><span class="sxs-lookup"><span data-stu-id="ff998-159">Indicates the type of execution context the device management script runs in.</span></span> <span data-ttu-id="ff998-160">可取值为：`system`、`user`。</span><span class="sxs-lookup"><span data-stu-id="ff998-160">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="ff998-161">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="ff998-161">enforceSignatureCheck</span></span>|<span data-ttu-id="ff998-162">布尔</span><span class="sxs-lookup"><span data-stu-id="ff998-162">Boolean</span></span>|<span data-ttu-id="ff998-163">指示是否需要检查脚本签名。</span><span class="sxs-lookup"><span data-stu-id="ff998-163">Indicate whether the script signature needs be checked.</span></span>|
|<span data-ttu-id="ff998-164">fileName</span><span class="sxs-lookup"><span data-stu-id="ff998-164">fileName</span></span>|<span data-ttu-id="ff998-165">String</span><span class="sxs-lookup"><span data-stu-id="ff998-165">String</span></span>|<span data-ttu-id="ff998-166">脚本文件名。</span><span class="sxs-lookup"><span data-stu-id="ff998-166">Script file name.</span></span>|
|<span data-ttu-id="ff998-167">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ff998-167">roleScopeTagIds</span></span>|<span data-ttu-id="ff998-168">String collection</span><span class="sxs-lookup"><span data-stu-id="ff998-168">String collection</span></span>|<span data-ttu-id="ff998-169">此 PowerShellScript 实例的范围标记 id 的列表。</span><span class="sxs-lookup"><span data-stu-id="ff998-169">List of Scope Tag IDs for this PowerShellScript instance.</span></span>|
|<span data-ttu-id="ff998-170">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="ff998-170">runAs32Bit</span></span>|<span data-ttu-id="ff998-171">布尔</span><span class="sxs-lookup"><span data-stu-id="ff998-171">Boolean</span></span>|<span data-ttu-id="ff998-172">一个指示 PowerShell 脚本是否应作为32位运行的值</span><span class="sxs-lookup"><span data-stu-id="ff998-172">A value indicating whether the PowerShell script should run as 32-bit</span></span>|

## <a name="relationships"></a><span data-ttu-id="ff998-173">关系</span><span class="sxs-lookup"><span data-stu-id="ff998-173">Relationships</span></span>
|<span data-ttu-id="ff998-174">关系</span><span class="sxs-lookup"><span data-stu-id="ff998-174">Relationship</span></span>|<span data-ttu-id="ff998-175">类型</span><span class="sxs-lookup"><span data-stu-id="ff998-175">Type</span></span>|<span data-ttu-id="ff998-176">说明</span><span class="sxs-lookup"><span data-stu-id="ff998-176">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff998-177">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="ff998-177">groupAssignments</span></span>|<span data-ttu-id="ff998-178">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="ff998-178">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) collection</span></span>|<span data-ttu-id="ff998-179">设备管理脚本的组分配的列表。</span><span class="sxs-lookup"><span data-stu-id="ff998-179">The list of group assignments for the device management script.</span></span>|
|<span data-ttu-id="ff998-180">assignments</span><span class="sxs-lookup"><span data-stu-id="ff998-180">assignments</span></span>|<span data-ttu-id="ff998-181">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="ff998-181">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) collection</span></span>|<span data-ttu-id="ff998-182">设备管理脚本的组分配的列表。</span><span class="sxs-lookup"><span data-stu-id="ff998-182">The list of group assignments for the device management script.</span></span>|
|<span data-ttu-id="ff998-183">runSummary</span><span class="sxs-lookup"><span data-stu-id="ff998-183">runSummary</span></span>|[<span data-ttu-id="ff998-184">deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="ff998-184">deviceManagementScriptRunSummary</span></span>](../resources/intune-devices-devicemanagementscriptrunsummary.md)|<span data-ttu-id="ff998-185">设备管理脚本的运行摘要。</span><span class="sxs-lookup"><span data-stu-id="ff998-185">Run summary for device management script.</span></span>|
|<span data-ttu-id="ff998-186">deviceRunStates</span><span class="sxs-lookup"><span data-stu-id="ff998-186">deviceRunStates</span></span>|<span data-ttu-id="ff998-187">[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)集合</span><span class="sxs-lookup"><span data-stu-id="ff998-187">[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) collection</span></span>|<span data-ttu-id="ff998-188">此脚本在所有设备上的运行状态列表。</span><span class="sxs-lookup"><span data-stu-id="ff998-188">List of run states for this script across all devices.</span></span>|
|<span data-ttu-id="ff998-189">userRunStates</span><span class="sxs-lookup"><span data-stu-id="ff998-189">userRunStates</span></span>|<span data-ttu-id="ff998-190">[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)集合</span><span class="sxs-lookup"><span data-stu-id="ff998-190">[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) collection</span></span>|<span data-ttu-id="ff998-191">此脚本在所有用户中的运行状态列表。</span><span class="sxs-lookup"><span data-stu-id="ff998-191">List of run states for this script across all users.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ff998-192">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ff998-192">JSON Representation</span></span>
<span data-ttu-id="ff998-193">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ff998-193">Here is a JSON representation of the resource.</span></span>
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




