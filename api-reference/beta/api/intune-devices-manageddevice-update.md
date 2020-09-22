---
title: 更新 managedDevice
description: 更新 managedDevice 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6417612a89f862c7add02fb3fed818ea3966c4ed
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48072506"
---
# <a name="update-manageddevice"></a><span data-ttu-id="8dbab-103">更新 managedDevice</span><span class="sxs-lookup"><span data-stu-id="8dbab-103">Update managedDevice</span></span>

<span data-ttu-id="8dbab-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8dbab-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8dbab-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8dbab-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8dbab-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8dbab-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8dbab-107">更新 [managedDevice](../resources/intune-devices-manageddevice.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8dbab-107">Update the properties of a [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8dbab-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="8dbab-108">Prerequisites</span></span>
<span data-ttu-id="8dbab-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8dbab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8dbab-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="8dbab-111">Permission type</span></span>|<span data-ttu-id="8dbab-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8dbab-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8dbab-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8dbab-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8dbab-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8dbab-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="8dbab-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8dbab-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8dbab-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8dbab-116">Not supported.</span></span>|
|<span data-ttu-id="8dbab-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="8dbab-117">Application</span></span>|<span data-ttu-id="8dbab-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8dbab-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8dbab-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8dbab-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managedDevices/{managedDeviceId}
PATCH /deviceManagement/comanagedDevices/{managedDeviceId}
PATCH /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice
PATCH /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates/{deviceComplianceScriptDeviceStateId}/managedDevice
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}
```

## <a name="request-headers"></a><span data-ttu-id="8dbab-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="8dbab-120">Request headers</span></span>
|<span data-ttu-id="8dbab-121">标头</span><span class="sxs-lookup"><span data-stu-id="8dbab-121">Header</span></span>|<span data-ttu-id="8dbab-122">值</span><span class="sxs-lookup"><span data-stu-id="8dbab-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8dbab-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8dbab-123">Authorization</span></span>|<span data-ttu-id="8dbab-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8dbab-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8dbab-125">接受</span><span class="sxs-lookup"><span data-stu-id="8dbab-125">Accept</span></span>|<span data-ttu-id="8dbab-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8dbab-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8dbab-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="8dbab-127">Request body</span></span>
<span data-ttu-id="8dbab-128">在请求正文中，提供 [managedDevice](../resources/intune-devices-manageddevice.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8dbab-128">In the request body, supply a JSON representation for the [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>

<span data-ttu-id="8dbab-129">下表显示创建 [managedDevice](../resources/intune-devices-manageddevice.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="8dbab-129">The following table shows the properties that are required when you create the [managedDevice](../resources/intune-devices-manageddevice.md).</span></span>

|<span data-ttu-id="8dbab-130">属性</span><span class="sxs-lookup"><span data-stu-id="8dbab-130">Property</span></span>|<span data-ttu-id="8dbab-131">类型</span><span class="sxs-lookup"><span data-stu-id="8dbab-131">Type</span></span>|<span data-ttu-id="8dbab-132">说明</span><span class="sxs-lookup"><span data-stu-id="8dbab-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8dbab-133">id</span><span class="sxs-lookup"><span data-stu-id="8dbab-133">id</span></span>|<span data-ttu-id="8dbab-134">String</span><span class="sxs-lookup"><span data-stu-id="8dbab-134">String</span></span>|<span data-ttu-id="8dbab-135">设备的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="8dbab-135">Unique Identifier for the device.</span></span> <span data-ttu-id="8dbab-136">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8dbab-136">This property is read-only.</span></span>|
|<span data-ttu-id="8dbab-137">userId</span><span class="sxs-lookup"><span data-stu-id="8dbab-137">userId</span></span>|<span data-ttu-id="8dbab-138">String</span><span class="sxs-lookup"><span data-stu-id="8dbab-138">String</span></span>|<span data-ttu-id="8dbab-139">与设备关联的用户的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="8dbab-139">Unique Identifier for the user associated with the device.</span></span> <span data-ttu-id="8dbab-140">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8dbab-140">This property is read-only.</span></span>|
|<span data-ttu-id="8dbab-141">deviceName</span><span class="sxs-lookup"><span data-stu-id="8dbab-141">deviceName</span></span>|<span data-ttu-id="8dbab-142">String</span><span class="sxs-lookup"><span data-stu-id="8dbab-142">String</span></span>|<span data-ttu-id="8dbab-143">设备的名称。</span><span class="sxs-lookup"><span data-stu-id="8dbab-143">Name of the device.</span></span> <span data-ttu-id="8dbab-144">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8dbab-144">This property is read-only.</span></span>|
|<span data-ttu-id="8dbab-145">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="8dbab-145">hardwareInformation</span></span>|[<span data-ttu-id="8dbab-146">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="8dbab-146">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="8dbab-147">设备的 hardward 详细信息。</span><span class="sxs-lookup"><span data-stu-id="8dbab-147">The hardward details for the device.</span></span>  <span data-ttu-id="8dbab-148">包括存储空间、制造商、序列号等信息。此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8dbab-148">Includes information such as storage space, manufacturer, serial number, etc. This property is read-only.</span></span>|
|<span data-ttu-id="8dbab-149">所有者</span><span class="sxs-lookup"><span data-stu-id="8dbab-149">ownerType</span></span>|[<span data-ttu-id="8dbab-150">所有者</span><span class="sxs-lookup"><span data-stu-id="8dbab-150">ownerType</span></span>](../resources/intune-shared-ownertype.md)|<span data-ttu-id="8dbab-151">设备的所有权。</span><span class="sxs-lookup"><span data-stu-id="8dbab-151">Ownership of the device.</span></span> <span data-ttu-id="8dbab-152">可以是 "公司" 或 "个人"。</span><span class="sxs-lookup"><span data-stu-id="8dbab-152">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="8dbab-153">可取值为：`unknown`、`company`、`personal`。</span><span class="sxs-lookup"><span data-stu-id="8dbab-153">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="8dbab-154">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="8dbab-154">managedDeviceOwnerType</span></span>|[<span data-ttu-id="8dbab-155">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="8dbab-155">managedDeviceOwnerType</span></span>](../resources/intune-shared-manageddeviceownertype.md)|<span data-ttu-id="8dbab-156">设备的所有权。</span><span class="sxs-lookup"><span data-stu-id="8dbab-156">Ownership of the device.</span></span> <span data-ttu-id="8dbab-157">可以是 "公司" 或 "个人"。</span><span class="sxs-lookup"><span data-stu-id="8dbab-157">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="8dbab-158">可取值为：`unknown`、`company`、`personal`。</span><span class="sxs-lookup"><span data-stu-id="8dbab-158">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="8dbab-159">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="8dbab-159">deviceActionResults</span></span>|<span data-ttu-id="8dbab-160">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8dbab-160">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="8dbab-161">ComplexType deviceActionResult 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="8dbab-161">List of ComplexType deviceActionResult objects.</span></span> <span data-ttu-id="8dbab-162">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8dbab-162">This property is read-only.</span></span>|
|<span data-ttu-id="8dbab-163">managementState</span><span class="sxs-lookup"><span data-stu-id="8dbab-163">managementState</span></span>|[<span data-ttu-id="8dbab-164">managementState</span><span class="sxs-lookup"><span data-stu-id="8dbab-164">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="8dbab-165">设备的管理状态。</span><span class="sxs-lookup"><span data-stu-id="8dbab-165">Management state of the device.</span></span> <span data-ttu-id="8dbab-166">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8dbab-166">This property is read-only.</span></span> <span data-ttu-id="8dbab-167">可取值为：`managed`、`retirePending`、`retireFailed`、`wipePending`、`wipeFailed`、`unhealthy`、`deletePending`、`retireIssued`、`wipeIssued`、`wipeCanceled`、`retireCanceled`、`discovered`。</span><span class="sxs-lookup"><span data-stu-id="8dbab-167">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="8dbab-168">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="8dbab-168">enrolledDateTime</span></span>|<span data-ttu-id="8dbab-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8dbab-169">DateTimeOffset</span></span>|<span data-ttu-id="8dbab-170">设备的注册时间。</span><span class="sxs-lookup"><span data-stu-id="8dbab-170">Enrollment time of the device.</span></span> <span data-ttu-id="8dbab-171">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8dbab-171">This property is read-only.</span></span>|
|<span data-ttu-id="8dbab-172">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="8dbab-172">lastSyncDateTime</span></span>|<span data-ttu-id="8dbab-173">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8dbab-173">DateTimeOffset</span></span>|<span data-ttu-id="8dbab-174">设备上次成功完成与 Intune 同步的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="8dbab-174">The date and time that the device last completed a successful sync with Intune.</span></span> <span data-ttu-id="8dbab-175">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8dbab-175">This property is read-only.</span></span>|
|<span data-ttu-id="8dbab-176">chassisType</span><span class="sxs-lookup"><span data-stu-id="8dbab-176">chassisType</span></span>|[<span data-ttu-id="8dbab-177">chassisType</span><span class="sxs-lookup"><span data-stu-id="8dbab-177">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="8dbab-178">设备的机箱类型。</span><span class="sxs-lookup"><span data-stu-id="8dbab-178">Chassis type of the device.</span></span> <span data-ttu-id="8dbab-179">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8dbab-179">This property is read-only.</span></span> <span data-ttu-id="8dbab-180">可取值为：`unknown`、`desktop`、`laptop`、`worksWorkstation`、`enterpriseServer`、`phone`、`tablet`、`mobileOther`、`mobileUnknown`。</span><span class="sxs-lookup"><span data-stu-id="8dbab-180">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="8dbab-181">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="8dbab-181">operatingSystem</span></span>|<span data-ttu-id="8dbab-182">String</span><span class="sxs-lookup"><span data-stu-id="8dbab-182">String</span></span>|<span data-ttu-id="8dbab-183">设备的操作系统。</span><span class="sxs-lookup"><span data-stu-id="8dbab-183">Operating system of the device.</span></span> <span data-ttu-id="8dbab-184">Windows、iOS 等。此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8dbab-184">Windows, iOS, etc. This property is read-only.</span></span>|
|<span data-ttu-id="8dbab-185">deviceType</span><span class="sxs-lookup"><span data-stu-id="8dbab-185">deviceType</span></span>|[<span data-ttu-id="8dbab-186">deviceType</span><span class="sxs-lookup"><span data-stu-id="8dbab-186">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="8dbab-187">设备的平台。</span><span class="sxs-lookup"><span data-stu-id="8dbab-187">Platform of the device.</span></span> <span data-ttu-id="8dbab-188">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8dbab-188">This property is read-only.</span></span> <span data-ttu-id="8dbab-189">可能的值为：、、、、、、、、、、、、、、、、、、、、、、、、 `desktop` `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `windows10x` `androidnGMS` `cloudPC` `blackberry` `palm` `unknown` 。</span><span class="sxs-lookup"><span data-stu-id="8dbab-189">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `androidnGMS`, `cloudPC`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="8dbab-190">complianceState</span><span class="sxs-lookup"><span data-stu-id="8dbab-190">complianceState</span></span>|[<span data-ttu-id="8dbab-191">complianceState</span><span class="sxs-lookup"><span data-stu-id="8dbab-191">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="8dbab-192">设备的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="8dbab-192">Compliance state of the device.</span></span> <span data-ttu-id="8dbab-193">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8dbab-193">This property is read-only.</span></span> <span data-ttu-id="8dbab-194">可取值为：`unknown`、`compliant`、`noncompliant`、`conflict`、`error`、`inGracePeriod`、`configManager`。</span><span class="sxs-lookup"><span data-stu-id="8dbab-194">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="8dbab-195">jailBroken</span><span class="sxs-lookup"><span data-stu-id="8dbab-195">jailBroken</span></span>|<span data-ttu-id="8dbab-196">String</span><span class="sxs-lookup"><span data-stu-id="8dbab-196">String</span></span>|<span data-ttu-id="8dbab-197">设备是否已越狱或取得 root 权限。</span><span class="sxs-lookup"><span data-stu-id="8dbab-197">whether the device is jail broken or rooted.</span></span> <span data-ttu-id="8dbab-198">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8dbab-198">This property is read-only.</span></span>|
|<span data-ttu-id="8dbab-199">managementAgent</span><span class="sxs-lookup"><span data-stu-id="8dbab-199">managementAgent</span></span>|[<span data-ttu-id="8dbab-200">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="8dbab-200">managementAgentType</span></span>](../resources/intune-shared-managementagenttype.md)|<span data-ttu-id="8dbab-201">设备的管理通道。</span><span class="sxs-lookup"><span data-stu-id="8dbab-201">Management channel of the device.</span></span> <span data-ttu-id="8dbab-202">Intune、EAS 等。此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8dbab-202">Intune, EAS, etc. This property is read-only.</span></span> <span data-ttu-id="8dbab-203">可能的值是：`eas`、`mdm`、`easMdm`、`intuneClient`、`easIntuneClient`、`configurationManagerClient`、`configurationManagerClientMdm`、`configurationManagerClientMdmEas`、`unknown`、`jamf`、`googleCloudDevicePolicyController`、`microsoft365ManagedMdm`、`windowsManagementCloudApi`。</span><span class="sxs-lookup"><span data-stu-id="8dbab-203">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`, `windowsManagementCloudApi`.</span></span>|
|<span data-ttu-id="8dbab-204">osVersion</span><span class="sxs-lookup"><span data-stu-id="8dbab-204">osVersion</span></span>|<span data-ttu-id="8dbab-205">String</span><span class="sxs-lookup"><span data-stu-id="8dbab-205">String</span></span>|<span data-ttu-id="8dbab-206">设备的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="8dbab-206">Operating system version of the device.</span></span> <span data-ttu-id="8dbab-207">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8dbab-207">This property is read-only.</span></span>|
|<span data-ttu-id="8dbab-208">easActivated</span><span class="sxs-lookup"><span data-stu-id="8dbab-208">easActivated</span></span>|<span data-ttu-id="8dbab-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="8dbab-209">Boolean</span></span>|<span data-ttu-id="8dbab-210">设备是否已激活 Exchange ActiveSync。</span><span class="sxs-lookup"><span data-stu-id="8dbab-210">Whether the device is Exchange ActiveSync activated.</span></span> <span data-ttu-id="8dbab-211">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8dbab-211">This property is read-only.</span></span>|
|<span data-ttu-id="8dbab-212">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="8dbab-212">easDeviceId</span></span>|<span data-ttu-id="8dbab-213">String</span><span class="sxs-lookup"><span data-stu-id="8dbab-213">String</span></span>|<span data-ttu-id="8dbab-214">设备的 Exchange ActiveSync ID。</span><span class="sxs-lookup"><span data-stu-id="8dbab-214">Exchange ActiveSync Id of the device.</span></span> <span data-ttu-id="8dbab-215">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8dbab-215">This property is read-only.</span></span>|
|<span data-ttu-id="8dbab-216">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="8dbab-216">easActivationDateTime</span></span>|<span data-ttu-id="8dbab-217">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8dbab-217">DateTimeOffset</span></span>|<span data-ttu-id="8dbab-218">设备的 Exchange ActivationSync 激活时间。</span><span class="sxs-lookup"><span data-stu-id="8dbab-218">Exchange ActivationSync activation time of the device.</span></span> <span data-ttu-id="8dbab-219">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8dbab-219">This property is read-only.</span></span>|
|<span data-ttu-id="8dbab-220">aadRegistered</span><span class="sxs-lookup"><span data-stu-id="8dbab-220">aadRegistered</span></span>|<span data-ttu-id="8dbab-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="8dbab-221">Boolean</span></span>|<span data-ttu-id="8dbab-222">设备是否已注册 Azure Active Directory。</span><span class="sxs-lookup"><span data-stu-id="8dbab-222">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="8dbab-223">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8dbab-223">This property is read-only.</span></span>|
|<span data-ttu-id="8dbab-224">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="8dbab-224">azureADRegistered</span></span>|<span data-ttu-id="8dbab-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="8dbab-225">Boolean</span></span>|<span data-ttu-id="8dbab-226">设备是否已注册 Azure Active Directory。</span><span class="sxs-lookup"><span data-stu-id="8dbab-226">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="8dbab-227">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8dbab-227">This property is read-only.</span></span>|
|<span data-ttu-id="8dbab-228">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="8dbab-228">deviceEnrollmentType</span></span>|[<span data-ttu-id="8dbab-229">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="8dbab-229">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="8dbab-230">设备的注册类型。</span><span class="sxs-lookup"><span data-stu-id="8dbab-230">Enrollment type of the device.</span></span> <span data-ttu-id="8dbab-231">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8dbab-231">This property is read-only.</span></span> <span data-ttu-id="8dbab-232">可取值为：`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement`、`appleUserEnrollment`、`appleUserEnrollmentWithServiceAccount`、`azureAdJoinUsingAzureVmExtension`、`androidEnterpriseDedicatedDevice`、`androidEnterpriseFullyManaged`、`androidEnterpriseCorporateWorkProfile`。</span><span class="sxs-lookup"><span data-stu-id="8dbab-232">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`, `azureAdJoinUsingAzureVmExtension`, `androidEnterpriseDedicatedDevice`, `androidEnterpriseFullyManaged`, `androidEnterpriseCorporateWorkProfile`.</span></span>|
|<span data-ttu-id="8dbab-233">lostModeState</span><span class="sxs-lookup"><span data-stu-id="8dbab-233">lostModeState</span></span>|[<span data-ttu-id="8dbab-234">lostModeState</span><span class="sxs-lookup"><span data-stu-id="8dbab-234">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="8dbab-235">指示是否已启用或禁用了丢失模式。</span><span class="sxs-lookup"><span data-stu-id="8dbab-235">Indicates if Lost mode is enabled or disabled.</span></span> <span data-ttu-id="8dbab-236">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8dbab-236">This property is read-only.</span></span> <span data-ttu-id="8dbab-237">可取值为：`disabled`、`enabled`。</span><span class="sxs-lookup"><span data-stu-id="8dbab-237">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="8dbab-238">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="8dbab-238">activationLockBypassCode</span></span>|<span data-ttu-id="8dbab-239">String</span><span class="sxs-lookup"><span data-stu-id="8dbab-239">String</span></span>|<span data-ttu-id="8dbab-240">允许绕过设备上的激活锁的代码。</span><span class="sxs-lookup"><span data-stu-id="8dbab-240">Code that allows the Activation Lock on a device to be bypassed.</span></span> <span data-ttu-id="8dbab-241">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8dbab-241">This property is read-only.</span></span>|
|<span data-ttu-id="8dbab-242">emailAddress</span><span class="sxs-lookup"><span data-stu-id="8dbab-242">emailAddress</span></span>|<span data-ttu-id="8dbab-243">String</span><span class="sxs-lookup"><span data-stu-id="8dbab-243">String</span></span>|<span data-ttu-id="8dbab-244">与设备关联的用户的电子邮件 (s) 。</span><span class="sxs-lookup"><span data-stu-id="8dbab-244">Email(s) for the user associated with the device.</span></span> <span data-ttu-id="8dbab-245">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8dbab-245">This property is read-only.</span></span>|
|<span data-ttu-id="8dbab-246">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="8dbab-246">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="8dbab-247">String</span><span class="sxs-lookup"><span data-stu-id="8dbab-247">String</span></span>|<span data-ttu-id="8dbab-248">Azure Active Directory 设备的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="8dbab-248">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="8dbab-249">只读。</span><span class="sxs-lookup"><span data-stu-id="8dbab-249">Read only.</span></span> <span data-ttu-id="8dbab-250">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8dbab-250">This property is read-only.</span></span>|
|<span data-ttu-id="8dbab-251">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="8dbab-251">azureADDeviceId</span></span>|<span data-ttu-id="8dbab-252">String</span><span class="sxs-lookup"><span data-stu-id="8dbab-252">String</span></span>|<span data-ttu-id="8dbab-253">Azure Active Directory 设备的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="8dbab-253">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="8dbab-254">只读。</span><span class="sxs-lookup"><span data-stu-id="8dbab-254">Read only.</span></span> <span data-ttu-id="8dbab-255">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8dbab-255">This property is read-only.</span></span>|
|<span data-ttu-id="8dbab-256">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="8dbab-256">deviceRegistrationState</span></span>|[<span data-ttu-id="8dbab-257">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="8dbab-257">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="8dbab-258">设备注册状态。</span><span class="sxs-lookup"><span data-stu-id="8dbab-258">Device registration state.</span></span> <span data-ttu-id="8dbab-259">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8dbab-259">This property is read-only.</span></span> <span data-ttu-id="8dbab-260">可取值为：`notRegistered`、`registered`、`revoked`、`keyConflict`、`approvalPending`、`certificateReset`、`notRegisteredPendingEnrollment`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="8dbab-260">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="8dbab-261">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="8dbab-261">deviceCategoryDisplayName</span></span>|<span data-ttu-id="8dbab-262">String</span><span class="sxs-lookup"><span data-stu-id="8dbab-262">String</span></span>|<span data-ttu-id="8dbab-263">设备类别显示名称。</span><span class="sxs-lookup"><span data-stu-id="8dbab-263">Device category display name.</span></span> <span data-ttu-id="8dbab-264">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8dbab-264">This property is read-only.</span></span>|
|<span data-ttu-id="8dbab-265">isSupervised</span><span class="sxs-lookup"><span data-stu-id="8dbab-265">isSupervised</span></span>|<span data-ttu-id="8dbab-266">Boolean</span><span class="sxs-lookup"><span data-stu-id="8dbab-266">Boolean</span></span>|<span data-ttu-id="8dbab-267">设备监督状态。</span><span class="sxs-lookup"><span data-stu-id="8dbab-267">Device supervised status.</span></span> <span data-ttu-id="8dbab-268">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8dbab-268">This property is read-only.</span></span>|
|<span data-ttu-id="8dbab-269">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="8dbab-269">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="8dbab-270">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8dbab-270">DateTimeOffset</span></span>|<span data-ttu-id="8dbab-271">设备上次与 Exchange 联系的时间。</span><span class="sxs-lookup"><span data-stu-id="8dbab-271">Last time the device contacted Exchange.</span></span> <span data-ttu-id="8dbab-272">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8dbab-272">This property is read-only.</span></span>|
|<span data-ttu-id="8dbab-273">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="8dbab-273">exchangeAccessState</span></span>|[<span data-ttu-id="8dbab-274">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="8dbab-274">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="8dbab-275">Exchange 中设备的访问状态。</span><span class="sxs-lookup"><span data-stu-id="8dbab-275">The Access State of the device in Exchange.</span></span> <span data-ttu-id="8dbab-276">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8dbab-276">This property is read-only.</span></span> <span data-ttu-id="8dbab-277">可取值为：`none`、`unknown`、`allowed`、`blocked`、`quarantined`。</span><span class="sxs-lookup"><span data-stu-id="8dbab-277">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="8dbab-278">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="8dbab-278">exchangeAccessStateReason</span></span>|[<span data-ttu-id="8dbab-279">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="8dbab-279">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="8dbab-280">Exchange 中设备访问状态的出现原因。</span><span class="sxs-lookup"><span data-stu-id="8dbab-280">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="8dbab-281">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8dbab-281">This property is read-only.</span></span> <span data-ttu-id="8dbab-282">可取值为：`none`、`unknown`、`exchangeGlobalRule`、`exchangeIndividualRule`、`exchangeDeviceRule`、`exchangeUpgrade`、`exchangeMailboxPolicy`、`other`、`compliant`、`notCompliant`、`notEnrolled`、`unknownLocation`、`mfaRequired`、`azureADBlockDueToAccessPolicy`、`compromisedPassword`、`deviceNotKnownWithManagedApp`。</span><span class="sxs-lookup"><span data-stu-id="8dbab-282">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="8dbab-283">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="8dbab-283">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="8dbab-284">String</span><span class="sxs-lookup"><span data-stu-id="8dbab-284">String</span></span>|<span data-ttu-id="8dbab-285">允许与设备建立远程协助会话的 URL。</span><span class="sxs-lookup"><span data-stu-id="8dbab-285">Url that allows a Remote Assistance session to be established with the device.</span></span> <span data-ttu-id="8dbab-286">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8dbab-286">This property is read-only.</span></span>|
|<span data-ttu-id="8dbab-287">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="8dbab-287">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="8dbab-288">String</span><span class="sxs-lookup"><span data-stu-id="8dbab-288">String</span></span>|<span data-ttu-id="8dbab-289">用于在创建远程协助会话对象时识别问题的错误字符串。</span><span class="sxs-lookup"><span data-stu-id="8dbab-289">An error string that identifies issues when creating Remote Assistance session objects.</span></span> <span data-ttu-id="8dbab-290">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8dbab-290">This property is read-only.</span></span>|
|<span data-ttu-id="8dbab-291">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="8dbab-291">isEncrypted</span></span>|<span data-ttu-id="8dbab-292">Boolean</span><span class="sxs-lookup"><span data-stu-id="8dbab-292">Boolean</span></span>|<span data-ttu-id="8dbab-293">设备加密状态。</span><span class="sxs-lookup"><span data-stu-id="8dbab-293">Device encryption status.</span></span> <span data-ttu-id="8dbab-294">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8dbab-294">This property is read-only.</span></span>|
|<span data-ttu-id="8dbab-295">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8dbab-295">userPrincipalName</span></span>|<span data-ttu-id="8dbab-296">String</span><span class="sxs-lookup"><span data-stu-id="8dbab-296">String</span></span>|<span data-ttu-id="8dbab-297">设备用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="8dbab-297">Device user principal name.</span></span> <span data-ttu-id="8dbab-298">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8dbab-298">This property is read-only.</span></span>|
|<span data-ttu-id="8dbab-299">model</span><span class="sxs-lookup"><span data-stu-id="8dbab-299">model</span></span>|<span data-ttu-id="8dbab-300">String</span><span class="sxs-lookup"><span data-stu-id="8dbab-300">String</span></span>|<span data-ttu-id="8dbab-301">设备的模型。</span><span class="sxs-lookup"><span data-stu-id="8dbab-301">Model of the device.</span></span> <span data-ttu-id="8dbab-302">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8dbab-302">This property is read-only.</span></span>|
|<span data-ttu-id="8dbab-303">manufacturer</span><span class="sxs-lookup"><span data-stu-id="8dbab-303">manufacturer</span></span>|<span data-ttu-id="8dbab-304">String</span><span class="sxs-lookup"><span data-stu-id="8dbab-304">String</span></span>|<span data-ttu-id="8dbab-305">设备的制造商。</span><span class="sxs-lookup"><span data-stu-id="8dbab-305">Manufacturer of the device.</span></span> <span data-ttu-id="8dbab-306">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8dbab-306">This property is read-only.</span></span>|
|<span data-ttu-id="8dbab-307">imei</span><span class="sxs-lookup"><span data-stu-id="8dbab-307">imei</span></span>|<span data-ttu-id="8dbab-308">String</span><span class="sxs-lookup"><span data-stu-id="8dbab-308">String</span></span>|<span data-ttu-id="8dbab-309">IMEI.</span><span class="sxs-lookup"><span data-stu-id="8dbab-309">IMEI.</span></span> <span data-ttu-id="8dbab-310">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8dbab-310">This property is read-only.</span></span>|
|<span data-ttu-id="8dbab-311">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="8dbab-311">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="8dbab-312">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8dbab-312">DateTimeOffset</span></span>|<span data-ttu-id="8dbab-313">设备符合性宽限期到期时的日期时间。</span><span class="sxs-lookup"><span data-stu-id="8dbab-313">The DateTime when device compliance grace period expires.</span></span> <span data-ttu-id="8dbab-314">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8dbab-314">This property is read-only.</span></span>|
|<span data-ttu-id="8dbab-315">serialNumber</span><span class="sxs-lookup"><span data-stu-id="8dbab-315">serialNumber</span></span>|<span data-ttu-id="8dbab-316">String</span><span class="sxs-lookup"><span data-stu-id="8dbab-316">String</span></span>|<span data-ttu-id="8dbab-317">SerialNumber.</span><span class="sxs-lookup"><span data-stu-id="8dbab-317">SerialNumber.</span></span> <span data-ttu-id="8dbab-318">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8dbab-318">This property is read-only.</span></span>|
|<span data-ttu-id="8dbab-319">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="8dbab-319">phoneNumber</span></span>|<span data-ttu-id="8dbab-320">String</span><span class="sxs-lookup"><span data-stu-id="8dbab-320">String</span></span>|<span data-ttu-id="8dbab-321">设备的电话号码。</span><span class="sxs-lookup"><span data-stu-id="8dbab-321">Phone number of the device.</span></span> <span data-ttu-id="8dbab-322">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8dbab-322">This property is read-only.</span></span>|
|<span data-ttu-id="8dbab-323">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="8dbab-323">androidSecurityPatchLevel</span></span>|<span data-ttu-id="8dbab-324">String</span><span class="sxs-lookup"><span data-stu-id="8dbab-324">String</span></span>|<span data-ttu-id="8dbab-325">Android 安全修补程序级别。</span><span class="sxs-lookup"><span data-stu-id="8dbab-325">Android security patch level.</span></span> <span data-ttu-id="8dbab-326">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8dbab-326">This property is read-only.</span></span>|
|<span data-ttu-id="8dbab-327">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="8dbab-327">userDisplayName</span></span>|<span data-ttu-id="8dbab-328">String</span><span class="sxs-lookup"><span data-stu-id="8dbab-328">String</span></span>|<span data-ttu-id="8dbab-329">用户显示名称。</span><span class="sxs-lookup"><span data-stu-id="8dbab-329">User display name.</span></span> <span data-ttu-id="8dbab-330">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8dbab-330">This property is read-only.</span></span>|
|<span data-ttu-id="8dbab-331">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="8dbab-331">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="8dbab-332">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="8dbab-332">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="8dbab-333">ConfigrMgr 客户端启用的功能。</span><span class="sxs-lookup"><span data-stu-id="8dbab-333">ConfigrMgr client enabled features.</span></span> <span data-ttu-id="8dbab-334">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8dbab-334">This property is read-only.</span></span>|
|<span data-ttu-id="8dbab-335">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="8dbab-335">wiFiMacAddress</span></span>|<span data-ttu-id="8dbab-336">String</span><span class="sxs-lookup"><span data-stu-id="8dbab-336">String</span></span>|<span data-ttu-id="8dbab-337">Wi-fi MAC。</span><span class="sxs-lookup"><span data-stu-id="8dbab-337">Wi-Fi MAC.</span></span> <span data-ttu-id="8dbab-338">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8dbab-338">This property is read-only.</span></span>|
|<span data-ttu-id="8dbab-339">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="8dbab-339">deviceHealthAttestationState</span></span>|[<span data-ttu-id="8dbab-340">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="8dbab-340">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="8dbab-341">设备运行状况证明状态。</span><span class="sxs-lookup"><span data-stu-id="8dbab-341">The device health attestation state.</span></span> <span data-ttu-id="8dbab-342">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8dbab-342">This property is read-only.</span></span>|
|<span data-ttu-id="8dbab-343">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="8dbab-343">subscriberCarrier</span></span>|<span data-ttu-id="8dbab-344">String</span><span class="sxs-lookup"><span data-stu-id="8dbab-344">String</span></span>|<span data-ttu-id="8dbab-345">订阅者运营商。</span><span class="sxs-lookup"><span data-stu-id="8dbab-345">Subscriber Carrier.</span></span> <span data-ttu-id="8dbab-346">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8dbab-346">This property is read-only.</span></span>|
|<span data-ttu-id="8dbab-347">meid</span><span class="sxs-lookup"><span data-stu-id="8dbab-347">meid</span></span>|<span data-ttu-id="8dbab-348">String</span><span class="sxs-lookup"><span data-stu-id="8dbab-348">String</span></span>|<span data-ttu-id="8dbab-349">MEID.</span><span class="sxs-lookup"><span data-stu-id="8dbab-349">MEID.</span></span> <span data-ttu-id="8dbab-350">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8dbab-350">This property is read-only.</span></span>|
|<span data-ttu-id="8dbab-351">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="8dbab-351">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="8dbab-352">Int64</span><span class="sxs-lookup"><span data-stu-id="8dbab-352">Int64</span></span>|<span data-ttu-id="8dbab-353">总存储量（以字节为单位）。</span><span class="sxs-lookup"><span data-stu-id="8dbab-353">Total Storage in Bytes.</span></span> <span data-ttu-id="8dbab-354">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8dbab-354">This property is read-only.</span></span>|
|<span data-ttu-id="8dbab-355">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="8dbab-355">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="8dbab-356">Int64</span><span class="sxs-lookup"><span data-stu-id="8dbab-356">Int64</span></span>|<span data-ttu-id="8dbab-357">以字节为单位的可用存储空间。</span><span class="sxs-lookup"><span data-stu-id="8dbab-357">Free Storage in Bytes.</span></span> <span data-ttu-id="8dbab-358">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8dbab-358">This property is read-only.</span></span>|
|<span data-ttu-id="8dbab-359">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="8dbab-359">managedDeviceName</span></span>|<span data-ttu-id="8dbab-360">String</span><span class="sxs-lookup"><span data-stu-id="8dbab-360">String</span></span>|<span data-ttu-id="8dbab-361">用于识别设备的自动生成的名称。</span><span class="sxs-lookup"><span data-stu-id="8dbab-361">Automatically generated name to identify a device.</span></span> <span data-ttu-id="8dbab-362">可以覆盖为用户友好名称。</span><span class="sxs-lookup"><span data-stu-id="8dbab-362">Can be overwritten to a user friendly name.</span></span>|
|<span data-ttu-id="8dbab-363">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="8dbab-363">partnerReportedThreatState</span></span>|[<span data-ttu-id="8dbab-364">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="8dbab-364">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="8dbab-365">指示帐户和设备正在使用移动威胁防护合作伙伴时设备的威胁状态。</span><span class="sxs-lookup"><span data-stu-id="8dbab-365">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="8dbab-366">只读。</span><span class="sxs-lookup"><span data-stu-id="8dbab-366">Read Only.</span></span> <span data-ttu-id="8dbab-367">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8dbab-367">This property is read-only.</span></span> <span data-ttu-id="8dbab-368">可取值为：`unknown`、`activated`、`deactivated`、`secured`、`lowSeverity`、`mediumSeverity`、`highSeverity`、`unresponsive`、`compromised`、`misconfigured`。</span><span class="sxs-lookup"><span data-stu-id="8dbab-368">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="8dbab-369">retireAfterDateTime</span><span class="sxs-lookup"><span data-stu-id="8dbab-369">retireAfterDateTime</span></span>|<span data-ttu-id="8dbab-370">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8dbab-370">DateTimeOffset</span></span>|<span data-ttu-id="8dbab-371">指示当设备因计划操作而自动停用的时间。</span><span class="sxs-lookup"><span data-stu-id="8dbab-371">Indicates the time after when a device will be auto retired because of scheduled action.</span></span> <span data-ttu-id="8dbab-372">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8dbab-372">This property is read-only.</span></span>|
|<span data-ttu-id="8dbab-373">usersLoggedOn</span><span class="sxs-lookup"><span data-stu-id="8dbab-373">usersLoggedOn</span></span>|<span data-ttu-id="8dbab-374">[loggedOnUser](../resources/intune-devices-loggedonuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8dbab-374">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="8dbab-375">指示设备的上次登录用户。</span><span class="sxs-lookup"><span data-stu-id="8dbab-375">Indicates the last logged on users of a device.</span></span> <span data-ttu-id="8dbab-376">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8dbab-376">This property is read-only.</span></span>|
|<span data-ttu-id="8dbab-377">preferMdmOverGroupPolicyAppliedDateTime</span><span class="sxs-lookup"><span data-stu-id="8dbab-377">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="8dbab-378">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8dbab-378">DateTimeOffset</span></span>|<span data-ttu-id="8dbab-379">报告设置了 preferMdmOverGroupPolicy 设置的 DateTime。</span><span class="sxs-lookup"><span data-stu-id="8dbab-379">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="8dbab-380">设置后，如果存在冲突，Intune MDM 设置将覆盖组策略设置。</span><span class="sxs-lookup"><span data-stu-id="8dbab-380">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="8dbab-381">只读。</span><span class="sxs-lookup"><span data-stu-id="8dbab-381">Read Only.</span></span> <span data-ttu-id="8dbab-382">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8dbab-382">This property is read-only.</span></span>|
|<span data-ttu-id="8dbab-383">autopilotEnrolled</span><span class="sxs-lookup"><span data-stu-id="8dbab-383">autopilotEnrolled</span></span>|<span data-ttu-id="8dbab-384">Boolean</span><span class="sxs-lookup"><span data-stu-id="8dbab-384">Boolean</span></span>|<span data-ttu-id="8dbab-385">如果托管设备是通过自动引导注册的，则报告。</span><span class="sxs-lookup"><span data-stu-id="8dbab-385">Reports if the managed device is enrolled via auto-pilot.</span></span> <span data-ttu-id="8dbab-386">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8dbab-386">This property is read-only.</span></span>|
|<span data-ttu-id="8dbab-387">requireUserEnrollmentApproval</span><span class="sxs-lookup"><span data-stu-id="8dbab-387">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="8dbab-388">Boolean</span><span class="sxs-lookup"><span data-stu-id="8dbab-388">Boolean</span></span>|<span data-ttu-id="8dbab-389">如果托管 iOS 设备是用户审批注册，则报告。</span><span class="sxs-lookup"><span data-stu-id="8dbab-389">Reports if the managed iOS device is user approval enrollment.</span></span> <span data-ttu-id="8dbab-390">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8dbab-390">This property is read-only.</span></span>|
|<span data-ttu-id="8dbab-391">managementCertificateExpirationDate</span><span class="sxs-lookup"><span data-stu-id="8dbab-391">managementCertificateExpirationDate</span></span>|<span data-ttu-id="8dbab-392">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8dbab-392">DateTimeOffset</span></span>|<span data-ttu-id="8dbab-393">报告设备管理证书到期日期。</span><span class="sxs-lookup"><span data-stu-id="8dbab-393">Reports device management certificate expiration date.</span></span> <span data-ttu-id="8dbab-394">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8dbab-394">This property is read-only.</span></span>|
|<span data-ttu-id="8dbab-395">iccid</span><span class="sxs-lookup"><span data-stu-id="8dbab-395">iccid</span></span>|<span data-ttu-id="8dbab-396">String</span><span class="sxs-lookup"><span data-stu-id="8dbab-396">String</span></span>|<span data-ttu-id="8dbab-397">集成的电路卡标识符，它是 SIM 卡的唯一标识号。</span><span class="sxs-lookup"><span data-stu-id="8dbab-397">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span> <span data-ttu-id="8dbab-398">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8dbab-398">This property is read-only.</span></span>|
|<span data-ttu-id="8dbab-399">udid</span><span class="sxs-lookup"><span data-stu-id="8dbab-399">udid</span></span>|<span data-ttu-id="8dbab-400">String</span><span class="sxs-lookup"><span data-stu-id="8dbab-400">String</span></span>|<span data-ttu-id="8dbab-401">IOS 和 macOS 设备的唯一设备标识符。</span><span class="sxs-lookup"><span data-stu-id="8dbab-401">Unique Device Identifier for iOS and macOS devices.</span></span> <span data-ttu-id="8dbab-402">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8dbab-402">This property is read-only.</span></span>|
|<span data-ttu-id="8dbab-403">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8dbab-403">roleScopeTagIds</span></span>|<span data-ttu-id="8dbab-404">String 集合</span><span class="sxs-lookup"><span data-stu-id="8dbab-404">String collection</span></span>|<span data-ttu-id="8dbab-405">此设备实例的范围标记 Id 的列表。</span><span class="sxs-lookup"><span data-stu-id="8dbab-405">List of Scope Tag IDs for this Device instance.</span></span>|
|<span data-ttu-id="8dbab-406">windowsActiveMalwareCount</span><span class="sxs-lookup"><span data-stu-id="8dbab-406">windowsActiveMalwareCount</span></span>|<span data-ttu-id="8dbab-407">Int32</span><span class="sxs-lookup"><span data-stu-id="8dbab-407">Int32</span></span>|<span data-ttu-id="8dbab-408">此 windows 设备的活动恶意软件的计数。</span><span class="sxs-lookup"><span data-stu-id="8dbab-408">Count of active malware for this windows device.</span></span> <span data-ttu-id="8dbab-409">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8dbab-409">This property is read-only.</span></span>|
|<span data-ttu-id="8dbab-410">windowsRemediatedMalwareCount</span><span class="sxs-lookup"><span data-stu-id="8dbab-410">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="8dbab-411">Int32</span><span class="sxs-lookup"><span data-stu-id="8dbab-411">Int32</span></span>|<span data-ttu-id="8dbab-412">此 windows 设备的修正的恶意软件的计数。</span><span class="sxs-lookup"><span data-stu-id="8dbab-412">Count of remediated malware for this windows device.</span></span> <span data-ttu-id="8dbab-413">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8dbab-413">This property is read-only.</span></span>|
|<span data-ttu-id="8dbab-414">notes</span><span class="sxs-lookup"><span data-stu-id="8dbab-414">notes</span></span>|<span data-ttu-id="8dbab-415">String</span><span class="sxs-lookup"><span data-stu-id="8dbab-415">String</span></span>|<span data-ttu-id="8dbab-416">IT 管理员创建的设备上的注释</span><span class="sxs-lookup"><span data-stu-id="8dbab-416">Notes on the device created by IT Admin</span></span>|
|<span data-ttu-id="8dbab-417">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="8dbab-417">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="8dbab-418">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="8dbab-418">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="8dbab-419">Configuration manager 客户端运行状况状态，仅对由 MDM/ConfigMgr 代理管理的设备有效</span><span class="sxs-lookup"><span data-stu-id="8dbab-419">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent</span></span>|
|<span data-ttu-id="8dbab-420">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="8dbab-420">configurationManagerClientInformation</span></span>|[<span data-ttu-id="8dbab-421">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="8dbab-421">configurationManagerClientInformation</span></span>](../resources/intune-devices-configurationmanagerclientinformation.md)|<span data-ttu-id="8dbab-422">Configuration manager 客户端信息，仅对受 ConfigMgr 代理管理、duel 管理或三方管理的设备有效</span><span class="sxs-lookup"><span data-stu-id="8dbab-422">Configuration manager client information, valid only for devices managed, duel-managed or tri-managed by ConfigMgr Agent</span></span>|
|<span data-ttu-id="8dbab-423">ethernetMacAddress</span><span class="sxs-lookup"><span data-stu-id="8dbab-423">ethernetMacAddress</span></span>|<span data-ttu-id="8dbab-424">String</span><span class="sxs-lookup"><span data-stu-id="8dbab-424">String</span></span>|<span data-ttu-id="8dbab-425">以太网 MAC。</span><span class="sxs-lookup"><span data-stu-id="8dbab-425">Ethernet MAC.</span></span> <span data-ttu-id="8dbab-426">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8dbab-426">This property is read-only.</span></span>|
|<span data-ttu-id="8dbab-427">physicalMemoryInBytes</span><span class="sxs-lookup"><span data-stu-id="8dbab-427">physicalMemoryInBytes</span></span>|<span data-ttu-id="8dbab-428">Int64</span><span class="sxs-lookup"><span data-stu-id="8dbab-428">Int64</span></span>|<span data-ttu-id="8dbab-429">内存总量（以字节为单位）。</span><span class="sxs-lookup"><span data-stu-id="8dbab-429">Total Memory in Bytes.</span></span> <span data-ttu-id="8dbab-430">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8dbab-430">This property is read-only.</span></span>|
|<span data-ttu-id="8dbab-431">processorArchitecture</span><span class="sxs-lookup"><span data-stu-id="8dbab-431">processorArchitecture</span></span>|[<span data-ttu-id="8dbab-432">managedDeviceArchitecture</span><span class="sxs-lookup"><span data-stu-id="8dbab-432">managedDeviceArchitecture</span></span>](../resources/intune-devices-manageddevicearchitecture.md)|<span data-ttu-id="8dbab-433">处理器体系结构。</span><span class="sxs-lookup"><span data-stu-id="8dbab-433">Processor architecture.</span></span> <span data-ttu-id="8dbab-434">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8dbab-434">This property is read-only.</span></span> <span data-ttu-id="8dbab-435">可取值为：`unknown`、`x86`、`x64`、`arm`、`arM64`。</span><span class="sxs-lookup"><span data-stu-id="8dbab-435">Possible values are: `unknown`, `x86`, `x64`, `arm`, `arM64`.</span></span>|
|<span data-ttu-id="8dbab-436">specificationVersion</span><span class="sxs-lookup"><span data-stu-id="8dbab-436">specificationVersion</span></span>|<span data-ttu-id="8dbab-437">String</span><span class="sxs-lookup"><span data-stu-id="8dbab-437">String</span></span>|<span data-ttu-id="8dbab-438">规范版本。</span><span class="sxs-lookup"><span data-stu-id="8dbab-438">Specification version.</span></span> <span data-ttu-id="8dbab-439">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8dbab-439">This property is read-only.</span></span>|
|<span data-ttu-id="8dbab-440">joinType</span><span class="sxs-lookup"><span data-stu-id="8dbab-440">joinType</span></span>|[<span data-ttu-id="8dbab-441">joinType</span><span class="sxs-lookup"><span data-stu-id="8dbab-441">joinType</span></span>](../resources/intune-devices-jointype.md)|<span data-ttu-id="8dbab-442">设备加入类型。</span><span class="sxs-lookup"><span data-stu-id="8dbab-442">Device join type.</span></span> <span data-ttu-id="8dbab-443">可取值为：`unknown`、`azureADJoined`、`azureADRegistered`、`hybridAzureADJoined`。</span><span class="sxs-lookup"><span data-stu-id="8dbab-443">Possible values are: `unknown`, `azureADJoined`, `azureADRegistered`, `hybridAzureADJoined`.</span></span>|
|<span data-ttu-id="8dbab-444">skuFamily</span><span class="sxs-lookup"><span data-stu-id="8dbab-444">skuFamily</span></span>|<span data-ttu-id="8dbab-445">String</span><span class="sxs-lookup"><span data-stu-id="8dbab-445">String</span></span>|<span data-ttu-id="8dbab-446">设备 sku 系列</span><span class="sxs-lookup"><span data-stu-id="8dbab-446">Device sku family</span></span>|
|<span data-ttu-id="8dbab-447">skuNumber</span><span class="sxs-lookup"><span data-stu-id="8dbab-447">skuNumber</span></span>|<span data-ttu-id="8dbab-448">Int32</span><span class="sxs-lookup"><span data-stu-id="8dbab-448">Int32</span></span>|<span data-ttu-id="8dbab-449">设备 sku 编号，另请参阅： https://docs.microsoft.com/windows/win32/api/sysinfoapi/nf-sysinfoapi-getproductinfo 。</span><span class="sxs-lookup"><span data-stu-id="8dbab-449">Device sku number, see also: https://docs.microsoft.com/windows/win32/api/sysinfoapi/nf-sysinfoapi-getproductinfo.</span></span> <span data-ttu-id="8dbab-450">有效的值为0到2147483647。</span><span class="sxs-lookup"><span data-stu-id="8dbab-450">Valid values 0 to 2147483647.</span></span> <span data-ttu-id="8dbab-451">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8dbab-451">This property is read-only.</span></span>|
|<span data-ttu-id="8dbab-452">managementFeatures</span><span class="sxs-lookup"><span data-stu-id="8dbab-452">managementFeatures</span></span>|[<span data-ttu-id="8dbab-453">managedDeviceManagementFeatures</span><span class="sxs-lookup"><span data-stu-id="8dbab-453">managedDeviceManagementFeatures</span></span>](../resources/intune-devices-manageddevicemanagementfeatures.md)|<span data-ttu-id="8dbab-454">设备管理功能。</span><span class="sxs-lookup"><span data-stu-id="8dbab-454">Device management features.</span></span> <span data-ttu-id="8dbab-455">可取值为：`none`、`microsoftManagedDesktop`。</span><span class="sxs-lookup"><span data-stu-id="8dbab-455">Possible values are: `none`, `microsoftManagedDesktop`.</span></span>|



## <a name="response"></a><span data-ttu-id="8dbab-456">响应</span><span class="sxs-lookup"><span data-stu-id="8dbab-456">Response</span></span>
<span data-ttu-id="8dbab-457">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [managedDevice](../resources/intune-devices-manageddevice.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8dbab-457">If successful, this method returns a `200 OK` response code and an updated [managedDevice](../resources/intune-devices-manageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8dbab-458">示例</span><span class="sxs-lookup"><span data-stu-id="8dbab-458">Example</span></span>

### <a name="request"></a><span data-ttu-id="8dbab-459">请求</span><span class="sxs-lookup"><span data-stu-id="8dbab-459">Request</span></span>
<span data-ttu-id="8dbab-460">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8dbab-460">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}
Content-type: application/json
Content-length: 8019

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
    "batterySerialNumber": "Battery Serial Number value",
    "batteryHealthPercentage": 7,
    "batteryChargeCycles": 3,
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
    "deviceGuardLocalSystemAuthorityCredentialGuardState": "rebootRequired",
    "osBuildNumber": "Os Build Number value",
    "operatingSystemProductType": 10
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
  "retireAfterDateTime": "2016-12-31T23:57:37.576134-08:00",
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
  },
  "configurationManagerClientInformation": {
    "@odata.type": "microsoft.graph.configurationManagerClientInformation",
    "clientIdentifier": "Client Identifier value",
    "isBlocked": true
  },
  "ethernetMacAddress": "Ethernet Mac Address value",
  "physicalMemoryInBytes": 5,
  "processorArchitecture": "x86",
  "specificationVersion": "Specification Version value",
  "joinType": "azureADJoined",
  "skuFamily": "Sku Family value",
  "skuNumber": 9,
  "managementFeatures": "microsoftManagedDesktop"
}
```

### <a name="response"></a><span data-ttu-id="8dbab-461">响应</span><span class="sxs-lookup"><span data-stu-id="8dbab-461">Response</span></span>
<span data-ttu-id="8dbab-p174">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8dbab-p174">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 8068

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
    "batterySerialNumber": "Battery Serial Number value",
    "batteryHealthPercentage": 7,
    "batteryChargeCycles": 3,
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
    "deviceGuardLocalSystemAuthorityCredentialGuardState": "rebootRequired",
    "osBuildNumber": "Os Build Number value",
    "operatingSystemProductType": 10
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
  "retireAfterDateTime": "2016-12-31T23:57:37.576134-08:00",
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
  },
  "configurationManagerClientInformation": {
    "@odata.type": "microsoft.graph.configurationManagerClientInformation",
    "clientIdentifier": "Client Identifier value",
    "isBlocked": true
  },
  "ethernetMacAddress": "Ethernet Mac Address value",
  "physicalMemoryInBytes": 5,
  "processorArchitecture": "x86",
  "specificationVersion": "Specification Version value",
  "joinType": "azureADJoined",
  "skuFamily": "Sku Family value",
  "skuNumber": 9,
  "managementFeatures": "microsoftManagedDesktop"
}
```






