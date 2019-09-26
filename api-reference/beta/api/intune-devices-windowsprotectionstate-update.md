---
title: 更新 windowsProtectionState
description: 更新 windowsProtectionState 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 74824bbc5c066d0e3df398786e5163642b64707a
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37187981"
---
# <a name="update-windowsprotectionstate"></a><span data-ttu-id="6b79e-103">更新 windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="6b79e-103">Update windowsProtectionState</span></span>

> <span data-ttu-id="6b79e-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6b79e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6b79e-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6b79e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6b79e-106">更新[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6b79e-106">Update the properties of a [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6b79e-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="6b79e-107">Prerequisites</span></span>
<span data-ttu-id="6b79e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6b79e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b79e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="6b79e-110">Permission type</span></span>|<span data-ttu-id="6b79e-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6b79e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6b79e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6b79e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6b79e-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b79e-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="6b79e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6b79e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6b79e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6b79e-115">Not supported.</span></span>|
|<span data-ttu-id="6b79e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="6b79e-116">Application</span></span>|<span data-ttu-id="6b79e-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b79e-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6b79e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6b79e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsMalwareInformation/{windowsMalwareInformationId}/windowsDevicesProtectionState/{windowsProtectionStateId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/windowsProtectionState
```

## <a name="request-headers"></a><span data-ttu-id="6b79e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="6b79e-119">Request headers</span></span>
|<span data-ttu-id="6b79e-120">标头</span><span class="sxs-lookup"><span data-stu-id="6b79e-120">Header</span></span>|<span data-ttu-id="6b79e-121">值</span><span class="sxs-lookup"><span data-stu-id="6b79e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6b79e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6b79e-122">Authorization</span></span>|<span data-ttu-id="6b79e-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6b79e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6b79e-124">接受</span><span class="sxs-lookup"><span data-stu-id="6b79e-124">Accept</span></span>|<span data-ttu-id="6b79e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6b79e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6b79e-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="6b79e-126">Request body</span></span>
<span data-ttu-id="6b79e-127">在请求正文中，提供[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6b79e-127">In the request body, supply a JSON representation for the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>

<span data-ttu-id="6b79e-128">下表显示创建[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6b79e-128">The following table shows the properties that are required when you create the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md).</span></span>

|<span data-ttu-id="6b79e-129">属性</span><span class="sxs-lookup"><span data-stu-id="6b79e-129">Property</span></span>|<span data-ttu-id="6b79e-130">类型</span><span class="sxs-lookup"><span data-stu-id="6b79e-130">Type</span></span>|<span data-ttu-id="6b79e-131">说明</span><span class="sxs-lookup"><span data-stu-id="6b79e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b79e-132">id</span><span class="sxs-lookup"><span data-stu-id="6b79e-132">id</span></span>|<span data-ttu-id="6b79e-133">String</span><span class="sxs-lookup"><span data-stu-id="6b79e-133">String</span></span>|<span data-ttu-id="6b79e-134">设备保护状态对象的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="6b79e-134">The unique Identifier for the device protection status object.</span></span> <span data-ttu-id="6b79e-135">这是设备的设备 id</span><span class="sxs-lookup"><span data-stu-id="6b79e-135">This is device id of the device</span></span>|
|<span data-ttu-id="6b79e-136">malwareProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="6b79e-136">malwareProtectionEnabled</span></span>|<span data-ttu-id="6b79e-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b79e-137">Boolean</span></span>|<span data-ttu-id="6b79e-138">已启用反恶意软件</span><span class="sxs-lookup"><span data-stu-id="6b79e-138">Anti malware is enabled or not</span></span>|
|<span data-ttu-id="6b79e-139">deviceState</span><span class="sxs-lookup"><span data-stu-id="6b79e-139">deviceState</span></span>|[<span data-ttu-id="6b79e-140">windowsDeviceHealthState</span><span class="sxs-lookup"><span data-stu-id="6b79e-140">windowsDeviceHealthState</span></span>](../resources/intune-devices-windowsdevicehealthstate.md)|<span data-ttu-id="6b79e-141">计算机的状态（如清理或挂起完全扫描或等待重新启动等）。</span><span class="sxs-lookup"><span data-stu-id="6b79e-141">Computer's state (like clean or pending full scan or pending reboot etc).</span></span> <span data-ttu-id="6b79e-142">可取值为：`clean`、`fullScanPending`、`rebootPending`、`manualStepsPending`、`offlineScanPending`、`critical`。</span><span class="sxs-lookup"><span data-stu-id="6b79e-142">Possible values are: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span></span>|
|<span data-ttu-id="6b79e-143">realTimeProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="6b79e-143">realTimeProtectionEnabled</span></span>|<span data-ttu-id="6b79e-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b79e-144">Boolean</span></span>|<span data-ttu-id="6b79e-145">是否启用了实时保护？</span><span class="sxs-lookup"><span data-stu-id="6b79e-145">Real time protection is enabled or not?</span></span>|
|<span data-ttu-id="6b79e-146">networkInspectionSystemEnabled</span><span class="sxs-lookup"><span data-stu-id="6b79e-146">networkInspectionSystemEnabled</span></span>|<span data-ttu-id="6b79e-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b79e-147">Boolean</span></span>|<span data-ttu-id="6b79e-148">网络检查系统是否已启用？</span><span class="sxs-lookup"><span data-stu-id="6b79e-148">Network inspection system enabled or not?</span></span>|
|<span data-ttu-id="6b79e-149">quickScanOverdue</span><span class="sxs-lookup"><span data-stu-id="6b79e-149">quickScanOverdue</span></span>|<span data-ttu-id="6b79e-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b79e-150">Boolean</span></span>|<span data-ttu-id="6b79e-151">快速扫描是否过期？</span><span class="sxs-lookup"><span data-stu-id="6b79e-151">Quick scan overdue or not?</span></span>|
|<span data-ttu-id="6b79e-152">fullScanOverdue</span><span class="sxs-lookup"><span data-stu-id="6b79e-152">fullScanOverdue</span></span>|<span data-ttu-id="6b79e-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b79e-153">Boolean</span></span>|<span data-ttu-id="6b79e-154">完全扫描逾期？</span><span class="sxs-lookup"><span data-stu-id="6b79e-154">Full scan overdue or not?</span></span>|
|<span data-ttu-id="6b79e-155">signatureUpdateOverdue</span><span class="sxs-lookup"><span data-stu-id="6b79e-155">signatureUpdateOverdue</span></span>|<span data-ttu-id="6b79e-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b79e-156">Boolean</span></span>|<span data-ttu-id="6b79e-157">签名是否已过期？</span><span class="sxs-lookup"><span data-stu-id="6b79e-157">Signature out of date or not?</span></span>|
|<span data-ttu-id="6b79e-158">rebootRequired</span><span class="sxs-lookup"><span data-stu-id="6b79e-158">rebootRequired</span></span>|<span data-ttu-id="6b79e-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b79e-159">Boolean</span></span>|<span data-ttu-id="6b79e-160">是否需要重新启动？</span><span class="sxs-lookup"><span data-stu-id="6b79e-160">Reboot required or not?</span></span>|
|<span data-ttu-id="6b79e-161">fullScanRequired</span><span class="sxs-lookup"><span data-stu-id="6b79e-161">fullScanRequired</span></span>|<span data-ttu-id="6b79e-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b79e-162">Boolean</span></span>|<span data-ttu-id="6b79e-163">需要完全扫描吗？</span><span class="sxs-lookup"><span data-stu-id="6b79e-163">Full scan required or not?</span></span>|
|<span data-ttu-id="6b79e-164">engineVersion</span><span class="sxs-lookup"><span data-stu-id="6b79e-164">engineVersion</span></span>|<span data-ttu-id="6b79e-165">String</span><span class="sxs-lookup"><span data-stu-id="6b79e-165">String</span></span>|<span data-ttu-id="6b79e-166">当前 endpoint protection 引擎的版本</span><span class="sxs-lookup"><span data-stu-id="6b79e-166">Current endpoint protection engine's version</span></span>|
|<span data-ttu-id="6b79e-167">signatureVersion</span><span class="sxs-lookup"><span data-stu-id="6b79e-167">signatureVersion</span></span>|<span data-ttu-id="6b79e-168">String</span><span class="sxs-lookup"><span data-stu-id="6b79e-168">String</span></span>|<span data-ttu-id="6b79e-169">当前恶意软件定义版本</span><span class="sxs-lookup"><span data-stu-id="6b79e-169">Current malware definitions version</span></span>|
|<span data-ttu-id="6b79e-170">antiMalwareVersion</span><span class="sxs-lookup"><span data-stu-id="6b79e-170">antiMalwareVersion</span></span>|<span data-ttu-id="6b79e-171">String</span><span class="sxs-lookup"><span data-stu-id="6b79e-171">String</span></span>|<span data-ttu-id="6b79e-172">当前反恶意软件版本</span><span class="sxs-lookup"><span data-stu-id="6b79e-172">Current anti malware version</span></span>|
|<span data-ttu-id="6b79e-173">lastQuickScanDateTime</span><span class="sxs-lookup"><span data-stu-id="6b79e-173">lastQuickScanDateTime</span></span>|<span data-ttu-id="6b79e-174">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6b79e-174">DateTimeOffset</span></span>|<span data-ttu-id="6b79e-175">上次快速扫描日期时间</span><span class="sxs-lookup"><span data-stu-id="6b79e-175">Last quick scan datetime</span></span>|
|<span data-ttu-id="6b79e-176">lastFullScanDateTime</span><span class="sxs-lookup"><span data-stu-id="6b79e-176">lastFullScanDateTime</span></span>|<span data-ttu-id="6b79e-177">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6b79e-177">DateTimeOffset</span></span>|<span data-ttu-id="6b79e-178">上次快速扫描日期时间</span><span class="sxs-lookup"><span data-stu-id="6b79e-178">Last quick scan datetime</span></span>|
|<span data-ttu-id="6b79e-179">lastQuickScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="6b79e-179">lastQuickScanSignatureVersion</span></span>|<span data-ttu-id="6b79e-180">String</span><span class="sxs-lookup"><span data-stu-id="6b79e-180">String</span></span>|<span data-ttu-id="6b79e-181">上次快速扫描签名版本</span><span class="sxs-lookup"><span data-stu-id="6b79e-181">Last quick scan signature version</span></span>|
|<span data-ttu-id="6b79e-182">lastFullScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="6b79e-182">lastFullScanSignatureVersion</span></span>|<span data-ttu-id="6b79e-183">String</span><span class="sxs-lookup"><span data-stu-id="6b79e-183">String</span></span>|<span data-ttu-id="6b79e-184">上次完全扫描签名版本</span><span class="sxs-lookup"><span data-stu-id="6b79e-184">Last full scan signature version</span></span>|
|<span data-ttu-id="6b79e-185">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="6b79e-185">lastReportedDateTime</span></span>|<span data-ttu-id="6b79e-186">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6b79e-186">DateTimeOffset</span></span>|<span data-ttu-id="6b79e-187">上次设备运行状况状态报告时间</span><span class="sxs-lookup"><span data-stu-id="6b79e-187">Last device health status reported time</span></span>|



## <a name="response"></a><span data-ttu-id="6b79e-188">响应</span><span class="sxs-lookup"><span data-stu-id="6b79e-188">Response</span></span>
<span data-ttu-id="6b79e-189">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6b79e-189">If successful, this method returns a `200 OK` response code and an updated [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b79e-190">示例</span><span class="sxs-lookup"><span data-stu-id="6b79e-190">Example</span></span>

### <a name="request"></a><span data-ttu-id="6b79e-191">请求</span><span class="sxs-lookup"><span data-stu-id="6b79e-191">Request</span></span>
<span data-ttu-id="6b79e-192">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6b79e-192">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsMalwareInformation/{windowsMalwareInformationId}/windowsDevicesProtectionState/{windowsProtectionStateId}
Content-type: application/json
Content-length: 865

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
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00"
}
```

### <a name="response"></a><span data-ttu-id="6b79e-193">响应</span><span class="sxs-lookup"><span data-stu-id="6b79e-193">Response</span></span>
<span data-ttu-id="6b79e-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6b79e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 914

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
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00"
}
```




