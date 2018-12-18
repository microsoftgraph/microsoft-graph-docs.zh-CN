---
title: 更新 managedDevice
description: 更新 managedDevice 对象的属性。
author: tfitzmac
ms.openlocfilehash: 9f608f13f7580e76d1e1934d5aea788a2ce6738f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27357825"
---
# <a name="update-manageddevice"></a><span data-ttu-id="d928a-103">更新 managedDevice</span><span class="sxs-lookup"><span data-stu-id="d928a-103">Update managedDevice</span></span>

> <span data-ttu-id="d928a-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d928a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d928a-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d928a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d928a-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d928a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d928a-107">更新 [managedDevice](../resources/intune-devices-manageddevice.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d928a-107">Update the properties of a [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d928a-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="d928a-108">Prerequisites</span></span>
<span data-ttu-id="d928a-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="d928a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d928a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d928a-111">Permission type</span></span>|<span data-ttu-id="d928a-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d928a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d928a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d928a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d928a-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d928a-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="d928a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d928a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d928a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d928a-116">Not supported.</span></span>|
|<span data-ttu-id="d928a-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d928a-117">Application</span></span>|<span data-ttu-id="d928a-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="d928a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d928a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d928a-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="d928a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d928a-120">Request headers</span></span>
|<span data-ttu-id="d928a-121">标头</span><span class="sxs-lookup"><span data-stu-id="d928a-121">Header</span></span>|<span data-ttu-id="d928a-122">值</span><span class="sxs-lookup"><span data-stu-id="d928a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d928a-123">授权</span><span class="sxs-lookup"><span data-stu-id="d928a-123">Authorization</span></span>|<span data-ttu-id="d928a-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d928a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d928a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d928a-125">Accept</span></span>|<span data-ttu-id="d928a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d928a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d928a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d928a-127">Request body</span></span>
<span data-ttu-id="d928a-128">在请求正文中，提供 [managedDevice](../resources/intune-devices-manageddevice.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d928a-128">In the request body, supply a JSON representation for the [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>

<span data-ttu-id="d928a-129">下表显示创建 [managedDevice](../resources/intune-devices-manageddevice.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d928a-129">The following table shows the properties that are required when you create the [managedDevice](../resources/intune-devices-manageddevice.md).</span></span>

|<span data-ttu-id="d928a-130">属性</span><span class="sxs-lookup"><span data-stu-id="d928a-130">Property</span></span>|<span data-ttu-id="d928a-131">类型</span><span class="sxs-lookup"><span data-stu-id="d928a-131">Type</span></span>|<span data-ttu-id="d928a-132">说明</span><span class="sxs-lookup"><span data-stu-id="d928a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d928a-133">id</span><span class="sxs-lookup"><span data-stu-id="d928a-133">id</span></span>|<span data-ttu-id="d928a-134">String</span><span class="sxs-lookup"><span data-stu-id="d928a-134">String</span></span>|<span data-ttu-id="d928a-135">设备唯一标识符</span><span class="sxs-lookup"><span data-stu-id="d928a-135">Unique Identifier for the device</span></span>|
|<span data-ttu-id="d928a-136">userId</span><span class="sxs-lookup"><span data-stu-id="d928a-136">userId</span></span>|<span data-ttu-id="d928a-137">String</span><span class="sxs-lookup"><span data-stu-id="d928a-137">String</span></span>|<span data-ttu-id="d928a-138">与设备关联的用户的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="d928a-138">Unique Identifier for the user associated with the device</span></span>|
|<span data-ttu-id="d928a-139">deviceName</span><span class="sxs-lookup"><span data-stu-id="d928a-139">deviceName</span></span>|<span data-ttu-id="d928a-140">String</span><span class="sxs-lookup"><span data-stu-id="d928a-140">String</span></span>|<span data-ttu-id="d928a-141">设备的名称</span><span class="sxs-lookup"><span data-stu-id="d928a-141">Name of the device</span></span>|
|<span data-ttu-id="d928a-142">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="d928a-142">hardwareInformation</span></span>|[<span data-ttu-id="d928a-143">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="d928a-143">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="d928a-144">设备 hardward 详细信息。</span><span class="sxs-lookup"><span data-stu-id="d928a-144">The hardward details for the device.</span></span>  <span data-ttu-id="d928a-145">包含信息，如存储空间、 制造商、 序列号等。</span><span class="sxs-lookup"><span data-stu-id="d928a-145">Includes information such as storage space, manufacturer, serial number, etc.</span></span>|
|<span data-ttu-id="d928a-146">所有者类型</span><span class="sxs-lookup"><span data-stu-id="d928a-146">ownerType</span></span>|[<span data-ttu-id="d928a-147">所有者类型</span><span class="sxs-lookup"><span data-stu-id="d928a-147">ownerType</span></span>](../resources/intune-devices-ownertype.md)|<span data-ttu-id="d928a-148">设备的所有权。</span><span class="sxs-lookup"><span data-stu-id="d928a-148">Ownership of the device.</span></span> <span data-ttu-id="d928a-149">可以是公司或个人。</span><span class="sxs-lookup"><span data-stu-id="d928a-149">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="d928a-150">可取值为：`unknown`、`company`、`personal`。</span><span class="sxs-lookup"><span data-stu-id="d928a-150">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="d928a-151">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="d928a-151">managedDeviceOwnerType</span></span>|[<span data-ttu-id="d928a-152">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="d928a-152">managedDeviceOwnerType</span></span>](../resources/intune-devices-manageddeviceownertype.md)|<span data-ttu-id="d928a-153">设备的所有权。</span><span class="sxs-lookup"><span data-stu-id="d928a-153">Ownership of the device.</span></span> <span data-ttu-id="d928a-154">可以是公司或个人。</span><span class="sxs-lookup"><span data-stu-id="d928a-154">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="d928a-155">可取值为：`unknown`、`company`、`personal`。</span><span class="sxs-lookup"><span data-stu-id="d928a-155">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="d928a-156">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="d928a-156">deviceActionResults</span></span>|<span data-ttu-id="d928a-157">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d928a-157">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="d928a-158">ComplexType deviceActionResult 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="d928a-158">List of ComplexType deviceActionResult objects.</span></span>|
|<span data-ttu-id="d928a-159">管理</span><span class="sxs-lookup"><span data-stu-id="d928a-159">managementState</span></span>|[<span data-ttu-id="d928a-160">管理</span><span class="sxs-lookup"><span data-stu-id="d928a-160">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="d928a-161">管理设备的状态。</span><span class="sxs-lookup"><span data-stu-id="d928a-161">Management state of the device.</span></span> <span data-ttu-id="d928a-162">可取值为：`managed`、`retirePending`、`retireFailed`、`wipePending`、`wipeFailed`、`unhealthy`、`deletePending`、`retireIssued`、`wipeIssued`、`wipeCanceled`、`retireCanceled`、`discovered`。</span><span class="sxs-lookup"><span data-stu-id="d928a-162">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="d928a-163">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="d928a-163">enrolledDateTime</span></span>|<span data-ttu-id="d928a-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d928a-164">DateTimeOffset</span></span>|<span data-ttu-id="d928a-165">设备的注册时间。</span><span class="sxs-lookup"><span data-stu-id="d928a-165">Enrollment time of the device.</span></span>|
|<span data-ttu-id="d928a-166">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="d928a-166">lastSyncDateTime</span></span>|<span data-ttu-id="d928a-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d928a-167">DateTimeOffset</span></span>|<span data-ttu-id="d928a-168">设备上次成功完成与 Intune 同步的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="d928a-168">The date and time that the device last completed a successful sync with Intune.</span></span>|
|<span data-ttu-id="d928a-169">chassisType</span><span class="sxs-lookup"><span data-stu-id="d928a-169">chassisType</span></span>|[<span data-ttu-id="d928a-170">chassisType</span><span class="sxs-lookup"><span data-stu-id="d928a-170">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="d928a-171">机箱设备的类型。</span><span class="sxs-lookup"><span data-stu-id="d928a-171">Chassis type of the device.</span></span> <span data-ttu-id="d928a-172">可取值为：`unknown`、`desktop`、`laptop`、`worksWorkstation`、`enterpriseServer`、`phone`、`tablet`、`mobileOther`、`mobileUnknown`。</span><span class="sxs-lookup"><span data-stu-id="d928a-172">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="d928a-173">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="d928a-173">operatingSystem</span></span>|<span data-ttu-id="d928a-174">String</span><span class="sxs-lookup"><span data-stu-id="d928a-174">String</span></span>|<span data-ttu-id="d928a-175">设备的操作系统。</span><span class="sxs-lookup"><span data-stu-id="d928a-175">Operating system of the device.</span></span> <span data-ttu-id="d928a-176">Windows、iOS 等。</span><span class="sxs-lookup"><span data-stu-id="d928a-176">Windows, iOS, etc.</span></span>|
|<span data-ttu-id="d928a-177">deviceType</span><span class="sxs-lookup"><span data-stu-id="d928a-177">deviceType</span></span>|[<span data-ttu-id="d928a-178">deviceType</span><span class="sxs-lookup"><span data-stu-id="d928a-178">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="d928a-179">设备的平台。</span><span class="sxs-lookup"><span data-stu-id="d928a-179">Platform of the device.</span></span> <span data-ttu-id="d928a-180">可能的值为： `desktop`， `windowsRT`， `winMO6`， `nokia`， `windowsPhone`， `mac`， `winCE`， `winEmbedded`， `iPhone`， `iPad`， `iPod`， `android`， `iSocConsumer`， `unix`， `macMDM`， `holoLens`， `surfaceHub`， `androidForWork`， `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="d928a-180">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="d928a-181">complianceState</span><span class="sxs-lookup"><span data-stu-id="d928a-181">complianceState</span></span>|[<span data-ttu-id="d928a-182">complianceState</span><span class="sxs-lookup"><span data-stu-id="d928a-182">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="d928a-183">设备的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="d928a-183">Compliance state of the device.</span></span> <span data-ttu-id="d928a-184">可取值为：`unknown`、`compliant`、`noncompliant`、`conflict`、`error`、`inGracePeriod`、`configManager`。</span><span class="sxs-lookup"><span data-stu-id="d928a-184">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="d928a-185">jailBroken</span><span class="sxs-lookup"><span data-stu-id="d928a-185">jailBroken</span></span>|<span data-ttu-id="d928a-186">String</span><span class="sxs-lookup"><span data-stu-id="d928a-186">String</span></span>|<span data-ttu-id="d928a-187">设备是否已越狱或取得 root 权限。</span><span class="sxs-lookup"><span data-stu-id="d928a-187">whether the device is jail broken or rooted.</span></span>|
|<span data-ttu-id="d928a-188">managementAgent</span><span class="sxs-lookup"><span data-stu-id="d928a-188">managementAgent</span></span>|[<span data-ttu-id="d928a-189">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="d928a-189">managementAgentType</span></span>](../resources/intune-devices-managementagenttype.md)|<span data-ttu-id="d928a-190">设备的管理通道。</span><span class="sxs-lookup"><span data-stu-id="d928a-190">Management channel of the device.</span></span> <span data-ttu-id="d928a-191">Intune、 EAS 等。可能的值为： `eas`， `mdm`， `easMdm`， `intuneClient`， `easIntuneClient`， `configurationManagerClient`， `configurationManagerClientMdm`， `configurationManagerClientMdmEas`， `unknown`， `jamf`， `googleCloudDevicePolicyController`， `microsoft365ManagedMdm`。</span><span class="sxs-lookup"><span data-stu-id="d928a-191">Intune, EAS, etc. Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span></span>|
|<span data-ttu-id="d928a-192">osVersion</span><span class="sxs-lookup"><span data-stu-id="d928a-192">osVersion</span></span>|<span data-ttu-id="d928a-193">String</span><span class="sxs-lookup"><span data-stu-id="d928a-193">String</span></span>|<span data-ttu-id="d928a-194">设备的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="d928a-194">Operating system version of the device.</span></span>|
|<span data-ttu-id="d928a-195">easActivated</span><span class="sxs-lookup"><span data-stu-id="d928a-195">easActivated</span></span>|<span data-ttu-id="d928a-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="d928a-196">Boolean</span></span>|<span data-ttu-id="d928a-197">设备是否已激活 Exchange ActiveSync。</span><span class="sxs-lookup"><span data-stu-id="d928a-197">Whether the device is Exchange ActiveSync activated.</span></span>|
|<span data-ttu-id="d928a-198">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="d928a-198">easDeviceId</span></span>|<span data-ttu-id="d928a-199">String</span><span class="sxs-lookup"><span data-stu-id="d928a-199">String</span></span>|<span data-ttu-id="d928a-200">设备的 Exchange ActiveSync ID。</span><span class="sxs-lookup"><span data-stu-id="d928a-200">Exchange ActiveSync Id of the device.</span></span>|
|<span data-ttu-id="d928a-201">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="d928a-201">easActivationDateTime</span></span>|<span data-ttu-id="d928a-202">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d928a-202">DateTimeOffset</span></span>|<span data-ttu-id="d928a-203">设备的 Exchange ActivationSync 激活时间。</span><span class="sxs-lookup"><span data-stu-id="d928a-203">Exchange ActivationSync activation time of the device.</span></span>|
|<span data-ttu-id="d928a-204">aadRegistered</span><span class="sxs-lookup"><span data-stu-id="d928a-204">aadRegistered</span></span>|<span data-ttu-id="d928a-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="d928a-205">Boolean</span></span>|<span data-ttu-id="d928a-206">设备是否已注册 Azure Active Directory。</span><span class="sxs-lookup"><span data-stu-id="d928a-206">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="d928a-207">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="d928a-207">azureADRegistered</span></span>|<span data-ttu-id="d928a-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="d928a-208">Boolean</span></span>|<span data-ttu-id="d928a-209">设备是否已注册 Azure Active Directory。</span><span class="sxs-lookup"><span data-stu-id="d928a-209">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="d928a-210">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="d928a-210">deviceEnrollmentType</span></span>|[<span data-ttu-id="d928a-211">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="d928a-211">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="d928a-212">设备的注册类型。</span><span class="sxs-lookup"><span data-stu-id="d928a-212">Enrollment type of the device.</span></span> <span data-ttu-id="d928a-213">可取值为：`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement`。</span><span class="sxs-lookup"><span data-stu-id="d928a-213">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="d928a-214">lostModeState</span><span class="sxs-lookup"><span data-stu-id="d928a-214">lostModeState</span></span>|[<span data-ttu-id="d928a-215">lostModeState</span><span class="sxs-lookup"><span data-stu-id="d928a-215">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="d928a-216">指示是否启用或禁用丢失的模式。</span><span class="sxs-lookup"><span data-stu-id="d928a-216">Indicates if Lost mode is enabled or disabled.</span></span> <span data-ttu-id="d928a-217">可取值为：`disabled`、`enabled`。</span><span class="sxs-lookup"><span data-stu-id="d928a-217">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="d928a-218">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="d928a-218">activationLockBypassCode</span></span>|<span data-ttu-id="d928a-219">String</span><span class="sxs-lookup"><span data-stu-id="d928a-219">String</span></span>|<span data-ttu-id="d928a-220">允许绕过设备上的激活锁的代码。</span><span class="sxs-lookup"><span data-stu-id="d928a-220">Code that allows the Activation Lock on a device to be bypassed.</span></span>|
|<span data-ttu-id="d928a-221">emailAddress</span><span class="sxs-lookup"><span data-stu-id="d928a-221">emailAddress</span></span>|<span data-ttu-id="d928a-222">String</span><span class="sxs-lookup"><span data-stu-id="d928a-222">String</span></span>|<span data-ttu-id="d928a-223">与设备关联的用户的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="d928a-223">Email(s) for the user associated with the device</span></span>|
|<span data-ttu-id="d928a-224">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="d928a-224">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="d928a-225">String</span><span class="sxs-lookup"><span data-stu-id="d928a-225">String</span></span>|<span data-ttu-id="d928a-226">Azure Active Directory 设备的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="d928a-226">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="d928a-227">只读。</span><span class="sxs-lookup"><span data-stu-id="d928a-227">Read only.</span></span>|
|<span data-ttu-id="d928a-228">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="d928a-228">azureADDeviceId</span></span>|<span data-ttu-id="d928a-229">String</span><span class="sxs-lookup"><span data-stu-id="d928a-229">String</span></span>|<span data-ttu-id="d928a-230">Azure Active Directory 设备的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="d928a-230">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="d928a-231">只读。</span><span class="sxs-lookup"><span data-stu-id="d928a-231">Read only.</span></span>|
|<span data-ttu-id="d928a-232">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="d928a-232">deviceRegistrationState</span></span>|[<span data-ttu-id="d928a-233">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="d928a-233">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="d928a-234">设备注册状态。</span><span class="sxs-lookup"><span data-stu-id="d928a-234">Device registration state.</span></span> <span data-ttu-id="d928a-235">可取值为：`notRegistered`、`registered`、`revoked`、`keyConflict`、`approvalPending`、`certificateReset`、`notRegisteredPendingEnrollment`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="d928a-235">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="d928a-236">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="d928a-236">deviceCategoryDisplayName</span></span>|<span data-ttu-id="d928a-237">String</span><span class="sxs-lookup"><span data-stu-id="d928a-237">String</span></span>|<span data-ttu-id="d928a-238">设备类别显示名称。</span><span class="sxs-lookup"><span data-stu-id="d928a-238">Device category display name</span></span>|
|<span data-ttu-id="d928a-239">isSupervised</span><span class="sxs-lookup"><span data-stu-id="d928a-239">isSupervised</span></span>|<span data-ttu-id="d928a-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="d928a-240">Boolean</span></span>|<span data-ttu-id="d928a-241">设备受监督状态</span><span class="sxs-lookup"><span data-stu-id="d928a-241">Device supervised status</span></span>|
|<span data-ttu-id="d928a-242">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="d928a-242">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="d928a-243">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d928a-243">DateTimeOffset</span></span>|<span data-ttu-id="d928a-244">设备上次与 Exchange 联系的时间。</span><span class="sxs-lookup"><span data-stu-id="d928a-244">Last time the device contacted Exchange.</span></span>|
|<span data-ttu-id="d928a-245">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="d928a-245">exchangeAccessState</span></span>|[<span data-ttu-id="d928a-246">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="d928a-246">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="d928a-247">Exchange 中设备的访问状态。</span><span class="sxs-lookup"><span data-stu-id="d928a-247">The Access State of the device in Exchange.</span></span> <span data-ttu-id="d928a-248">可取值为：`none`、`unknown`、`allowed`、`blocked`、`quarantined`。</span><span class="sxs-lookup"><span data-stu-id="d928a-248">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="d928a-249">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="d928a-249">exchangeAccessStateReason</span></span>|[<span data-ttu-id="d928a-250">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="d928a-250">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="d928a-251">Exchange 中设备访问状态的出现原因。</span><span class="sxs-lookup"><span data-stu-id="d928a-251">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="d928a-252">可取值为：`none`、`unknown`、`exchangeGlobalRule`、`exchangeIndividualRule`、`exchangeDeviceRule`、`exchangeUpgrade`、`exchangeMailboxPolicy`、`other`、`compliant`、`notCompliant`、`notEnrolled`、`unknownLocation`、`mfaRequired`、`azureADBlockDueToAccessPolicy`、`compromisedPassword`、`deviceNotKnownWithManagedApp`。</span><span class="sxs-lookup"><span data-stu-id="d928a-252">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="d928a-253">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="d928a-253">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="d928a-254">String</span><span class="sxs-lookup"><span data-stu-id="d928a-254">String</span></span>|<span data-ttu-id="d928a-255">允许与设备建立远程协助会话的 URL。</span><span class="sxs-lookup"><span data-stu-id="d928a-255">Url that allows a Remote Assistance session to be established with the device.</span></span>|
|<span data-ttu-id="d928a-256">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="d928a-256">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="d928a-257">String</span><span class="sxs-lookup"><span data-stu-id="d928a-257">String</span></span>|<span data-ttu-id="d928a-258">用于在创建远程协助会话对象时识别问题的错误字符串。</span><span class="sxs-lookup"><span data-stu-id="d928a-258">An error string that identifies issues when creating Remote Assistance session objects.</span></span>|
|<span data-ttu-id="d928a-259">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="d928a-259">isEncrypted</span></span>|<span data-ttu-id="d928a-260">Boolean</span><span class="sxs-lookup"><span data-stu-id="d928a-260">Boolean</span></span>|<span data-ttu-id="d928a-261">设备加密状态</span><span class="sxs-lookup"><span data-stu-id="d928a-261">Device encryption status</span></span>|
|<span data-ttu-id="d928a-262">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d928a-262">userPrincipalName</span></span>|<span data-ttu-id="d928a-263">String</span><span class="sxs-lookup"><span data-stu-id="d928a-263">String</span></span>|<span data-ttu-id="d928a-264">设备用户主体名称</span><span class="sxs-lookup"><span data-stu-id="d928a-264">Device user principal name</span></span>|
|<span data-ttu-id="d928a-265">model</span><span class="sxs-lookup"><span data-stu-id="d928a-265">model</span></span>|<span data-ttu-id="d928a-266">String</span><span class="sxs-lookup"><span data-stu-id="d928a-266">String</span></span>|<span data-ttu-id="d928a-267">设备的型号</span><span class="sxs-lookup"><span data-stu-id="d928a-267">Model of the device</span></span>|
|<span data-ttu-id="d928a-268">manufacturer</span><span class="sxs-lookup"><span data-stu-id="d928a-268">manufacturer</span></span>|<span data-ttu-id="d928a-269">String</span><span class="sxs-lookup"><span data-stu-id="d928a-269">String</span></span>|<span data-ttu-id="d928a-270">设备的制造商</span><span class="sxs-lookup"><span data-stu-id="d928a-270">Manufacturer of the device</span></span>|
|<span data-ttu-id="d928a-271">imei</span><span class="sxs-lookup"><span data-stu-id="d928a-271">imei</span></span>|<span data-ttu-id="d928a-272">String</span><span class="sxs-lookup"><span data-stu-id="d928a-272">String</span></span>|<span data-ttu-id="d928a-273">IMEI</span><span class="sxs-lookup"><span data-stu-id="d928a-273">IMEI</span></span>|
|<span data-ttu-id="d928a-274">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="d928a-274">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="d928a-275">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d928a-275">DateTimeOffset</span></span>|<span data-ttu-id="d928a-276">设备符合性宽限期的到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="d928a-276">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="d928a-277">serialNumber</span><span class="sxs-lookup"><span data-stu-id="d928a-277">serialNumber</span></span>|<span data-ttu-id="d928a-278">String</span><span class="sxs-lookup"><span data-stu-id="d928a-278">String</span></span>|<span data-ttu-id="d928a-279">序列号</span><span class="sxs-lookup"><span data-stu-id="d928a-279">SerialNumber</span></span>|
|<span data-ttu-id="d928a-280">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="d928a-280">phoneNumber</span></span>|<span data-ttu-id="d928a-281">String</span><span class="sxs-lookup"><span data-stu-id="d928a-281">String</span></span>|<span data-ttu-id="d928a-282">设备的电话号码</span><span class="sxs-lookup"><span data-stu-id="d928a-282">Phone number of the device</span></span>|
|<span data-ttu-id="d928a-283">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="d928a-283">androidSecurityPatchLevel</span></span>|<span data-ttu-id="d928a-284">String</span><span class="sxs-lookup"><span data-stu-id="d928a-284">String</span></span>|<span data-ttu-id="d928a-285">Android 安全修补程序级别</span><span class="sxs-lookup"><span data-stu-id="d928a-285">Android security patch level</span></span>|
|<span data-ttu-id="d928a-286">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="d928a-286">userDisplayName</span></span>|<span data-ttu-id="d928a-287">String</span><span class="sxs-lookup"><span data-stu-id="d928a-287">String</span></span>|<span data-ttu-id="d928a-288">用户显示名称</span><span class="sxs-lookup"><span data-stu-id="d928a-288">User display name</span></span>|
|<span data-ttu-id="d928a-289">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="d928a-289">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="d928a-290">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="d928a-290">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="d928a-291">ConfigrMgr 客户端启用的功能</span><span class="sxs-lookup"><span data-stu-id="d928a-291">ConfigrMgr client enabled features</span></span>|
|<span data-ttu-id="d928a-292">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="d928a-292">wiFiMacAddress</span></span>|<span data-ttu-id="d928a-293">String</span><span class="sxs-lookup"><span data-stu-id="d928a-293">String</span></span>|<span data-ttu-id="d928a-294">Wi-Fi MAC</span><span class="sxs-lookup"><span data-stu-id="d928a-294">Wi-Fi MAC</span></span>|
|<span data-ttu-id="d928a-295">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="d928a-295">deviceHealthAttestationState</span></span>|[<span data-ttu-id="d928a-296">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="d928a-296">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="d928a-297">设备运行状况证明状态。</span><span class="sxs-lookup"><span data-stu-id="d928a-297">The device health attestation state.</span></span>|
|<span data-ttu-id="d928a-298">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="d928a-298">subscriberCarrier</span></span>|<span data-ttu-id="d928a-299">String</span><span class="sxs-lookup"><span data-stu-id="d928a-299">String</span></span>|<span data-ttu-id="d928a-300">订阅者运营商</span><span class="sxs-lookup"><span data-stu-id="d928a-300">Subscriber Carrier</span></span>|
|<span data-ttu-id="d928a-301">meid</span><span class="sxs-lookup"><span data-stu-id="d928a-301">meid</span></span>|<span data-ttu-id="d928a-302">String</span><span class="sxs-lookup"><span data-stu-id="d928a-302">String</span></span>|<span data-ttu-id="d928a-303">MEID</span><span class="sxs-lookup"><span data-stu-id="d928a-303">MEID</span></span>|
|<span data-ttu-id="d928a-304">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="d928a-304">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="d928a-305">Int64</span><span class="sxs-lookup"><span data-stu-id="d928a-305">Int64</span></span>|<span data-ttu-id="d928a-306">存储空间总字节数</span><span class="sxs-lookup"><span data-stu-id="d928a-306">Total Storage in Bytes</span></span>|
|<span data-ttu-id="d928a-307">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="d928a-307">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="d928a-308">Int64</span><span class="sxs-lookup"><span data-stu-id="d928a-308">Int64</span></span>|<span data-ttu-id="d928a-309">可用存储空间字节数</span><span class="sxs-lookup"><span data-stu-id="d928a-309">Free Storage in Bytes</span></span>|
|<span data-ttu-id="d928a-310">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="d928a-310">managedDeviceName</span></span>|<span data-ttu-id="d928a-311">String</span><span class="sxs-lookup"><span data-stu-id="d928a-311">String</span></span>|<span data-ttu-id="d928a-312">用于识别设备的自动生成的名称。</span><span class="sxs-lookup"><span data-stu-id="d928a-312">Automatically generated name to identify a device.</span></span> <span data-ttu-id="d928a-313">可以覆盖为用户友好名称。</span><span class="sxs-lookup"><span data-stu-id="d928a-313">Can be overwritten to a user friendly name.</span></span>|
|<span data-ttu-id="d928a-314">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="d928a-314">partnerReportedThreatState</span></span>|[<span data-ttu-id="d928a-315">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="d928a-315">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="d928a-316">指示帐户和设备正在使用移动威胁防护合作伙伴时设备的威胁状态。</span><span class="sxs-lookup"><span data-stu-id="d928a-316">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="d928a-317">只读。</span><span class="sxs-lookup"><span data-stu-id="d928a-317">Read Only.</span></span> <span data-ttu-id="d928a-318">可取值为：`unknown`、`activated`、`deactivated`、`secured`、`lowSeverity`、`mediumSeverity`、`highSeverity`、`unresponsive`、`compromised`、`misconfigured`。</span><span class="sxs-lookup"><span data-stu-id="d928a-318">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="d928a-319">usersLoggedOn</span><span class="sxs-lookup"><span data-stu-id="d928a-319">usersLoggedOn</span></span>|<span data-ttu-id="d928a-320">[loggedOnUser](../resources/intune-devices-loggedonuser.md)集合</span><span class="sxs-lookup"><span data-stu-id="d928a-320">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="d928a-321">指示上次登录的设备的用户</span><span class="sxs-lookup"><span data-stu-id="d928a-321">Indicates the last logged on users of a device</span></span>|
|<span data-ttu-id="d928a-322">preferMdmOverGroupPolicyAppliedDateTime</span><span class="sxs-lookup"><span data-stu-id="d928a-322">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="d928a-323">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d928a-323">DateTimeOffset</span></span>|<span data-ttu-id="d928a-324">报告 DateTime 的 preferMdmOverGroupPolicy 设置。</span><span class="sxs-lookup"><span data-stu-id="d928a-324">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="d928a-325">设置时，这些 Intune MDM 设置将覆盖组策略设置冲突时。</span><span class="sxs-lookup"><span data-stu-id="d928a-325">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="d928a-326">只读。</span><span class="sxs-lookup"><span data-stu-id="d928a-326">Read Only.</span></span>|
|<span data-ttu-id="d928a-327">autopilotEnrolled</span><span class="sxs-lookup"><span data-stu-id="d928a-327">autopilotEnrolled</span></span>|<span data-ttu-id="d928a-328">Boolean</span><span class="sxs-lookup"><span data-stu-id="d928a-328">Boolean</span></span>|<span data-ttu-id="d928a-329">如果通过自动试点注册托管的设备，报告。</span><span class="sxs-lookup"><span data-stu-id="d928a-329">Reports if the managed device is enrolled via auto-pilot.</span></span>|
|<span data-ttu-id="d928a-330">requireUserEnrollmentApproval</span><span class="sxs-lookup"><span data-stu-id="d928a-330">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="d928a-331">Boolean</span><span class="sxs-lookup"><span data-stu-id="d928a-331">Boolean</span></span>|<span data-ttu-id="d928a-332">报告托管的 iOS 设备是否用户审批注册。</span><span class="sxs-lookup"><span data-stu-id="d928a-332">Reports if the managed iOS device is user approval enrollment.</span></span>|
|<span data-ttu-id="d928a-333">managementCertificateExpirationDate</span><span class="sxs-lookup"><span data-stu-id="d928a-333">managementCertificateExpirationDate</span></span>|<span data-ttu-id="d928a-334">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d928a-334">DateTimeOffset</span></span>|<span data-ttu-id="d928a-335">报告设备管理证书过期日期</span><span class="sxs-lookup"><span data-stu-id="d928a-335">Reports device management certificate expiration date</span></span>|
|<span data-ttu-id="d928a-336">iccid</span><span class="sxs-lookup"><span data-stu-id="d928a-336">iccid</span></span>|<span data-ttu-id="d928a-337">字符串</span><span class="sxs-lookup"><span data-stu-id="d928a-337">String</span></span>|<span data-ttu-id="d928a-338">集成的电路卡标识符，它是 SIM 卡的唯一标识号。</span><span class="sxs-lookup"><span data-stu-id="d928a-338">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span>|
|<span data-ttu-id="d928a-339">udid</span><span class="sxs-lookup"><span data-stu-id="d928a-339">udid</span></span>|<span data-ttu-id="d928a-340">字符串</span><span class="sxs-lookup"><span data-stu-id="d928a-340">String</span></span>|<span data-ttu-id="d928a-341">IOS 和 macOS 设备的唯一设备标识符。</span><span class="sxs-lookup"><span data-stu-id="d928a-341">Unique Device Identifier for iOS and macOS devices.</span></span>|
|<span data-ttu-id="d928a-342">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d928a-342">roleScopeTagIds</span></span>|<span data-ttu-id="d928a-343">String 集合</span><span class="sxs-lookup"><span data-stu-id="d928a-343">String collection</span></span>|<span data-ttu-id="d928a-344">此设备实例范围标记 Id 的列表。</span><span class="sxs-lookup"><span data-stu-id="d928a-344">List of Scope Tag IDs for this Device instance.</span></span>|
|<span data-ttu-id="d928a-345">windowsActiveMalwareCount</span><span class="sxs-lookup"><span data-stu-id="d928a-345">windowsActiveMalwareCount</span></span>|<span data-ttu-id="d928a-346">Int32</span><span class="sxs-lookup"><span data-stu-id="d928a-346">Int32</span></span>|<span data-ttu-id="d928a-347">此 windows 设备的活动恶意软件的计数</span><span class="sxs-lookup"><span data-stu-id="d928a-347">Count of active malware for this windows device</span></span>|
|<span data-ttu-id="d928a-348">windowsRemediatedMalwareCount</span><span class="sxs-lookup"><span data-stu-id="d928a-348">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="d928a-349">Int32</span><span class="sxs-lookup"><span data-stu-id="d928a-349">Int32</span></span>|<span data-ttu-id="d928a-350">此 windows 设备的补救恶意软件的计数</span><span class="sxs-lookup"><span data-stu-id="d928a-350">Count of remediated malware for this windows device</span></span>|
|<span data-ttu-id="d928a-351">notes</span><span class="sxs-lookup"><span data-stu-id="d928a-351">notes</span></span>|<span data-ttu-id="d928a-352">String</span><span class="sxs-lookup"><span data-stu-id="d928a-352">String</span></span>|<span data-ttu-id="d928a-353">由 IT 管理员在设备上的说明</span><span class="sxs-lookup"><span data-stu-id="d928a-353">Notes on the device created by IT Admin</span></span>|
|<span data-ttu-id="d928a-354">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="d928a-354">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="d928a-355">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="d928a-355">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="d928a-356">配置管理器客户端健康状态，仅供 MDM/ConfigMgr 代理管理设备</span><span class="sxs-lookup"><span data-stu-id="d928a-356">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent</span></span>|



## <a name="response"></a><span data-ttu-id="d928a-357">响应</span><span class="sxs-lookup"><span data-stu-id="d928a-357">Response</span></span>
<span data-ttu-id="d928a-358">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [managedDevice](../resources/intune-devices-manageddevice.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d928a-358">If successful, this method returns a `200 OK` response code and an updated [managedDevice](../resources/intune-devices-manageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d928a-359">示例</span><span class="sxs-lookup"><span data-stu-id="d928a-359">Example</span></span>
### <a name="request"></a><span data-ttu-id="d928a-360">请求</span><span class="sxs-lookup"><span data-stu-id="d928a-360">Request</span></span>
<span data-ttu-id="d928a-361">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d928a-361">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/users/{usersId}/managedDevices/{managedDeviceId}
Content-type: application/json
Content-length: 7114

{
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

### <a name="response"></a><span data-ttu-id="d928a-362">响应</span><span class="sxs-lookup"><span data-stu-id="d928a-362">Response</span></span>
<span data-ttu-id="d928a-p122">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d928a-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 7215

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





