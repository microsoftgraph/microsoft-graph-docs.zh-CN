---
title: 更新 managedDevice
description: 更新 managedDevice 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 78db2a2308cbd664c2d711b0103ad94812a48fde
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52664942"
---
# <a name="update-manageddevice"></a><span data-ttu-id="5ee01-103">更新 managedDevice</span><span class="sxs-lookup"><span data-stu-id="5ee01-103">Update managedDevice</span></span>

<span data-ttu-id="5ee01-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ee01-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5ee01-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5ee01-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5ee01-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5ee01-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5ee01-107">更新 [managedDevice](../resources/intune-devices-manageddevice.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5ee01-107">Update the properties of a [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5ee01-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="5ee01-108">Prerequisites</span></span>
<span data-ttu-id="5ee01-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5ee01-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ee01-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="5ee01-111">Permission type</span></span>|<span data-ttu-id="5ee01-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5ee01-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5ee01-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5ee01-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5ee01-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ee01-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="5ee01-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5ee01-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5ee01-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5ee01-116">Not supported.</span></span>|
|<span data-ttu-id="5ee01-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="5ee01-117">Application</span></span>|<span data-ttu-id="5ee01-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ee01-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5ee01-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5ee01-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="5ee01-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="5ee01-120">Request headers</span></span>
|<span data-ttu-id="5ee01-121">标头</span><span class="sxs-lookup"><span data-stu-id="5ee01-121">Header</span></span>|<span data-ttu-id="5ee01-122">值</span><span class="sxs-lookup"><span data-stu-id="5ee01-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5ee01-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5ee01-123">Authorization</span></span>|<span data-ttu-id="5ee01-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5ee01-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5ee01-125">接受</span><span class="sxs-lookup"><span data-stu-id="5ee01-125">Accept</span></span>|<span data-ttu-id="5ee01-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5ee01-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5ee01-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="5ee01-127">Request body</span></span>
<span data-ttu-id="5ee01-128">在请求正文中，提供 [managedDevice](../resources/intune-devices-manageddevice.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5ee01-128">In the request body, supply a JSON representation for the [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>

<span data-ttu-id="5ee01-129">下表显示创建 [managedDevice](../resources/intune-devices-manageddevice.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="5ee01-129">The following table shows the properties that are required when you create the [managedDevice](../resources/intune-devices-manageddevice.md).</span></span>

|<span data-ttu-id="5ee01-130">属性</span><span class="sxs-lookup"><span data-stu-id="5ee01-130">Property</span></span>|<span data-ttu-id="5ee01-131">类型</span><span class="sxs-lookup"><span data-stu-id="5ee01-131">Type</span></span>|<span data-ttu-id="5ee01-132">说明</span><span class="sxs-lookup"><span data-stu-id="5ee01-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ee01-133">id</span><span class="sxs-lookup"><span data-stu-id="5ee01-133">id</span></span>|<span data-ttu-id="5ee01-134">String</span><span class="sxs-lookup"><span data-stu-id="5ee01-134">String</span></span>|<span data-ttu-id="5ee01-135">设备的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="5ee01-135">Unique Identifier for the device.</span></span> <span data-ttu-id="5ee01-136">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5ee01-136">This property is read-only.</span></span>|
|<span data-ttu-id="5ee01-137">userId</span><span class="sxs-lookup"><span data-stu-id="5ee01-137">userId</span></span>|<span data-ttu-id="5ee01-138">String</span><span class="sxs-lookup"><span data-stu-id="5ee01-138">String</span></span>|<span data-ttu-id="5ee01-139">与设备关联的用户的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="5ee01-139">Unique Identifier for the user associated with the device.</span></span> <span data-ttu-id="5ee01-140">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5ee01-140">This property is read-only.</span></span>|
|<span data-ttu-id="5ee01-141">deviceName</span><span class="sxs-lookup"><span data-stu-id="5ee01-141">deviceName</span></span>|<span data-ttu-id="5ee01-142">String</span><span class="sxs-lookup"><span data-stu-id="5ee01-142">String</span></span>|<span data-ttu-id="5ee01-143">设备的名称。</span><span class="sxs-lookup"><span data-stu-id="5ee01-143">Name of the device.</span></span> <span data-ttu-id="5ee01-144">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5ee01-144">This property is read-only.</span></span>|
|<span data-ttu-id="5ee01-145">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="5ee01-145">hardwareInformation</span></span>|[<span data-ttu-id="5ee01-146">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="5ee01-146">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="5ee01-147">设备的硬向详细信息。</span><span class="sxs-lookup"><span data-stu-id="5ee01-147">The hardward details for the device.</span></span>  <span data-ttu-id="5ee01-148">包括存储空间、制造商、序列号等信息。此属性为只读。</span><span class="sxs-lookup"><span data-stu-id="5ee01-148">Includes information such as storage space, manufacturer, serial number, etc. This property is read-only.</span></span>|
|<span data-ttu-id="5ee01-149">ownerType</span><span class="sxs-lookup"><span data-stu-id="5ee01-149">ownerType</span></span>|[<span data-ttu-id="5ee01-150">ownerType</span><span class="sxs-lookup"><span data-stu-id="5ee01-150">ownerType</span></span>](../resources/intune-shared-ownertype.md)|<span data-ttu-id="5ee01-151">设备的所有权。</span><span class="sxs-lookup"><span data-stu-id="5ee01-151">Ownership of the device.</span></span> <span data-ttu-id="5ee01-152">可以是"公司"或"个人"。</span><span class="sxs-lookup"><span data-stu-id="5ee01-152">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="5ee01-153">可取值为：`unknown`、`company`、`personal`。</span><span class="sxs-lookup"><span data-stu-id="5ee01-153">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="5ee01-154">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="5ee01-154">managedDeviceOwnerType</span></span>|[<span data-ttu-id="5ee01-155">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="5ee01-155">managedDeviceOwnerType</span></span>](../resources/intune-shared-manageddeviceownertype.md)|<span data-ttu-id="5ee01-156">设备的所有权。</span><span class="sxs-lookup"><span data-stu-id="5ee01-156">Ownership of the device.</span></span> <span data-ttu-id="5ee01-157">可以是"公司"或"个人"。</span><span class="sxs-lookup"><span data-stu-id="5ee01-157">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="5ee01-158">可取值为：`unknown`、`company`、`personal`。</span><span class="sxs-lookup"><span data-stu-id="5ee01-158">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="5ee01-159">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="5ee01-159">deviceActionResults</span></span>|<span data-ttu-id="5ee01-160">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5ee01-160">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="5ee01-161">ComplexType deviceActionResult 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="5ee01-161">List of ComplexType deviceActionResult objects.</span></span> <span data-ttu-id="5ee01-162">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5ee01-162">This property is read-only.</span></span>|
|<span data-ttu-id="5ee01-163">managementState</span><span class="sxs-lookup"><span data-stu-id="5ee01-163">managementState</span></span>|[<span data-ttu-id="5ee01-164">managementState</span><span class="sxs-lookup"><span data-stu-id="5ee01-164">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="5ee01-165">设备的管理状态。</span><span class="sxs-lookup"><span data-stu-id="5ee01-165">Management state of the device.</span></span> <span data-ttu-id="5ee01-166">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5ee01-166">This property is read-only.</span></span> <span data-ttu-id="5ee01-167">可取值为：`managed`、`retirePending`、`retireFailed`、`wipePending`、`wipeFailed`、`unhealthy`、`deletePending`、`retireIssued`、`wipeIssued`、`wipeCanceled`、`retireCanceled`、`discovered`。</span><span class="sxs-lookup"><span data-stu-id="5ee01-167">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="5ee01-168">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="5ee01-168">enrolledDateTime</span></span>|<span data-ttu-id="5ee01-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ee01-169">DateTimeOffset</span></span>|<span data-ttu-id="5ee01-170">设备的注册时间。</span><span class="sxs-lookup"><span data-stu-id="5ee01-170">Enrollment time of the device.</span></span> <span data-ttu-id="5ee01-171">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5ee01-171">This property is read-only.</span></span>|
|<span data-ttu-id="5ee01-172">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="5ee01-172">lastSyncDateTime</span></span>|<span data-ttu-id="5ee01-173">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ee01-173">DateTimeOffset</span></span>|<span data-ttu-id="5ee01-174">设备上次成功完成与 Intune 同步的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="5ee01-174">The date and time that the device last completed a successful sync with Intune.</span></span> <span data-ttu-id="5ee01-175">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5ee01-175">This property is read-only.</span></span>|
|<span data-ttu-id="5ee01-176">chassisType</span><span class="sxs-lookup"><span data-stu-id="5ee01-176">chassisType</span></span>|[<span data-ttu-id="5ee01-177">chassisType</span><span class="sxs-lookup"><span data-stu-id="5ee01-177">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="5ee01-178">设备的机架类型。</span><span class="sxs-lookup"><span data-stu-id="5ee01-178">Chassis type of the device.</span></span> <span data-ttu-id="5ee01-179">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5ee01-179">This property is read-only.</span></span> <span data-ttu-id="5ee01-180">可取值为：`unknown`、`desktop`、`laptop`、`worksWorkstation`、`enterpriseServer`、`phone`、`tablet`、`mobileOther`、`mobileUnknown`。</span><span class="sxs-lookup"><span data-stu-id="5ee01-180">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="5ee01-181">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="5ee01-181">operatingSystem</span></span>|<span data-ttu-id="5ee01-182">String</span><span class="sxs-lookup"><span data-stu-id="5ee01-182">String</span></span>|<span data-ttu-id="5ee01-183">设备的操作系统。</span><span class="sxs-lookup"><span data-stu-id="5ee01-183">Operating system of the device.</span></span> <span data-ttu-id="5ee01-184">Windows、iOS 等。此属性为只读。</span><span class="sxs-lookup"><span data-stu-id="5ee01-184">Windows, iOS, etc. This property is read-only.</span></span>|
|<span data-ttu-id="5ee01-185">deviceType</span><span class="sxs-lookup"><span data-stu-id="5ee01-185">deviceType</span></span>|[<span data-ttu-id="5ee01-186">deviceType</span><span class="sxs-lookup"><span data-stu-id="5ee01-186">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="5ee01-187">设备平台。</span><span class="sxs-lookup"><span data-stu-id="5ee01-187">Platform of the device.</span></span> <span data-ttu-id="5ee01-188">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5ee01-188">This property is read-only.</span></span> <span data-ttu-id="5ee01-189">可能的值是 `desktop` `windowsRT` `winMO6` ：、、、、、、、、、、 `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `windows10x` `androidnGMS` `chromeOS` `linux` `blackberry` `palm` `unknown` `cloudPC` 、</span><span class="sxs-lookup"><span data-stu-id="5ee01-189">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `androidnGMS`, `chromeOS`, `linux`, `blackberry`, `palm`, `unknown`, `cloudPC`.</span></span>|
|<span data-ttu-id="5ee01-190">complianceState</span><span class="sxs-lookup"><span data-stu-id="5ee01-190">complianceState</span></span>|[<span data-ttu-id="5ee01-191">complianceState</span><span class="sxs-lookup"><span data-stu-id="5ee01-191">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="5ee01-192">设备的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="5ee01-192">Compliance state of the device.</span></span> <span data-ttu-id="5ee01-193">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5ee01-193">This property is read-only.</span></span> <span data-ttu-id="5ee01-194">可取值为：`unknown`、`compliant`、`noncompliant`、`conflict`、`error`、`inGracePeriod`、`configManager`。</span><span class="sxs-lookup"><span data-stu-id="5ee01-194">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="5ee01-195">jailBroken</span><span class="sxs-lookup"><span data-stu-id="5ee01-195">jailBroken</span></span>|<span data-ttu-id="5ee01-196">String</span><span class="sxs-lookup"><span data-stu-id="5ee01-196">String</span></span>|<span data-ttu-id="5ee01-197">设备是否已越狱或取得 root 权限。</span><span class="sxs-lookup"><span data-stu-id="5ee01-197">whether the device is jail broken or rooted.</span></span> <span data-ttu-id="5ee01-198">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5ee01-198">This property is read-only.</span></span>|
|<span data-ttu-id="5ee01-199">managementAgent</span><span class="sxs-lookup"><span data-stu-id="5ee01-199">managementAgent</span></span>|[<span data-ttu-id="5ee01-200">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="5ee01-200">managementAgentType</span></span>](../resources/intune-shared-managementagenttype.md)|<span data-ttu-id="5ee01-201">设备的管理通道。</span><span class="sxs-lookup"><span data-stu-id="5ee01-201">Management channel of the device.</span></span> <span data-ttu-id="5ee01-202">Intune、EAS 等此属性为只读。</span><span class="sxs-lookup"><span data-stu-id="5ee01-202">Intune, EAS, etc. This property is read-only.</span></span> <span data-ttu-id="5ee01-203">可能的值是 `eas` `mdm` `easMdm` ：、、、、、、、、、、 `intuneClient` `easIntuneClient` `configurationManagerClient` `configurationManagerClientMdm` `configurationManagerClientMdmEas` `unknown` `jamf` `googleCloudDevicePolicyController` `microsoft365ManagedMdm` `msSense` `intuneAosp` 。</span><span class="sxs-lookup"><span data-stu-id="5ee01-203">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`, `msSense`, `intuneAosp`.</span></span>|
|<span data-ttu-id="5ee01-204">osVersion</span><span class="sxs-lookup"><span data-stu-id="5ee01-204">osVersion</span></span>|<span data-ttu-id="5ee01-205">String</span><span class="sxs-lookup"><span data-stu-id="5ee01-205">String</span></span>|<span data-ttu-id="5ee01-206">设备的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="5ee01-206">Operating system version of the device.</span></span> <span data-ttu-id="5ee01-207">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5ee01-207">This property is read-only.</span></span>|
|<span data-ttu-id="5ee01-208">easActivated</span><span class="sxs-lookup"><span data-stu-id="5ee01-208">easActivated</span></span>|<span data-ttu-id="5ee01-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="5ee01-209">Boolean</span></span>|<span data-ttu-id="5ee01-210">设备是否已激活 Exchange ActiveSync。</span><span class="sxs-lookup"><span data-stu-id="5ee01-210">Whether the device is Exchange ActiveSync activated.</span></span> <span data-ttu-id="5ee01-211">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5ee01-211">This property is read-only.</span></span>|
|<span data-ttu-id="5ee01-212">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="5ee01-212">easDeviceId</span></span>|<span data-ttu-id="5ee01-213">String</span><span class="sxs-lookup"><span data-stu-id="5ee01-213">String</span></span>|<span data-ttu-id="5ee01-214">设备的 Exchange ActiveSync ID。</span><span class="sxs-lookup"><span data-stu-id="5ee01-214">Exchange ActiveSync Id of the device.</span></span> <span data-ttu-id="5ee01-215">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5ee01-215">This property is read-only.</span></span>|
|<span data-ttu-id="5ee01-216">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="5ee01-216">easActivationDateTime</span></span>|<span data-ttu-id="5ee01-217">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ee01-217">DateTimeOffset</span></span>|<span data-ttu-id="5ee01-218">设备的 Exchange ActivationSync 激活时间。</span><span class="sxs-lookup"><span data-stu-id="5ee01-218">Exchange ActivationSync activation time of the device.</span></span> <span data-ttu-id="5ee01-219">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5ee01-219">This property is read-only.</span></span>|
|<span data-ttu-id="5ee01-220">aadRegistered</span><span class="sxs-lookup"><span data-stu-id="5ee01-220">aadRegistered</span></span>|<span data-ttu-id="5ee01-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="5ee01-221">Boolean</span></span>|<span data-ttu-id="5ee01-222">设备是否已注册 Azure Active Directory。</span><span class="sxs-lookup"><span data-stu-id="5ee01-222">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="5ee01-223">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5ee01-223">This property is read-only.</span></span>|
|<span data-ttu-id="5ee01-224">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="5ee01-224">azureADRegistered</span></span>|<span data-ttu-id="5ee01-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="5ee01-225">Boolean</span></span>|<span data-ttu-id="5ee01-226">设备是否已注册 Azure Active Directory。</span><span class="sxs-lookup"><span data-stu-id="5ee01-226">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="5ee01-227">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5ee01-227">This property is read-only.</span></span>|
|<span data-ttu-id="5ee01-228">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="5ee01-228">deviceEnrollmentType</span></span>|[<span data-ttu-id="5ee01-229">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="5ee01-229">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="5ee01-230">设备的注册类型。</span><span class="sxs-lookup"><span data-stu-id="5ee01-230">Enrollment type of the device.</span></span> <span data-ttu-id="5ee01-231">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5ee01-231">This property is read-only.</span></span> <span data-ttu-id="5ee01-232">可能的值是 `unknown` `userEnrollment` `deviceEnrollmentManager` ：、、、、、、、、、 `appleBulkWithUser` `appleBulkWithoutUser` `windowsAzureADJoin` `windowsBulkUserless` `windowsAutoEnrollment` `windowsBulkAzureDomainJoin` `windowsCoManagement` `windowsAzureADJoinUsingDeviceAuth` `appleUserEnrollment` `appleUserEnrollmentWithServiceAccount` `azureAdJoinUsingAzureVmExtension` `androidEnterpriseDedicatedDevice` `androidEnterpriseFullyManaged` `androidEnterpriseCorporateWorkProfile` 。</span><span class="sxs-lookup"><span data-stu-id="5ee01-232">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `windowsAzureADJoinUsingDeviceAuth`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`, `azureAdJoinUsingAzureVmExtension`, `androidEnterpriseDedicatedDevice`, `androidEnterpriseFullyManaged`, `androidEnterpriseCorporateWorkProfile`.</span></span>|
|<span data-ttu-id="5ee01-233">lostModeState</span><span class="sxs-lookup"><span data-stu-id="5ee01-233">lostModeState</span></span>|[<span data-ttu-id="5ee01-234">lostModeState</span><span class="sxs-lookup"><span data-stu-id="5ee01-234">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="5ee01-235">指示是启用还是禁用丢失模式。</span><span class="sxs-lookup"><span data-stu-id="5ee01-235">Indicates if Lost mode is enabled or disabled.</span></span> <span data-ttu-id="5ee01-236">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5ee01-236">This property is read-only.</span></span> <span data-ttu-id="5ee01-237">可取值为：`disabled`、`enabled`。</span><span class="sxs-lookup"><span data-stu-id="5ee01-237">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="5ee01-238">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="5ee01-238">activationLockBypassCode</span></span>|<span data-ttu-id="5ee01-239">String</span><span class="sxs-lookup"><span data-stu-id="5ee01-239">String</span></span>|<span data-ttu-id="5ee01-240">允许绕过设备上的激活锁的代码。</span><span class="sxs-lookup"><span data-stu-id="5ee01-240">Code that allows the Activation Lock on a device to be bypassed.</span></span> <span data-ttu-id="5ee01-241">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5ee01-241">This property is read-only.</span></span>|
|<span data-ttu-id="5ee01-242">emailAddress</span><span class="sxs-lookup"><span data-stu-id="5ee01-242">emailAddress</span></span>|<span data-ttu-id="5ee01-243">String</span><span class="sxs-lookup"><span data-stu-id="5ee01-243">String</span></span>|<span data-ttu-id="5ee01-244">电子邮件 () 设备关联的用户的邮箱。</span><span class="sxs-lookup"><span data-stu-id="5ee01-244">Email(s) for the user associated with the device.</span></span> <span data-ttu-id="5ee01-245">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5ee01-245">This property is read-only.</span></span>|
|<span data-ttu-id="5ee01-246">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="5ee01-246">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="5ee01-247">String</span><span class="sxs-lookup"><span data-stu-id="5ee01-247">String</span></span>|<span data-ttu-id="5ee01-248">Azure Active Directory 设备的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="5ee01-248">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="5ee01-249">只读。</span><span class="sxs-lookup"><span data-stu-id="5ee01-249">Read only.</span></span> <span data-ttu-id="5ee01-250">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5ee01-250">This property is read-only.</span></span>|
|<span data-ttu-id="5ee01-251">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="5ee01-251">azureADDeviceId</span></span>|<span data-ttu-id="5ee01-252">String</span><span class="sxs-lookup"><span data-stu-id="5ee01-252">String</span></span>|<span data-ttu-id="5ee01-253">Azure Active Directory 设备的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="5ee01-253">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="5ee01-254">只读。</span><span class="sxs-lookup"><span data-stu-id="5ee01-254">Read only.</span></span> <span data-ttu-id="5ee01-255">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5ee01-255">This property is read-only.</span></span>|
|<span data-ttu-id="5ee01-256">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="5ee01-256">deviceRegistrationState</span></span>|[<span data-ttu-id="5ee01-257">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="5ee01-257">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="5ee01-258">设备注册状态。</span><span class="sxs-lookup"><span data-stu-id="5ee01-258">Device registration state.</span></span> <span data-ttu-id="5ee01-259">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5ee01-259">This property is read-only.</span></span> <span data-ttu-id="5ee01-260">可取值为：`notRegistered`、`registered`、`revoked`、`keyConflict`、`approvalPending`、`certificateReset`、`notRegisteredPendingEnrollment`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="5ee01-260">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="5ee01-261">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="5ee01-261">deviceCategoryDisplayName</span></span>|<span data-ttu-id="5ee01-262">String</span><span class="sxs-lookup"><span data-stu-id="5ee01-262">String</span></span>|<span data-ttu-id="5ee01-263">设备类别显示名称。</span><span class="sxs-lookup"><span data-stu-id="5ee01-263">Device category display name.</span></span> <span data-ttu-id="5ee01-264">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5ee01-264">This property is read-only.</span></span>|
|<span data-ttu-id="5ee01-265">isSupervised</span><span class="sxs-lookup"><span data-stu-id="5ee01-265">isSupervised</span></span>|<span data-ttu-id="5ee01-266">Boolean</span><span class="sxs-lookup"><span data-stu-id="5ee01-266">Boolean</span></span>|<span data-ttu-id="5ee01-267">设备监督状态。</span><span class="sxs-lookup"><span data-stu-id="5ee01-267">Device supervised status.</span></span> <span data-ttu-id="5ee01-268">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5ee01-268">This property is read-only.</span></span>|
|<span data-ttu-id="5ee01-269">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="5ee01-269">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="5ee01-270">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ee01-270">DateTimeOffset</span></span>|<span data-ttu-id="5ee01-271">设备上次与 Exchange 联系的时间。</span><span class="sxs-lookup"><span data-stu-id="5ee01-271">Last time the device contacted Exchange.</span></span> <span data-ttu-id="5ee01-272">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5ee01-272">This property is read-only.</span></span>|
|<span data-ttu-id="5ee01-273">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="5ee01-273">exchangeAccessState</span></span>|[<span data-ttu-id="5ee01-274">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="5ee01-274">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="5ee01-275">Exchange 中设备的访问状态。</span><span class="sxs-lookup"><span data-stu-id="5ee01-275">The Access State of the device in Exchange.</span></span> <span data-ttu-id="5ee01-276">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5ee01-276">This property is read-only.</span></span> <span data-ttu-id="5ee01-277">可取值为：`none`、`unknown`、`allowed`、`blocked`、`quarantined`。</span><span class="sxs-lookup"><span data-stu-id="5ee01-277">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="5ee01-278">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="5ee01-278">exchangeAccessStateReason</span></span>|[<span data-ttu-id="5ee01-279">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="5ee01-279">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="5ee01-280">Exchange 中设备访问状态的出现原因。</span><span class="sxs-lookup"><span data-stu-id="5ee01-280">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="5ee01-281">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5ee01-281">This property is read-only.</span></span> <span data-ttu-id="5ee01-282">可取值为：`none`、`unknown`、`exchangeGlobalRule`、`exchangeIndividualRule`、`exchangeDeviceRule`、`exchangeUpgrade`、`exchangeMailboxPolicy`、`other`、`compliant`、`notCompliant`、`notEnrolled`、`unknownLocation`、`mfaRequired`、`azureADBlockDueToAccessPolicy`、`compromisedPassword`、`deviceNotKnownWithManagedApp`。</span><span class="sxs-lookup"><span data-stu-id="5ee01-282">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="5ee01-283">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="5ee01-283">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="5ee01-284">String</span><span class="sxs-lookup"><span data-stu-id="5ee01-284">String</span></span>|<span data-ttu-id="5ee01-285">允许与设备建立远程协助会话的 URL。</span><span class="sxs-lookup"><span data-stu-id="5ee01-285">Url that allows a Remote Assistance session to be established with the device.</span></span> <span data-ttu-id="5ee01-286">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5ee01-286">This property is read-only.</span></span>|
|<span data-ttu-id="5ee01-287">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="5ee01-287">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="5ee01-288">String</span><span class="sxs-lookup"><span data-stu-id="5ee01-288">String</span></span>|<span data-ttu-id="5ee01-289">用于在创建远程协助会话对象时识别问题的错误字符串。</span><span class="sxs-lookup"><span data-stu-id="5ee01-289">An error string that identifies issues when creating Remote Assistance session objects.</span></span> <span data-ttu-id="5ee01-290">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5ee01-290">This property is read-only.</span></span>|
|<span data-ttu-id="5ee01-291">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="5ee01-291">isEncrypted</span></span>|<span data-ttu-id="5ee01-292">Boolean</span><span class="sxs-lookup"><span data-stu-id="5ee01-292">Boolean</span></span>|<span data-ttu-id="5ee01-293">设备加密状态。</span><span class="sxs-lookup"><span data-stu-id="5ee01-293">Device encryption status.</span></span> <span data-ttu-id="5ee01-294">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5ee01-294">This property is read-only.</span></span>|
|<span data-ttu-id="5ee01-295">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="5ee01-295">userPrincipalName</span></span>|<span data-ttu-id="5ee01-296">String</span><span class="sxs-lookup"><span data-stu-id="5ee01-296">String</span></span>|<span data-ttu-id="5ee01-297">设备用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="5ee01-297">Device user principal name.</span></span> <span data-ttu-id="5ee01-298">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5ee01-298">This property is read-only.</span></span>|
|<span data-ttu-id="5ee01-299">model</span><span class="sxs-lookup"><span data-stu-id="5ee01-299">model</span></span>|<span data-ttu-id="5ee01-300">String</span><span class="sxs-lookup"><span data-stu-id="5ee01-300">String</span></span>|<span data-ttu-id="5ee01-301">设备型号。</span><span class="sxs-lookup"><span data-stu-id="5ee01-301">Model of the device.</span></span> <span data-ttu-id="5ee01-302">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5ee01-302">This property is read-only.</span></span>|
|<span data-ttu-id="5ee01-303">manufacturer</span><span class="sxs-lookup"><span data-stu-id="5ee01-303">manufacturer</span></span>|<span data-ttu-id="5ee01-304">String</span><span class="sxs-lookup"><span data-stu-id="5ee01-304">String</span></span>|<span data-ttu-id="5ee01-305">设备的制造商。</span><span class="sxs-lookup"><span data-stu-id="5ee01-305">Manufacturer of the device.</span></span> <span data-ttu-id="5ee01-306">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5ee01-306">This property is read-only.</span></span>|
|<span data-ttu-id="5ee01-307">imei</span><span class="sxs-lookup"><span data-stu-id="5ee01-307">imei</span></span>|<span data-ttu-id="5ee01-308">String</span><span class="sxs-lookup"><span data-stu-id="5ee01-308">String</span></span>|<span data-ttu-id="5ee01-309">IMEI。</span><span class="sxs-lookup"><span data-stu-id="5ee01-309">IMEI.</span></span> <span data-ttu-id="5ee01-310">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5ee01-310">This property is read-only.</span></span>|
|<span data-ttu-id="5ee01-311">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="5ee01-311">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="5ee01-312">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ee01-312">DateTimeOffset</span></span>|<span data-ttu-id="5ee01-313">设备合规性宽限期到期的 DateTime。</span><span class="sxs-lookup"><span data-stu-id="5ee01-313">The DateTime when device compliance grace period expires.</span></span> <span data-ttu-id="5ee01-314">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5ee01-314">This property is read-only.</span></span>|
|<span data-ttu-id="5ee01-315">serialNumber</span><span class="sxs-lookup"><span data-stu-id="5ee01-315">serialNumber</span></span>|<span data-ttu-id="5ee01-316">String</span><span class="sxs-lookup"><span data-stu-id="5ee01-316">String</span></span>|<span data-ttu-id="5ee01-317">SerialNumber。</span><span class="sxs-lookup"><span data-stu-id="5ee01-317">SerialNumber.</span></span> <span data-ttu-id="5ee01-318">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5ee01-318">This property is read-only.</span></span>|
|<span data-ttu-id="5ee01-319">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="5ee01-319">phoneNumber</span></span>|<span data-ttu-id="5ee01-320">String</span><span class="sxs-lookup"><span data-stu-id="5ee01-320">String</span></span>|<span data-ttu-id="5ee01-321">电话设备的数量。</span><span class="sxs-lookup"><span data-stu-id="5ee01-321">Phone number of the device.</span></span> <span data-ttu-id="5ee01-322">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5ee01-322">This property is read-only.</span></span>|
|<span data-ttu-id="5ee01-323">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="5ee01-323">androidSecurityPatchLevel</span></span>|<span data-ttu-id="5ee01-324">String</span><span class="sxs-lookup"><span data-stu-id="5ee01-324">String</span></span>|<span data-ttu-id="5ee01-325">Android 安全修补程序级别。</span><span class="sxs-lookup"><span data-stu-id="5ee01-325">Android security patch level.</span></span> <span data-ttu-id="5ee01-326">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5ee01-326">This property is read-only.</span></span>|
|<span data-ttu-id="5ee01-327">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="5ee01-327">userDisplayName</span></span>|<span data-ttu-id="5ee01-328">String</span><span class="sxs-lookup"><span data-stu-id="5ee01-328">String</span></span>|<span data-ttu-id="5ee01-329">用户显示名称。</span><span class="sxs-lookup"><span data-stu-id="5ee01-329">User display name.</span></span> <span data-ttu-id="5ee01-330">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5ee01-330">This property is read-only.</span></span>|
|<span data-ttu-id="5ee01-331">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="5ee01-331">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="5ee01-332">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="5ee01-332">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="5ee01-333">ConfigrMgr 客户端启用的功能。</span><span class="sxs-lookup"><span data-stu-id="5ee01-333">ConfigrMgr client enabled features.</span></span> <span data-ttu-id="5ee01-334">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5ee01-334">This property is read-only.</span></span>|
|<span data-ttu-id="5ee01-335">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="5ee01-335">wiFiMacAddress</span></span>|<span data-ttu-id="5ee01-336">String</span><span class="sxs-lookup"><span data-stu-id="5ee01-336">String</span></span>|<span data-ttu-id="5ee01-337">Wi-Fi MAC。</span><span class="sxs-lookup"><span data-stu-id="5ee01-337">Wi-Fi MAC.</span></span> <span data-ttu-id="5ee01-338">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5ee01-338">This property is read-only.</span></span>|
|<span data-ttu-id="5ee01-339">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="5ee01-339">deviceHealthAttestationState</span></span>|[<span data-ttu-id="5ee01-340">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="5ee01-340">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="5ee01-341">设备运行状况证明状态。</span><span class="sxs-lookup"><span data-stu-id="5ee01-341">The device health attestation state.</span></span> <span data-ttu-id="5ee01-342">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5ee01-342">This property is read-only.</span></span>|
|<span data-ttu-id="5ee01-343">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="5ee01-343">subscriberCarrier</span></span>|<span data-ttu-id="5ee01-344">String</span><span class="sxs-lookup"><span data-stu-id="5ee01-344">String</span></span>|<span data-ttu-id="5ee01-345">订阅者运营商。</span><span class="sxs-lookup"><span data-stu-id="5ee01-345">Subscriber Carrier.</span></span> <span data-ttu-id="5ee01-346">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5ee01-346">This property is read-only.</span></span>|
|<span data-ttu-id="5ee01-347">meid</span><span class="sxs-lookup"><span data-stu-id="5ee01-347">meid</span></span>|<span data-ttu-id="5ee01-348">String</span><span class="sxs-lookup"><span data-stu-id="5ee01-348">String</span></span>|<span data-ttu-id="5ee01-349">MEID。</span><span class="sxs-lookup"><span data-stu-id="5ee01-349">MEID.</span></span> <span data-ttu-id="5ee01-350">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5ee01-350">This property is read-only.</span></span>|
|<span data-ttu-id="5ee01-351">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="5ee01-351">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="5ee01-352">Int64</span><span class="sxs-lookup"><span data-stu-id="5ee01-352">Int64</span></span>|<span data-ttu-id="5ee01-353">总存储字节数。</span><span class="sxs-lookup"><span data-stu-id="5ee01-353">Total Storage in Bytes.</span></span> <span data-ttu-id="5ee01-354">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5ee01-354">This property is read-only.</span></span>|
|<span data-ttu-id="5ee01-355">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="5ee01-355">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="5ee01-356">Int64</span><span class="sxs-lookup"><span data-stu-id="5ee01-356">Int64</span></span>|<span data-ttu-id="5ee01-357">可用存储字节为单位。</span><span class="sxs-lookup"><span data-stu-id="5ee01-357">Free Storage in Bytes.</span></span> <span data-ttu-id="5ee01-358">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5ee01-358">This property is read-only.</span></span>|
|<span data-ttu-id="5ee01-359">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="5ee01-359">managedDeviceName</span></span>|<span data-ttu-id="5ee01-360">String</span><span class="sxs-lookup"><span data-stu-id="5ee01-360">String</span></span>|<span data-ttu-id="5ee01-361">用于识别设备的自动生成的名称。</span><span class="sxs-lookup"><span data-stu-id="5ee01-361">Automatically generated name to identify a device.</span></span> <span data-ttu-id="5ee01-362">可以覆盖为用户友好名称。</span><span class="sxs-lookup"><span data-stu-id="5ee01-362">Can be overwritten to a user friendly name.</span></span>|
|<span data-ttu-id="5ee01-363">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="5ee01-363">partnerReportedThreatState</span></span>|[<span data-ttu-id="5ee01-364">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="5ee01-364">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="5ee01-365">指示帐户和设备正在使用移动威胁防护合作伙伴时设备的威胁状态。</span><span class="sxs-lookup"><span data-stu-id="5ee01-365">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="5ee01-366">只读。</span><span class="sxs-lookup"><span data-stu-id="5ee01-366">Read Only.</span></span> <span data-ttu-id="5ee01-367">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5ee01-367">This property is read-only.</span></span> <span data-ttu-id="5ee01-368">可取值为：`unknown`、`activated`、`deactivated`、`secured`、`lowSeverity`、`mediumSeverity`、`highSeverity`、`unresponsive`、`compromised`、`misconfigured`。</span><span class="sxs-lookup"><span data-stu-id="5ee01-368">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="5ee01-369">retireAfterDateTime</span><span class="sxs-lookup"><span data-stu-id="5ee01-369">retireAfterDateTime</span></span>|<span data-ttu-id="5ee01-370">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ee01-370">DateTimeOffset</span></span>|<span data-ttu-id="5ee01-371">指示设备因计划操作而自动停用的时间。</span><span class="sxs-lookup"><span data-stu-id="5ee01-371">Indicates the time after when a device will be auto retired because of scheduled action.</span></span> <span data-ttu-id="5ee01-372">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5ee01-372">This property is read-only.</span></span>|
|<span data-ttu-id="5ee01-373">usersLoggedOn</span><span class="sxs-lookup"><span data-stu-id="5ee01-373">usersLoggedOn</span></span>|<span data-ttu-id="5ee01-374">[loggedOnUser](../resources/intune-devices-loggedonuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5ee01-374">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="5ee01-375">指示设备上最后一次登录的用户。</span><span class="sxs-lookup"><span data-stu-id="5ee01-375">Indicates the last logged on users of a device.</span></span> <span data-ttu-id="5ee01-376">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5ee01-376">This property is read-only.</span></span>|
|<span data-ttu-id="5ee01-377">preferMdmOverGroupPolicyAppliedDateTime</span><span class="sxs-lookup"><span data-stu-id="5ee01-377">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="5ee01-378">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ee01-378">DateTimeOffset</span></span>|<span data-ttu-id="5ee01-379">报告 DateTime 设置了 preferMdmOverGroupPolicy 设置。</span><span class="sxs-lookup"><span data-stu-id="5ee01-379">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="5ee01-380">设置后，如果存在冲突，Intune MDM 设置将覆盖组策略设置。</span><span class="sxs-lookup"><span data-stu-id="5ee01-380">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="5ee01-381">只读。</span><span class="sxs-lookup"><span data-stu-id="5ee01-381">Read Only.</span></span> <span data-ttu-id="5ee01-382">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5ee01-382">This property is read-only.</span></span>|
|<span data-ttu-id="5ee01-383">autopilotEnrolled</span><span class="sxs-lookup"><span data-stu-id="5ee01-383">autopilotEnrolled</span></span>|<span data-ttu-id="5ee01-384">布尔值</span><span class="sxs-lookup"><span data-stu-id="5ee01-384">Boolean</span></span>|<span data-ttu-id="5ee01-385">报告托管设备是否通过自动试点注册。</span><span class="sxs-lookup"><span data-stu-id="5ee01-385">Reports if the managed device is enrolled via auto-pilot.</span></span> <span data-ttu-id="5ee01-386">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5ee01-386">This property is read-only.</span></span>|
|<span data-ttu-id="5ee01-387">requireUserEnrollmentApproval</span><span class="sxs-lookup"><span data-stu-id="5ee01-387">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="5ee01-388">布尔值</span><span class="sxs-lookup"><span data-stu-id="5ee01-388">Boolean</span></span>|<span data-ttu-id="5ee01-389">报告托管 iOS 设备是否注册用户审批。</span><span class="sxs-lookup"><span data-stu-id="5ee01-389">Reports if the managed iOS device is user approval enrollment.</span></span> <span data-ttu-id="5ee01-390">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5ee01-390">This property is read-only.</span></span>|
|<span data-ttu-id="5ee01-391">managementCertificateExpirationDate</span><span class="sxs-lookup"><span data-stu-id="5ee01-391">managementCertificateExpirationDate</span></span>|<span data-ttu-id="5ee01-392">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ee01-392">DateTimeOffset</span></span>|<span data-ttu-id="5ee01-393">报告设备管理证书到期日期。</span><span class="sxs-lookup"><span data-stu-id="5ee01-393">Reports device management certificate expiration date.</span></span> <span data-ttu-id="5ee01-394">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5ee01-394">This property is read-only.</span></span>|
|<span data-ttu-id="5ee01-395">iccid</span><span class="sxs-lookup"><span data-stu-id="5ee01-395">iccid</span></span>|<span data-ttu-id="5ee01-396">String</span><span class="sxs-lookup"><span data-stu-id="5ee01-396">String</span></span>|<span data-ttu-id="5ee01-397">集成的电路卡标识符，它是 SIM 卡的唯一标识号。</span><span class="sxs-lookup"><span data-stu-id="5ee01-397">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span> <span data-ttu-id="5ee01-398">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5ee01-398">This property is read-only.</span></span>|
|<span data-ttu-id="5ee01-399">udid</span><span class="sxs-lookup"><span data-stu-id="5ee01-399">udid</span></span>|<span data-ttu-id="5ee01-400">String</span><span class="sxs-lookup"><span data-stu-id="5ee01-400">String</span></span>|<span data-ttu-id="5ee01-401">iOS 和 macOS 设备的唯一设备标识符。</span><span class="sxs-lookup"><span data-stu-id="5ee01-401">Unique Device Identifier for iOS and macOS devices.</span></span> <span data-ttu-id="5ee01-402">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5ee01-402">This property is read-only.</span></span>|
|<span data-ttu-id="5ee01-403">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5ee01-403">roleScopeTagIds</span></span>|<span data-ttu-id="5ee01-404">String collection</span><span class="sxs-lookup"><span data-stu-id="5ee01-404">String collection</span></span>|<span data-ttu-id="5ee01-405">此设备实例的范围标记标识列表。</span><span class="sxs-lookup"><span data-stu-id="5ee01-405">List of Scope Tag IDs for this Device instance.</span></span>|
|<span data-ttu-id="5ee01-406">windowsActiveMalwareCount</span><span class="sxs-lookup"><span data-stu-id="5ee01-406">windowsActiveMalwareCount</span></span>|<span data-ttu-id="5ee01-407">Int32</span><span class="sxs-lookup"><span data-stu-id="5ee01-407">Int32</span></span>|<span data-ttu-id="5ee01-408">此 Windows 设备的活动恶意软件计数。</span><span class="sxs-lookup"><span data-stu-id="5ee01-408">Count of active malware for this windows device.</span></span> <span data-ttu-id="5ee01-409">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5ee01-409">This property is read-only.</span></span>|
|<span data-ttu-id="5ee01-410">windowsRemediatedMalwareCount</span><span class="sxs-lookup"><span data-stu-id="5ee01-410">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="5ee01-411">Int32</span><span class="sxs-lookup"><span data-stu-id="5ee01-411">Int32</span></span>|<span data-ttu-id="5ee01-412">此 Windows 设备的已修复恶意软件计数。</span><span class="sxs-lookup"><span data-stu-id="5ee01-412">Count of remediated malware for this windows device.</span></span> <span data-ttu-id="5ee01-413">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5ee01-413">This property is read-only.</span></span>|
|<span data-ttu-id="5ee01-414">notes</span><span class="sxs-lookup"><span data-stu-id="5ee01-414">notes</span></span>|<span data-ttu-id="5ee01-415">String</span><span class="sxs-lookup"><span data-stu-id="5ee01-415">String</span></span>|<span data-ttu-id="5ee01-416">IT 管理员在设备上创建的备注</span><span class="sxs-lookup"><span data-stu-id="5ee01-416">Notes on the device created by IT Admin</span></span>|
|<span data-ttu-id="5ee01-417">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="5ee01-417">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="5ee01-418">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="5ee01-418">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="5ee01-419">配置管理器客户端运行状况状态，仅对 MDM/ConfigMgr 代理管理的设备有效</span><span class="sxs-lookup"><span data-stu-id="5ee01-419">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent</span></span>|
|<span data-ttu-id="5ee01-420">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="5ee01-420">configurationManagerClientInformation</span></span>|[<span data-ttu-id="5ee01-421">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="5ee01-421">configurationManagerClientInformation</span></span>](../resources/intune-devices-configurationmanagerclientinformation.md)|<span data-ttu-id="5ee01-422">配置管理器客户端信息，仅对 ConfigMgr 代理托管、duel 托管或三管理的设备有效</span><span class="sxs-lookup"><span data-stu-id="5ee01-422">Configuration manager client information, valid only for devices managed, duel-managed or tri-managed by ConfigMgr Agent</span></span>|
|<span data-ttu-id="5ee01-423">ethernetMacAddress</span><span class="sxs-lookup"><span data-stu-id="5ee01-423">ethernetMacAddress</span></span>|<span data-ttu-id="5ee01-424">String</span><span class="sxs-lookup"><span data-stu-id="5ee01-424">String</span></span>|<span data-ttu-id="5ee01-425">以太网 MAC。</span><span class="sxs-lookup"><span data-stu-id="5ee01-425">Ethernet MAC.</span></span> <span data-ttu-id="5ee01-426">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5ee01-426">This property is read-only.</span></span>|
|<span data-ttu-id="5ee01-427">physicalMemoryInBytes</span><span class="sxs-lookup"><span data-stu-id="5ee01-427">physicalMemoryInBytes</span></span>|<span data-ttu-id="5ee01-428">Int64</span><span class="sxs-lookup"><span data-stu-id="5ee01-428">Int64</span></span>|<span data-ttu-id="5ee01-429">内存总量（以字节为单位）。</span><span class="sxs-lookup"><span data-stu-id="5ee01-429">Total Memory in Bytes.</span></span> <span data-ttu-id="5ee01-430">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5ee01-430">This property is read-only.</span></span>|
|<span data-ttu-id="5ee01-431">processorArchitecture</span><span class="sxs-lookup"><span data-stu-id="5ee01-431">processorArchitecture</span></span>|[<span data-ttu-id="5ee01-432">managedDeviceArchitecture</span><span class="sxs-lookup"><span data-stu-id="5ee01-432">managedDeviceArchitecture</span></span>](../resources/intune-devices-manageddevicearchitecture.md)|<span data-ttu-id="5ee01-433">处理器体系结构。</span><span class="sxs-lookup"><span data-stu-id="5ee01-433">Processor architecture.</span></span> <span data-ttu-id="5ee01-434">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5ee01-434">This property is read-only.</span></span> <span data-ttu-id="5ee01-435">可取值为：`unknown`、`x86`、`x64`、`arm`、`arM64`。</span><span class="sxs-lookup"><span data-stu-id="5ee01-435">Possible values are: `unknown`, `x86`, `x64`, `arm`, `arM64`.</span></span>|
|<span data-ttu-id="5ee01-436">specificationVersion</span><span class="sxs-lookup"><span data-stu-id="5ee01-436">specificationVersion</span></span>|<span data-ttu-id="5ee01-437">String</span><span class="sxs-lookup"><span data-stu-id="5ee01-437">String</span></span>|<span data-ttu-id="5ee01-438">规范版本。</span><span class="sxs-lookup"><span data-stu-id="5ee01-438">Specification version.</span></span> <span data-ttu-id="5ee01-439">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5ee01-439">This property is read-only.</span></span>|
|<span data-ttu-id="5ee01-440">joinType</span><span class="sxs-lookup"><span data-stu-id="5ee01-440">joinType</span></span>|[<span data-ttu-id="5ee01-441">joinType</span><span class="sxs-lookup"><span data-stu-id="5ee01-441">joinType</span></span>](../resources/intune-devices-jointype.md)|<span data-ttu-id="5ee01-442">设备加入类型。</span><span class="sxs-lookup"><span data-stu-id="5ee01-442">Device join type.</span></span> <span data-ttu-id="5ee01-443">可取值为：`unknown`、`azureADJoined`、`azureADRegistered`、`hybridAzureADJoined`。</span><span class="sxs-lookup"><span data-stu-id="5ee01-443">Possible values are: `unknown`, `azureADJoined`, `azureADRegistered`, `hybridAzureADJoined`.</span></span>|
|<span data-ttu-id="5ee01-444">skuFamily</span><span class="sxs-lookup"><span data-stu-id="5ee01-444">skuFamily</span></span>|<span data-ttu-id="5ee01-445">String</span><span class="sxs-lookup"><span data-stu-id="5ee01-445">String</span></span>|<span data-ttu-id="5ee01-446">设备 sku 系列</span><span class="sxs-lookup"><span data-stu-id="5ee01-446">Device sku family</span></span>|
|<span data-ttu-id="5ee01-447">skuNumber</span><span class="sxs-lookup"><span data-stu-id="5ee01-447">skuNumber</span></span>|<span data-ttu-id="5ee01-448">Int32</span><span class="sxs-lookup"><span data-stu-id="5ee01-448">Int32</span></span>|<span data-ttu-id="5ee01-449">设备 sku 号，另请参阅 https://docs.microsoft.com/windows/win32/api/sysinfoapi/nf-sysinfoapi-getproductinfo ：。</span><span class="sxs-lookup"><span data-stu-id="5ee01-449">Device sku number, see also: https://docs.microsoft.com/windows/win32/api/sysinfoapi/nf-sysinfoapi-getproductinfo.</span></span> <span data-ttu-id="5ee01-450">有效值为 0 到 2147483647。</span><span class="sxs-lookup"><span data-stu-id="5ee01-450">Valid values 0 to 2147483647.</span></span> <span data-ttu-id="5ee01-451">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5ee01-451">This property is read-only.</span></span>|
|<span data-ttu-id="5ee01-452">managementFeatures</span><span class="sxs-lookup"><span data-stu-id="5ee01-452">managementFeatures</span></span>|[<span data-ttu-id="5ee01-453">managedDeviceManagementFeatures</span><span class="sxs-lookup"><span data-stu-id="5ee01-453">managedDeviceManagementFeatures</span></span>](../resources/intune-devices-manageddevicemanagementfeatures.md)|<span data-ttu-id="5ee01-454">设备管理功能。</span><span class="sxs-lookup"><span data-stu-id="5ee01-454">Device management features.</span></span> <span data-ttu-id="5ee01-455">可取值为：`none`、`microsoftManagedDesktop`。</span><span class="sxs-lookup"><span data-stu-id="5ee01-455">Possible values are: `none`, `microsoftManagedDesktop`.</span></span>|
|<span data-ttu-id="5ee01-456">chromeOSDeviceInfo</span><span class="sxs-lookup"><span data-stu-id="5ee01-456">chromeOSDeviceInfo</span></span>|<span data-ttu-id="5ee01-457">[chromeOSDeviceProperty](../resources/intune-devices-chromeosdeviceproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5ee01-457">[chromeOSDeviceProperty](../resources/intune-devices-chromeosdeviceproperty.md) collection</span></span>|<span data-ttu-id="5ee01-458">ChromeOS 设备的属性列表。</span><span class="sxs-lookup"><span data-stu-id="5ee01-458">List of properties of the ChromeOS Device.</span></span>|



## <a name="response"></a><span data-ttu-id="5ee01-459">响应</span><span class="sxs-lookup"><span data-stu-id="5ee01-459">Response</span></span>
<span data-ttu-id="5ee01-460">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [managedDevice](../resources/intune-devices-manageddevice.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5ee01-460">If successful, this method returns a `200 OK` response code and an updated [managedDevice](../resources/intune-devices-manageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ee01-461">示例</span><span class="sxs-lookup"><span data-stu-id="5ee01-461">Example</span></span>

### <a name="request"></a><span data-ttu-id="5ee01-462">请求</span><span class="sxs-lookup"><span data-stu-id="5ee01-462">Request</span></span>
<span data-ttu-id="5ee01-463">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5ee01-463">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}
Content-type: application/json
Content-length: 8557

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
    "operatingSystemProductType": 10,
    "ipAddressV4": "Ip Address V4 value",
    "subnetAddress": "Subnet Address value",
    "esimIdentifier": "Esim Identifier value",
    "systemManagementBIOSVersion": "System Management BIOSVersion value",
    "tpmManufacturer": "Tpm Manufacturer value",
    "tpmVersion": "Tpm Version value"
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
  "managementFeatures": "microsoftManagedDesktop",
  "chromeOSDeviceInfo": [
    {
      "@odata.type": "microsoft.graph.chromeOSDeviceProperty",
      "name": "Name value",
      "value": "Value value",
      "valueType": "Value Type value",
      "updatable": true
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="5ee01-464">响应</span><span class="sxs-lookup"><span data-stu-id="5ee01-464">Response</span></span>
<span data-ttu-id="5ee01-p174">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5ee01-p174">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 8606

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
    "operatingSystemProductType": 10,
    "ipAddressV4": "Ip Address V4 value",
    "subnetAddress": "Subnet Address value",
    "esimIdentifier": "Esim Identifier value",
    "systemManagementBIOSVersion": "System Management BIOSVersion value",
    "tpmManufacturer": "Tpm Manufacturer value",
    "tpmVersion": "Tpm Version value"
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
  "managementFeatures": "microsoftManagedDesktop",
  "chromeOSDeviceInfo": [
    {
      "@odata.type": "microsoft.graph.chromeOSDeviceProperty",
      "name": "Name value",
      "value": "Value value",
      "valueType": "Value Type value",
      "updatable": true
    }
  ]
}
```




