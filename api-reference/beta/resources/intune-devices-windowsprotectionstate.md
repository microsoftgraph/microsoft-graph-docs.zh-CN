---
title: windowsProtectionState 资源类型
description: 设备保护状态实体。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b2651aa9fad173654d8fff554bdf89f7ab36da14
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49207559"
---
# <a name="windowsprotectionstate-resource-type"></a><span data-ttu-id="d78dd-103">windowsProtectionState 资源类型</span><span class="sxs-lookup"><span data-stu-id="d78dd-103">windowsProtectionState resource type</span></span>

<span data-ttu-id="d78dd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d78dd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d78dd-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d78dd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d78dd-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d78dd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d78dd-107">设备保护状态实体。</span><span class="sxs-lookup"><span data-stu-id="d78dd-107">Device protection status entity.</span></span>

## <a name="methods"></a><span data-ttu-id="d78dd-108">方法</span><span class="sxs-lookup"><span data-stu-id="d78dd-108">Methods</span></span>
|<span data-ttu-id="d78dd-109">方法</span><span class="sxs-lookup"><span data-stu-id="d78dd-109">Method</span></span>|<span data-ttu-id="d78dd-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="d78dd-110">Return Type</span></span>|<span data-ttu-id="d78dd-111">说明</span><span class="sxs-lookup"><span data-stu-id="d78dd-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d78dd-112">获取 windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="d78dd-112">Get windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-get.md)|[<span data-ttu-id="d78dd-113">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="d78dd-113">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="d78dd-114">读取 [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d78dd-114">Read properties and relationships of the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|
|[<span data-ttu-id="d78dd-115">更新 windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="d78dd-115">Update windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-update.md)|[<span data-ttu-id="d78dd-116">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="d78dd-116">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="d78dd-117">更新 [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d78dd-117">Update the properties of a [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d78dd-118">属性</span><span class="sxs-lookup"><span data-stu-id="d78dd-118">Properties</span></span>
|<span data-ttu-id="d78dd-119">属性</span><span class="sxs-lookup"><span data-stu-id="d78dd-119">Property</span></span>|<span data-ttu-id="d78dd-120">类型</span><span class="sxs-lookup"><span data-stu-id="d78dd-120">Type</span></span>|<span data-ttu-id="d78dd-121">说明</span><span class="sxs-lookup"><span data-stu-id="d78dd-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d78dd-122">id</span><span class="sxs-lookup"><span data-stu-id="d78dd-122">id</span></span>|<span data-ttu-id="d78dd-123">String</span><span class="sxs-lookup"><span data-stu-id="d78dd-123">String</span></span>|<span data-ttu-id="d78dd-124">设备保护状态对象的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="d78dd-124">The unique Identifier for the device protection status object.</span></span> <span data-ttu-id="d78dd-125">这是设备的设备 id</span><span class="sxs-lookup"><span data-stu-id="d78dd-125">This is device id of the device</span></span>|
|<span data-ttu-id="d78dd-126">malwareProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="d78dd-126">malwareProtectionEnabled</span></span>|<span data-ttu-id="d78dd-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="d78dd-127">Boolean</span></span>|<span data-ttu-id="d78dd-128">已启用反恶意软件</span><span class="sxs-lookup"><span data-stu-id="d78dd-128">Anti malware is enabled or not</span></span>|
|<span data-ttu-id="d78dd-129">deviceState</span><span class="sxs-lookup"><span data-stu-id="d78dd-129">deviceState</span></span>|[<span data-ttu-id="d78dd-130">windowsDeviceHealthState</span><span class="sxs-lookup"><span data-stu-id="d78dd-130">windowsDeviceHealthState</span></span>](../resources/intune-devices-windowsdevicehealthstate.md)|<span data-ttu-id="d78dd-131">计算机的状态 (如干净或挂起的完全扫描或挂起的重新启动等) 。</span><span class="sxs-lookup"><span data-stu-id="d78dd-131">Computer's state (like clean or pending full scan or pending reboot etc).</span></span> <span data-ttu-id="d78dd-132">可取值为：`clean`、`fullScanPending`、`rebootPending`、`manualStepsPending`、`offlineScanPending`、`critical`。</span><span class="sxs-lookup"><span data-stu-id="d78dd-132">Possible values are: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span></span>|
|<span data-ttu-id="d78dd-133">realTimeProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="d78dd-133">realTimeProtectionEnabled</span></span>|<span data-ttu-id="d78dd-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="d78dd-134">Boolean</span></span>|<span data-ttu-id="d78dd-135">是否启用了实时保护？</span><span class="sxs-lookup"><span data-stu-id="d78dd-135">Real time protection is enabled or not?</span></span>|
|<span data-ttu-id="d78dd-136">networkInspectionSystemEnabled</span><span class="sxs-lookup"><span data-stu-id="d78dd-136">networkInspectionSystemEnabled</span></span>|<span data-ttu-id="d78dd-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="d78dd-137">Boolean</span></span>|<span data-ttu-id="d78dd-138">网络检查系统是否已启用？</span><span class="sxs-lookup"><span data-stu-id="d78dd-138">Network inspection system enabled or not?</span></span>|
|<span data-ttu-id="d78dd-139">quickScanOverdue</span><span class="sxs-lookup"><span data-stu-id="d78dd-139">quickScanOverdue</span></span>|<span data-ttu-id="d78dd-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="d78dd-140">Boolean</span></span>|<span data-ttu-id="d78dd-141">快速扫描是否过期？</span><span class="sxs-lookup"><span data-stu-id="d78dd-141">Quick scan overdue or not?</span></span>|
|<span data-ttu-id="d78dd-142">fullScanOverdue</span><span class="sxs-lookup"><span data-stu-id="d78dd-142">fullScanOverdue</span></span>|<span data-ttu-id="d78dd-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="d78dd-143">Boolean</span></span>|<span data-ttu-id="d78dd-144">完全扫描逾期？</span><span class="sxs-lookup"><span data-stu-id="d78dd-144">Full scan overdue or not?</span></span>|
|<span data-ttu-id="d78dd-145">signatureUpdateOverdue</span><span class="sxs-lookup"><span data-stu-id="d78dd-145">signatureUpdateOverdue</span></span>|<span data-ttu-id="d78dd-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="d78dd-146">Boolean</span></span>|<span data-ttu-id="d78dd-147">签名是否已过期？</span><span class="sxs-lookup"><span data-stu-id="d78dd-147">Signature out of date or not?</span></span>|
|<span data-ttu-id="d78dd-148">rebootRequired</span><span class="sxs-lookup"><span data-stu-id="d78dd-148">rebootRequired</span></span>|<span data-ttu-id="d78dd-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="d78dd-149">Boolean</span></span>|<span data-ttu-id="d78dd-150">是否需要重新启动？</span><span class="sxs-lookup"><span data-stu-id="d78dd-150">Reboot required or not?</span></span>|
|<span data-ttu-id="d78dd-151">fullScanRequired</span><span class="sxs-lookup"><span data-stu-id="d78dd-151">fullScanRequired</span></span>|<span data-ttu-id="d78dd-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="d78dd-152">Boolean</span></span>|<span data-ttu-id="d78dd-153">需要完全扫描吗？</span><span class="sxs-lookup"><span data-stu-id="d78dd-153">Full scan required or not?</span></span>|
|<span data-ttu-id="d78dd-154">engineVersion</span><span class="sxs-lookup"><span data-stu-id="d78dd-154">engineVersion</span></span>|<span data-ttu-id="d78dd-155">String</span><span class="sxs-lookup"><span data-stu-id="d78dd-155">String</span></span>|<span data-ttu-id="d78dd-156">当前 endpoint protection 引擎的版本</span><span class="sxs-lookup"><span data-stu-id="d78dd-156">Current endpoint protection engine's version</span></span>|
|<span data-ttu-id="d78dd-157">signatureVersion</span><span class="sxs-lookup"><span data-stu-id="d78dd-157">signatureVersion</span></span>|<span data-ttu-id="d78dd-158">String</span><span class="sxs-lookup"><span data-stu-id="d78dd-158">String</span></span>|<span data-ttu-id="d78dd-159">当前恶意软件定义版本</span><span class="sxs-lookup"><span data-stu-id="d78dd-159">Current malware definitions version</span></span>|
|<span data-ttu-id="d78dd-160">antiMalwareVersion</span><span class="sxs-lookup"><span data-stu-id="d78dd-160">antiMalwareVersion</span></span>|<span data-ttu-id="d78dd-161">String</span><span class="sxs-lookup"><span data-stu-id="d78dd-161">String</span></span>|<span data-ttu-id="d78dd-162">当前反恶意软件版本</span><span class="sxs-lookup"><span data-stu-id="d78dd-162">Current anti malware version</span></span>|
|<span data-ttu-id="d78dd-163">lastQuickScanDateTime</span><span class="sxs-lookup"><span data-stu-id="d78dd-163">lastQuickScanDateTime</span></span>|<span data-ttu-id="d78dd-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d78dd-164">DateTimeOffset</span></span>|<span data-ttu-id="d78dd-165">上次快速扫描日期时间</span><span class="sxs-lookup"><span data-stu-id="d78dd-165">Last quick scan datetime</span></span>|
|<span data-ttu-id="d78dd-166">lastFullScanDateTime</span><span class="sxs-lookup"><span data-stu-id="d78dd-166">lastFullScanDateTime</span></span>|<span data-ttu-id="d78dd-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d78dd-167">DateTimeOffset</span></span>|<span data-ttu-id="d78dd-168">上次快速扫描日期时间</span><span class="sxs-lookup"><span data-stu-id="d78dd-168">Last quick scan datetime</span></span>|
|<span data-ttu-id="d78dd-169">lastQuickScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="d78dd-169">lastQuickScanSignatureVersion</span></span>|<span data-ttu-id="d78dd-170">String</span><span class="sxs-lookup"><span data-stu-id="d78dd-170">String</span></span>|<span data-ttu-id="d78dd-171">上次快速扫描签名版本</span><span class="sxs-lookup"><span data-stu-id="d78dd-171">Last quick scan signature version</span></span>|
|<span data-ttu-id="d78dd-172">lastFullScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="d78dd-172">lastFullScanSignatureVersion</span></span>|<span data-ttu-id="d78dd-173">String</span><span class="sxs-lookup"><span data-stu-id="d78dd-173">String</span></span>|<span data-ttu-id="d78dd-174">上次完全扫描签名版本</span><span class="sxs-lookup"><span data-stu-id="d78dd-174">Last full scan signature version</span></span>|
|<span data-ttu-id="d78dd-175">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="d78dd-175">lastReportedDateTime</span></span>|<span data-ttu-id="d78dd-176">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d78dd-176">DateTimeOffset</span></span>|<span data-ttu-id="d78dd-177">上次设备运行状况状态报告时间</span><span class="sxs-lookup"><span data-stu-id="d78dd-177">Last device health status reported time</span></span>|
|<span data-ttu-id="d78dd-178">productStatus</span><span class="sxs-lookup"><span data-stu-id="d78dd-178">productStatus</span></span>|[<span data-ttu-id="d78dd-179">windowsDefenderProductStatus</span><span class="sxs-lookup"><span data-stu-id="d78dd-179">windowsDefenderProductStatus</span></span>](../resources/intune-devices-windowsdefenderproductstatus.md)|<span data-ttu-id="d78dd-180">Windows Defender 防病毒的产品状态。</span><span class="sxs-lookup"><span data-stu-id="d78dd-180">Product Status of Windows Defender Antivirus.</span></span> <span data-ttu-id="d78dd-181">可能的值为：、、、、、、、、、、、、、、、、、、、、、、、、、 `noStatus` `serviceNotRunning` `serviceStartedWithoutMalwareProtection` `pendingFullScanDueToThreatAction` `pendingRebootDueToThreatAction` `pendingManualStepsDueToThreatAction` `avSignaturesOutOfDate` `asSignaturesOutOfDate` `noQuickScanHappenedForSpecifiedPeriod` `noFullScanHappenedForSpecifiedPeriod` `systemInitiatedScanInProgress` `systemInitiatedCleanInProgress` `samplesPendingSubmission` `productRunningInEvaluationMode` `productRunningInNonGenuineMode` `productExpired` `offlineScanRequired` `serviceShutdownAsPartOfSystemShutdown` `threatRemediationFailedCritically` `threatRemediationFailedNonCritically` `noStatusFlagsSet` `platformOutOfDate` `platformUpdateInProgress` `platformAboutToBeOutdated` `signatureOrPlatformEndOfLifeIsPastOrIsImpending` `windowsSModeSignaturesInUseOnNonWin10SInstall` 。</span><span class="sxs-lookup"><span data-stu-id="d78dd-181">Possible values are: `noStatus`, `serviceNotRunning`, `serviceStartedWithoutMalwareProtection`, `pendingFullScanDueToThreatAction`, `pendingRebootDueToThreatAction`, `pendingManualStepsDueToThreatAction`, `avSignaturesOutOfDate`, `asSignaturesOutOfDate`, `noQuickScanHappenedForSpecifiedPeriod`, `noFullScanHappenedForSpecifiedPeriod`, `systemInitiatedScanInProgress`, `systemInitiatedCleanInProgress`, `samplesPendingSubmission`, `productRunningInEvaluationMode`, `productRunningInNonGenuineMode`, `productExpired`, `offlineScanRequired`, `serviceShutdownAsPartOfSystemShutdown`, `threatRemediationFailedCritically`, `threatRemediationFailedNonCritically`, `noStatusFlagsSet`, `platformOutOfDate`, `platformUpdateInProgress`, `platformAboutToBeOutdated`, `signatureOrPlatformEndOfLifeIsPastOrIsImpending`, `windowsSModeSignaturesInUseOnNonWin10SInstall`.</span></span>|
|<span data-ttu-id="d78dd-182">isVirtualMachine</span><span class="sxs-lookup"><span data-stu-id="d78dd-182">isVirtualMachine</span></span>|<span data-ttu-id="d78dd-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="d78dd-183">Boolean</span></span>|<span data-ttu-id="d78dd-184">指示设备是否为虚拟机。</span><span class="sxs-lookup"><span data-stu-id="d78dd-184">Indicates whether the device is a virtual machine.</span></span>|
|<span data-ttu-id="d78dd-185">tamperProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="d78dd-185">tamperProtectionEnabled</span></span>|<span data-ttu-id="d78dd-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="d78dd-186">Boolean</span></span>|<span data-ttu-id="d78dd-187">指示是否已启用 Windows Defender 防篡改保护功能。</span><span class="sxs-lookup"><span data-stu-id="d78dd-187">Indicates whether the Windows Defender tamper protection feature is enabled.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d78dd-188">关系</span><span class="sxs-lookup"><span data-stu-id="d78dd-188">Relationships</span></span>
|<span data-ttu-id="d78dd-189">关系</span><span class="sxs-lookup"><span data-stu-id="d78dd-189">Relationship</span></span>|<span data-ttu-id="d78dd-190">类型</span><span class="sxs-lookup"><span data-stu-id="d78dd-190">Type</span></span>|<span data-ttu-id="d78dd-191">说明</span><span class="sxs-lookup"><span data-stu-id="d78dd-191">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d78dd-192">detectedMalwareState</span><span class="sxs-lookup"><span data-stu-id="d78dd-192">detectedMalwareState</span></span>|<span data-ttu-id="d78dd-193">[windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d78dd-193">[windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md) collection</span></span>|<span data-ttu-id="d78dd-194">设备恶意软件列表</span><span class="sxs-lookup"><span data-stu-id="d78dd-194">Device malware list</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d78dd-195">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d78dd-195">JSON Representation</span></span>
<span data-ttu-id="d78dd-196">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d78dd-196">Here is a JSON representation of the resource.</span></span>
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
  "lastReportedDateTime": "String (timestamp)",
  "productStatus": "String",
  "isVirtualMachine": true,
  "tamperProtectionEnabled": true
}
```




