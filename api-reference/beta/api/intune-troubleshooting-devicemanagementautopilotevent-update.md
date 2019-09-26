---
title: 更新 deviceManagementAutopilotEvent
description: 更新 deviceManagementAutopilotEvent 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fb5d7c7cd07f29715639c61ca5c877e802cdbd0b
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37199807"
---
# <a name="update-devicemanagementautopilotevent"></a><span data-ttu-id="c5970-103">更新 deviceManagementAutopilotEvent</span><span class="sxs-lookup"><span data-stu-id="c5970-103">Update deviceManagementAutopilotEvent</span></span>

> <span data-ttu-id="c5970-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c5970-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c5970-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c5970-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5970-106">更新[deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c5970-106">Update the properties of a [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c5970-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="c5970-107">Prerequisites</span></span>
<span data-ttu-id="c5970-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c5970-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5970-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c5970-110">Permission type</span></span>|<span data-ttu-id="c5970-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c5970-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c5970-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c5970-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c5970-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5970-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="c5970-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c5970-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c5970-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c5970-115">Not supported.</span></span>|
|<span data-ttu-id="c5970-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c5970-116">Application</span></span>|<span data-ttu-id="c5970-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5970-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c5970-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c5970-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/autopilotEvents/{deviceManagementAutopilotEventId}
```

## <a name="request-headers"></a><span data-ttu-id="c5970-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c5970-119">Request headers</span></span>
|<span data-ttu-id="c5970-120">标头</span><span class="sxs-lookup"><span data-stu-id="c5970-120">Header</span></span>|<span data-ttu-id="c5970-121">值</span><span class="sxs-lookup"><span data-stu-id="c5970-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c5970-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c5970-122">Authorization</span></span>|<span data-ttu-id="c5970-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c5970-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c5970-124">接受</span><span class="sxs-lookup"><span data-stu-id="c5970-124">Accept</span></span>|<span data-ttu-id="c5970-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c5970-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5970-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c5970-126">Request body</span></span>
<span data-ttu-id="c5970-127">在请求正文中，提供[deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c5970-127">In the request body, supply a JSON representation for the [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) object.</span></span>

<span data-ttu-id="c5970-128">下表显示创建[deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c5970-128">The following table shows the properties that are required when you create the [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md).</span></span>

|<span data-ttu-id="c5970-129">属性</span><span class="sxs-lookup"><span data-stu-id="c5970-129">Property</span></span>|<span data-ttu-id="c5970-130">类型</span><span class="sxs-lookup"><span data-stu-id="c5970-130">Type</span></span>|<span data-ttu-id="c5970-131">说明</span><span class="sxs-lookup"><span data-stu-id="c5970-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5970-132">id</span><span class="sxs-lookup"><span data-stu-id="c5970-132">id</span></span>|<span data-ttu-id="c5970-133">String</span><span class="sxs-lookup"><span data-stu-id="c5970-133">String</span></span>|<span data-ttu-id="c5970-134">对象的 UUID</span><span class="sxs-lookup"><span data-stu-id="c5970-134">UUID for the object</span></span>|
|<span data-ttu-id="c5970-135">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="c5970-135">eventDateTime</span></span>|<span data-ttu-id="c5970-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5970-136">DateTimeOffset</span></span>|<span data-ttu-id="c5970-137">事件发生的时间。</span><span class="sxs-lookup"><span data-stu-id="c5970-137">Time when the event occurred .</span></span>|
|<span data-ttu-id="c5970-138">deviceRegisteredDateTime</span><span class="sxs-lookup"><span data-stu-id="c5970-138">deviceRegisteredDateTime</span></span>|<span data-ttu-id="c5970-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5970-139">DateTimeOffset</span></span>|<span data-ttu-id="c5970-140">设备注册日期。</span><span class="sxs-lookup"><span data-stu-id="c5970-140">Device registration date.</span></span>|
|<span data-ttu-id="c5970-141">enrollmentStartDateTime</span><span class="sxs-lookup"><span data-stu-id="c5970-141">enrollmentStartDateTime</span></span>|<span data-ttu-id="c5970-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5970-142">DateTimeOffset</span></span>|<span data-ttu-id="c5970-143">设备注册开始日期。</span><span class="sxs-lookup"><span data-stu-id="c5970-143">Device enrollment start date.</span></span>|
|<span data-ttu-id="c5970-144">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="c5970-144">enrollmentType</span></span>|[<span data-ttu-id="c5970-145">windowsAutopilotEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="c5970-145">windowsAutopilotEnrollmentType</span></span>](../resources/intune-troubleshooting-windowsautopilotenrollmenttype.md)|<span data-ttu-id="c5970-146">注册类型。</span><span class="sxs-lookup"><span data-stu-id="c5970-146">Enrollment type.</span></span> <span data-ttu-id="c5970-147">可取值为：`unknown`、`azureADJoinedWithAutopilotProfile`、`offlineDomainJoined`、`azureADJoinedUsingDeviceAuthWithAutopilotProfile`、`azureADJoinedUsingDeviceAuthWithoutAutopilotProfile`、`azureADJoinedWithOfflineAutopilotProfile`、`azureADJoinedWithWhiteGlove`、`offlineDomainJoinedWithWhiteGlove`、`offlineDomainJoinedWithOfflineAutopilotProfile`。</span><span class="sxs-lookup"><span data-stu-id="c5970-147">Possible values are: `unknown`, `azureADJoinedWithAutopilotProfile`, `offlineDomainJoined`, `azureADJoinedUsingDeviceAuthWithAutopilotProfile`, `azureADJoinedUsingDeviceAuthWithoutAutopilotProfile`, `azureADJoinedWithOfflineAutopilotProfile`, `azureADJoinedWithWhiteGlove`, `offlineDomainJoinedWithWhiteGlove`, `offlineDomainJoinedWithOfflineAutopilotProfile`.</span></span>|
|<span data-ttu-id="c5970-148">deviceSerialNumber</span><span class="sxs-lookup"><span data-stu-id="c5970-148">deviceSerialNumber</span></span>|<span data-ttu-id="c5970-149">String</span><span class="sxs-lookup"><span data-stu-id="c5970-149">String</span></span>|<span data-ttu-id="c5970-150">设备序列号。</span><span class="sxs-lookup"><span data-stu-id="c5970-150">Device serial number.</span></span>|
|<span data-ttu-id="c5970-151">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="c5970-151">managedDeviceName</span></span>|<span data-ttu-id="c5970-152">String</span><span class="sxs-lookup"><span data-stu-id="c5970-152">String</span></span>|<span data-ttu-id="c5970-153">托管设备名称。</span><span class="sxs-lookup"><span data-stu-id="c5970-153">Managed device name.</span></span>|
|<span data-ttu-id="c5970-154">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c5970-154">userPrincipalName</span></span>|<span data-ttu-id="c5970-155">String</span><span class="sxs-lookup"><span data-stu-id="c5970-155">String</span></span>|<span data-ttu-id="c5970-156">用于注册设备的用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="c5970-156">User principal name used to enroll the device.</span></span>|
|<span data-ttu-id="c5970-157">windowsAutopilotDeploymentProfileDisplayName</span><span class="sxs-lookup"><span data-stu-id="c5970-157">windowsAutopilotDeploymentProfileDisplayName</span></span>|<span data-ttu-id="c5970-158">String</span><span class="sxs-lookup"><span data-stu-id="c5970-158">String</span></span>|<span data-ttu-id="c5970-159">Autopilot 配置文件名称。</span><span class="sxs-lookup"><span data-stu-id="c5970-159">Autopilot profile name.</span></span>|
|<span data-ttu-id="c5970-160">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="c5970-160">enrollmentState</span></span>|[<span data-ttu-id="c5970-161">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="c5970-161">enrollmentState</span></span>](../resources/intune-shared-enrollmentstate.md)|<span data-ttu-id="c5970-162">注册状态，如 "已注册"，失败。</span><span class="sxs-lookup"><span data-stu-id="c5970-162">Enrollment state like Enrolled, Failed.</span></span> <span data-ttu-id="c5970-163">可取值为：`unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="c5970-163">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="c5970-164">windows10EnrollmentCompletionPageConfigurationDisplayName</span><span class="sxs-lookup"><span data-stu-id="c5970-164">windows10EnrollmentCompletionPageConfigurationDisplayName</span></span>|<span data-ttu-id="c5970-165">String</span><span class="sxs-lookup"><span data-stu-id="c5970-165">String</span></span>|<span data-ttu-id="c5970-166">注册状态页面配置文件名称</span><span class="sxs-lookup"><span data-stu-id="c5970-166">Enrollment Status Page profile name</span></span>|
|<span data-ttu-id="c5970-167">deploymentState</span><span class="sxs-lookup"><span data-stu-id="c5970-167">deploymentState</span></span>|[<span data-ttu-id="c5970-168">windowsAutopilotDeploymentState</span><span class="sxs-lookup"><span data-stu-id="c5970-168">windowsAutopilotDeploymentState</span></span>](../resources/intune-troubleshooting-windowsautopilotdeploymentstate.md)|<span data-ttu-id="c5970-169">部署状态，如成功、失败、InProgress、SuccessWithTimeout。</span><span class="sxs-lookup"><span data-stu-id="c5970-169">Deployment state like Success, Failure, InProgress, SuccessWithTimeout.</span></span> <span data-ttu-id="c5970-170">可取值为：`unknown`、`success`、`inProgress`、`failure`、`successWithTimeout`。</span><span class="sxs-lookup"><span data-stu-id="c5970-170">Possible values are: `unknown`, `success`, `inProgress`, `failure`, `successWithTimeout`.</span></span>|
|<span data-ttu-id="c5970-171">osVersion</span><span class="sxs-lookup"><span data-stu-id="c5970-171">osVersion</span></span>|<span data-ttu-id="c5970-172">String</span><span class="sxs-lookup"><span data-stu-id="c5970-172">String</span></span>|<span data-ttu-id="c5970-173">设备操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="c5970-173">Device operating system version.</span></span>|
|<span data-ttu-id="c5970-174">deploymentDuration</span><span class="sxs-lookup"><span data-stu-id="c5970-174">deploymentDuration</span></span>|<span data-ttu-id="c5970-175">持续时间</span><span class="sxs-lookup"><span data-stu-id="c5970-175">Duration</span></span>|<span data-ttu-id="c5970-176">包含注册的 Autopilot 部署持续时间。</span><span class="sxs-lookup"><span data-stu-id="c5970-176">Autopilot deployment duration including enrollment.</span></span>|
|<span data-ttu-id="c5970-177">deploymentTotalDuration</span><span class="sxs-lookup"><span data-stu-id="c5970-177">deploymentTotalDuration</span></span>|<span data-ttu-id="c5970-178">持续时间</span><span class="sxs-lookup"><span data-stu-id="c5970-178">Duration</span></span>|<span data-ttu-id="c5970-179">从注册到桌面屏幕的总部署持续时间。</span><span class="sxs-lookup"><span data-stu-id="c5970-179">Total deployment duration from enrollment to Desktop screen.</span></span>|
|<span data-ttu-id="c5970-180">devicePreparationDuration</span><span class="sxs-lookup"><span data-stu-id="c5970-180">devicePreparationDuration</span></span>|<span data-ttu-id="c5970-181">持续时间</span><span class="sxs-lookup"><span data-stu-id="c5970-181">Duration</span></span>|<span data-ttu-id="c5970-182">在设备注册中花费的时间。</span><span class="sxs-lookup"><span data-stu-id="c5970-182">Time spent in device enrollment.</span></span>|
|<span data-ttu-id="c5970-183">deviceSetupDuration</span><span class="sxs-lookup"><span data-stu-id="c5970-183">deviceSetupDuration</span></span>|<span data-ttu-id="c5970-184">持续时间</span><span class="sxs-lookup"><span data-stu-id="c5970-184">Duration</span></span>|<span data-ttu-id="c5970-185">在设备 ESP 中花费的时间。</span><span class="sxs-lookup"><span data-stu-id="c5970-185">Time spent in device ESP.</span></span>|
|<span data-ttu-id="c5970-186">accountSetupDuration</span><span class="sxs-lookup"><span data-stu-id="c5970-186">accountSetupDuration</span></span>|<span data-ttu-id="c5970-187">持续时间</span><span class="sxs-lookup"><span data-stu-id="c5970-187">Duration</span></span>|<span data-ttu-id="c5970-188">用户 ESP 中所用的时间。</span><span class="sxs-lookup"><span data-stu-id="c5970-188">Time spent in user ESP.</span></span>|
|<span data-ttu-id="c5970-189">deploymentStartDateTime</span><span class="sxs-lookup"><span data-stu-id="c5970-189">deploymentStartDateTime</span></span>|<span data-ttu-id="c5970-190">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5970-190">DateTimeOffset</span></span>|<span data-ttu-id="c5970-191">部署开始时间。</span><span class="sxs-lookup"><span data-stu-id="c5970-191">Deployment start time.</span></span>|
|<span data-ttu-id="c5970-192">deploymentEndDateTime</span><span class="sxs-lookup"><span data-stu-id="c5970-192">deploymentEndDateTime</span></span>|<span data-ttu-id="c5970-193">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5970-193">DateTimeOffset</span></span>|<span data-ttu-id="c5970-194">部署结束时间。</span><span class="sxs-lookup"><span data-stu-id="c5970-194">Deployment end time.</span></span>|
|<span data-ttu-id="c5970-195">targetedAppCount</span><span class="sxs-lookup"><span data-stu-id="c5970-195">targetedAppCount</span></span>|<span data-ttu-id="c5970-196">Int32</span><span class="sxs-lookup"><span data-stu-id="c5970-196">Int32</span></span>|<span data-ttu-id="c5970-197">目标应用程序的计数。</span><span class="sxs-lookup"><span data-stu-id="c5970-197">Count of applications targeted.</span></span>|
|<span data-ttu-id="c5970-198">targetedPolicyCount</span><span class="sxs-lookup"><span data-stu-id="c5970-198">targetedPolicyCount</span></span>|<span data-ttu-id="c5970-199">Int32</span><span class="sxs-lookup"><span data-stu-id="c5970-199">Int32</span></span>|<span data-ttu-id="c5970-200">目标策略的计数。</span><span class="sxs-lookup"><span data-stu-id="c5970-200">Count of policies targeted.</span></span>|
|<span data-ttu-id="c5970-201">enrollmentFailureDetails</span><span class="sxs-lookup"><span data-stu-id="c5970-201">enrollmentFailureDetails</span></span>|<span data-ttu-id="c5970-202">String</span><span class="sxs-lookup"><span data-stu-id="c5970-202">String</span></span>|<span data-ttu-id="c5970-203">注册失败详细信息。</span><span class="sxs-lookup"><span data-stu-id="c5970-203">Enrollment failure details.</span></span>|



## <a name="response"></a><span data-ttu-id="c5970-204">响应</span><span class="sxs-lookup"><span data-stu-id="c5970-204">Response</span></span>
<span data-ttu-id="c5970-205">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c5970-205">If successful, this method returns a `200 OK` response code and an updated [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5970-206">示例</span><span class="sxs-lookup"><span data-stu-id="c5970-206">Example</span></span>

### <a name="request"></a><span data-ttu-id="c5970-207">请求</span><span class="sxs-lookup"><span data-stu-id="c5970-207">Request</span></span>
<span data-ttu-id="c5970-208">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c5970-208">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/autopilotEvents/{deviceManagementAutopilotEventId}
Content-type: application/json
Content-length: 1323

{
  "@odata.type": "#microsoft.graph.deviceManagementAutopilotEvent",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "deviceRegisteredDateTime": "2017-01-01T00:02:48.7185581-08:00",
  "enrollmentStartDateTime": "2017-01-01T00:00:19.6280481-08:00",
  "enrollmentType": "azureADJoinedWithAutopilotProfile",
  "deviceSerialNumber": "Device Serial Number value",
  "managedDeviceName": "Managed Device Name value",
  "userPrincipalName": "User Principal Name value",
  "windowsAutopilotDeploymentProfileDisplayName": "Windows Autopilot Deployment Profile Display Name value",
  "enrollmentState": "enrolled",
  "windows10EnrollmentCompletionPageConfigurationDisplayName": "Windows10Enrollment Completion Page Configuration Display Name value",
  "deploymentState": "success",
  "osVersion": "Os Version value",
  "deploymentDuration": "PT3M21.5549443S",
  "deploymentTotalDuration": "PT1M43.5284261S",
  "devicePreparationDuration": "-PT1M32.1347897S",
  "deviceSetupDuration": "-PT2M57.2190107S",
  "accountSetupDuration": "-PT2M32.0507894S",
  "deploymentStartDateTime": "2016-12-31T23:59:37.257201-08:00",
  "deploymentEndDateTime": "2017-01-01T00:00:46.5128291-08:00",
  "targetedAppCount": 0,
  "targetedPolicyCount": 3,
  "enrollmentFailureDetails": "Enrollment Failure Details value"
}
```

### <a name="response"></a><span data-ttu-id="c5970-209">响应</span><span class="sxs-lookup"><span data-stu-id="c5970-209">Response</span></span>
<span data-ttu-id="c5970-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c5970-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1372

{
  "@odata.type": "#microsoft.graph.deviceManagementAutopilotEvent",
  "id": "3e455cab-5cab-3e45-ab5c-453eab5c453e",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "deviceRegisteredDateTime": "2017-01-01T00:02:48.7185581-08:00",
  "enrollmentStartDateTime": "2017-01-01T00:00:19.6280481-08:00",
  "enrollmentType": "azureADJoinedWithAutopilotProfile",
  "deviceSerialNumber": "Device Serial Number value",
  "managedDeviceName": "Managed Device Name value",
  "userPrincipalName": "User Principal Name value",
  "windowsAutopilotDeploymentProfileDisplayName": "Windows Autopilot Deployment Profile Display Name value",
  "enrollmentState": "enrolled",
  "windows10EnrollmentCompletionPageConfigurationDisplayName": "Windows10Enrollment Completion Page Configuration Display Name value",
  "deploymentState": "success",
  "osVersion": "Os Version value",
  "deploymentDuration": "PT3M21.5549443S",
  "deploymentTotalDuration": "PT1M43.5284261S",
  "devicePreparationDuration": "-PT1M32.1347897S",
  "deviceSetupDuration": "-PT2M57.2190107S",
  "accountSetupDuration": "-PT2M32.0507894S",
  "deploymentStartDateTime": "2016-12-31T23:59:37.257201-08:00",
  "deploymentEndDateTime": "2017-01-01T00:00:46.5128291-08:00",
  "targetedAppCount": 0,
  "targetedPolicyCount": 3,
  "enrollmentFailureDetails": "Enrollment Failure Details value"
}
```




