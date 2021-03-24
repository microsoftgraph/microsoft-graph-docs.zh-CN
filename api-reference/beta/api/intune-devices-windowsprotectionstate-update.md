---
title: 更新 windowsProtectionState
description: 更新 windowsProtectionState 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2a500c5f1510a28638e58be0ef32d328cc598776
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51135829"
---
# <a name="update-windowsprotectionstate"></a><span data-ttu-id="e2a11-103">更新 windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="e2a11-103">Update windowsProtectionState</span></span>

<span data-ttu-id="e2a11-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e2a11-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e2a11-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e2a11-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e2a11-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e2a11-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e2a11-107">更新 [windowsProtectionState 对象](../resources/intune-devices-windowsprotectionstate.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="e2a11-107">Update the properties of a [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e2a11-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="e2a11-108">Prerequisites</span></span>
<span data-ttu-id="e2a11-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e2a11-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2a11-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e2a11-111">Permission type</span></span>|<span data-ttu-id="e2a11-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e2a11-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e2a11-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e2a11-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e2a11-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2a11-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="e2a11-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e2a11-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e2a11-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e2a11-116">Not supported.</span></span>|
|<span data-ttu-id="e2a11-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e2a11-117">Application</span></span>|<span data-ttu-id="e2a11-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2a11-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e2a11-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e2a11-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/windowsProtectionState
```

## <a name="request-headers"></a><span data-ttu-id="e2a11-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e2a11-120">Request headers</span></span>
|<span data-ttu-id="e2a11-121">标头</span><span class="sxs-lookup"><span data-stu-id="e2a11-121">Header</span></span>|<span data-ttu-id="e2a11-122">值</span><span class="sxs-lookup"><span data-stu-id="e2a11-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e2a11-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e2a11-123">Authorization</span></span>|<span data-ttu-id="e2a11-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e2a11-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e2a11-125">接受</span><span class="sxs-lookup"><span data-stu-id="e2a11-125">Accept</span></span>|<span data-ttu-id="e2a11-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e2a11-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e2a11-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e2a11-127">Request body</span></span>
<span data-ttu-id="e2a11-128">在请求正文中，提供 [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e2a11-128">In the request body, supply a JSON representation for the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>

<span data-ttu-id="e2a11-129">下表显示创建 [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e2a11-129">The following table shows the properties that are required when you create the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md).</span></span>

|<span data-ttu-id="e2a11-130">属性</span><span class="sxs-lookup"><span data-stu-id="e2a11-130">Property</span></span>|<span data-ttu-id="e2a11-131">类型</span><span class="sxs-lookup"><span data-stu-id="e2a11-131">Type</span></span>|<span data-ttu-id="e2a11-132">说明</span><span class="sxs-lookup"><span data-stu-id="e2a11-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2a11-133">id</span><span class="sxs-lookup"><span data-stu-id="e2a11-133">id</span></span>|<span data-ttu-id="e2a11-134">String</span><span class="sxs-lookup"><span data-stu-id="e2a11-134">String</span></span>|<span data-ttu-id="e2a11-135">设备保护状态对象的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="e2a11-135">The unique Identifier for the device protection status object.</span></span> <span data-ttu-id="e2a11-136">这是设备的设备 ID</span><span class="sxs-lookup"><span data-stu-id="e2a11-136">This is device id of the device</span></span>|
|<span data-ttu-id="e2a11-137">malwareProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="e2a11-137">malwareProtectionEnabled</span></span>|<span data-ttu-id="e2a11-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2a11-138">Boolean</span></span>|<span data-ttu-id="e2a11-139">反恶意软件是否已启用</span><span class="sxs-lookup"><span data-stu-id="e2a11-139">Anti malware is enabled or not</span></span>|
|<span data-ttu-id="e2a11-140">deviceState</span><span class="sxs-lookup"><span data-stu-id="e2a11-140">deviceState</span></span>|[<span data-ttu-id="e2a11-141">windowsDeviceHealthState</span><span class="sxs-lookup"><span data-stu-id="e2a11-141">windowsDeviceHealthState</span></span>](../resources/intune-devices-windowsdevicehealthstate.md)|<span data-ttu-id="e2a11-142">计算机的状态 (干净或挂起完全扫描或挂起重启等) 。</span><span class="sxs-lookup"><span data-stu-id="e2a11-142">Computer's state (like clean or pending full scan or pending reboot etc).</span></span> <span data-ttu-id="e2a11-143">可取值为：`clean`、`fullScanPending`、`rebootPending`、`manualStepsPending`、`offlineScanPending`、`critical`。</span><span class="sxs-lookup"><span data-stu-id="e2a11-143">Possible values are: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span></span>|
|<span data-ttu-id="e2a11-144">realTimeProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="e2a11-144">realTimeProtectionEnabled</span></span>|<span data-ttu-id="e2a11-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2a11-145">Boolean</span></span>|<span data-ttu-id="e2a11-146">实时保护是否已启用？</span><span class="sxs-lookup"><span data-stu-id="e2a11-146">Real time protection is enabled or not?</span></span>|
|<span data-ttu-id="e2a11-147">networkInspectionSystemEnabled</span><span class="sxs-lookup"><span data-stu-id="e2a11-147">networkInspectionSystemEnabled</span></span>|<span data-ttu-id="e2a11-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2a11-148">Boolean</span></span>|<span data-ttu-id="e2a11-149">网络检查系统是否已启用？</span><span class="sxs-lookup"><span data-stu-id="e2a11-149">Network inspection system enabled or not?</span></span>|
|<span data-ttu-id="e2a11-150">quickScanOverdue</span><span class="sxs-lookup"><span data-stu-id="e2a11-150">quickScanOverdue</span></span>|<span data-ttu-id="e2a11-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2a11-151">Boolean</span></span>|<span data-ttu-id="e2a11-152">快速扫描是否过期？</span><span class="sxs-lookup"><span data-stu-id="e2a11-152">Quick scan overdue or not?</span></span>|
|<span data-ttu-id="e2a11-153">fullScanOverdue</span><span class="sxs-lookup"><span data-stu-id="e2a11-153">fullScanOverdue</span></span>|<span data-ttu-id="e2a11-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2a11-154">Boolean</span></span>|<span data-ttu-id="e2a11-155">完全扫描是否过期？</span><span class="sxs-lookup"><span data-stu-id="e2a11-155">Full scan overdue or not?</span></span>|
|<span data-ttu-id="e2a11-156">signatureUpdateOverdue</span><span class="sxs-lookup"><span data-stu-id="e2a11-156">signatureUpdateOverdue</span></span>|<span data-ttu-id="e2a11-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2a11-157">Boolean</span></span>|<span data-ttu-id="e2a11-158">签名是否过期？</span><span class="sxs-lookup"><span data-stu-id="e2a11-158">Signature out of date or not?</span></span>|
|<span data-ttu-id="e2a11-159">rebootRequired</span><span class="sxs-lookup"><span data-stu-id="e2a11-159">rebootRequired</span></span>|<span data-ttu-id="e2a11-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2a11-160">Boolean</span></span>|<span data-ttu-id="e2a11-161">是否要求重新启动？</span><span class="sxs-lookup"><span data-stu-id="e2a11-161">Reboot required or not?</span></span>|
|<span data-ttu-id="e2a11-162">fullScanRequired</span><span class="sxs-lookup"><span data-stu-id="e2a11-162">fullScanRequired</span></span>|<span data-ttu-id="e2a11-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2a11-163">Boolean</span></span>|<span data-ttu-id="e2a11-164">是否要求进行完全扫描？</span><span class="sxs-lookup"><span data-stu-id="e2a11-164">Full scan required or not?</span></span>|
|<span data-ttu-id="e2a11-165">engineVersion</span><span class="sxs-lookup"><span data-stu-id="e2a11-165">engineVersion</span></span>|<span data-ttu-id="e2a11-166">String</span><span class="sxs-lookup"><span data-stu-id="e2a11-166">String</span></span>|<span data-ttu-id="e2a11-167">当前终结点保护引擎的版本</span><span class="sxs-lookup"><span data-stu-id="e2a11-167">Current endpoint protection engine's version</span></span>|
|<span data-ttu-id="e2a11-168">signatureVersion</span><span class="sxs-lookup"><span data-stu-id="e2a11-168">signatureVersion</span></span>|<span data-ttu-id="e2a11-169">String</span><span class="sxs-lookup"><span data-stu-id="e2a11-169">String</span></span>|<span data-ttu-id="e2a11-170">当前恶意软件定义版本</span><span class="sxs-lookup"><span data-stu-id="e2a11-170">Current malware definitions version</span></span>|
|<span data-ttu-id="e2a11-171">antiMalwareVersion</span><span class="sxs-lookup"><span data-stu-id="e2a11-171">antiMalwareVersion</span></span>|<span data-ttu-id="e2a11-172">String</span><span class="sxs-lookup"><span data-stu-id="e2a11-172">String</span></span>|<span data-ttu-id="e2a11-173">当前反恶意软件版本</span><span class="sxs-lookup"><span data-stu-id="e2a11-173">Current anti malware version</span></span>|
|<span data-ttu-id="e2a11-174">lastQuickScanDateTime</span><span class="sxs-lookup"><span data-stu-id="e2a11-174">lastQuickScanDateTime</span></span>|<span data-ttu-id="e2a11-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2a11-175">DateTimeOffset</span></span>|<span data-ttu-id="e2a11-176">上次快速扫描日期/时间</span><span class="sxs-lookup"><span data-stu-id="e2a11-176">Last quick scan datetime</span></span>|
|<span data-ttu-id="e2a11-177">lastFullScanDateTime</span><span class="sxs-lookup"><span data-stu-id="e2a11-177">lastFullScanDateTime</span></span>|<span data-ttu-id="e2a11-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2a11-178">DateTimeOffset</span></span>|<span data-ttu-id="e2a11-179">上次快速扫描日期/时间</span><span class="sxs-lookup"><span data-stu-id="e2a11-179">Last quick scan datetime</span></span>|
|<span data-ttu-id="e2a11-180">lastQuickScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="e2a11-180">lastQuickScanSignatureVersion</span></span>|<span data-ttu-id="e2a11-181">String</span><span class="sxs-lookup"><span data-stu-id="e2a11-181">String</span></span>|<span data-ttu-id="e2a11-182">上次快速扫描签名版本</span><span class="sxs-lookup"><span data-stu-id="e2a11-182">Last quick scan signature version</span></span>|
|<span data-ttu-id="e2a11-183">lastFullScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="e2a11-183">lastFullScanSignatureVersion</span></span>|<span data-ttu-id="e2a11-184">String</span><span class="sxs-lookup"><span data-stu-id="e2a11-184">String</span></span>|<span data-ttu-id="e2a11-185">上次完全扫描签名版本</span><span class="sxs-lookup"><span data-stu-id="e2a11-185">Last full scan signature version</span></span>|
|<span data-ttu-id="e2a11-186">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="e2a11-186">lastReportedDateTime</span></span>|<span data-ttu-id="e2a11-187">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2a11-187">DateTimeOffset</span></span>|<span data-ttu-id="e2a11-188">上次设备运行状况报告时间</span><span class="sxs-lookup"><span data-stu-id="e2a11-188">Last device health status reported time</span></span>|
|<span data-ttu-id="e2a11-189">productStatus</span><span class="sxs-lookup"><span data-stu-id="e2a11-189">productStatus</span></span>|[<span data-ttu-id="e2a11-190">windowsDefenderProductStatus</span><span class="sxs-lookup"><span data-stu-id="e2a11-190">windowsDefenderProductStatus</span></span>](../resources/intune-devices-windowsdefenderproductstatus.md)|<span data-ttu-id="e2a11-191">防病毒Windows Defender状态。</span><span class="sxs-lookup"><span data-stu-id="e2a11-191">Product Status of Windows Defender Antivirus.</span></span> <span data-ttu-id="e2a11-192">可能的值是 `noStatus` `serviceNotRunning` `serviceStartedWithoutMalwareProtection` ：、、、、、、、、、、 `pendingFullScanDueToThreatAction` `pendingRebootDueToThreatAction` `pendingManualStepsDueToThreatAction` `avSignaturesOutOfDate` `asSignaturesOutOfDate` `noQuickScanHappenedForSpecifiedPeriod` `noFullScanHappenedForSpecifiedPeriod` `systemInitiatedScanInProgress` `systemInitiatedCleanInProgress` `samplesPendingSubmission` `productRunningInEvaluationMode` `productRunningInNonGenuineMode` `productExpired` `offlineScanRequired` `serviceShutdownAsPartOfSystemShutdown` `threatRemediationFailedCritically` `threatRemediationFailedNonCritically` `noStatusFlagsSet` `platformOutOfDate` `platformUpdateInProgress` `platformAboutToBeOutdated` `signatureOrPlatformEndOfLifeIsPastOrIsImpending` `windowsSModeSignaturesInUseOnNonWin10SInstall` 、</span><span class="sxs-lookup"><span data-stu-id="e2a11-192">Possible values are: `noStatus`, `serviceNotRunning`, `serviceStartedWithoutMalwareProtection`, `pendingFullScanDueToThreatAction`, `pendingRebootDueToThreatAction`, `pendingManualStepsDueToThreatAction`, `avSignaturesOutOfDate`, `asSignaturesOutOfDate`, `noQuickScanHappenedForSpecifiedPeriod`, `noFullScanHappenedForSpecifiedPeriod`, `systemInitiatedScanInProgress`, `systemInitiatedCleanInProgress`, `samplesPendingSubmission`, `productRunningInEvaluationMode`, `productRunningInNonGenuineMode`, `productExpired`, `offlineScanRequired`, `serviceShutdownAsPartOfSystemShutdown`, `threatRemediationFailedCritically`, `threatRemediationFailedNonCritically`, `noStatusFlagsSet`, `platformOutOfDate`, `platformUpdateInProgress`, `platformAboutToBeOutdated`, `signatureOrPlatformEndOfLifeIsPastOrIsImpending`, `windowsSModeSignaturesInUseOnNonWin10SInstall`.</span></span>|
|<span data-ttu-id="e2a11-193">isVirtualMachine</span><span class="sxs-lookup"><span data-stu-id="e2a11-193">isVirtualMachine</span></span>|<span data-ttu-id="e2a11-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2a11-194">Boolean</span></span>|<span data-ttu-id="e2a11-195">指示设备是否是虚拟机。</span><span class="sxs-lookup"><span data-stu-id="e2a11-195">Indicates whether the device is a virtual machine.</span></span>|
|<span data-ttu-id="e2a11-196">tamperProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="e2a11-196">tamperProtectionEnabled</span></span>|<span data-ttu-id="e2a11-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2a11-197">Boolean</span></span>|<span data-ttu-id="e2a11-198">指示是否Windows Defender防篡改保护功能。</span><span class="sxs-lookup"><span data-stu-id="e2a11-198">Indicates whether the Windows Defender tamper protection feature is enabled.</span></span>|



## <a name="response"></a><span data-ttu-id="e2a11-199">响应</span><span class="sxs-lookup"><span data-stu-id="e2a11-199">Response</span></span>
<span data-ttu-id="e2a11-200">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e2a11-200">If successful, this method returns a `200 OK` response code and an updated [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2a11-201">示例</span><span class="sxs-lookup"><span data-stu-id="e2a11-201">Example</span></span>

### <a name="request"></a><span data-ttu-id="e2a11-202">请求</span><span class="sxs-lookup"><span data-stu-id="e2a11-202">Request</span></span>
<span data-ttu-id="e2a11-203">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e2a11-203">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/windowsProtectionState
Content-type: application/json
Content-length: 971

{
  "@odata.type": "#microsoft.graph.windowsProtectionState",
  "malwareProtectionEnabled": true,
  "deviceState": "fullScanPending",
  "realTimeProtectionEnabled": true,
  "networkInspectionSystemEnabled": true,
  "quickScanOverdue": true,
  "fullScanOverdue": true,
  "signatureUpdateOverdue": true,
  "rebootRequired": true,
  "fullScanRequired": true,
  "engineVersion": "Engine Version value",
  "signatureVersion": "Signature Version value",
  "antiMalwareVersion": "Anti Malware Version value",
  "lastQuickScanDateTime": "2016-12-31T23:58:27.5900669-08:00",
  "lastFullScanDateTime": "2017-01-01T00:01:44.9405639-08:00",
  "lastQuickScanSignatureVersion": "Last Quick Scan Signature Version value",
  "lastFullScanSignatureVersion": "Last Full Scan Signature Version value",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "productStatus": "serviceNotRunning",
  "isVirtualMachine": true,
  "tamperProtectionEnabled": true
}
```

### <a name="response"></a><span data-ttu-id="e2a11-204">响应</span><span class="sxs-lookup"><span data-stu-id="e2a11-204">Response</span></span>
<span data-ttu-id="e2a11-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e2a11-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1020

{
  "@odata.type": "#microsoft.graph.windowsProtectionState",
  "id": "1ac6ea5a-ea5a-1ac6-5aea-c61a5aeac61a",
  "malwareProtectionEnabled": true,
  "deviceState": "fullScanPending",
  "realTimeProtectionEnabled": true,
  "networkInspectionSystemEnabled": true,
  "quickScanOverdue": true,
  "fullScanOverdue": true,
  "signatureUpdateOverdue": true,
  "rebootRequired": true,
  "fullScanRequired": true,
  "engineVersion": "Engine Version value",
  "signatureVersion": "Signature Version value",
  "antiMalwareVersion": "Anti Malware Version value",
  "lastQuickScanDateTime": "2016-12-31T23:58:27.5900669-08:00",
  "lastFullScanDateTime": "2017-01-01T00:01:44.9405639-08:00",
  "lastQuickScanSignatureVersion": "Last Quick Scan Signature Version value",
  "lastFullScanSignatureVersion": "Last Full Scan Signature Version value",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "productStatus": "serviceNotRunning",
  "isVirtualMachine": true,
  "tamperProtectionEnabled": true
}
```




