---
title: 更新 managedDevice
description: 更新 managedDevice 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 07e25aa9390bfdd11801b499f516ba9e7e6dbd27
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42513474"
---
# <a name="update-manageddevice"></a><span data-ttu-id="0ebae-103">更新 managedDevice</span><span class="sxs-lookup"><span data-stu-id="0ebae-103">Update managedDevice</span></span>

<span data-ttu-id="0ebae-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0ebae-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0ebae-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0ebae-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0ebae-106">更新 [managedDevice](../resources/intune-devices-manageddevice.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0ebae-106">Update the properties of a [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0ebae-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="0ebae-107">Prerequisites</span></span>
<span data-ttu-id="0ebae-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0ebae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ebae-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="0ebae-110">Permission type</span></span>|<span data-ttu-id="0ebae-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0ebae-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0ebae-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0ebae-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0ebae-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ebae-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="0ebae-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0ebae-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0ebae-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0ebae-115">Not supported.</span></span>|
|<span data-ttu-id="0ebae-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="0ebae-116">Application</span></span>|<span data-ttu-id="0ebae-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="0ebae-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0ebae-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0ebae-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}/managedDevices/{managedDeviceId}
PATCH /deviceManagement/managedDevices/{managedDeviceId}
PATCH /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}
```

## <a name="request-headers"></a><span data-ttu-id="0ebae-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="0ebae-119">Request headers</span></span>
|<span data-ttu-id="0ebae-120">标头</span><span class="sxs-lookup"><span data-stu-id="0ebae-120">Header</span></span>|<span data-ttu-id="0ebae-121">值</span><span class="sxs-lookup"><span data-stu-id="0ebae-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0ebae-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ebae-122">Authorization</span></span>|<span data-ttu-id="0ebae-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0ebae-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0ebae-124">接受</span><span class="sxs-lookup"><span data-stu-id="0ebae-124">Accept</span></span>|<span data-ttu-id="0ebae-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0ebae-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ebae-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="0ebae-126">Request body</span></span>
<span data-ttu-id="0ebae-127">在请求正文中，提供 [managedDevice](../resources/intune-devices-manageddevice.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0ebae-127">In the request body, supply a JSON representation for the [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>

<span data-ttu-id="0ebae-128">下表显示创建 [managedDevice](../resources/intune-devices-manageddevice.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="0ebae-128">The following table shows the properties that are required when you create the [managedDevice](../resources/intune-devices-manageddevice.md).</span></span>

|<span data-ttu-id="0ebae-129">属性</span><span class="sxs-lookup"><span data-stu-id="0ebae-129">Property</span></span>|<span data-ttu-id="0ebae-130">类型</span><span class="sxs-lookup"><span data-stu-id="0ebae-130">Type</span></span>|<span data-ttu-id="0ebae-131">说明</span><span class="sxs-lookup"><span data-stu-id="0ebae-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ebae-132">id</span><span class="sxs-lookup"><span data-stu-id="0ebae-132">id</span></span>|<span data-ttu-id="0ebae-133">字符串</span><span class="sxs-lookup"><span data-stu-id="0ebae-133">String</span></span>|<span data-ttu-id="0ebae-134">设备唯一标识符</span><span class="sxs-lookup"><span data-stu-id="0ebae-134">Unique Identifier for the device</span></span>|
|<span data-ttu-id="0ebae-135">userId</span><span class="sxs-lookup"><span data-stu-id="0ebae-135">userId</span></span>|<span data-ttu-id="0ebae-136">String</span><span class="sxs-lookup"><span data-stu-id="0ebae-136">String</span></span>|<span data-ttu-id="0ebae-137">与设备关联的用户的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="0ebae-137">Unique Identifier for the user associated with the device</span></span>|
|<span data-ttu-id="0ebae-138">deviceName</span><span class="sxs-lookup"><span data-stu-id="0ebae-138">deviceName</span></span>|<span data-ttu-id="0ebae-139">字符串</span><span class="sxs-lookup"><span data-stu-id="0ebae-139">String</span></span>|<span data-ttu-id="0ebae-140">设备的名称</span><span class="sxs-lookup"><span data-stu-id="0ebae-140">Name of the device</span></span>|
|<span data-ttu-id="0ebae-141">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="0ebae-141">managedDeviceOwnerType</span></span>|[<span data-ttu-id="0ebae-142">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="0ebae-142">managedDeviceOwnerType</span></span>](../resources/intune-devices-manageddeviceownertype.md)|<span data-ttu-id="0ebae-143">设备的所有权。</span><span class="sxs-lookup"><span data-stu-id="0ebae-143">Ownership of the device.</span></span> <span data-ttu-id="0ebae-144">可以是 "公司" 或 "个人"。</span><span class="sxs-lookup"><span data-stu-id="0ebae-144">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="0ebae-145">可取值为：`unknown`、`company`、`personal`。</span><span class="sxs-lookup"><span data-stu-id="0ebae-145">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="0ebae-146">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="0ebae-146">deviceActionResults</span></span>|<span data-ttu-id="0ebae-147">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0ebae-147">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="0ebae-148">ComplexType deviceActionResult 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="0ebae-148">List of ComplexType deviceActionResult objects.</span></span>|
|<span data-ttu-id="0ebae-149">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="0ebae-149">enrolledDateTime</span></span>|<span data-ttu-id="0ebae-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ebae-150">DateTimeOffset</span></span>|<span data-ttu-id="0ebae-151">设备的注册时间。</span><span class="sxs-lookup"><span data-stu-id="0ebae-151">Enrollment time of the device.</span></span>|
|<span data-ttu-id="0ebae-152">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="0ebae-152">lastSyncDateTime</span></span>|<span data-ttu-id="0ebae-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ebae-153">DateTimeOffset</span></span>|<span data-ttu-id="0ebae-154">设备上次成功完成与 Intune 同步的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="0ebae-154">The date and time that the device last completed a successful sync with Intune.</span></span>|
|<span data-ttu-id="0ebae-155">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="0ebae-155">operatingSystem</span></span>|<span data-ttu-id="0ebae-156">字符串</span><span class="sxs-lookup"><span data-stu-id="0ebae-156">String</span></span>|<span data-ttu-id="0ebae-157">设备的操作系统。</span><span class="sxs-lookup"><span data-stu-id="0ebae-157">Operating system of the device.</span></span> <span data-ttu-id="0ebae-158">Windows、iOS 等。</span><span class="sxs-lookup"><span data-stu-id="0ebae-158">Windows, iOS, etc.</span></span>|
|<span data-ttu-id="0ebae-159">complianceState</span><span class="sxs-lookup"><span data-stu-id="0ebae-159">complianceState</span></span>|[<span data-ttu-id="0ebae-160">complianceState</span><span class="sxs-lookup"><span data-stu-id="0ebae-160">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="0ebae-161">设备的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="0ebae-161">Compliance state of the device.</span></span> <span data-ttu-id="0ebae-162">可取值为：`unknown`、`compliant`、`noncompliant`、`conflict`、`error`、`inGracePeriod`、`configManager`。</span><span class="sxs-lookup"><span data-stu-id="0ebae-162">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="0ebae-163">jailBroken</span><span class="sxs-lookup"><span data-stu-id="0ebae-163">jailBroken</span></span>|<span data-ttu-id="0ebae-164">字符串</span><span class="sxs-lookup"><span data-stu-id="0ebae-164">String</span></span>|<span data-ttu-id="0ebae-165">设备是否已越狱或取得 root 权限。</span><span class="sxs-lookup"><span data-stu-id="0ebae-165">whether the device is jail broken or rooted.</span></span>|
|<span data-ttu-id="0ebae-166">managementAgent</span><span class="sxs-lookup"><span data-stu-id="0ebae-166">managementAgent</span></span>|[<span data-ttu-id="0ebae-167">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="0ebae-167">managementAgentType</span></span>](../resources/intune-devices-managementagenttype.md)|<span data-ttu-id="0ebae-168">设备的管理通道。</span><span class="sxs-lookup"><span data-stu-id="0ebae-168">Management channel of the device.</span></span> <span data-ttu-id="0ebae-169">Intune、EAS 等 可取值为：`eas`、`mdm`、`easMdm`、`intuneClient`、`easIntuneClient`、`configurationManagerClient`、`configurationManagerClientMdm`、`configurationManagerClientMdmEas`、`unknown`、`jamf`、`googleCloudDevicePolicyController`。</span><span class="sxs-lookup"><span data-stu-id="0ebae-169">Intune, EAS, etc. Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`.</span></span>|
|<span data-ttu-id="0ebae-170">osVersion</span><span class="sxs-lookup"><span data-stu-id="0ebae-170">osVersion</span></span>|<span data-ttu-id="0ebae-171">字符串</span><span class="sxs-lookup"><span data-stu-id="0ebae-171">String</span></span>|<span data-ttu-id="0ebae-172">设备的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="0ebae-172">Operating system version of the device.</span></span>|
|<span data-ttu-id="0ebae-173">easActivated</span><span class="sxs-lookup"><span data-stu-id="0ebae-173">easActivated</span></span>|<span data-ttu-id="0ebae-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ebae-174">Boolean</span></span>|<span data-ttu-id="0ebae-175">设备是否已激活 Exchange ActiveSync。</span><span class="sxs-lookup"><span data-stu-id="0ebae-175">Whether the device is Exchange ActiveSync activated.</span></span>|
|<span data-ttu-id="0ebae-176">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="0ebae-176">easDeviceId</span></span>|<span data-ttu-id="0ebae-177">字符串</span><span class="sxs-lookup"><span data-stu-id="0ebae-177">String</span></span>|<span data-ttu-id="0ebae-178">设备的 Exchange ActiveSync ID。</span><span class="sxs-lookup"><span data-stu-id="0ebae-178">Exchange ActiveSync Id of the device.</span></span>|
|<span data-ttu-id="0ebae-179">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="0ebae-179">easActivationDateTime</span></span>|<span data-ttu-id="0ebae-180">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ebae-180">DateTimeOffset</span></span>|<span data-ttu-id="0ebae-181">设备的 Exchange ActivationSync 激活时间。</span><span class="sxs-lookup"><span data-stu-id="0ebae-181">Exchange ActivationSync activation time of the device.</span></span>|
|<span data-ttu-id="0ebae-182">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="0ebae-182">azureADRegistered</span></span>|<span data-ttu-id="0ebae-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ebae-183">Boolean</span></span>|<span data-ttu-id="0ebae-184">设备是否已注册 Azure Active Directory。</span><span class="sxs-lookup"><span data-stu-id="0ebae-184">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="0ebae-185">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="0ebae-185">deviceEnrollmentType</span></span>|[<span data-ttu-id="0ebae-186">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="0ebae-186">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="0ebae-187">设备的注册类型。</span><span class="sxs-lookup"><span data-stu-id="0ebae-187">Enrollment type of the device.</span></span> <span data-ttu-id="0ebae-188">可取值为：`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement`。</span><span class="sxs-lookup"><span data-stu-id="0ebae-188">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="0ebae-189">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="0ebae-189">activationLockBypassCode</span></span>|<span data-ttu-id="0ebae-190">字符串</span><span class="sxs-lookup"><span data-stu-id="0ebae-190">String</span></span>|<span data-ttu-id="0ebae-191">允许绕过设备上的激活锁的代码。</span><span class="sxs-lookup"><span data-stu-id="0ebae-191">Code that allows the Activation Lock on a device to be bypassed.</span></span>|
|<span data-ttu-id="0ebae-192">emailAddress</span><span class="sxs-lookup"><span data-stu-id="0ebae-192">emailAddress</span></span>|<span data-ttu-id="0ebae-193">字符串</span><span class="sxs-lookup"><span data-stu-id="0ebae-193">String</span></span>|<span data-ttu-id="0ebae-194">与设备关联的用户的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="0ebae-194">Email(s) for the user associated with the device</span></span>|
|<span data-ttu-id="0ebae-195">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="0ebae-195">azureADDeviceId</span></span>|<span data-ttu-id="0ebae-196">字符串</span><span class="sxs-lookup"><span data-stu-id="0ebae-196">String</span></span>|<span data-ttu-id="0ebae-197">Azure Active Directory 设备的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="0ebae-197">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="0ebae-198">只读。</span><span class="sxs-lookup"><span data-stu-id="0ebae-198">Read only.</span></span>|
|<span data-ttu-id="0ebae-199">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="0ebae-199">deviceRegistrationState</span></span>|[<span data-ttu-id="0ebae-200">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="0ebae-200">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="0ebae-201">设备注册状态。</span><span class="sxs-lookup"><span data-stu-id="0ebae-201">Device registration state.</span></span> <span data-ttu-id="0ebae-202">可取值为：`notRegistered`、`registered`、`revoked`、`keyConflict`、`approvalPending`、`certificateReset`、`notRegisteredPendingEnrollment`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="0ebae-202">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="0ebae-203">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="0ebae-203">deviceCategoryDisplayName</span></span>|<span data-ttu-id="0ebae-204">字符串</span><span class="sxs-lookup"><span data-stu-id="0ebae-204">String</span></span>|<span data-ttu-id="0ebae-205">设备类别显示名称。</span><span class="sxs-lookup"><span data-stu-id="0ebae-205">Device category display name</span></span>|
|<span data-ttu-id="0ebae-206">isSupervised</span><span class="sxs-lookup"><span data-stu-id="0ebae-206">isSupervised</span></span>|<span data-ttu-id="0ebae-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ebae-207">Boolean</span></span>|<span data-ttu-id="0ebae-208">设备受监督状态</span><span class="sxs-lookup"><span data-stu-id="0ebae-208">Device supervised status</span></span>|
|<span data-ttu-id="0ebae-209">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="0ebae-209">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="0ebae-210">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ebae-210">DateTimeOffset</span></span>|<span data-ttu-id="0ebae-211">设备上次与 Exchange 联系的时间。</span><span class="sxs-lookup"><span data-stu-id="0ebae-211">Last time the device contacted Exchange.</span></span>|
|<span data-ttu-id="0ebae-212">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="0ebae-212">exchangeAccessState</span></span>|[<span data-ttu-id="0ebae-213">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="0ebae-213">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="0ebae-214">Exchange 中设备的访问状态。</span><span class="sxs-lookup"><span data-stu-id="0ebae-214">The Access State of the device in Exchange.</span></span> <span data-ttu-id="0ebae-215">可取值为：`none`、`unknown`、`allowed`、`blocked`、`quarantined`。</span><span class="sxs-lookup"><span data-stu-id="0ebae-215">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="0ebae-216">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="0ebae-216">exchangeAccessStateReason</span></span>|[<span data-ttu-id="0ebae-217">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="0ebae-217">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="0ebae-218">Exchange 中设备访问状态的出现原因。</span><span class="sxs-lookup"><span data-stu-id="0ebae-218">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="0ebae-219">可取值为：`none`、`unknown`、`exchangeGlobalRule`、`exchangeIndividualRule`、`exchangeDeviceRule`、`exchangeUpgrade`、`exchangeMailboxPolicy`、`other`、`compliant`、`notCompliant`、`notEnrolled`、`unknownLocation`、`mfaRequired`、`azureADBlockDueToAccessPolicy`、`compromisedPassword`、`deviceNotKnownWithManagedApp`。</span><span class="sxs-lookup"><span data-stu-id="0ebae-219">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="0ebae-220">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="0ebae-220">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="0ebae-221">String</span><span class="sxs-lookup"><span data-stu-id="0ebae-221">String</span></span>|<span data-ttu-id="0ebae-222">允许与设备建立远程协助会话的 URL。</span><span class="sxs-lookup"><span data-stu-id="0ebae-222">Url that allows a Remote Assistance session to be established with the device.</span></span>|
|<span data-ttu-id="0ebae-223">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="0ebae-223">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="0ebae-224">字符串</span><span class="sxs-lookup"><span data-stu-id="0ebae-224">String</span></span>|<span data-ttu-id="0ebae-225">用于在创建远程协助会话对象时识别问题的错误字符串。</span><span class="sxs-lookup"><span data-stu-id="0ebae-225">An error string that identifies issues when creating Remote Assistance session objects.</span></span>|
|<span data-ttu-id="0ebae-226">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="0ebae-226">isEncrypted</span></span>|<span data-ttu-id="0ebae-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ebae-227">Boolean</span></span>|<span data-ttu-id="0ebae-228">设备加密状态</span><span class="sxs-lookup"><span data-stu-id="0ebae-228">Device encryption status</span></span>|
|<span data-ttu-id="0ebae-229">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0ebae-229">userPrincipalName</span></span>|<span data-ttu-id="0ebae-230">字符串</span><span class="sxs-lookup"><span data-stu-id="0ebae-230">String</span></span>|<span data-ttu-id="0ebae-231">设备用户主体名称</span><span class="sxs-lookup"><span data-stu-id="0ebae-231">Device user principal name</span></span>|
|<span data-ttu-id="0ebae-232">model</span><span class="sxs-lookup"><span data-stu-id="0ebae-232">model</span></span>|<span data-ttu-id="0ebae-233">字符串</span><span class="sxs-lookup"><span data-stu-id="0ebae-233">String</span></span>|<span data-ttu-id="0ebae-234">设备的型号</span><span class="sxs-lookup"><span data-stu-id="0ebae-234">Model of the device</span></span>|
|<span data-ttu-id="0ebae-235">manufacturer</span><span class="sxs-lookup"><span data-stu-id="0ebae-235">manufacturer</span></span>|<span data-ttu-id="0ebae-236">字符串</span><span class="sxs-lookup"><span data-stu-id="0ebae-236">String</span></span>|<span data-ttu-id="0ebae-237">设备的制造商</span><span class="sxs-lookup"><span data-stu-id="0ebae-237">Manufacturer of the device</span></span>|
|<span data-ttu-id="0ebae-238">imei</span><span class="sxs-lookup"><span data-stu-id="0ebae-238">imei</span></span>|<span data-ttu-id="0ebae-239">字符串</span><span class="sxs-lookup"><span data-stu-id="0ebae-239">String</span></span>|<span data-ttu-id="0ebae-240">IMEI</span><span class="sxs-lookup"><span data-stu-id="0ebae-240">IMEI</span></span>|
|<span data-ttu-id="0ebae-241">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="0ebae-241">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="0ebae-242">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ebae-242">DateTimeOffset</span></span>|<span data-ttu-id="0ebae-243">设备符合性宽限期的到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="0ebae-243">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="0ebae-244">serialNumber</span><span class="sxs-lookup"><span data-stu-id="0ebae-244">serialNumber</span></span>|<span data-ttu-id="0ebae-245">字符串</span><span class="sxs-lookup"><span data-stu-id="0ebae-245">String</span></span>|<span data-ttu-id="0ebae-246">序列号</span><span class="sxs-lookup"><span data-stu-id="0ebae-246">SerialNumber</span></span>|
|<span data-ttu-id="0ebae-247">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="0ebae-247">phoneNumber</span></span>|<span data-ttu-id="0ebae-248">字符串</span><span class="sxs-lookup"><span data-stu-id="0ebae-248">String</span></span>|<span data-ttu-id="0ebae-249">设备的电话号码</span><span class="sxs-lookup"><span data-stu-id="0ebae-249">Phone number of the device</span></span>|
|<span data-ttu-id="0ebae-250">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="0ebae-250">androidSecurityPatchLevel</span></span>|<span data-ttu-id="0ebae-251">字符串</span><span class="sxs-lookup"><span data-stu-id="0ebae-251">String</span></span>|<span data-ttu-id="0ebae-252">Android 安全修补程序级别</span><span class="sxs-lookup"><span data-stu-id="0ebae-252">Android security patch level</span></span>|
|<span data-ttu-id="0ebae-253">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="0ebae-253">userDisplayName</span></span>|<span data-ttu-id="0ebae-254">String</span><span class="sxs-lookup"><span data-stu-id="0ebae-254">String</span></span>|<span data-ttu-id="0ebae-255">用户显示名称</span><span class="sxs-lookup"><span data-stu-id="0ebae-255">User display name</span></span>|
|<span data-ttu-id="0ebae-256">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="0ebae-256">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="0ebae-257">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="0ebae-257">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="0ebae-258">ConfigrMgr 客户端启用的功能</span><span class="sxs-lookup"><span data-stu-id="0ebae-258">ConfigrMgr client enabled features</span></span>|
|<span data-ttu-id="0ebae-259">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="0ebae-259">wiFiMacAddress</span></span>|<span data-ttu-id="0ebae-260">字符串</span><span class="sxs-lookup"><span data-stu-id="0ebae-260">String</span></span>|<span data-ttu-id="0ebae-261">Wi-Fi MAC</span><span class="sxs-lookup"><span data-stu-id="0ebae-261">Wi-Fi MAC</span></span>|
|<span data-ttu-id="0ebae-262">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="0ebae-262">deviceHealthAttestationState</span></span>|[<span data-ttu-id="0ebae-263">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="0ebae-263">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="0ebae-264">设备运行状况证明状态。</span><span class="sxs-lookup"><span data-stu-id="0ebae-264">The device health attestation state.</span></span>|
|<span data-ttu-id="0ebae-265">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="0ebae-265">subscriberCarrier</span></span>|<span data-ttu-id="0ebae-266">字符串</span><span class="sxs-lookup"><span data-stu-id="0ebae-266">String</span></span>|<span data-ttu-id="0ebae-267">订阅者运营商</span><span class="sxs-lookup"><span data-stu-id="0ebae-267">Subscriber Carrier</span></span>|
|<span data-ttu-id="0ebae-268">meid</span><span class="sxs-lookup"><span data-stu-id="0ebae-268">meid</span></span>|<span data-ttu-id="0ebae-269">字符串</span><span class="sxs-lookup"><span data-stu-id="0ebae-269">String</span></span>|<span data-ttu-id="0ebae-270">MEID</span><span class="sxs-lookup"><span data-stu-id="0ebae-270">MEID</span></span>|
|<span data-ttu-id="0ebae-271">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="0ebae-271">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="0ebae-272">Int64</span><span class="sxs-lookup"><span data-stu-id="0ebae-272">Int64</span></span>|<span data-ttu-id="0ebae-273">存储空间总字节数</span><span class="sxs-lookup"><span data-stu-id="0ebae-273">Total Storage in Bytes</span></span>|
|<span data-ttu-id="0ebae-274">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="0ebae-274">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="0ebae-275">Int64</span><span class="sxs-lookup"><span data-stu-id="0ebae-275">Int64</span></span>|<span data-ttu-id="0ebae-276">可用存储空间字节数</span><span class="sxs-lookup"><span data-stu-id="0ebae-276">Free Storage in Bytes</span></span>|
|<span data-ttu-id="0ebae-277">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="0ebae-277">managedDeviceName</span></span>|<span data-ttu-id="0ebae-278">String</span><span class="sxs-lookup"><span data-stu-id="0ebae-278">String</span></span>|<span data-ttu-id="0ebae-279">用于识别设备的自动生成的名称。</span><span class="sxs-lookup"><span data-stu-id="0ebae-279">Automatically generated name to identify a device.</span></span> <span data-ttu-id="0ebae-280">可以覆盖为用户友好名称。</span><span class="sxs-lookup"><span data-stu-id="0ebae-280">Can be overwritten to a user friendly name.</span></span>|
|<span data-ttu-id="0ebae-281">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="0ebae-281">partnerReportedThreatState</span></span>|[<span data-ttu-id="0ebae-282">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="0ebae-282">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="0ebae-283">指示帐户和设备正在使用移动威胁防护合作伙伴时设备的威胁状态。</span><span class="sxs-lookup"><span data-stu-id="0ebae-283">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="0ebae-284">只读。</span><span class="sxs-lookup"><span data-stu-id="0ebae-284">Read Only.</span></span> <span data-ttu-id="0ebae-285">可取值为：`unknown`、`activated`、`deactivated`、`secured`、`lowSeverity`、`mediumSeverity`、`highSeverity`、`unresponsive`、`compromised`、`misconfigured`。</span><span class="sxs-lookup"><span data-stu-id="0ebae-285">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|



## <a name="response"></a><span data-ttu-id="0ebae-286">响应</span><span class="sxs-lookup"><span data-stu-id="0ebae-286">Response</span></span>
<span data-ttu-id="0ebae-287">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [managedDevice](../resources/intune-devices-manageddevice.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0ebae-287">If successful, this method returns a `200 OK` response code and an updated [managedDevice](../resources/intune-devices-manageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ebae-288">示例</span><span class="sxs-lookup"><span data-stu-id="0ebae-288">Example</span></span>

### <a name="request"></a><span data-ttu-id="0ebae-289">请求</span><span class="sxs-lookup"><span data-stu-id="0ebae-289">Request</span></span>
<span data-ttu-id="0ebae-290">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0ebae-290">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0ebae-291">响应</span><span class="sxs-lookup"><span data-stu-id="0ebae-291">Response</span></span>
<span data-ttu-id="0ebae-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0ebae-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




