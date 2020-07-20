---
title: deviceComplianceScript 资源类型
description: Intune 将向客户提供在已注册的 windows 10 Azure Active Directory 联接设备上运行其 Powershell 合规性脚本（检测）的功能。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: aba8998ff1615741e481924a6602dc10f0171371
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: Auto
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44789372"
---
# <a name="devicecompliancescript-resource-type"></a><span data-ttu-id="23861-103">deviceComplianceScript 资源类型</span><span class="sxs-lookup"><span data-stu-id="23861-103">deviceComplianceScript resource type</span></span>

<span data-ttu-id="23861-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23861-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="23861-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="23861-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="23861-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="23861-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="23861-107">Intune 将向客户提供在已注册的 windows 10 Azure Active Directory 联接设备上运行其 Powershell 合规性脚本（检测）的功能。</span><span class="sxs-lookup"><span data-stu-id="23861-107">Intune will provide customer the ability to run their Powershell Compliance scripts (detection) on the enrolled windows 10 Azure Active Directory joined devices.</span></span>

## <a name="methods"></a><span data-ttu-id="23861-108">Methods</span><span class="sxs-lookup"><span data-stu-id="23861-108">Methods</span></span>
|<span data-ttu-id="23861-109">方法</span><span class="sxs-lookup"><span data-stu-id="23861-109">Method</span></span>|<span data-ttu-id="23861-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="23861-110">Return Type</span></span>|<span data-ttu-id="23861-111">说明</span><span class="sxs-lookup"><span data-stu-id="23861-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="23861-112">列出 deviceComplianceScripts</span><span class="sxs-lookup"><span data-stu-id="23861-112">List deviceComplianceScripts</span></span>](../api/intune-devices-devicecompliancescript-list.md)|<span data-ttu-id="23861-113">[deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md)集合</span><span class="sxs-lookup"><span data-stu-id="23861-113">[deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md) collection</span></span>|<span data-ttu-id="23861-114">列出[deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="23861-114">List properties and relationships of the [deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md) objects.</span></span>|
|[<span data-ttu-id="23861-115">获取 deviceComplianceScript</span><span class="sxs-lookup"><span data-stu-id="23861-115">Get deviceComplianceScript</span></span>](../api/intune-devices-devicecompliancescript-get.md)|[<span data-ttu-id="23861-116">deviceComplianceScript</span><span class="sxs-lookup"><span data-stu-id="23861-116">deviceComplianceScript</span></span>](../resources/intune-devices-devicecompliancescript.md)|<span data-ttu-id="23861-117">读取[deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="23861-117">Read properties and relationships of the [deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md) object.</span></span>|
|[<span data-ttu-id="23861-118">创建 deviceComplianceScript</span><span class="sxs-lookup"><span data-stu-id="23861-118">Create deviceComplianceScript</span></span>](../api/intune-devices-devicecompliancescript-create.md)|[<span data-ttu-id="23861-119">deviceComplianceScript</span><span class="sxs-lookup"><span data-stu-id="23861-119">deviceComplianceScript</span></span>](../resources/intune-devices-devicecompliancescript.md)|<span data-ttu-id="23861-120">创建新的[deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md)对象。</span><span class="sxs-lookup"><span data-stu-id="23861-120">Create a new [deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md) object.</span></span>|
|[<span data-ttu-id="23861-121">删除 deviceComplianceScript</span><span class="sxs-lookup"><span data-stu-id="23861-121">Delete deviceComplianceScript</span></span>](../api/intune-devices-devicecompliancescript-delete.md)|<span data-ttu-id="23861-122">无</span><span class="sxs-lookup"><span data-stu-id="23861-122">None</span></span>|<span data-ttu-id="23861-123">删除[deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md)。</span><span class="sxs-lookup"><span data-stu-id="23861-123">Deletes a [deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md).</span></span>|
|[<span data-ttu-id="23861-124">更新 deviceComplianceScript</span><span class="sxs-lookup"><span data-stu-id="23861-124">Update deviceComplianceScript</span></span>](../api/intune-devices-devicecompliancescript-update.md)|[<span data-ttu-id="23861-125">deviceComplianceScript</span><span class="sxs-lookup"><span data-stu-id="23861-125">deviceComplianceScript</span></span>](../resources/intune-devices-devicecompliancescript.md)|<span data-ttu-id="23861-126">更新[deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="23861-126">Update the properties of a [deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md) object.</span></span>|
|[<span data-ttu-id="23861-127">分配操作</span><span class="sxs-lookup"><span data-stu-id="23861-127">assign action</span></span>](../api/intune-devices-devicecompliancescript-assign.md)|<span data-ttu-id="23861-128">无</span><span class="sxs-lookup"><span data-stu-id="23861-128">None</span></span>|<span data-ttu-id="23861-129">尚未记录</span><span class="sxs-lookup"><span data-stu-id="23861-129">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="23861-130">属性</span><span class="sxs-lookup"><span data-stu-id="23861-130">Properties</span></span>
|<span data-ttu-id="23861-131">属性</span><span class="sxs-lookup"><span data-stu-id="23861-131">Property</span></span>|<span data-ttu-id="23861-132">类型</span><span class="sxs-lookup"><span data-stu-id="23861-132">Type</span></span>|<span data-ttu-id="23861-133">说明</span><span class="sxs-lookup"><span data-stu-id="23861-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23861-134">id</span><span class="sxs-lookup"><span data-stu-id="23861-134">id</span></span>|<span data-ttu-id="23861-135">字符串</span><span class="sxs-lookup"><span data-stu-id="23861-135">String</span></span>|<span data-ttu-id="23861-136">设备符合性脚本的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="23861-136">Unique Identifier for the device compliance script</span></span>|
|<span data-ttu-id="23861-137">发布者</span><span class="sxs-lookup"><span data-stu-id="23861-137">publisher</span></span>|<span data-ttu-id="23861-138">String</span><span class="sxs-lookup"><span data-stu-id="23861-138">String</span></span>|<span data-ttu-id="23861-139">设备合规性脚本发布者的名称</span><span class="sxs-lookup"><span data-stu-id="23861-139">Name of the device compliance script publisher</span></span>|
|<span data-ttu-id="23861-140">version</span><span class="sxs-lookup"><span data-stu-id="23861-140">version</span></span>|<span data-ttu-id="23861-141">String</span><span class="sxs-lookup"><span data-stu-id="23861-141">String</span></span>|<span data-ttu-id="23861-142">设备合规性脚本的版本</span><span class="sxs-lookup"><span data-stu-id="23861-142">Version of the device compliance script</span></span>|
|<span data-ttu-id="23861-143">displayName</span><span class="sxs-lookup"><span data-stu-id="23861-143">displayName</span></span>|<span data-ttu-id="23861-144">字符串</span><span class="sxs-lookup"><span data-stu-id="23861-144">String</span></span>|<span data-ttu-id="23861-145">设备合规性脚本的名称</span><span class="sxs-lookup"><span data-stu-id="23861-145">Name of the device compliance script</span></span>|
|<span data-ttu-id="23861-146">说明</span><span class="sxs-lookup"><span data-stu-id="23861-146">description</span></span>|<span data-ttu-id="23861-147">String</span><span class="sxs-lookup"><span data-stu-id="23861-147">String</span></span>|<span data-ttu-id="23861-148">设备合规性脚本的说明</span><span class="sxs-lookup"><span data-stu-id="23861-148">Description of the device compliance script</span></span>|
|<span data-ttu-id="23861-149">detectionScriptContent</span><span class="sxs-lookup"><span data-stu-id="23861-149">detectionScriptContent</span></span>|<span data-ttu-id="23861-150">Binary</span><span class="sxs-lookup"><span data-stu-id="23861-150">Binary</span></span>|<span data-ttu-id="23861-151">检测 powershell 脚本的全部内容</span><span class="sxs-lookup"><span data-stu-id="23861-151">The entire content of the detection powershell script</span></span>|
|<span data-ttu-id="23861-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="23861-152">createdDateTime</span></span>|<span data-ttu-id="23861-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23861-153">DateTimeOffset</span></span>|<span data-ttu-id="23861-154">创建设备符合性脚本的时间戳。</span><span class="sxs-lookup"><span data-stu-id="23861-154">The timestamp of when the device compliance script was created.</span></span> <span data-ttu-id="23861-155">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="23861-155">This property is read-only.</span></span>|
|<span data-ttu-id="23861-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="23861-156">lastModifiedDateTime</span></span>|<span data-ttu-id="23861-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23861-157">DateTimeOffset</span></span>|<span data-ttu-id="23861-158">修改设备符合性脚本的时间戳。</span><span class="sxs-lookup"><span data-stu-id="23861-158">The timestamp of when the device compliance script was modified.</span></span> <span data-ttu-id="23861-159">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="23861-159">This property is read-only.</span></span>|
|<span data-ttu-id="23861-160">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="23861-160">runAsAccount</span></span>|[<span data-ttu-id="23861-161">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="23861-161">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="23861-162">指示执行上下文的类型。</span><span class="sxs-lookup"><span data-stu-id="23861-162">Indicates the type of execution context.</span></span> <span data-ttu-id="23861-163">可取值为：`system`、`user`。</span><span class="sxs-lookup"><span data-stu-id="23861-163">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="23861-164">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="23861-164">enforceSignatureCheck</span></span>|<span data-ttu-id="23861-165">布尔值</span><span class="sxs-lookup"><span data-stu-id="23861-165">Boolean</span></span>|<span data-ttu-id="23861-166">指示是否需要检查脚本签名</span><span class="sxs-lookup"><span data-stu-id="23861-166">Indicate whether the script signature needs be checked</span></span>|
|<span data-ttu-id="23861-167">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="23861-167">runAs32Bit</span></span>|<span data-ttu-id="23861-168">布尔值</span><span class="sxs-lookup"><span data-stu-id="23861-168">Boolean</span></span>|<span data-ttu-id="23861-169">指示 PowerShell 脚本是否应作为32位运行</span><span class="sxs-lookup"><span data-stu-id="23861-169">Indicate whether PowerShell script(s) should run as 32-bit</span></span>|
|<span data-ttu-id="23861-170">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="23861-170">roleScopeTagIds</span></span>|<span data-ttu-id="23861-171">String collection</span><span class="sxs-lookup"><span data-stu-id="23861-171">String collection</span></span>|<span data-ttu-id="23861-172">设备符合性脚本的作用域标记 Id 列表</span><span class="sxs-lookup"><span data-stu-id="23861-172">List of Scope Tag IDs for the device compliance script</span></span>|

## <a name="relationships"></a><span data-ttu-id="23861-173">关系</span><span class="sxs-lookup"><span data-stu-id="23861-173">Relationships</span></span>
|<span data-ttu-id="23861-174">关系</span><span class="sxs-lookup"><span data-stu-id="23861-174">Relationship</span></span>|<span data-ttu-id="23861-175">类型</span><span class="sxs-lookup"><span data-stu-id="23861-175">Type</span></span>|<span data-ttu-id="23861-176">说明</span><span class="sxs-lookup"><span data-stu-id="23861-176">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23861-177">assignments</span><span class="sxs-lookup"><span data-stu-id="23861-177">assignments</span></span>|<span data-ttu-id="23861-178">[deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="23861-178">[deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) collection</span></span>|<span data-ttu-id="23861-179">设备符合性脚本的组分配列表</span><span class="sxs-lookup"><span data-stu-id="23861-179">The list of group assignments for the device compliance script</span></span>|
|<span data-ttu-id="23861-180">runSummary</span><span class="sxs-lookup"><span data-stu-id="23861-180">runSummary</span></span>|[<span data-ttu-id="23861-181">deviceComplianceScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="23861-181">deviceComplianceScriptRunSummary</span></span>](../resources/intune-devices-devicecompliancescriptrunsummary.md)|<span data-ttu-id="23861-182">设备符合性脚本的高级别运行摘要。</span><span class="sxs-lookup"><span data-stu-id="23861-182">High level run summary for device compliance script.</span></span>|
|<span data-ttu-id="23861-183">deviceRunStates</span><span class="sxs-lookup"><span data-stu-id="23861-183">deviceRunStates</span></span>|<span data-ttu-id="23861-184">[deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md)集合</span><span class="sxs-lookup"><span data-stu-id="23861-184">[deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md) collection</span></span>|<span data-ttu-id="23861-185">跨所有设备的设备合规性脚本的运行状态列表</span><span class="sxs-lookup"><span data-stu-id="23861-185">List of run states for the device compliance script across all devices</span></span>|

## <a name="json-representation"></a><span data-ttu-id="23861-186">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="23861-186">JSON Representation</span></span>
<span data-ttu-id="23861-187">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="23861-187">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceScript"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceScript",
  "id": "String (identifier)",
  "publisher": "String",
  "version": "String",
  "displayName": "String",
  "description": "String",
  "detectionScriptContent": "binary",
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



