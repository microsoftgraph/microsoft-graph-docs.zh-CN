---
title: deviceManagementScript 资源类型
description: Intune 将使客户能够在注册的 windows 10 Azure Active Directory 加入设备上运行其 Powershell 脚本。 一次或定期，可以运行该脚本。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 321d525aaf9de386ba639bc904915a06eda56a75
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27811044"
---
# <a name="devicemanagementscript-resource-type"></a><span data-ttu-id="c6ef6-104">deviceManagementScript 资源类型</span><span class="sxs-lookup"><span data-stu-id="c6ef6-104">deviceManagementScript resource type</span></span>

> <span data-ttu-id="c6ef6-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c6ef6-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c6ef6-106">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c6ef6-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c6ef6-107">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="c6ef6-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c6ef6-108">Intune 将使客户能够在注册的 windows 10 Azure Active Directory 加入设备上运行其 Powershell 脚本。</span><span class="sxs-lookup"><span data-stu-id="c6ef6-108">Intune will provide customer the ability to run their Powershell scripts on the enrolled windows 10 Azure Active Directory joined devices.</span></span> <span data-ttu-id="c6ef6-109">一次或定期，可以运行该脚本。</span><span class="sxs-lookup"><span data-stu-id="c6ef6-109">The script can be run once or periodically.</span></span>
## <a name="methods"></a><span data-ttu-id="c6ef6-110">方法</span><span class="sxs-lookup"><span data-stu-id="c6ef6-110">Methods</span></span>
|<span data-ttu-id="c6ef6-111">方法</span><span class="sxs-lookup"><span data-stu-id="c6ef6-111">Method</span></span>|<span data-ttu-id="c6ef6-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="c6ef6-112">Return Type</span></span>|<span data-ttu-id="c6ef6-113">说明</span><span class="sxs-lookup"><span data-stu-id="c6ef6-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c6ef6-114">列表 deviceManagementScripts</span><span class="sxs-lookup"><span data-stu-id="c6ef6-114">List deviceManagementScripts</span></span>](../api/intune-devices-devicemanagementscript-list.md)|<span data-ttu-id="c6ef6-115">[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)集合</span><span class="sxs-lookup"><span data-stu-id="c6ef6-115">[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) collection</span></span>|<span data-ttu-id="c6ef6-116">列出属性和[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="c6ef6-116">List properties and relationships of the [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) objects.</span></span>|
|[<span data-ttu-id="c6ef6-117">获取 deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="c6ef6-117">Get deviceManagementScript</span></span>](../api/intune-devices-devicemanagementscript-get.md)|[<span data-ttu-id="c6ef6-118">deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="c6ef6-118">deviceManagementScript</span></span>](../resources/intune-devices-devicemanagementscript.md)|<span data-ttu-id="c6ef6-119">读取属性和[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="c6ef6-119">Read properties and relationships of the [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object.</span></span>|
|[<span data-ttu-id="c6ef6-120">创建 deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="c6ef6-120">Create deviceManagementScript</span></span>](../api/intune-devices-devicemanagementscript-create.md)|[<span data-ttu-id="c6ef6-121">deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="c6ef6-121">deviceManagementScript</span></span>](../resources/intune-devices-devicemanagementscript.md)|<span data-ttu-id="c6ef6-122">创建新的[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c6ef6-122">Create a new [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object.</span></span>|
|[<span data-ttu-id="c6ef6-123">删除 deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="c6ef6-123">Delete deviceManagementScript</span></span>](../api/intune-devices-devicemanagementscript-delete.md)|<span data-ttu-id="c6ef6-124">无</span><span class="sxs-lookup"><span data-stu-id="c6ef6-124">None</span></span>|<span data-ttu-id="c6ef6-125">删除[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)。</span><span class="sxs-lookup"><span data-stu-id="c6ef6-125">Deletes a [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md).</span></span>|
|[<span data-ttu-id="c6ef6-126">更新 deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="c6ef6-126">Update deviceManagementScript</span></span>](../api/intune-devices-devicemanagementscript-update.md)|[<span data-ttu-id="c6ef6-127">deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="c6ef6-127">deviceManagementScript</span></span>](../resources/intune-devices-devicemanagementscript.md)|<span data-ttu-id="c6ef6-128">更新[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c6ef6-128">Update the properties of a [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object.</span></span>|
|[<span data-ttu-id="c6ef6-129">assign 操作</span><span class="sxs-lookup"><span data-stu-id="c6ef6-129">assign action</span></span>](../api/intune-devices-devicemanagementscript-assign.md)|<span data-ttu-id="c6ef6-130">无</span><span class="sxs-lookup"><span data-stu-id="c6ef6-130">None</span></span>|<span data-ttu-id="c6ef6-131">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c6ef6-131">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="c6ef6-132">属性</span><span class="sxs-lookup"><span data-stu-id="c6ef6-132">Properties</span></span>
|<span data-ttu-id="c6ef6-133">属性</span><span class="sxs-lookup"><span data-stu-id="c6ef6-133">Property</span></span>|<span data-ttu-id="c6ef6-134">类型</span><span class="sxs-lookup"><span data-stu-id="c6ef6-134">Type</span></span>|<span data-ttu-id="c6ef6-135">说明</span><span class="sxs-lookup"><span data-stu-id="c6ef6-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6ef6-136">id</span><span class="sxs-lookup"><span data-stu-id="c6ef6-136">id</span></span>|<span data-ttu-id="c6ef6-137">字符串</span><span class="sxs-lookup"><span data-stu-id="c6ef6-137">String</span></span>|<span data-ttu-id="c6ef6-138">设备管理脚本的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="c6ef6-138">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="c6ef6-139">displayName</span><span class="sxs-lookup"><span data-stu-id="c6ef6-139">displayName</span></span>|<span data-ttu-id="c6ef6-140">字符串</span><span class="sxs-lookup"><span data-stu-id="c6ef6-140">String</span></span>|<span data-ttu-id="c6ef6-141">设备管理脚本的名称。</span><span class="sxs-lookup"><span data-stu-id="c6ef6-141">Name of the device management script.</span></span>|
|<span data-ttu-id="c6ef6-142">说明</span><span class="sxs-lookup"><span data-stu-id="c6ef6-142">description</span></span>|<span data-ttu-id="c6ef6-143">字符串</span><span class="sxs-lookup"><span data-stu-id="c6ef6-143">String</span></span>|<span data-ttu-id="c6ef6-144">设备管理脚本的可选说明。</span><span class="sxs-lookup"><span data-stu-id="c6ef6-144">Optional description for the device management script.</span></span>|
|<span data-ttu-id="c6ef6-145">runSchedule</span><span class="sxs-lookup"><span data-stu-id="c6ef6-145">runSchedule</span></span>|[<span data-ttu-id="c6ef6-146">runSchedule</span><span class="sxs-lookup"><span data-stu-id="c6ef6-146">runSchedule</span></span>](../resources/intune-devices-runschedule.md)|<span data-ttu-id="c6ef6-147">Script to run 时间间隔。</span><span class="sxs-lookup"><span data-stu-id="c6ef6-147">The interval for script to run.</span></span> <span data-ttu-id="c6ef6-148">如果未定义脚本将运行一次</span><span class="sxs-lookup"><span data-stu-id="c6ef6-148">If not defined the script will run once</span></span>|
|<span data-ttu-id="c6ef6-149">scriptContent</span><span class="sxs-lookup"><span data-stu-id="c6ef6-149">scriptContent</span></span>|<span data-ttu-id="c6ef6-150">Binary</span><span class="sxs-lookup"><span data-stu-id="c6ef6-150">Binary</span></span>|<span data-ttu-id="c6ef6-151">脚本内容。</span><span class="sxs-lookup"><span data-stu-id="c6ef6-151">The script content.</span></span>|
|<span data-ttu-id="c6ef6-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c6ef6-152">createdDateTime</span></span>|<span data-ttu-id="c6ef6-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c6ef6-153">DateTimeOffset</span></span>|<span data-ttu-id="c6ef6-154">创建设备管理脚本的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="c6ef6-154">The date and time the device management script was created.</span></span>|
|<span data-ttu-id="c6ef6-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c6ef6-155">lastModifiedDateTime</span></span>|<span data-ttu-id="c6ef6-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c6ef6-156">DateTimeOffset</span></span>|<span data-ttu-id="c6ef6-157">日期和设备管理脚本上次修改的时间。</span><span class="sxs-lookup"><span data-stu-id="c6ef6-157">The date and time the device management script was last modified.</span></span>|
|<span data-ttu-id="c6ef6-158">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="c6ef6-158">runAsAccount</span></span>|[<span data-ttu-id="c6ef6-159">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="c6ef6-159">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="c6ef6-160">指示执行上下文中运行的设备管理脚本的类型。</span><span class="sxs-lookup"><span data-stu-id="c6ef6-160">Indicates the type of execution context the device management script runs in.</span></span> <span data-ttu-id="c6ef6-161">可取值为：`system`、`user`。</span><span class="sxs-lookup"><span data-stu-id="c6ef6-161">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="c6ef6-162">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="c6ef6-162">enforceSignatureCheck</span></span>|<span data-ttu-id="c6ef6-163">布尔</span><span class="sxs-lookup"><span data-stu-id="c6ef6-163">Boolean</span></span>|<span data-ttu-id="c6ef6-164">指示是否需要签脚本签名。</span><span class="sxs-lookup"><span data-stu-id="c6ef6-164">Indicate whether the script signature needs be checked.</span></span>|
|<span data-ttu-id="c6ef6-165">fileName</span><span class="sxs-lookup"><span data-stu-id="c6ef6-165">fileName</span></span>|<span data-ttu-id="c6ef6-166">String</span><span class="sxs-lookup"><span data-stu-id="c6ef6-166">String</span></span>|<span data-ttu-id="c6ef6-167">脚本文件的名称。</span><span class="sxs-lookup"><span data-stu-id="c6ef6-167">Script file name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c6ef6-168">Relationships</span><span class="sxs-lookup"><span data-stu-id="c6ef6-168">Relationships</span></span>
|<span data-ttu-id="c6ef6-169">关系</span><span class="sxs-lookup"><span data-stu-id="c6ef6-169">Relationship</span></span>|<span data-ttu-id="c6ef6-170">类型</span><span class="sxs-lookup"><span data-stu-id="c6ef6-170">Type</span></span>|<span data-ttu-id="c6ef6-171">Description</span><span class="sxs-lookup"><span data-stu-id="c6ef6-171">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6ef6-172">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="c6ef6-172">groupAssignments</span></span>|<span data-ttu-id="c6ef6-173">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="c6ef6-173">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) collection</span></span>|<span data-ttu-id="c6ef6-174">设备管理脚本的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="c6ef6-174">The list of group assignments for the device management script.</span></span>|
|<span data-ttu-id="c6ef6-175">assignments</span><span class="sxs-lookup"><span data-stu-id="c6ef6-175">assignments</span></span>|<span data-ttu-id="c6ef6-176">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="c6ef6-176">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) collection</span></span>|<span data-ttu-id="c6ef6-177">设备管理脚本的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="c6ef6-177">The list of group assignments for the device management script.</span></span>|
|<span data-ttu-id="c6ef6-178">runSummary</span><span class="sxs-lookup"><span data-stu-id="c6ef6-178">runSummary</span></span>|[<span data-ttu-id="c6ef6-179">deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="c6ef6-179">deviceManagementScriptRunSummary</span></span>](../resources/intune-devices-devicemanagementscriptrunsummary.md)|<span data-ttu-id="c6ef6-180">运行设备管理脚本摘要。</span><span class="sxs-lookup"><span data-stu-id="c6ef6-180">Run summary for device management script.</span></span>|
|<span data-ttu-id="c6ef6-181">deviceRunStates</span><span class="sxs-lookup"><span data-stu-id="c6ef6-181">deviceRunStates</span></span>|<span data-ttu-id="c6ef6-182">[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)集合</span><span class="sxs-lookup"><span data-stu-id="c6ef6-182">[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) collection</span></span>|<span data-ttu-id="c6ef6-183">此脚本跨所有设备的运行状态的列表。</span><span class="sxs-lookup"><span data-stu-id="c6ef6-183">List of run states for this script across all devices.</span></span>|
|<span data-ttu-id="c6ef6-184">userRunStates</span><span class="sxs-lookup"><span data-stu-id="c6ef6-184">userRunStates</span></span>|<span data-ttu-id="c6ef6-185">[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)集合</span><span class="sxs-lookup"><span data-stu-id="c6ef6-185">[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) collection</span></span>|<span data-ttu-id="c6ef6-186">列表的所有用户此脚本运行状态。</span><span class="sxs-lookup"><span data-stu-id="c6ef6-186">List of run states for this script across all users.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c6ef6-187">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c6ef6-187">JSON Representation</span></span>
<span data-ttu-id="c6ef6-188">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c6ef6-188">Here is a JSON representation of the resource.</span></span>
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
  "fileName": "String"
}
```





