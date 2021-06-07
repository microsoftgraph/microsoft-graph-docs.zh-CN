---
title: 创建 managedDevice
description: 创建新的 managedDevice 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4bdd3bc460148298b91386e6ce0988f743cc78e5
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756153"
---
# <a name="create-manageddevice"></a><span data-ttu-id="952ea-103">创建 managedDevice</span><span class="sxs-lookup"><span data-stu-id="952ea-103">Create managedDevice</span></span>

<span data-ttu-id="952ea-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="952ea-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="952ea-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="952ea-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="952ea-106">创建新的 [managedDevice](../resources/intune-devices-manageddevice.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="952ea-106">Create a new [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="952ea-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="952ea-107">Prerequisites</span></span>
<span data-ttu-id="952ea-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="952ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="952ea-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="952ea-110">Permission type</span></span>|<span data-ttu-id="952ea-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="952ea-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="952ea-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="952ea-112">Delegated (work or school account)</span></span>|<span data-ttu-id="952ea-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="952ea-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="952ea-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="952ea-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="952ea-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="952ea-115">Not supported.</span></span>|
|<span data-ttu-id="952ea-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="952ea-116">Application</span></span>|<span data-ttu-id="952ea-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="952ea-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="952ea-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="952ea-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices
POST /deviceManagement/managedDevices
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices
```

## <a name="request-headers"></a><span data-ttu-id="952ea-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="952ea-119">Request headers</span></span>
|<span data-ttu-id="952ea-120">标头</span><span class="sxs-lookup"><span data-stu-id="952ea-120">Header</span></span>|<span data-ttu-id="952ea-121">值</span><span class="sxs-lookup"><span data-stu-id="952ea-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="952ea-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="952ea-122">Authorization</span></span>|<span data-ttu-id="952ea-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="952ea-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="952ea-124">接受</span><span class="sxs-lookup"><span data-stu-id="952ea-124">Accept</span></span>|<span data-ttu-id="952ea-125">application/json</span><span class="sxs-lookup"><span data-stu-id="952ea-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="952ea-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="952ea-126">Request body</span></span>
<span data-ttu-id="952ea-127">在请求正文中，提供 managedDevice 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="952ea-127">In the request body, supply a JSON representation for the managedDevice object.</span></span>

<span data-ttu-id="952ea-128">下表显示创建 managedDevice 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="952ea-128">The following table shows the properties that are required when you create the managedDevice.</span></span>

|<span data-ttu-id="952ea-129">属性</span><span class="sxs-lookup"><span data-stu-id="952ea-129">Property</span></span>|<span data-ttu-id="952ea-130">类型</span><span class="sxs-lookup"><span data-stu-id="952ea-130">Type</span></span>|<span data-ttu-id="952ea-131">说明</span><span class="sxs-lookup"><span data-stu-id="952ea-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="952ea-132">id</span><span class="sxs-lookup"><span data-stu-id="952ea-132">id</span></span>|<span data-ttu-id="952ea-133">String</span><span class="sxs-lookup"><span data-stu-id="952ea-133">String</span></span>|<span data-ttu-id="952ea-134">设备的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="952ea-134">Unique Identifier for the device.</span></span> <span data-ttu-id="952ea-135">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="952ea-135">This property is read-only.</span></span>|
|<span data-ttu-id="952ea-136">userId</span><span class="sxs-lookup"><span data-stu-id="952ea-136">userId</span></span>|<span data-ttu-id="952ea-137">String</span><span class="sxs-lookup"><span data-stu-id="952ea-137">String</span></span>|<span data-ttu-id="952ea-138">与设备关联的用户的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="952ea-138">Unique Identifier for the user associated with the device.</span></span> <span data-ttu-id="952ea-139">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="952ea-139">This property is read-only.</span></span>|
|<span data-ttu-id="952ea-140">deviceName</span><span class="sxs-lookup"><span data-stu-id="952ea-140">deviceName</span></span>|<span data-ttu-id="952ea-141">String</span><span class="sxs-lookup"><span data-stu-id="952ea-141">String</span></span>|<span data-ttu-id="952ea-142">设备的名称。</span><span class="sxs-lookup"><span data-stu-id="952ea-142">Name of the device.</span></span> <span data-ttu-id="952ea-143">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="952ea-143">This property is read-only.</span></span>|
|<span data-ttu-id="952ea-144">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="952ea-144">managedDeviceOwnerType</span></span>|[<span data-ttu-id="952ea-145">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="952ea-145">managedDeviceOwnerType</span></span>](../resources/intune-devices-manageddeviceownertype.md)|<span data-ttu-id="952ea-146">设备的所有权。</span><span class="sxs-lookup"><span data-stu-id="952ea-146">Ownership of the device.</span></span> <span data-ttu-id="952ea-147">可以是"公司"或"个人"。</span><span class="sxs-lookup"><span data-stu-id="952ea-147">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="952ea-148">可取值为：`unknown`、`company`、`personal`。</span><span class="sxs-lookup"><span data-stu-id="952ea-148">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="952ea-149">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="952ea-149">deviceActionResults</span></span>|<span data-ttu-id="952ea-150">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) 集合</span><span class="sxs-lookup"><span data-stu-id="952ea-150">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="952ea-151">ComplexType deviceActionResult 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="952ea-151">List of ComplexType deviceActionResult objects.</span></span> <span data-ttu-id="952ea-152">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="952ea-152">This property is read-only.</span></span>|
|<span data-ttu-id="952ea-153">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="952ea-153">enrolledDateTime</span></span>|<span data-ttu-id="952ea-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="952ea-154">DateTimeOffset</span></span>|<span data-ttu-id="952ea-155">设备的注册时间。</span><span class="sxs-lookup"><span data-stu-id="952ea-155">Enrollment time of the device.</span></span> <span data-ttu-id="952ea-156">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="952ea-156">This property is read-only.</span></span>|
|<span data-ttu-id="952ea-157">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="952ea-157">lastSyncDateTime</span></span>|<span data-ttu-id="952ea-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="952ea-158">DateTimeOffset</span></span>|<span data-ttu-id="952ea-159">设备上次成功完成与 Intune 同步的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="952ea-159">The date and time that the device last completed a successful sync with Intune.</span></span> <span data-ttu-id="952ea-160">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="952ea-160">This property is read-only.</span></span>|
|<span data-ttu-id="952ea-161">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="952ea-161">operatingSystem</span></span>|<span data-ttu-id="952ea-162">String</span><span class="sxs-lookup"><span data-stu-id="952ea-162">String</span></span>|<span data-ttu-id="952ea-163">设备的操作系统。</span><span class="sxs-lookup"><span data-stu-id="952ea-163">Operating system of the device.</span></span> <span data-ttu-id="952ea-164">Windows、iOS 等。此属性为只读。</span><span class="sxs-lookup"><span data-stu-id="952ea-164">Windows, iOS, etc. This property is read-only.</span></span>|
|<span data-ttu-id="952ea-165">complianceState</span><span class="sxs-lookup"><span data-stu-id="952ea-165">complianceState</span></span>|[<span data-ttu-id="952ea-166">complianceState</span><span class="sxs-lookup"><span data-stu-id="952ea-166">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="952ea-167">设备的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="952ea-167">Compliance state of the device.</span></span> <span data-ttu-id="952ea-168">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="952ea-168">This property is read-only.</span></span> <span data-ttu-id="952ea-169">可取值为：`unknown`、`compliant`、`noncompliant`、`conflict`、`error`、`inGracePeriod`、`configManager`。</span><span class="sxs-lookup"><span data-stu-id="952ea-169">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="952ea-170">jailBroken</span><span class="sxs-lookup"><span data-stu-id="952ea-170">jailBroken</span></span>|<span data-ttu-id="952ea-171">String</span><span class="sxs-lookup"><span data-stu-id="952ea-171">String</span></span>|<span data-ttu-id="952ea-172">设备是否已越狱或取得 root 权限。</span><span class="sxs-lookup"><span data-stu-id="952ea-172">whether the device is jail broken or rooted.</span></span> <span data-ttu-id="952ea-173">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="952ea-173">This property is read-only.</span></span>|
|<span data-ttu-id="952ea-174">managementAgent</span><span class="sxs-lookup"><span data-stu-id="952ea-174">managementAgent</span></span>|[<span data-ttu-id="952ea-175">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="952ea-175">managementAgentType</span></span>](../resources/intune-devices-managementagenttype.md)|<span data-ttu-id="952ea-176">设备的管理通道。</span><span class="sxs-lookup"><span data-stu-id="952ea-176">Management channel of the device.</span></span> <span data-ttu-id="952ea-177">Intune、EAS 等此属性为只读。</span><span class="sxs-lookup"><span data-stu-id="952ea-177">Intune, EAS, etc. This property is read-only.</span></span> <span data-ttu-id="952ea-178">可取值为：`eas`、`mdm`、`easMdm`、`intuneClient`、`easIntuneClient`、`configurationManagerClient`、`configurationManagerClientMdm`、`configurationManagerClientMdmEas`、`unknown`、`jamf`、`googleCloudDevicePolicyController`。</span><span class="sxs-lookup"><span data-stu-id="952ea-178">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`.</span></span>|
|<span data-ttu-id="952ea-179">osVersion</span><span class="sxs-lookup"><span data-stu-id="952ea-179">osVersion</span></span>|<span data-ttu-id="952ea-180">String</span><span class="sxs-lookup"><span data-stu-id="952ea-180">String</span></span>|<span data-ttu-id="952ea-181">设备的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="952ea-181">Operating system version of the device.</span></span> <span data-ttu-id="952ea-182">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="952ea-182">This property is read-only.</span></span>|
|<span data-ttu-id="952ea-183">easActivated</span><span class="sxs-lookup"><span data-stu-id="952ea-183">easActivated</span></span>|<span data-ttu-id="952ea-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="952ea-184">Boolean</span></span>|<span data-ttu-id="952ea-185">设备是否已激活 Exchange ActiveSync。</span><span class="sxs-lookup"><span data-stu-id="952ea-185">Whether the device is Exchange ActiveSync activated.</span></span> <span data-ttu-id="952ea-186">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="952ea-186">This property is read-only.</span></span>|
|<span data-ttu-id="952ea-187">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="952ea-187">easDeviceId</span></span>|<span data-ttu-id="952ea-188">String</span><span class="sxs-lookup"><span data-stu-id="952ea-188">String</span></span>|<span data-ttu-id="952ea-189">设备的 Exchange ActiveSync ID。</span><span class="sxs-lookup"><span data-stu-id="952ea-189">Exchange ActiveSync Id of the device.</span></span> <span data-ttu-id="952ea-190">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="952ea-190">This property is read-only.</span></span>|
|<span data-ttu-id="952ea-191">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="952ea-191">easActivationDateTime</span></span>|<span data-ttu-id="952ea-192">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="952ea-192">DateTimeOffset</span></span>|<span data-ttu-id="952ea-193">设备的 Exchange ActivationSync 激活时间。</span><span class="sxs-lookup"><span data-stu-id="952ea-193">Exchange ActivationSync activation time of the device.</span></span> <span data-ttu-id="952ea-194">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="952ea-194">This property is read-only.</span></span>|
|<span data-ttu-id="952ea-195">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="952ea-195">azureADRegistered</span></span>|<span data-ttu-id="952ea-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="952ea-196">Boolean</span></span>|<span data-ttu-id="952ea-197">设备是否已注册 Azure Active Directory。</span><span class="sxs-lookup"><span data-stu-id="952ea-197">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="952ea-198">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="952ea-198">This property is read-only.</span></span>|
|<span data-ttu-id="952ea-199">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="952ea-199">deviceEnrollmentType</span></span>|[<span data-ttu-id="952ea-200">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="952ea-200">deviceEnrollmentType</span></span>](../resources/intune-devices-deviceenrollmenttype.md)|<span data-ttu-id="952ea-201">设备的注册类型。</span><span class="sxs-lookup"><span data-stu-id="952ea-201">Enrollment type of the device.</span></span> <span data-ttu-id="952ea-202">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="952ea-202">This property is read-only.</span></span> <span data-ttu-id="952ea-203">可能的值是：`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement`、`windowsAzureADJoinUsingDeviceAuth`、`appleUserEnrollment`、`appleUserEnrollmentWithServiceAccount`。</span><span class="sxs-lookup"><span data-stu-id="952ea-203">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `windowsAzureADJoinUsingDeviceAuth`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`.</span></span>|
|<span data-ttu-id="952ea-204">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="952ea-204">activationLockBypassCode</span></span>|<span data-ttu-id="952ea-205">String</span><span class="sxs-lookup"><span data-stu-id="952ea-205">String</span></span>|<span data-ttu-id="952ea-206">允许绕过设备上的激活锁的代码。</span><span class="sxs-lookup"><span data-stu-id="952ea-206">Code that allows the Activation Lock on a device to be bypassed.</span></span> <span data-ttu-id="952ea-207">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="952ea-207">This property is read-only.</span></span>|
|<span data-ttu-id="952ea-208">emailAddress</span><span class="sxs-lookup"><span data-stu-id="952ea-208">emailAddress</span></span>|<span data-ttu-id="952ea-209">String</span><span class="sxs-lookup"><span data-stu-id="952ea-209">String</span></span>|<span data-ttu-id="952ea-210">电子邮件 () 设备关联的用户的邮箱。</span><span class="sxs-lookup"><span data-stu-id="952ea-210">Email(s) for the user associated with the device.</span></span> <span data-ttu-id="952ea-211">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="952ea-211">This property is read-only.</span></span>|
|<span data-ttu-id="952ea-212">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="952ea-212">azureADDeviceId</span></span>|<span data-ttu-id="952ea-213">String</span><span class="sxs-lookup"><span data-stu-id="952ea-213">String</span></span>|<span data-ttu-id="952ea-214">Azure Active Directory 设备的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="952ea-214">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="952ea-215">只读。</span><span class="sxs-lookup"><span data-stu-id="952ea-215">Read only.</span></span> <span data-ttu-id="952ea-216">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="952ea-216">This property is read-only.</span></span>|
|<span data-ttu-id="952ea-217">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="952ea-217">deviceRegistrationState</span></span>|[<span data-ttu-id="952ea-218">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="952ea-218">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="952ea-219">设备注册状态。</span><span class="sxs-lookup"><span data-stu-id="952ea-219">Device registration state.</span></span> <span data-ttu-id="952ea-220">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="952ea-220">This property is read-only.</span></span> <span data-ttu-id="952ea-221">可取值为：`notRegistered`、`registered`、`revoked`、`keyConflict`、`approvalPending`、`certificateReset`、`notRegisteredPendingEnrollment`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="952ea-221">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="952ea-222">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="952ea-222">deviceCategoryDisplayName</span></span>|<span data-ttu-id="952ea-223">String</span><span class="sxs-lookup"><span data-stu-id="952ea-223">String</span></span>|<span data-ttu-id="952ea-224">设备类别显示名称。</span><span class="sxs-lookup"><span data-stu-id="952ea-224">Device category display name.</span></span> <span data-ttu-id="952ea-225">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="952ea-225">This property is read-only.</span></span>|
|<span data-ttu-id="952ea-226">isSupervised</span><span class="sxs-lookup"><span data-stu-id="952ea-226">isSupervised</span></span>|<span data-ttu-id="952ea-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="952ea-227">Boolean</span></span>|<span data-ttu-id="952ea-228">设备监督状态。</span><span class="sxs-lookup"><span data-stu-id="952ea-228">Device supervised status.</span></span> <span data-ttu-id="952ea-229">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="952ea-229">This property is read-only.</span></span>|
|<span data-ttu-id="952ea-230">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="952ea-230">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="952ea-231">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="952ea-231">DateTimeOffset</span></span>|<span data-ttu-id="952ea-232">设备上次与 Exchange 联系的时间。</span><span class="sxs-lookup"><span data-stu-id="952ea-232">Last time the device contacted Exchange.</span></span> <span data-ttu-id="952ea-233">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="952ea-233">This property is read-only.</span></span>|
|<span data-ttu-id="952ea-234">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="952ea-234">exchangeAccessState</span></span>|[<span data-ttu-id="952ea-235">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="952ea-235">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="952ea-236">Exchange 中设备的访问状态。</span><span class="sxs-lookup"><span data-stu-id="952ea-236">The Access State of the device in Exchange.</span></span> <span data-ttu-id="952ea-237">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="952ea-237">This property is read-only.</span></span> <span data-ttu-id="952ea-238">可取值为：`none`、`unknown`、`allowed`、`blocked`、`quarantined`。</span><span class="sxs-lookup"><span data-stu-id="952ea-238">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="952ea-239">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="952ea-239">exchangeAccessStateReason</span></span>|[<span data-ttu-id="952ea-240">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="952ea-240">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="952ea-241">Exchange 中设备访问状态的出现原因。</span><span class="sxs-lookup"><span data-stu-id="952ea-241">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="952ea-242">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="952ea-242">This property is read-only.</span></span> <span data-ttu-id="952ea-243">可取值为：`none`、`unknown`、`exchangeGlobalRule`、`exchangeIndividualRule`、`exchangeDeviceRule`、`exchangeUpgrade`、`exchangeMailboxPolicy`、`other`、`compliant`、`notCompliant`、`notEnrolled`、`unknownLocation`、`mfaRequired`、`azureADBlockDueToAccessPolicy`、`compromisedPassword`、`deviceNotKnownWithManagedApp`。</span><span class="sxs-lookup"><span data-stu-id="952ea-243">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="952ea-244">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="952ea-244">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="952ea-245">String</span><span class="sxs-lookup"><span data-stu-id="952ea-245">String</span></span>|<span data-ttu-id="952ea-246">允许与设备建立远程协助会话的 URL。</span><span class="sxs-lookup"><span data-stu-id="952ea-246">Url that allows a Remote Assistance session to be established with the device.</span></span> <span data-ttu-id="952ea-247">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="952ea-247">This property is read-only.</span></span>|
|<span data-ttu-id="952ea-248">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="952ea-248">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="952ea-249">String</span><span class="sxs-lookup"><span data-stu-id="952ea-249">String</span></span>|<span data-ttu-id="952ea-250">用于在创建远程协助会话对象时识别问题的错误字符串。</span><span class="sxs-lookup"><span data-stu-id="952ea-250">An error string that identifies issues when creating Remote Assistance session objects.</span></span> <span data-ttu-id="952ea-251">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="952ea-251">This property is read-only.</span></span>|
|<span data-ttu-id="952ea-252">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="952ea-252">isEncrypted</span></span>|<span data-ttu-id="952ea-253">Boolean</span><span class="sxs-lookup"><span data-stu-id="952ea-253">Boolean</span></span>|<span data-ttu-id="952ea-254">设备加密状态。</span><span class="sxs-lookup"><span data-stu-id="952ea-254">Device encryption status.</span></span> <span data-ttu-id="952ea-255">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="952ea-255">This property is read-only.</span></span>|
|<span data-ttu-id="952ea-256">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="952ea-256">userPrincipalName</span></span>|<span data-ttu-id="952ea-257">String</span><span class="sxs-lookup"><span data-stu-id="952ea-257">String</span></span>|<span data-ttu-id="952ea-258">设备用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="952ea-258">Device user principal name.</span></span> <span data-ttu-id="952ea-259">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="952ea-259">This property is read-only.</span></span>|
|<span data-ttu-id="952ea-260">model</span><span class="sxs-lookup"><span data-stu-id="952ea-260">model</span></span>|<span data-ttu-id="952ea-261">String</span><span class="sxs-lookup"><span data-stu-id="952ea-261">String</span></span>|<span data-ttu-id="952ea-262">设备型号。</span><span class="sxs-lookup"><span data-stu-id="952ea-262">Model of the device.</span></span> <span data-ttu-id="952ea-263">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="952ea-263">This property is read-only.</span></span>|
|<span data-ttu-id="952ea-264">manufacturer</span><span class="sxs-lookup"><span data-stu-id="952ea-264">manufacturer</span></span>|<span data-ttu-id="952ea-265">String</span><span class="sxs-lookup"><span data-stu-id="952ea-265">String</span></span>|<span data-ttu-id="952ea-266">设备的制造商。</span><span class="sxs-lookup"><span data-stu-id="952ea-266">Manufacturer of the device.</span></span> <span data-ttu-id="952ea-267">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="952ea-267">This property is read-only.</span></span>|
|<span data-ttu-id="952ea-268">imei</span><span class="sxs-lookup"><span data-stu-id="952ea-268">imei</span></span>|<span data-ttu-id="952ea-269">String</span><span class="sxs-lookup"><span data-stu-id="952ea-269">String</span></span>|<span data-ttu-id="952ea-270">IMEI。</span><span class="sxs-lookup"><span data-stu-id="952ea-270">IMEI.</span></span> <span data-ttu-id="952ea-271">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="952ea-271">This property is read-only.</span></span>|
|<span data-ttu-id="952ea-272">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="952ea-272">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="952ea-273">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="952ea-273">DateTimeOffset</span></span>|<span data-ttu-id="952ea-274">设备合规性宽限期到期的 DateTime。</span><span class="sxs-lookup"><span data-stu-id="952ea-274">The DateTime when device compliance grace period expires.</span></span> <span data-ttu-id="952ea-275">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="952ea-275">This property is read-only.</span></span>|
|<span data-ttu-id="952ea-276">serialNumber</span><span class="sxs-lookup"><span data-stu-id="952ea-276">serialNumber</span></span>|<span data-ttu-id="952ea-277">String</span><span class="sxs-lookup"><span data-stu-id="952ea-277">String</span></span>|<span data-ttu-id="952ea-278">SerialNumber。</span><span class="sxs-lookup"><span data-stu-id="952ea-278">SerialNumber.</span></span> <span data-ttu-id="952ea-279">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="952ea-279">This property is read-only.</span></span>|
|<span data-ttu-id="952ea-280">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="952ea-280">phoneNumber</span></span>|<span data-ttu-id="952ea-281">String</span><span class="sxs-lookup"><span data-stu-id="952ea-281">String</span></span>|<span data-ttu-id="952ea-282">电话设备的数量。</span><span class="sxs-lookup"><span data-stu-id="952ea-282">Phone number of the device.</span></span> <span data-ttu-id="952ea-283">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="952ea-283">This property is read-only.</span></span>|
|<span data-ttu-id="952ea-284">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="952ea-284">androidSecurityPatchLevel</span></span>|<span data-ttu-id="952ea-285">String</span><span class="sxs-lookup"><span data-stu-id="952ea-285">String</span></span>|<span data-ttu-id="952ea-286">Android 安全修补程序级别。</span><span class="sxs-lookup"><span data-stu-id="952ea-286">Android security patch level.</span></span> <span data-ttu-id="952ea-287">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="952ea-287">This property is read-only.</span></span>|
|<span data-ttu-id="952ea-288">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="952ea-288">userDisplayName</span></span>|<span data-ttu-id="952ea-289">String</span><span class="sxs-lookup"><span data-stu-id="952ea-289">String</span></span>|<span data-ttu-id="952ea-290">用户显示名称。</span><span class="sxs-lookup"><span data-stu-id="952ea-290">User display name.</span></span> <span data-ttu-id="952ea-291">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="952ea-291">This property is read-only.</span></span>|
|<span data-ttu-id="952ea-292">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="952ea-292">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="952ea-293">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="952ea-293">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="952ea-294">ConfigrMgr 客户端启用的功能。</span><span class="sxs-lookup"><span data-stu-id="952ea-294">ConfigrMgr client enabled features.</span></span> <span data-ttu-id="952ea-295">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="952ea-295">This property is read-only.</span></span>|
|<span data-ttu-id="952ea-296">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="952ea-296">wiFiMacAddress</span></span>|<span data-ttu-id="952ea-297">String</span><span class="sxs-lookup"><span data-stu-id="952ea-297">String</span></span>|<span data-ttu-id="952ea-298">Wi-Fi MAC。</span><span class="sxs-lookup"><span data-stu-id="952ea-298">Wi-Fi MAC.</span></span> <span data-ttu-id="952ea-299">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="952ea-299">This property is read-only.</span></span>|
|<span data-ttu-id="952ea-300">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="952ea-300">deviceHealthAttestationState</span></span>|[<span data-ttu-id="952ea-301">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="952ea-301">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="952ea-302">设备运行状况证明状态。</span><span class="sxs-lookup"><span data-stu-id="952ea-302">The device health attestation state.</span></span> <span data-ttu-id="952ea-303">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="952ea-303">This property is read-only.</span></span>|
|<span data-ttu-id="952ea-304">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="952ea-304">subscriberCarrier</span></span>|<span data-ttu-id="952ea-305">String</span><span class="sxs-lookup"><span data-stu-id="952ea-305">String</span></span>|<span data-ttu-id="952ea-306">订阅者运营商。</span><span class="sxs-lookup"><span data-stu-id="952ea-306">Subscriber Carrier.</span></span> <span data-ttu-id="952ea-307">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="952ea-307">This property is read-only.</span></span>|
|<span data-ttu-id="952ea-308">meid</span><span class="sxs-lookup"><span data-stu-id="952ea-308">meid</span></span>|<span data-ttu-id="952ea-309">String</span><span class="sxs-lookup"><span data-stu-id="952ea-309">String</span></span>|<span data-ttu-id="952ea-310">MEID。</span><span class="sxs-lookup"><span data-stu-id="952ea-310">MEID.</span></span> <span data-ttu-id="952ea-311">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="952ea-311">This property is read-only.</span></span>|
|<span data-ttu-id="952ea-312">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="952ea-312">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="952ea-313">Int64</span><span class="sxs-lookup"><span data-stu-id="952ea-313">Int64</span></span>|<span data-ttu-id="952ea-314">总存储字节数。</span><span class="sxs-lookup"><span data-stu-id="952ea-314">Total Storage in Bytes.</span></span> <span data-ttu-id="952ea-315">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="952ea-315">This property is read-only.</span></span>|
|<span data-ttu-id="952ea-316">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="952ea-316">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="952ea-317">Int64</span><span class="sxs-lookup"><span data-stu-id="952ea-317">Int64</span></span>|<span data-ttu-id="952ea-318">可用存储字节为单位。</span><span class="sxs-lookup"><span data-stu-id="952ea-318">Free Storage in Bytes.</span></span> <span data-ttu-id="952ea-319">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="952ea-319">This property is read-only.</span></span>|
|<span data-ttu-id="952ea-320">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="952ea-320">managedDeviceName</span></span>|<span data-ttu-id="952ea-321">String</span><span class="sxs-lookup"><span data-stu-id="952ea-321">String</span></span>|<span data-ttu-id="952ea-322">用于识别设备的自动生成的名称。</span><span class="sxs-lookup"><span data-stu-id="952ea-322">Automatically generated name to identify a device.</span></span> <span data-ttu-id="952ea-323">可以覆盖为用户友好名称。</span><span class="sxs-lookup"><span data-stu-id="952ea-323">Can be overwritten to a user friendly name.</span></span>|
|<span data-ttu-id="952ea-324">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="952ea-324">partnerReportedThreatState</span></span>|[<span data-ttu-id="952ea-325">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="952ea-325">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="952ea-326">指示帐户和设备正在使用移动威胁防护合作伙伴时设备的威胁状态。</span><span class="sxs-lookup"><span data-stu-id="952ea-326">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="952ea-327">只读。</span><span class="sxs-lookup"><span data-stu-id="952ea-327">Read Only.</span></span> <span data-ttu-id="952ea-328">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="952ea-328">This property is read-only.</span></span> <span data-ttu-id="952ea-329">可取值为：`unknown`、`activated`、`deactivated`、`secured`、`lowSeverity`、`mediumSeverity`、`highSeverity`、`unresponsive`、`compromised`、`misconfigured`。</span><span class="sxs-lookup"><span data-stu-id="952ea-329">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="952ea-330">iccid</span><span class="sxs-lookup"><span data-stu-id="952ea-330">iccid</span></span>|<span data-ttu-id="952ea-331">String</span><span class="sxs-lookup"><span data-stu-id="952ea-331">String</span></span>|<span data-ttu-id="952ea-332">集成的电路卡标识符，它是 SIM 卡的唯一标识号。</span><span class="sxs-lookup"><span data-stu-id="952ea-332">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span> <span data-ttu-id="952ea-333">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="952ea-333">This property is read-only.</span></span>|
|<span data-ttu-id="952ea-334">udid</span><span class="sxs-lookup"><span data-stu-id="952ea-334">udid</span></span>|<span data-ttu-id="952ea-335">String</span><span class="sxs-lookup"><span data-stu-id="952ea-335">String</span></span>|<span data-ttu-id="952ea-336">iOS 和 macOS 设备的唯一设备标识符。</span><span class="sxs-lookup"><span data-stu-id="952ea-336">Unique Device Identifier for iOS and macOS devices.</span></span> <span data-ttu-id="952ea-337">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="952ea-337">This property is read-only.</span></span>|
|<span data-ttu-id="952ea-338">notes</span><span class="sxs-lookup"><span data-stu-id="952ea-338">notes</span></span>|<span data-ttu-id="952ea-339">String</span><span class="sxs-lookup"><span data-stu-id="952ea-339">String</span></span>|<span data-ttu-id="952ea-340">IT 管理员在设备上创建的备注</span><span class="sxs-lookup"><span data-stu-id="952ea-340">Notes on the device created by IT Admin</span></span>|
|<span data-ttu-id="952ea-341">ethernetMacAddress</span><span class="sxs-lookup"><span data-stu-id="952ea-341">ethernetMacAddress</span></span>|<span data-ttu-id="952ea-342">String</span><span class="sxs-lookup"><span data-stu-id="952ea-342">String</span></span>|<span data-ttu-id="952ea-343">以太网 MAC。</span><span class="sxs-lookup"><span data-stu-id="952ea-343">Ethernet MAC.</span></span> <span data-ttu-id="952ea-344">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="952ea-344">This property is read-only.</span></span>|
|<span data-ttu-id="952ea-345">physicalMemoryInBytes</span><span class="sxs-lookup"><span data-stu-id="952ea-345">physicalMemoryInBytes</span></span>|<span data-ttu-id="952ea-346">Int64</span><span class="sxs-lookup"><span data-stu-id="952ea-346">Int64</span></span>|<span data-ttu-id="952ea-347">内存总量（以字节为单位）。</span><span class="sxs-lookup"><span data-stu-id="952ea-347">Total Memory in Bytes.</span></span> <span data-ttu-id="952ea-348">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="952ea-348">This property is read-only.</span></span>|



## <a name="response"></a><span data-ttu-id="952ea-349">响应</span><span class="sxs-lookup"><span data-stu-id="952ea-349">Response</span></span>
<span data-ttu-id="952ea-350">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [managedDevice](../resources/intune-devices-manageddevice.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="952ea-350">If successful, this method returns a `201 Created` response code and a [managedDevice](../resources/intune-devices-manageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="952ea-351">示例</span><span class="sxs-lookup"><span data-stu-id="952ea-351">Example</span></span>

### <a name="request"></a><span data-ttu-id="952ea-352">请求</span><span class="sxs-lookup"><span data-stu-id="952ea-352">Request</span></span>
<span data-ttu-id="952ea-353">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="952ea-353">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices
Content-type: application/json
Content-length: 4821

{
  "@odata.type": "#microsoft.graph.managedDevice",
  "userId": "User Id value",
  "deviceName": "Device Name value",
  "managedDeviceOwnerType": "company",
  "deviceActionResults": [
    {
      "@odata.type": "microsoft.graph.deviceActionResult",
      "actionName": "Action Name value",
      "actionState": "pending",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ],
  "enrolledDateTime": "2016-12-31T23:59:43.797191-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "operatingSystem": "Operating System value",
  "complianceState": "compliant",
  "jailBroken": "Jail Broken value",
  "managementAgent": "mdm",
  "osVersion": "Os Version value",
  "easActivated": true,
  "easDeviceId": "Eas Device Id value",
  "easActivationDateTime": "2016-12-31T23:59:43.4878784-08:00",
  "azureADRegistered": true,
  "deviceEnrollmentType": "userEnrollment",
  "activationLockBypassCode": "Activation Lock Bypass Code value",
  "emailAddress": "Email Address value",
  "azureADDeviceId": "Azure ADDevice Id value",
  "deviceRegistrationState": "registered",
  "deviceCategoryDisplayName": "Device Category Display Name value",
  "isSupervised": true,
  "exchangeLastSuccessfulSyncDateTime": "2017-01-01T00:00:45.8803083-08:00",
  "exchangeAccessState": "unknown",
  "exchangeAccessStateReason": "unknown",
  "remoteAssistanceSessionUrl": "https://example.com/remoteAssistanceSessionUrl/",
  "remoteAssistanceSessionErrorDetails": "Remote Assistance Session Error Details value",
  "isEncrypted": true,
  "userPrincipalName": "User Principal Name value",
  "model": "Model value",
  "manufacturer": "Manufacturer value",
  "imei": "Imei value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "serialNumber": "Serial Number value",
  "phoneNumber": "Phone Number value",
  "androidSecurityPatchLevel": "Android Security Patch Level value",
  "userDisplayName": "User Display Name value",
  "configurationManagerClientEnabledFeatures": {
    "@odata.type": "microsoft.graph.configurationManagerClientEnabledFeatures",
    "inventory": true,
    "modernApps": true,
    "resourceAccess": true,
    "deviceConfiguration": true,
    "compliancePolicy": true,
    "windowsUpdateForBusiness": true
  },
  "wiFiMacAddress": "Wi Fi Mac Address value",
  "deviceHealthAttestationState": {
    "@odata.type": "microsoft.graph.deviceHealthAttestationState",
    "lastUpdateDateTime": "Last Update Date Time value",
    "contentNamespaceUrl": "https://example.com/contentNamespaceUrl/",
    "deviceHealthAttestationStatus": "Device Health Attestation Status value",
    "contentVersion": "Content Version value",
    "issuedDateTime": "2016-12-31T23:58:22.1231038-08:00",
    "attestationIdentityKey": "Attestation Identity Key value",
    "resetCount": 10,
    "restartCount": 12,
    "dataExcutionPolicy": "Data Excution Policy value",
    "bitLockerStatus": "Bit Locker Status value",
    "bootManagerVersion": "Boot Manager Version value",
    "codeIntegrityCheckVersion": "Code Integrity Check Version value",
    "secureBoot": "Secure Boot value",
    "bootDebugging": "Boot Debugging value",
    "operatingSystemKernelDebugging": "Operating System Kernel Debugging value",
    "codeIntegrity": "Code Integrity value",
    "testSigning": "Test Signing value",
    "safeMode": "Safe Mode value",
    "windowsPE": "Windows PE value",
    "earlyLaunchAntiMalwareDriverProtection": "Early Launch Anti Malware Driver Protection value",
    "virtualSecureMode": "Virtual Secure Mode value",
    "pcrHashAlgorithm": "Pcr Hash Algorithm value",
    "bootAppSecurityVersion": "Boot App Security Version value",
    "bootManagerSecurityVersion": "Boot Manager Security Version value",
    "tpmVersion": "Tpm Version value",
    "pcr0": "Pcr0 value",
    "secureBootConfigurationPolicyFingerPrint": "Secure Boot Configuration Policy Finger Print value",
    "codeIntegrityPolicy": "Code Integrity Policy value",
    "bootRevisionListInfo": "Boot Revision List Info value",
    "operatingSystemRevListInfo": "Operating System Rev List Info value",
    "healthStatusMismatchInfo": "Health Status Mismatch Info value",
    "healthAttestationSupportedStatus": "Health Attestation Supported Status value"
  },
  "subscriberCarrier": "Subscriber Carrier value",
  "meid": "Meid value",
  "totalStorageSpaceInBytes": 8,
  "freeStorageSpaceInBytes": 7,
  "managedDeviceName": "Managed Device Name value",
  "partnerReportedThreatState": "activated",
  "iccid": "Iccid value",
  "udid": "Udid value",
  "notes": "Notes value",
  "ethernetMacAddress": "Ethernet Mac Address value",
  "physicalMemoryInBytes": 5
}
```

### <a name="response"></a><span data-ttu-id="952ea-354">响应</span><span class="sxs-lookup"><span data-stu-id="952ea-354">Response</span></span>
<span data-ttu-id="952ea-p153">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="952ea-p153">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 4870

{
  "@odata.type": "#microsoft.graph.managedDevice",
  "id": "705c034c-034c-705c-4c03-5c704c035c70",
  "userId": "User Id value",
  "deviceName": "Device Name value",
  "managedDeviceOwnerType": "company",
  "deviceActionResults": [
    {
      "@odata.type": "microsoft.graph.deviceActionResult",
      "actionName": "Action Name value",
      "actionState": "pending",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ],
  "enrolledDateTime": "2016-12-31T23:59:43.797191-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "operatingSystem": "Operating System value",
  "complianceState": "compliant",
  "jailBroken": "Jail Broken value",
  "managementAgent": "mdm",
  "osVersion": "Os Version value",
  "easActivated": true,
  "easDeviceId": "Eas Device Id value",
  "easActivationDateTime": "2016-12-31T23:59:43.4878784-08:00",
  "azureADRegistered": true,
  "deviceEnrollmentType": "userEnrollment",
  "activationLockBypassCode": "Activation Lock Bypass Code value",
  "emailAddress": "Email Address value",
  "azureADDeviceId": "Azure ADDevice Id value",
  "deviceRegistrationState": "registered",
  "deviceCategoryDisplayName": "Device Category Display Name value",
  "isSupervised": true,
  "exchangeLastSuccessfulSyncDateTime": "2017-01-01T00:00:45.8803083-08:00",
  "exchangeAccessState": "unknown",
  "exchangeAccessStateReason": "unknown",
  "remoteAssistanceSessionUrl": "https://example.com/remoteAssistanceSessionUrl/",
  "remoteAssistanceSessionErrorDetails": "Remote Assistance Session Error Details value",
  "isEncrypted": true,
  "userPrincipalName": "User Principal Name value",
  "model": "Model value",
  "manufacturer": "Manufacturer value",
  "imei": "Imei value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "serialNumber": "Serial Number value",
  "phoneNumber": "Phone Number value",
  "androidSecurityPatchLevel": "Android Security Patch Level value",
  "userDisplayName": "User Display Name value",
  "configurationManagerClientEnabledFeatures": {
    "@odata.type": "microsoft.graph.configurationManagerClientEnabledFeatures",
    "inventory": true,
    "modernApps": true,
    "resourceAccess": true,
    "deviceConfiguration": true,
    "compliancePolicy": true,
    "windowsUpdateForBusiness": true
  },
  "wiFiMacAddress": "Wi Fi Mac Address value",
  "deviceHealthAttestationState": {
    "@odata.type": "microsoft.graph.deviceHealthAttestationState",
    "lastUpdateDateTime": "Last Update Date Time value",
    "contentNamespaceUrl": "https://example.com/contentNamespaceUrl/",
    "deviceHealthAttestationStatus": "Device Health Attestation Status value",
    "contentVersion": "Content Version value",
    "issuedDateTime": "2016-12-31T23:58:22.1231038-08:00",
    "attestationIdentityKey": "Attestation Identity Key value",
    "resetCount": 10,
    "restartCount": 12,
    "dataExcutionPolicy": "Data Excution Policy value",
    "bitLockerStatus": "Bit Locker Status value",
    "bootManagerVersion": "Boot Manager Version value",
    "codeIntegrityCheckVersion": "Code Integrity Check Version value",
    "secureBoot": "Secure Boot value",
    "bootDebugging": "Boot Debugging value",
    "operatingSystemKernelDebugging": "Operating System Kernel Debugging value",
    "codeIntegrity": "Code Integrity value",
    "testSigning": "Test Signing value",
    "safeMode": "Safe Mode value",
    "windowsPE": "Windows PE value",
    "earlyLaunchAntiMalwareDriverProtection": "Early Launch Anti Malware Driver Protection value",
    "virtualSecureMode": "Virtual Secure Mode value",
    "pcrHashAlgorithm": "Pcr Hash Algorithm value",
    "bootAppSecurityVersion": "Boot App Security Version value",
    "bootManagerSecurityVersion": "Boot Manager Security Version value",
    "tpmVersion": "Tpm Version value",
    "pcr0": "Pcr0 value",
    "secureBootConfigurationPolicyFingerPrint": "Secure Boot Configuration Policy Finger Print value",
    "codeIntegrityPolicy": "Code Integrity Policy value",
    "bootRevisionListInfo": "Boot Revision List Info value",
    "operatingSystemRevListInfo": "Operating System Rev List Info value",
    "healthStatusMismatchInfo": "Health Status Mismatch Info value",
    "healthAttestationSupportedStatus": "Health Attestation Supported Status value"
  },
  "subscriberCarrier": "Subscriber Carrier value",
  "meid": "Meid value",
  "totalStorageSpaceInBytes": 8,
  "freeStorageSpaceInBytes": 7,
  "managedDeviceName": "Managed Device Name value",
  "partnerReportedThreatState": "activated",
  "iccid": "Iccid value",
  "udid": "Udid value",
  "notes": "Notes value",
  "ethernetMacAddress": "Ethernet Mac Address value",
  "physicalMemoryInBytes": 5
}
```




