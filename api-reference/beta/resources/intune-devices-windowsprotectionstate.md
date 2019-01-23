---
title: windowsProtectionState 资源类型
description: 设备的保护状态实体。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1ef6c86983475abc687055ac2322ba02fae27ecd
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423585"
---
# <a name="windowsprotectionstate-resource-type"></a><span data-ttu-id="effec-103">windowsProtectionState 资源类型</span><span class="sxs-lookup"><span data-stu-id="effec-103">windowsProtectionState resource type</span></span>

> <span data-ttu-id="effec-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="effec-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="effec-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="effec-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="effec-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="effec-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="effec-107">设备的保护状态实体。</span><span class="sxs-lookup"><span data-stu-id="effec-107">Device protection status entity.</span></span>

## <a name="methods"></a><span data-ttu-id="effec-108">方法</span><span class="sxs-lookup"><span data-stu-id="effec-108">Methods</span></span>
|<span data-ttu-id="effec-109">方法</span><span class="sxs-lookup"><span data-stu-id="effec-109">Method</span></span>|<span data-ttu-id="effec-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="effec-110">Return Type</span></span>|<span data-ttu-id="effec-111">说明</span><span class="sxs-lookup"><span data-stu-id="effec-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="effec-112">获取 windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="effec-112">Get windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-get.md)|[<span data-ttu-id="effec-113">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="effec-113">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="effec-114">读取属性和[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="effec-114">Read properties and relationships of the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|
|[<span data-ttu-id="effec-115">更新 windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="effec-115">Update windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-update.md)|[<span data-ttu-id="effec-116">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="effec-116">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="effec-117">更新[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="effec-117">Update the properties of a [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="effec-118">属性</span><span class="sxs-lookup"><span data-stu-id="effec-118">Properties</span></span>
|<span data-ttu-id="effec-119">属性</span><span class="sxs-lookup"><span data-stu-id="effec-119">Property</span></span>|<span data-ttu-id="effec-120">类型</span><span class="sxs-lookup"><span data-stu-id="effec-120">Type</span></span>|<span data-ttu-id="effec-121">说明</span><span class="sxs-lookup"><span data-stu-id="effec-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="effec-122">id</span><span class="sxs-lookup"><span data-stu-id="effec-122">id</span></span>|<span data-ttu-id="effec-123">String</span><span class="sxs-lookup"><span data-stu-id="effec-123">String</span></span>|<span data-ttu-id="effec-124">设备保护状态对象的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="effec-124">The unique Identifier for the device protection status object.</span></span> <span data-ttu-id="effec-125">这是设备的设备 id</span><span class="sxs-lookup"><span data-stu-id="effec-125">This is device id of the device</span></span>|
|<span data-ttu-id="effec-126">malwareProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="effec-126">malwareProtectionEnabled</span></span>|<span data-ttu-id="effec-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="effec-127">Boolean</span></span>|<span data-ttu-id="effec-128">反恶意软件被启用还是没有</span><span class="sxs-lookup"><span data-stu-id="effec-128">Anti malware is enabled or not</span></span>|
|<span data-ttu-id="effec-129">deviceState</span><span class="sxs-lookup"><span data-stu-id="effec-129">deviceState</span></span>|[<span data-ttu-id="effec-130">windowsDeviceHealthState</span><span class="sxs-lookup"><span data-stu-id="effec-130">windowsDeviceHealthState</span></span>](../resources/intune-devices-windowsdevicehealthstate.md)|<span data-ttu-id="effec-131">计算机的状态 （如清理挂起完全扫描或挂起的重新启动等）。</span><span class="sxs-lookup"><span data-stu-id="effec-131">Computer's state (like clean or pending full scan or pending reboot etc).</span></span> <span data-ttu-id="effec-132">可取值为：`clean`、`fullScanPending`、`rebootPending`、`manualStepsPending`、`offlineScanPending`、`critical`。</span><span class="sxs-lookup"><span data-stu-id="effec-132">Possible values are: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span></span>|
|<span data-ttu-id="effec-133">realTimeProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="effec-133">realTimeProtectionEnabled</span></span>|<span data-ttu-id="effec-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="effec-134">Boolean</span></span>|<span data-ttu-id="effec-135">是否启用实时保护？</span><span class="sxs-lookup"><span data-stu-id="effec-135">Real time protection is enabled or not?</span></span>|
|<span data-ttu-id="effec-136">networkInspectionSystemEnabled</span><span class="sxs-lookup"><span data-stu-id="effec-136">networkInspectionSystemEnabled</span></span>|<span data-ttu-id="effec-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="effec-137">Boolean</span></span>|<span data-ttu-id="effec-138">启用或不网络检查系统？</span><span class="sxs-lookup"><span data-stu-id="effec-138">Network inspection system enabled or not?</span></span>|
|<span data-ttu-id="effec-139">quickScanOverdue</span><span class="sxs-lookup"><span data-stu-id="effec-139">quickScanOverdue</span></span>|<span data-ttu-id="effec-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="effec-140">Boolean</span></span>|<span data-ttu-id="effec-141">快速扫描过期，或不？</span><span class="sxs-lookup"><span data-stu-id="effec-141">Quick scan overdue or not?</span></span>|
|<span data-ttu-id="effec-142">fullScanOverdue</span><span class="sxs-lookup"><span data-stu-id="effec-142">fullScanOverdue</span></span>|<span data-ttu-id="effec-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="effec-143">Boolean</span></span>|<span data-ttu-id="effec-144">或不完全扫描过期？</span><span class="sxs-lookup"><span data-stu-id="effec-144">Full scan overdue or not?</span></span>|
|<span data-ttu-id="effec-145">signatureUpdateOverdue</span><span class="sxs-lookup"><span data-stu-id="effec-145">signatureUpdateOverdue</span></span>|<span data-ttu-id="effec-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="effec-146">Boolean</span></span>|<span data-ttu-id="effec-147">过期的签名或不？</span><span class="sxs-lookup"><span data-stu-id="effec-147">Signature out of date or not?</span></span>|
|<span data-ttu-id="effec-148">rebootRequired</span><span class="sxs-lookup"><span data-stu-id="effec-148">rebootRequired</span></span>|<span data-ttu-id="effec-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="effec-149">Boolean</span></span>|<span data-ttu-id="effec-150">需要或不重新启动？</span><span class="sxs-lookup"><span data-stu-id="effec-150">Reboot required or not?</span></span>|
|<span data-ttu-id="effec-151">fullScanRequired</span><span class="sxs-lookup"><span data-stu-id="effec-151">fullScanRequired</span></span>|<span data-ttu-id="effec-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="effec-152">Boolean</span></span>|<span data-ttu-id="effec-153">所需或不完全扫描？</span><span class="sxs-lookup"><span data-stu-id="effec-153">Full scan required or not?</span></span>|
|<span data-ttu-id="effec-154">engineVersion</span><span class="sxs-lookup"><span data-stu-id="effec-154">engineVersion</span></span>|<span data-ttu-id="effec-155">String</span><span class="sxs-lookup"><span data-stu-id="effec-155">String</span></span>|<span data-ttu-id="effec-156">当前终结点保护引擎的版本</span><span class="sxs-lookup"><span data-stu-id="effec-156">Current endpoint protection engine's version</span></span>|
|<span data-ttu-id="effec-157">特征码版本</span><span class="sxs-lookup"><span data-stu-id="effec-157">signatureVersion</span></span>|<span data-ttu-id="effec-158">String</span><span class="sxs-lookup"><span data-stu-id="effec-158">String</span></span>|<span data-ttu-id="effec-159">当前的恶意软件定义版本</span><span class="sxs-lookup"><span data-stu-id="effec-159">Current malware definitions version</span></span>|
|<span data-ttu-id="effec-160">antiMalwareVersion</span><span class="sxs-lookup"><span data-stu-id="effec-160">antiMalwareVersion</span></span>|<span data-ttu-id="effec-161">String</span><span class="sxs-lookup"><span data-stu-id="effec-161">String</span></span>|<span data-ttu-id="effec-162">当前防恶意软件版本</span><span class="sxs-lookup"><span data-stu-id="effec-162">Current anti malware version</span></span>|
|<span data-ttu-id="effec-163">lastQuickScanDateTime</span><span class="sxs-lookup"><span data-stu-id="effec-163">lastQuickScanDateTime</span></span>|<span data-ttu-id="effec-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="effec-164">DateTimeOffset</span></span>|<span data-ttu-id="effec-165">最后一个快速扫描 datetime</span><span class="sxs-lookup"><span data-stu-id="effec-165">Last quick scan datetime</span></span>|
|<span data-ttu-id="effec-166">lastFullScanDateTime</span><span class="sxs-lookup"><span data-stu-id="effec-166">lastFullScanDateTime</span></span>|<span data-ttu-id="effec-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="effec-167">DateTimeOffset</span></span>|<span data-ttu-id="effec-168">最后一个快速扫描 datetime</span><span class="sxs-lookup"><span data-stu-id="effec-168">Last quick scan datetime</span></span>|
|<span data-ttu-id="effec-169">lastQuickScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="effec-169">lastQuickScanSignatureVersion</span></span>|<span data-ttu-id="effec-170">String</span><span class="sxs-lookup"><span data-stu-id="effec-170">String</span></span>|<span data-ttu-id="effec-171">最后一个快速扫描病毒特征版本</span><span class="sxs-lookup"><span data-stu-id="effec-171">Last quick scan signature version</span></span>|
|<span data-ttu-id="effec-172">lastFullScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="effec-172">lastFullScanSignatureVersion</span></span>|<span data-ttu-id="effec-173">String</span><span class="sxs-lookup"><span data-stu-id="effec-173">String</span></span>|<span data-ttu-id="effec-174">最后一个完全扫描病毒特征版本</span><span class="sxs-lookup"><span data-stu-id="effec-174">Last full scan signature version</span></span>|
|<span data-ttu-id="effec-175">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="effec-175">lastReportedDateTime</span></span>|<span data-ttu-id="effec-176">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="effec-176">DateTimeOffset</span></span>|<span data-ttu-id="effec-177">最后一个设备运行状况状态报告的时间</span><span class="sxs-lookup"><span data-stu-id="effec-177">Last device health status reported time</span></span>|

## <a name="relationships"></a><span data-ttu-id="effec-178">关系</span><span class="sxs-lookup"><span data-stu-id="effec-178">Relationships</span></span>
|<span data-ttu-id="effec-179">关系</span><span class="sxs-lookup"><span data-stu-id="effec-179">Relationship</span></span>|<span data-ttu-id="effec-180">类型</span><span class="sxs-lookup"><span data-stu-id="effec-180">Type</span></span>|<span data-ttu-id="effec-181">说明</span><span class="sxs-lookup"><span data-stu-id="effec-181">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="effec-182">detectedMalwareState</span><span class="sxs-lookup"><span data-stu-id="effec-182">detectedMalwareState</span></span>|<span data-ttu-id="effec-183">[windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md)集合</span><span class="sxs-lookup"><span data-stu-id="effec-183">[windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md) collection</span></span>|<span data-ttu-id="effec-184">设备恶意软件的列表</span><span class="sxs-lookup"><span data-stu-id="effec-184">Device malware list</span></span>|

## <a name="json-representation"></a><span data-ttu-id="effec-185">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="effec-185">JSON Representation</span></span>
<span data-ttu-id="effec-186">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="effec-186">Here is a JSON representation of the resource.</span></span>
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




