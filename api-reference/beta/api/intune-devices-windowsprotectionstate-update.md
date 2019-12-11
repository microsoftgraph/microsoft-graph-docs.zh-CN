---
title: 更新 windowsProtectionState
description: 更新 windowsProtectionState 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4c64d51e88bc4e4bcff7baf5214f61e094b7ff53
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39944200"
---
# <a name="update-windowsprotectionstate"></a><span data-ttu-id="51091-103">更新 windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="51091-103">Update windowsProtectionState</span></span>

> <span data-ttu-id="51091-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="51091-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="51091-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="51091-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51091-106">更新[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="51091-106">Update the properties of a [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="51091-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="51091-107">Prerequisites</span></span>
<span data-ttu-id="51091-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="51091-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51091-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="51091-110">Permission type</span></span>|<span data-ttu-id="51091-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="51091-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51091-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="51091-112">Delegated (work or school account)</span></span>|<span data-ttu-id="51091-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51091-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="51091-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="51091-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51091-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="51091-115">Not supported.</span></span>|
|<span data-ttu-id="51091-116">Application</span><span class="sxs-lookup"><span data-stu-id="51091-116">Application</span></span>|<span data-ttu-id="51091-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51091-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="51091-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="51091-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsMalwareInformation/{windowsMalwareInformationId}/windowsDevicesProtectionState/{windowsProtectionStateId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/windowsProtectionState
```

## <a name="request-headers"></a><span data-ttu-id="51091-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="51091-119">Request headers</span></span>
|<span data-ttu-id="51091-120">标头</span><span class="sxs-lookup"><span data-stu-id="51091-120">Header</span></span>|<span data-ttu-id="51091-121">值</span><span class="sxs-lookup"><span data-stu-id="51091-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="51091-122">授权</span><span class="sxs-lookup"><span data-stu-id="51091-122">Authorization</span></span>|<span data-ttu-id="51091-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="51091-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="51091-124">接受</span><span class="sxs-lookup"><span data-stu-id="51091-124">Accept</span></span>|<span data-ttu-id="51091-125">application/json</span><span class="sxs-lookup"><span data-stu-id="51091-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="51091-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="51091-126">Request body</span></span>
<span data-ttu-id="51091-127">在请求正文中，提供[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="51091-127">In the request body, supply a JSON representation for the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>

<span data-ttu-id="51091-128">下表显示创建[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="51091-128">The following table shows the properties that are required when you create the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md).</span></span>

|<span data-ttu-id="51091-129">属性</span><span class="sxs-lookup"><span data-stu-id="51091-129">Property</span></span>|<span data-ttu-id="51091-130">类型</span><span class="sxs-lookup"><span data-stu-id="51091-130">Type</span></span>|<span data-ttu-id="51091-131">说明</span><span class="sxs-lookup"><span data-stu-id="51091-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51091-132">id</span><span class="sxs-lookup"><span data-stu-id="51091-132">id</span></span>|<span data-ttu-id="51091-133">字符串</span><span class="sxs-lookup"><span data-stu-id="51091-133">String</span></span>|<span data-ttu-id="51091-134">设备保护状态对象的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="51091-134">The unique Identifier for the device protection status object.</span></span> <span data-ttu-id="51091-135">这是设备的设备 id</span><span class="sxs-lookup"><span data-stu-id="51091-135">This is device id of the device</span></span>|
|<span data-ttu-id="51091-136">malwareProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="51091-136">malwareProtectionEnabled</span></span>|<span data-ttu-id="51091-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="51091-137">Boolean</span></span>|<span data-ttu-id="51091-138">已启用反恶意软件</span><span class="sxs-lookup"><span data-stu-id="51091-138">Anti malware is enabled or not</span></span>|
|<span data-ttu-id="51091-139">deviceState</span><span class="sxs-lookup"><span data-stu-id="51091-139">deviceState</span></span>|[<span data-ttu-id="51091-140">windowsDeviceHealthState</span><span class="sxs-lookup"><span data-stu-id="51091-140">windowsDeviceHealthState</span></span>](../resources/intune-devices-windowsdevicehealthstate.md)|<span data-ttu-id="51091-141">计算机的状态（如清理或挂起完全扫描或等待重新启动等）。</span><span class="sxs-lookup"><span data-stu-id="51091-141">Computer's state (like clean or pending full scan or pending reboot etc).</span></span> <span data-ttu-id="51091-142">可取值为：`clean`、`fullScanPending`、`rebootPending`、`manualStepsPending`、`offlineScanPending`、`critical`。</span><span class="sxs-lookup"><span data-stu-id="51091-142">Possible values are: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span></span>|
|<span data-ttu-id="51091-143">realTimeProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="51091-143">realTimeProtectionEnabled</span></span>|<span data-ttu-id="51091-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="51091-144">Boolean</span></span>|<span data-ttu-id="51091-145">是否启用了实时保护？</span><span class="sxs-lookup"><span data-stu-id="51091-145">Real time protection is enabled or not?</span></span>|
|<span data-ttu-id="51091-146">networkInspectionSystemEnabled</span><span class="sxs-lookup"><span data-stu-id="51091-146">networkInspectionSystemEnabled</span></span>|<span data-ttu-id="51091-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="51091-147">Boolean</span></span>|<span data-ttu-id="51091-148">网络检查系统是否已启用？</span><span class="sxs-lookup"><span data-stu-id="51091-148">Network inspection system enabled or not?</span></span>|
|<span data-ttu-id="51091-149">quickScanOverdue</span><span class="sxs-lookup"><span data-stu-id="51091-149">quickScanOverdue</span></span>|<span data-ttu-id="51091-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="51091-150">Boolean</span></span>|<span data-ttu-id="51091-151">快速扫描是否过期？</span><span class="sxs-lookup"><span data-stu-id="51091-151">Quick scan overdue or not?</span></span>|
|<span data-ttu-id="51091-152">fullScanOverdue</span><span class="sxs-lookup"><span data-stu-id="51091-152">fullScanOverdue</span></span>|<span data-ttu-id="51091-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="51091-153">Boolean</span></span>|<span data-ttu-id="51091-154">完全扫描逾期？</span><span class="sxs-lookup"><span data-stu-id="51091-154">Full scan overdue or not?</span></span>|
|<span data-ttu-id="51091-155">signatureUpdateOverdue</span><span class="sxs-lookup"><span data-stu-id="51091-155">signatureUpdateOverdue</span></span>|<span data-ttu-id="51091-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="51091-156">Boolean</span></span>|<span data-ttu-id="51091-157">签名是否已过期？</span><span class="sxs-lookup"><span data-stu-id="51091-157">Signature out of date or not?</span></span>|
|<span data-ttu-id="51091-158">rebootRequired</span><span class="sxs-lookup"><span data-stu-id="51091-158">rebootRequired</span></span>|<span data-ttu-id="51091-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="51091-159">Boolean</span></span>|<span data-ttu-id="51091-160">是否需要重新启动？</span><span class="sxs-lookup"><span data-stu-id="51091-160">Reboot required or not?</span></span>|
|<span data-ttu-id="51091-161">fullScanRequired</span><span class="sxs-lookup"><span data-stu-id="51091-161">fullScanRequired</span></span>|<span data-ttu-id="51091-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="51091-162">Boolean</span></span>|<span data-ttu-id="51091-163">需要完全扫描吗？</span><span class="sxs-lookup"><span data-stu-id="51091-163">Full scan required or not?</span></span>|
|<span data-ttu-id="51091-164">engineVersion</span><span class="sxs-lookup"><span data-stu-id="51091-164">engineVersion</span></span>|<span data-ttu-id="51091-165">字符串</span><span class="sxs-lookup"><span data-stu-id="51091-165">String</span></span>|<span data-ttu-id="51091-166">当前 endpoint protection 引擎的版本</span><span class="sxs-lookup"><span data-stu-id="51091-166">Current endpoint protection engine's version</span></span>|
|<span data-ttu-id="51091-167">signatureVersion</span><span class="sxs-lookup"><span data-stu-id="51091-167">signatureVersion</span></span>|<span data-ttu-id="51091-168">字符串</span><span class="sxs-lookup"><span data-stu-id="51091-168">String</span></span>|<span data-ttu-id="51091-169">当前恶意软件定义版本</span><span class="sxs-lookup"><span data-stu-id="51091-169">Current malware definitions version</span></span>|
|<span data-ttu-id="51091-170">antiMalwareVersion</span><span class="sxs-lookup"><span data-stu-id="51091-170">antiMalwareVersion</span></span>|<span data-ttu-id="51091-171">字符串</span><span class="sxs-lookup"><span data-stu-id="51091-171">String</span></span>|<span data-ttu-id="51091-172">当前反恶意软件版本</span><span class="sxs-lookup"><span data-stu-id="51091-172">Current anti malware version</span></span>|
|<span data-ttu-id="51091-173">lastQuickScanDateTime</span><span class="sxs-lookup"><span data-stu-id="51091-173">lastQuickScanDateTime</span></span>|<span data-ttu-id="51091-174">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51091-174">DateTimeOffset</span></span>|<span data-ttu-id="51091-175">上次快速扫描日期时间</span><span class="sxs-lookup"><span data-stu-id="51091-175">Last quick scan datetime</span></span>|
|<span data-ttu-id="51091-176">lastFullScanDateTime</span><span class="sxs-lookup"><span data-stu-id="51091-176">lastFullScanDateTime</span></span>|<span data-ttu-id="51091-177">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51091-177">DateTimeOffset</span></span>|<span data-ttu-id="51091-178">上次快速扫描日期时间</span><span class="sxs-lookup"><span data-stu-id="51091-178">Last quick scan datetime</span></span>|
|<span data-ttu-id="51091-179">lastQuickScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="51091-179">lastQuickScanSignatureVersion</span></span>|<span data-ttu-id="51091-180">字符串</span><span class="sxs-lookup"><span data-stu-id="51091-180">String</span></span>|<span data-ttu-id="51091-181">上次快速扫描签名版本</span><span class="sxs-lookup"><span data-stu-id="51091-181">Last quick scan signature version</span></span>|
|<span data-ttu-id="51091-182">lastFullScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="51091-182">lastFullScanSignatureVersion</span></span>|<span data-ttu-id="51091-183">字符串</span><span class="sxs-lookup"><span data-stu-id="51091-183">String</span></span>|<span data-ttu-id="51091-184">上次完全扫描签名版本</span><span class="sxs-lookup"><span data-stu-id="51091-184">Last full scan signature version</span></span>|
|<span data-ttu-id="51091-185">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="51091-185">lastReportedDateTime</span></span>|<span data-ttu-id="51091-186">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51091-186">DateTimeOffset</span></span>|<span data-ttu-id="51091-187">上次设备运行状况状态报告时间</span><span class="sxs-lookup"><span data-stu-id="51091-187">Last device health status reported time</span></span>|



## <a name="response"></a><span data-ttu-id="51091-188">响应</span><span class="sxs-lookup"><span data-stu-id="51091-188">Response</span></span>
<span data-ttu-id="51091-189">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="51091-189">If successful, this method returns a `200 OK` response code and an updated [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51091-190">示例</span><span class="sxs-lookup"><span data-stu-id="51091-190">Example</span></span>

### <a name="request"></a><span data-ttu-id="51091-191">请求</span><span class="sxs-lookup"><span data-stu-id="51091-191">Request</span></span>
<span data-ttu-id="51091-192">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="51091-192">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="51091-193">响应</span><span class="sxs-lookup"><span data-stu-id="51091-193">Response</span></span>
<span data-ttu-id="51091-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="51091-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





