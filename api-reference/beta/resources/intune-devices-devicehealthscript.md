---
title: deviceHealthScript 资源类型
description: Intune 将向客户提供在已注册的 windows 10 Azure Active Directory 联接设备上运行其 Powershell 运行状况脚本（修正 + 检测）的功能。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 83d3f8e084b824baa40c41ace5045fd814e38592
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/09/2019
ms.locfileid: "38088103"
---
# <a name="devicehealthscript-resource-type"></a><span data-ttu-id="254dd-103">deviceHealthScript 资源类型</span><span class="sxs-lookup"><span data-stu-id="254dd-103">deviceHealthScript resource type</span></span>

> <span data-ttu-id="254dd-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="254dd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="254dd-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="254dd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="254dd-106">Intune 将向客户提供在已注册的 windows 10 Azure Active Directory 联接设备上运行其 Powershell 运行状况脚本（修正 + 检测）的功能。</span><span class="sxs-lookup"><span data-stu-id="254dd-106">Intune will provide customer the ability to run their Powershell Health scripts (remediation + detection) on the enrolled windows 10 Azure Active Directory joined devices.</span></span>

## <a name="methods"></a><span data-ttu-id="254dd-107">方法</span><span class="sxs-lookup"><span data-stu-id="254dd-107">Methods</span></span>
|<span data-ttu-id="254dd-108">方法</span><span class="sxs-lookup"><span data-stu-id="254dd-108">Method</span></span>|<span data-ttu-id="254dd-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="254dd-109">Return Type</span></span>|<span data-ttu-id="254dd-110">说明</span><span class="sxs-lookup"><span data-stu-id="254dd-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="254dd-111">列出 deviceHealthScripts</span><span class="sxs-lookup"><span data-stu-id="254dd-111">List deviceHealthScripts</span></span>](../api/intune-devices-devicehealthscript-list.md)|<span data-ttu-id="254dd-112">[deviceHealthScript](../resources/intune-devices-devicehealthscript.md)集合</span><span class="sxs-lookup"><span data-stu-id="254dd-112">[deviceHealthScript](../resources/intune-devices-devicehealthscript.md) collection</span></span>|<span data-ttu-id="254dd-113">列出[deviceHealthScript](../resources/intune-devices-devicehealthscript.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="254dd-113">List properties and relationships of the [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) objects.</span></span>|
|[<span data-ttu-id="254dd-114">获取 deviceHealthScript</span><span class="sxs-lookup"><span data-stu-id="254dd-114">Get deviceHealthScript</span></span>](../api/intune-devices-devicehealthscript-get.md)|[<span data-ttu-id="254dd-115">deviceHealthScript</span><span class="sxs-lookup"><span data-stu-id="254dd-115">deviceHealthScript</span></span>](../resources/intune-devices-devicehealthscript.md)|<span data-ttu-id="254dd-116">读取[deviceHealthScript](../resources/intune-devices-devicehealthscript.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="254dd-116">Read properties and relationships of the [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object.</span></span>|
|[<span data-ttu-id="254dd-117">创建 deviceHealthScript</span><span class="sxs-lookup"><span data-stu-id="254dd-117">Create deviceHealthScript</span></span>](../api/intune-devices-devicehealthscript-create.md)|[<span data-ttu-id="254dd-118">deviceHealthScript</span><span class="sxs-lookup"><span data-stu-id="254dd-118">deviceHealthScript</span></span>](../resources/intune-devices-devicehealthscript.md)|<span data-ttu-id="254dd-119">创建新的[deviceHealthScript](../resources/intune-devices-devicehealthscript.md)对象。</span><span class="sxs-lookup"><span data-stu-id="254dd-119">Create a new [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object.</span></span>|
|[<span data-ttu-id="254dd-120">删除 deviceHealthScript</span><span class="sxs-lookup"><span data-stu-id="254dd-120">Delete deviceHealthScript</span></span>](../api/intune-devices-devicehealthscript-delete.md)|<span data-ttu-id="254dd-121">无</span><span class="sxs-lookup"><span data-stu-id="254dd-121">None</span></span>|<span data-ttu-id="254dd-122">删除[deviceHealthScript](../resources/intune-devices-devicehealthscript.md)。</span><span class="sxs-lookup"><span data-stu-id="254dd-122">Deletes a [deviceHealthScript](../resources/intune-devices-devicehealthscript.md).</span></span>|
|[<span data-ttu-id="254dd-123">更新 deviceHealthScript</span><span class="sxs-lookup"><span data-stu-id="254dd-123">Update deviceHealthScript</span></span>](../api/intune-devices-devicehealthscript-update.md)|[<span data-ttu-id="254dd-124">deviceHealthScript</span><span class="sxs-lookup"><span data-stu-id="254dd-124">deviceHealthScript</span></span>](../resources/intune-devices-devicehealthscript.md)|<span data-ttu-id="254dd-125">更新[deviceHealthScript](../resources/intune-devices-devicehealthscript.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="254dd-125">Update the properties of a [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object.</span></span>|
|[<span data-ttu-id="254dd-126">分配操作</span><span class="sxs-lookup"><span data-stu-id="254dd-126">assign action</span></span>](../api/intune-devices-devicehealthscript-assign.md)|<span data-ttu-id="254dd-127">无</span><span class="sxs-lookup"><span data-stu-id="254dd-127">None</span></span>|<span data-ttu-id="254dd-128">尚未记录</span><span class="sxs-lookup"><span data-stu-id="254dd-128">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="254dd-129">属性</span><span class="sxs-lookup"><span data-stu-id="254dd-129">Properties</span></span>
|<span data-ttu-id="254dd-130">属性</span><span class="sxs-lookup"><span data-stu-id="254dd-130">Property</span></span>|<span data-ttu-id="254dd-131">类型</span><span class="sxs-lookup"><span data-stu-id="254dd-131">Type</span></span>|<span data-ttu-id="254dd-132">描述</span><span class="sxs-lookup"><span data-stu-id="254dd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="254dd-133">id</span><span class="sxs-lookup"><span data-stu-id="254dd-133">id</span></span>|<span data-ttu-id="254dd-134">字符串</span><span class="sxs-lookup"><span data-stu-id="254dd-134">String</span></span>|<span data-ttu-id="254dd-135">设备运行状况脚本的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="254dd-135">Unique Identifier for the device health script</span></span>|
|<span data-ttu-id="254dd-136">发布者</span><span class="sxs-lookup"><span data-stu-id="254dd-136">publisher</span></span>|<span data-ttu-id="254dd-137">String</span><span class="sxs-lookup"><span data-stu-id="254dd-137">String</span></span>|<span data-ttu-id="254dd-138">设备运行状况脚本发布者的名称</span><span class="sxs-lookup"><span data-stu-id="254dd-138">Name of the device health script publisher</span></span>|
|<span data-ttu-id="254dd-139">version</span><span class="sxs-lookup"><span data-stu-id="254dd-139">version</span></span>|<span data-ttu-id="254dd-140">String</span><span class="sxs-lookup"><span data-stu-id="254dd-140">String</span></span>|<span data-ttu-id="254dd-141">设备运行状况脚本的版本</span><span class="sxs-lookup"><span data-stu-id="254dd-141">Version of the device health script</span></span>|
|<span data-ttu-id="254dd-142">displayName</span><span class="sxs-lookup"><span data-stu-id="254dd-142">displayName</span></span>|<span data-ttu-id="254dd-143">字符串</span><span class="sxs-lookup"><span data-stu-id="254dd-143">String</span></span>|<span data-ttu-id="254dd-144">设备运行状况脚本的名称</span><span class="sxs-lookup"><span data-stu-id="254dd-144">Name of the device health script</span></span>|
|<span data-ttu-id="254dd-145">说明</span><span class="sxs-lookup"><span data-stu-id="254dd-145">description</span></span>|<span data-ttu-id="254dd-146">String</span><span class="sxs-lookup"><span data-stu-id="254dd-146">String</span></span>|<span data-ttu-id="254dd-147">设备运行状况脚本的说明</span><span class="sxs-lookup"><span data-stu-id="254dd-147">Description of the device health script</span></span>|
|<span data-ttu-id="254dd-148">detectionScriptContent</span><span class="sxs-lookup"><span data-stu-id="254dd-148">detectionScriptContent</span></span>|<span data-ttu-id="254dd-149">Binary</span><span class="sxs-lookup"><span data-stu-id="254dd-149">Binary</span></span>|<span data-ttu-id="254dd-150">检测 powershell 脚本的全部内容</span><span class="sxs-lookup"><span data-stu-id="254dd-150">The entire content of the detection powershell script</span></span>|
|<span data-ttu-id="254dd-151">remediationScriptContent</span><span class="sxs-lookup"><span data-stu-id="254dd-151">remediationScriptContent</span></span>|<span data-ttu-id="254dd-152">Binary</span><span class="sxs-lookup"><span data-stu-id="254dd-152">Binary</span></span>|<span data-ttu-id="254dd-153">修正 powershell 脚本的全部内容</span><span class="sxs-lookup"><span data-stu-id="254dd-153">The entire content of the remediation powershell script</span></span>|
|<span data-ttu-id="254dd-154">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="254dd-154">createdDateTime</span></span>|<span data-ttu-id="254dd-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="254dd-155">DateTimeOffset</span></span>|<span data-ttu-id="254dd-156">设备运行状况脚本的创建时间的时间戳。</span><span class="sxs-lookup"><span data-stu-id="254dd-156">The timestamp of when the device health script was created.</span></span> <span data-ttu-id="254dd-157">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="254dd-157">This property is read-only.</span></span>|
|<span data-ttu-id="254dd-158">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="254dd-158">lastModifiedDateTime</span></span>|<span data-ttu-id="254dd-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="254dd-159">DateTimeOffset</span></span>|<span data-ttu-id="254dd-160">修改设备运行状况脚本的时间戳。</span><span class="sxs-lookup"><span data-stu-id="254dd-160">The timestamp of when the device health script was modified.</span></span> <span data-ttu-id="254dd-161">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="254dd-161">This property is read-only.</span></span>|
|<span data-ttu-id="254dd-162">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="254dd-162">runAsAccount</span></span>|[<span data-ttu-id="254dd-163">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="254dd-163">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="254dd-164">指示执行上下文的类型。</span><span class="sxs-lookup"><span data-stu-id="254dd-164">Indicates the type of execution context.</span></span> <span data-ttu-id="254dd-165">可取值为：`system`、`user`。</span><span class="sxs-lookup"><span data-stu-id="254dd-165">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="254dd-166">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="254dd-166">enforceSignatureCheck</span></span>|<span data-ttu-id="254dd-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="254dd-167">Boolean</span></span>|<span data-ttu-id="254dd-168">指示是否需要检查脚本签名</span><span class="sxs-lookup"><span data-stu-id="254dd-168">Indicate whether the script signature needs be checked</span></span>|
|<span data-ttu-id="254dd-169">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="254dd-169">runAs32Bit</span></span>|<span data-ttu-id="254dd-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="254dd-170">Boolean</span></span>|<span data-ttu-id="254dd-171">指示 PowerShell 脚本是否应作为32位运行</span><span class="sxs-lookup"><span data-stu-id="254dd-171">Indicate whether PowerShell script(s) should run as 32-bit</span></span>|
|<span data-ttu-id="254dd-172">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="254dd-172">roleScopeTagIds</span></span>|<span data-ttu-id="254dd-173">String collection</span><span class="sxs-lookup"><span data-stu-id="254dd-173">String collection</span></span>|<span data-ttu-id="254dd-174">设备运行状况脚本的范围标记 Id 列表</span><span class="sxs-lookup"><span data-stu-id="254dd-174">List of Scope Tag IDs for the device health script</span></span>|

## <a name="relationships"></a><span data-ttu-id="254dd-175">关系</span><span class="sxs-lookup"><span data-stu-id="254dd-175">Relationships</span></span>
|<span data-ttu-id="254dd-176">关系</span><span class="sxs-lookup"><span data-stu-id="254dd-176">Relationship</span></span>|<span data-ttu-id="254dd-177">类型</span><span class="sxs-lookup"><span data-stu-id="254dd-177">Type</span></span>|<span data-ttu-id="254dd-178">描述</span><span class="sxs-lookup"><span data-stu-id="254dd-178">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="254dd-179">assignments</span><span class="sxs-lookup"><span data-stu-id="254dd-179">assignments</span></span>|<span data-ttu-id="254dd-180">[deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="254dd-180">[deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) collection</span></span>|<span data-ttu-id="254dd-181">设备运行状况脚本的组分配列表</span><span class="sxs-lookup"><span data-stu-id="254dd-181">The list of group assignments for the device health script</span></span>|
|<span data-ttu-id="254dd-182">runSummary</span><span class="sxs-lookup"><span data-stu-id="254dd-182">runSummary</span></span>|[<span data-ttu-id="254dd-183">deviceHealthScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="254dd-183">deviceHealthScriptRunSummary</span></span>](../resources/intune-devices-devicehealthscriptrunsummary.md)|<span data-ttu-id="254dd-184">设备运行状况脚本的高级别运行摘要。</span><span class="sxs-lookup"><span data-stu-id="254dd-184">High level run summary for device health script.</span></span>|
|<span data-ttu-id="254dd-185">deviceRunStates</span><span class="sxs-lookup"><span data-stu-id="254dd-185">deviceRunStates</span></span>|<span data-ttu-id="254dd-186">[deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md)集合</span><span class="sxs-lookup"><span data-stu-id="254dd-186">[deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) collection</span></span>|<span data-ttu-id="254dd-187">跨所有设备的设备运行状况脚本的运行状态列表</span><span class="sxs-lookup"><span data-stu-id="254dd-187">List of run states for the device health script across all devices</span></span>|

## <a name="json-representation"></a><span data-ttu-id="254dd-188">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="254dd-188">JSON Representation</span></span>
<span data-ttu-id="254dd-189">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="254dd-189">Here is a JSON representation of the resource.</span></span>
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
  ]
}
```



