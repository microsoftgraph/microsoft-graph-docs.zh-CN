---
title: 更新 managedDevice
description: 更新 managedDevice 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1d4cdc3242c176c92c595573de0509d151261941
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42814125"
---
# <a name="update-manageddevice"></a><span data-ttu-id="9e201-103">更新 managedDevice</span><span class="sxs-lookup"><span data-stu-id="9e201-103">Update managedDevice</span></span>

> <span data-ttu-id="9e201-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9e201-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9e201-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9e201-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9e201-106">更新 [managedDevice](../resources/intune-devices-manageddevice.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9e201-106">Update the properties of a [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9e201-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="9e201-107">Prerequisites</span></span>
<span data-ttu-id="9e201-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9e201-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e201-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="9e201-110">Permission type</span></span>|<span data-ttu-id="9e201-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9e201-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9e201-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9e201-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9e201-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e201-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="9e201-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9e201-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9e201-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9e201-115">Not supported.</span></span>|
|<span data-ttu-id="9e201-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="9e201-116">Application</span></span>|<span data-ttu-id="9e201-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e201-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9e201-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9e201-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managedDevices/{managedDeviceId}
PATCH /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}
```

## <a name="request-headers"></a><span data-ttu-id="9e201-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="9e201-119">Request headers</span></span>
|<span data-ttu-id="9e201-120">标头</span><span class="sxs-lookup"><span data-stu-id="9e201-120">Header</span></span>|<span data-ttu-id="9e201-121">值</span><span class="sxs-lookup"><span data-stu-id="9e201-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9e201-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9e201-122">Authorization</span></span>|<span data-ttu-id="9e201-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9e201-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9e201-124">接受</span><span class="sxs-lookup"><span data-stu-id="9e201-124">Accept</span></span>|<span data-ttu-id="9e201-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9e201-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9e201-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="9e201-126">Request body</span></span>
<span data-ttu-id="9e201-127">在请求正文中，提供 [managedDevice](../resources/intune-devices-manageddevice.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9e201-127">In the request body, supply a JSON representation for the [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>

<span data-ttu-id="9e201-128">下表显示创建 [managedDevice](../resources/intune-devices-manageddevice.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="9e201-128">The following table shows the properties that are required when you create the [managedDevice](../resources/intune-devices-manageddevice.md).</span></span>

|<span data-ttu-id="9e201-129">属性</span><span class="sxs-lookup"><span data-stu-id="9e201-129">Property</span></span>|<span data-ttu-id="9e201-130">类型</span><span class="sxs-lookup"><span data-stu-id="9e201-130">Type</span></span>|<span data-ttu-id="9e201-131">说明</span><span class="sxs-lookup"><span data-stu-id="9e201-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e201-132">id</span><span class="sxs-lookup"><span data-stu-id="9e201-132">id</span></span>|<span data-ttu-id="9e201-133">字符串</span><span class="sxs-lookup"><span data-stu-id="9e201-133">String</span></span>|<span data-ttu-id="9e201-134">设备的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="9e201-134">Unique Identifier for the device.</span></span> <span data-ttu-id="9e201-135">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9e201-135">This property is read-only.</span></span>|
|<span data-ttu-id="9e201-136">userId</span><span class="sxs-lookup"><span data-stu-id="9e201-136">userId</span></span>|<span data-ttu-id="9e201-137">String</span><span class="sxs-lookup"><span data-stu-id="9e201-137">String</span></span>|<span data-ttu-id="9e201-138">与设备关联的用户的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="9e201-138">Unique Identifier for the user associated with the device.</span></span> <span data-ttu-id="9e201-139">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9e201-139">This property is read-only.</span></span>|
|<span data-ttu-id="9e201-140">deviceName</span><span class="sxs-lookup"><span data-stu-id="9e201-140">deviceName</span></span>|<span data-ttu-id="9e201-141">String</span><span class="sxs-lookup"><span data-stu-id="9e201-141">String</span></span>|<span data-ttu-id="9e201-142">设备的名称。</span><span class="sxs-lookup"><span data-stu-id="9e201-142">Name of the device.</span></span> <span data-ttu-id="9e201-143">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9e201-143">This property is read-only.</span></span>|
|<span data-ttu-id="9e201-144">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="9e201-144">hardwareInformation</span></span>|[<span data-ttu-id="9e201-145">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="9e201-145">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="9e201-146">设备的 hardward 详细信息。</span><span class="sxs-lookup"><span data-stu-id="9e201-146">The hardward details for the device.</span></span>  <span data-ttu-id="9e201-147">包括存储空间、制造商、序列号等信息。此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9e201-147">Includes information such as storage space, manufacturer, serial number, etc. This property is read-only.</span></span>|
|<span data-ttu-id="9e201-148">所有者</span><span class="sxs-lookup"><span data-stu-id="9e201-148">ownerType</span></span>|[<span data-ttu-id="9e201-149">所有者</span><span class="sxs-lookup"><span data-stu-id="9e201-149">ownerType</span></span>](../resources/intune-shared-ownertype.md)|<span data-ttu-id="9e201-150">设备的所有权。</span><span class="sxs-lookup"><span data-stu-id="9e201-150">Ownership of the device.</span></span> <span data-ttu-id="9e201-151">可以是 "公司" 或 "个人"。</span><span class="sxs-lookup"><span data-stu-id="9e201-151">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="9e201-152">可取值为：`unknown`、`company`、`personal`。</span><span class="sxs-lookup"><span data-stu-id="9e201-152">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="9e201-153">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="9e201-153">managedDeviceOwnerType</span></span>|[<span data-ttu-id="9e201-154">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="9e201-154">managedDeviceOwnerType</span></span>](../resources/intune-shared-manageddeviceownertype.md)|<span data-ttu-id="9e201-155">设备的所有权。</span><span class="sxs-lookup"><span data-stu-id="9e201-155">Ownership of the device.</span></span> <span data-ttu-id="9e201-156">可以是 "公司" 或 "个人"。</span><span class="sxs-lookup"><span data-stu-id="9e201-156">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="9e201-157">可取值为：`unknown`、`company`、`personal`。</span><span class="sxs-lookup"><span data-stu-id="9e201-157">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="9e201-158">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="9e201-158">deviceActionResults</span></span>|<span data-ttu-id="9e201-159">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9e201-159">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="9e201-160">ComplexType deviceActionResult 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="9e201-160">List of ComplexType deviceActionResult objects.</span></span> <span data-ttu-id="9e201-161">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9e201-161">This property is read-only.</span></span>|
|<span data-ttu-id="9e201-162">managementState</span><span class="sxs-lookup"><span data-stu-id="9e201-162">managementState</span></span>|[<span data-ttu-id="9e201-163">managementState</span><span class="sxs-lookup"><span data-stu-id="9e201-163">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="9e201-164">设备的管理状态。</span><span class="sxs-lookup"><span data-stu-id="9e201-164">Management state of the device.</span></span> <span data-ttu-id="9e201-165">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9e201-165">This property is read-only.</span></span> <span data-ttu-id="9e201-166">可取值为：`managed`、`retirePending`、`retireFailed`、`wipePending`、`wipeFailed`、`unhealthy`、`deletePending`、`retireIssued`、`wipeIssued`、`wipeCanceled`、`retireCanceled`、`discovered`。</span><span class="sxs-lookup"><span data-stu-id="9e201-166">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="9e201-167">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="9e201-167">enrolledDateTime</span></span>|<span data-ttu-id="9e201-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e201-168">DateTimeOffset</span></span>|<span data-ttu-id="9e201-169">设备的注册时间。</span><span class="sxs-lookup"><span data-stu-id="9e201-169">Enrollment time of the device.</span></span> <span data-ttu-id="9e201-170">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9e201-170">This property is read-only.</span></span>|
|<span data-ttu-id="9e201-171">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="9e201-171">lastSyncDateTime</span></span>|<span data-ttu-id="9e201-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e201-172">DateTimeOffset</span></span>|<span data-ttu-id="9e201-173">设备上次成功完成与 Intune 同步的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="9e201-173">The date and time that the device last completed a successful sync with Intune.</span></span> <span data-ttu-id="9e201-174">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9e201-174">This property is read-only.</span></span>|
|<span data-ttu-id="9e201-175">chassisType</span><span class="sxs-lookup"><span data-stu-id="9e201-175">chassisType</span></span>|[<span data-ttu-id="9e201-176">chassisType</span><span class="sxs-lookup"><span data-stu-id="9e201-176">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="9e201-177">设备的机箱类型。</span><span class="sxs-lookup"><span data-stu-id="9e201-177">Chassis type of the device.</span></span> <span data-ttu-id="9e201-178">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9e201-178">This property is read-only.</span></span> <span data-ttu-id="9e201-179">可取值为：`unknown`、`desktop`、`laptop`、`worksWorkstation`、`enterpriseServer`、`phone`、`tablet`、`mobileOther`、`mobileUnknown`。</span><span class="sxs-lookup"><span data-stu-id="9e201-179">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="9e201-180">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="9e201-180">operatingSystem</span></span>|<span data-ttu-id="9e201-181">String</span><span class="sxs-lookup"><span data-stu-id="9e201-181">String</span></span>|<span data-ttu-id="9e201-182">设备的操作系统。</span><span class="sxs-lookup"><span data-stu-id="9e201-182">Operating system of the device.</span></span> <span data-ttu-id="9e201-183">Windows、iOS 等。此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9e201-183">Windows, iOS, etc. This property is read-only.</span></span>|
|<span data-ttu-id="9e201-184">deviceType</span><span class="sxs-lookup"><span data-stu-id="9e201-184">deviceType</span></span>|[<span data-ttu-id="9e201-185">deviceType</span><span class="sxs-lookup"><span data-stu-id="9e201-185">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="9e201-186">设备的平台。</span><span class="sxs-lookup"><span data-stu-id="9e201-186">Platform of the device.</span></span> <span data-ttu-id="9e201-187">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9e201-187">This property is read-only.</span></span> <span data-ttu-id="9e201-188">可能的值为`desktop`： `windowsRT`、 `winMO6`、 `nokia` `windowsPhone` `mac` `winCE` `palm` `unknown`、、、、、、、、、、、、、、、、、、、、。 `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `windows10x` `blackberry`</span><span class="sxs-lookup"><span data-stu-id="9e201-188">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="9e201-189">complianceState</span><span class="sxs-lookup"><span data-stu-id="9e201-189">complianceState</span></span>|[<span data-ttu-id="9e201-190">complianceState</span><span class="sxs-lookup"><span data-stu-id="9e201-190">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="9e201-191">设备的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="9e201-191">Compliance state of the device.</span></span> <span data-ttu-id="9e201-192">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9e201-192">This property is read-only.</span></span> <span data-ttu-id="9e201-193">可取值为：`unknown`、`compliant`、`noncompliant`、`conflict`、`error`、`inGracePeriod`、`configManager`。</span><span class="sxs-lookup"><span data-stu-id="9e201-193">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="9e201-194">jailBroken</span><span class="sxs-lookup"><span data-stu-id="9e201-194">jailBroken</span></span>|<span data-ttu-id="9e201-195">String</span><span class="sxs-lookup"><span data-stu-id="9e201-195">String</span></span>|<span data-ttu-id="9e201-196">设备是否已越狱或取得 root 权限。</span><span class="sxs-lookup"><span data-stu-id="9e201-196">whether the device is jail broken or rooted.</span></span> <span data-ttu-id="9e201-197">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9e201-197">This property is read-only.</span></span>|
|<span data-ttu-id="9e201-198">managementAgent</span><span class="sxs-lookup"><span data-stu-id="9e201-198">managementAgent</span></span>|[<span data-ttu-id="9e201-199">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="9e201-199">managementAgentType</span></span>](../resources/intune-shared-managementagenttype.md)|<span data-ttu-id="9e201-200">设备的管理通道。</span><span class="sxs-lookup"><span data-stu-id="9e201-200">Management channel of the device.</span></span> <span data-ttu-id="9e201-201">Intune、EAS 等。此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9e201-201">Intune, EAS, etc. This property is read-only.</span></span> <span data-ttu-id="9e201-202">可能的值是：`eas`、`mdm`、`easMdm`、`intuneClient`、`easIntuneClient`、`configurationManagerClient`、`configurationManagerClientMdm`、`configurationManagerClientMdmEas`、`unknown`、`jamf`、`googleCloudDevicePolicyController`、`microsoft365ManagedMdm`、`windowsManagementCloudApi`。</span><span class="sxs-lookup"><span data-stu-id="9e201-202">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`, `windowsManagementCloudApi`.</span></span>|
|<span data-ttu-id="9e201-203">osVersion</span><span class="sxs-lookup"><span data-stu-id="9e201-203">osVersion</span></span>|<span data-ttu-id="9e201-204">String</span><span class="sxs-lookup"><span data-stu-id="9e201-204">String</span></span>|<span data-ttu-id="9e201-205">设备的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="9e201-205">Operating system version of the device.</span></span> <span data-ttu-id="9e201-206">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9e201-206">This property is read-only.</span></span>|
|<span data-ttu-id="9e201-207">easActivated</span><span class="sxs-lookup"><span data-stu-id="9e201-207">easActivated</span></span>|<span data-ttu-id="9e201-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e201-208">Boolean</span></span>|<span data-ttu-id="9e201-209">设备是否已激活 Exchange ActiveSync。</span><span class="sxs-lookup"><span data-stu-id="9e201-209">Whether the device is Exchange ActiveSync activated.</span></span> <span data-ttu-id="9e201-210">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9e201-210">This property is read-only.</span></span>|
|<span data-ttu-id="9e201-211">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="9e201-211">easDeviceId</span></span>|<span data-ttu-id="9e201-212">String</span><span class="sxs-lookup"><span data-stu-id="9e201-212">String</span></span>|<span data-ttu-id="9e201-213">设备的 Exchange ActiveSync ID。</span><span class="sxs-lookup"><span data-stu-id="9e201-213">Exchange ActiveSync Id of the device.</span></span> <span data-ttu-id="9e201-214">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9e201-214">This property is read-only.</span></span>|
|<span data-ttu-id="9e201-215">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="9e201-215">easActivationDateTime</span></span>|<span data-ttu-id="9e201-216">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e201-216">DateTimeOffset</span></span>|<span data-ttu-id="9e201-217">设备的 Exchange ActivationSync 激活时间。</span><span class="sxs-lookup"><span data-stu-id="9e201-217">Exchange ActivationSync activation time of the device.</span></span> <span data-ttu-id="9e201-218">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9e201-218">This property is read-only.</span></span>|
|<span data-ttu-id="9e201-219">aadRegistered</span><span class="sxs-lookup"><span data-stu-id="9e201-219">aadRegistered</span></span>|<span data-ttu-id="9e201-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e201-220">Boolean</span></span>|<span data-ttu-id="9e201-221">设备是否已注册 Azure Active Directory。</span><span class="sxs-lookup"><span data-stu-id="9e201-221">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="9e201-222">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9e201-222">This property is read-only.</span></span>|
|<span data-ttu-id="9e201-223">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="9e201-223">azureADRegistered</span></span>|<span data-ttu-id="9e201-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e201-224">Boolean</span></span>|<span data-ttu-id="9e201-225">设备是否已注册 Azure Active Directory。</span><span class="sxs-lookup"><span data-stu-id="9e201-225">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="9e201-226">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9e201-226">This property is read-only.</span></span>|
|<span data-ttu-id="9e201-227">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="9e201-227">deviceEnrollmentType</span></span>|[<span data-ttu-id="9e201-228">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="9e201-228">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="9e201-229">设备的注册类型。</span><span class="sxs-lookup"><span data-stu-id="9e201-229">Enrollment type of the device.</span></span> <span data-ttu-id="9e201-230">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9e201-230">This property is read-only.</span></span> <span data-ttu-id="9e201-231">可取值为：`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement`、`appleUserEnrollment`、`appleUserEnrollmentWithServiceAccount`。</span><span class="sxs-lookup"><span data-stu-id="9e201-231">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`.</span></span>|
|<span data-ttu-id="9e201-232">lostModeState</span><span class="sxs-lookup"><span data-stu-id="9e201-232">lostModeState</span></span>|[<span data-ttu-id="9e201-233">lostModeState</span><span class="sxs-lookup"><span data-stu-id="9e201-233">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="9e201-234">指示是否已启用或禁用了丢失模式。</span><span class="sxs-lookup"><span data-stu-id="9e201-234">Indicates if Lost mode is enabled or disabled.</span></span> <span data-ttu-id="9e201-235">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9e201-235">This property is read-only.</span></span> <span data-ttu-id="9e201-236">可取值为：`disabled`、`enabled`。</span><span class="sxs-lookup"><span data-stu-id="9e201-236">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="9e201-237">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="9e201-237">activationLockBypassCode</span></span>|<span data-ttu-id="9e201-238">String</span><span class="sxs-lookup"><span data-stu-id="9e201-238">String</span></span>|<span data-ttu-id="9e201-239">允许绕过设备上的激活锁的代码。</span><span class="sxs-lookup"><span data-stu-id="9e201-239">Code that allows the Activation Lock on a device to be bypassed.</span></span> <span data-ttu-id="9e201-240">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9e201-240">This property is read-only.</span></span>|
|<span data-ttu-id="9e201-241">emailAddress</span><span class="sxs-lookup"><span data-stu-id="9e201-241">emailAddress</span></span>|<span data-ttu-id="9e201-242">String</span><span class="sxs-lookup"><span data-stu-id="9e201-242">String</span></span>|<span data-ttu-id="9e201-243">与设备关联的用户的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="9e201-243">Email(s) for the user associated with the device.</span></span> <span data-ttu-id="9e201-244">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9e201-244">This property is read-only.</span></span>|
|<span data-ttu-id="9e201-245">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="9e201-245">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="9e201-246">String</span><span class="sxs-lookup"><span data-stu-id="9e201-246">String</span></span>|<span data-ttu-id="9e201-247">Azure Active Directory 设备的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="9e201-247">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="9e201-248">只读。</span><span class="sxs-lookup"><span data-stu-id="9e201-248">Read only.</span></span> <span data-ttu-id="9e201-249">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9e201-249">This property is read-only.</span></span>|
|<span data-ttu-id="9e201-250">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="9e201-250">azureADDeviceId</span></span>|<span data-ttu-id="9e201-251">String</span><span class="sxs-lookup"><span data-stu-id="9e201-251">String</span></span>|<span data-ttu-id="9e201-252">Azure Active Directory 设备的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="9e201-252">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="9e201-253">只读。</span><span class="sxs-lookup"><span data-stu-id="9e201-253">Read only.</span></span> <span data-ttu-id="9e201-254">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9e201-254">This property is read-only.</span></span>|
|<span data-ttu-id="9e201-255">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="9e201-255">deviceRegistrationState</span></span>|[<span data-ttu-id="9e201-256">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="9e201-256">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="9e201-257">设备注册状态。</span><span class="sxs-lookup"><span data-stu-id="9e201-257">Device registration state.</span></span> <span data-ttu-id="9e201-258">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9e201-258">This property is read-only.</span></span> <span data-ttu-id="9e201-259">可取值为：`notRegistered`、`registered`、`revoked`、`keyConflict`、`approvalPending`、`certificateReset`、`notRegisteredPendingEnrollment`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="9e201-259">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="9e201-260">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="9e201-260">deviceCategoryDisplayName</span></span>|<span data-ttu-id="9e201-261">String</span><span class="sxs-lookup"><span data-stu-id="9e201-261">String</span></span>|<span data-ttu-id="9e201-262">设备类别显示名称。</span><span class="sxs-lookup"><span data-stu-id="9e201-262">Device category display name.</span></span> <span data-ttu-id="9e201-263">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9e201-263">This property is read-only.</span></span>|
|<span data-ttu-id="9e201-264">isSupervised</span><span class="sxs-lookup"><span data-stu-id="9e201-264">isSupervised</span></span>|<span data-ttu-id="9e201-265">布尔值</span><span class="sxs-lookup"><span data-stu-id="9e201-265">Boolean</span></span>|<span data-ttu-id="9e201-266">设备监督状态。</span><span class="sxs-lookup"><span data-stu-id="9e201-266">Device supervised status.</span></span> <span data-ttu-id="9e201-267">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9e201-267">This property is read-only.</span></span>|
|<span data-ttu-id="9e201-268">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="9e201-268">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="9e201-269">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e201-269">DateTimeOffset</span></span>|<span data-ttu-id="9e201-270">设备上次与 Exchange 联系的时间。</span><span class="sxs-lookup"><span data-stu-id="9e201-270">Last time the device contacted Exchange.</span></span> <span data-ttu-id="9e201-271">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9e201-271">This property is read-only.</span></span>|
|<span data-ttu-id="9e201-272">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="9e201-272">exchangeAccessState</span></span>|[<span data-ttu-id="9e201-273">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="9e201-273">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="9e201-274">Exchange 中设备的访问状态。</span><span class="sxs-lookup"><span data-stu-id="9e201-274">The Access State of the device in Exchange.</span></span> <span data-ttu-id="9e201-275">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9e201-275">This property is read-only.</span></span> <span data-ttu-id="9e201-276">可取值为：`none`、`unknown`、`allowed`、`blocked`、`quarantined`。</span><span class="sxs-lookup"><span data-stu-id="9e201-276">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="9e201-277">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="9e201-277">exchangeAccessStateReason</span></span>|[<span data-ttu-id="9e201-278">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="9e201-278">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="9e201-279">Exchange 中设备访问状态的出现原因。</span><span class="sxs-lookup"><span data-stu-id="9e201-279">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="9e201-280">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9e201-280">This property is read-only.</span></span> <span data-ttu-id="9e201-281">可取值为：`none`、`unknown`、`exchangeGlobalRule`、`exchangeIndividualRule`、`exchangeDeviceRule`、`exchangeUpgrade`、`exchangeMailboxPolicy`、`other`、`compliant`、`notCompliant`、`notEnrolled`、`unknownLocation`、`mfaRequired`、`azureADBlockDueToAccessPolicy`、`compromisedPassword`、`deviceNotKnownWithManagedApp`。</span><span class="sxs-lookup"><span data-stu-id="9e201-281">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="9e201-282">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="9e201-282">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="9e201-283">String</span><span class="sxs-lookup"><span data-stu-id="9e201-283">String</span></span>|<span data-ttu-id="9e201-284">允许与设备建立远程协助会话的 URL。</span><span class="sxs-lookup"><span data-stu-id="9e201-284">Url that allows a Remote Assistance session to be established with the device.</span></span> <span data-ttu-id="9e201-285">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9e201-285">This property is read-only.</span></span>|
|<span data-ttu-id="9e201-286">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="9e201-286">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="9e201-287">String</span><span class="sxs-lookup"><span data-stu-id="9e201-287">String</span></span>|<span data-ttu-id="9e201-288">用于在创建远程协助会话对象时识别问题的错误字符串。</span><span class="sxs-lookup"><span data-stu-id="9e201-288">An error string that identifies issues when creating Remote Assistance session objects.</span></span> <span data-ttu-id="9e201-289">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9e201-289">This property is read-only.</span></span>|
|<span data-ttu-id="9e201-290">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="9e201-290">isEncrypted</span></span>|<span data-ttu-id="9e201-291">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e201-291">Boolean</span></span>|<span data-ttu-id="9e201-292">设备加密状态。</span><span class="sxs-lookup"><span data-stu-id="9e201-292">Device encryption status.</span></span> <span data-ttu-id="9e201-293">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9e201-293">This property is read-only.</span></span>|
|<span data-ttu-id="9e201-294">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="9e201-294">userPrincipalName</span></span>|<span data-ttu-id="9e201-295">String</span><span class="sxs-lookup"><span data-stu-id="9e201-295">String</span></span>|<span data-ttu-id="9e201-296">设备用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="9e201-296">Device user principal name.</span></span> <span data-ttu-id="9e201-297">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9e201-297">This property is read-only.</span></span>|
|<span data-ttu-id="9e201-298">model</span><span class="sxs-lookup"><span data-stu-id="9e201-298">model</span></span>|<span data-ttu-id="9e201-299">String</span><span class="sxs-lookup"><span data-stu-id="9e201-299">String</span></span>|<span data-ttu-id="9e201-300">设备的模型。</span><span class="sxs-lookup"><span data-stu-id="9e201-300">Model of the device.</span></span> <span data-ttu-id="9e201-301">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9e201-301">This property is read-only.</span></span>|
|<span data-ttu-id="9e201-302">manufacturer</span><span class="sxs-lookup"><span data-stu-id="9e201-302">manufacturer</span></span>|<span data-ttu-id="9e201-303">String</span><span class="sxs-lookup"><span data-stu-id="9e201-303">String</span></span>|<span data-ttu-id="9e201-304">设备的制造商。</span><span class="sxs-lookup"><span data-stu-id="9e201-304">Manufacturer of the device.</span></span> <span data-ttu-id="9e201-305">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9e201-305">This property is read-only.</span></span>|
|<span data-ttu-id="9e201-306">imei</span><span class="sxs-lookup"><span data-stu-id="9e201-306">imei</span></span>|<span data-ttu-id="9e201-307">String</span><span class="sxs-lookup"><span data-stu-id="9e201-307">String</span></span>|<span data-ttu-id="9e201-308">IMEI.</span><span class="sxs-lookup"><span data-stu-id="9e201-308">IMEI.</span></span> <span data-ttu-id="9e201-309">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9e201-309">This property is read-only.</span></span>|
|<span data-ttu-id="9e201-310">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="9e201-310">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="9e201-311">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e201-311">DateTimeOffset</span></span>|<span data-ttu-id="9e201-312">设备符合性宽限期到期时的日期时间。</span><span class="sxs-lookup"><span data-stu-id="9e201-312">The DateTime when device compliance grace period expires.</span></span> <span data-ttu-id="9e201-313">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9e201-313">This property is read-only.</span></span>|
|<span data-ttu-id="9e201-314">serialNumber</span><span class="sxs-lookup"><span data-stu-id="9e201-314">serialNumber</span></span>|<span data-ttu-id="9e201-315">字符串</span><span class="sxs-lookup"><span data-stu-id="9e201-315">String</span></span>|<span data-ttu-id="9e201-316">SerialNumber.</span><span class="sxs-lookup"><span data-stu-id="9e201-316">SerialNumber.</span></span> <span data-ttu-id="9e201-317">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9e201-317">This property is read-only.</span></span>|
|<span data-ttu-id="9e201-318">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="9e201-318">phoneNumber</span></span>|<span data-ttu-id="9e201-319">String</span><span class="sxs-lookup"><span data-stu-id="9e201-319">String</span></span>|<span data-ttu-id="9e201-320">设备的电话号码。</span><span class="sxs-lookup"><span data-stu-id="9e201-320">Phone number of the device.</span></span> <span data-ttu-id="9e201-321">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9e201-321">This property is read-only.</span></span>|
|<span data-ttu-id="9e201-322">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="9e201-322">androidSecurityPatchLevel</span></span>|<span data-ttu-id="9e201-323">String</span><span class="sxs-lookup"><span data-stu-id="9e201-323">String</span></span>|<span data-ttu-id="9e201-324">Android 安全修补程序级别。</span><span class="sxs-lookup"><span data-stu-id="9e201-324">Android security patch level.</span></span> <span data-ttu-id="9e201-325">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9e201-325">This property is read-only.</span></span>|
|<span data-ttu-id="9e201-326">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="9e201-326">userDisplayName</span></span>|<span data-ttu-id="9e201-327">String</span><span class="sxs-lookup"><span data-stu-id="9e201-327">String</span></span>|<span data-ttu-id="9e201-328">用户显示名称。</span><span class="sxs-lookup"><span data-stu-id="9e201-328">User display name.</span></span> <span data-ttu-id="9e201-329">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9e201-329">This property is read-only.</span></span>|
|<span data-ttu-id="9e201-330">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="9e201-330">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="9e201-331">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="9e201-331">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="9e201-332">ConfigrMgr 客户端启用的功能。</span><span class="sxs-lookup"><span data-stu-id="9e201-332">ConfigrMgr client enabled features.</span></span> <span data-ttu-id="9e201-333">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9e201-333">This property is read-only.</span></span>|
|<span data-ttu-id="9e201-334">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="9e201-334">wiFiMacAddress</span></span>|<span data-ttu-id="9e201-335">String</span><span class="sxs-lookup"><span data-stu-id="9e201-335">String</span></span>|<span data-ttu-id="9e201-336">Wi-fi MAC。</span><span class="sxs-lookup"><span data-stu-id="9e201-336">Wi-Fi MAC.</span></span> <span data-ttu-id="9e201-337">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9e201-337">This property is read-only.</span></span>|
|<span data-ttu-id="9e201-338">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="9e201-338">deviceHealthAttestationState</span></span>|[<span data-ttu-id="9e201-339">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="9e201-339">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="9e201-340">设备运行状况证明状态。</span><span class="sxs-lookup"><span data-stu-id="9e201-340">The device health attestation state.</span></span> <span data-ttu-id="9e201-341">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9e201-341">This property is read-only.</span></span>|
|<span data-ttu-id="9e201-342">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="9e201-342">subscriberCarrier</span></span>|<span data-ttu-id="9e201-343">String</span><span class="sxs-lookup"><span data-stu-id="9e201-343">String</span></span>|<span data-ttu-id="9e201-344">订阅者运营商。</span><span class="sxs-lookup"><span data-stu-id="9e201-344">Subscriber Carrier.</span></span> <span data-ttu-id="9e201-345">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9e201-345">This property is read-only.</span></span>|
|<span data-ttu-id="9e201-346">meid</span><span class="sxs-lookup"><span data-stu-id="9e201-346">meid</span></span>|<span data-ttu-id="9e201-347">String</span><span class="sxs-lookup"><span data-stu-id="9e201-347">String</span></span>|<span data-ttu-id="9e201-348">MEID.</span><span class="sxs-lookup"><span data-stu-id="9e201-348">MEID.</span></span> <span data-ttu-id="9e201-349">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9e201-349">This property is read-only.</span></span>|
|<span data-ttu-id="9e201-350">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="9e201-350">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="9e201-351">Int64</span><span class="sxs-lookup"><span data-stu-id="9e201-351">Int64</span></span>|<span data-ttu-id="9e201-352">总存储量（以字节为单位）。</span><span class="sxs-lookup"><span data-stu-id="9e201-352">Total Storage in Bytes.</span></span> <span data-ttu-id="9e201-353">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9e201-353">This property is read-only.</span></span>|
|<span data-ttu-id="9e201-354">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="9e201-354">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="9e201-355">Int64</span><span class="sxs-lookup"><span data-stu-id="9e201-355">Int64</span></span>|<span data-ttu-id="9e201-356">以字节为单位的可用存储空间。</span><span class="sxs-lookup"><span data-stu-id="9e201-356">Free Storage in Bytes.</span></span> <span data-ttu-id="9e201-357">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9e201-357">This property is read-only.</span></span>|
|<span data-ttu-id="9e201-358">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="9e201-358">managedDeviceName</span></span>|<span data-ttu-id="9e201-359">String</span><span class="sxs-lookup"><span data-stu-id="9e201-359">String</span></span>|<span data-ttu-id="9e201-360">用于识别设备的自动生成的名称。</span><span class="sxs-lookup"><span data-stu-id="9e201-360">Automatically generated name to identify a device.</span></span> <span data-ttu-id="9e201-361">可以覆盖为用户友好名称。</span><span class="sxs-lookup"><span data-stu-id="9e201-361">Can be overwritten to a user friendly name.</span></span>|
|<span data-ttu-id="9e201-362">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="9e201-362">partnerReportedThreatState</span></span>|[<span data-ttu-id="9e201-363">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="9e201-363">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="9e201-364">指示帐户和设备正在使用移动威胁防护合作伙伴时设备的威胁状态。</span><span class="sxs-lookup"><span data-stu-id="9e201-364">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="9e201-365">只读。</span><span class="sxs-lookup"><span data-stu-id="9e201-365">Read Only.</span></span> <span data-ttu-id="9e201-366">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9e201-366">This property is read-only.</span></span> <span data-ttu-id="9e201-367">可取值为：`unknown`、`activated`、`deactivated`、`secured`、`lowSeverity`、`mediumSeverity`、`highSeverity`、`unresponsive`、`compromised`、`misconfigured`。</span><span class="sxs-lookup"><span data-stu-id="9e201-367">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="9e201-368">retireAfterDateTime</span><span class="sxs-lookup"><span data-stu-id="9e201-368">retireAfterDateTime</span></span>|<span data-ttu-id="9e201-369">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e201-369">DateTimeOffset</span></span>|<span data-ttu-id="9e201-370">指示当设备因计划操作而自动停用的时间。</span><span class="sxs-lookup"><span data-stu-id="9e201-370">Indicates the time after when a device will be auto retired because of scheduled action.</span></span> <span data-ttu-id="9e201-371">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9e201-371">This property is read-only.</span></span>|
|<span data-ttu-id="9e201-372">usersLoggedOn</span><span class="sxs-lookup"><span data-stu-id="9e201-372">usersLoggedOn</span></span>|<span data-ttu-id="9e201-373">[loggedOnUser](../resources/intune-devices-loggedonuser.md)集合</span><span class="sxs-lookup"><span data-stu-id="9e201-373">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="9e201-374">指示设备的上次登录用户。</span><span class="sxs-lookup"><span data-stu-id="9e201-374">Indicates the last logged on users of a device.</span></span> <span data-ttu-id="9e201-375">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9e201-375">This property is read-only.</span></span>|
|<span data-ttu-id="9e201-376">preferMdmOverGroupPolicyAppliedDateTime</span><span class="sxs-lookup"><span data-stu-id="9e201-376">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="9e201-377">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e201-377">DateTimeOffset</span></span>|<span data-ttu-id="9e201-378">报告设置了 preferMdmOverGroupPolicy 设置的 DateTime。</span><span class="sxs-lookup"><span data-stu-id="9e201-378">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="9e201-379">设置后，如果存在冲突，Intune MDM 设置将覆盖组策略设置。</span><span class="sxs-lookup"><span data-stu-id="9e201-379">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="9e201-380">只读。</span><span class="sxs-lookup"><span data-stu-id="9e201-380">Read Only.</span></span> <span data-ttu-id="9e201-381">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9e201-381">This property is read-only.</span></span>|
|<span data-ttu-id="9e201-382">autopilotEnrolled</span><span class="sxs-lookup"><span data-stu-id="9e201-382">autopilotEnrolled</span></span>|<span data-ttu-id="9e201-383">布尔值</span><span class="sxs-lookup"><span data-stu-id="9e201-383">Boolean</span></span>|<span data-ttu-id="9e201-384">如果托管设备是通过自动引导注册的，则报告。</span><span class="sxs-lookup"><span data-stu-id="9e201-384">Reports if the managed device is enrolled via auto-pilot.</span></span> <span data-ttu-id="9e201-385">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9e201-385">This property is read-only.</span></span>|
|<span data-ttu-id="9e201-386">requireUserEnrollmentApproval</span><span class="sxs-lookup"><span data-stu-id="9e201-386">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="9e201-387">布尔值</span><span class="sxs-lookup"><span data-stu-id="9e201-387">Boolean</span></span>|<span data-ttu-id="9e201-388">如果托管 iOS 设备是用户审批注册，则报告。</span><span class="sxs-lookup"><span data-stu-id="9e201-388">Reports if the managed iOS device is user approval enrollment.</span></span> <span data-ttu-id="9e201-389">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9e201-389">This property is read-only.</span></span>|
|<span data-ttu-id="9e201-390">managementCertificateExpirationDate</span><span class="sxs-lookup"><span data-stu-id="9e201-390">managementCertificateExpirationDate</span></span>|<span data-ttu-id="9e201-391">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e201-391">DateTimeOffset</span></span>|<span data-ttu-id="9e201-392">报告设备管理证书到期日期。</span><span class="sxs-lookup"><span data-stu-id="9e201-392">Reports device management certificate expiration date.</span></span> <span data-ttu-id="9e201-393">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9e201-393">This property is read-only.</span></span>|
|<span data-ttu-id="9e201-394">iccid</span><span class="sxs-lookup"><span data-stu-id="9e201-394">iccid</span></span>|<span data-ttu-id="9e201-395">String</span><span class="sxs-lookup"><span data-stu-id="9e201-395">String</span></span>|<span data-ttu-id="9e201-396">集成的电路卡标识符，它是 SIM 卡的唯一标识号。</span><span class="sxs-lookup"><span data-stu-id="9e201-396">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span> <span data-ttu-id="9e201-397">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9e201-397">This property is read-only.</span></span>|
|<span data-ttu-id="9e201-398">udid</span><span class="sxs-lookup"><span data-stu-id="9e201-398">udid</span></span>|<span data-ttu-id="9e201-399">String</span><span class="sxs-lookup"><span data-stu-id="9e201-399">String</span></span>|<span data-ttu-id="9e201-400">IOS 和 macOS 设备的唯一设备标识符。</span><span class="sxs-lookup"><span data-stu-id="9e201-400">Unique Device Identifier for iOS and macOS devices.</span></span> <span data-ttu-id="9e201-401">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9e201-401">This property is read-only.</span></span>|
|<span data-ttu-id="9e201-402">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9e201-402">roleScopeTagIds</span></span>|<span data-ttu-id="9e201-403">String collection</span><span class="sxs-lookup"><span data-stu-id="9e201-403">String collection</span></span>|<span data-ttu-id="9e201-404">此设备实例的范围标记 Id 的列表。</span><span class="sxs-lookup"><span data-stu-id="9e201-404">List of Scope Tag IDs for this Device instance.</span></span>|
|<span data-ttu-id="9e201-405">windowsActiveMalwareCount</span><span class="sxs-lookup"><span data-stu-id="9e201-405">windowsActiveMalwareCount</span></span>|<span data-ttu-id="9e201-406">Int32</span><span class="sxs-lookup"><span data-stu-id="9e201-406">Int32</span></span>|<span data-ttu-id="9e201-407">此 windows 设备的活动恶意软件的计数。</span><span class="sxs-lookup"><span data-stu-id="9e201-407">Count of active malware for this windows device.</span></span> <span data-ttu-id="9e201-408">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9e201-408">This property is read-only.</span></span>|
|<span data-ttu-id="9e201-409">windowsRemediatedMalwareCount</span><span class="sxs-lookup"><span data-stu-id="9e201-409">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="9e201-410">Int32</span><span class="sxs-lookup"><span data-stu-id="9e201-410">Int32</span></span>|<span data-ttu-id="9e201-411">此 windows 设备的修正的恶意软件的计数。</span><span class="sxs-lookup"><span data-stu-id="9e201-411">Count of remediated malware for this windows device.</span></span> <span data-ttu-id="9e201-412">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9e201-412">This property is read-only.</span></span>|
|<span data-ttu-id="9e201-413">notes</span><span class="sxs-lookup"><span data-stu-id="9e201-413">notes</span></span>|<span data-ttu-id="9e201-414">String</span><span class="sxs-lookup"><span data-stu-id="9e201-414">String</span></span>|<span data-ttu-id="9e201-415">IT 管理员创建的设备上的注释</span><span class="sxs-lookup"><span data-stu-id="9e201-415">Notes on the device created by IT Admin</span></span>|
|<span data-ttu-id="9e201-416">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="9e201-416">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="9e201-417">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="9e201-417">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="9e201-418">Configuration manager 客户端运行状况状态，仅对由 MDM/ConfigMgr 代理管理的设备有效</span><span class="sxs-lookup"><span data-stu-id="9e201-418">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent</span></span>|
|<span data-ttu-id="9e201-419">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="9e201-419">configurationManagerClientInformation</span></span>|[<span data-ttu-id="9e201-420">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="9e201-420">configurationManagerClientInformation</span></span>](../resources/intune-devices-configurationmanagerclientinformation.md)|<span data-ttu-id="9e201-421">Configuration manager 客户端信息，仅对受 ConfigMgr 代理管理、duel 管理或三方管理的设备有效</span><span class="sxs-lookup"><span data-stu-id="9e201-421">Configuration manager client information, valid only for devices managed, duel-managed or tri-managed by ConfigMgr Agent</span></span>|
|<span data-ttu-id="9e201-422">ethernetMacAddress</span><span class="sxs-lookup"><span data-stu-id="9e201-422">ethernetMacAddress</span></span>|<span data-ttu-id="9e201-423">String</span><span class="sxs-lookup"><span data-stu-id="9e201-423">String</span></span>|<span data-ttu-id="9e201-424">以太网 MAC。</span><span class="sxs-lookup"><span data-stu-id="9e201-424">Ethernet MAC.</span></span> <span data-ttu-id="9e201-425">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9e201-425">This property is read-only.</span></span>|
|<span data-ttu-id="9e201-426">physicalMemoryInBytes</span><span class="sxs-lookup"><span data-stu-id="9e201-426">physicalMemoryInBytes</span></span>|<span data-ttu-id="9e201-427">Int64</span><span class="sxs-lookup"><span data-stu-id="9e201-427">Int64</span></span>|<span data-ttu-id="9e201-428">内存总量（以字节为单位）。</span><span class="sxs-lookup"><span data-stu-id="9e201-428">Total Memory in Bytes.</span></span> <span data-ttu-id="9e201-429">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9e201-429">This property is read-only.</span></span>|
|<span data-ttu-id="9e201-430">processorArchitecture</span><span class="sxs-lookup"><span data-stu-id="9e201-430">processorArchitecture</span></span>|[<span data-ttu-id="9e201-431">managedDeviceArchitecture</span><span class="sxs-lookup"><span data-stu-id="9e201-431">managedDeviceArchitecture</span></span>](../resources/intune-devices-manageddevicearchitecture.md)|<span data-ttu-id="9e201-432">处理器体系结构。</span><span class="sxs-lookup"><span data-stu-id="9e201-432">Processor architecture.</span></span> <span data-ttu-id="9e201-433">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9e201-433">This property is read-only.</span></span> <span data-ttu-id="9e201-434">可取值为：`unknown`、`x86`、`x64`、`arm`、`arM64`。</span><span class="sxs-lookup"><span data-stu-id="9e201-434">Possible values are: `unknown`, `x86`, `x64`, `arm`, `arM64`.</span></span>|



## <a name="response"></a><span data-ttu-id="9e201-435">响应</span><span class="sxs-lookup"><span data-stu-id="9e201-435">Response</span></span>
<span data-ttu-id="9e201-436">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [managedDevice](../resources/intune-devices-manageddevice.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9e201-436">If successful, this method returns a `200 OK` response code and an updated [managedDevice](../resources/intune-devices-manageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9e201-437">示例</span><span class="sxs-lookup"><span data-stu-id="9e201-437">Example</span></span>

### <a name="request"></a><span data-ttu-id="9e201-438">请求</span><span class="sxs-lookup"><span data-stu-id="9e201-438">Request</span></span>
<span data-ttu-id="9e201-439">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9e201-439">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}
Content-type: application/json
Content-length: 7658

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
    "deviceGuardLocalSystemAuthorityCredentialGuardState": "rebootRequired",
    "osBuildNumber": "Os Build Number value"
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
  "processorArchitecture": "x86"
}
```

### <a name="response"></a><span data-ttu-id="9e201-440">响应</span><span class="sxs-lookup"><span data-stu-id="9e201-440">Response</span></span>
<span data-ttu-id="9e201-p170">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9e201-p170">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 7707

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
    "deviceGuardLocalSystemAuthorityCredentialGuardState": "rebootRequired",
    "osBuildNumber": "Os Build Number value"
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
  "processorArchitecture": "x86"
}
```




