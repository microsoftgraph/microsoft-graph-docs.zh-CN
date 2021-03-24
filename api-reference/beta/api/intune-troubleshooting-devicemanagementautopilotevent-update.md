---
title: 更新 deviceManagementAutopilotEvent
description: 更新 deviceManagementAutopilotEvent 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f97cdb540d33de6a2ac9f919093dba5d534a32c6
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51134212"
---
# <a name="update-devicemanagementautopilotevent"></a><span data-ttu-id="a053e-103">更新 deviceManagementAutopilotEvent</span><span class="sxs-lookup"><span data-stu-id="a053e-103">Update deviceManagementAutopilotEvent</span></span>

<span data-ttu-id="a053e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a053e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a053e-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a053e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a053e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a053e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a053e-107">更新 [deviceManagementAutopilotEvent 对象](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="a053e-107">Update the properties of a [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a053e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="a053e-108">Prerequisites</span></span>
<span data-ttu-id="a053e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a053e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a053e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a053e-111">Permission type</span></span>|<span data-ttu-id="a053e-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a053e-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a053e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a053e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a053e-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a053e-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="a053e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a053e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a053e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a053e-116">Not supported.</span></span>|
|<span data-ttu-id="a053e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a053e-117">Application</span></span>|<span data-ttu-id="a053e-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a053e-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a053e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a053e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/autopilotEvents/{deviceManagementAutopilotEventId}
```

## <a name="request-headers"></a><span data-ttu-id="a053e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a053e-120">Request headers</span></span>
|<span data-ttu-id="a053e-121">标头</span><span class="sxs-lookup"><span data-stu-id="a053e-121">Header</span></span>|<span data-ttu-id="a053e-122">值</span><span class="sxs-lookup"><span data-stu-id="a053e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a053e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a053e-123">Authorization</span></span>|<span data-ttu-id="a053e-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a053e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a053e-125">接受</span><span class="sxs-lookup"><span data-stu-id="a053e-125">Accept</span></span>|<span data-ttu-id="a053e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a053e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a053e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a053e-127">Request body</span></span>
<span data-ttu-id="a053e-128">在请求正文中，提供 [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a053e-128">In the request body, supply a JSON representation for the [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) object.</span></span>

<span data-ttu-id="a053e-129">下表显示创建 [deviceManagementAutopilotEvent 时所需的属性](../resources/intune-troubleshooting-devicemanagementautopilotevent.md)。</span><span class="sxs-lookup"><span data-stu-id="a053e-129">The following table shows the properties that are required when you create the [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md).</span></span>

|<span data-ttu-id="a053e-130">属性</span><span class="sxs-lookup"><span data-stu-id="a053e-130">Property</span></span>|<span data-ttu-id="a053e-131">类型</span><span class="sxs-lookup"><span data-stu-id="a053e-131">Type</span></span>|<span data-ttu-id="a053e-132">说明</span><span class="sxs-lookup"><span data-stu-id="a053e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a053e-133">id</span><span class="sxs-lookup"><span data-stu-id="a053e-133">id</span></span>|<span data-ttu-id="a053e-134">String</span><span class="sxs-lookup"><span data-stu-id="a053e-134">String</span></span>|<span data-ttu-id="a053e-135">对象的 UUID</span><span class="sxs-lookup"><span data-stu-id="a053e-135">UUID for the object</span></span>|
|<span data-ttu-id="a053e-136">deviceId</span><span class="sxs-lookup"><span data-stu-id="a053e-136">deviceId</span></span>|<span data-ttu-id="a053e-137">String</span><span class="sxs-lookup"><span data-stu-id="a053e-137">String</span></span>|<span data-ttu-id="a053e-138">与对象关联的设备 ID</span><span class="sxs-lookup"><span data-stu-id="a053e-138">Device id associated with the object</span></span>|
|<span data-ttu-id="a053e-139">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="a053e-139">eventDateTime</span></span>|<span data-ttu-id="a053e-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a053e-140">DateTimeOffset</span></span>|<span data-ttu-id="a053e-141">事件发生的时间。</span><span class="sxs-lookup"><span data-stu-id="a053e-141">Time when the event occurred .</span></span>|
|<span data-ttu-id="a053e-142">deviceRegisteredDateTime</span><span class="sxs-lookup"><span data-stu-id="a053e-142">deviceRegisteredDateTime</span></span>|<span data-ttu-id="a053e-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a053e-143">DateTimeOffset</span></span>|<span data-ttu-id="a053e-144">设备注册日期。</span><span class="sxs-lookup"><span data-stu-id="a053e-144">Device registration date.</span></span>|
|<span data-ttu-id="a053e-145">enrollmentStartDateTime</span><span class="sxs-lookup"><span data-stu-id="a053e-145">enrollmentStartDateTime</span></span>|<span data-ttu-id="a053e-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a053e-146">DateTimeOffset</span></span>|<span data-ttu-id="a053e-147">设备注册开始日期。</span><span class="sxs-lookup"><span data-stu-id="a053e-147">Device enrollment start date.</span></span>|
|<span data-ttu-id="a053e-148">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="a053e-148">enrollmentType</span></span>|[<span data-ttu-id="a053e-149">windowsAutopilotEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="a053e-149">windowsAutopilotEnrollmentType</span></span>](../resources/intune-troubleshooting-windowsautopilotenrollmenttype.md)|<span data-ttu-id="a053e-150">注册类型。</span><span class="sxs-lookup"><span data-stu-id="a053e-150">Enrollment type.</span></span> <span data-ttu-id="a053e-151">可取值为：`unknown`、`azureADJoinedWithAutopilotProfile`、`offlineDomainJoined`、`azureADJoinedUsingDeviceAuthWithAutopilotProfile`、`azureADJoinedUsingDeviceAuthWithoutAutopilotProfile`、`azureADJoinedWithOfflineAutopilotProfile`、`azureADJoinedWithWhiteGlove`、`offlineDomainJoinedWithWhiteGlove`、`offlineDomainJoinedWithOfflineAutopilotProfile`。</span><span class="sxs-lookup"><span data-stu-id="a053e-151">Possible values are: `unknown`, `azureADJoinedWithAutopilotProfile`, `offlineDomainJoined`, `azureADJoinedUsingDeviceAuthWithAutopilotProfile`, `azureADJoinedUsingDeviceAuthWithoutAutopilotProfile`, `azureADJoinedWithOfflineAutopilotProfile`, `azureADJoinedWithWhiteGlove`, `offlineDomainJoinedWithWhiteGlove`, `offlineDomainJoinedWithOfflineAutopilotProfile`.</span></span>|
|<span data-ttu-id="a053e-152">deviceSerialNumber</span><span class="sxs-lookup"><span data-stu-id="a053e-152">deviceSerialNumber</span></span>|<span data-ttu-id="a053e-153">String</span><span class="sxs-lookup"><span data-stu-id="a053e-153">String</span></span>|<span data-ttu-id="a053e-154">设备序列号。</span><span class="sxs-lookup"><span data-stu-id="a053e-154">Device serial number.</span></span>|
|<span data-ttu-id="a053e-155">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="a053e-155">managedDeviceName</span></span>|<span data-ttu-id="a053e-156">String</span><span class="sxs-lookup"><span data-stu-id="a053e-156">String</span></span>|<span data-ttu-id="a053e-157">托管设备名称。</span><span class="sxs-lookup"><span data-stu-id="a053e-157">Managed device name.</span></span>|
|<span data-ttu-id="a053e-158">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a053e-158">userPrincipalName</span></span>|<span data-ttu-id="a053e-159">String</span><span class="sxs-lookup"><span data-stu-id="a053e-159">String</span></span>|<span data-ttu-id="a053e-160">用于注册设备的用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="a053e-160">User principal name used to enroll the device.</span></span>|
|<span data-ttu-id="a053e-161">windowsAutopilotDeploymentProfileDisplayName</span><span class="sxs-lookup"><span data-stu-id="a053e-161">windowsAutopilotDeploymentProfileDisplayName</span></span>|<span data-ttu-id="a053e-162">String</span><span class="sxs-lookup"><span data-stu-id="a053e-162">String</span></span>|<span data-ttu-id="a053e-163">Autopilot 配置文件名称。</span><span class="sxs-lookup"><span data-stu-id="a053e-163">Autopilot profile name.</span></span>|
|<span data-ttu-id="a053e-164">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="a053e-164">enrollmentState</span></span>|[<span data-ttu-id="a053e-165">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="a053e-165">enrollmentState</span></span>](../resources/intune-shared-enrollmentstate.md)|<span data-ttu-id="a053e-166">注册状态，如已注册、已失败。</span><span class="sxs-lookup"><span data-stu-id="a053e-166">Enrollment state like Enrolled, Failed.</span></span> <span data-ttu-id="a053e-167">可取值为：`unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="a053e-167">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="a053e-168">windows10EnrollmentCompletionPageConfigurationDisplayName</span><span class="sxs-lookup"><span data-stu-id="a053e-168">windows10EnrollmentCompletionPageConfigurationDisplayName</span></span>|<span data-ttu-id="a053e-169">String</span><span class="sxs-lookup"><span data-stu-id="a053e-169">String</span></span>|<span data-ttu-id="a053e-170">注册状态页面配置文件名称</span><span class="sxs-lookup"><span data-stu-id="a053e-170">Enrollment Status Page profile name</span></span>|
|<span data-ttu-id="a053e-171">windows10EnrollmentCompletionPageConfigurationId</span><span class="sxs-lookup"><span data-stu-id="a053e-171">windows10EnrollmentCompletionPageConfigurationId</span></span>|<span data-ttu-id="a053e-172">String</span><span class="sxs-lookup"><span data-stu-id="a053e-172">String</span></span>|<span data-ttu-id="a053e-173">注册状态页面配置文件 ID</span><span class="sxs-lookup"><span data-stu-id="a053e-173">Enrollment Status Page profile ID</span></span>|
|<span data-ttu-id="a053e-174">deploymentState</span><span class="sxs-lookup"><span data-stu-id="a053e-174">deploymentState</span></span>|[<span data-ttu-id="a053e-175">windowsAutopilotDeploymentState</span><span class="sxs-lookup"><span data-stu-id="a053e-175">windowsAutopilotDeploymentState</span></span>](../resources/intune-troubleshooting-windowsautopilotdeploymentstate.md)|<span data-ttu-id="a053e-176">部署状态，如 Success、Failure、InProgress、SuccessWithTimeout。</span><span class="sxs-lookup"><span data-stu-id="a053e-176">Deployment state like Success, Failure, InProgress, SuccessWithTimeout.</span></span> <span data-ttu-id="a053e-177">可取值为：`unknown`、`success`、`inProgress`、`failure`、`successWithTimeout`、`notAttempted` 或 `disabled`。</span><span class="sxs-lookup"><span data-stu-id="a053e-177">Possible values are: `unknown`, `success`, `inProgress`, `failure`, `successWithTimeout`, `notAttempted`, `disabled`.</span></span>|
|<span data-ttu-id="a053e-178">deviceSetupStatus</span><span class="sxs-lookup"><span data-stu-id="a053e-178">deviceSetupStatus</span></span>|[<span data-ttu-id="a053e-179">windowsAutopilotDeploymentState</span><span class="sxs-lookup"><span data-stu-id="a053e-179">windowsAutopilotDeploymentState</span></span>](../resources/intune-troubleshooting-windowsautopilotdeploymentstate.md)|<span data-ttu-id="a053e-180">注册状态页设备设置阶段的部署状态。</span><span class="sxs-lookup"><span data-stu-id="a053e-180">Deployment status for the enrollment status page device setup phase.</span></span> <span data-ttu-id="a053e-181">可取值为：`unknown`、`success`、`inProgress`、`failure`、`successWithTimeout`、`notAttempted` 或 `disabled`。</span><span class="sxs-lookup"><span data-stu-id="a053e-181">Possible values are: `unknown`, `success`, `inProgress`, `failure`, `successWithTimeout`, `notAttempted`, `disabled`.</span></span>|
|<span data-ttu-id="a053e-182">accountSetupStatus</span><span class="sxs-lookup"><span data-stu-id="a053e-182">accountSetupStatus</span></span>|[<span data-ttu-id="a053e-183">windowsAutopilotDeploymentState</span><span class="sxs-lookup"><span data-stu-id="a053e-183">windowsAutopilotDeploymentState</span></span>](../resources/intune-troubleshooting-windowsautopilotdeploymentstate.md)|<span data-ttu-id="a053e-184">注册状态页帐户设置阶段的部署状态。</span><span class="sxs-lookup"><span data-stu-id="a053e-184">Deployment status for the enrollment status page account setup phase.</span></span> <span data-ttu-id="a053e-185">可取值为：`unknown`、`success`、`inProgress`、`failure`、`successWithTimeout`、`notAttempted` 或 `disabled`。</span><span class="sxs-lookup"><span data-stu-id="a053e-185">Possible values are: `unknown`, `success`, `inProgress`, `failure`, `successWithTimeout`, `notAttempted`, `disabled`.</span></span>|
|<span data-ttu-id="a053e-186">osVersion</span><span class="sxs-lookup"><span data-stu-id="a053e-186">osVersion</span></span>|<span data-ttu-id="a053e-187">String</span><span class="sxs-lookup"><span data-stu-id="a053e-187">String</span></span>|<span data-ttu-id="a053e-188">设备操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="a053e-188">Device operating system version.</span></span>|
|<span data-ttu-id="a053e-189">deploymentDuration</span><span class="sxs-lookup"><span data-stu-id="a053e-189">deploymentDuration</span></span>|<span data-ttu-id="a053e-190">持续时间</span><span class="sxs-lookup"><span data-stu-id="a053e-190">Duration</span></span>|<span data-ttu-id="a053e-191">Autopilot 部署持续时间（包括注册）。</span><span class="sxs-lookup"><span data-stu-id="a053e-191">Autopilot deployment duration including enrollment.</span></span>|
|<span data-ttu-id="a053e-192">deploymentTotalDuration</span><span class="sxs-lookup"><span data-stu-id="a053e-192">deploymentTotalDuration</span></span>|<span data-ttu-id="a053e-193">持续时间</span><span class="sxs-lookup"><span data-stu-id="a053e-193">Duration</span></span>|<span data-ttu-id="a053e-194">从注册到桌面屏幕的总部署持续时间。</span><span class="sxs-lookup"><span data-stu-id="a053e-194">Total deployment duration from enrollment to Desktop screen.</span></span>|
|<span data-ttu-id="a053e-195">devicePreparationDuration</span><span class="sxs-lookup"><span data-stu-id="a053e-195">devicePreparationDuration</span></span>|<span data-ttu-id="a053e-196">持续时间</span><span class="sxs-lookup"><span data-stu-id="a053e-196">Duration</span></span>|<span data-ttu-id="a053e-197">设备注册所花费的时间。</span><span class="sxs-lookup"><span data-stu-id="a053e-197">Time spent in device enrollment.</span></span>|
|<span data-ttu-id="a053e-198">deviceSetupDuration</span><span class="sxs-lookup"><span data-stu-id="a053e-198">deviceSetupDuration</span></span>|<span data-ttu-id="a053e-199">持续时间</span><span class="sxs-lookup"><span data-stu-id="a053e-199">Duration</span></span>|<span data-ttu-id="a053e-200">在设备 ESP 上花费的时间。</span><span class="sxs-lookup"><span data-stu-id="a053e-200">Time spent in device ESP.</span></span>|
|<span data-ttu-id="a053e-201">accountSetupDuration</span><span class="sxs-lookup"><span data-stu-id="a053e-201">accountSetupDuration</span></span>|<span data-ttu-id="a053e-202">持续时间</span><span class="sxs-lookup"><span data-stu-id="a053e-202">Duration</span></span>|<span data-ttu-id="a053e-203">在用户 ESP 中花费的时间。</span><span class="sxs-lookup"><span data-stu-id="a053e-203">Time spent in user ESP.</span></span>|
|<span data-ttu-id="a053e-204">deploymentStartDateTime</span><span class="sxs-lookup"><span data-stu-id="a053e-204">deploymentStartDateTime</span></span>|<span data-ttu-id="a053e-205">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a053e-205">DateTimeOffset</span></span>|<span data-ttu-id="a053e-206">部署开始时间。</span><span class="sxs-lookup"><span data-stu-id="a053e-206">Deployment start time.</span></span>|
|<span data-ttu-id="a053e-207">deploymentEndDateTime</span><span class="sxs-lookup"><span data-stu-id="a053e-207">deploymentEndDateTime</span></span>|<span data-ttu-id="a053e-208">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a053e-208">DateTimeOffset</span></span>|<span data-ttu-id="a053e-209">部署结束时间。</span><span class="sxs-lookup"><span data-stu-id="a053e-209">Deployment end time.</span></span>|
|<span data-ttu-id="a053e-210">targetedAppCount</span><span class="sxs-lookup"><span data-stu-id="a053e-210">targetedAppCount</span></span>|<span data-ttu-id="a053e-211">Int32</span><span class="sxs-lookup"><span data-stu-id="a053e-211">Int32</span></span>|<span data-ttu-id="a053e-212">目标应用程序计数。</span><span class="sxs-lookup"><span data-stu-id="a053e-212">Count of applications targeted.</span></span>|
|<span data-ttu-id="a053e-213">targetedPolicyCount</span><span class="sxs-lookup"><span data-stu-id="a053e-213">targetedPolicyCount</span></span>|<span data-ttu-id="a053e-214">Int32</span><span class="sxs-lookup"><span data-stu-id="a053e-214">Int32</span></span>|<span data-ttu-id="a053e-215">目标策略计数。</span><span class="sxs-lookup"><span data-stu-id="a053e-215">Count of policies targeted.</span></span>|
|<span data-ttu-id="a053e-216">enrollmentFailureDetails</span><span class="sxs-lookup"><span data-stu-id="a053e-216">enrollmentFailureDetails</span></span>|<span data-ttu-id="a053e-217">String</span><span class="sxs-lookup"><span data-stu-id="a053e-217">String</span></span>|<span data-ttu-id="a053e-218">注册失败详细信息。</span><span class="sxs-lookup"><span data-stu-id="a053e-218">Enrollment failure details.</span></span>|



## <a name="response"></a><span data-ttu-id="a053e-219">响应</span><span class="sxs-lookup"><span data-stu-id="a053e-219">Response</span></span>
<span data-ttu-id="a053e-220">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a053e-220">If successful, this method returns a `200 OK` response code and an updated [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a053e-221">示例</span><span class="sxs-lookup"><span data-stu-id="a053e-221">Example</span></span>

### <a name="request"></a><span data-ttu-id="a053e-222">请求</span><span class="sxs-lookup"><span data-stu-id="a053e-222">Request</span></span>
<span data-ttu-id="a053e-223">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a053e-223">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/autopilotEvents/{deviceManagementAutopilotEventId}
Content-type: application/json
Content-length: 1545

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
  "windows10EnrollmentCompletionPageConfigurationId": "Windows10Enrollment Completion Page Configuration Id value",
  "deploymentState": "success",
  "deviceSetupStatus": "success",
  "accountSetupStatus": "success",
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

### <a name="response"></a><span data-ttu-id="a053e-224">响应</span><span class="sxs-lookup"><span data-stu-id="a053e-224">Response</span></span>
<span data-ttu-id="a053e-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a053e-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1594

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
  "windows10EnrollmentCompletionPageConfigurationId": "Windows10Enrollment Completion Page Configuration Id value",
  "deploymentState": "success",
  "deviceSetupStatus": "success",
  "accountSetupStatus": "success",
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




