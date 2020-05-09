---
title: deviceHealthScript 资源类型
description: Intune 将向客户提供在已注册的 windows 10 Azure Active Directory 联接设备上运行其 Powershell 运行状况脚本（修正 + 检测）的功能。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: baefb8e0b6975d1269a76a20aeb453972270cb46
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/09/2020
ms.locfileid: "44175635"
---
# <a name="devicehealthscript-resource-type"></a><span data-ttu-id="94934-103">deviceHealthScript 资源类型</span><span class="sxs-lookup"><span data-stu-id="94934-103">deviceHealthScript resource type</span></span>

<span data-ttu-id="94934-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="94934-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="94934-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="94934-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="94934-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="94934-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="94934-107">Intune 将向客户提供在已注册的 windows 10 Azure Active Directory 联接设备上运行其 Powershell 运行状况脚本（修正 + 检测）的功能。</span><span class="sxs-lookup"><span data-stu-id="94934-107">Intune will provide customer the ability to run their Powershell Health scripts (remediation + detection) on the enrolled windows 10 Azure Active Directory joined devices.</span></span>

## <a name="methods"></a><span data-ttu-id="94934-108">方法</span><span class="sxs-lookup"><span data-stu-id="94934-108">Methods</span></span>
|<span data-ttu-id="94934-109">方法</span><span class="sxs-lookup"><span data-stu-id="94934-109">Method</span></span>|<span data-ttu-id="94934-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="94934-110">Return Type</span></span>|<span data-ttu-id="94934-111">说明</span><span class="sxs-lookup"><span data-stu-id="94934-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="94934-112">列出 deviceHealthScripts</span><span class="sxs-lookup"><span data-stu-id="94934-112">List deviceHealthScripts</span></span>](../api/intune-devices-devicehealthscript-list.md)|<span data-ttu-id="94934-113">[deviceHealthScript](../resources/intune-devices-devicehealthscript.md)集合</span><span class="sxs-lookup"><span data-stu-id="94934-113">[deviceHealthScript](../resources/intune-devices-devicehealthscript.md) collection</span></span>|<span data-ttu-id="94934-114">列出[deviceHealthScript](../resources/intune-devices-devicehealthscript.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="94934-114">List properties and relationships of the [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) objects.</span></span>|
|[<span data-ttu-id="94934-115">获取 deviceHealthScript</span><span class="sxs-lookup"><span data-stu-id="94934-115">Get deviceHealthScript</span></span>](../api/intune-devices-devicehealthscript-get.md)|[<span data-ttu-id="94934-116">deviceHealthScript</span><span class="sxs-lookup"><span data-stu-id="94934-116">deviceHealthScript</span></span>](../resources/intune-devices-devicehealthscript.md)|<span data-ttu-id="94934-117">读取[deviceHealthScript](../resources/intune-devices-devicehealthscript.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="94934-117">Read properties and relationships of the [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object.</span></span>|
|[<span data-ttu-id="94934-118">创建 deviceHealthScript</span><span class="sxs-lookup"><span data-stu-id="94934-118">Create deviceHealthScript</span></span>](../api/intune-devices-devicehealthscript-create.md)|[<span data-ttu-id="94934-119">deviceHealthScript</span><span class="sxs-lookup"><span data-stu-id="94934-119">deviceHealthScript</span></span>](../resources/intune-devices-devicehealthscript.md)|<span data-ttu-id="94934-120">创建新的[deviceHealthScript](../resources/intune-devices-devicehealthscript.md)对象。</span><span class="sxs-lookup"><span data-stu-id="94934-120">Create a new [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object.</span></span>|
|[<span data-ttu-id="94934-121">删除 deviceHealthScript</span><span class="sxs-lookup"><span data-stu-id="94934-121">Delete deviceHealthScript</span></span>](../api/intune-devices-devicehealthscript-delete.md)|<span data-ttu-id="94934-122">无</span><span class="sxs-lookup"><span data-stu-id="94934-122">None</span></span>|<span data-ttu-id="94934-123">删除[deviceHealthScript](../resources/intune-devices-devicehealthscript.md)。</span><span class="sxs-lookup"><span data-stu-id="94934-123">Deletes a [deviceHealthScript](../resources/intune-devices-devicehealthscript.md).</span></span>|
|[<span data-ttu-id="94934-124">更新 deviceHealthScript</span><span class="sxs-lookup"><span data-stu-id="94934-124">Update deviceHealthScript</span></span>](../api/intune-devices-devicehealthscript-update.md)|[<span data-ttu-id="94934-125">deviceHealthScript</span><span class="sxs-lookup"><span data-stu-id="94934-125">deviceHealthScript</span></span>](../resources/intune-devices-devicehealthscript.md)|<span data-ttu-id="94934-126">更新[deviceHealthScript](../resources/intune-devices-devicehealthscript.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="94934-126">Update the properties of a [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object.</span></span>|
|[<span data-ttu-id="94934-127">分配操作</span><span class="sxs-lookup"><span data-stu-id="94934-127">assign action</span></span>](../api/intune-devices-devicehealthscript-assign.md)|<span data-ttu-id="94934-128">无</span><span class="sxs-lookup"><span data-stu-id="94934-128">None</span></span>|<span data-ttu-id="94934-129">尚未记录</span><span class="sxs-lookup"><span data-stu-id="94934-129">Not yet documented</span></span>|
|[<span data-ttu-id="94934-130">updateGlobalScript 操作</span><span class="sxs-lookup"><span data-stu-id="94934-130">updateGlobalScript action</span></span>](../api/intune-devices-devicehealthscript-updateglobalscript.md)|<span data-ttu-id="94934-131">字符串</span><span class="sxs-lookup"><span data-stu-id="94934-131">String</span></span>|<span data-ttu-id="94934-132">更新专用设备运行状况脚本</span><span class="sxs-lookup"><span data-stu-id="94934-132">Update the Proprietary Device Health Script</span></span>|
|[<span data-ttu-id="94934-133">getGlobalScriptHighestAvailableVersion 操作</span><span class="sxs-lookup"><span data-stu-id="94934-133">getGlobalScriptHighestAvailableVersion action</span></span>](../api/intune-devices-devicehealthscript-getglobalscripthighestavailableversion.md)|<span data-ttu-id="94934-134">字符串</span><span class="sxs-lookup"><span data-stu-id="94934-134">String</span></span>|<span data-ttu-id="94934-135">更新专用设备运行状况脚本</span><span class="sxs-lookup"><span data-stu-id="94934-135">Update the Proprietary Device Health Script</span></span>|
|[<span data-ttu-id="94934-136">enableGlobalScripts 操作</span><span class="sxs-lookup"><span data-stu-id="94934-136">enableGlobalScripts action</span></span>](../api/intune-devices-devicehealthscript-enableglobalscripts.md)|<span data-ttu-id="94934-137">无</span><span class="sxs-lookup"><span data-stu-id="94934-137">None</span></span>|<span data-ttu-id="94934-138">尚未记录</span><span class="sxs-lookup"><span data-stu-id="94934-138">Not yet documented</span></span>|
|[<span data-ttu-id="94934-139">areGlobalScriptsAvailable 函数</span><span class="sxs-lookup"><span data-stu-id="94934-139">areGlobalScriptsAvailable function</span></span>](../api/intune-devices-devicehealthscript-areglobalscriptsavailable.md)|[<span data-ttu-id="94934-140">globalDeviceHealthScriptState</span><span class="sxs-lookup"><span data-stu-id="94934-140">globalDeviceHealthScriptState</span></span>](../resources/intune-devices-globaldevicehealthscriptstate.md)|<span data-ttu-id="94934-141">尚未记录</span><span class="sxs-lookup"><span data-stu-id="94934-141">Not yet documented</span></span>|
|[<span data-ttu-id="94934-142">getRemediationSummary 函数</span><span class="sxs-lookup"><span data-stu-id="94934-142">getRemediationSummary function</span></span>](../api/intune-devices-devicehealthscript-getremediationsummary.md)|[<span data-ttu-id="94934-143">deviceHealthScriptRemediationSummary</span><span class="sxs-lookup"><span data-stu-id="94934-143">deviceHealthScriptRemediationSummary</span></span>](../resources/intune-devices-devicehealthscriptremediationsummary.md)|<span data-ttu-id="94934-144">尚未记录</span><span class="sxs-lookup"><span data-stu-id="94934-144">Not yet documented</span></span>|
|[<span data-ttu-id="94934-145">getRemediationHistory 函数</span><span class="sxs-lookup"><span data-stu-id="94934-145">getRemediationHistory function</span></span>](../api/intune-devices-devicehealthscript-getremediationhistory.md)|[<span data-ttu-id="94934-146">deviceHealthScriptRemediationHistory</span><span class="sxs-lookup"><span data-stu-id="94934-146">deviceHealthScriptRemediationHistory</span></span>](../resources/intune-devices-devicehealthscriptremediationhistory.md)|<span data-ttu-id="94934-147">用于获取设备运行状况脚本的 remediations 数的函数</span><span class="sxs-lookup"><span data-stu-id="94934-147">Function to get the number of remediations by a device health scripts</span></span>|

## <a name="properties"></a><span data-ttu-id="94934-148">属性</span><span class="sxs-lookup"><span data-stu-id="94934-148">Properties</span></span>
|<span data-ttu-id="94934-149">属性</span><span class="sxs-lookup"><span data-stu-id="94934-149">Property</span></span>|<span data-ttu-id="94934-150">类型</span><span class="sxs-lookup"><span data-stu-id="94934-150">Type</span></span>|<span data-ttu-id="94934-151">说明</span><span class="sxs-lookup"><span data-stu-id="94934-151">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94934-152">id</span><span class="sxs-lookup"><span data-stu-id="94934-152">id</span></span>|<span data-ttu-id="94934-153">字符串</span><span class="sxs-lookup"><span data-stu-id="94934-153">String</span></span>|<span data-ttu-id="94934-154">设备运行状况脚本的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="94934-154">Unique Identifier for the device health script</span></span>|
|<span data-ttu-id="94934-155">发布者</span><span class="sxs-lookup"><span data-stu-id="94934-155">publisher</span></span>|<span data-ttu-id="94934-156">字符串</span><span class="sxs-lookup"><span data-stu-id="94934-156">String</span></span>|<span data-ttu-id="94934-157">设备运行状况脚本发布者的名称</span><span class="sxs-lookup"><span data-stu-id="94934-157">Name of the device health script publisher</span></span>|
|<span data-ttu-id="94934-158">version</span><span class="sxs-lookup"><span data-stu-id="94934-158">version</span></span>|<span data-ttu-id="94934-159">String</span><span class="sxs-lookup"><span data-stu-id="94934-159">String</span></span>|<span data-ttu-id="94934-160">设备运行状况脚本的版本</span><span class="sxs-lookup"><span data-stu-id="94934-160">Version of the device health script</span></span>|
|<span data-ttu-id="94934-161">displayName</span><span class="sxs-lookup"><span data-stu-id="94934-161">displayName</span></span>|<span data-ttu-id="94934-162">字符串</span><span class="sxs-lookup"><span data-stu-id="94934-162">String</span></span>|<span data-ttu-id="94934-163">设备运行状况脚本的名称</span><span class="sxs-lookup"><span data-stu-id="94934-163">Name of the device health script</span></span>|
|<span data-ttu-id="94934-164">说明</span><span class="sxs-lookup"><span data-stu-id="94934-164">description</span></span>|<span data-ttu-id="94934-165">String</span><span class="sxs-lookup"><span data-stu-id="94934-165">String</span></span>|<span data-ttu-id="94934-166">设备运行状况脚本的说明</span><span class="sxs-lookup"><span data-stu-id="94934-166">Description of the device health script</span></span>|
|<span data-ttu-id="94934-167">detectionScriptContent</span><span class="sxs-lookup"><span data-stu-id="94934-167">detectionScriptContent</span></span>|<span data-ttu-id="94934-168">Binary</span><span class="sxs-lookup"><span data-stu-id="94934-168">Binary</span></span>|<span data-ttu-id="94934-169">检测 powershell 脚本的全部内容</span><span class="sxs-lookup"><span data-stu-id="94934-169">The entire content of the detection powershell script</span></span>|
|<span data-ttu-id="94934-170">remediationScriptContent</span><span class="sxs-lookup"><span data-stu-id="94934-170">remediationScriptContent</span></span>|<span data-ttu-id="94934-171">Binary</span><span class="sxs-lookup"><span data-stu-id="94934-171">Binary</span></span>|<span data-ttu-id="94934-172">修正 powershell 脚本的全部内容</span><span class="sxs-lookup"><span data-stu-id="94934-172">The entire content of the remediation powershell script</span></span>|
|<span data-ttu-id="94934-173">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="94934-173">createdDateTime</span></span>|<span data-ttu-id="94934-174">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="94934-174">DateTimeOffset</span></span>|<span data-ttu-id="94934-175">设备运行状况脚本的创建时间的时间戳。</span><span class="sxs-lookup"><span data-stu-id="94934-175">The timestamp of when the device health script was created.</span></span> <span data-ttu-id="94934-176">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="94934-176">This property is read-only.</span></span>|
|<span data-ttu-id="94934-177">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="94934-177">lastModifiedDateTime</span></span>|<span data-ttu-id="94934-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="94934-178">DateTimeOffset</span></span>|<span data-ttu-id="94934-179">修改设备运行状况脚本的时间戳。</span><span class="sxs-lookup"><span data-stu-id="94934-179">The timestamp of when the device health script was modified.</span></span> <span data-ttu-id="94934-180">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="94934-180">This property is read-only.</span></span>|
|<span data-ttu-id="94934-181">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="94934-181">runAsAccount</span></span>|[<span data-ttu-id="94934-182">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="94934-182">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="94934-183">指示执行上下文的类型。</span><span class="sxs-lookup"><span data-stu-id="94934-183">Indicates the type of execution context.</span></span> <span data-ttu-id="94934-184">可取值为：`system`、`user`。</span><span class="sxs-lookup"><span data-stu-id="94934-184">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="94934-185">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="94934-185">enforceSignatureCheck</span></span>|<span data-ttu-id="94934-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="94934-186">Boolean</span></span>|<span data-ttu-id="94934-187">指示是否需要检查脚本签名</span><span class="sxs-lookup"><span data-stu-id="94934-187">Indicate whether the script signature needs be checked</span></span>|
|<span data-ttu-id="94934-188">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="94934-188">runAs32Bit</span></span>|<span data-ttu-id="94934-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="94934-189">Boolean</span></span>|<span data-ttu-id="94934-190">指示 PowerShell 脚本是否应作为32位运行</span><span class="sxs-lookup"><span data-stu-id="94934-190">Indicate whether PowerShell script(s) should run as 32-bit</span></span>|
|<span data-ttu-id="94934-191">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="94934-191">roleScopeTagIds</span></span>|<span data-ttu-id="94934-192">字符串集合</span><span class="sxs-lookup"><span data-stu-id="94934-192">String collection</span></span>|<span data-ttu-id="94934-193">设备运行状况脚本的范围标记 Id 列表</span><span class="sxs-lookup"><span data-stu-id="94934-193">List of Scope Tag IDs for the device health script</span></span>|
|<span data-ttu-id="94934-194">isGlobalScript</span><span class="sxs-lookup"><span data-stu-id="94934-194">isGlobalScript</span></span>|<span data-ttu-id="94934-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="94934-195">Boolean</span></span>|<span data-ttu-id="94934-196">确定这是否为 Microsoft 专用脚本。</span><span class="sxs-lookup"><span data-stu-id="94934-196">Determines if this is Microsoft Proprietary Script.</span></span> <span data-ttu-id="94934-197">专用脚本为只读</span><span class="sxs-lookup"><span data-stu-id="94934-197">Proprietary scripts are read-only</span></span>|
|<span data-ttu-id="94934-198">highestAvailableVersion</span><span class="sxs-lookup"><span data-stu-id="94934-198">highestAvailableVersion</span></span>|<span data-ttu-id="94934-199">字符串</span><span class="sxs-lookup"><span data-stu-id="94934-199">String</span></span>|<span data-ttu-id="94934-200">Microsoft 专用脚本的最高可用版本</span><span class="sxs-lookup"><span data-stu-id="94934-200">Highest available version for a Microsoft Proprietary script</span></span>|
|<span data-ttu-id="94934-201">detectionScriptParameters</span><span class="sxs-lookup"><span data-stu-id="94934-201">detectionScriptParameters</span></span>|<span data-ttu-id="94934-202">[deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)集合</span><span class="sxs-lookup"><span data-stu-id="94934-202">[deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md) collection</span></span>|<span data-ttu-id="94934-203">复杂类型 DetectionScriptParameters 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="94934-203">List of ComplexType DetectionScriptParameters objects.</span></span>|
|<span data-ttu-id="94934-204">remediationScriptParameters</span><span class="sxs-lookup"><span data-stu-id="94934-204">remediationScriptParameters</span></span>|<span data-ttu-id="94934-205">[deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)集合</span><span class="sxs-lookup"><span data-stu-id="94934-205">[deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md) collection</span></span>|<span data-ttu-id="94934-206">复杂类型 RemediationScriptParameters 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="94934-206">List of ComplexType RemediationScriptParameters objects.</span></span>|

## <a name="relationships"></a><span data-ttu-id="94934-207">关系</span><span class="sxs-lookup"><span data-stu-id="94934-207">Relationships</span></span>
|<span data-ttu-id="94934-208">关系</span><span class="sxs-lookup"><span data-stu-id="94934-208">Relationship</span></span>|<span data-ttu-id="94934-209">类型</span><span class="sxs-lookup"><span data-stu-id="94934-209">Type</span></span>|<span data-ttu-id="94934-210">说明</span><span class="sxs-lookup"><span data-stu-id="94934-210">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94934-211">assignments</span><span class="sxs-lookup"><span data-stu-id="94934-211">assignments</span></span>|<span data-ttu-id="94934-212">[deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="94934-212">[deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) collection</span></span>|<span data-ttu-id="94934-213">设备运行状况脚本的组分配列表</span><span class="sxs-lookup"><span data-stu-id="94934-213">The list of group assignments for the device health script</span></span>|
|<span data-ttu-id="94934-214">runSummary</span><span class="sxs-lookup"><span data-stu-id="94934-214">runSummary</span></span>|[<span data-ttu-id="94934-215">deviceHealthScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="94934-215">deviceHealthScriptRunSummary</span></span>](../resources/intune-devices-devicehealthscriptrunsummary.md)|<span data-ttu-id="94934-216">设备运行状况脚本的高级别运行摘要。</span><span class="sxs-lookup"><span data-stu-id="94934-216">High level run summary for device health script.</span></span>|
|<span data-ttu-id="94934-217">deviceRunStates</span><span class="sxs-lookup"><span data-stu-id="94934-217">deviceRunStates</span></span>|<span data-ttu-id="94934-218">[deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md)集合</span><span class="sxs-lookup"><span data-stu-id="94934-218">[deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) collection</span></span>|<span data-ttu-id="94934-219">跨所有设备的设备运行状况脚本的运行状态列表</span><span class="sxs-lookup"><span data-stu-id="94934-219">List of run states for the device health script across all devices</span></span>|

## <a name="json-representation"></a><span data-ttu-id="94934-220">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="94934-220">JSON Representation</span></span>
<span data-ttu-id="94934-221">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="94934-221">Here is a JSON representation of the resource.</span></span>
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
  "highestAvailableVersion": "String",
  "detectionScriptParameters": [
    {
      "@odata.type": "microsoft.graph.deviceHealthScriptStringParameter",
      "name": "String",
      "description": "String",
      "isRequired": true,
      "applyDefaultValueWhenNotAssigned": true,
      "defaultValue": "String"
    }
  ],
  "remediationScriptParameters": [
    {
      "@odata.type": "microsoft.graph.deviceHealthScriptStringParameter",
      "name": "String",
      "description": "String",
      "isRequired": true,
      "applyDefaultValueWhenNotAssigned": true,
      "defaultValue": "String"
    }
  ]
}
```



