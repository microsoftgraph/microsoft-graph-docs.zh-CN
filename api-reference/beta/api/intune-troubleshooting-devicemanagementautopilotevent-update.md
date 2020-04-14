---
title: 更新 deviceManagementAutopilotEvent
description: 更新 deviceManagementAutopilotEvent 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ed84a7c1bee3c1b6a6a06136392350a6883d870d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43443453"
---
# <a name="update-devicemanagementautopilotevent"></a><span data-ttu-id="cf06f-103">更新 deviceManagementAutopilotEvent</span><span class="sxs-lookup"><span data-stu-id="cf06f-103">Update deviceManagementAutopilotEvent</span></span>

<span data-ttu-id="cf06f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf06f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cf06f-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="cf06f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cf06f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cf06f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cf06f-107">更新[deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="cf06f-107">Update the properties of a [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cf06f-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="cf06f-108">Prerequisites</span></span>
<span data-ttu-id="cf06f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cf06f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf06f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="cf06f-111">Permission type</span></span>|<span data-ttu-id="cf06f-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="cf06f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cf06f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cf06f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cf06f-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf06f-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="cf06f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cf06f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cf06f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="cf06f-116">Not supported.</span></span>|
|<span data-ttu-id="cf06f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="cf06f-117">Application</span></span>|<span data-ttu-id="cf06f-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf06f-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cf06f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cf06f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/autopilotEvents/{deviceManagementAutopilotEventId}
```

## <a name="request-headers"></a><span data-ttu-id="cf06f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="cf06f-120">Request headers</span></span>
|<span data-ttu-id="cf06f-121">标头</span><span class="sxs-lookup"><span data-stu-id="cf06f-121">Header</span></span>|<span data-ttu-id="cf06f-122">值</span><span class="sxs-lookup"><span data-stu-id="cf06f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cf06f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cf06f-123">Authorization</span></span>|<span data-ttu-id="cf06f-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="cf06f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cf06f-125">接受</span><span class="sxs-lookup"><span data-stu-id="cf06f-125">Accept</span></span>|<span data-ttu-id="cf06f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cf06f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf06f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="cf06f-127">Request body</span></span>
<span data-ttu-id="cf06f-128">在请求正文中，提供[deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cf06f-128">In the request body, supply a JSON representation for the [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) object.</span></span>

<span data-ttu-id="cf06f-129">下表显示创建[deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="cf06f-129">The following table shows the properties that are required when you create the [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md).</span></span>

|<span data-ttu-id="cf06f-130">属性</span><span class="sxs-lookup"><span data-stu-id="cf06f-130">Property</span></span>|<span data-ttu-id="cf06f-131">类型</span><span class="sxs-lookup"><span data-stu-id="cf06f-131">Type</span></span>|<span data-ttu-id="cf06f-132">说明</span><span class="sxs-lookup"><span data-stu-id="cf06f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf06f-133">id</span><span class="sxs-lookup"><span data-stu-id="cf06f-133">id</span></span>|<span data-ttu-id="cf06f-134">String</span><span class="sxs-lookup"><span data-stu-id="cf06f-134">String</span></span>|<span data-ttu-id="cf06f-135">对象的 UUID</span><span class="sxs-lookup"><span data-stu-id="cf06f-135">UUID for the object</span></span>|
|<span data-ttu-id="cf06f-136">deviceId</span><span class="sxs-lookup"><span data-stu-id="cf06f-136">deviceId</span></span>|<span data-ttu-id="cf06f-137">String</span><span class="sxs-lookup"><span data-stu-id="cf06f-137">String</span></span>|<span data-ttu-id="cf06f-138">与对象关联的设备 id</span><span class="sxs-lookup"><span data-stu-id="cf06f-138">Device id associated with the object</span></span>|
|<span data-ttu-id="cf06f-139">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="cf06f-139">eventDateTime</span></span>|<span data-ttu-id="cf06f-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf06f-140">DateTimeOffset</span></span>|<span data-ttu-id="cf06f-141">事件发生的时间。</span><span class="sxs-lookup"><span data-stu-id="cf06f-141">Time when the event occurred .</span></span>|
|<span data-ttu-id="cf06f-142">deviceRegisteredDateTime</span><span class="sxs-lookup"><span data-stu-id="cf06f-142">deviceRegisteredDateTime</span></span>|<span data-ttu-id="cf06f-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf06f-143">DateTimeOffset</span></span>|<span data-ttu-id="cf06f-144">设备注册日期。</span><span class="sxs-lookup"><span data-stu-id="cf06f-144">Device registration date.</span></span>|
|<span data-ttu-id="cf06f-145">enrollmentStartDateTime</span><span class="sxs-lookup"><span data-stu-id="cf06f-145">enrollmentStartDateTime</span></span>|<span data-ttu-id="cf06f-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf06f-146">DateTimeOffset</span></span>|<span data-ttu-id="cf06f-147">设备注册开始日期。</span><span class="sxs-lookup"><span data-stu-id="cf06f-147">Device enrollment start date.</span></span>|
|<span data-ttu-id="cf06f-148">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="cf06f-148">enrollmentType</span></span>|[<span data-ttu-id="cf06f-149">windowsAutopilotEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="cf06f-149">windowsAutopilotEnrollmentType</span></span>](../resources/intune-troubleshooting-windowsautopilotenrollmenttype.md)|<span data-ttu-id="cf06f-150">注册类型。</span><span class="sxs-lookup"><span data-stu-id="cf06f-150">Enrollment type.</span></span> <span data-ttu-id="cf06f-151">可取值为：`unknown`、`azureADJoinedWithAutopilotProfile`、`offlineDomainJoined`、`azureADJoinedUsingDeviceAuthWithAutopilotProfile`、`azureADJoinedUsingDeviceAuthWithoutAutopilotProfile`、`azureADJoinedWithOfflineAutopilotProfile`、`azureADJoinedWithWhiteGlove`、`offlineDomainJoinedWithWhiteGlove`、`offlineDomainJoinedWithOfflineAutopilotProfile`。</span><span class="sxs-lookup"><span data-stu-id="cf06f-151">Possible values are: `unknown`, `azureADJoinedWithAutopilotProfile`, `offlineDomainJoined`, `azureADJoinedUsingDeviceAuthWithAutopilotProfile`, `azureADJoinedUsingDeviceAuthWithoutAutopilotProfile`, `azureADJoinedWithOfflineAutopilotProfile`, `azureADJoinedWithWhiteGlove`, `offlineDomainJoinedWithWhiteGlove`, `offlineDomainJoinedWithOfflineAutopilotProfile`.</span></span>|
|<span data-ttu-id="cf06f-152">deviceSerialNumber</span><span class="sxs-lookup"><span data-stu-id="cf06f-152">deviceSerialNumber</span></span>|<span data-ttu-id="cf06f-153">String</span><span class="sxs-lookup"><span data-stu-id="cf06f-153">String</span></span>|<span data-ttu-id="cf06f-154">设备序列号。</span><span class="sxs-lookup"><span data-stu-id="cf06f-154">Device serial number.</span></span>|
|<span data-ttu-id="cf06f-155">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="cf06f-155">managedDeviceName</span></span>|<span data-ttu-id="cf06f-156">String</span><span class="sxs-lookup"><span data-stu-id="cf06f-156">String</span></span>|<span data-ttu-id="cf06f-157">托管设备名称。</span><span class="sxs-lookup"><span data-stu-id="cf06f-157">Managed device name.</span></span>|
|<span data-ttu-id="cf06f-158">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="cf06f-158">userPrincipalName</span></span>|<span data-ttu-id="cf06f-159">String</span><span class="sxs-lookup"><span data-stu-id="cf06f-159">String</span></span>|<span data-ttu-id="cf06f-160">用于注册设备的用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="cf06f-160">User principal name used to enroll the device.</span></span>|
|<span data-ttu-id="cf06f-161">windowsAutopilotDeploymentProfileDisplayName</span><span class="sxs-lookup"><span data-stu-id="cf06f-161">windowsAutopilotDeploymentProfileDisplayName</span></span>|<span data-ttu-id="cf06f-162">String</span><span class="sxs-lookup"><span data-stu-id="cf06f-162">String</span></span>|<span data-ttu-id="cf06f-163">Autopilot 配置文件名称。</span><span class="sxs-lookup"><span data-stu-id="cf06f-163">Autopilot profile name.</span></span>|
|<span data-ttu-id="cf06f-164">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="cf06f-164">enrollmentState</span></span>|[<span data-ttu-id="cf06f-165">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="cf06f-165">enrollmentState</span></span>](../resources/intune-shared-enrollmentstate.md)|<span data-ttu-id="cf06f-166">注册状态，如 "已注册"，失败。</span><span class="sxs-lookup"><span data-stu-id="cf06f-166">Enrollment state like Enrolled, Failed.</span></span> <span data-ttu-id="cf06f-167">可取值为：`unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="cf06f-167">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="cf06f-168">windows10EnrollmentCompletionPageConfigurationDisplayName</span><span class="sxs-lookup"><span data-stu-id="cf06f-168">windows10EnrollmentCompletionPageConfigurationDisplayName</span></span>|<span data-ttu-id="cf06f-169">String</span><span class="sxs-lookup"><span data-stu-id="cf06f-169">String</span></span>|<span data-ttu-id="cf06f-170">注册状态页面配置文件名称</span><span class="sxs-lookup"><span data-stu-id="cf06f-170">Enrollment Status Page profile name</span></span>|
|<span data-ttu-id="cf06f-171">deploymentState</span><span class="sxs-lookup"><span data-stu-id="cf06f-171">deploymentState</span></span>|[<span data-ttu-id="cf06f-172">windowsAutopilotDeploymentState</span><span class="sxs-lookup"><span data-stu-id="cf06f-172">windowsAutopilotDeploymentState</span></span>](../resources/intune-troubleshooting-windowsautopilotdeploymentstate.md)|<span data-ttu-id="cf06f-173">部署状态，如成功、失败、InProgress、SuccessWithTimeout。</span><span class="sxs-lookup"><span data-stu-id="cf06f-173">Deployment state like Success, Failure, InProgress, SuccessWithTimeout.</span></span> <span data-ttu-id="cf06f-174">可取值为：`unknown`、`success`、`inProgress`、`failure`、`successWithTimeout`。</span><span class="sxs-lookup"><span data-stu-id="cf06f-174">Possible values are: `unknown`, `success`, `inProgress`, `failure`, `successWithTimeout`.</span></span>|
|<span data-ttu-id="cf06f-175">osVersion</span><span class="sxs-lookup"><span data-stu-id="cf06f-175">osVersion</span></span>|<span data-ttu-id="cf06f-176">String</span><span class="sxs-lookup"><span data-stu-id="cf06f-176">String</span></span>|<span data-ttu-id="cf06f-177">设备操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="cf06f-177">Device operating system version.</span></span>|
|<span data-ttu-id="cf06f-178">deploymentDuration</span><span class="sxs-lookup"><span data-stu-id="cf06f-178">deploymentDuration</span></span>|<span data-ttu-id="cf06f-179">持续时间</span><span class="sxs-lookup"><span data-stu-id="cf06f-179">Duration</span></span>|<span data-ttu-id="cf06f-180">包含注册的 Autopilot 部署持续时间。</span><span class="sxs-lookup"><span data-stu-id="cf06f-180">Autopilot deployment duration including enrollment.</span></span>|
|<span data-ttu-id="cf06f-181">deploymentTotalDuration</span><span class="sxs-lookup"><span data-stu-id="cf06f-181">deploymentTotalDuration</span></span>|<span data-ttu-id="cf06f-182">持续时间</span><span class="sxs-lookup"><span data-stu-id="cf06f-182">Duration</span></span>|<span data-ttu-id="cf06f-183">从注册到桌面屏幕的总部署持续时间。</span><span class="sxs-lookup"><span data-stu-id="cf06f-183">Total deployment duration from enrollment to Desktop screen.</span></span>|
|<span data-ttu-id="cf06f-184">devicePreparationDuration</span><span class="sxs-lookup"><span data-stu-id="cf06f-184">devicePreparationDuration</span></span>|<span data-ttu-id="cf06f-185">持续时间</span><span class="sxs-lookup"><span data-stu-id="cf06f-185">Duration</span></span>|<span data-ttu-id="cf06f-186">在设备注册中花费的时间。</span><span class="sxs-lookup"><span data-stu-id="cf06f-186">Time spent in device enrollment.</span></span>|
|<span data-ttu-id="cf06f-187">deviceSetupDuration</span><span class="sxs-lookup"><span data-stu-id="cf06f-187">deviceSetupDuration</span></span>|<span data-ttu-id="cf06f-188">持续时间</span><span class="sxs-lookup"><span data-stu-id="cf06f-188">Duration</span></span>|<span data-ttu-id="cf06f-189">在设备 ESP 中花费的时间。</span><span class="sxs-lookup"><span data-stu-id="cf06f-189">Time spent in device ESP.</span></span>|
|<span data-ttu-id="cf06f-190">accountSetupDuration</span><span class="sxs-lookup"><span data-stu-id="cf06f-190">accountSetupDuration</span></span>|<span data-ttu-id="cf06f-191">持续时间</span><span class="sxs-lookup"><span data-stu-id="cf06f-191">Duration</span></span>|<span data-ttu-id="cf06f-192">用户 ESP 中所用的时间。</span><span class="sxs-lookup"><span data-stu-id="cf06f-192">Time spent in user ESP.</span></span>|
|<span data-ttu-id="cf06f-193">deploymentStartDateTime</span><span class="sxs-lookup"><span data-stu-id="cf06f-193">deploymentStartDateTime</span></span>|<span data-ttu-id="cf06f-194">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf06f-194">DateTimeOffset</span></span>|<span data-ttu-id="cf06f-195">部署开始时间。</span><span class="sxs-lookup"><span data-stu-id="cf06f-195">Deployment start time.</span></span>|
|<span data-ttu-id="cf06f-196">deploymentEndDateTime</span><span class="sxs-lookup"><span data-stu-id="cf06f-196">deploymentEndDateTime</span></span>|<span data-ttu-id="cf06f-197">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf06f-197">DateTimeOffset</span></span>|<span data-ttu-id="cf06f-198">部署结束时间。</span><span class="sxs-lookup"><span data-stu-id="cf06f-198">Deployment end time.</span></span>|
|<span data-ttu-id="cf06f-199">targetedAppCount</span><span class="sxs-lookup"><span data-stu-id="cf06f-199">targetedAppCount</span></span>|<span data-ttu-id="cf06f-200">Int32</span><span class="sxs-lookup"><span data-stu-id="cf06f-200">Int32</span></span>|<span data-ttu-id="cf06f-201">目标应用程序的计数。</span><span class="sxs-lookup"><span data-stu-id="cf06f-201">Count of applications targeted.</span></span>|
|<span data-ttu-id="cf06f-202">targetedPolicyCount</span><span class="sxs-lookup"><span data-stu-id="cf06f-202">targetedPolicyCount</span></span>|<span data-ttu-id="cf06f-203">Int32</span><span class="sxs-lookup"><span data-stu-id="cf06f-203">Int32</span></span>|<span data-ttu-id="cf06f-204">目标策略的计数。</span><span class="sxs-lookup"><span data-stu-id="cf06f-204">Count of policies targeted.</span></span>|
|<span data-ttu-id="cf06f-205">enrollmentFailureDetails</span><span class="sxs-lookup"><span data-stu-id="cf06f-205">enrollmentFailureDetails</span></span>|<span data-ttu-id="cf06f-206">String</span><span class="sxs-lookup"><span data-stu-id="cf06f-206">String</span></span>|<span data-ttu-id="cf06f-207">注册失败详细信息。</span><span class="sxs-lookup"><span data-stu-id="cf06f-207">Enrollment failure details.</span></span>|



## <a name="response"></a><span data-ttu-id="cf06f-208">响应</span><span class="sxs-lookup"><span data-stu-id="cf06f-208">Response</span></span>
<span data-ttu-id="cf06f-209">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md)对象。</span><span class="sxs-lookup"><span data-stu-id="cf06f-209">If successful, this method returns a `200 OK` response code and an updated [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf06f-210">示例</span><span class="sxs-lookup"><span data-stu-id="cf06f-210">Example</span></span>

### <a name="request"></a><span data-ttu-id="cf06f-211">请求</span><span class="sxs-lookup"><span data-stu-id="cf06f-211">Request</span></span>
<span data-ttu-id="cf06f-212">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cf06f-212">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/autopilotEvents/{deviceManagementAutopilotEventId}
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

### <a name="response"></a><span data-ttu-id="cf06f-213">响应</span><span class="sxs-lookup"><span data-stu-id="cf06f-213">Response</span></span>
<span data-ttu-id="cf06f-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cf06f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



