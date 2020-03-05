---
title: deviceHealthScript 资源类型
description: Intune 将向客户提供在已注册的 windows 10 Azure Active Directory 联接设备上运行其 Powershell 运行状况脚本（修正 + 检测）的功能。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0579008f0994aba06de3bc5869af998a80cab683
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525087"
---
# <a name="devicehealthscript-resource-type"></a><span data-ttu-id="dabd5-103">deviceHealthScript 资源类型</span><span class="sxs-lookup"><span data-stu-id="dabd5-103">deviceHealthScript resource type</span></span>

<span data-ttu-id="dabd5-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="dabd5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dabd5-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="dabd5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dabd5-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="dabd5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dabd5-107">Intune 将向客户提供在已注册的 windows 10 Azure Active Directory 联接设备上运行其 Powershell 运行状况脚本（修正 + 检测）的功能。</span><span class="sxs-lookup"><span data-stu-id="dabd5-107">Intune will provide customer the ability to run their Powershell Health scripts (remediation + detection) on the enrolled windows 10 Azure Active Directory joined devices.</span></span>

## <a name="methods"></a><span data-ttu-id="dabd5-108">方法</span><span class="sxs-lookup"><span data-stu-id="dabd5-108">Methods</span></span>
|<span data-ttu-id="dabd5-109">方法</span><span class="sxs-lookup"><span data-stu-id="dabd5-109">Method</span></span>|<span data-ttu-id="dabd5-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="dabd5-110">Return Type</span></span>|<span data-ttu-id="dabd5-111">说明</span><span class="sxs-lookup"><span data-stu-id="dabd5-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="dabd5-112">列出 deviceHealthScripts</span><span class="sxs-lookup"><span data-stu-id="dabd5-112">List deviceHealthScripts</span></span>](../api/intune-devices-devicehealthscript-list.md)|<span data-ttu-id="dabd5-113">[deviceHealthScript](../resources/intune-devices-devicehealthscript.md)集合</span><span class="sxs-lookup"><span data-stu-id="dabd5-113">[deviceHealthScript](../resources/intune-devices-devicehealthscript.md) collection</span></span>|<span data-ttu-id="dabd5-114">列出[deviceHealthScript](../resources/intune-devices-devicehealthscript.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="dabd5-114">List properties and relationships of the [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) objects.</span></span>|
|[<span data-ttu-id="dabd5-115">获取 deviceHealthScript</span><span class="sxs-lookup"><span data-stu-id="dabd5-115">Get deviceHealthScript</span></span>](../api/intune-devices-devicehealthscript-get.md)|[<span data-ttu-id="dabd5-116">deviceHealthScript</span><span class="sxs-lookup"><span data-stu-id="dabd5-116">deviceHealthScript</span></span>](../resources/intune-devices-devicehealthscript.md)|<span data-ttu-id="dabd5-117">读取[deviceHealthScript](../resources/intune-devices-devicehealthscript.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="dabd5-117">Read properties and relationships of the [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object.</span></span>|
|[<span data-ttu-id="dabd5-118">创建 deviceHealthScript</span><span class="sxs-lookup"><span data-stu-id="dabd5-118">Create deviceHealthScript</span></span>](../api/intune-devices-devicehealthscript-create.md)|[<span data-ttu-id="dabd5-119">deviceHealthScript</span><span class="sxs-lookup"><span data-stu-id="dabd5-119">deviceHealthScript</span></span>](../resources/intune-devices-devicehealthscript.md)|<span data-ttu-id="dabd5-120">创建新的[deviceHealthScript](../resources/intune-devices-devicehealthscript.md)对象。</span><span class="sxs-lookup"><span data-stu-id="dabd5-120">Create a new [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object.</span></span>|
|[<span data-ttu-id="dabd5-121">删除 deviceHealthScript</span><span class="sxs-lookup"><span data-stu-id="dabd5-121">Delete deviceHealthScript</span></span>](../api/intune-devices-devicehealthscript-delete.md)|<span data-ttu-id="dabd5-122">无</span><span class="sxs-lookup"><span data-stu-id="dabd5-122">None</span></span>|<span data-ttu-id="dabd5-123">删除[deviceHealthScript](../resources/intune-devices-devicehealthscript.md)。</span><span class="sxs-lookup"><span data-stu-id="dabd5-123">Deletes a [deviceHealthScript](../resources/intune-devices-devicehealthscript.md).</span></span>|
|[<span data-ttu-id="dabd5-124">更新 deviceHealthScript</span><span class="sxs-lookup"><span data-stu-id="dabd5-124">Update deviceHealthScript</span></span>](../api/intune-devices-devicehealthscript-update.md)|[<span data-ttu-id="dabd5-125">deviceHealthScript</span><span class="sxs-lookup"><span data-stu-id="dabd5-125">deviceHealthScript</span></span>](../resources/intune-devices-devicehealthscript.md)|<span data-ttu-id="dabd5-126">更新[deviceHealthScript](../resources/intune-devices-devicehealthscript.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="dabd5-126">Update the properties of a [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object.</span></span>|
|[<span data-ttu-id="dabd5-127">分配操作</span><span class="sxs-lookup"><span data-stu-id="dabd5-127">assign action</span></span>](../api/intune-devices-devicehealthscript-assign.md)|<span data-ttu-id="dabd5-128">无</span><span class="sxs-lookup"><span data-stu-id="dabd5-128">None</span></span>|<span data-ttu-id="dabd5-129">尚未记录</span><span class="sxs-lookup"><span data-stu-id="dabd5-129">Not yet documented</span></span>|
|[<span data-ttu-id="dabd5-130">updateGlobalScript 操作</span><span class="sxs-lookup"><span data-stu-id="dabd5-130">updateGlobalScript action</span></span>](../api/intune-devices-devicehealthscript-updateglobalscript.md)|<span data-ttu-id="dabd5-131">String</span><span class="sxs-lookup"><span data-stu-id="dabd5-131">String</span></span>|<span data-ttu-id="dabd5-132">更新专用设备运行状况脚本</span><span class="sxs-lookup"><span data-stu-id="dabd5-132">Update the Proprietary Device Health Script</span></span>|
|[<span data-ttu-id="dabd5-133">getGlobalScriptHighestAvailableVersion 操作</span><span class="sxs-lookup"><span data-stu-id="dabd5-133">getGlobalScriptHighestAvailableVersion action</span></span>](../api/intune-devices-devicehealthscript-getglobalscripthighestavailableversion.md)|<span data-ttu-id="dabd5-134">String</span><span class="sxs-lookup"><span data-stu-id="dabd5-134">String</span></span>|<span data-ttu-id="dabd5-135">更新专用设备运行状况脚本</span><span class="sxs-lookup"><span data-stu-id="dabd5-135">Update the Proprietary Device Health Script</span></span>|
|[<span data-ttu-id="dabd5-136">enableGlobalScripts 操作</span><span class="sxs-lookup"><span data-stu-id="dabd5-136">enableGlobalScripts action</span></span>](../api/intune-devices-devicehealthscript-enableglobalscripts.md)|<span data-ttu-id="dabd5-137">无</span><span class="sxs-lookup"><span data-stu-id="dabd5-137">None</span></span>|<span data-ttu-id="dabd5-138">尚未记录</span><span class="sxs-lookup"><span data-stu-id="dabd5-138">Not yet documented</span></span>|
|[<span data-ttu-id="dabd5-139">areGlobalScriptsAvailable 函数</span><span class="sxs-lookup"><span data-stu-id="dabd5-139">areGlobalScriptsAvailable function</span></span>](../api/intune-devices-devicehealthscript-areglobalscriptsavailable.md)|[<span data-ttu-id="dabd5-140">globalDeviceHealthScriptState</span><span class="sxs-lookup"><span data-stu-id="dabd5-140">globalDeviceHealthScriptState</span></span>](../resources/intune-devices-globaldevicehealthscriptstate.md)|<span data-ttu-id="dabd5-141">尚未记录</span><span class="sxs-lookup"><span data-stu-id="dabd5-141">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="dabd5-142">属性</span><span class="sxs-lookup"><span data-stu-id="dabd5-142">Properties</span></span>
|<span data-ttu-id="dabd5-143">属性</span><span class="sxs-lookup"><span data-stu-id="dabd5-143">Property</span></span>|<span data-ttu-id="dabd5-144">类型</span><span class="sxs-lookup"><span data-stu-id="dabd5-144">Type</span></span>|<span data-ttu-id="dabd5-145">说明</span><span class="sxs-lookup"><span data-stu-id="dabd5-145">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dabd5-146">id</span><span class="sxs-lookup"><span data-stu-id="dabd5-146">id</span></span>|<span data-ttu-id="dabd5-147">字符串</span><span class="sxs-lookup"><span data-stu-id="dabd5-147">String</span></span>|<span data-ttu-id="dabd5-148">设备运行状况脚本的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="dabd5-148">Unique Identifier for the device health script</span></span>|
|<span data-ttu-id="dabd5-149">发布者</span><span class="sxs-lookup"><span data-stu-id="dabd5-149">publisher</span></span>|<span data-ttu-id="dabd5-150">String</span><span class="sxs-lookup"><span data-stu-id="dabd5-150">String</span></span>|<span data-ttu-id="dabd5-151">设备运行状况脚本发布者的名称</span><span class="sxs-lookup"><span data-stu-id="dabd5-151">Name of the device health script publisher</span></span>|
|<span data-ttu-id="dabd5-152">version</span><span class="sxs-lookup"><span data-stu-id="dabd5-152">version</span></span>|<span data-ttu-id="dabd5-153">String</span><span class="sxs-lookup"><span data-stu-id="dabd5-153">String</span></span>|<span data-ttu-id="dabd5-154">设备运行状况脚本的版本</span><span class="sxs-lookup"><span data-stu-id="dabd5-154">Version of the device health script</span></span>|
|<span data-ttu-id="dabd5-155">displayName</span><span class="sxs-lookup"><span data-stu-id="dabd5-155">displayName</span></span>|<span data-ttu-id="dabd5-156">字符串</span><span class="sxs-lookup"><span data-stu-id="dabd5-156">String</span></span>|<span data-ttu-id="dabd5-157">设备运行状况脚本的名称</span><span class="sxs-lookup"><span data-stu-id="dabd5-157">Name of the device health script</span></span>|
|<span data-ttu-id="dabd5-158">说明</span><span class="sxs-lookup"><span data-stu-id="dabd5-158">description</span></span>|<span data-ttu-id="dabd5-159">String</span><span class="sxs-lookup"><span data-stu-id="dabd5-159">String</span></span>|<span data-ttu-id="dabd5-160">设备运行状况脚本的说明</span><span class="sxs-lookup"><span data-stu-id="dabd5-160">Description of the device health script</span></span>|
|<span data-ttu-id="dabd5-161">detectionScriptContent</span><span class="sxs-lookup"><span data-stu-id="dabd5-161">detectionScriptContent</span></span>|<span data-ttu-id="dabd5-162">Binary</span><span class="sxs-lookup"><span data-stu-id="dabd5-162">Binary</span></span>|<span data-ttu-id="dabd5-163">检测 powershell 脚本的全部内容</span><span class="sxs-lookup"><span data-stu-id="dabd5-163">The entire content of the detection powershell script</span></span>|
|<span data-ttu-id="dabd5-164">remediationScriptContent</span><span class="sxs-lookup"><span data-stu-id="dabd5-164">remediationScriptContent</span></span>|<span data-ttu-id="dabd5-165">Binary</span><span class="sxs-lookup"><span data-stu-id="dabd5-165">Binary</span></span>|<span data-ttu-id="dabd5-166">修正 powershell 脚本的全部内容</span><span class="sxs-lookup"><span data-stu-id="dabd5-166">The entire content of the remediation powershell script</span></span>|
|<span data-ttu-id="dabd5-167">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dabd5-167">createdDateTime</span></span>|<span data-ttu-id="dabd5-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dabd5-168">DateTimeOffset</span></span>|<span data-ttu-id="dabd5-169">设备运行状况脚本的创建时间的时间戳。</span><span class="sxs-lookup"><span data-stu-id="dabd5-169">The timestamp of when the device health script was created.</span></span> <span data-ttu-id="dabd5-170">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="dabd5-170">This property is read-only.</span></span>|
|<span data-ttu-id="dabd5-171">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dabd5-171">lastModifiedDateTime</span></span>|<span data-ttu-id="dabd5-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dabd5-172">DateTimeOffset</span></span>|<span data-ttu-id="dabd5-173">修改设备运行状况脚本的时间戳。</span><span class="sxs-lookup"><span data-stu-id="dabd5-173">The timestamp of when the device health script was modified.</span></span> <span data-ttu-id="dabd5-174">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="dabd5-174">This property is read-only.</span></span>|
|<span data-ttu-id="dabd5-175">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="dabd5-175">runAsAccount</span></span>|[<span data-ttu-id="dabd5-176">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="dabd5-176">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="dabd5-177">指示执行上下文的类型。</span><span class="sxs-lookup"><span data-stu-id="dabd5-177">Indicates the type of execution context.</span></span> <span data-ttu-id="dabd5-178">可取值为：`system`、`user`。</span><span class="sxs-lookup"><span data-stu-id="dabd5-178">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="dabd5-179">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="dabd5-179">enforceSignatureCheck</span></span>|<span data-ttu-id="dabd5-180">布尔</span><span class="sxs-lookup"><span data-stu-id="dabd5-180">Boolean</span></span>|<span data-ttu-id="dabd5-181">指示是否需要检查脚本签名</span><span class="sxs-lookup"><span data-stu-id="dabd5-181">Indicate whether the script signature needs be checked</span></span>|
|<span data-ttu-id="dabd5-182">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="dabd5-182">runAs32Bit</span></span>|<span data-ttu-id="dabd5-183">布尔</span><span class="sxs-lookup"><span data-stu-id="dabd5-183">Boolean</span></span>|<span data-ttu-id="dabd5-184">指示 PowerShell 脚本是否应作为32位运行</span><span class="sxs-lookup"><span data-stu-id="dabd5-184">Indicate whether PowerShell script(s) should run as 32-bit</span></span>|
|<span data-ttu-id="dabd5-185">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="dabd5-185">roleScopeTagIds</span></span>|<span data-ttu-id="dabd5-186">String 集合</span><span class="sxs-lookup"><span data-stu-id="dabd5-186">String collection</span></span>|<span data-ttu-id="dabd5-187">设备运行状况脚本的范围标记 Id 列表</span><span class="sxs-lookup"><span data-stu-id="dabd5-187">List of Scope Tag IDs for the device health script</span></span>|
|<span data-ttu-id="dabd5-188">isGlobalScript</span><span class="sxs-lookup"><span data-stu-id="dabd5-188">isGlobalScript</span></span>|<span data-ttu-id="dabd5-189">布尔</span><span class="sxs-lookup"><span data-stu-id="dabd5-189">Boolean</span></span>|<span data-ttu-id="dabd5-190">确定这是否为 Microsoft 专用脚本。</span><span class="sxs-lookup"><span data-stu-id="dabd5-190">Determines if this is Microsoft Proprietary Script.</span></span> <span data-ttu-id="dabd5-191">专用脚本为只读</span><span class="sxs-lookup"><span data-stu-id="dabd5-191">Proprietary scripts are read-only</span></span>|
|<span data-ttu-id="dabd5-192">highestAvailableVersion</span><span class="sxs-lookup"><span data-stu-id="dabd5-192">highestAvailableVersion</span></span>|<span data-ttu-id="dabd5-193">String</span><span class="sxs-lookup"><span data-stu-id="dabd5-193">String</span></span>|<span data-ttu-id="dabd5-194">Microsoft 专用脚本的最高可用版本</span><span class="sxs-lookup"><span data-stu-id="dabd5-194">Highest available version for a Microsoft Proprietary script</span></span>|

## <a name="relationships"></a><span data-ttu-id="dabd5-195">关系</span><span class="sxs-lookup"><span data-stu-id="dabd5-195">Relationships</span></span>
|<span data-ttu-id="dabd5-196">关系</span><span class="sxs-lookup"><span data-stu-id="dabd5-196">Relationship</span></span>|<span data-ttu-id="dabd5-197">类型</span><span class="sxs-lookup"><span data-stu-id="dabd5-197">Type</span></span>|<span data-ttu-id="dabd5-198">说明</span><span class="sxs-lookup"><span data-stu-id="dabd5-198">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dabd5-199">assignments</span><span class="sxs-lookup"><span data-stu-id="dabd5-199">assignments</span></span>|<span data-ttu-id="dabd5-200">[deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="dabd5-200">[deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) collection</span></span>|<span data-ttu-id="dabd5-201">设备运行状况脚本的组分配列表</span><span class="sxs-lookup"><span data-stu-id="dabd5-201">The list of group assignments for the device health script</span></span>|
|<span data-ttu-id="dabd5-202">runSummary</span><span class="sxs-lookup"><span data-stu-id="dabd5-202">runSummary</span></span>|[<span data-ttu-id="dabd5-203">deviceHealthScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="dabd5-203">deviceHealthScriptRunSummary</span></span>](../resources/intune-devices-devicehealthscriptrunsummary.md)|<span data-ttu-id="dabd5-204">设备运行状况脚本的高级别运行摘要。</span><span class="sxs-lookup"><span data-stu-id="dabd5-204">High level run summary for device health script.</span></span>|
|<span data-ttu-id="dabd5-205">deviceRunStates</span><span class="sxs-lookup"><span data-stu-id="dabd5-205">deviceRunStates</span></span>|<span data-ttu-id="dabd5-206">[deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md)集合</span><span class="sxs-lookup"><span data-stu-id="dabd5-206">[deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) collection</span></span>|<span data-ttu-id="dabd5-207">跨所有设备的设备运行状况脚本的运行状态列表</span><span class="sxs-lookup"><span data-stu-id="dabd5-207">List of run states for the device health script across all devices</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dabd5-208">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dabd5-208">JSON Representation</span></span>
<span data-ttu-id="dabd5-209">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dabd5-209">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceHealthScript"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScript",
  "id": "String (identifier)",
  "publisher": "String",
  "version": "String",
  "displayName": "String",
  "description": "String",
  "detectionScriptContent": "binary",
  "remediationScriptContent": "binary",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "runAsAccount": "String",
  "enforceSignatureCheck": true,
  "runAs32Bit": true,
  "roleScopeTagIds": [
    "String"
  ],
  "isGlobalScript": true,
  "highestAvailableVersion": "String"
}
```



