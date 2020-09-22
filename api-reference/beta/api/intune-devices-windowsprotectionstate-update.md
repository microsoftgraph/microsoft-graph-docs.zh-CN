---
title: 更新 windowsProtectionState
description: 更新 windowsProtectionState 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 655a26c781dfa5badbd4c672579326e2a77079d0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48056084"
---
# <a name="update-windowsprotectionstate"></a><span data-ttu-id="3275f-103">更新 windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="3275f-103">Update windowsProtectionState</span></span>

<span data-ttu-id="3275f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3275f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3275f-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3275f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3275f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3275f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3275f-107">更新 [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="3275f-107">Update the properties of a [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3275f-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="3275f-108">Prerequisites</span></span>
<span data-ttu-id="3275f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3275f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3275f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="3275f-111">Permission type</span></span>|<span data-ttu-id="3275f-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3275f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3275f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3275f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3275f-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3275f-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="3275f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3275f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3275f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3275f-116">Not supported.</span></span>|
|<span data-ttu-id="3275f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="3275f-117">Application</span></span>|<span data-ttu-id="3275f-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3275f-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3275f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3275f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/windowsProtectionState
```

## <a name="request-headers"></a><span data-ttu-id="3275f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="3275f-120">Request headers</span></span>
|<span data-ttu-id="3275f-121">标头</span><span class="sxs-lookup"><span data-stu-id="3275f-121">Header</span></span>|<span data-ttu-id="3275f-122">值</span><span class="sxs-lookup"><span data-stu-id="3275f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3275f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3275f-123">Authorization</span></span>|<span data-ttu-id="3275f-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3275f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3275f-125">接受</span><span class="sxs-lookup"><span data-stu-id="3275f-125">Accept</span></span>|<span data-ttu-id="3275f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3275f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3275f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3275f-127">Request body</span></span>
<span data-ttu-id="3275f-128">在请求正文中，提供 [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3275f-128">In the request body, supply a JSON representation for the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>

<span data-ttu-id="3275f-129">下表显示创建 [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3275f-129">The following table shows the properties that are required when you create the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md).</span></span>

|<span data-ttu-id="3275f-130">属性</span><span class="sxs-lookup"><span data-stu-id="3275f-130">Property</span></span>|<span data-ttu-id="3275f-131">类型</span><span class="sxs-lookup"><span data-stu-id="3275f-131">Type</span></span>|<span data-ttu-id="3275f-132">说明</span><span class="sxs-lookup"><span data-stu-id="3275f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3275f-133">id</span><span class="sxs-lookup"><span data-stu-id="3275f-133">id</span></span>|<span data-ttu-id="3275f-134">String</span><span class="sxs-lookup"><span data-stu-id="3275f-134">String</span></span>|<span data-ttu-id="3275f-135">设备保护状态对象的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="3275f-135">The unique Identifier for the device protection status object.</span></span> <span data-ttu-id="3275f-136">这是设备的设备 id</span><span class="sxs-lookup"><span data-stu-id="3275f-136">This is device id of the device</span></span>|
|<span data-ttu-id="3275f-137">malwareProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="3275f-137">malwareProtectionEnabled</span></span>|<span data-ttu-id="3275f-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="3275f-138">Boolean</span></span>|<span data-ttu-id="3275f-139">已启用反恶意软件</span><span class="sxs-lookup"><span data-stu-id="3275f-139">Anti malware is enabled or not</span></span>|
|<span data-ttu-id="3275f-140">deviceState</span><span class="sxs-lookup"><span data-stu-id="3275f-140">deviceState</span></span>|[<span data-ttu-id="3275f-141">windowsDeviceHealthState</span><span class="sxs-lookup"><span data-stu-id="3275f-141">windowsDeviceHealthState</span></span>](../resources/intune-devices-windowsdevicehealthstate.md)|<span data-ttu-id="3275f-142">计算机的状态 (如干净或挂起的完全扫描或挂起的重新启动等) 。</span><span class="sxs-lookup"><span data-stu-id="3275f-142">Computer's state (like clean or pending full scan or pending reboot etc).</span></span> <span data-ttu-id="3275f-143">可取值为：`clean`、`fullScanPending`、`rebootPending`、`manualStepsPending`、`offlineScanPending`、`critical`。</span><span class="sxs-lookup"><span data-stu-id="3275f-143">Possible values are: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span></span>|
|<span data-ttu-id="3275f-144">realTimeProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="3275f-144">realTimeProtectionEnabled</span></span>|<span data-ttu-id="3275f-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="3275f-145">Boolean</span></span>|<span data-ttu-id="3275f-146">是否启用了实时保护？</span><span class="sxs-lookup"><span data-stu-id="3275f-146">Real time protection is enabled or not?</span></span>|
|<span data-ttu-id="3275f-147">networkInspectionSystemEnabled</span><span class="sxs-lookup"><span data-stu-id="3275f-147">networkInspectionSystemEnabled</span></span>|<span data-ttu-id="3275f-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="3275f-148">Boolean</span></span>|<span data-ttu-id="3275f-149">网络检查系统是否已启用？</span><span class="sxs-lookup"><span data-stu-id="3275f-149">Network inspection system enabled or not?</span></span>|
|<span data-ttu-id="3275f-150">quickScanOverdue</span><span class="sxs-lookup"><span data-stu-id="3275f-150">quickScanOverdue</span></span>|<span data-ttu-id="3275f-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="3275f-151">Boolean</span></span>|<span data-ttu-id="3275f-152">快速扫描是否过期？</span><span class="sxs-lookup"><span data-stu-id="3275f-152">Quick scan overdue or not?</span></span>|
|<span data-ttu-id="3275f-153">fullScanOverdue</span><span class="sxs-lookup"><span data-stu-id="3275f-153">fullScanOverdue</span></span>|<span data-ttu-id="3275f-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="3275f-154">Boolean</span></span>|<span data-ttu-id="3275f-155">完全扫描逾期？</span><span class="sxs-lookup"><span data-stu-id="3275f-155">Full scan overdue or not?</span></span>|
|<span data-ttu-id="3275f-156">signatureUpdateOverdue</span><span class="sxs-lookup"><span data-stu-id="3275f-156">signatureUpdateOverdue</span></span>|<span data-ttu-id="3275f-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="3275f-157">Boolean</span></span>|<span data-ttu-id="3275f-158">签名是否已过期？</span><span class="sxs-lookup"><span data-stu-id="3275f-158">Signature out of date or not?</span></span>|
|<span data-ttu-id="3275f-159">rebootRequired</span><span class="sxs-lookup"><span data-stu-id="3275f-159">rebootRequired</span></span>|<span data-ttu-id="3275f-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="3275f-160">Boolean</span></span>|<span data-ttu-id="3275f-161">是否需要重新启动？</span><span class="sxs-lookup"><span data-stu-id="3275f-161">Reboot required or not?</span></span>|
|<span data-ttu-id="3275f-162">fullScanRequired</span><span class="sxs-lookup"><span data-stu-id="3275f-162">fullScanRequired</span></span>|<span data-ttu-id="3275f-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="3275f-163">Boolean</span></span>|<span data-ttu-id="3275f-164">需要完全扫描吗？</span><span class="sxs-lookup"><span data-stu-id="3275f-164">Full scan required or not?</span></span>|
|<span data-ttu-id="3275f-165">engineVersion</span><span class="sxs-lookup"><span data-stu-id="3275f-165">engineVersion</span></span>|<span data-ttu-id="3275f-166">String</span><span class="sxs-lookup"><span data-stu-id="3275f-166">String</span></span>|<span data-ttu-id="3275f-167">当前 endpoint protection 引擎的版本</span><span class="sxs-lookup"><span data-stu-id="3275f-167">Current endpoint protection engine's version</span></span>|
|<span data-ttu-id="3275f-168">signatureVersion</span><span class="sxs-lookup"><span data-stu-id="3275f-168">signatureVersion</span></span>|<span data-ttu-id="3275f-169">String</span><span class="sxs-lookup"><span data-stu-id="3275f-169">String</span></span>|<span data-ttu-id="3275f-170">当前恶意软件定义版本</span><span class="sxs-lookup"><span data-stu-id="3275f-170">Current malware definitions version</span></span>|
|<span data-ttu-id="3275f-171">antiMalwareVersion</span><span class="sxs-lookup"><span data-stu-id="3275f-171">antiMalwareVersion</span></span>|<span data-ttu-id="3275f-172">String</span><span class="sxs-lookup"><span data-stu-id="3275f-172">String</span></span>|<span data-ttu-id="3275f-173">当前反恶意软件版本</span><span class="sxs-lookup"><span data-stu-id="3275f-173">Current anti malware version</span></span>|
|<span data-ttu-id="3275f-174">lastQuickScanDateTime</span><span class="sxs-lookup"><span data-stu-id="3275f-174">lastQuickScanDateTime</span></span>|<span data-ttu-id="3275f-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3275f-175">DateTimeOffset</span></span>|<span data-ttu-id="3275f-176">上次快速扫描日期时间</span><span class="sxs-lookup"><span data-stu-id="3275f-176">Last quick scan datetime</span></span>|
|<span data-ttu-id="3275f-177">lastFullScanDateTime</span><span class="sxs-lookup"><span data-stu-id="3275f-177">lastFullScanDateTime</span></span>|<span data-ttu-id="3275f-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3275f-178">DateTimeOffset</span></span>|<span data-ttu-id="3275f-179">上次快速扫描日期时间</span><span class="sxs-lookup"><span data-stu-id="3275f-179">Last quick scan datetime</span></span>|
|<span data-ttu-id="3275f-180">lastQuickScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="3275f-180">lastQuickScanSignatureVersion</span></span>|<span data-ttu-id="3275f-181">String</span><span class="sxs-lookup"><span data-stu-id="3275f-181">String</span></span>|<span data-ttu-id="3275f-182">上次快速扫描签名版本</span><span class="sxs-lookup"><span data-stu-id="3275f-182">Last quick scan signature version</span></span>|
|<span data-ttu-id="3275f-183">lastFullScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="3275f-183">lastFullScanSignatureVersion</span></span>|<span data-ttu-id="3275f-184">String</span><span class="sxs-lookup"><span data-stu-id="3275f-184">String</span></span>|<span data-ttu-id="3275f-185">上次完全扫描签名版本</span><span class="sxs-lookup"><span data-stu-id="3275f-185">Last full scan signature version</span></span>|
|<span data-ttu-id="3275f-186">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="3275f-186">lastReportedDateTime</span></span>|<span data-ttu-id="3275f-187">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3275f-187">DateTimeOffset</span></span>|<span data-ttu-id="3275f-188">上次设备运行状况状态报告时间</span><span class="sxs-lookup"><span data-stu-id="3275f-188">Last device health status reported time</span></span>|



## <a name="response"></a><span data-ttu-id="3275f-189">响应</span><span class="sxs-lookup"><span data-stu-id="3275f-189">Response</span></span>
<span data-ttu-id="3275f-190">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3275f-190">If successful, this method returns a `200 OK` response code and an updated [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3275f-191">示例</span><span class="sxs-lookup"><span data-stu-id="3275f-191">Example</span></span>

### <a name="request"></a><span data-ttu-id="3275f-192">请求</span><span class="sxs-lookup"><span data-stu-id="3275f-192">Request</span></span>
<span data-ttu-id="3275f-193">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3275f-193">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/windowsProtectionState
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

### <a name="response"></a><span data-ttu-id="3275f-194">响应</span><span class="sxs-lookup"><span data-stu-id="3275f-194">Response</span></span>
<span data-ttu-id="3275f-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3275f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






