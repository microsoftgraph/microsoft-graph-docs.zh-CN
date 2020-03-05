---
title: 更新 deviceManagementAutopilotEvent
description: 更新 deviceManagementAutopilotEvent 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: db30ad9e855ae7371b055e033e4b1d8c6036125d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42457711"
---
# <a name="update-devicemanagementautopilotevent"></a><span data-ttu-id="9de5c-103">更新 deviceManagementAutopilotEvent</span><span class="sxs-lookup"><span data-stu-id="9de5c-103">Update deviceManagementAutopilotEvent</span></span>

<span data-ttu-id="9de5c-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="9de5c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9de5c-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9de5c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9de5c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9de5c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9de5c-107">更新[deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9de5c-107">Update the properties of a [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9de5c-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="9de5c-108">Prerequisites</span></span>
<span data-ttu-id="9de5c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9de5c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9de5c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9de5c-111">Permission type</span></span>|<span data-ttu-id="9de5c-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9de5c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9de5c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9de5c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9de5c-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9de5c-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="9de5c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9de5c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9de5c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9de5c-116">Not supported.</span></span>|
|<span data-ttu-id="9de5c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9de5c-117">Application</span></span>|<span data-ttu-id="9de5c-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9de5c-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9de5c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9de5c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/autopilotEvents/{deviceManagementAutopilotEventId}
```

## <a name="request-headers"></a><span data-ttu-id="9de5c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9de5c-120">Request headers</span></span>
|<span data-ttu-id="9de5c-121">标头</span><span class="sxs-lookup"><span data-stu-id="9de5c-121">Header</span></span>|<span data-ttu-id="9de5c-122">值</span><span class="sxs-lookup"><span data-stu-id="9de5c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9de5c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9de5c-123">Authorization</span></span>|<span data-ttu-id="9de5c-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9de5c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9de5c-125">接受</span><span class="sxs-lookup"><span data-stu-id="9de5c-125">Accept</span></span>|<span data-ttu-id="9de5c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9de5c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9de5c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9de5c-127">Request body</span></span>
<span data-ttu-id="9de5c-128">在请求正文中，提供[deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9de5c-128">In the request body, supply a JSON representation for the [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) object.</span></span>

<span data-ttu-id="9de5c-129">下表显示创建[deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="9de5c-129">The following table shows the properties that are required when you create the [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md).</span></span>

|<span data-ttu-id="9de5c-130">属性</span><span class="sxs-lookup"><span data-stu-id="9de5c-130">Property</span></span>|<span data-ttu-id="9de5c-131">类型</span><span class="sxs-lookup"><span data-stu-id="9de5c-131">Type</span></span>|<span data-ttu-id="9de5c-132">说明</span><span class="sxs-lookup"><span data-stu-id="9de5c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9de5c-133">id</span><span class="sxs-lookup"><span data-stu-id="9de5c-133">id</span></span>|<span data-ttu-id="9de5c-134">String</span><span class="sxs-lookup"><span data-stu-id="9de5c-134">String</span></span>|<span data-ttu-id="9de5c-135">对象的 UUID</span><span class="sxs-lookup"><span data-stu-id="9de5c-135">UUID for the object</span></span>|
|<span data-ttu-id="9de5c-136">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="9de5c-136">eventDateTime</span></span>|<span data-ttu-id="9de5c-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9de5c-137">DateTimeOffset</span></span>|<span data-ttu-id="9de5c-138">事件发生的时间。</span><span class="sxs-lookup"><span data-stu-id="9de5c-138">Time when the event occurred .</span></span>|
|<span data-ttu-id="9de5c-139">deviceRegisteredDateTime</span><span class="sxs-lookup"><span data-stu-id="9de5c-139">deviceRegisteredDateTime</span></span>|<span data-ttu-id="9de5c-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9de5c-140">DateTimeOffset</span></span>|<span data-ttu-id="9de5c-141">设备注册日期。</span><span class="sxs-lookup"><span data-stu-id="9de5c-141">Device registration date.</span></span>|
|<span data-ttu-id="9de5c-142">enrollmentStartDateTime</span><span class="sxs-lookup"><span data-stu-id="9de5c-142">enrollmentStartDateTime</span></span>|<span data-ttu-id="9de5c-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9de5c-143">DateTimeOffset</span></span>|<span data-ttu-id="9de5c-144">设备注册开始日期。</span><span class="sxs-lookup"><span data-stu-id="9de5c-144">Device enrollment start date.</span></span>|
|<span data-ttu-id="9de5c-145">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="9de5c-145">enrollmentType</span></span>|[<span data-ttu-id="9de5c-146">windowsAutopilotEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="9de5c-146">windowsAutopilotEnrollmentType</span></span>](../resources/intune-troubleshooting-windowsautopilotenrollmenttype.md)|<span data-ttu-id="9de5c-147">注册类型。</span><span class="sxs-lookup"><span data-stu-id="9de5c-147">Enrollment type.</span></span> <span data-ttu-id="9de5c-148">可取值为：`unknown`、`azureADJoinedWithAutopilotProfile`、`offlineDomainJoined`、`azureADJoinedUsingDeviceAuthWithAutopilotProfile`、`azureADJoinedUsingDeviceAuthWithoutAutopilotProfile`、`azureADJoinedWithOfflineAutopilotProfile`、`azureADJoinedWithWhiteGlove`、`offlineDomainJoinedWithWhiteGlove`、`offlineDomainJoinedWithOfflineAutopilotProfile`。</span><span class="sxs-lookup"><span data-stu-id="9de5c-148">Possible values are: `unknown`, `azureADJoinedWithAutopilotProfile`, `offlineDomainJoined`, `azureADJoinedUsingDeviceAuthWithAutopilotProfile`, `azureADJoinedUsingDeviceAuthWithoutAutopilotProfile`, `azureADJoinedWithOfflineAutopilotProfile`, `azureADJoinedWithWhiteGlove`, `offlineDomainJoinedWithWhiteGlove`, `offlineDomainJoinedWithOfflineAutopilotProfile`.</span></span>|
|<span data-ttu-id="9de5c-149">deviceSerialNumber</span><span class="sxs-lookup"><span data-stu-id="9de5c-149">deviceSerialNumber</span></span>|<span data-ttu-id="9de5c-150">String</span><span class="sxs-lookup"><span data-stu-id="9de5c-150">String</span></span>|<span data-ttu-id="9de5c-151">设备序列号。</span><span class="sxs-lookup"><span data-stu-id="9de5c-151">Device serial number.</span></span>|
|<span data-ttu-id="9de5c-152">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="9de5c-152">managedDeviceName</span></span>|<span data-ttu-id="9de5c-153">String</span><span class="sxs-lookup"><span data-stu-id="9de5c-153">String</span></span>|<span data-ttu-id="9de5c-154">托管设备名称。</span><span class="sxs-lookup"><span data-stu-id="9de5c-154">Managed device name.</span></span>|
|<span data-ttu-id="9de5c-155">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="9de5c-155">userPrincipalName</span></span>|<span data-ttu-id="9de5c-156">String</span><span class="sxs-lookup"><span data-stu-id="9de5c-156">String</span></span>|<span data-ttu-id="9de5c-157">用于注册设备的用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="9de5c-157">User principal name used to enroll the device.</span></span>|
|<span data-ttu-id="9de5c-158">windowsAutopilotDeploymentProfileDisplayName</span><span class="sxs-lookup"><span data-stu-id="9de5c-158">windowsAutopilotDeploymentProfileDisplayName</span></span>|<span data-ttu-id="9de5c-159">String</span><span class="sxs-lookup"><span data-stu-id="9de5c-159">String</span></span>|<span data-ttu-id="9de5c-160">Autopilot 配置文件名称。</span><span class="sxs-lookup"><span data-stu-id="9de5c-160">Autopilot profile name.</span></span>|
|<span data-ttu-id="9de5c-161">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="9de5c-161">enrollmentState</span></span>|[<span data-ttu-id="9de5c-162">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="9de5c-162">enrollmentState</span></span>](../resources/intune-shared-enrollmentstate.md)|<span data-ttu-id="9de5c-163">注册状态，如 "已注册"，失败。</span><span class="sxs-lookup"><span data-stu-id="9de5c-163">Enrollment state like Enrolled, Failed.</span></span> <span data-ttu-id="9de5c-164">可取值为：`unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="9de5c-164">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="9de5c-165">windows10EnrollmentCompletionPageConfigurationDisplayName</span><span class="sxs-lookup"><span data-stu-id="9de5c-165">windows10EnrollmentCompletionPageConfigurationDisplayName</span></span>|<span data-ttu-id="9de5c-166">String</span><span class="sxs-lookup"><span data-stu-id="9de5c-166">String</span></span>|<span data-ttu-id="9de5c-167">注册状态页面配置文件名称</span><span class="sxs-lookup"><span data-stu-id="9de5c-167">Enrollment Status Page profile name</span></span>|
|<span data-ttu-id="9de5c-168">deploymentState</span><span class="sxs-lookup"><span data-stu-id="9de5c-168">deploymentState</span></span>|[<span data-ttu-id="9de5c-169">windowsAutopilotDeploymentState</span><span class="sxs-lookup"><span data-stu-id="9de5c-169">windowsAutopilotDeploymentState</span></span>](../resources/intune-troubleshooting-windowsautopilotdeploymentstate.md)|<span data-ttu-id="9de5c-170">部署状态，如成功、失败、InProgress、SuccessWithTimeout。</span><span class="sxs-lookup"><span data-stu-id="9de5c-170">Deployment state like Success, Failure, InProgress, SuccessWithTimeout.</span></span> <span data-ttu-id="9de5c-171">可取值为：`unknown`、`success`、`inProgress`、`failure`、`successWithTimeout`。</span><span class="sxs-lookup"><span data-stu-id="9de5c-171">Possible values are: `unknown`, `success`, `inProgress`, `failure`, `successWithTimeout`.</span></span>|
|<span data-ttu-id="9de5c-172">osVersion</span><span class="sxs-lookup"><span data-stu-id="9de5c-172">osVersion</span></span>|<span data-ttu-id="9de5c-173">String</span><span class="sxs-lookup"><span data-stu-id="9de5c-173">String</span></span>|<span data-ttu-id="9de5c-174">设备操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="9de5c-174">Device operating system version.</span></span>|
|<span data-ttu-id="9de5c-175">deploymentDuration</span><span class="sxs-lookup"><span data-stu-id="9de5c-175">deploymentDuration</span></span>|<span data-ttu-id="9de5c-176">持续时间</span><span class="sxs-lookup"><span data-stu-id="9de5c-176">Duration</span></span>|<span data-ttu-id="9de5c-177">包含注册的 Autopilot 部署持续时间。</span><span class="sxs-lookup"><span data-stu-id="9de5c-177">Autopilot deployment duration including enrollment.</span></span>|
|<span data-ttu-id="9de5c-178">deploymentTotalDuration</span><span class="sxs-lookup"><span data-stu-id="9de5c-178">deploymentTotalDuration</span></span>|<span data-ttu-id="9de5c-179">持续时间</span><span class="sxs-lookup"><span data-stu-id="9de5c-179">Duration</span></span>|<span data-ttu-id="9de5c-180">从注册到桌面屏幕的总部署持续时间。</span><span class="sxs-lookup"><span data-stu-id="9de5c-180">Total deployment duration from enrollment to Desktop screen.</span></span>|
|<span data-ttu-id="9de5c-181">devicePreparationDuration</span><span class="sxs-lookup"><span data-stu-id="9de5c-181">devicePreparationDuration</span></span>|<span data-ttu-id="9de5c-182">持续时间</span><span class="sxs-lookup"><span data-stu-id="9de5c-182">Duration</span></span>|<span data-ttu-id="9de5c-183">在设备注册中花费的时间。</span><span class="sxs-lookup"><span data-stu-id="9de5c-183">Time spent in device enrollment.</span></span>|
|<span data-ttu-id="9de5c-184">deviceSetupDuration</span><span class="sxs-lookup"><span data-stu-id="9de5c-184">deviceSetupDuration</span></span>|<span data-ttu-id="9de5c-185">持续时间</span><span class="sxs-lookup"><span data-stu-id="9de5c-185">Duration</span></span>|<span data-ttu-id="9de5c-186">在设备 ESP 中花费的时间。</span><span class="sxs-lookup"><span data-stu-id="9de5c-186">Time spent in device ESP.</span></span>|
|<span data-ttu-id="9de5c-187">accountSetupDuration</span><span class="sxs-lookup"><span data-stu-id="9de5c-187">accountSetupDuration</span></span>|<span data-ttu-id="9de5c-188">持续时间</span><span class="sxs-lookup"><span data-stu-id="9de5c-188">Duration</span></span>|<span data-ttu-id="9de5c-189">用户 ESP 中所用的时间。</span><span class="sxs-lookup"><span data-stu-id="9de5c-189">Time spent in user ESP.</span></span>|
|<span data-ttu-id="9de5c-190">deploymentStartDateTime</span><span class="sxs-lookup"><span data-stu-id="9de5c-190">deploymentStartDateTime</span></span>|<span data-ttu-id="9de5c-191">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9de5c-191">DateTimeOffset</span></span>|<span data-ttu-id="9de5c-192">部署开始时间。</span><span class="sxs-lookup"><span data-stu-id="9de5c-192">Deployment start time.</span></span>|
|<span data-ttu-id="9de5c-193">deploymentEndDateTime</span><span class="sxs-lookup"><span data-stu-id="9de5c-193">deploymentEndDateTime</span></span>|<span data-ttu-id="9de5c-194">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9de5c-194">DateTimeOffset</span></span>|<span data-ttu-id="9de5c-195">部署结束时间。</span><span class="sxs-lookup"><span data-stu-id="9de5c-195">Deployment end time.</span></span>|
|<span data-ttu-id="9de5c-196">targetedAppCount</span><span class="sxs-lookup"><span data-stu-id="9de5c-196">targetedAppCount</span></span>|<span data-ttu-id="9de5c-197">Int32</span><span class="sxs-lookup"><span data-stu-id="9de5c-197">Int32</span></span>|<span data-ttu-id="9de5c-198">目标应用程序的计数。</span><span class="sxs-lookup"><span data-stu-id="9de5c-198">Count of applications targeted.</span></span>|
|<span data-ttu-id="9de5c-199">targetedPolicyCount</span><span class="sxs-lookup"><span data-stu-id="9de5c-199">targetedPolicyCount</span></span>|<span data-ttu-id="9de5c-200">Int32</span><span class="sxs-lookup"><span data-stu-id="9de5c-200">Int32</span></span>|<span data-ttu-id="9de5c-201">目标策略的计数。</span><span class="sxs-lookup"><span data-stu-id="9de5c-201">Count of policies targeted.</span></span>|
|<span data-ttu-id="9de5c-202">enrollmentFailureDetails</span><span class="sxs-lookup"><span data-stu-id="9de5c-202">enrollmentFailureDetails</span></span>|<span data-ttu-id="9de5c-203">String</span><span class="sxs-lookup"><span data-stu-id="9de5c-203">String</span></span>|<span data-ttu-id="9de5c-204">注册失败详细信息。</span><span class="sxs-lookup"><span data-stu-id="9de5c-204">Enrollment failure details.</span></span>|



## <a name="response"></a><span data-ttu-id="9de5c-205">响应</span><span class="sxs-lookup"><span data-stu-id="9de5c-205">Response</span></span>
<span data-ttu-id="9de5c-206">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9de5c-206">If successful, this method returns a `200 OK` response code and an updated [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9de5c-207">示例</span><span class="sxs-lookup"><span data-stu-id="9de5c-207">Example</span></span>

### <a name="request"></a><span data-ttu-id="9de5c-208">请求</span><span class="sxs-lookup"><span data-stu-id="9de5c-208">Request</span></span>
<span data-ttu-id="9de5c-209">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9de5c-209">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9de5c-210">响应</span><span class="sxs-lookup"><span data-stu-id="9de5c-210">Response</span></span>
<span data-ttu-id="9de5c-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9de5c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





