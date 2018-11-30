---
title: 更新 windowsProtectionState
description: 更新 windowsProtectionState 对象的属性。
ms.openlocfilehash: f1323baa9a6611e5f6057456fbbefbaddefa626e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046886"
---
# <a name="update-windowsprotectionstate"></a><span data-ttu-id="3f2e8-103">更新 windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="3f2e8-103">Update windowsProtectionState</span></span>

> <span data-ttu-id="3f2e8-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="3f2e8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3f2e8-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="3f2e8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3f2e8-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="3f2e8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3f2e8-107">更新[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="3f2e8-107">Update the properties of a [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3f2e8-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="3f2e8-108">Prerequisites</span></span>
<span data-ttu-id="3f2e8-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="3f2e8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3f2e8-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="3f2e8-111">Permission type</span></span>|<span data-ttu-id="3f2e8-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3f2e8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3f2e8-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3f2e8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3f2e8-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f2e8-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="3f2e8-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3f2e8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3f2e8-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3f2e8-116">Not supported.</span></span>|
|<span data-ttu-id="3f2e8-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="3f2e8-117">Application</span></span>|<span data-ttu-id="3f2e8-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="3f2e8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3f2e8-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3f2e8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsMalwareInformation/{windowsMalwareInformationId}/windowsDevicesProtectionState/{windowsProtectionStateId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/windowsProtectionState
```

## <a name="request-headers"></a><span data-ttu-id="3f2e8-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="3f2e8-120">Request headers</span></span>
|<span data-ttu-id="3f2e8-121">标头</span><span class="sxs-lookup"><span data-stu-id="3f2e8-121">Header</span></span>|<span data-ttu-id="3f2e8-122">值</span><span class="sxs-lookup"><span data-stu-id="3f2e8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3f2e8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3f2e8-123">Authorization</span></span>|<span data-ttu-id="3f2e8-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3f2e8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3f2e8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3f2e8-125">Accept</span></span>|<span data-ttu-id="3f2e8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3f2e8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3f2e8-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3f2e8-127">Request body</span></span>
<span data-ttu-id="3f2e8-128">在请求正文中，提供[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3f2e8-128">In the request body, supply a JSON representation for the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>

<span data-ttu-id="3f2e8-129">下表显示时创建[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3f2e8-129">The following table shows the properties that are required when you create the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md).</span></span>

|<span data-ttu-id="3f2e8-130">属性</span><span class="sxs-lookup"><span data-stu-id="3f2e8-130">Property</span></span>|<span data-ttu-id="3f2e8-131">类型</span><span class="sxs-lookup"><span data-stu-id="3f2e8-131">Type</span></span>|<span data-ttu-id="3f2e8-132">说明</span><span class="sxs-lookup"><span data-stu-id="3f2e8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f2e8-133">id</span><span class="sxs-lookup"><span data-stu-id="3f2e8-133">id</span></span>|<span data-ttu-id="3f2e8-134">字符串</span><span class="sxs-lookup"><span data-stu-id="3f2e8-134">String</span></span>|<span data-ttu-id="3f2e8-135">设备保护状态对象的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="3f2e8-135">The unique Identifier for the device protection status object.</span></span> <span data-ttu-id="3f2e8-136">这是设备的设备 id</span><span class="sxs-lookup"><span data-stu-id="3f2e8-136">This is device id of the device</span></span>|
|<span data-ttu-id="3f2e8-137">malwareProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="3f2e8-137">malwareProtectionEnabled</span></span>|<span data-ttu-id="3f2e8-138">布尔</span><span class="sxs-lookup"><span data-stu-id="3f2e8-138">Boolean</span></span>|<span data-ttu-id="3f2e8-139">反恶意软件被启用还是没有</span><span class="sxs-lookup"><span data-stu-id="3f2e8-139">Anti malware is enabled or not</span></span>|
|<span data-ttu-id="3f2e8-140">deviceState</span><span class="sxs-lookup"><span data-stu-id="3f2e8-140">deviceState</span></span>|[<span data-ttu-id="3f2e8-141">windowsDeviceHealthState</span><span class="sxs-lookup"><span data-stu-id="3f2e8-141">windowsDeviceHealthState</span></span>](../resources/intune-devices-windowsdevicehealthstate.md)|<span data-ttu-id="3f2e8-142">计算机的状态 （如清理挂起完全扫描或挂起的重新启动等）。</span><span class="sxs-lookup"><span data-stu-id="3f2e8-142">Computer's state (like clean or pending full scan or pending reboot etc).</span></span> <span data-ttu-id="3f2e8-143">可取值为：`clean`、`fullScanPending`、`rebootPending`、`manualStepsPending`、`offlineScanPending`、`critical`。</span><span class="sxs-lookup"><span data-stu-id="3f2e8-143">Possible values are: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span></span>|
|<span data-ttu-id="3f2e8-144">realTimeProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="3f2e8-144">realTimeProtectionEnabled</span></span>|<span data-ttu-id="3f2e8-145">布尔</span><span class="sxs-lookup"><span data-stu-id="3f2e8-145">Boolean</span></span>|<span data-ttu-id="3f2e8-146">是否启用实时保护？</span><span class="sxs-lookup"><span data-stu-id="3f2e8-146">Real time protection is enabled or not?</span></span>|
|<span data-ttu-id="3f2e8-147">networkInspectionSystemEnabled</span><span class="sxs-lookup"><span data-stu-id="3f2e8-147">networkInspectionSystemEnabled</span></span>|<span data-ttu-id="3f2e8-148">布尔</span><span class="sxs-lookup"><span data-stu-id="3f2e8-148">Boolean</span></span>|<span data-ttu-id="3f2e8-149">启用或不网络检查系统？</span><span class="sxs-lookup"><span data-stu-id="3f2e8-149">Network inspection system enabled or not?</span></span>|
|<span data-ttu-id="3f2e8-150">quickScanOverdue</span><span class="sxs-lookup"><span data-stu-id="3f2e8-150">quickScanOverdue</span></span>|<span data-ttu-id="3f2e8-151">布尔</span><span class="sxs-lookup"><span data-stu-id="3f2e8-151">Boolean</span></span>|<span data-ttu-id="3f2e8-152">快速扫描过期，或不？</span><span class="sxs-lookup"><span data-stu-id="3f2e8-152">Quick scan overdue or not?</span></span>|
|<span data-ttu-id="3f2e8-153">fullScanOverdue</span><span class="sxs-lookup"><span data-stu-id="3f2e8-153">fullScanOverdue</span></span>|<span data-ttu-id="3f2e8-154">布尔</span><span class="sxs-lookup"><span data-stu-id="3f2e8-154">Boolean</span></span>|<span data-ttu-id="3f2e8-155">或不完全扫描过期？</span><span class="sxs-lookup"><span data-stu-id="3f2e8-155">Full scan overdue or not?</span></span>|
|<span data-ttu-id="3f2e8-156">signatureUpdateOverdue</span><span class="sxs-lookup"><span data-stu-id="3f2e8-156">signatureUpdateOverdue</span></span>|<span data-ttu-id="3f2e8-157">布尔</span><span class="sxs-lookup"><span data-stu-id="3f2e8-157">Boolean</span></span>|<span data-ttu-id="3f2e8-158">过期的签名或不？</span><span class="sxs-lookup"><span data-stu-id="3f2e8-158">Signature out of date or not?</span></span>|
|<span data-ttu-id="3f2e8-159">rebootRequired</span><span class="sxs-lookup"><span data-stu-id="3f2e8-159">rebootRequired</span></span>|<span data-ttu-id="3f2e8-160">布尔</span><span class="sxs-lookup"><span data-stu-id="3f2e8-160">Boolean</span></span>|<span data-ttu-id="3f2e8-161">需要或不重新启动？</span><span class="sxs-lookup"><span data-stu-id="3f2e8-161">Reboot required or not?</span></span>|
|<span data-ttu-id="3f2e8-162">fullScanRequired</span><span class="sxs-lookup"><span data-stu-id="3f2e8-162">fullScanRequired</span></span>|<span data-ttu-id="3f2e8-163">布尔</span><span class="sxs-lookup"><span data-stu-id="3f2e8-163">Boolean</span></span>|<span data-ttu-id="3f2e8-164">所需或不完全扫描？</span><span class="sxs-lookup"><span data-stu-id="3f2e8-164">Full scan required or not?</span></span>|
|<span data-ttu-id="3f2e8-165">engineVersion</span><span class="sxs-lookup"><span data-stu-id="3f2e8-165">engineVersion</span></span>|<span data-ttu-id="3f2e8-166">字符串</span><span class="sxs-lookup"><span data-stu-id="3f2e8-166">String</span></span>|<span data-ttu-id="3f2e8-167">当前终结点保护引擎的版本</span><span class="sxs-lookup"><span data-stu-id="3f2e8-167">Current endpoint protection engine's version</span></span>|
|<span data-ttu-id="3f2e8-168">特征码版本</span><span class="sxs-lookup"><span data-stu-id="3f2e8-168">signatureVersion</span></span>|<span data-ttu-id="3f2e8-169">字符串</span><span class="sxs-lookup"><span data-stu-id="3f2e8-169">String</span></span>|<span data-ttu-id="3f2e8-170">当前的恶意软件定义版本</span><span class="sxs-lookup"><span data-stu-id="3f2e8-170">Current malware definitions version</span></span>|
|<span data-ttu-id="3f2e8-171">antiMalwareVersion</span><span class="sxs-lookup"><span data-stu-id="3f2e8-171">antiMalwareVersion</span></span>|<span data-ttu-id="3f2e8-172">字符串</span><span class="sxs-lookup"><span data-stu-id="3f2e8-172">String</span></span>|<span data-ttu-id="3f2e8-173">当前防恶意软件版本</span><span class="sxs-lookup"><span data-stu-id="3f2e8-173">Current anti malware version</span></span>|
|<span data-ttu-id="3f2e8-174">lastQuickScanDateTime</span><span class="sxs-lookup"><span data-stu-id="3f2e8-174">lastQuickScanDateTime</span></span>|<span data-ttu-id="3f2e8-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3f2e8-175">DateTimeOffset</span></span>|<span data-ttu-id="3f2e8-176">最后一个快速扫描 datetime</span><span class="sxs-lookup"><span data-stu-id="3f2e8-176">Last quick scan datetime</span></span>|
|<span data-ttu-id="3f2e8-177">lastFullScanDateTime</span><span class="sxs-lookup"><span data-stu-id="3f2e8-177">lastFullScanDateTime</span></span>|<span data-ttu-id="3f2e8-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3f2e8-178">DateTimeOffset</span></span>|<span data-ttu-id="3f2e8-179">最后一个快速扫描 datetime</span><span class="sxs-lookup"><span data-stu-id="3f2e8-179">Last quick scan datetime</span></span>|
|<span data-ttu-id="3f2e8-180">lastQuickScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="3f2e8-180">lastQuickScanSignatureVersion</span></span>|<span data-ttu-id="3f2e8-181">字符串</span><span class="sxs-lookup"><span data-stu-id="3f2e8-181">String</span></span>|<span data-ttu-id="3f2e8-182">最后一个快速扫描病毒特征版本</span><span class="sxs-lookup"><span data-stu-id="3f2e8-182">Last quick scan signature version</span></span>|
|<span data-ttu-id="3f2e8-183">lastFullScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="3f2e8-183">lastFullScanSignatureVersion</span></span>|<span data-ttu-id="3f2e8-184">字符串</span><span class="sxs-lookup"><span data-stu-id="3f2e8-184">String</span></span>|<span data-ttu-id="3f2e8-185">最后一个完全扫描病毒特征版本</span><span class="sxs-lookup"><span data-stu-id="3f2e8-185">Last full scan signature version</span></span>|
|<span data-ttu-id="3f2e8-186">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="3f2e8-186">lastReportedDateTime</span></span>|<span data-ttu-id="3f2e8-187">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3f2e8-187">DateTimeOffset</span></span>|<span data-ttu-id="3f2e8-188">最后一个设备运行状况状态报告的时间</span><span class="sxs-lookup"><span data-stu-id="3f2e8-188">Last device health status reported time</span></span>|



## <a name="response"></a><span data-ttu-id="3f2e8-189">响应</span><span class="sxs-lookup"><span data-stu-id="3f2e8-189">Response</span></span>
<span data-ttu-id="3f2e8-190">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="3f2e8-190">If successful, this method returns a `200 OK` response code and an updated [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3f2e8-191">示例</span><span class="sxs-lookup"><span data-stu-id="3f2e8-191">Example</span></span>
### <a name="request"></a><span data-ttu-id="3f2e8-192">请求</span><span class="sxs-lookup"><span data-stu-id="3f2e8-192">Request</span></span>
<span data-ttu-id="3f2e8-193">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3f2e8-193">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsMalwareInformation/{windowsMalwareInformationId}/windowsDevicesProtectionState/{windowsProtectionStateId}
Content-type: application/json
Content-length: 804

{
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

### <a name="response"></a><span data-ttu-id="3f2e8-194">响应</span><span class="sxs-lookup"><span data-stu-id="3f2e8-194">Response</span></span>
<span data-ttu-id="3f2e8-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3f2e8-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





