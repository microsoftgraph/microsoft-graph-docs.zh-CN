---
title: 更新 managedDevice
description: 更新 managedDevice 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e3711888ee2c5e6f3d3a5281ec6e14d521eb9695
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30162466"
---
# <a name="update-manageddevice"></a><span data-ttu-id="99fc9-103">更新 managedDevice</span><span class="sxs-lookup"><span data-stu-id="99fc9-103">Update managedDevice</span></span>

> <span data-ttu-id="99fc9-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="99fc9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="99fc9-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="99fc9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="99fc9-106">更新 [managedDevice](../resources/intune-devices-manageddevice.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="99fc9-106">Update the properties of a [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="99fc9-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="99fc9-107">Prerequisites</span></span>
<span data-ttu-id="99fc9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="99fc9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="99fc9-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="99fc9-110">Permission type</span></span>|<span data-ttu-id="99fc9-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="99fc9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="99fc9-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="99fc9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="99fc9-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99fc9-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="99fc9-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="99fc9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="99fc9-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="99fc9-115">Not supported.</span></span>|
|<span data-ttu-id="99fc9-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="99fc9-116">Application</span></span>|<span data-ttu-id="99fc9-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="99fc9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="99fc9-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="99fc9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}/managedDevices/{managedDeviceId}
PATCH /deviceManagement/managedDevices/{managedDeviceId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}
```

## <a name="request-headers"></a><span data-ttu-id="99fc9-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="99fc9-119">Request headers</span></span>
|<span data-ttu-id="99fc9-120">标头</span><span class="sxs-lookup"><span data-stu-id="99fc9-120">Header</span></span>|<span data-ttu-id="99fc9-121">值</span><span class="sxs-lookup"><span data-stu-id="99fc9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="99fc9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="99fc9-122">Authorization</span></span>|<span data-ttu-id="99fc9-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="99fc9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="99fc9-124">Accept</span><span class="sxs-lookup"><span data-stu-id="99fc9-124">Accept</span></span>|<span data-ttu-id="99fc9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="99fc9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="99fc9-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="99fc9-126">Request body</span></span>
<span data-ttu-id="99fc9-127">在请求正文中，提供 [managedDevice](../resources/intune-devices-manageddevice.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="99fc9-127">In the request body, supply a JSON representation for the [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>

<span data-ttu-id="99fc9-128">下表显示创建 [managedDevice](../resources/intune-devices-manageddevice.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="99fc9-128">The following table shows the properties that are required when you create the [managedDevice](../resources/intune-devices-manageddevice.md).</span></span>

|<span data-ttu-id="99fc9-129">属性</span><span class="sxs-lookup"><span data-stu-id="99fc9-129">Property</span></span>|<span data-ttu-id="99fc9-130">类型</span><span class="sxs-lookup"><span data-stu-id="99fc9-130">Type</span></span>|<span data-ttu-id="99fc9-131">说明</span><span class="sxs-lookup"><span data-stu-id="99fc9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99fc9-132">id</span><span class="sxs-lookup"><span data-stu-id="99fc9-132">id</span></span>|<span data-ttu-id="99fc9-133">字符串</span><span class="sxs-lookup"><span data-stu-id="99fc9-133">String</span></span>|<span data-ttu-id="99fc9-134">设备唯一标识符</span><span class="sxs-lookup"><span data-stu-id="99fc9-134">Unique Identifier for the device</span></span>|
|<span data-ttu-id="99fc9-135">userId</span><span class="sxs-lookup"><span data-stu-id="99fc9-135">userId</span></span>|<span data-ttu-id="99fc9-136">String</span><span class="sxs-lookup"><span data-stu-id="99fc9-136">String</span></span>|<span data-ttu-id="99fc9-137">与设备关联的用户的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="99fc9-137">Unique Identifier for the user associated with the device</span></span>|
|<span data-ttu-id="99fc9-138">deviceName</span><span class="sxs-lookup"><span data-stu-id="99fc9-138">deviceName</span></span>|<span data-ttu-id="99fc9-139">String</span><span class="sxs-lookup"><span data-stu-id="99fc9-139">String</span></span>|<span data-ttu-id="99fc9-140">设备的名称</span><span class="sxs-lookup"><span data-stu-id="99fc9-140">Name of the device</span></span>|
|<span data-ttu-id="99fc9-141">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="99fc9-141">hardwareInformation</span></span>|[<span data-ttu-id="99fc9-142">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="99fc9-142">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="99fc9-143">设备的 hardward 详细信息。</span><span class="sxs-lookup"><span data-stu-id="99fc9-143">The hardward details for the device.</span></span>  <span data-ttu-id="99fc9-144">包括存储空间、制造商、序列号等信息。</span><span class="sxs-lookup"><span data-stu-id="99fc9-144">Includes information such as storage space, manufacturer, serial number, etc.</span></span>|
|<span data-ttu-id="99fc9-145">所有者</span><span class="sxs-lookup"><span data-stu-id="99fc9-145">ownerType</span></span>|[<span data-ttu-id="99fc9-146">所有者</span><span class="sxs-lookup"><span data-stu-id="99fc9-146">ownerType</span></span>](../resources/intune-devices-ownertype.md)|<span data-ttu-id="99fc9-147">设备的所有权。</span><span class="sxs-lookup"><span data-stu-id="99fc9-147">Ownership of the device.</span></span> <span data-ttu-id="99fc9-148">可以是 "公司" 或 "个人"。</span><span class="sxs-lookup"><span data-stu-id="99fc9-148">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="99fc9-149">可取值为：`unknown`、`company`、`personal`。</span><span class="sxs-lookup"><span data-stu-id="99fc9-149">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="99fc9-150">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="99fc9-150">managedDeviceOwnerType</span></span>|[<span data-ttu-id="99fc9-151">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="99fc9-151">managedDeviceOwnerType</span></span>](../resources/intune-devices-manageddeviceownertype.md)|<span data-ttu-id="99fc9-152">设备的所有权。</span><span class="sxs-lookup"><span data-stu-id="99fc9-152">Ownership of the device.</span></span> <span data-ttu-id="99fc9-153">可以是 "公司" 或 "个人"。</span><span class="sxs-lookup"><span data-stu-id="99fc9-153">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="99fc9-154">可取值为：`unknown`、`company`、`personal`。</span><span class="sxs-lookup"><span data-stu-id="99fc9-154">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="99fc9-155">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="99fc9-155">deviceActionResults</span></span>|<span data-ttu-id="99fc9-156">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) 集合</span><span class="sxs-lookup"><span data-stu-id="99fc9-156">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="99fc9-157">ComplexType deviceActionResult 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="99fc9-157">List of ComplexType deviceActionResult objects.</span></span>|
|<span data-ttu-id="99fc9-158">managementState</span><span class="sxs-lookup"><span data-stu-id="99fc9-158">managementState</span></span>|[<span data-ttu-id="99fc9-159">managementState</span><span class="sxs-lookup"><span data-stu-id="99fc9-159">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="99fc9-160">设备的管理状态。</span><span class="sxs-lookup"><span data-stu-id="99fc9-160">Management state of the device.</span></span> <span data-ttu-id="99fc9-161">可取值为：`managed`、`retirePending`、`retireFailed`、`wipePending`、`wipeFailed`、`unhealthy`、`deletePending`、`retireIssued`、`wipeIssued`、`wipeCanceled`、`retireCanceled`、`discovered`。</span><span class="sxs-lookup"><span data-stu-id="99fc9-161">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="99fc9-162">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="99fc9-162">enrolledDateTime</span></span>|<span data-ttu-id="99fc9-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99fc9-163">DateTimeOffset</span></span>|<span data-ttu-id="99fc9-164">设备的注册时间。</span><span class="sxs-lookup"><span data-stu-id="99fc9-164">Enrollment time of the device.</span></span>|
|<span data-ttu-id="99fc9-165">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="99fc9-165">lastSyncDateTime</span></span>|<span data-ttu-id="99fc9-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99fc9-166">DateTimeOffset</span></span>|<span data-ttu-id="99fc9-167">设备上次成功完成与 Intune 同步的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="99fc9-167">The date and time that the device last completed a successful sync with Intune.</span></span>|
|<span data-ttu-id="99fc9-168">chassisType</span><span class="sxs-lookup"><span data-stu-id="99fc9-168">chassisType</span></span>|[<span data-ttu-id="99fc9-169">chassisType</span><span class="sxs-lookup"><span data-stu-id="99fc9-169">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="99fc9-170">设备的机箱类型。</span><span class="sxs-lookup"><span data-stu-id="99fc9-170">Chassis type of the device.</span></span> <span data-ttu-id="99fc9-171">可取值为：`unknown`、`desktop`、`laptop`、`worksWorkstation`、`enterpriseServer`、`phone`、`tablet`、`mobileOther`、`mobileUnknown`。</span><span class="sxs-lookup"><span data-stu-id="99fc9-171">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="99fc9-172">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="99fc9-172">operatingSystem</span></span>|<span data-ttu-id="99fc9-173">String</span><span class="sxs-lookup"><span data-stu-id="99fc9-173">String</span></span>|<span data-ttu-id="99fc9-174">设备的操作系统。</span><span class="sxs-lookup"><span data-stu-id="99fc9-174">Operating system of the device.</span></span> <span data-ttu-id="99fc9-175">Windows、iOS 等。</span><span class="sxs-lookup"><span data-stu-id="99fc9-175">Windows, iOS, etc.</span></span>|
|<span data-ttu-id="99fc9-176">deviceType</span><span class="sxs-lookup"><span data-stu-id="99fc9-176">deviceType</span></span>|[<span data-ttu-id="99fc9-177">deviceType</span><span class="sxs-lookup"><span data-stu-id="99fc9-177">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="99fc9-178">设备的平台。</span><span class="sxs-lookup"><span data-stu-id="99fc9-178">Platform of the device.</span></span> <span data-ttu-id="99fc9-179">可能的值为`desktop`: `windowsRT`、 `winMO6`、 `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer`、、、、、、、、、、、、、、、、 `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="99fc9-179">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="99fc9-180">complianceState</span><span class="sxs-lookup"><span data-stu-id="99fc9-180">complianceState</span></span>|[<span data-ttu-id="99fc9-181">complianceState</span><span class="sxs-lookup"><span data-stu-id="99fc9-181">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="99fc9-182">设备的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="99fc9-182">Compliance state of the device.</span></span> <span data-ttu-id="99fc9-183">可取值为：`unknown`、`compliant`、`noncompliant`、`conflict`、`error`、`inGracePeriod`、`configManager`。</span><span class="sxs-lookup"><span data-stu-id="99fc9-183">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="99fc9-184">jailBroken</span><span class="sxs-lookup"><span data-stu-id="99fc9-184">jailBroken</span></span>|<span data-ttu-id="99fc9-185">String</span><span class="sxs-lookup"><span data-stu-id="99fc9-185">String</span></span>|<span data-ttu-id="99fc9-186">设备是否已越狱或取得 root 权限。</span><span class="sxs-lookup"><span data-stu-id="99fc9-186">whether the device is jail broken or rooted.</span></span>|
|<span data-ttu-id="99fc9-187">managementAgent</span><span class="sxs-lookup"><span data-stu-id="99fc9-187">managementAgent</span></span>|[<span data-ttu-id="99fc9-188">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="99fc9-188">managementAgentType</span></span>](../resources/intune-devices-managementagenttype.md)|<span data-ttu-id="99fc9-189">设备的管理通道。</span><span class="sxs-lookup"><span data-stu-id="99fc9-189">Management channel of the device.</span></span> <span data-ttu-id="99fc9-190">Intune、EAS 等。可能的值为`eas`: `mdm`、 `easMdm`、 `intuneClient` `easIntuneClient` `configurationManagerClient` `configurationManagerClientMdm` `configurationManagerClientMdmEas` `unknown`、、、、、、、、 `microsoft365ManagedMdm` `jamf` `googleCloudDevicePolicyController`</span><span class="sxs-lookup"><span data-stu-id="99fc9-190">Intune, EAS, etc. Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span></span>|
|<span data-ttu-id="99fc9-191">osVersion</span><span class="sxs-lookup"><span data-stu-id="99fc9-191">osVersion</span></span>|<span data-ttu-id="99fc9-192">String</span><span class="sxs-lookup"><span data-stu-id="99fc9-192">String</span></span>|<span data-ttu-id="99fc9-193">设备的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="99fc9-193">Operating system version of the device.</span></span>|
|<span data-ttu-id="99fc9-194">easActivated</span><span class="sxs-lookup"><span data-stu-id="99fc9-194">easActivated</span></span>|<span data-ttu-id="99fc9-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="99fc9-195">Boolean</span></span>|<span data-ttu-id="99fc9-196">设备是否已激活 Exchange ActiveSync。</span><span class="sxs-lookup"><span data-stu-id="99fc9-196">Whether the device is Exchange ActiveSync activated.</span></span>|
|<span data-ttu-id="99fc9-197">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="99fc9-197">easDeviceId</span></span>|<span data-ttu-id="99fc9-198">String</span><span class="sxs-lookup"><span data-stu-id="99fc9-198">String</span></span>|<span data-ttu-id="99fc9-199">设备的 Exchange ActiveSync ID。</span><span class="sxs-lookup"><span data-stu-id="99fc9-199">Exchange ActiveSync Id of the device.</span></span>|
|<span data-ttu-id="99fc9-200">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="99fc9-200">easActivationDateTime</span></span>|<span data-ttu-id="99fc9-201">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99fc9-201">DateTimeOffset</span></span>|<span data-ttu-id="99fc9-202">设备的 Exchange ActivationSync 激活时间。</span><span class="sxs-lookup"><span data-stu-id="99fc9-202">Exchange ActivationSync activation time of the device.</span></span>|
|<span data-ttu-id="99fc9-203">aadRegistered</span><span class="sxs-lookup"><span data-stu-id="99fc9-203">aadRegistered</span></span>|<span data-ttu-id="99fc9-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="99fc9-204">Boolean</span></span>|<span data-ttu-id="99fc9-205">设备是否已注册 Azure Active Directory。</span><span class="sxs-lookup"><span data-stu-id="99fc9-205">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="99fc9-206">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="99fc9-206">azureADRegistered</span></span>|<span data-ttu-id="99fc9-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="99fc9-207">Boolean</span></span>|<span data-ttu-id="99fc9-208">设备是否已注册 Azure Active Directory。</span><span class="sxs-lookup"><span data-stu-id="99fc9-208">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="99fc9-209">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="99fc9-209">deviceEnrollmentType</span></span>|[<span data-ttu-id="99fc9-210">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="99fc9-210">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="99fc9-211">设备的注册类型。</span><span class="sxs-lookup"><span data-stu-id="99fc9-211">Enrollment type of the device.</span></span> <span data-ttu-id="99fc9-212">可取值为：`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement`。</span><span class="sxs-lookup"><span data-stu-id="99fc9-212">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="99fc9-213">lostModeState</span><span class="sxs-lookup"><span data-stu-id="99fc9-213">lostModeState</span></span>|[<span data-ttu-id="99fc9-214">lostModeState</span><span class="sxs-lookup"><span data-stu-id="99fc9-214">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="99fc9-215">指示是否已启用或禁用了丢失模式。</span><span class="sxs-lookup"><span data-stu-id="99fc9-215">Indicates if Lost mode is enabled or disabled.</span></span> <span data-ttu-id="99fc9-216">可取值为：`disabled`、`enabled`。</span><span class="sxs-lookup"><span data-stu-id="99fc9-216">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="99fc9-217">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="99fc9-217">activationLockBypassCode</span></span>|<span data-ttu-id="99fc9-218">String</span><span class="sxs-lookup"><span data-stu-id="99fc9-218">String</span></span>|<span data-ttu-id="99fc9-219">允许绕过设备上的激活锁的代码。</span><span class="sxs-lookup"><span data-stu-id="99fc9-219">Code that allows the Activation Lock on a device to be bypassed.</span></span>|
|<span data-ttu-id="99fc9-220">emailAddress</span><span class="sxs-lookup"><span data-stu-id="99fc9-220">emailAddress</span></span>|<span data-ttu-id="99fc9-221">String</span><span class="sxs-lookup"><span data-stu-id="99fc9-221">String</span></span>|<span data-ttu-id="99fc9-222">与设备关联的用户的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="99fc9-222">Email(s) for the user associated with the device</span></span>|
|<span data-ttu-id="99fc9-223">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="99fc9-223">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="99fc9-224">String</span><span class="sxs-lookup"><span data-stu-id="99fc9-224">String</span></span>|<span data-ttu-id="99fc9-225">Azure Active Directory 设备的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="99fc9-225">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="99fc9-226">只读。</span><span class="sxs-lookup"><span data-stu-id="99fc9-226">Read only.</span></span>|
|<span data-ttu-id="99fc9-227">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="99fc9-227">azureADDeviceId</span></span>|<span data-ttu-id="99fc9-228">String</span><span class="sxs-lookup"><span data-stu-id="99fc9-228">String</span></span>|<span data-ttu-id="99fc9-229">Azure Active Directory 设备的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="99fc9-229">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="99fc9-230">只读。</span><span class="sxs-lookup"><span data-stu-id="99fc9-230">Read only.</span></span>|
|<span data-ttu-id="99fc9-231">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="99fc9-231">deviceRegistrationState</span></span>|[<span data-ttu-id="99fc9-232">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="99fc9-232">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="99fc9-233">设备注册状态。</span><span class="sxs-lookup"><span data-stu-id="99fc9-233">Device registration state.</span></span> <span data-ttu-id="99fc9-234">可取值为：`notRegistered`、`registered`、`revoked`、`keyConflict`、`approvalPending`、`certificateReset`、`notRegisteredPendingEnrollment`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="99fc9-234">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="99fc9-235">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="99fc9-235">deviceCategoryDisplayName</span></span>|<span data-ttu-id="99fc9-236">String</span><span class="sxs-lookup"><span data-stu-id="99fc9-236">String</span></span>|<span data-ttu-id="99fc9-237">设备类别显示名称。</span><span class="sxs-lookup"><span data-stu-id="99fc9-237">Device category display name</span></span>|
|<span data-ttu-id="99fc9-238">isSupervised</span><span class="sxs-lookup"><span data-stu-id="99fc9-238">isSupervised</span></span>|<span data-ttu-id="99fc9-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="99fc9-239">Boolean</span></span>|<span data-ttu-id="99fc9-240">设备受监督状态</span><span class="sxs-lookup"><span data-stu-id="99fc9-240">Device supervised status</span></span>|
|<span data-ttu-id="99fc9-241">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="99fc9-241">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="99fc9-242">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99fc9-242">DateTimeOffset</span></span>|<span data-ttu-id="99fc9-243">设备上次与 Exchange 联系的时间。</span><span class="sxs-lookup"><span data-stu-id="99fc9-243">Last time the device contacted Exchange.</span></span>|
|<span data-ttu-id="99fc9-244">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="99fc9-244">exchangeAccessState</span></span>|[<span data-ttu-id="99fc9-245">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="99fc9-245">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="99fc9-246">Exchange 中设备的访问状态。</span><span class="sxs-lookup"><span data-stu-id="99fc9-246">The Access State of the device in Exchange.</span></span> <span data-ttu-id="99fc9-247">可取值为：`none`、`unknown`、`allowed`、`blocked`、`quarantined`。</span><span class="sxs-lookup"><span data-stu-id="99fc9-247">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="99fc9-248">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="99fc9-248">exchangeAccessStateReason</span></span>|[<span data-ttu-id="99fc9-249">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="99fc9-249">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="99fc9-250">Exchange 中设备访问状态的出现原因。</span><span class="sxs-lookup"><span data-stu-id="99fc9-250">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="99fc9-251">可取值为：`none`、`unknown`、`exchangeGlobalRule`、`exchangeIndividualRule`、`exchangeDeviceRule`、`exchangeUpgrade`、`exchangeMailboxPolicy`、`other`、`compliant`、`notCompliant`、`notEnrolled`、`unknownLocation`、`mfaRequired`、`azureADBlockDueToAccessPolicy`、`compromisedPassword`、`deviceNotKnownWithManagedApp`。</span><span class="sxs-lookup"><span data-stu-id="99fc9-251">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="99fc9-252">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="99fc9-252">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="99fc9-253">String</span><span class="sxs-lookup"><span data-stu-id="99fc9-253">String</span></span>|<span data-ttu-id="99fc9-254">允许与设备建立远程协助会话的 URL。</span><span class="sxs-lookup"><span data-stu-id="99fc9-254">Url that allows a Remote Assistance session to be established with the device.</span></span>|
|<span data-ttu-id="99fc9-255">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="99fc9-255">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="99fc9-256">String</span><span class="sxs-lookup"><span data-stu-id="99fc9-256">String</span></span>|<span data-ttu-id="99fc9-257">用于在创建远程协助会话对象时识别问题的错误字符串。</span><span class="sxs-lookup"><span data-stu-id="99fc9-257">An error string that identifies issues when creating Remote Assistance session objects.</span></span>|
|<span data-ttu-id="99fc9-258">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="99fc9-258">isEncrypted</span></span>|<span data-ttu-id="99fc9-259">Boolean</span><span class="sxs-lookup"><span data-stu-id="99fc9-259">Boolean</span></span>|<span data-ttu-id="99fc9-260">设备加密状态</span><span class="sxs-lookup"><span data-stu-id="99fc9-260">Device encryption status</span></span>|
|<span data-ttu-id="99fc9-261">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="99fc9-261">userPrincipalName</span></span>|<span data-ttu-id="99fc9-262">String</span><span class="sxs-lookup"><span data-stu-id="99fc9-262">String</span></span>|<span data-ttu-id="99fc9-263">设备用户主体名称</span><span class="sxs-lookup"><span data-stu-id="99fc9-263">Device user principal name</span></span>|
|<span data-ttu-id="99fc9-264">model</span><span class="sxs-lookup"><span data-stu-id="99fc9-264">model</span></span>|<span data-ttu-id="99fc9-265">String</span><span class="sxs-lookup"><span data-stu-id="99fc9-265">String</span></span>|<span data-ttu-id="99fc9-266">设备的型号</span><span class="sxs-lookup"><span data-stu-id="99fc9-266">Model of the device</span></span>|
|<span data-ttu-id="99fc9-267">manufacturer</span><span class="sxs-lookup"><span data-stu-id="99fc9-267">manufacturer</span></span>|<span data-ttu-id="99fc9-268">String</span><span class="sxs-lookup"><span data-stu-id="99fc9-268">String</span></span>|<span data-ttu-id="99fc9-269">设备的制造商</span><span class="sxs-lookup"><span data-stu-id="99fc9-269">Manufacturer of the device</span></span>|
|<span data-ttu-id="99fc9-270">imei</span><span class="sxs-lookup"><span data-stu-id="99fc9-270">imei</span></span>|<span data-ttu-id="99fc9-271">String</span><span class="sxs-lookup"><span data-stu-id="99fc9-271">String</span></span>|<span data-ttu-id="99fc9-272">IMEI</span><span class="sxs-lookup"><span data-stu-id="99fc9-272">IMEI</span></span>|
|<span data-ttu-id="99fc9-273">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="99fc9-273">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="99fc9-274">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99fc9-274">DateTimeOffset</span></span>|<span data-ttu-id="99fc9-275">设备符合性宽限期的到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="99fc9-275">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="99fc9-276">serialNumber</span><span class="sxs-lookup"><span data-stu-id="99fc9-276">serialNumber</span></span>|<span data-ttu-id="99fc9-277">字符串</span><span class="sxs-lookup"><span data-stu-id="99fc9-277">String</span></span>|<span data-ttu-id="99fc9-278">序列号</span><span class="sxs-lookup"><span data-stu-id="99fc9-278">SerialNumber</span></span>|
|<span data-ttu-id="99fc9-279">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="99fc9-279">phoneNumber</span></span>|<span data-ttu-id="99fc9-280">String</span><span class="sxs-lookup"><span data-stu-id="99fc9-280">String</span></span>|<span data-ttu-id="99fc9-281">设备的电话号码</span><span class="sxs-lookup"><span data-stu-id="99fc9-281">Phone number of the device</span></span>|
|<span data-ttu-id="99fc9-282">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="99fc9-282">androidSecurityPatchLevel</span></span>|<span data-ttu-id="99fc9-283">String</span><span class="sxs-lookup"><span data-stu-id="99fc9-283">String</span></span>|<span data-ttu-id="99fc9-284">Android 安全修补程序级别</span><span class="sxs-lookup"><span data-stu-id="99fc9-284">Android security patch level</span></span>|
|<span data-ttu-id="99fc9-285">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="99fc9-285">userDisplayName</span></span>|<span data-ttu-id="99fc9-286">String</span><span class="sxs-lookup"><span data-stu-id="99fc9-286">String</span></span>|<span data-ttu-id="99fc9-287">用户显示名称</span><span class="sxs-lookup"><span data-stu-id="99fc9-287">User display name</span></span>|
|<span data-ttu-id="99fc9-288">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="99fc9-288">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="99fc9-289">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="99fc9-289">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="99fc9-290">ConfigrMgr 客户端启用的功能</span><span class="sxs-lookup"><span data-stu-id="99fc9-290">ConfigrMgr client enabled features</span></span>|
|<span data-ttu-id="99fc9-291">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="99fc9-291">wiFiMacAddress</span></span>|<span data-ttu-id="99fc9-292">String</span><span class="sxs-lookup"><span data-stu-id="99fc9-292">String</span></span>|<span data-ttu-id="99fc9-293">Wi-Fi MAC</span><span class="sxs-lookup"><span data-stu-id="99fc9-293">Wi-Fi MAC</span></span>|
|<span data-ttu-id="99fc9-294">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="99fc9-294">deviceHealthAttestationState</span></span>|[<span data-ttu-id="99fc9-295">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="99fc9-295">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="99fc9-296">设备运行状况证明状态。</span><span class="sxs-lookup"><span data-stu-id="99fc9-296">The device health attestation state.</span></span>|
|<span data-ttu-id="99fc9-297">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="99fc9-297">subscriberCarrier</span></span>|<span data-ttu-id="99fc9-298">String</span><span class="sxs-lookup"><span data-stu-id="99fc9-298">String</span></span>|<span data-ttu-id="99fc9-299">订阅者运营商</span><span class="sxs-lookup"><span data-stu-id="99fc9-299">Subscriber Carrier</span></span>|
|<span data-ttu-id="99fc9-300">meid</span><span class="sxs-lookup"><span data-stu-id="99fc9-300">meid</span></span>|<span data-ttu-id="99fc9-301">String</span><span class="sxs-lookup"><span data-stu-id="99fc9-301">String</span></span>|<span data-ttu-id="99fc9-302">MEID</span><span class="sxs-lookup"><span data-stu-id="99fc9-302">MEID</span></span>|
|<span data-ttu-id="99fc9-303">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="99fc9-303">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="99fc9-304">Int64</span><span class="sxs-lookup"><span data-stu-id="99fc9-304">Int64</span></span>|<span data-ttu-id="99fc9-305">存储空间总字节数</span><span class="sxs-lookup"><span data-stu-id="99fc9-305">Total Storage in Bytes</span></span>|
|<span data-ttu-id="99fc9-306">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="99fc9-306">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="99fc9-307">Int64</span><span class="sxs-lookup"><span data-stu-id="99fc9-307">Int64</span></span>|<span data-ttu-id="99fc9-308">可用存储空间字节数</span><span class="sxs-lookup"><span data-stu-id="99fc9-308">Free Storage in Bytes</span></span>|
|<span data-ttu-id="99fc9-309">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="99fc9-309">managedDeviceName</span></span>|<span data-ttu-id="99fc9-310">String</span><span class="sxs-lookup"><span data-stu-id="99fc9-310">String</span></span>|<span data-ttu-id="99fc9-311">用于识别设备的自动生成的名称。</span><span class="sxs-lookup"><span data-stu-id="99fc9-311">Automatically generated name to identify a device.</span></span> <span data-ttu-id="99fc9-312">可以覆盖为用户友好名称。</span><span class="sxs-lookup"><span data-stu-id="99fc9-312">Can be overwritten to a user friendly name.</span></span>|
|<span data-ttu-id="99fc9-313">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="99fc9-313">partnerReportedThreatState</span></span>|[<span data-ttu-id="99fc9-314">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="99fc9-314">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="99fc9-315">指示帐户和设备正在使用移动威胁防护合作伙伴时设备的威胁状态。</span><span class="sxs-lookup"><span data-stu-id="99fc9-315">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="99fc9-316">只读。</span><span class="sxs-lookup"><span data-stu-id="99fc9-316">Read Only.</span></span> <span data-ttu-id="99fc9-317">可取值为：`unknown`、`activated`、`deactivated`、`secured`、`lowSeverity`、`mediumSeverity`、`highSeverity`、`unresponsive`、`compromised`、`misconfigured`。</span><span class="sxs-lookup"><span data-stu-id="99fc9-317">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="99fc9-318">usersLoggedOn</span><span class="sxs-lookup"><span data-stu-id="99fc9-318">usersLoggedOn</span></span>|<span data-ttu-id="99fc9-319">[loggedOnUser](../resources/intune-devices-loggedonuser.md)集合</span><span class="sxs-lookup"><span data-stu-id="99fc9-319">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="99fc9-320">指示设备的上次登录用户</span><span class="sxs-lookup"><span data-stu-id="99fc9-320">Indicates the last logged on users of a device</span></span>|
|<span data-ttu-id="99fc9-321">preferMdmOverGroupPolicyAppliedDateTime</span><span class="sxs-lookup"><span data-stu-id="99fc9-321">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="99fc9-322">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99fc9-322">DateTimeOffset</span></span>|<span data-ttu-id="99fc9-323">报告设置了 preferMdmOverGroupPolicy 设置的 DateTime。</span><span class="sxs-lookup"><span data-stu-id="99fc9-323">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="99fc9-324">设置后, 如果存在冲突, Intune MDM 设置将覆盖组策略设置。</span><span class="sxs-lookup"><span data-stu-id="99fc9-324">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="99fc9-325">只读。</span><span class="sxs-lookup"><span data-stu-id="99fc9-325">Read Only.</span></span>|
|<span data-ttu-id="99fc9-326">autopilotEnrolled</span><span class="sxs-lookup"><span data-stu-id="99fc9-326">autopilotEnrolled</span></span>|<span data-ttu-id="99fc9-327">Boolean</span><span class="sxs-lookup"><span data-stu-id="99fc9-327">Boolean</span></span>|<span data-ttu-id="99fc9-328">如果托管设备是通过自动引导注册的, 则报告。</span><span class="sxs-lookup"><span data-stu-id="99fc9-328">Reports if the managed device is enrolled via auto-pilot.</span></span>|
|<span data-ttu-id="99fc9-329">requireUserEnrollmentApproval</span><span class="sxs-lookup"><span data-stu-id="99fc9-329">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="99fc9-330">Boolean</span><span class="sxs-lookup"><span data-stu-id="99fc9-330">Boolean</span></span>|<span data-ttu-id="99fc9-331">如果托管 iOS 设备是用户审批注册, 则报告。</span><span class="sxs-lookup"><span data-stu-id="99fc9-331">Reports if the managed iOS device is user approval enrollment.</span></span>|
|<span data-ttu-id="99fc9-332">managementCertificateExpirationDate</span><span class="sxs-lookup"><span data-stu-id="99fc9-332">managementCertificateExpirationDate</span></span>|<span data-ttu-id="99fc9-333">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99fc9-333">DateTimeOffset</span></span>|<span data-ttu-id="99fc9-334">报告设备管理证书到期日期</span><span class="sxs-lookup"><span data-stu-id="99fc9-334">Reports device management certificate expiration date</span></span>|
|<span data-ttu-id="99fc9-335">iccid</span><span class="sxs-lookup"><span data-stu-id="99fc9-335">iccid</span></span>|<span data-ttu-id="99fc9-336">String</span><span class="sxs-lookup"><span data-stu-id="99fc9-336">String</span></span>|<span data-ttu-id="99fc9-337">集成的电路卡标识符, 它是 SIM 卡的唯一标识号。</span><span class="sxs-lookup"><span data-stu-id="99fc9-337">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span>|
|<span data-ttu-id="99fc9-338">udid</span><span class="sxs-lookup"><span data-stu-id="99fc9-338">udid</span></span>|<span data-ttu-id="99fc9-339">String</span><span class="sxs-lookup"><span data-stu-id="99fc9-339">String</span></span>|<span data-ttu-id="99fc9-340">iOS 和 macOS 设备的唯一设备标识符。</span><span class="sxs-lookup"><span data-stu-id="99fc9-340">Unique Device Identifier for iOS and macOS devices.</span></span>|
|<span data-ttu-id="99fc9-341">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="99fc9-341">roleScopeTagIds</span></span>|<span data-ttu-id="99fc9-342">String collection</span><span class="sxs-lookup"><span data-stu-id="99fc9-342">String collection</span></span>|<span data-ttu-id="99fc9-343">此设备实例的范围标记 id 的列表。</span><span class="sxs-lookup"><span data-stu-id="99fc9-343">List of Scope Tag IDs for this Device instance.</span></span>|
|<span data-ttu-id="99fc9-344">windowsActiveMalwareCount</span><span class="sxs-lookup"><span data-stu-id="99fc9-344">windowsActiveMalwareCount</span></span>|<span data-ttu-id="99fc9-345">Int32</span><span class="sxs-lookup"><span data-stu-id="99fc9-345">Int32</span></span>|<span data-ttu-id="99fc9-346">此 windows 设备的活动恶意软件计数</span><span class="sxs-lookup"><span data-stu-id="99fc9-346">Count of active malware for this windows device</span></span>|
|<span data-ttu-id="99fc9-347">windowsRemediatedMalwareCount</span><span class="sxs-lookup"><span data-stu-id="99fc9-347">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="99fc9-348">Int32</span><span class="sxs-lookup"><span data-stu-id="99fc9-348">Int32</span></span>|<span data-ttu-id="99fc9-349">此 windows 设备的修正的恶意软件计数</span><span class="sxs-lookup"><span data-stu-id="99fc9-349">Count of remediated malware for this windows device</span></span>|
|<span data-ttu-id="99fc9-350">notes</span><span class="sxs-lookup"><span data-stu-id="99fc9-350">notes</span></span>|<span data-ttu-id="99fc9-351">String</span><span class="sxs-lookup"><span data-stu-id="99fc9-351">String</span></span>|<span data-ttu-id="99fc9-352">IT 管理员创建的设备上的注释</span><span class="sxs-lookup"><span data-stu-id="99fc9-352">Notes on the device created by IT Admin</span></span>|
|<span data-ttu-id="99fc9-353">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="99fc9-353">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="99fc9-354">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="99fc9-354">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="99fc9-355">Configuration manager 客户端运行状况状态, 仅对由 MDM/ConfigMgr 代理管理的设备有效</span><span class="sxs-lookup"><span data-stu-id="99fc9-355">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent</span></span>|



## <a name="response"></a><span data-ttu-id="99fc9-356">响应</span><span class="sxs-lookup"><span data-stu-id="99fc9-356">Response</span></span>
<span data-ttu-id="99fc9-357">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [managedDevice](../resources/intune-devices-manageddevice.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="99fc9-357">If successful, this method returns a `200 OK` response code and an updated [managedDevice](../resources/intune-devices-manageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="99fc9-358">示例</span><span class="sxs-lookup"><span data-stu-id="99fc9-358">Example</span></span>

### <a name="request"></a><span data-ttu-id="99fc9-359">请求</span><span class="sxs-lookup"><span data-stu-id="99fc9-359">Request</span></span>
<span data-ttu-id="99fc9-360">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="99fc9-360">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/users/{usersId}/managedDevices/{managedDeviceId}
Content-type: application/json
Content-length: 7224

{
  "@odata.type": "#microsoft.graph.managedDevice",
  "userId": "User Id value",
  "deviceName": "Device Name value",
  "hardwareInformation": {
    "@odata.type": "microsoft.graph.hardwareInformation",
    "serialNumber": "Serial Number value",
    "totalStorageSpace": 1,
    "freeStorageSpace": 0,
    "imei": "Imei value",
    "meid": "Meid value",
    "manufacturer": "Manufacturer value",
    "model": "Model value",
    "phoneNumber": "Phone Number value",
    "subscriberCarrier": "Subscriber Carrier value",
    "cellularTechnology": "Cellular Technology value",
    "wifiMac": "Wifi Mac value",
    "operatingSystemLanguage": "Operating System Language value",
    "isSupervised": true,
    "isEncrypted": true,
    "isSharedDevice": true,
    "sharedDeviceCachedUsers": [
      {
        "@odata.type": "microsoft.graph.sharedAppleDeviceUser",
        "userPrincipalName": "User Principal Name value",
        "dataToSync": true,
        "dataQuota": 9,
        "dataUsed": 8
      }
    ],
    "tpmSpecificationVersion": "Tpm Specification Version value",
    "operatingSystemEdition": "Operating System Edition value",
    "deviceFullQualifiedDomainName": "Device Full Qualified Domain Name value",
    "deviceGuardVirtualizationBasedSecurityHardwareRequirementState": "secureBootRequired",
    "deviceGuardVirtualizationBasedSecurityState": "rebootRequired",
    "deviceGuardLocalSystemAuthorityCredentialGuardState": "rebootRequired"
  },
  "ownerType": "company",
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
  "managementState": "retirePending",
  "enrolledDateTime": "2016-12-31T23:59:43.797191-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "chassisType": "desktop",
  "operatingSystem": "Operating System value",
  "deviceType": "windowsRT",
  "complianceState": "compliant",
  "jailBroken": "Jail Broken value",
  "managementAgent": "mdm",
  "osVersion": "Os Version value",
  "easActivated": true,
  "easDeviceId": "Eas Device Id value",
  "easActivationDateTime": "2016-12-31T23:59:43.4878784-08:00",
  "aadRegistered": true,
  "azureADRegistered": true,
  "deviceEnrollmentType": "userEnrollment",
  "lostModeState": "enabled",
  "activationLockBypassCode": "Activation Lock Bypass Code value",
  "emailAddress": "Email Address value",
  "azureActiveDirectoryDeviceId": "Azure Active Directory Device Id value",
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
    "windowsUpdateForBusiness": true,
    "endpointProtection": true,
    "officeApps": true
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
  "usersLoggedOn": [
    {
      "@odata.type": "microsoft.graph.loggedOnUser",
      "userId": "User Id value",
      "lastLogOnDateTime": "2016-12-31T23:58:37.4262708-08:00"
    }
  ],
  "preferMdmOverGroupPolicyAppliedDateTime": "2016-12-31T23:57:34.4649887-08:00",
  "autopilotEnrolled": true,
  "requireUserEnrollmentApproval": true,
  "managementCertificateExpirationDate": "2016-12-31T23:57:59.9789653-08:00",
  "iccid": "Iccid value",
  "udid": "Udid value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "windowsActiveMalwareCount": 9,
  "windowsRemediatedMalwareCount": 13,
  "notes": "Notes value",
  "configurationManagerClientHealthState": {
    "@odata.type": "microsoft.graph.configurationManagerClientHealthState",
    "state": "installed",
    "errorCode": 9,
    "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00"
  }
}
```

### <a name="response"></a><span data-ttu-id="99fc9-361">响应</span><span class="sxs-lookup"><span data-stu-id="99fc9-361">Response</span></span>
<span data-ttu-id="99fc9-p121">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="99fc9-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 7273

{
  "@odata.type": "#microsoft.graph.managedDevice",
  "id": "705c034c-034c-705c-4c03-5c704c035c70",
  "userId": "User Id value",
  "deviceName": "Device Name value",
  "hardwareInformation": {
    "@odata.type": "microsoft.graph.hardwareInformation",
    "serialNumber": "Serial Number value",
    "totalStorageSpace": 1,
    "freeStorageSpace": 0,
    "imei": "Imei value",
    "meid": "Meid value",
    "manufacturer": "Manufacturer value",
    "model": "Model value",
    "phoneNumber": "Phone Number value",
    "subscriberCarrier": "Subscriber Carrier value",
    "cellularTechnology": "Cellular Technology value",
    "wifiMac": "Wifi Mac value",
    "operatingSystemLanguage": "Operating System Language value",
    "isSupervised": true,
    "isEncrypted": true,
    "isSharedDevice": true,
    "sharedDeviceCachedUsers": [
      {
        "@odata.type": "microsoft.graph.sharedAppleDeviceUser",
        "userPrincipalName": "User Principal Name value",
        "dataToSync": true,
        "dataQuota": 9,
        "dataUsed": 8
      }
    ],
    "tpmSpecificationVersion": "Tpm Specification Version value",
    "operatingSystemEdition": "Operating System Edition value",
    "deviceFullQualifiedDomainName": "Device Full Qualified Domain Name value",
    "deviceGuardVirtualizationBasedSecurityHardwareRequirementState": "secureBootRequired",
    "deviceGuardVirtualizationBasedSecurityState": "rebootRequired",
    "deviceGuardLocalSystemAuthorityCredentialGuardState": "rebootRequired"
  },
  "ownerType": "company",
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
  "managementState": "retirePending",
  "enrolledDateTime": "2016-12-31T23:59:43.797191-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "chassisType": "desktop",
  "operatingSystem": "Operating System value",
  "deviceType": "windowsRT",
  "complianceState": "compliant",
  "jailBroken": "Jail Broken value",
  "managementAgent": "mdm",
  "osVersion": "Os Version value",
  "easActivated": true,
  "easDeviceId": "Eas Device Id value",
  "easActivationDateTime": "2016-12-31T23:59:43.4878784-08:00",
  "aadRegistered": true,
  "azureADRegistered": true,
  "deviceEnrollmentType": "userEnrollment",
  "lostModeState": "enabled",
  "activationLockBypassCode": "Activation Lock Bypass Code value",
  "emailAddress": "Email Address value",
  "azureActiveDirectoryDeviceId": "Azure Active Directory Device Id value",
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
    "windowsUpdateForBusiness": true,
    "endpointProtection": true,
    "officeApps": true
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
  "usersLoggedOn": [
    {
      "@odata.type": "microsoft.graph.loggedOnUser",
      "userId": "User Id value",
      "lastLogOnDateTime": "2016-12-31T23:58:37.4262708-08:00"
    }
  ],
  "preferMdmOverGroupPolicyAppliedDateTime": "2016-12-31T23:57:34.4649887-08:00",
  "autopilotEnrolled": true,
  "requireUserEnrollmentApproval": true,
  "managementCertificateExpirationDate": "2016-12-31T23:57:59.9789653-08:00",
  "iccid": "Iccid value",
  "udid": "Udid value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "windowsActiveMalwareCount": 9,
  "windowsRemediatedMalwareCount": 13,
  "notes": "Notes value",
  "configurationManagerClientHealthState": {
    "@odata.type": "microsoft.graph.configurationManagerClientHealthState",
    "state": "installed",
    "errorCode": 9,
    "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00"
  }
}
```




