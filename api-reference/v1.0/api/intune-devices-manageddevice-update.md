---
title: 更新 managedDevice
description: 更新 managedDevice 对象的属性。
ms.openlocfilehash: 4e4f0cc7213a20477227683431fdd8af6e06bb9e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27011393"
---
# <a name="update-manageddevice"></a><span data-ttu-id="eacd8-103">更新 managedDevice</span><span class="sxs-lookup"><span data-stu-id="eacd8-103">Update managedDevice</span></span>

> <span data-ttu-id="eacd8-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="eacd8-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="eacd8-105">更新 [managedDevice](../resources/intune-devices-manageddevice.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="eacd8-105">Update the properties of a [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="eacd8-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="eacd8-106">Prerequisites</span></span>
<span data-ttu-id="eacd8-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="eacd8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eacd8-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="eacd8-109">Permission type</span></span>|<span data-ttu-id="eacd8-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="eacd8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eacd8-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="eacd8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="eacd8-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eacd8-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="eacd8-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="eacd8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eacd8-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="eacd8-114">Not supported.</span></span>|
|<span data-ttu-id="eacd8-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="eacd8-115">Application</span></span>|<span data-ttu-id="eacd8-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="eacd8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eacd8-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="eacd8-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}/managedDevices/{managedDeviceId}
PATCH /deviceManagement/managedDevices/{managedDeviceId}
PATCH /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}
```

## <a name="request-headers"></a><span data-ttu-id="eacd8-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="eacd8-118">Request headers</span></span>
|<span data-ttu-id="eacd8-119">标头</span><span class="sxs-lookup"><span data-stu-id="eacd8-119">Header</span></span>|<span data-ttu-id="eacd8-120">值</span><span class="sxs-lookup"><span data-stu-id="eacd8-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eacd8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="eacd8-121">Authorization</span></span>|<span data-ttu-id="eacd8-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="eacd8-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eacd8-123">Accept</span><span class="sxs-lookup"><span data-stu-id="eacd8-123">Accept</span></span>|<span data-ttu-id="eacd8-124">application/json</span><span class="sxs-lookup"><span data-stu-id="eacd8-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eacd8-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="eacd8-125">Request body</span></span>
<span data-ttu-id="eacd8-126">在请求正文中，提供 [managedDevice](../resources/intune-devices-manageddevice.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="eacd8-126">In the request body, supply a JSON representation for the [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>

<span data-ttu-id="eacd8-127">下表显示创建 [managedDevice](../resources/intune-devices-manageddevice.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="eacd8-127">The following table shows the properties that are required when you create the [managedDevice](../resources/intune-devices-manageddevice.md).</span></span>

|<span data-ttu-id="eacd8-128">属性</span><span class="sxs-lookup"><span data-stu-id="eacd8-128">Property</span></span>|<span data-ttu-id="eacd8-129">类型</span><span class="sxs-lookup"><span data-stu-id="eacd8-129">Type</span></span>|<span data-ttu-id="eacd8-130">说明</span><span class="sxs-lookup"><span data-stu-id="eacd8-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eacd8-131">id</span><span class="sxs-lookup"><span data-stu-id="eacd8-131">id</span></span>|<span data-ttu-id="eacd8-132">String</span><span class="sxs-lookup"><span data-stu-id="eacd8-132">String</span></span>|<span data-ttu-id="eacd8-133">设备唯一标识符</span><span class="sxs-lookup"><span data-stu-id="eacd8-133">Unique Identifier for the device</span></span>|
|<span data-ttu-id="eacd8-134">userId</span><span class="sxs-lookup"><span data-stu-id="eacd8-134">userId</span></span>|<span data-ttu-id="eacd8-135">String</span><span class="sxs-lookup"><span data-stu-id="eacd8-135">String</span></span>|<span data-ttu-id="eacd8-136">与设备关联的用户的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="eacd8-136">Unique Identifier for the user associated with the device</span></span>|
|<span data-ttu-id="eacd8-137">deviceName</span><span class="sxs-lookup"><span data-stu-id="eacd8-137">deviceName</span></span>|<span data-ttu-id="eacd8-138">String</span><span class="sxs-lookup"><span data-stu-id="eacd8-138">String</span></span>|<span data-ttu-id="eacd8-139">设备的名称</span><span class="sxs-lookup"><span data-stu-id="eacd8-139">Name of the device</span></span>|
|<span data-ttu-id="eacd8-140">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="eacd8-140">managedDeviceOwnerType</span></span>|[<span data-ttu-id="eacd8-141">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="eacd8-141">managedDeviceOwnerType</span></span>](../resources/intune-devices-manageddeviceownertype.md)|<span data-ttu-id="eacd8-142">设备的所有权。</span><span class="sxs-lookup"><span data-stu-id="eacd8-142">Ownership of the device.</span></span> <span data-ttu-id="eacd8-143">可以是公司或个人。</span><span class="sxs-lookup"><span data-stu-id="eacd8-143">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="eacd8-144">可取值为：`unknown`、`company`、`personal`。</span><span class="sxs-lookup"><span data-stu-id="eacd8-144">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="eacd8-145">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="eacd8-145">deviceActionResults</span></span>|<span data-ttu-id="eacd8-146">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) 集合</span><span class="sxs-lookup"><span data-stu-id="eacd8-146">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="eacd8-147">ComplexType deviceActionResult 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="eacd8-147">List of ComplexType deviceActionResult objects.</span></span>|
|<span data-ttu-id="eacd8-148">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="eacd8-148">enrolledDateTime</span></span>|<span data-ttu-id="eacd8-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eacd8-149">DateTimeOffset</span></span>|<span data-ttu-id="eacd8-150">设备的注册时间。</span><span class="sxs-lookup"><span data-stu-id="eacd8-150">Enrollment time of the device.</span></span>|
|<span data-ttu-id="eacd8-151">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="eacd8-151">lastSyncDateTime</span></span>|<span data-ttu-id="eacd8-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eacd8-152">DateTimeOffset</span></span>|<span data-ttu-id="eacd8-153">设备上次成功完成与 Intune 同步的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="eacd8-153">The date and time that the device last completed a successful sync with Intune.</span></span>|
|<span data-ttu-id="eacd8-154">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="eacd8-154">operatingSystem</span></span>|<span data-ttu-id="eacd8-155">String</span><span class="sxs-lookup"><span data-stu-id="eacd8-155">String</span></span>|<span data-ttu-id="eacd8-156">设备的操作系统。</span><span class="sxs-lookup"><span data-stu-id="eacd8-156">Operating system of the device.</span></span> <span data-ttu-id="eacd8-157">Windows、iOS 等。</span><span class="sxs-lookup"><span data-stu-id="eacd8-157">Windows, iOS, etc.</span></span>|
|<span data-ttu-id="eacd8-158">complianceState</span><span class="sxs-lookup"><span data-stu-id="eacd8-158">complianceState</span></span>|[<span data-ttu-id="eacd8-159">complianceState</span><span class="sxs-lookup"><span data-stu-id="eacd8-159">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="eacd8-160">设备的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="eacd8-160">Compliance state of the device.</span></span> <span data-ttu-id="eacd8-161">可取值为：`unknown`、`compliant`、`noncompliant`、`conflict`、`error`、`inGracePeriod`、`configManager`。</span><span class="sxs-lookup"><span data-stu-id="eacd8-161">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="eacd8-162">jailBroken</span><span class="sxs-lookup"><span data-stu-id="eacd8-162">jailBroken</span></span>|<span data-ttu-id="eacd8-163">String</span><span class="sxs-lookup"><span data-stu-id="eacd8-163">String</span></span>|<span data-ttu-id="eacd8-164">设备是否已越狱或取得 root 权限。</span><span class="sxs-lookup"><span data-stu-id="eacd8-164">whether the device is jail broken or rooted.</span></span>|
|<span data-ttu-id="eacd8-165">managementAgent</span><span class="sxs-lookup"><span data-stu-id="eacd8-165">managementAgent</span></span>|[<span data-ttu-id="eacd8-166">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="eacd8-166">managementAgentType</span></span>](../resources/intune-devices-managementagenttype.md)|<span data-ttu-id="eacd8-167">设备的管理通道。</span><span class="sxs-lookup"><span data-stu-id="eacd8-167">Management channel of the device.</span></span> <span data-ttu-id="eacd8-168">Intune、EAS 等 可取值为：`eas`、`mdm`、`easMdm`、`intuneClient`、`easIntuneClient`、`configurationManagerClient`、`configurationManagerClientMdm`、`configurationManagerClientMdmEas`、`unknown`、`jamf`、`googleCloudDevicePolicyController`。</span><span class="sxs-lookup"><span data-stu-id="eacd8-168">Intune, EAS, etc. Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`.</span></span>|
|<span data-ttu-id="eacd8-169">osVersion</span><span class="sxs-lookup"><span data-stu-id="eacd8-169">osVersion</span></span>|<span data-ttu-id="eacd8-170">String</span><span class="sxs-lookup"><span data-stu-id="eacd8-170">String</span></span>|<span data-ttu-id="eacd8-171">设备的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="eacd8-171">Operating system version of the device.</span></span>|
|<span data-ttu-id="eacd8-172">easActivated</span><span class="sxs-lookup"><span data-stu-id="eacd8-172">easActivated</span></span>|<span data-ttu-id="eacd8-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="eacd8-173">Boolean</span></span>|<span data-ttu-id="eacd8-174">设备是否已激活 Exchange ActiveSync。</span><span class="sxs-lookup"><span data-stu-id="eacd8-174">Whether the device is Exchange ActiveSync activated.</span></span>|
|<span data-ttu-id="eacd8-175">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="eacd8-175">easDeviceId</span></span>|<span data-ttu-id="eacd8-176">String</span><span class="sxs-lookup"><span data-stu-id="eacd8-176">String</span></span>|<span data-ttu-id="eacd8-177">设备的 Exchange ActiveSync ID。</span><span class="sxs-lookup"><span data-stu-id="eacd8-177">Exchange ActiveSync Id of the device.</span></span>|
|<span data-ttu-id="eacd8-178">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="eacd8-178">easActivationDateTime</span></span>|<span data-ttu-id="eacd8-179">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eacd8-179">DateTimeOffset</span></span>|<span data-ttu-id="eacd8-180">设备的 Exchange ActivationSync 激活时间。</span><span class="sxs-lookup"><span data-stu-id="eacd8-180">Exchange ActivationSync activation time of the device.</span></span>|
|<span data-ttu-id="eacd8-181">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="eacd8-181">azureADRegistered</span></span>|<span data-ttu-id="eacd8-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="eacd8-182">Boolean</span></span>|<span data-ttu-id="eacd8-183">设备是否已注册 Azure Active Directory。</span><span class="sxs-lookup"><span data-stu-id="eacd8-183">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="eacd8-184">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="eacd8-184">deviceEnrollmentType</span></span>|[<span data-ttu-id="eacd8-185">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="eacd8-185">deviceEnrollmentType</span></span>](../resources/intune-devices-deviceenrollmenttype.md)|<span data-ttu-id="eacd8-186">设备的注册类型。</span><span class="sxs-lookup"><span data-stu-id="eacd8-186">Enrollment type of the device.</span></span> <span data-ttu-id="eacd8-187">可取值为：`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement`。</span><span class="sxs-lookup"><span data-stu-id="eacd8-187">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="eacd8-188">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="eacd8-188">activationLockBypassCode</span></span>|<span data-ttu-id="eacd8-189">String</span><span class="sxs-lookup"><span data-stu-id="eacd8-189">String</span></span>|<span data-ttu-id="eacd8-190">允许绕过设备上的激活锁的代码。</span><span class="sxs-lookup"><span data-stu-id="eacd8-190">Code that allows the Activation Lock on a device to be bypassed.</span></span>|
|<span data-ttu-id="eacd8-191">emailAddress</span><span class="sxs-lookup"><span data-stu-id="eacd8-191">emailAddress</span></span>|<span data-ttu-id="eacd8-192">String</span><span class="sxs-lookup"><span data-stu-id="eacd8-192">String</span></span>|<span data-ttu-id="eacd8-193">与设备关联的用户的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="eacd8-193">Email(s) for the user associated with the device</span></span>|
|<span data-ttu-id="eacd8-194">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="eacd8-194">azureADDeviceId</span></span>|<span data-ttu-id="eacd8-195">String</span><span class="sxs-lookup"><span data-stu-id="eacd8-195">String</span></span>|<span data-ttu-id="eacd8-196">Azure Active Directory 设备的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="eacd8-196">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="eacd8-197">只读。</span><span class="sxs-lookup"><span data-stu-id="eacd8-197">Read only.</span></span>|
|<span data-ttu-id="eacd8-198">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="eacd8-198">deviceRegistrationState</span></span>|[<span data-ttu-id="eacd8-199">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="eacd8-199">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="eacd8-200">设备注册状态。</span><span class="sxs-lookup"><span data-stu-id="eacd8-200">Device registration state.</span></span> <span data-ttu-id="eacd8-201">可取值为：`notRegistered`、`registered`、`revoked`、`keyConflict`、`approvalPending`、`certificateReset`、`notRegisteredPendingEnrollment`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="eacd8-201">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="eacd8-202">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="eacd8-202">deviceCategoryDisplayName</span></span>|<span data-ttu-id="eacd8-203">String</span><span class="sxs-lookup"><span data-stu-id="eacd8-203">String</span></span>|<span data-ttu-id="eacd8-204">设备类别显示名称。</span><span class="sxs-lookup"><span data-stu-id="eacd8-204">Device category display name</span></span>|
|<span data-ttu-id="eacd8-205">isSupervised</span><span class="sxs-lookup"><span data-stu-id="eacd8-205">isSupervised</span></span>|<span data-ttu-id="eacd8-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="eacd8-206">Boolean</span></span>|<span data-ttu-id="eacd8-207">设备受监督状态</span><span class="sxs-lookup"><span data-stu-id="eacd8-207">Device supervised status</span></span>|
|<span data-ttu-id="eacd8-208">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="eacd8-208">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="eacd8-209">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eacd8-209">DateTimeOffset</span></span>|<span data-ttu-id="eacd8-210">设备上次与 Exchange 联系的时间。</span><span class="sxs-lookup"><span data-stu-id="eacd8-210">Last time the device contacted Exchange.</span></span>|
|<span data-ttu-id="eacd8-211">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="eacd8-211">exchangeAccessState</span></span>|[<span data-ttu-id="eacd8-212">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="eacd8-212">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="eacd8-213">Exchange 中设备的访问状态。</span><span class="sxs-lookup"><span data-stu-id="eacd8-213">The Access State of the device in Exchange.</span></span> <span data-ttu-id="eacd8-214">可取值为：`none`、`unknown`、`allowed`、`blocked`、`quarantined`。</span><span class="sxs-lookup"><span data-stu-id="eacd8-214">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="eacd8-215">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="eacd8-215">exchangeAccessStateReason</span></span>|[<span data-ttu-id="eacd8-216">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="eacd8-216">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="eacd8-217">Exchange 中设备访问状态的出现原因。</span><span class="sxs-lookup"><span data-stu-id="eacd8-217">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="eacd8-218">可取值为：`none`、`unknown`、`exchangeGlobalRule`、`exchangeIndividualRule`、`exchangeDeviceRule`、`exchangeUpgrade`、`exchangeMailboxPolicy`、`other`、`compliant`、`notCompliant`、`notEnrolled`、`unknownLocation`、`mfaRequired`、`azureADBlockDueToAccessPolicy`、`compromisedPassword`、`deviceNotKnownWithManagedApp`。</span><span class="sxs-lookup"><span data-stu-id="eacd8-218">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="eacd8-219">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="eacd8-219">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="eacd8-220">String</span><span class="sxs-lookup"><span data-stu-id="eacd8-220">String</span></span>|<span data-ttu-id="eacd8-221">允许与设备建立远程协助会话的 URL。</span><span class="sxs-lookup"><span data-stu-id="eacd8-221">Url that allows a Remote Assistance session to be established with the device.</span></span>|
|<span data-ttu-id="eacd8-222">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="eacd8-222">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="eacd8-223">String</span><span class="sxs-lookup"><span data-stu-id="eacd8-223">String</span></span>|<span data-ttu-id="eacd8-224">用于在创建远程协助会话对象时识别问题的错误字符串。</span><span class="sxs-lookup"><span data-stu-id="eacd8-224">An error string that identifies issues when creating Remote Assistance session objects.</span></span>|
|<span data-ttu-id="eacd8-225">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="eacd8-225">isEncrypted</span></span>|<span data-ttu-id="eacd8-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="eacd8-226">Boolean</span></span>|<span data-ttu-id="eacd8-227">设备加密状态</span><span class="sxs-lookup"><span data-stu-id="eacd8-227">Device encryption status</span></span>|
|<span data-ttu-id="eacd8-228">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="eacd8-228">userPrincipalName</span></span>|<span data-ttu-id="eacd8-229">String</span><span class="sxs-lookup"><span data-stu-id="eacd8-229">String</span></span>|<span data-ttu-id="eacd8-230">设备用户主体名称</span><span class="sxs-lookup"><span data-stu-id="eacd8-230">Device user principal name</span></span>|
|<span data-ttu-id="eacd8-231">model</span><span class="sxs-lookup"><span data-stu-id="eacd8-231">model</span></span>|<span data-ttu-id="eacd8-232">String</span><span class="sxs-lookup"><span data-stu-id="eacd8-232">String</span></span>|<span data-ttu-id="eacd8-233">设备的型号</span><span class="sxs-lookup"><span data-stu-id="eacd8-233">Model of the device</span></span>|
|<span data-ttu-id="eacd8-234">manufacturer</span><span class="sxs-lookup"><span data-stu-id="eacd8-234">manufacturer</span></span>|<span data-ttu-id="eacd8-235">String</span><span class="sxs-lookup"><span data-stu-id="eacd8-235">String</span></span>|<span data-ttu-id="eacd8-236">设备的制造商</span><span class="sxs-lookup"><span data-stu-id="eacd8-236">Manufacturer of the device</span></span>|
|<span data-ttu-id="eacd8-237">imei</span><span class="sxs-lookup"><span data-stu-id="eacd8-237">imei</span></span>|<span data-ttu-id="eacd8-238">String</span><span class="sxs-lookup"><span data-stu-id="eacd8-238">String</span></span>|<span data-ttu-id="eacd8-239">IMEI</span><span class="sxs-lookup"><span data-stu-id="eacd8-239">IMEI</span></span>|
|<span data-ttu-id="eacd8-240">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="eacd8-240">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="eacd8-241">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eacd8-241">DateTimeOffset</span></span>|<span data-ttu-id="eacd8-242">设备符合性宽限期的到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="eacd8-242">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="eacd8-243">serialNumber</span><span class="sxs-lookup"><span data-stu-id="eacd8-243">serialNumber</span></span>|<span data-ttu-id="eacd8-244">String</span><span class="sxs-lookup"><span data-stu-id="eacd8-244">String</span></span>|<span data-ttu-id="eacd8-245">序列号</span><span class="sxs-lookup"><span data-stu-id="eacd8-245">SerialNumber</span></span>|
|<span data-ttu-id="eacd8-246">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="eacd8-246">phoneNumber</span></span>|<span data-ttu-id="eacd8-247">String</span><span class="sxs-lookup"><span data-stu-id="eacd8-247">String</span></span>|<span data-ttu-id="eacd8-248">设备的电话号码</span><span class="sxs-lookup"><span data-stu-id="eacd8-248">Phone number of the device</span></span>|
|<span data-ttu-id="eacd8-249">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="eacd8-249">androidSecurityPatchLevel</span></span>|<span data-ttu-id="eacd8-250">String</span><span class="sxs-lookup"><span data-stu-id="eacd8-250">String</span></span>|<span data-ttu-id="eacd8-251">Android 安全修补程序级别</span><span class="sxs-lookup"><span data-stu-id="eacd8-251">Android security patch level</span></span>|
|<span data-ttu-id="eacd8-252">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="eacd8-252">userDisplayName</span></span>|<span data-ttu-id="eacd8-253">String</span><span class="sxs-lookup"><span data-stu-id="eacd8-253">String</span></span>|<span data-ttu-id="eacd8-254">用户显示名称</span><span class="sxs-lookup"><span data-stu-id="eacd8-254">User display name</span></span>|
|<span data-ttu-id="eacd8-255">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="eacd8-255">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="eacd8-256">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="eacd8-256">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="eacd8-257">ConfigrMgr 客户端启用的功能</span><span class="sxs-lookup"><span data-stu-id="eacd8-257">ConfigrMgr client enabled features</span></span>|
|<span data-ttu-id="eacd8-258">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="eacd8-258">wiFiMacAddress</span></span>|<span data-ttu-id="eacd8-259">String</span><span class="sxs-lookup"><span data-stu-id="eacd8-259">String</span></span>|<span data-ttu-id="eacd8-260">Wi-Fi MAC</span><span class="sxs-lookup"><span data-stu-id="eacd8-260">Wi-Fi MAC</span></span>|
|<span data-ttu-id="eacd8-261">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="eacd8-261">deviceHealthAttestationState</span></span>|[<span data-ttu-id="eacd8-262">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="eacd8-262">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="eacd8-263">设备运行状况证明状态。</span><span class="sxs-lookup"><span data-stu-id="eacd8-263">The device health attestation state.</span></span>|
|<span data-ttu-id="eacd8-264">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="eacd8-264">subscriberCarrier</span></span>|<span data-ttu-id="eacd8-265">String</span><span class="sxs-lookup"><span data-stu-id="eacd8-265">String</span></span>|<span data-ttu-id="eacd8-266">订阅者运营商</span><span class="sxs-lookup"><span data-stu-id="eacd8-266">Subscriber Carrier</span></span>|
|<span data-ttu-id="eacd8-267">meid</span><span class="sxs-lookup"><span data-stu-id="eacd8-267">meid</span></span>|<span data-ttu-id="eacd8-268">String</span><span class="sxs-lookup"><span data-stu-id="eacd8-268">String</span></span>|<span data-ttu-id="eacd8-269">MEID</span><span class="sxs-lookup"><span data-stu-id="eacd8-269">MEID</span></span>|
|<span data-ttu-id="eacd8-270">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="eacd8-270">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="eacd8-271">Int64</span><span class="sxs-lookup"><span data-stu-id="eacd8-271">Int64</span></span>|<span data-ttu-id="eacd8-272">存储空间总字节数</span><span class="sxs-lookup"><span data-stu-id="eacd8-272">Total Storage in Bytes</span></span>|
|<span data-ttu-id="eacd8-273">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="eacd8-273">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="eacd8-274">Int64</span><span class="sxs-lookup"><span data-stu-id="eacd8-274">Int64</span></span>|<span data-ttu-id="eacd8-275">可用存储空间字节数</span><span class="sxs-lookup"><span data-stu-id="eacd8-275">Free Storage in Bytes</span></span>|
|<span data-ttu-id="eacd8-276">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="eacd8-276">managedDeviceName</span></span>|<span data-ttu-id="eacd8-277">String</span><span class="sxs-lookup"><span data-stu-id="eacd8-277">String</span></span>|<span data-ttu-id="eacd8-278">用于识别设备的自动生成的名称。</span><span class="sxs-lookup"><span data-stu-id="eacd8-278">Automatically generated name to identify a device.</span></span> <span data-ttu-id="eacd8-279">可以覆盖为用户友好名称。</span><span class="sxs-lookup"><span data-stu-id="eacd8-279">Can be overwritten to a user friendly name.</span></span>|
|<span data-ttu-id="eacd8-280">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="eacd8-280">partnerReportedThreatState</span></span>|[<span data-ttu-id="eacd8-281">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="eacd8-281">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="eacd8-282">指示帐户和设备正在使用移动威胁防护合作伙伴时设备的威胁状态。</span><span class="sxs-lookup"><span data-stu-id="eacd8-282">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="eacd8-283">只读。</span><span class="sxs-lookup"><span data-stu-id="eacd8-283">Read Only.</span></span> <span data-ttu-id="eacd8-284">可取值为：`unknown`、`activated`、`deactivated`、`secured`、`lowSeverity`、`mediumSeverity`、`highSeverity`、`unresponsive`、`compromised`、`misconfigured`。</span><span class="sxs-lookup"><span data-stu-id="eacd8-284">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|



## <a name="response"></a><span data-ttu-id="eacd8-285">响应</span><span class="sxs-lookup"><span data-stu-id="eacd8-285">Response</span></span>
<span data-ttu-id="eacd8-286">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [managedDevice](../resources/intune-devices-manageddevice.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="eacd8-286">If successful, this method returns a `200 OK` response code and an updated [managedDevice](../resources/intune-devices-manageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eacd8-287">示例</span><span class="sxs-lookup"><span data-stu-id="eacd8-287">Example</span></span>
### <a name="request"></a><span data-ttu-id="eacd8-288">请求</span><span class="sxs-lookup"><span data-stu-id="eacd8-288">Request</span></span>
<span data-ttu-id="eacd8-289">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="eacd8-289">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}
Content-type: application/json
Content-length: 4656

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
  "partnerReportedThreatState": "activated"
}
```

### <a name="response"></a><span data-ttu-id="eacd8-290">响应</span><span class="sxs-lookup"><span data-stu-id="eacd8-290">Response</span></span>
<span data-ttu-id="eacd8-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="eacd8-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4705

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
  "partnerReportedThreatState": "activated"
}
```



