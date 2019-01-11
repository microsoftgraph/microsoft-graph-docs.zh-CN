---
title: windowsProtectionState 资源类型
description: 设备的保护状态实体。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5a21cc27039f3119836e0027b2558cadadab1b5d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884103"
---
# <a name="windowsprotectionstate-resource-type"></a><span data-ttu-id="c67f6-103">windowsProtectionState 资源类型</span><span class="sxs-lookup"><span data-stu-id="c67f6-103">windowsProtectionState resource type</span></span>

> <span data-ttu-id="c67f6-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c67f6-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c67f6-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c67f6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c67f6-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="c67f6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c67f6-107">设备的保护状态实体。</span><span class="sxs-lookup"><span data-stu-id="c67f6-107">Device protection status entity.</span></span>
## <a name="methods"></a><span data-ttu-id="c67f6-108">方法</span><span class="sxs-lookup"><span data-stu-id="c67f6-108">Methods</span></span>
|<span data-ttu-id="c67f6-109">方法</span><span class="sxs-lookup"><span data-stu-id="c67f6-109">Method</span></span>|<span data-ttu-id="c67f6-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="c67f6-110">Return Type</span></span>|<span data-ttu-id="c67f6-111">说明</span><span class="sxs-lookup"><span data-stu-id="c67f6-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c67f6-112">获取 windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="c67f6-112">Get windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-get.md)|[<span data-ttu-id="c67f6-113">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="c67f6-113">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="c67f6-114">读取属性和[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="c67f6-114">Read properties and relationships of the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|
|[<span data-ttu-id="c67f6-115">更新 windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="c67f6-115">Update windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-update.md)|[<span data-ttu-id="c67f6-116">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="c67f6-116">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="c67f6-117">更新[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c67f6-117">Update the properties of a [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c67f6-118">属性</span><span class="sxs-lookup"><span data-stu-id="c67f6-118">Properties</span></span>
|<span data-ttu-id="c67f6-119">属性</span><span class="sxs-lookup"><span data-stu-id="c67f6-119">Property</span></span>|<span data-ttu-id="c67f6-120">类型</span><span class="sxs-lookup"><span data-stu-id="c67f6-120">Type</span></span>|<span data-ttu-id="c67f6-121">说明</span><span class="sxs-lookup"><span data-stu-id="c67f6-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c67f6-122">id</span><span class="sxs-lookup"><span data-stu-id="c67f6-122">id</span></span>|<span data-ttu-id="c67f6-123">字符串</span><span class="sxs-lookup"><span data-stu-id="c67f6-123">String</span></span>|<span data-ttu-id="c67f6-124">设备保护状态对象的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="c67f6-124">The unique Identifier for the device protection status object.</span></span> <span data-ttu-id="c67f6-125">这是设备的设备 id</span><span class="sxs-lookup"><span data-stu-id="c67f6-125">This is device id of the device</span></span>|
|<span data-ttu-id="c67f6-126">malwareProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="c67f6-126">malwareProtectionEnabled</span></span>|<span data-ttu-id="c67f6-127">布尔</span><span class="sxs-lookup"><span data-stu-id="c67f6-127">Boolean</span></span>|<span data-ttu-id="c67f6-128">反恶意软件被启用还是没有</span><span class="sxs-lookup"><span data-stu-id="c67f6-128">Anti malware is enabled or not</span></span>|
|<span data-ttu-id="c67f6-129">deviceState</span><span class="sxs-lookup"><span data-stu-id="c67f6-129">deviceState</span></span>|[<span data-ttu-id="c67f6-130">windowsDeviceHealthState</span><span class="sxs-lookup"><span data-stu-id="c67f6-130">windowsDeviceHealthState</span></span>](../resources/intune-devices-windowsdevicehealthstate.md)|<span data-ttu-id="c67f6-131">计算机的状态 （如清理挂起完全扫描或挂起的重新启动等）。</span><span class="sxs-lookup"><span data-stu-id="c67f6-131">Computer's state (like clean or pending full scan or pending reboot etc).</span></span> <span data-ttu-id="c67f6-132">可取值为：`clean`、`fullScanPending`、`rebootPending`、`manualStepsPending`、`offlineScanPending`、`critical`。</span><span class="sxs-lookup"><span data-stu-id="c67f6-132">Possible values are: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span></span>|
|<span data-ttu-id="c67f6-133">realTimeProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="c67f6-133">realTimeProtectionEnabled</span></span>|<span data-ttu-id="c67f6-134">布尔</span><span class="sxs-lookup"><span data-stu-id="c67f6-134">Boolean</span></span>|<span data-ttu-id="c67f6-135">是否启用实时保护？</span><span class="sxs-lookup"><span data-stu-id="c67f6-135">Real time protection is enabled or not?</span></span>|
|<span data-ttu-id="c67f6-136">networkInspectionSystemEnabled</span><span class="sxs-lookup"><span data-stu-id="c67f6-136">networkInspectionSystemEnabled</span></span>|<span data-ttu-id="c67f6-137">布尔</span><span class="sxs-lookup"><span data-stu-id="c67f6-137">Boolean</span></span>|<span data-ttu-id="c67f6-138">启用或不网络检查系统？</span><span class="sxs-lookup"><span data-stu-id="c67f6-138">Network inspection system enabled or not?</span></span>|
|<span data-ttu-id="c67f6-139">quickScanOverdue</span><span class="sxs-lookup"><span data-stu-id="c67f6-139">quickScanOverdue</span></span>|<span data-ttu-id="c67f6-140">布尔</span><span class="sxs-lookup"><span data-stu-id="c67f6-140">Boolean</span></span>|<span data-ttu-id="c67f6-141">快速扫描过期，或不？</span><span class="sxs-lookup"><span data-stu-id="c67f6-141">Quick scan overdue or not?</span></span>|
|<span data-ttu-id="c67f6-142">fullScanOverdue</span><span class="sxs-lookup"><span data-stu-id="c67f6-142">fullScanOverdue</span></span>|<span data-ttu-id="c67f6-143">布尔</span><span class="sxs-lookup"><span data-stu-id="c67f6-143">Boolean</span></span>|<span data-ttu-id="c67f6-144">或不完全扫描过期？</span><span class="sxs-lookup"><span data-stu-id="c67f6-144">Full scan overdue or not?</span></span>|
|<span data-ttu-id="c67f6-145">signatureUpdateOverdue</span><span class="sxs-lookup"><span data-stu-id="c67f6-145">signatureUpdateOverdue</span></span>|<span data-ttu-id="c67f6-146">布尔</span><span class="sxs-lookup"><span data-stu-id="c67f6-146">Boolean</span></span>|<span data-ttu-id="c67f6-147">过期的签名或不？</span><span class="sxs-lookup"><span data-stu-id="c67f6-147">Signature out of date or not?</span></span>|
|<span data-ttu-id="c67f6-148">rebootRequired</span><span class="sxs-lookup"><span data-stu-id="c67f6-148">rebootRequired</span></span>|<span data-ttu-id="c67f6-149">布尔</span><span class="sxs-lookup"><span data-stu-id="c67f6-149">Boolean</span></span>|<span data-ttu-id="c67f6-150">需要或不重新启动？</span><span class="sxs-lookup"><span data-stu-id="c67f6-150">Reboot required or not?</span></span>|
|<span data-ttu-id="c67f6-151">fullScanRequired</span><span class="sxs-lookup"><span data-stu-id="c67f6-151">fullScanRequired</span></span>|<span data-ttu-id="c67f6-152">布尔</span><span class="sxs-lookup"><span data-stu-id="c67f6-152">Boolean</span></span>|<span data-ttu-id="c67f6-153">所需或不完全扫描？</span><span class="sxs-lookup"><span data-stu-id="c67f6-153">Full scan required or not?</span></span>|
|<span data-ttu-id="c67f6-154">engineVersion</span><span class="sxs-lookup"><span data-stu-id="c67f6-154">engineVersion</span></span>|<span data-ttu-id="c67f6-155">字符串</span><span class="sxs-lookup"><span data-stu-id="c67f6-155">String</span></span>|<span data-ttu-id="c67f6-156">当前终结点保护引擎的版本</span><span class="sxs-lookup"><span data-stu-id="c67f6-156">Current endpoint protection engine's version</span></span>|
|<span data-ttu-id="c67f6-157">特征码版本</span><span class="sxs-lookup"><span data-stu-id="c67f6-157">signatureVersion</span></span>|<span data-ttu-id="c67f6-158">字符串</span><span class="sxs-lookup"><span data-stu-id="c67f6-158">String</span></span>|<span data-ttu-id="c67f6-159">当前的恶意软件定义版本</span><span class="sxs-lookup"><span data-stu-id="c67f6-159">Current malware definitions version</span></span>|
|<span data-ttu-id="c67f6-160">antiMalwareVersion</span><span class="sxs-lookup"><span data-stu-id="c67f6-160">antiMalwareVersion</span></span>|<span data-ttu-id="c67f6-161">字符串</span><span class="sxs-lookup"><span data-stu-id="c67f6-161">String</span></span>|<span data-ttu-id="c67f6-162">当前防恶意软件版本</span><span class="sxs-lookup"><span data-stu-id="c67f6-162">Current anti malware version</span></span>|
|<span data-ttu-id="c67f6-163">lastQuickScanDateTime</span><span class="sxs-lookup"><span data-stu-id="c67f6-163">lastQuickScanDateTime</span></span>|<span data-ttu-id="c67f6-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c67f6-164">DateTimeOffset</span></span>|<span data-ttu-id="c67f6-165">最后一个快速扫描 datetime</span><span class="sxs-lookup"><span data-stu-id="c67f6-165">Last quick scan datetime</span></span>|
|<span data-ttu-id="c67f6-166">lastFullScanDateTime</span><span class="sxs-lookup"><span data-stu-id="c67f6-166">lastFullScanDateTime</span></span>|<span data-ttu-id="c67f6-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c67f6-167">DateTimeOffset</span></span>|<span data-ttu-id="c67f6-168">最后一个快速扫描 datetime</span><span class="sxs-lookup"><span data-stu-id="c67f6-168">Last quick scan datetime</span></span>|
|<span data-ttu-id="c67f6-169">lastQuickScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="c67f6-169">lastQuickScanSignatureVersion</span></span>|<span data-ttu-id="c67f6-170">字符串</span><span class="sxs-lookup"><span data-stu-id="c67f6-170">String</span></span>|<span data-ttu-id="c67f6-171">最后一个快速扫描病毒特征版本</span><span class="sxs-lookup"><span data-stu-id="c67f6-171">Last quick scan signature version</span></span>|
|<span data-ttu-id="c67f6-172">lastFullScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="c67f6-172">lastFullScanSignatureVersion</span></span>|<span data-ttu-id="c67f6-173">字符串</span><span class="sxs-lookup"><span data-stu-id="c67f6-173">String</span></span>|<span data-ttu-id="c67f6-174">最后一个完全扫描病毒特征版本</span><span class="sxs-lookup"><span data-stu-id="c67f6-174">Last full scan signature version</span></span>|
|<span data-ttu-id="c67f6-175">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="c67f6-175">lastReportedDateTime</span></span>|<span data-ttu-id="c67f6-176">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c67f6-176">DateTimeOffset</span></span>|<span data-ttu-id="c67f6-177">最后一个设备运行状况状态报告的时间</span><span class="sxs-lookup"><span data-stu-id="c67f6-177">Last device health status reported time</span></span>|

## <a name="relationships"></a><span data-ttu-id="c67f6-178">Relationships</span><span class="sxs-lookup"><span data-stu-id="c67f6-178">Relationships</span></span>
|<span data-ttu-id="c67f6-179">关系</span><span class="sxs-lookup"><span data-stu-id="c67f6-179">Relationship</span></span>|<span data-ttu-id="c67f6-180">类型</span><span class="sxs-lookup"><span data-stu-id="c67f6-180">Type</span></span>|<span data-ttu-id="c67f6-181">Description</span><span class="sxs-lookup"><span data-stu-id="c67f6-181">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c67f6-182">detectedMalwareState</span><span class="sxs-lookup"><span data-stu-id="c67f6-182">detectedMalwareState</span></span>|<span data-ttu-id="c67f6-183">[windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md)集合</span><span class="sxs-lookup"><span data-stu-id="c67f6-183">[windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md) collection</span></span>|<span data-ttu-id="c67f6-184">设备恶意软件的列表</span><span class="sxs-lookup"><span data-stu-id="c67f6-184">Device malware list</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c67f6-185">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c67f6-185">JSON Representation</span></span>
<span data-ttu-id="c67f6-186">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c67f6-186">Here is a JSON representation of the resource.</span></span>
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





