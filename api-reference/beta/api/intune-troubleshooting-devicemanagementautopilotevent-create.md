---
title: 创建 deviceManagementAutopilotEvent
description: 创建新的 deviceManagementAutopilotEvent 对象。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e33ab0fc0b48284457785702d3591f462039505c
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42800261"
---
# <a name="create-devicemanagementautopilotevent"></a><span data-ttu-id="10c21-103">创建 deviceManagementAutopilotEvent</span><span class="sxs-lookup"><span data-stu-id="10c21-103">Create deviceManagementAutopilotEvent</span></span>

> <span data-ttu-id="10c21-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="10c21-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="10c21-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="10c21-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="10c21-106">创建新的[deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md)对象。</span><span class="sxs-lookup"><span data-stu-id="10c21-106">Create a new [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="10c21-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="10c21-107">Prerequisites</span></span>
<span data-ttu-id="10c21-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="10c21-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10c21-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="10c21-110">Permission type</span></span>|<span data-ttu-id="10c21-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="10c21-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="10c21-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="10c21-112">Delegated (work or school account)</span></span>|<span data-ttu-id="10c21-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10c21-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="10c21-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="10c21-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="10c21-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="10c21-115">Not supported.</span></span>|
|<span data-ttu-id="10c21-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="10c21-116">Application</span></span>|<span data-ttu-id="10c21-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10c21-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="10c21-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="10c21-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/autopilotEvents
```

## <a name="request-headers"></a><span data-ttu-id="10c21-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="10c21-119">Request headers</span></span>
|<span data-ttu-id="10c21-120">标头</span><span class="sxs-lookup"><span data-stu-id="10c21-120">Header</span></span>|<span data-ttu-id="10c21-121">值</span><span class="sxs-lookup"><span data-stu-id="10c21-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="10c21-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="10c21-122">Authorization</span></span>|<span data-ttu-id="10c21-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="10c21-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="10c21-124">接受</span><span class="sxs-lookup"><span data-stu-id="10c21-124">Accept</span></span>|<span data-ttu-id="10c21-125">application/json</span><span class="sxs-lookup"><span data-stu-id="10c21-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="10c21-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="10c21-126">Request body</span></span>
<span data-ttu-id="10c21-127">在请求正文中，提供 deviceManagementAutopilotEvent 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="10c21-127">In the request body, supply a JSON representation for the deviceManagementAutopilotEvent object.</span></span>

<span data-ttu-id="10c21-128">下表显示创建 deviceManagementAutopilotEvent 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="10c21-128">The following table shows the properties that are required when you create the deviceManagementAutopilotEvent.</span></span>

|<span data-ttu-id="10c21-129">属性</span><span class="sxs-lookup"><span data-stu-id="10c21-129">Property</span></span>|<span data-ttu-id="10c21-130">类型</span><span class="sxs-lookup"><span data-stu-id="10c21-130">Type</span></span>|<span data-ttu-id="10c21-131">说明</span><span class="sxs-lookup"><span data-stu-id="10c21-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10c21-132">id</span><span class="sxs-lookup"><span data-stu-id="10c21-132">id</span></span>|<span data-ttu-id="10c21-133">String</span><span class="sxs-lookup"><span data-stu-id="10c21-133">String</span></span>|<span data-ttu-id="10c21-134">对象的 UUID</span><span class="sxs-lookup"><span data-stu-id="10c21-134">UUID for the object</span></span>|
|<span data-ttu-id="10c21-135">deviceId</span><span class="sxs-lookup"><span data-stu-id="10c21-135">deviceId</span></span>|<span data-ttu-id="10c21-136">String</span><span class="sxs-lookup"><span data-stu-id="10c21-136">String</span></span>|<span data-ttu-id="10c21-137">与对象关联的设备 id</span><span class="sxs-lookup"><span data-stu-id="10c21-137">Device id associated with the object</span></span>|
|<span data-ttu-id="10c21-138">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="10c21-138">eventDateTime</span></span>|<span data-ttu-id="10c21-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="10c21-139">DateTimeOffset</span></span>|<span data-ttu-id="10c21-140">事件发生的时间。</span><span class="sxs-lookup"><span data-stu-id="10c21-140">Time when the event occurred .</span></span>|
|<span data-ttu-id="10c21-141">deviceRegisteredDateTime</span><span class="sxs-lookup"><span data-stu-id="10c21-141">deviceRegisteredDateTime</span></span>|<span data-ttu-id="10c21-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="10c21-142">DateTimeOffset</span></span>|<span data-ttu-id="10c21-143">设备注册日期。</span><span class="sxs-lookup"><span data-stu-id="10c21-143">Device registration date.</span></span>|
|<span data-ttu-id="10c21-144">enrollmentStartDateTime</span><span class="sxs-lookup"><span data-stu-id="10c21-144">enrollmentStartDateTime</span></span>|<span data-ttu-id="10c21-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="10c21-145">DateTimeOffset</span></span>|<span data-ttu-id="10c21-146">设备注册开始日期。</span><span class="sxs-lookup"><span data-stu-id="10c21-146">Device enrollment start date.</span></span>|
|<span data-ttu-id="10c21-147">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="10c21-147">enrollmentType</span></span>|[<span data-ttu-id="10c21-148">windowsAutopilotEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="10c21-148">windowsAutopilotEnrollmentType</span></span>](../resources/intune-troubleshooting-windowsautopilotenrollmenttype.md)|<span data-ttu-id="10c21-149">注册类型。</span><span class="sxs-lookup"><span data-stu-id="10c21-149">Enrollment type.</span></span> <span data-ttu-id="10c21-150">可取值为：`unknown`、`azureADJoinedWithAutopilotProfile`、`offlineDomainJoined`、`azureADJoinedUsingDeviceAuthWithAutopilotProfile`、`azureADJoinedUsingDeviceAuthWithoutAutopilotProfile`、`azureADJoinedWithOfflineAutopilotProfile`、`azureADJoinedWithWhiteGlove`、`offlineDomainJoinedWithWhiteGlove`、`offlineDomainJoinedWithOfflineAutopilotProfile`。</span><span class="sxs-lookup"><span data-stu-id="10c21-150">Possible values are: `unknown`, `azureADJoinedWithAutopilotProfile`, `offlineDomainJoined`, `azureADJoinedUsingDeviceAuthWithAutopilotProfile`, `azureADJoinedUsingDeviceAuthWithoutAutopilotProfile`, `azureADJoinedWithOfflineAutopilotProfile`, `azureADJoinedWithWhiteGlove`, `offlineDomainJoinedWithWhiteGlove`, `offlineDomainJoinedWithOfflineAutopilotProfile`.</span></span>|
|<span data-ttu-id="10c21-151">deviceSerialNumber</span><span class="sxs-lookup"><span data-stu-id="10c21-151">deviceSerialNumber</span></span>|<span data-ttu-id="10c21-152">String</span><span class="sxs-lookup"><span data-stu-id="10c21-152">String</span></span>|<span data-ttu-id="10c21-153">设备序列号。</span><span class="sxs-lookup"><span data-stu-id="10c21-153">Device serial number.</span></span>|
|<span data-ttu-id="10c21-154">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="10c21-154">managedDeviceName</span></span>|<span data-ttu-id="10c21-155">String</span><span class="sxs-lookup"><span data-stu-id="10c21-155">String</span></span>|<span data-ttu-id="10c21-156">托管设备名称。</span><span class="sxs-lookup"><span data-stu-id="10c21-156">Managed device name.</span></span>|
|<span data-ttu-id="10c21-157">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="10c21-157">userPrincipalName</span></span>|<span data-ttu-id="10c21-158">String</span><span class="sxs-lookup"><span data-stu-id="10c21-158">String</span></span>|<span data-ttu-id="10c21-159">用于注册设备的用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="10c21-159">User principal name used to enroll the device.</span></span>|
|<span data-ttu-id="10c21-160">windowsAutopilotDeploymentProfileDisplayName</span><span class="sxs-lookup"><span data-stu-id="10c21-160">windowsAutopilotDeploymentProfileDisplayName</span></span>|<span data-ttu-id="10c21-161">String</span><span class="sxs-lookup"><span data-stu-id="10c21-161">String</span></span>|<span data-ttu-id="10c21-162">Autopilot 配置文件名称。</span><span class="sxs-lookup"><span data-stu-id="10c21-162">Autopilot profile name.</span></span>|
|<span data-ttu-id="10c21-163">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="10c21-163">enrollmentState</span></span>|[<span data-ttu-id="10c21-164">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="10c21-164">enrollmentState</span></span>](../resources/intune-shared-enrollmentstate.md)|<span data-ttu-id="10c21-165">注册状态，如 "已注册"，失败。</span><span class="sxs-lookup"><span data-stu-id="10c21-165">Enrollment state like Enrolled, Failed.</span></span> <span data-ttu-id="10c21-166">可取值为：`unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="10c21-166">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="10c21-167">windows10EnrollmentCompletionPageConfigurationDisplayName</span><span class="sxs-lookup"><span data-stu-id="10c21-167">windows10EnrollmentCompletionPageConfigurationDisplayName</span></span>|<span data-ttu-id="10c21-168">String</span><span class="sxs-lookup"><span data-stu-id="10c21-168">String</span></span>|<span data-ttu-id="10c21-169">注册状态页面配置文件名称</span><span class="sxs-lookup"><span data-stu-id="10c21-169">Enrollment Status Page profile name</span></span>|
|<span data-ttu-id="10c21-170">deploymentState</span><span class="sxs-lookup"><span data-stu-id="10c21-170">deploymentState</span></span>|[<span data-ttu-id="10c21-171">windowsAutopilotDeploymentState</span><span class="sxs-lookup"><span data-stu-id="10c21-171">windowsAutopilotDeploymentState</span></span>](../resources/intune-troubleshooting-windowsautopilotdeploymentstate.md)|<span data-ttu-id="10c21-172">部署状态，如成功、失败、InProgress、SuccessWithTimeout。</span><span class="sxs-lookup"><span data-stu-id="10c21-172">Deployment state like Success, Failure, InProgress, SuccessWithTimeout.</span></span> <span data-ttu-id="10c21-173">可取值为：`unknown`、`success`、`inProgress`、`failure`、`successWithTimeout`。</span><span class="sxs-lookup"><span data-stu-id="10c21-173">Possible values are: `unknown`, `success`, `inProgress`, `failure`, `successWithTimeout`.</span></span>|
|<span data-ttu-id="10c21-174">osVersion</span><span class="sxs-lookup"><span data-stu-id="10c21-174">osVersion</span></span>|<span data-ttu-id="10c21-175">String</span><span class="sxs-lookup"><span data-stu-id="10c21-175">String</span></span>|<span data-ttu-id="10c21-176">设备操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="10c21-176">Device operating system version.</span></span>|
|<span data-ttu-id="10c21-177">deploymentDuration</span><span class="sxs-lookup"><span data-stu-id="10c21-177">deploymentDuration</span></span>|<span data-ttu-id="10c21-178">持续时间</span><span class="sxs-lookup"><span data-stu-id="10c21-178">Duration</span></span>|<span data-ttu-id="10c21-179">包含注册的 Autopilot 部署持续时间。</span><span class="sxs-lookup"><span data-stu-id="10c21-179">Autopilot deployment duration including enrollment.</span></span>|
|<span data-ttu-id="10c21-180">deploymentTotalDuration</span><span class="sxs-lookup"><span data-stu-id="10c21-180">deploymentTotalDuration</span></span>|<span data-ttu-id="10c21-181">持续时间</span><span class="sxs-lookup"><span data-stu-id="10c21-181">Duration</span></span>|<span data-ttu-id="10c21-182">从注册到桌面屏幕的总部署持续时间。</span><span class="sxs-lookup"><span data-stu-id="10c21-182">Total deployment duration from enrollment to Desktop screen.</span></span>|
|<span data-ttu-id="10c21-183">devicePreparationDuration</span><span class="sxs-lookup"><span data-stu-id="10c21-183">devicePreparationDuration</span></span>|<span data-ttu-id="10c21-184">持续时间</span><span class="sxs-lookup"><span data-stu-id="10c21-184">Duration</span></span>|<span data-ttu-id="10c21-185">在设备注册中花费的时间。</span><span class="sxs-lookup"><span data-stu-id="10c21-185">Time spent in device enrollment.</span></span>|
|<span data-ttu-id="10c21-186">deviceSetupDuration</span><span class="sxs-lookup"><span data-stu-id="10c21-186">deviceSetupDuration</span></span>|<span data-ttu-id="10c21-187">持续时间</span><span class="sxs-lookup"><span data-stu-id="10c21-187">Duration</span></span>|<span data-ttu-id="10c21-188">在设备 ESP 中花费的时间。</span><span class="sxs-lookup"><span data-stu-id="10c21-188">Time spent in device ESP.</span></span>|
|<span data-ttu-id="10c21-189">accountSetupDuration</span><span class="sxs-lookup"><span data-stu-id="10c21-189">accountSetupDuration</span></span>|<span data-ttu-id="10c21-190">持续时间</span><span class="sxs-lookup"><span data-stu-id="10c21-190">Duration</span></span>|<span data-ttu-id="10c21-191">用户 ESP 中所用的时间。</span><span class="sxs-lookup"><span data-stu-id="10c21-191">Time spent in user ESP.</span></span>|
|<span data-ttu-id="10c21-192">deploymentStartDateTime</span><span class="sxs-lookup"><span data-stu-id="10c21-192">deploymentStartDateTime</span></span>|<span data-ttu-id="10c21-193">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="10c21-193">DateTimeOffset</span></span>|<span data-ttu-id="10c21-194">部署开始时间。</span><span class="sxs-lookup"><span data-stu-id="10c21-194">Deployment start time.</span></span>|
|<span data-ttu-id="10c21-195">deploymentEndDateTime</span><span class="sxs-lookup"><span data-stu-id="10c21-195">deploymentEndDateTime</span></span>|<span data-ttu-id="10c21-196">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="10c21-196">DateTimeOffset</span></span>|<span data-ttu-id="10c21-197">部署结束时间。</span><span class="sxs-lookup"><span data-stu-id="10c21-197">Deployment end time.</span></span>|
|<span data-ttu-id="10c21-198">targetedAppCount</span><span class="sxs-lookup"><span data-stu-id="10c21-198">targetedAppCount</span></span>|<span data-ttu-id="10c21-199">Int32</span><span class="sxs-lookup"><span data-stu-id="10c21-199">Int32</span></span>|<span data-ttu-id="10c21-200">目标应用程序的计数。</span><span class="sxs-lookup"><span data-stu-id="10c21-200">Count of applications targeted.</span></span>|
|<span data-ttu-id="10c21-201">targetedPolicyCount</span><span class="sxs-lookup"><span data-stu-id="10c21-201">targetedPolicyCount</span></span>|<span data-ttu-id="10c21-202">Int32</span><span class="sxs-lookup"><span data-stu-id="10c21-202">Int32</span></span>|<span data-ttu-id="10c21-203">目标策略的计数。</span><span class="sxs-lookup"><span data-stu-id="10c21-203">Count of policies targeted.</span></span>|
|<span data-ttu-id="10c21-204">enrollmentFailureDetails</span><span class="sxs-lookup"><span data-stu-id="10c21-204">enrollmentFailureDetails</span></span>|<span data-ttu-id="10c21-205">String</span><span class="sxs-lookup"><span data-stu-id="10c21-205">String</span></span>|<span data-ttu-id="10c21-206">注册失败详细信息。</span><span class="sxs-lookup"><span data-stu-id="10c21-206">Enrollment failure details.</span></span>|



## <a name="response"></a><span data-ttu-id="10c21-207">响应</span><span class="sxs-lookup"><span data-stu-id="10c21-207">Response</span></span>
<span data-ttu-id="10c21-208">如果成功，此方法在响应`201 Created`正文中返回响应代码和[deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md)对象。</span><span class="sxs-lookup"><span data-stu-id="10c21-208">If successful, this method returns a `201 Created` response code and a [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="10c21-209">示例</span><span class="sxs-lookup"><span data-stu-id="10c21-209">Example</span></span>

### <a name="request"></a><span data-ttu-id="10c21-210">请求</span><span class="sxs-lookup"><span data-stu-id="10c21-210">Request</span></span>
<span data-ttu-id="10c21-211">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="10c21-211">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/autopilotEvents
Content-type: application/json
Content-length: 1357

{
  "@odata.type": "#microsoft.graph.deviceManagementAutopilotEvent",
  "deviceId": "Device Id value",
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

### <a name="response"></a><span data-ttu-id="10c21-212">响应</span><span class="sxs-lookup"><span data-stu-id="10c21-212">Response</span></span>
<span data-ttu-id="10c21-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="10c21-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1406

{
  "@odata.type": "#microsoft.graph.deviceManagementAutopilotEvent",
  "id": "3e455cab-5cab-3e45-ab5c-453eab5c453e",
  "deviceId": "Device Id value",
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




