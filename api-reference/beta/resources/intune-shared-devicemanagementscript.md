---
title: deviceManagementScript 资源类型
description: Intune 将向客户提供在已注册的 windows 10 Azure Active Directory 联接设备上运行其 Powershell 脚本的功能。 脚本可以运行一次，也可以定期运行。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1ed2e4a12d7070a93bd47662714d646a640989c1
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37199934"
---
# <a name="devicemanagementscript-resource-type"></a><span data-ttu-id="558cd-104">deviceManagementScript 资源类型</span><span class="sxs-lookup"><span data-stu-id="558cd-104">deviceManagementScript resource type</span></span>

> <span data-ttu-id="558cd-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="558cd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="558cd-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="558cd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="558cd-107">Intune 将向客户提供在已注册的 windows 10 Azure Active Directory 联接设备上运行其 Powershell 脚本的功能。</span><span class="sxs-lookup"><span data-stu-id="558cd-107">Intune will provide customer the ability to run their Powershell scripts on the enrolled windows 10 Azure Active Directory joined devices.</span></span> <span data-ttu-id="558cd-108">脚本可以运行一次，也可以定期运行。</span><span class="sxs-lookup"><span data-stu-id="558cd-108">The script can be run once or periodically.</span></span>

## <a name="methods"></a><span data-ttu-id="558cd-109">方法</span><span class="sxs-lookup"><span data-stu-id="558cd-109">Methods</span></span>
|<span data-ttu-id="558cd-110">方法</span><span class="sxs-lookup"><span data-stu-id="558cd-110">Method</span></span>|<span data-ttu-id="558cd-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="558cd-111">Return Type</span></span>|<span data-ttu-id="558cd-112">说明</span><span class="sxs-lookup"><span data-stu-id="558cd-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="558cd-113">列出 deviceManagementScripts</span><span class="sxs-lookup"><span data-stu-id="558cd-113">List deviceManagementScripts</span></span>](../api/intune-shared-devicemanagementscript-list.md)|<span data-ttu-id="558cd-114">[deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)集合</span><span class="sxs-lookup"><span data-stu-id="558cd-114">[deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) collection</span></span>|<span data-ttu-id="558cd-115">列出[deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="558cd-115">List properties and relationships of the [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) objects.</span></span>|
|[<span data-ttu-id="558cd-116">获取 deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="558cd-116">Get deviceManagementScript</span></span>](../api/intune-shared-devicemanagementscript-get.md)|[<span data-ttu-id="558cd-117">deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="558cd-117">deviceManagementScript</span></span>](../resources/intune-shared-devicemanagementscript.md)|<span data-ttu-id="558cd-118">读取[deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="558cd-118">Read properties and relationships of the [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) object.</span></span>|
|[<span data-ttu-id="558cd-119">创建 deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="558cd-119">Create deviceManagementScript</span></span>](../api/intune-shared-devicemanagementscript-create.md)|[<span data-ttu-id="558cd-120">deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="558cd-120">deviceManagementScript</span></span>](../resources/intune-shared-devicemanagementscript.md)|<span data-ttu-id="558cd-121">创建新的[deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)对象。</span><span class="sxs-lookup"><span data-stu-id="558cd-121">Create a new [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) object.</span></span>|
|[<span data-ttu-id="558cd-122">删除 deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="558cd-122">Delete deviceManagementScript</span></span>](../api/intune-shared-devicemanagementscript-delete.md)|<span data-ttu-id="558cd-123">无</span><span class="sxs-lookup"><span data-stu-id="558cd-123">None</span></span>|<span data-ttu-id="558cd-124">删除[deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)。</span><span class="sxs-lookup"><span data-stu-id="558cd-124">Deletes a [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md).</span></span>|
|[<span data-ttu-id="558cd-125">更新 deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="558cd-125">Update deviceManagementScript</span></span>](../api/intune-shared-devicemanagementscript-update.md)|[<span data-ttu-id="558cd-126">deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="558cd-126">deviceManagementScript</span></span>](../resources/intune-shared-devicemanagementscript.md)|<span data-ttu-id="558cd-127">更新[deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="558cd-127">Update the properties of a [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) object.</span></span>|
|<span data-ttu-id="558cd-128">**设备管理**</span><span class="sxs-lookup"><span data-stu-id="558cd-128">**Device management**</span></span>|
|[<span data-ttu-id="558cd-129">分配操作</span><span class="sxs-lookup"><span data-stu-id="558cd-129">assign action</span></span>](../api/intune-shared-devicemanagementscript-assign.md)|<span data-ttu-id="558cd-130">无</span><span class="sxs-lookup"><span data-stu-id="558cd-130">None</span></span>|<span data-ttu-id="558cd-131">尚未记录</span><span class="sxs-lookup"><span data-stu-id="558cd-131">Not yet documented</span></span>|
|<span data-ttu-id="558cd-132">**策略集**</span><span class="sxs-lookup"><span data-stu-id="558cd-132">**Policy Set**</span></span>|
|[<span data-ttu-id="558cd-133">hasPayloadLinks 操作</span><span class="sxs-lookup"><span data-stu-id="558cd-133">hasPayloadLinks action</span></span>](../api/intune-shared-devicemanagementscript-haspayloadlinks.md)|<span data-ttu-id="558cd-134">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="558cd-134">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) collection</span></span>|<span data-ttu-id="558cd-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="558cd-135">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="558cd-136">属性</span><span class="sxs-lookup"><span data-stu-id="558cd-136">Properties</span></span>
|<span data-ttu-id="558cd-137">属性</span><span class="sxs-lookup"><span data-stu-id="558cd-137">Property</span></span>|<span data-ttu-id="558cd-138">类型</span><span class="sxs-lookup"><span data-stu-id="558cd-138">Type</span></span>|<span data-ttu-id="558cd-139">说明</span><span class="sxs-lookup"><span data-stu-id="558cd-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="558cd-140">id</span><span class="sxs-lookup"><span data-stu-id="558cd-140">id</span></span>|<span data-ttu-id="558cd-141">字符串</span><span class="sxs-lookup"><span data-stu-id="558cd-141">String</span></span>|<span data-ttu-id="558cd-142">设备管理脚本的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="558cd-142">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="558cd-143">displayName</span><span class="sxs-lookup"><span data-stu-id="558cd-143">displayName</span></span>|<span data-ttu-id="558cd-144">字符串</span><span class="sxs-lookup"><span data-stu-id="558cd-144">String</span></span>|<span data-ttu-id="558cd-145">设备管理脚本的名称。</span><span class="sxs-lookup"><span data-stu-id="558cd-145">Name of the device management script.</span></span>|
|<span data-ttu-id="558cd-146">说明</span><span class="sxs-lookup"><span data-stu-id="558cd-146">description</span></span>|<span data-ttu-id="558cd-147">String</span><span class="sxs-lookup"><span data-stu-id="558cd-147">String</span></span>|<span data-ttu-id="558cd-148">设备管理脚本的可选说明。</span><span class="sxs-lookup"><span data-stu-id="558cd-148">Optional description for the device management script.</span></span>|
|<span data-ttu-id="558cd-149">runSchedule</span><span class="sxs-lookup"><span data-stu-id="558cd-149">runSchedule</span></span>|[<span data-ttu-id="558cd-150">runSchedule</span><span class="sxs-lookup"><span data-stu-id="558cd-150">runSchedule</span></span>](../resources/intune-devices-runschedule.md)|<span data-ttu-id="558cd-151">脚本运行的间隔。</span><span class="sxs-lookup"><span data-stu-id="558cd-151">The interval for script to run.</span></span> <span data-ttu-id="558cd-152">如果未定义，脚本将运行一次</span><span class="sxs-lookup"><span data-stu-id="558cd-152">If not defined the script will run once</span></span>|
|<span data-ttu-id="558cd-153">scriptContent</span><span class="sxs-lookup"><span data-stu-id="558cd-153">scriptContent</span></span>|<span data-ttu-id="558cd-154">Binary</span><span class="sxs-lookup"><span data-stu-id="558cd-154">Binary</span></span>|<span data-ttu-id="558cd-155">脚本内容。</span><span class="sxs-lookup"><span data-stu-id="558cd-155">The script content.</span></span>|
|<span data-ttu-id="558cd-156">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="558cd-156">createdDateTime</span></span>|<span data-ttu-id="558cd-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="558cd-157">DateTimeOffset</span></span>|<span data-ttu-id="558cd-158">设备管理脚本的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="558cd-158">The date and time the device management script was created.</span></span> <span data-ttu-id="558cd-159">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="558cd-159">This property is read-only.</span></span>|
|<span data-ttu-id="558cd-160">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="558cd-160">lastModifiedDateTime</span></span>|<span data-ttu-id="558cd-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="558cd-161">DateTimeOffset</span></span>|<span data-ttu-id="558cd-162">上次修改设备管理脚本的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="558cd-162">The date and time the device management script was last modified.</span></span> <span data-ttu-id="558cd-163">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="558cd-163">This property is read-only.</span></span>|
|<span data-ttu-id="558cd-164">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="558cd-164">runAsAccount</span></span>|[<span data-ttu-id="558cd-165">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="558cd-165">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="558cd-166">指示执行上下文的类型。</span><span class="sxs-lookup"><span data-stu-id="558cd-166">Indicates the type of execution context.</span></span> <span data-ttu-id="558cd-167">可取值为：`system`、`user`。</span><span class="sxs-lookup"><span data-stu-id="558cd-167">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="558cd-168">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="558cd-168">enforceSignatureCheck</span></span>|<span data-ttu-id="558cd-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="558cd-169">Boolean</span></span>|<span data-ttu-id="558cd-170">指示是否需要检查脚本签名。</span><span class="sxs-lookup"><span data-stu-id="558cd-170">Indicate whether the script signature needs be checked.</span></span>|
|<span data-ttu-id="558cd-171">fileName</span><span class="sxs-lookup"><span data-stu-id="558cd-171">fileName</span></span>|<span data-ttu-id="558cd-172">String</span><span class="sxs-lookup"><span data-stu-id="558cd-172">String</span></span>|<span data-ttu-id="558cd-173">脚本文件名。</span><span class="sxs-lookup"><span data-stu-id="558cd-173">Script file name.</span></span>|
|<span data-ttu-id="558cd-174">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="558cd-174">roleScopeTagIds</span></span>|<span data-ttu-id="558cd-175">String collection</span><span class="sxs-lookup"><span data-stu-id="558cd-175">String collection</span></span>|<span data-ttu-id="558cd-176">此 PowerShellScript 实例的范围标记 Id 的列表。</span><span class="sxs-lookup"><span data-stu-id="558cd-176">List of Scope Tag IDs for this PowerShellScript instance.</span></span>|
|<span data-ttu-id="558cd-177">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="558cd-177">runAs32Bit</span></span>|<span data-ttu-id="558cd-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="558cd-178">Boolean</span></span>|<span data-ttu-id="558cd-179">一个指示 PowerShell 脚本是否应作为32位运行的值</span><span class="sxs-lookup"><span data-stu-id="558cd-179">A value indicating whether the PowerShell script should run as 32-bit</span></span>|

## <a name="relationships"></a><span data-ttu-id="558cd-180">关系</span><span class="sxs-lookup"><span data-stu-id="558cd-180">Relationships</span></span>
|<span data-ttu-id="558cd-181">关系</span><span class="sxs-lookup"><span data-stu-id="558cd-181">Relationship</span></span>|<span data-ttu-id="558cd-182">类型</span><span class="sxs-lookup"><span data-stu-id="558cd-182">Type</span></span>|<span data-ttu-id="558cd-183">说明</span><span class="sxs-lookup"><span data-stu-id="558cd-183">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="558cd-184">**设备管理**</span><span class="sxs-lookup"><span data-stu-id="558cd-184">**Device management**</span></span>|
|<span data-ttu-id="558cd-185">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="558cd-185">groupAssignments</span></span>|<span data-ttu-id="558cd-186">deviceManagementScriptGroupAssignment 集合</span><span class="sxs-lookup"><span data-stu-id="558cd-186">deviceManagementScriptGroupAssignment collection</span></span>|<span data-ttu-id="558cd-187">设备管理脚本的组分配的列表。</span><span class="sxs-lookup"><span data-stu-id="558cd-187">The list of group assignments for the device management script.</span></span>|
|<span data-ttu-id="558cd-188">assignments</span><span class="sxs-lookup"><span data-stu-id="558cd-188">assignments</span></span>|<span data-ttu-id="558cd-189">deviceManagementScriptAssignment 集合</span><span class="sxs-lookup"><span data-stu-id="558cd-189">deviceManagementScriptAssignment collection</span></span>|<span data-ttu-id="558cd-190">设备管理脚本的组分配的列表。</span><span class="sxs-lookup"><span data-stu-id="558cd-190">The list of group assignments for the device management script.</span></span>|
|<span data-ttu-id="558cd-191">runSummary</span><span class="sxs-lookup"><span data-stu-id="558cd-191">runSummary</span></span>|<span data-ttu-id="558cd-192">deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="558cd-192">deviceManagementScriptRunSummary</span></span>|<span data-ttu-id="558cd-193">设备管理脚本的运行摘要。</span><span class="sxs-lookup"><span data-stu-id="558cd-193">Run summary for device management script.</span></span>|
|<span data-ttu-id="558cd-194">deviceRunStates</span><span class="sxs-lookup"><span data-stu-id="558cd-194">deviceRunStates</span></span>|<span data-ttu-id="558cd-195">deviceManagementScriptDeviceState 集合</span><span class="sxs-lookup"><span data-stu-id="558cd-195">deviceManagementScriptDeviceState collection</span></span>|<span data-ttu-id="558cd-196">此脚本在所有设备上的运行状态列表。</span><span class="sxs-lookup"><span data-stu-id="558cd-196">List of run states for this script across all devices.</span></span>|
|<span data-ttu-id="558cd-197">userRunStates</span><span class="sxs-lookup"><span data-stu-id="558cd-197">userRunStates</span></span>|<span data-ttu-id="558cd-198">deviceManagementScriptUserState 集合</span><span class="sxs-lookup"><span data-stu-id="558cd-198">deviceManagementScriptUserState collection</span></span>|<span data-ttu-id="558cd-199">此脚本在所有用户中的运行状态列表。</span><span class="sxs-lookup"><span data-stu-id="558cd-199">List of run states for this script across all users.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="558cd-200">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="558cd-200">JSON Representation</span></span>
<span data-ttu-id="558cd-201">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="558cd-201">Here is a JSON representation of the resource.</span></span>
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



