---
title: deviceManagementScript 资源类型
description: Intune 将使客户能够在注册的 windows 10 Azure Active Directory 加入设备上运行其 Powershell 脚本。 一次或定期，可以运行该脚本。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4fda826ec8033cd51ad4dd13dbc5b523a21e9e3a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412525"
---
# <a name="devicemanagementscript-resource-type"></a><span data-ttu-id="0e9dd-104">deviceManagementScript 资源类型</span><span class="sxs-lookup"><span data-stu-id="0e9dd-104">deviceManagementScript resource type</span></span>

> <span data-ttu-id="0e9dd-105">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="0e9dd-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0e9dd-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0e9dd-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0e9dd-107">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0e9dd-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0e9dd-108">Intune 将使客户能够在注册的 windows 10 Azure Active Directory 加入设备上运行其 Powershell 脚本。</span><span class="sxs-lookup"><span data-stu-id="0e9dd-108">Intune will provide customer the ability to run their Powershell scripts on the enrolled windows 10 Azure Active Directory joined devices.</span></span> <span data-ttu-id="0e9dd-109">一次或定期，可以运行该脚本。</span><span class="sxs-lookup"><span data-stu-id="0e9dd-109">The script can be run once or periodically.</span></span>

## <a name="methods"></a><span data-ttu-id="0e9dd-110">方法</span><span class="sxs-lookup"><span data-stu-id="0e9dd-110">Methods</span></span>
|<span data-ttu-id="0e9dd-111">方法</span><span class="sxs-lookup"><span data-stu-id="0e9dd-111">Method</span></span>|<span data-ttu-id="0e9dd-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="0e9dd-112">Return Type</span></span>|<span data-ttu-id="0e9dd-113">说明</span><span class="sxs-lookup"><span data-stu-id="0e9dd-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0e9dd-114">列表 deviceManagementScripts</span><span class="sxs-lookup"><span data-stu-id="0e9dd-114">List deviceManagementScripts</span></span>](../api/intune-devices-devicemanagementscript-list.md)|<span data-ttu-id="0e9dd-115">[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)集合</span><span class="sxs-lookup"><span data-stu-id="0e9dd-115">[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) collection</span></span>|<span data-ttu-id="0e9dd-116">列出属性和[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="0e9dd-116">List properties and relationships of the [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) objects.</span></span>|
|[<span data-ttu-id="0e9dd-117">获取 deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="0e9dd-117">Get deviceManagementScript</span></span>](../api/intune-devices-devicemanagementscript-get.md)|[<span data-ttu-id="0e9dd-118">deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="0e9dd-118">deviceManagementScript</span></span>](../resources/intune-devices-devicemanagementscript.md)|<span data-ttu-id="0e9dd-119">读取属性和[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="0e9dd-119">Read properties and relationships of the [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object.</span></span>|
|[<span data-ttu-id="0e9dd-120">创建 deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="0e9dd-120">Create deviceManagementScript</span></span>](../api/intune-devices-devicemanagementscript-create.md)|[<span data-ttu-id="0e9dd-121">deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="0e9dd-121">deviceManagementScript</span></span>](../resources/intune-devices-devicemanagementscript.md)|<span data-ttu-id="0e9dd-122">创建新的[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0e9dd-122">Create a new [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object.</span></span>|
|[<span data-ttu-id="0e9dd-123">删除 deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="0e9dd-123">Delete deviceManagementScript</span></span>](../api/intune-devices-devicemanagementscript-delete.md)|<span data-ttu-id="0e9dd-124">无</span><span class="sxs-lookup"><span data-stu-id="0e9dd-124">None</span></span>|<span data-ttu-id="0e9dd-125">删除[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)。</span><span class="sxs-lookup"><span data-stu-id="0e9dd-125">Deletes a [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md).</span></span>|
|[<span data-ttu-id="0e9dd-126">更新 deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="0e9dd-126">Update deviceManagementScript</span></span>](../api/intune-devices-devicemanagementscript-update.md)|[<span data-ttu-id="0e9dd-127">deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="0e9dd-127">deviceManagementScript</span></span>](../resources/intune-devices-devicemanagementscript.md)|<span data-ttu-id="0e9dd-128">更新[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0e9dd-128">Update the properties of a [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object.</span></span>|
|[<span data-ttu-id="0e9dd-129">assign 操作</span><span class="sxs-lookup"><span data-stu-id="0e9dd-129">assign action</span></span>](../api/intune-devices-devicemanagementscript-assign.md)|<span data-ttu-id="0e9dd-130">无</span><span class="sxs-lookup"><span data-stu-id="0e9dd-130">None</span></span>|<span data-ttu-id="0e9dd-131">尚未记录</span><span class="sxs-lookup"><span data-stu-id="0e9dd-131">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="0e9dd-132">属性</span><span class="sxs-lookup"><span data-stu-id="0e9dd-132">Properties</span></span>
|<span data-ttu-id="0e9dd-133">属性</span><span class="sxs-lookup"><span data-stu-id="0e9dd-133">Property</span></span>|<span data-ttu-id="0e9dd-134">类型</span><span class="sxs-lookup"><span data-stu-id="0e9dd-134">Type</span></span>|<span data-ttu-id="0e9dd-135">说明</span><span class="sxs-lookup"><span data-stu-id="0e9dd-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e9dd-136">id</span><span class="sxs-lookup"><span data-stu-id="0e9dd-136">id</span></span>|<span data-ttu-id="0e9dd-137">String</span><span class="sxs-lookup"><span data-stu-id="0e9dd-137">String</span></span>|<span data-ttu-id="0e9dd-138">设备管理脚本的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="0e9dd-138">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="0e9dd-139">displayName</span><span class="sxs-lookup"><span data-stu-id="0e9dd-139">displayName</span></span>|<span data-ttu-id="0e9dd-140">String</span><span class="sxs-lookup"><span data-stu-id="0e9dd-140">String</span></span>|<span data-ttu-id="0e9dd-141">设备管理脚本的名称。</span><span class="sxs-lookup"><span data-stu-id="0e9dd-141">Name of the device management script.</span></span>|
|<span data-ttu-id="0e9dd-142">说明</span><span class="sxs-lookup"><span data-stu-id="0e9dd-142">description</span></span>|<span data-ttu-id="0e9dd-143">String</span><span class="sxs-lookup"><span data-stu-id="0e9dd-143">String</span></span>|<span data-ttu-id="0e9dd-144">设备管理脚本的可选说明。</span><span class="sxs-lookup"><span data-stu-id="0e9dd-144">Optional description for the device management script.</span></span>|
|<span data-ttu-id="0e9dd-145">runSchedule</span><span class="sxs-lookup"><span data-stu-id="0e9dd-145">runSchedule</span></span>|[<span data-ttu-id="0e9dd-146">runSchedule</span><span class="sxs-lookup"><span data-stu-id="0e9dd-146">runSchedule</span></span>](../resources/intune-devices-runschedule.md)|<span data-ttu-id="0e9dd-147">Script to run 时间间隔。</span><span class="sxs-lookup"><span data-stu-id="0e9dd-147">The interval for script to run.</span></span> <span data-ttu-id="0e9dd-148">如果未定义脚本将运行一次</span><span class="sxs-lookup"><span data-stu-id="0e9dd-148">If not defined the script will run once</span></span>|
|<span data-ttu-id="0e9dd-149">scriptContent</span><span class="sxs-lookup"><span data-stu-id="0e9dd-149">scriptContent</span></span>|<span data-ttu-id="0e9dd-150">Binary</span><span class="sxs-lookup"><span data-stu-id="0e9dd-150">Binary</span></span>|<span data-ttu-id="0e9dd-151">脚本内容。</span><span class="sxs-lookup"><span data-stu-id="0e9dd-151">The script content.</span></span>|
|<span data-ttu-id="0e9dd-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0e9dd-152">createdDateTime</span></span>|<span data-ttu-id="0e9dd-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e9dd-153">DateTimeOffset</span></span>|<span data-ttu-id="0e9dd-154">创建设备管理脚本的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="0e9dd-154">The date and time the device management script was created.</span></span>|
|<span data-ttu-id="0e9dd-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0e9dd-155">lastModifiedDateTime</span></span>|<span data-ttu-id="0e9dd-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e9dd-156">DateTimeOffset</span></span>|<span data-ttu-id="0e9dd-157">日期和设备管理脚本上次修改的时间。</span><span class="sxs-lookup"><span data-stu-id="0e9dd-157">The date and time the device management script was last modified.</span></span>|
|<span data-ttu-id="0e9dd-158">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="0e9dd-158">runAsAccount</span></span>|[<span data-ttu-id="0e9dd-159">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="0e9dd-159">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="0e9dd-160">指示执行上下文中运行的设备管理脚本的类型。</span><span class="sxs-lookup"><span data-stu-id="0e9dd-160">Indicates the type of execution context the device management script runs in.</span></span> <span data-ttu-id="0e9dd-161">可取值为：`system`、`user`。</span><span class="sxs-lookup"><span data-stu-id="0e9dd-161">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="0e9dd-162">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="0e9dd-162">enforceSignatureCheck</span></span>|<span data-ttu-id="0e9dd-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="0e9dd-163">Boolean</span></span>|<span data-ttu-id="0e9dd-164">指示是否需要签脚本签名。</span><span class="sxs-lookup"><span data-stu-id="0e9dd-164">Indicate whether the script signature needs be checked.</span></span>|
|<span data-ttu-id="0e9dd-165">fileName</span><span class="sxs-lookup"><span data-stu-id="0e9dd-165">fileName</span></span>|<span data-ttu-id="0e9dd-166">String</span><span class="sxs-lookup"><span data-stu-id="0e9dd-166">String</span></span>|<span data-ttu-id="0e9dd-167">脚本文件的名称。</span><span class="sxs-lookup"><span data-stu-id="0e9dd-167">Script file name.</span></span>|
|<span data-ttu-id="0e9dd-168">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0e9dd-168">roleScopeTagIds</span></span>|<span data-ttu-id="0e9dd-169">String 集合</span><span class="sxs-lookup"><span data-stu-id="0e9dd-169">String collection</span></span>|<span data-ttu-id="0e9dd-170">此 PowerShellScript 实例范围标记 Id 的列表。</span><span class="sxs-lookup"><span data-stu-id="0e9dd-170">List of Scope Tag IDs for this PowerShellScript instance.</span></span>|
|<span data-ttu-id="0e9dd-171">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="0e9dd-171">runAs32Bit</span></span>|<span data-ttu-id="0e9dd-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="0e9dd-172">Boolean</span></span>|<span data-ttu-id="0e9dd-173">一个值，该值的 PowerShell 脚本是否应运行 32 位</span><span class="sxs-lookup"><span data-stu-id="0e9dd-173">A value indicating whether the PowerShell script should run as 32-bit</span></span>|

## <a name="relationships"></a><span data-ttu-id="0e9dd-174">关系</span><span class="sxs-lookup"><span data-stu-id="0e9dd-174">Relationships</span></span>
|<span data-ttu-id="0e9dd-175">关系</span><span class="sxs-lookup"><span data-stu-id="0e9dd-175">Relationship</span></span>|<span data-ttu-id="0e9dd-176">类型</span><span class="sxs-lookup"><span data-stu-id="0e9dd-176">Type</span></span>|<span data-ttu-id="0e9dd-177">说明</span><span class="sxs-lookup"><span data-stu-id="0e9dd-177">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e9dd-178">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="0e9dd-178">groupAssignments</span></span>|<span data-ttu-id="0e9dd-179">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="0e9dd-179">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) collection</span></span>|<span data-ttu-id="0e9dd-180">设备管理脚本的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="0e9dd-180">The list of group assignments for the device management script.</span></span>|
|<span data-ttu-id="0e9dd-181">assignments</span><span class="sxs-lookup"><span data-stu-id="0e9dd-181">assignments</span></span>|<span data-ttu-id="0e9dd-182">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="0e9dd-182">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) collection</span></span>|<span data-ttu-id="0e9dd-183">设备管理脚本的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="0e9dd-183">The list of group assignments for the device management script.</span></span>|
|<span data-ttu-id="0e9dd-184">runSummary</span><span class="sxs-lookup"><span data-stu-id="0e9dd-184">runSummary</span></span>|[<span data-ttu-id="0e9dd-185">deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="0e9dd-185">deviceManagementScriptRunSummary</span></span>](../resources/intune-devices-devicemanagementscriptrunsummary.md)|<span data-ttu-id="0e9dd-186">运行设备管理脚本摘要。</span><span class="sxs-lookup"><span data-stu-id="0e9dd-186">Run summary for device management script.</span></span>|
|<span data-ttu-id="0e9dd-187">deviceRunStates</span><span class="sxs-lookup"><span data-stu-id="0e9dd-187">deviceRunStates</span></span>|<span data-ttu-id="0e9dd-188">[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)集合</span><span class="sxs-lookup"><span data-stu-id="0e9dd-188">[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) collection</span></span>|<span data-ttu-id="0e9dd-189">此脚本跨所有设备的运行状态的列表。</span><span class="sxs-lookup"><span data-stu-id="0e9dd-189">List of run states for this script across all devices.</span></span>|
|<span data-ttu-id="0e9dd-190">userRunStates</span><span class="sxs-lookup"><span data-stu-id="0e9dd-190">userRunStates</span></span>|<span data-ttu-id="0e9dd-191">[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)集合</span><span class="sxs-lookup"><span data-stu-id="0e9dd-191">[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) collection</span></span>|<span data-ttu-id="0e9dd-192">列表的所有用户此脚本运行状态。</span><span class="sxs-lookup"><span data-stu-id="0e9dd-192">List of run states for this script across all users.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0e9dd-193">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0e9dd-193">JSON Representation</span></span>
<span data-ttu-id="0e9dd-194">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0e9dd-194">Here is a JSON representation of the resource.</span></span>
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




