---
title: 创建 deviceManagementAutopilotEvent
description: 创建新的 deviceManagementAutopilotEvent 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 411e7dd15a8f3fe75d726f0caab38c7592b3a8a6
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159211"
---
# <a name="create-devicemanagementautopilotevent"></a><span data-ttu-id="c81ec-103">创建 deviceManagementAutopilotEvent</span><span class="sxs-lookup"><span data-stu-id="c81ec-103">Create deviceManagementAutopilotEvent</span></span>

<span data-ttu-id="c81ec-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c81ec-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c81ec-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c81ec-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c81ec-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c81ec-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c81ec-107">创建新的 [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c81ec-107">Create a new [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c81ec-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="c81ec-108">Prerequisites</span></span>
<span data-ttu-id="c81ec-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c81ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c81ec-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c81ec-111">Permission type</span></span>|<span data-ttu-id="c81ec-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c81ec-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c81ec-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c81ec-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c81ec-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c81ec-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="c81ec-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c81ec-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c81ec-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c81ec-116">Not supported.</span></span>|
|<span data-ttu-id="c81ec-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c81ec-117">Application</span></span>|<span data-ttu-id="c81ec-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c81ec-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c81ec-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c81ec-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/autopilotEvents
```

## <a name="request-headers"></a><span data-ttu-id="c81ec-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c81ec-120">Request headers</span></span>
|<span data-ttu-id="c81ec-121">标头</span><span class="sxs-lookup"><span data-stu-id="c81ec-121">Header</span></span>|<span data-ttu-id="c81ec-122">值</span><span class="sxs-lookup"><span data-stu-id="c81ec-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c81ec-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c81ec-123">Authorization</span></span>|<span data-ttu-id="c81ec-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c81ec-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c81ec-125">接受</span><span class="sxs-lookup"><span data-stu-id="c81ec-125">Accept</span></span>|<span data-ttu-id="c81ec-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c81ec-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c81ec-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c81ec-127">Request body</span></span>
<span data-ttu-id="c81ec-128">在请求正文中，提供 deviceManagementAutopilotEvent 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c81ec-128">In the request body, supply a JSON representation for the deviceManagementAutopilotEvent object.</span></span>

<span data-ttu-id="c81ec-129">下表显示创建 deviceManagementAutopilotEvent 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c81ec-129">The following table shows the properties that are required when you create the deviceManagementAutopilotEvent.</span></span>

|<span data-ttu-id="c81ec-130">属性</span><span class="sxs-lookup"><span data-stu-id="c81ec-130">Property</span></span>|<span data-ttu-id="c81ec-131">类型</span><span class="sxs-lookup"><span data-stu-id="c81ec-131">Type</span></span>|<span data-ttu-id="c81ec-132">说明</span><span class="sxs-lookup"><span data-stu-id="c81ec-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c81ec-133">id</span><span class="sxs-lookup"><span data-stu-id="c81ec-133">id</span></span>|<span data-ttu-id="c81ec-134">String</span><span class="sxs-lookup"><span data-stu-id="c81ec-134">String</span></span>|<span data-ttu-id="c81ec-135">对象的 UUID</span><span class="sxs-lookup"><span data-stu-id="c81ec-135">UUID for the object</span></span>|
|<span data-ttu-id="c81ec-136">deviceId</span><span class="sxs-lookup"><span data-stu-id="c81ec-136">deviceId</span></span>|<span data-ttu-id="c81ec-137">String</span><span class="sxs-lookup"><span data-stu-id="c81ec-137">String</span></span>|<span data-ttu-id="c81ec-138">与对象关联的设备 ID</span><span class="sxs-lookup"><span data-stu-id="c81ec-138">Device id associated with the object</span></span>|
|<span data-ttu-id="c81ec-139">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="c81ec-139">eventDateTime</span></span>|<span data-ttu-id="c81ec-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c81ec-140">DateTimeOffset</span></span>|<span data-ttu-id="c81ec-141">事件发生的时间。</span><span class="sxs-lookup"><span data-stu-id="c81ec-141">Time when the event occurred .</span></span>|
|<span data-ttu-id="c81ec-142">deviceRegisteredDateTime</span><span class="sxs-lookup"><span data-stu-id="c81ec-142">deviceRegisteredDateTime</span></span>|<span data-ttu-id="c81ec-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c81ec-143">DateTimeOffset</span></span>|<span data-ttu-id="c81ec-144">设备注册日期。</span><span class="sxs-lookup"><span data-stu-id="c81ec-144">Device registration date.</span></span>|
|<span data-ttu-id="c81ec-145">enrollmentStartDateTime</span><span class="sxs-lookup"><span data-stu-id="c81ec-145">enrollmentStartDateTime</span></span>|<span data-ttu-id="c81ec-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c81ec-146">DateTimeOffset</span></span>|<span data-ttu-id="c81ec-147">设备注册开始日期。</span><span class="sxs-lookup"><span data-stu-id="c81ec-147">Device enrollment start date.</span></span>|
|<span data-ttu-id="c81ec-148">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="c81ec-148">enrollmentType</span></span>|[<span data-ttu-id="c81ec-149">windowsAutopilotEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="c81ec-149">windowsAutopilotEnrollmentType</span></span>](../resources/intune-troubleshooting-windowsautopilotenrollmenttype.md)|<span data-ttu-id="c81ec-150">注册类型。</span><span class="sxs-lookup"><span data-stu-id="c81ec-150">Enrollment type.</span></span> <span data-ttu-id="c81ec-151">可取值为：`unknown`、`azureADJoinedWithAutopilotProfile`、`offlineDomainJoined`、`azureADJoinedUsingDeviceAuthWithAutopilotProfile`、`azureADJoinedUsingDeviceAuthWithoutAutopilotProfile`、`azureADJoinedWithOfflineAutopilotProfile`、`azureADJoinedWithWhiteGlove`、`offlineDomainJoinedWithWhiteGlove`、`offlineDomainJoinedWithOfflineAutopilotProfile`。</span><span class="sxs-lookup"><span data-stu-id="c81ec-151">Possible values are: `unknown`, `azureADJoinedWithAutopilotProfile`, `offlineDomainJoined`, `azureADJoinedUsingDeviceAuthWithAutopilotProfile`, `azureADJoinedUsingDeviceAuthWithoutAutopilotProfile`, `azureADJoinedWithOfflineAutopilotProfile`, `azureADJoinedWithWhiteGlove`, `offlineDomainJoinedWithWhiteGlove`, `offlineDomainJoinedWithOfflineAutopilotProfile`.</span></span>|
|<span data-ttu-id="c81ec-152">deviceSerialNumber</span><span class="sxs-lookup"><span data-stu-id="c81ec-152">deviceSerialNumber</span></span>|<span data-ttu-id="c81ec-153">String</span><span class="sxs-lookup"><span data-stu-id="c81ec-153">String</span></span>|<span data-ttu-id="c81ec-154">设备序列号。</span><span class="sxs-lookup"><span data-stu-id="c81ec-154">Device serial number.</span></span>|
|<span data-ttu-id="c81ec-155">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="c81ec-155">managedDeviceName</span></span>|<span data-ttu-id="c81ec-156">String</span><span class="sxs-lookup"><span data-stu-id="c81ec-156">String</span></span>|<span data-ttu-id="c81ec-157">托管设备名称。</span><span class="sxs-lookup"><span data-stu-id="c81ec-157">Managed device name.</span></span>|
|<span data-ttu-id="c81ec-158">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c81ec-158">userPrincipalName</span></span>|<span data-ttu-id="c81ec-159">String</span><span class="sxs-lookup"><span data-stu-id="c81ec-159">String</span></span>|<span data-ttu-id="c81ec-160">用于注册设备的用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="c81ec-160">User principal name used to enroll the device.</span></span>|
|<span data-ttu-id="c81ec-161">windowsAutopilotDeploymentProfileDisplayName</span><span class="sxs-lookup"><span data-stu-id="c81ec-161">windowsAutopilotDeploymentProfileDisplayName</span></span>|<span data-ttu-id="c81ec-162">String</span><span class="sxs-lookup"><span data-stu-id="c81ec-162">String</span></span>|<span data-ttu-id="c81ec-163">Autopilot 配置文件名称。</span><span class="sxs-lookup"><span data-stu-id="c81ec-163">Autopilot profile name.</span></span>|
|<span data-ttu-id="c81ec-164">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="c81ec-164">enrollmentState</span></span>|[<span data-ttu-id="c81ec-165">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="c81ec-165">enrollmentState</span></span>](../resources/intune-shared-enrollmentstate.md)|<span data-ttu-id="c81ec-166">注册状态，如已注册、失败。</span><span class="sxs-lookup"><span data-stu-id="c81ec-166">Enrollment state like Enrolled, Failed.</span></span> <span data-ttu-id="c81ec-167">可取值为：`unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="c81ec-167">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="c81ec-168">windows10EnrollmentCompletionPageConfigurationDisplayName</span><span class="sxs-lookup"><span data-stu-id="c81ec-168">windows10EnrollmentCompletionPageConfigurationDisplayName</span></span>|<span data-ttu-id="c81ec-169">String</span><span class="sxs-lookup"><span data-stu-id="c81ec-169">String</span></span>|<span data-ttu-id="c81ec-170">注册状态页面配置文件名称</span><span class="sxs-lookup"><span data-stu-id="c81ec-170">Enrollment Status Page profile name</span></span>|
|<span data-ttu-id="c81ec-171">windows10EnrollmentCompletionPageConfigurationId</span><span class="sxs-lookup"><span data-stu-id="c81ec-171">windows10EnrollmentCompletionPageConfigurationId</span></span>|<span data-ttu-id="c81ec-172">String</span><span class="sxs-lookup"><span data-stu-id="c81ec-172">String</span></span>|<span data-ttu-id="c81ec-173">注册状态页面配置文件 ID</span><span class="sxs-lookup"><span data-stu-id="c81ec-173">Enrollment Status Page profile ID</span></span>|
|<span data-ttu-id="c81ec-174">deploymentState</span><span class="sxs-lookup"><span data-stu-id="c81ec-174">deploymentState</span></span>|[<span data-ttu-id="c81ec-175">windowsAutopilotDeploymentState</span><span class="sxs-lookup"><span data-stu-id="c81ec-175">windowsAutopilotDeploymentState</span></span>](../resources/intune-troubleshooting-windowsautopilotdeploymentstate.md)|<span data-ttu-id="c81ec-176">部署状态，如 Success、Failure、InProgress、SuccessWithTimeout。</span><span class="sxs-lookup"><span data-stu-id="c81ec-176">Deployment state like Success, Failure, InProgress, SuccessWithTimeout.</span></span> <span data-ttu-id="c81ec-177">可取值为：`unknown`、`success`、`inProgress`、`failure`、`successWithTimeout`、`notAttempted` 或 `disabled`。</span><span class="sxs-lookup"><span data-stu-id="c81ec-177">Possible values are: `unknown`, `success`, `inProgress`, `failure`, `successWithTimeout`, `notAttempted`, `disabled`.</span></span>|
|<span data-ttu-id="c81ec-178">deviceSetupStatus</span><span class="sxs-lookup"><span data-stu-id="c81ec-178">deviceSetupStatus</span></span>|[<span data-ttu-id="c81ec-179">windowsAutopilotDeploymentState</span><span class="sxs-lookup"><span data-stu-id="c81ec-179">windowsAutopilotDeploymentState</span></span>](../resources/intune-troubleshooting-windowsautopilotdeploymentstate.md)|<span data-ttu-id="c81ec-180">注册状态页设备设置阶段的部署状态。</span><span class="sxs-lookup"><span data-stu-id="c81ec-180">Deployment status for the enrollment status page device setup phase.</span></span> <span data-ttu-id="c81ec-181">可取值为：`unknown`、`success`、`inProgress`、`failure`、`successWithTimeout`、`notAttempted` 或 `disabled`。</span><span class="sxs-lookup"><span data-stu-id="c81ec-181">Possible values are: `unknown`, `success`, `inProgress`, `failure`, `successWithTimeout`, `notAttempted`, `disabled`.</span></span>|
|<span data-ttu-id="c81ec-182">accountSetupStatus</span><span class="sxs-lookup"><span data-stu-id="c81ec-182">accountSetupStatus</span></span>|[<span data-ttu-id="c81ec-183">windowsAutopilotDeploymentState</span><span class="sxs-lookup"><span data-stu-id="c81ec-183">windowsAutopilotDeploymentState</span></span>](../resources/intune-troubleshooting-windowsautopilotdeploymentstate.md)|<span data-ttu-id="c81ec-184">注册状态页帐户设置阶段的部署状态。</span><span class="sxs-lookup"><span data-stu-id="c81ec-184">Deployment status for the enrollment status page account setup phase.</span></span> <span data-ttu-id="c81ec-185">可取值为：`unknown`、`success`、`inProgress`、`failure`、`successWithTimeout`、`notAttempted` 或 `disabled`。</span><span class="sxs-lookup"><span data-stu-id="c81ec-185">Possible values are: `unknown`, `success`, `inProgress`, `failure`, `successWithTimeout`, `notAttempted`, `disabled`.</span></span>|
|<span data-ttu-id="c81ec-186">osVersion</span><span class="sxs-lookup"><span data-stu-id="c81ec-186">osVersion</span></span>|<span data-ttu-id="c81ec-187">String</span><span class="sxs-lookup"><span data-stu-id="c81ec-187">String</span></span>|<span data-ttu-id="c81ec-188">设备操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="c81ec-188">Device operating system version.</span></span>|
|<span data-ttu-id="c81ec-189">deploymentDuration</span><span class="sxs-lookup"><span data-stu-id="c81ec-189">deploymentDuration</span></span>|<span data-ttu-id="c81ec-190">持续时间</span><span class="sxs-lookup"><span data-stu-id="c81ec-190">Duration</span></span>|<span data-ttu-id="c81ec-191">Autopilot 部署持续时间（包括注册）。</span><span class="sxs-lookup"><span data-stu-id="c81ec-191">Autopilot deployment duration including enrollment.</span></span>|
|<span data-ttu-id="c81ec-192">deploymentTotalDuration</span><span class="sxs-lookup"><span data-stu-id="c81ec-192">deploymentTotalDuration</span></span>|<span data-ttu-id="c81ec-193">持续时间</span><span class="sxs-lookup"><span data-stu-id="c81ec-193">Duration</span></span>|<span data-ttu-id="c81ec-194">从注册到桌面屏幕的总部署持续时间。</span><span class="sxs-lookup"><span data-stu-id="c81ec-194">Total deployment duration from enrollment to Desktop screen.</span></span>|
|<span data-ttu-id="c81ec-195">devicePreparationDuration</span><span class="sxs-lookup"><span data-stu-id="c81ec-195">devicePreparationDuration</span></span>|<span data-ttu-id="c81ec-196">持续时间</span><span class="sxs-lookup"><span data-stu-id="c81ec-196">Duration</span></span>|<span data-ttu-id="c81ec-197">设备注册所花费的时间。</span><span class="sxs-lookup"><span data-stu-id="c81ec-197">Time spent in device enrollment.</span></span>|
|<span data-ttu-id="c81ec-198">deviceSetupDuration</span><span class="sxs-lookup"><span data-stu-id="c81ec-198">deviceSetupDuration</span></span>|<span data-ttu-id="c81ec-199">持续时间</span><span class="sxs-lookup"><span data-stu-id="c81ec-199">Duration</span></span>|<span data-ttu-id="c81ec-200">在设备 ESP 中花费的时间。</span><span class="sxs-lookup"><span data-stu-id="c81ec-200">Time spent in device ESP.</span></span>|
|<span data-ttu-id="c81ec-201">accountSetupDuration</span><span class="sxs-lookup"><span data-stu-id="c81ec-201">accountSetupDuration</span></span>|<span data-ttu-id="c81ec-202">持续时间</span><span class="sxs-lookup"><span data-stu-id="c81ec-202">Duration</span></span>|<span data-ttu-id="c81ec-203">在用户 ESP 中花费的时间。</span><span class="sxs-lookup"><span data-stu-id="c81ec-203">Time spent in user ESP.</span></span>|
|<span data-ttu-id="c81ec-204">deploymentStartDateTime</span><span class="sxs-lookup"><span data-stu-id="c81ec-204">deploymentStartDateTime</span></span>|<span data-ttu-id="c81ec-205">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c81ec-205">DateTimeOffset</span></span>|<span data-ttu-id="c81ec-206">部署开始时间。</span><span class="sxs-lookup"><span data-stu-id="c81ec-206">Deployment start time.</span></span>|
|<span data-ttu-id="c81ec-207">deploymentEndDateTime</span><span class="sxs-lookup"><span data-stu-id="c81ec-207">deploymentEndDateTime</span></span>|<span data-ttu-id="c81ec-208">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c81ec-208">DateTimeOffset</span></span>|<span data-ttu-id="c81ec-209">部署结束时间。</span><span class="sxs-lookup"><span data-stu-id="c81ec-209">Deployment end time.</span></span>|
|<span data-ttu-id="c81ec-210">targetedAppCount</span><span class="sxs-lookup"><span data-stu-id="c81ec-210">targetedAppCount</span></span>|<span data-ttu-id="c81ec-211">Int32</span><span class="sxs-lookup"><span data-stu-id="c81ec-211">Int32</span></span>|<span data-ttu-id="c81ec-212">目标应用程序计数。</span><span class="sxs-lookup"><span data-stu-id="c81ec-212">Count of applications targeted.</span></span>|
|<span data-ttu-id="c81ec-213">targetedPolicyCount</span><span class="sxs-lookup"><span data-stu-id="c81ec-213">targetedPolicyCount</span></span>|<span data-ttu-id="c81ec-214">Int32</span><span class="sxs-lookup"><span data-stu-id="c81ec-214">Int32</span></span>|<span data-ttu-id="c81ec-215">目标策略计数。</span><span class="sxs-lookup"><span data-stu-id="c81ec-215">Count of policies targeted.</span></span>|
|<span data-ttu-id="c81ec-216">enrollmentFailureDetails</span><span class="sxs-lookup"><span data-stu-id="c81ec-216">enrollmentFailureDetails</span></span>|<span data-ttu-id="c81ec-217">String</span><span class="sxs-lookup"><span data-stu-id="c81ec-217">String</span></span>|<span data-ttu-id="c81ec-218">注册失败详细信息。</span><span class="sxs-lookup"><span data-stu-id="c81ec-218">Enrollment failure details.</span></span>|



## <a name="response"></a><span data-ttu-id="c81ec-219">响应</span><span class="sxs-lookup"><span data-stu-id="c81ec-219">Response</span></span>
<span data-ttu-id="c81ec-220">如果成功，此方法在响应正文中返回响应代码和 `201 Created` [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c81ec-220">If successful, this method returns a `201 Created` response code and a [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c81ec-221">示例</span><span class="sxs-lookup"><span data-stu-id="c81ec-221">Example</span></span>

### <a name="request"></a><span data-ttu-id="c81ec-222">请求</span><span class="sxs-lookup"><span data-stu-id="c81ec-222">Request</span></span>
<span data-ttu-id="c81ec-223">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c81ec-223">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/autopilotEvents
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

### <a name="response"></a><span data-ttu-id="c81ec-224">响应</span><span class="sxs-lookup"><span data-stu-id="c81ec-224">Response</span></span>
<span data-ttu-id="c81ec-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c81ec-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




