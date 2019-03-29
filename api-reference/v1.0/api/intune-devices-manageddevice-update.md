---
title: 更新 managedDevice
description: 更新 managedDevice 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 12c8c2dc628b7fcecef81296ca56f17845b39478
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30962860"
---
# <a name="update-manageddevice"></a><span data-ttu-id="1dc3d-103">更新 managedDevice</span><span class="sxs-lookup"><span data-stu-id="1dc3d-103">Update managedDevice</span></span>

> <span data-ttu-id="1dc3d-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1dc3d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1dc3d-105">更新 [managedDevice](../resources/intune-devices-manageddevice.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="1dc3d-105">Update the properties of a [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1dc3d-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="1dc3d-106">Prerequisites</span></span>
<span data-ttu-id="1dc3d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1dc3d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1dc3d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1dc3d-109">Permission type</span></span>|<span data-ttu-id="1dc3d-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1dc3d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1dc3d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1dc3d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1dc3d-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1dc3d-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="1dc3d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1dc3d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1dc3d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="1dc3d-114">Not supported.</span></span>|
|<span data-ttu-id="1dc3d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="1dc3d-115">Application</span></span>|<span data-ttu-id="1dc3d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1dc3d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1dc3d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1dc3d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}/managedDevices/{managedDeviceId}
PATCH /deviceManagement/managedDevices/{managedDeviceId}
PATCH /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}
```

## <a name="request-headers"></a><span data-ttu-id="1dc3d-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="1dc3d-118">Request headers</span></span>
|<span data-ttu-id="1dc3d-119">标头</span><span class="sxs-lookup"><span data-stu-id="1dc3d-119">Header</span></span>|<span data-ttu-id="1dc3d-120">值</span><span class="sxs-lookup"><span data-stu-id="1dc3d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1dc3d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1dc3d-121">Authorization</span></span>|<span data-ttu-id="1dc3d-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1dc3d-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1dc3d-123">接受</span><span class="sxs-lookup"><span data-stu-id="1dc3d-123">Accept</span></span>|<span data-ttu-id="1dc3d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1dc3d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1dc3d-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="1dc3d-125">Request body</span></span>
<span data-ttu-id="1dc3d-126">在请求正文中，提供 [managedDevice](../resources/intune-devices-manageddevice.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1dc3d-126">In the request body, supply a JSON representation for the [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>

<span data-ttu-id="1dc3d-127">下表显示创建 [managedDevice](../resources/intune-devices-manageddevice.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="1dc3d-127">The following table shows the properties that are required when you create the [managedDevice](../resources/intune-devices-manageddevice.md).</span></span>

|<span data-ttu-id="1dc3d-128">属性</span><span class="sxs-lookup"><span data-stu-id="1dc3d-128">Property</span></span>|<span data-ttu-id="1dc3d-129">类型</span><span class="sxs-lookup"><span data-stu-id="1dc3d-129">Type</span></span>|<span data-ttu-id="1dc3d-130">说明</span><span class="sxs-lookup"><span data-stu-id="1dc3d-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1dc3d-131">id</span><span class="sxs-lookup"><span data-stu-id="1dc3d-131">id</span></span>|<span data-ttu-id="1dc3d-132">String</span><span class="sxs-lookup"><span data-stu-id="1dc3d-132">String</span></span>|<span data-ttu-id="1dc3d-133">设备唯一标识符</span><span class="sxs-lookup"><span data-stu-id="1dc3d-133">Unique Identifier for the device</span></span>|
|<span data-ttu-id="1dc3d-134">userId</span><span class="sxs-lookup"><span data-stu-id="1dc3d-134">userId</span></span>|<span data-ttu-id="1dc3d-135">String</span><span class="sxs-lookup"><span data-stu-id="1dc3d-135">String</span></span>|<span data-ttu-id="1dc3d-136">与设备关联的用户的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="1dc3d-136">Unique Identifier for the user associated with the device</span></span>|
|<span data-ttu-id="1dc3d-137">deviceName</span><span class="sxs-lookup"><span data-stu-id="1dc3d-137">deviceName</span></span>|<span data-ttu-id="1dc3d-138">String</span><span class="sxs-lookup"><span data-stu-id="1dc3d-138">String</span></span>|<span data-ttu-id="1dc3d-139">设备的名称</span><span class="sxs-lookup"><span data-stu-id="1dc3d-139">Name of the device</span></span>|
|<span data-ttu-id="1dc3d-140">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="1dc3d-140">managedDeviceOwnerType</span></span>|[<span data-ttu-id="1dc3d-141">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="1dc3d-141">managedDeviceOwnerType</span></span>](../resources/intune-devices-manageddeviceownertype.md)|<span data-ttu-id="1dc3d-142">设备的所有权。</span><span class="sxs-lookup"><span data-stu-id="1dc3d-142">Ownership of the device.</span></span> <span data-ttu-id="1dc3d-143">可以是 "公司" 或 "个人"。</span><span class="sxs-lookup"><span data-stu-id="1dc3d-143">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="1dc3d-144">可取值为：`unknown`、`company`、`personal`。</span><span class="sxs-lookup"><span data-stu-id="1dc3d-144">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="1dc3d-145">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="1dc3d-145">deviceActionResults</span></span>|<span data-ttu-id="1dc3d-146">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1dc3d-146">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="1dc3d-147">ComplexType deviceActionResult 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="1dc3d-147">List of ComplexType deviceActionResult objects.</span></span>|
|<span data-ttu-id="1dc3d-148">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="1dc3d-148">enrolledDateTime</span></span>|<span data-ttu-id="1dc3d-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1dc3d-149">DateTimeOffset</span></span>|<span data-ttu-id="1dc3d-150">设备的注册时间。</span><span class="sxs-lookup"><span data-stu-id="1dc3d-150">Enrollment time of the device.</span></span>|
|<span data-ttu-id="1dc3d-151">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="1dc3d-151">lastSyncDateTime</span></span>|<span data-ttu-id="1dc3d-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1dc3d-152">DateTimeOffset</span></span>|<span data-ttu-id="1dc3d-153">设备上次成功完成与 Intune 同步的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="1dc3d-153">The date and time that the device last completed a successful sync with Intune.</span></span>|
|<span data-ttu-id="1dc3d-154">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="1dc3d-154">operatingSystem</span></span>|<span data-ttu-id="1dc3d-155">String</span><span class="sxs-lookup"><span data-stu-id="1dc3d-155">String</span></span>|<span data-ttu-id="1dc3d-156">设备的操作系统。</span><span class="sxs-lookup"><span data-stu-id="1dc3d-156">Operating system of the device.</span></span> <span data-ttu-id="1dc3d-157">Windows、iOS 等。</span><span class="sxs-lookup"><span data-stu-id="1dc3d-157">Windows, iOS, etc.</span></span>|
|<span data-ttu-id="1dc3d-158">complianceState</span><span class="sxs-lookup"><span data-stu-id="1dc3d-158">complianceState</span></span>|[<span data-ttu-id="1dc3d-159">complianceState</span><span class="sxs-lookup"><span data-stu-id="1dc3d-159">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="1dc3d-160">设备的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="1dc3d-160">Compliance state of the device.</span></span> <span data-ttu-id="1dc3d-161">可取值为：`unknown`、`compliant`、`noncompliant`、`conflict`、`error`、`inGracePeriod`、`configManager`。</span><span class="sxs-lookup"><span data-stu-id="1dc3d-161">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="1dc3d-162">jailBroken</span><span class="sxs-lookup"><span data-stu-id="1dc3d-162">jailBroken</span></span>|<span data-ttu-id="1dc3d-163">String</span><span class="sxs-lookup"><span data-stu-id="1dc3d-163">String</span></span>|<span data-ttu-id="1dc3d-164">设备是否已越狱或取得 root 权限。</span><span class="sxs-lookup"><span data-stu-id="1dc3d-164">whether the device is jail broken or rooted.</span></span>|
|<span data-ttu-id="1dc3d-165">managementAgent</span><span class="sxs-lookup"><span data-stu-id="1dc3d-165">managementAgent</span></span>|[<span data-ttu-id="1dc3d-166">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="1dc3d-166">managementAgentType</span></span>](../resources/intune-devices-managementagenttype.md)|<span data-ttu-id="1dc3d-167">设备的管理通道。</span><span class="sxs-lookup"><span data-stu-id="1dc3d-167">Management channel of the device.</span></span> <span data-ttu-id="1dc3d-168">Intune、EAS 等 可取值为：`eas`、`mdm`、`easMdm`、`intuneClient`、`easIntuneClient`、`configurationManagerClient`、`configurationManagerClientMdm`、`configurationManagerClientMdmEas`、`unknown`、`jamf`、`googleCloudDevicePolicyController`。</span><span class="sxs-lookup"><span data-stu-id="1dc3d-168">Intune, EAS, etc. Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`.</span></span>|
|<span data-ttu-id="1dc3d-169">osVersion</span><span class="sxs-lookup"><span data-stu-id="1dc3d-169">osVersion</span></span>|<span data-ttu-id="1dc3d-170">String</span><span class="sxs-lookup"><span data-stu-id="1dc3d-170">String</span></span>|<span data-ttu-id="1dc3d-171">设备的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="1dc3d-171">Operating system version of the device.</span></span>|
|<span data-ttu-id="1dc3d-172">easActivated</span><span class="sxs-lookup"><span data-stu-id="1dc3d-172">easActivated</span></span>|<span data-ttu-id="1dc3d-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="1dc3d-173">Boolean</span></span>|<span data-ttu-id="1dc3d-174">设备是否已激活 Exchange ActiveSync。</span><span class="sxs-lookup"><span data-stu-id="1dc3d-174">Whether the device is Exchange ActiveSync activated.</span></span>|
|<span data-ttu-id="1dc3d-175">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="1dc3d-175">easDeviceId</span></span>|<span data-ttu-id="1dc3d-176">String</span><span class="sxs-lookup"><span data-stu-id="1dc3d-176">String</span></span>|<span data-ttu-id="1dc3d-177">设备的 Exchange ActiveSync ID。</span><span class="sxs-lookup"><span data-stu-id="1dc3d-177">Exchange ActiveSync Id of the device.</span></span>|
|<span data-ttu-id="1dc3d-178">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="1dc3d-178">easActivationDateTime</span></span>|<span data-ttu-id="1dc3d-179">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1dc3d-179">DateTimeOffset</span></span>|<span data-ttu-id="1dc3d-180">设备的 Exchange ActivationSync 激活时间。</span><span class="sxs-lookup"><span data-stu-id="1dc3d-180">Exchange ActivationSync activation time of the device.</span></span>|
|<span data-ttu-id="1dc3d-181">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="1dc3d-181">azureADRegistered</span></span>|<span data-ttu-id="1dc3d-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="1dc3d-182">Boolean</span></span>|<span data-ttu-id="1dc3d-183">设备是否已注册 Azure Active Directory。</span><span class="sxs-lookup"><span data-stu-id="1dc3d-183">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="1dc3d-184">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="1dc3d-184">deviceEnrollmentType</span></span>|[<span data-ttu-id="1dc3d-185">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="1dc3d-185">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="1dc3d-186">设备的注册类型。</span><span class="sxs-lookup"><span data-stu-id="1dc3d-186">Enrollment type of the device.</span></span> <span data-ttu-id="1dc3d-187">可取值为：`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement`。</span><span class="sxs-lookup"><span data-stu-id="1dc3d-187">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="1dc3d-188">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="1dc3d-188">activationLockBypassCode</span></span>|<span data-ttu-id="1dc3d-189">String</span><span class="sxs-lookup"><span data-stu-id="1dc3d-189">String</span></span>|<span data-ttu-id="1dc3d-190">允许绕过设备上的激活锁的代码。</span><span class="sxs-lookup"><span data-stu-id="1dc3d-190">Code that allows the Activation Lock on a device to be bypassed.</span></span>|
|<span data-ttu-id="1dc3d-191">emailAddress</span><span class="sxs-lookup"><span data-stu-id="1dc3d-191">emailAddress</span></span>|<span data-ttu-id="1dc3d-192">String</span><span class="sxs-lookup"><span data-stu-id="1dc3d-192">String</span></span>|<span data-ttu-id="1dc3d-193">与设备关联的用户的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="1dc3d-193">Email(s) for the user associated with the device</span></span>|
|<span data-ttu-id="1dc3d-194">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="1dc3d-194">azureADDeviceId</span></span>|<span data-ttu-id="1dc3d-195">String</span><span class="sxs-lookup"><span data-stu-id="1dc3d-195">String</span></span>|<span data-ttu-id="1dc3d-196">Azure Active Directory 设备的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="1dc3d-196">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="1dc3d-197">只读。</span><span class="sxs-lookup"><span data-stu-id="1dc3d-197">Read only.</span></span>|
|<span data-ttu-id="1dc3d-198">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="1dc3d-198">deviceRegistrationState</span></span>|[<span data-ttu-id="1dc3d-199">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="1dc3d-199">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="1dc3d-200">设备注册状态。</span><span class="sxs-lookup"><span data-stu-id="1dc3d-200">Device registration state.</span></span> <span data-ttu-id="1dc3d-201">可取值为：`notRegistered`、`registered`、`revoked`、`keyConflict`、`approvalPending`、`certificateReset`、`notRegisteredPendingEnrollment`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="1dc3d-201">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="1dc3d-202">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="1dc3d-202">deviceCategoryDisplayName</span></span>|<span data-ttu-id="1dc3d-203">String</span><span class="sxs-lookup"><span data-stu-id="1dc3d-203">String</span></span>|<span data-ttu-id="1dc3d-204">设备类别显示名称。</span><span class="sxs-lookup"><span data-stu-id="1dc3d-204">Device category display name</span></span>|
|<span data-ttu-id="1dc3d-205">isSupervised</span><span class="sxs-lookup"><span data-stu-id="1dc3d-205">isSupervised</span></span>|<span data-ttu-id="1dc3d-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="1dc3d-206">Boolean</span></span>|<span data-ttu-id="1dc3d-207">设备受监督状态</span><span class="sxs-lookup"><span data-stu-id="1dc3d-207">Device supervised status</span></span>|
|<span data-ttu-id="1dc3d-208">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="1dc3d-208">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="1dc3d-209">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1dc3d-209">DateTimeOffset</span></span>|<span data-ttu-id="1dc3d-210">设备上次与 Exchange 联系的时间。</span><span class="sxs-lookup"><span data-stu-id="1dc3d-210">Last time the device contacted Exchange.</span></span>|
|<span data-ttu-id="1dc3d-211">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="1dc3d-211">exchangeAccessState</span></span>|[<span data-ttu-id="1dc3d-212">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="1dc3d-212">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="1dc3d-213">Exchange 中设备的访问状态。</span><span class="sxs-lookup"><span data-stu-id="1dc3d-213">The Access State of the device in Exchange.</span></span> <span data-ttu-id="1dc3d-214">可取值为：`none`、`unknown`、`allowed`、`blocked`、`quarantined`。</span><span class="sxs-lookup"><span data-stu-id="1dc3d-214">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="1dc3d-215">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="1dc3d-215">exchangeAccessStateReason</span></span>|[<span data-ttu-id="1dc3d-216">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="1dc3d-216">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="1dc3d-217">Exchange 中设备访问状态的出现原因。</span><span class="sxs-lookup"><span data-stu-id="1dc3d-217">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="1dc3d-218">可取值为：`none`、`unknown`、`exchangeGlobalRule`、`exchangeIndividualRule`、`exchangeDeviceRule`、`exchangeUpgrade`、`exchangeMailboxPolicy`、`other`、`compliant`、`notCompliant`、`notEnrolled`、`unknownLocation`、`mfaRequired`、`azureADBlockDueToAccessPolicy`、`compromisedPassword`、`deviceNotKnownWithManagedApp`。</span><span class="sxs-lookup"><span data-stu-id="1dc3d-218">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="1dc3d-219">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="1dc3d-219">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="1dc3d-220">String</span><span class="sxs-lookup"><span data-stu-id="1dc3d-220">String</span></span>|<span data-ttu-id="1dc3d-221">允许与设备建立远程协助会话的 URL。</span><span class="sxs-lookup"><span data-stu-id="1dc3d-221">Url that allows a Remote Assistance session to be established with the device.</span></span>|
|<span data-ttu-id="1dc3d-222">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="1dc3d-222">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="1dc3d-223">String</span><span class="sxs-lookup"><span data-stu-id="1dc3d-223">String</span></span>|<span data-ttu-id="1dc3d-224">用于在创建远程协助会话对象时识别问题的错误字符串。</span><span class="sxs-lookup"><span data-stu-id="1dc3d-224">An error string that identifies issues when creating Remote Assistance session objects.</span></span>|
|<span data-ttu-id="1dc3d-225">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="1dc3d-225">isEncrypted</span></span>|<span data-ttu-id="1dc3d-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="1dc3d-226">Boolean</span></span>|<span data-ttu-id="1dc3d-227">设备加密状态</span><span class="sxs-lookup"><span data-stu-id="1dc3d-227">Device encryption status</span></span>|
|<span data-ttu-id="1dc3d-228">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="1dc3d-228">userPrincipalName</span></span>|<span data-ttu-id="1dc3d-229">String</span><span class="sxs-lookup"><span data-stu-id="1dc3d-229">String</span></span>|<span data-ttu-id="1dc3d-230">设备用户主体名称</span><span class="sxs-lookup"><span data-stu-id="1dc3d-230">Device user principal name</span></span>|
|<span data-ttu-id="1dc3d-231">model</span><span class="sxs-lookup"><span data-stu-id="1dc3d-231">model</span></span>|<span data-ttu-id="1dc3d-232">String</span><span class="sxs-lookup"><span data-stu-id="1dc3d-232">String</span></span>|<span data-ttu-id="1dc3d-233">设备的型号</span><span class="sxs-lookup"><span data-stu-id="1dc3d-233">Model of the device</span></span>|
|<span data-ttu-id="1dc3d-234">manufacturer</span><span class="sxs-lookup"><span data-stu-id="1dc3d-234">manufacturer</span></span>|<span data-ttu-id="1dc3d-235">String</span><span class="sxs-lookup"><span data-stu-id="1dc3d-235">String</span></span>|<span data-ttu-id="1dc3d-236">设备的制造商</span><span class="sxs-lookup"><span data-stu-id="1dc3d-236">Manufacturer of the device</span></span>|
|<span data-ttu-id="1dc3d-237">imei</span><span class="sxs-lookup"><span data-stu-id="1dc3d-237">imei</span></span>|<span data-ttu-id="1dc3d-238">String</span><span class="sxs-lookup"><span data-stu-id="1dc3d-238">String</span></span>|<span data-ttu-id="1dc3d-239">IMEI</span><span class="sxs-lookup"><span data-stu-id="1dc3d-239">IMEI</span></span>|
|<span data-ttu-id="1dc3d-240">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="1dc3d-240">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="1dc3d-241">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1dc3d-241">DateTimeOffset</span></span>|<span data-ttu-id="1dc3d-242">设备符合性宽限期的到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="1dc3d-242">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="1dc3d-243">serialNumber</span><span class="sxs-lookup"><span data-stu-id="1dc3d-243">serialNumber</span></span>|<span data-ttu-id="1dc3d-244">字符串</span><span class="sxs-lookup"><span data-stu-id="1dc3d-244">String</span></span>|<span data-ttu-id="1dc3d-245">序列号</span><span class="sxs-lookup"><span data-stu-id="1dc3d-245">SerialNumber</span></span>|
|<span data-ttu-id="1dc3d-246">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="1dc3d-246">phoneNumber</span></span>|<span data-ttu-id="1dc3d-247">String</span><span class="sxs-lookup"><span data-stu-id="1dc3d-247">String</span></span>|<span data-ttu-id="1dc3d-248">设备的电话号码</span><span class="sxs-lookup"><span data-stu-id="1dc3d-248">Phone number of the device</span></span>|
|<span data-ttu-id="1dc3d-249">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="1dc3d-249">androidSecurityPatchLevel</span></span>|<span data-ttu-id="1dc3d-250">String</span><span class="sxs-lookup"><span data-stu-id="1dc3d-250">String</span></span>|<span data-ttu-id="1dc3d-251">Android 安全修补程序级别</span><span class="sxs-lookup"><span data-stu-id="1dc3d-251">Android security patch level</span></span>|
|<span data-ttu-id="1dc3d-252">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="1dc3d-252">userDisplayName</span></span>|<span data-ttu-id="1dc3d-253">String</span><span class="sxs-lookup"><span data-stu-id="1dc3d-253">String</span></span>|<span data-ttu-id="1dc3d-254">用户显示名称</span><span class="sxs-lookup"><span data-stu-id="1dc3d-254">User display name</span></span>|
|<span data-ttu-id="1dc3d-255">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="1dc3d-255">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="1dc3d-256">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="1dc3d-256">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="1dc3d-257">ConfigrMgr 客户端启用的功能</span><span class="sxs-lookup"><span data-stu-id="1dc3d-257">ConfigrMgr client enabled features</span></span>|
|<span data-ttu-id="1dc3d-258">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="1dc3d-258">wiFiMacAddress</span></span>|<span data-ttu-id="1dc3d-259">String</span><span class="sxs-lookup"><span data-stu-id="1dc3d-259">String</span></span>|<span data-ttu-id="1dc3d-260">Wi-Fi MAC</span><span class="sxs-lookup"><span data-stu-id="1dc3d-260">Wi-Fi MAC</span></span>|
|<span data-ttu-id="1dc3d-261">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="1dc3d-261">deviceHealthAttestationState</span></span>|[<span data-ttu-id="1dc3d-262">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="1dc3d-262">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="1dc3d-263">设备运行状况证明状态。</span><span class="sxs-lookup"><span data-stu-id="1dc3d-263">The device health attestation state.</span></span>|
|<span data-ttu-id="1dc3d-264">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="1dc3d-264">subscriberCarrier</span></span>|<span data-ttu-id="1dc3d-265">String</span><span class="sxs-lookup"><span data-stu-id="1dc3d-265">String</span></span>|<span data-ttu-id="1dc3d-266">订阅者运营商</span><span class="sxs-lookup"><span data-stu-id="1dc3d-266">Subscriber Carrier</span></span>|
|<span data-ttu-id="1dc3d-267">meid</span><span class="sxs-lookup"><span data-stu-id="1dc3d-267">meid</span></span>|<span data-ttu-id="1dc3d-268">String</span><span class="sxs-lookup"><span data-stu-id="1dc3d-268">String</span></span>|<span data-ttu-id="1dc3d-269">MEID</span><span class="sxs-lookup"><span data-stu-id="1dc3d-269">MEID</span></span>|
|<span data-ttu-id="1dc3d-270">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="1dc3d-270">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="1dc3d-271">Int64</span><span class="sxs-lookup"><span data-stu-id="1dc3d-271">Int64</span></span>|<span data-ttu-id="1dc3d-272">存储空间总字节数</span><span class="sxs-lookup"><span data-stu-id="1dc3d-272">Total Storage in Bytes</span></span>|
|<span data-ttu-id="1dc3d-273">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="1dc3d-273">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="1dc3d-274">Int64</span><span class="sxs-lookup"><span data-stu-id="1dc3d-274">Int64</span></span>|<span data-ttu-id="1dc3d-275">可用存储空间字节数</span><span class="sxs-lookup"><span data-stu-id="1dc3d-275">Free Storage in Bytes</span></span>|
|<span data-ttu-id="1dc3d-276">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="1dc3d-276">managedDeviceName</span></span>|<span data-ttu-id="1dc3d-277">String</span><span class="sxs-lookup"><span data-stu-id="1dc3d-277">String</span></span>|<span data-ttu-id="1dc3d-278">用于识别设备的自动生成的名称。</span><span class="sxs-lookup"><span data-stu-id="1dc3d-278">Automatically generated name to identify a device.</span></span> <span data-ttu-id="1dc3d-279">可以覆盖为用户友好名称。</span><span class="sxs-lookup"><span data-stu-id="1dc3d-279">Can be overwritten to a user friendly name.</span></span>|
|<span data-ttu-id="1dc3d-280">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="1dc3d-280">partnerReportedThreatState</span></span>|[<span data-ttu-id="1dc3d-281">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="1dc3d-281">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="1dc3d-282">指示帐户和设备正在使用移动威胁防护合作伙伴时设备的威胁状态。</span><span class="sxs-lookup"><span data-stu-id="1dc3d-282">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="1dc3d-283">只读。</span><span class="sxs-lookup"><span data-stu-id="1dc3d-283">Read Only.</span></span> <span data-ttu-id="1dc3d-284">可取值为：`unknown`、`activated`、`deactivated`、`secured`、`lowSeverity`、`mediumSeverity`、`highSeverity`、`unresponsive`、`compromised`、`misconfigured`。</span><span class="sxs-lookup"><span data-stu-id="1dc3d-284">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|



## <a name="response"></a><span data-ttu-id="1dc3d-285">响应</span><span class="sxs-lookup"><span data-stu-id="1dc3d-285">Response</span></span>
<span data-ttu-id="1dc3d-286">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [managedDevice](../resources/intune-devices-manageddevice.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1dc3d-286">If successful, this method returns a `200 OK` response code and an updated [managedDevice](../resources/intune-devices-manageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1dc3d-287">示例</span><span class="sxs-lookup"><span data-stu-id="1dc3d-287">Example</span></span>

### <a name="request"></a><span data-ttu-id="1dc3d-288">请求</span><span class="sxs-lookup"><span data-stu-id="1dc3d-288">Request</span></span>
<span data-ttu-id="1dc3d-289">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1dc3d-289">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1dc3d-290">响应</span><span class="sxs-lookup"><span data-stu-id="1dc3d-290">Response</span></span>
<span data-ttu-id="1dc3d-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1dc3d-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



