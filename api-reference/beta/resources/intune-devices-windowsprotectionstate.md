---
title: windowsProtectionState 资源类型
description: 设备的保护状态实体。
author: tfitzmac
ms.openlocfilehash: 636b969ddafde5976939df764ae1180e19a181c0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27328075"
---
# <a name="windowsprotectionstate-resource-type"></a><span data-ttu-id="e8bec-103">windowsProtectionState 资源类型</span><span class="sxs-lookup"><span data-stu-id="e8bec-103">windowsProtectionState resource type</span></span>

> <span data-ttu-id="e8bec-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e8bec-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e8bec-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e8bec-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e8bec-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e8bec-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e8bec-107">设备的保护状态实体。</span><span class="sxs-lookup"><span data-stu-id="e8bec-107">Device protection status entity.</span></span>
## <a name="methods"></a><span data-ttu-id="e8bec-108">方法</span><span class="sxs-lookup"><span data-stu-id="e8bec-108">Methods</span></span>
|<span data-ttu-id="e8bec-109">方法</span><span class="sxs-lookup"><span data-stu-id="e8bec-109">Method</span></span>|<span data-ttu-id="e8bec-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="e8bec-110">Return Type</span></span>|<span data-ttu-id="e8bec-111">说明</span><span class="sxs-lookup"><span data-stu-id="e8bec-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e8bec-112">获取 windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="e8bec-112">Get windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-get.md)|[<span data-ttu-id="e8bec-113">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="e8bec-113">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="e8bec-114">读取属性和[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="e8bec-114">Read properties and relationships of the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|
|[<span data-ttu-id="e8bec-115">更新 windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="e8bec-115">Update windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-update.md)|[<span data-ttu-id="e8bec-116">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="e8bec-116">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="e8bec-117">更新[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e8bec-117">Update the properties of a [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e8bec-118">属性</span><span class="sxs-lookup"><span data-stu-id="e8bec-118">Properties</span></span>
|<span data-ttu-id="e8bec-119">属性</span><span class="sxs-lookup"><span data-stu-id="e8bec-119">Property</span></span>|<span data-ttu-id="e8bec-120">类型</span><span class="sxs-lookup"><span data-stu-id="e8bec-120">Type</span></span>|<span data-ttu-id="e8bec-121">说明</span><span class="sxs-lookup"><span data-stu-id="e8bec-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8bec-122">id</span><span class="sxs-lookup"><span data-stu-id="e8bec-122">id</span></span>|<span data-ttu-id="e8bec-123">字符串</span><span class="sxs-lookup"><span data-stu-id="e8bec-123">String</span></span>|<span data-ttu-id="e8bec-124">设备保护状态对象的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="e8bec-124">The unique Identifier for the device protection status object.</span></span> <span data-ttu-id="e8bec-125">这是设备的设备 id</span><span class="sxs-lookup"><span data-stu-id="e8bec-125">This is device id of the device</span></span>|
|<span data-ttu-id="e8bec-126">malwareProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="e8bec-126">malwareProtectionEnabled</span></span>|<span data-ttu-id="e8bec-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8bec-127">Boolean</span></span>|<span data-ttu-id="e8bec-128">反恶意软件被启用还是没有</span><span class="sxs-lookup"><span data-stu-id="e8bec-128">Anti malware is enabled or not</span></span>|
|<span data-ttu-id="e8bec-129">deviceState</span><span class="sxs-lookup"><span data-stu-id="e8bec-129">deviceState</span></span>|[<span data-ttu-id="e8bec-130">windowsDeviceHealthState</span><span class="sxs-lookup"><span data-stu-id="e8bec-130">windowsDeviceHealthState</span></span>](../resources/intune-devices-windowsdevicehealthstate.md)|<span data-ttu-id="e8bec-131">计算机的状态 （如清理挂起完全扫描或挂起的重新启动等）。</span><span class="sxs-lookup"><span data-stu-id="e8bec-131">Computer's state (like clean or pending full scan or pending reboot etc).</span></span> <span data-ttu-id="e8bec-132">可取值为：`clean`、`fullScanPending`、`rebootPending`、`manualStepsPending`、`offlineScanPending`、`critical`。</span><span class="sxs-lookup"><span data-stu-id="e8bec-132">Possible values are: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span></span>|
|<span data-ttu-id="e8bec-133">realTimeProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="e8bec-133">realTimeProtectionEnabled</span></span>|<span data-ttu-id="e8bec-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8bec-134">Boolean</span></span>|<span data-ttu-id="e8bec-135">是否启用实时保护？</span><span class="sxs-lookup"><span data-stu-id="e8bec-135">Real time protection is enabled or not?</span></span>|
|<span data-ttu-id="e8bec-136">networkInspectionSystemEnabled</span><span class="sxs-lookup"><span data-stu-id="e8bec-136">networkInspectionSystemEnabled</span></span>|<span data-ttu-id="e8bec-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8bec-137">Boolean</span></span>|<span data-ttu-id="e8bec-138">启用或不网络检查系统？</span><span class="sxs-lookup"><span data-stu-id="e8bec-138">Network inspection system enabled or not?</span></span>|
|<span data-ttu-id="e8bec-139">quickScanOverdue</span><span class="sxs-lookup"><span data-stu-id="e8bec-139">quickScanOverdue</span></span>|<span data-ttu-id="e8bec-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8bec-140">Boolean</span></span>|<span data-ttu-id="e8bec-141">快速扫描过期，或不？</span><span class="sxs-lookup"><span data-stu-id="e8bec-141">Quick scan overdue or not?</span></span>|
|<span data-ttu-id="e8bec-142">fullScanOverdue</span><span class="sxs-lookup"><span data-stu-id="e8bec-142">fullScanOverdue</span></span>|<span data-ttu-id="e8bec-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8bec-143">Boolean</span></span>|<span data-ttu-id="e8bec-144">或不完全扫描过期？</span><span class="sxs-lookup"><span data-stu-id="e8bec-144">Full scan overdue or not?</span></span>|
|<span data-ttu-id="e8bec-145">signatureUpdateOverdue</span><span class="sxs-lookup"><span data-stu-id="e8bec-145">signatureUpdateOverdue</span></span>|<span data-ttu-id="e8bec-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8bec-146">Boolean</span></span>|<span data-ttu-id="e8bec-147">过期的签名或不？</span><span class="sxs-lookup"><span data-stu-id="e8bec-147">Signature out of date or not?</span></span>|
|<span data-ttu-id="e8bec-148">rebootRequired</span><span class="sxs-lookup"><span data-stu-id="e8bec-148">rebootRequired</span></span>|<span data-ttu-id="e8bec-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8bec-149">Boolean</span></span>|<span data-ttu-id="e8bec-150">需要或不重新启动？</span><span class="sxs-lookup"><span data-stu-id="e8bec-150">Reboot required or not?</span></span>|
|<span data-ttu-id="e8bec-151">fullScanRequired</span><span class="sxs-lookup"><span data-stu-id="e8bec-151">fullScanRequired</span></span>|<span data-ttu-id="e8bec-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8bec-152">Boolean</span></span>|<span data-ttu-id="e8bec-153">所需或不完全扫描？</span><span class="sxs-lookup"><span data-stu-id="e8bec-153">Full scan required or not?</span></span>|
|<span data-ttu-id="e8bec-154">engineVersion</span><span class="sxs-lookup"><span data-stu-id="e8bec-154">engineVersion</span></span>|<span data-ttu-id="e8bec-155">字符串</span><span class="sxs-lookup"><span data-stu-id="e8bec-155">String</span></span>|<span data-ttu-id="e8bec-156">当前终结点保护引擎的版本</span><span class="sxs-lookup"><span data-stu-id="e8bec-156">Current endpoint protection engine's version</span></span>|
|<span data-ttu-id="e8bec-157">特征码版本</span><span class="sxs-lookup"><span data-stu-id="e8bec-157">signatureVersion</span></span>|<span data-ttu-id="e8bec-158">字符串</span><span class="sxs-lookup"><span data-stu-id="e8bec-158">String</span></span>|<span data-ttu-id="e8bec-159">当前的恶意软件定义版本</span><span class="sxs-lookup"><span data-stu-id="e8bec-159">Current malware definitions version</span></span>|
|<span data-ttu-id="e8bec-160">antiMalwareVersion</span><span class="sxs-lookup"><span data-stu-id="e8bec-160">antiMalwareVersion</span></span>|<span data-ttu-id="e8bec-161">字符串</span><span class="sxs-lookup"><span data-stu-id="e8bec-161">String</span></span>|<span data-ttu-id="e8bec-162">当前防恶意软件版本</span><span class="sxs-lookup"><span data-stu-id="e8bec-162">Current anti malware version</span></span>|
|<span data-ttu-id="e8bec-163">lastQuickScanDateTime</span><span class="sxs-lookup"><span data-stu-id="e8bec-163">lastQuickScanDateTime</span></span>|<span data-ttu-id="e8bec-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e8bec-164">DateTimeOffset</span></span>|<span data-ttu-id="e8bec-165">最后一个快速扫描 datetime</span><span class="sxs-lookup"><span data-stu-id="e8bec-165">Last quick scan datetime</span></span>|
|<span data-ttu-id="e8bec-166">lastFullScanDateTime</span><span class="sxs-lookup"><span data-stu-id="e8bec-166">lastFullScanDateTime</span></span>|<span data-ttu-id="e8bec-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e8bec-167">DateTimeOffset</span></span>|<span data-ttu-id="e8bec-168">最后一个快速扫描 datetime</span><span class="sxs-lookup"><span data-stu-id="e8bec-168">Last quick scan datetime</span></span>|
|<span data-ttu-id="e8bec-169">lastQuickScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="e8bec-169">lastQuickScanSignatureVersion</span></span>|<span data-ttu-id="e8bec-170">字符串</span><span class="sxs-lookup"><span data-stu-id="e8bec-170">String</span></span>|<span data-ttu-id="e8bec-171">最后一个快速扫描病毒特征版本</span><span class="sxs-lookup"><span data-stu-id="e8bec-171">Last quick scan signature version</span></span>|
|<span data-ttu-id="e8bec-172">lastFullScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="e8bec-172">lastFullScanSignatureVersion</span></span>|<span data-ttu-id="e8bec-173">字符串</span><span class="sxs-lookup"><span data-stu-id="e8bec-173">String</span></span>|<span data-ttu-id="e8bec-174">最后一个完全扫描病毒特征版本</span><span class="sxs-lookup"><span data-stu-id="e8bec-174">Last full scan signature version</span></span>|
|<span data-ttu-id="e8bec-175">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="e8bec-175">lastReportedDateTime</span></span>|<span data-ttu-id="e8bec-176">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e8bec-176">DateTimeOffset</span></span>|<span data-ttu-id="e8bec-177">最后一个设备运行状况状态报告的时间</span><span class="sxs-lookup"><span data-stu-id="e8bec-177">Last device health status reported time</span></span>|

## <a name="relationships"></a><span data-ttu-id="e8bec-178">Relationships</span><span class="sxs-lookup"><span data-stu-id="e8bec-178">Relationships</span></span>
|<span data-ttu-id="e8bec-179">关系</span><span class="sxs-lookup"><span data-stu-id="e8bec-179">Relationship</span></span>|<span data-ttu-id="e8bec-180">类型</span><span class="sxs-lookup"><span data-stu-id="e8bec-180">Type</span></span>|<span data-ttu-id="e8bec-181">说明</span><span class="sxs-lookup"><span data-stu-id="e8bec-181">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8bec-182">detectedMalwareState</span><span class="sxs-lookup"><span data-stu-id="e8bec-182">detectedMalwareState</span></span>|<span data-ttu-id="e8bec-183">[windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md)集合</span><span class="sxs-lookup"><span data-stu-id="e8bec-183">[windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md) collection</span></span>|<span data-ttu-id="e8bec-184">设备恶意软件的列表</span><span class="sxs-lookup"><span data-stu-id="e8bec-184">Device malware list</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e8bec-185">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e8bec-185">JSON Representation</span></span>
<span data-ttu-id="e8bec-186">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e8bec-186">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsProtectionState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsProtectionState",
  "id": "String (identifier)",
  "malwareProtectionEnabled": true,
  "deviceState": "String",
  "realTimeProtectionEnabled": true,
  "networkInspectionSystemEnabled": true,
  "quickScanOverdue": true,
  "fullScanOverdue": true,
  "signatureUpdateOverdue": true,
  "rebootRequired": true,
  "fullScanRequired": true,
  "engineVersion": "String",
  "signatureVersion": "String",
  "antiMalwareVersion": "String",
  "lastQuickScanDateTime": "String (timestamp)",
  "lastFullScanDateTime": "String (timestamp)",
  "lastQuickScanSignatureVersion": "String",
  "lastFullScanSignatureVersion": "String",
  "lastReportedDateTime": "String (timestamp)"
}
```





