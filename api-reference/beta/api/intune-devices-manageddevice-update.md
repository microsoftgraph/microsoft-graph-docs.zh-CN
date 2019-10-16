---
title: 更新 managedDevice
description: 更新 managedDevice 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a51ae80b13e1b6a0a571e1213c0c7638d945f3c5
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37528239"
---
# <a name="update-manageddevice"></a><span data-ttu-id="53ee0-103">更新 managedDevice</span><span class="sxs-lookup"><span data-stu-id="53ee0-103">Update managedDevice</span></span>

> <span data-ttu-id="53ee0-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="53ee0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="53ee0-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="53ee0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="53ee0-106">更新 [managedDevice](../resources/intune-devices-manageddevice.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="53ee0-106">Update the properties of a [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="53ee0-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="53ee0-107">Prerequisites</span></span>
<span data-ttu-id="53ee0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="53ee0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53ee0-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="53ee0-110">Permission type</span></span>|<span data-ttu-id="53ee0-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="53ee0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="53ee0-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="53ee0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="53ee0-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53ee0-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="53ee0-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="53ee0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="53ee0-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="53ee0-115">Not supported.</span></span>|
|<span data-ttu-id="53ee0-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="53ee0-116">Application</span></span>|<span data-ttu-id="53ee0-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53ee0-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="53ee0-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="53ee0-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="53ee0-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="53ee0-119">Request headers</span></span>
|<span data-ttu-id="53ee0-120">标头</span><span class="sxs-lookup"><span data-stu-id="53ee0-120">Header</span></span>|<span data-ttu-id="53ee0-121">值</span><span class="sxs-lookup"><span data-stu-id="53ee0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="53ee0-122">授权</span><span class="sxs-lookup"><span data-stu-id="53ee0-122">Authorization</span></span>|<span data-ttu-id="53ee0-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="53ee0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="53ee0-124">接受</span><span class="sxs-lookup"><span data-stu-id="53ee0-124">Accept</span></span>|<span data-ttu-id="53ee0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="53ee0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="53ee0-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="53ee0-126">Request body</span></span>
<span data-ttu-id="53ee0-127">在请求正文中，提供 [managedDevice](../resources/intune-devices-manageddevice.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="53ee0-127">In the request body, supply a JSON representation for the [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>

<span data-ttu-id="53ee0-128">下表显示创建 [managedDevice](../resources/intune-devices-manageddevice.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="53ee0-128">The following table shows the properties that are required when you create the [managedDevice](../resources/intune-devices-manageddevice.md).</span></span>

|<span data-ttu-id="53ee0-129">属性</span><span class="sxs-lookup"><span data-stu-id="53ee0-129">Property</span></span>|<span data-ttu-id="53ee0-130">类型</span><span class="sxs-lookup"><span data-stu-id="53ee0-130">Type</span></span>|<span data-ttu-id="53ee0-131">说明</span><span class="sxs-lookup"><span data-stu-id="53ee0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53ee0-132">id</span><span class="sxs-lookup"><span data-stu-id="53ee0-132">id</span></span>|<span data-ttu-id="53ee0-133">字符串</span><span class="sxs-lookup"><span data-stu-id="53ee0-133">String</span></span>|<span data-ttu-id="53ee0-134">设备的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="53ee0-134">Unique Identifier for the device.</span></span> <span data-ttu-id="53ee0-135">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="53ee0-135">This property is read-only.</span></span>|
|<span data-ttu-id="53ee0-136">userId</span><span class="sxs-lookup"><span data-stu-id="53ee0-136">userId</span></span>|<span data-ttu-id="53ee0-137">String</span><span class="sxs-lookup"><span data-stu-id="53ee0-137">String</span></span>|<span data-ttu-id="53ee0-138">与设备关联的用户的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="53ee0-138">Unique Identifier for the user associated with the device.</span></span> <span data-ttu-id="53ee0-139">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="53ee0-139">This property is read-only.</span></span>|
|<span data-ttu-id="53ee0-140">deviceName</span><span class="sxs-lookup"><span data-stu-id="53ee0-140">deviceName</span></span>|<span data-ttu-id="53ee0-141">字符串</span><span class="sxs-lookup"><span data-stu-id="53ee0-141">String</span></span>|<span data-ttu-id="53ee0-142">设备的名称。</span><span class="sxs-lookup"><span data-stu-id="53ee0-142">Name of the device.</span></span> <span data-ttu-id="53ee0-143">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="53ee0-143">This property is read-only.</span></span>|
|<span data-ttu-id="53ee0-144">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="53ee0-144">hardwareInformation</span></span>|[<span data-ttu-id="53ee0-145">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="53ee0-145">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="53ee0-146">设备的 hardward 详细信息。</span><span class="sxs-lookup"><span data-stu-id="53ee0-146">The hardward details for the device.</span></span>  <span data-ttu-id="53ee0-147">包括存储空间、制造商、序列号等信息。此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="53ee0-147">Includes information such as storage space, manufacturer, serial number, etc. This property is read-only.</span></span>|
|<span data-ttu-id="53ee0-148">所有者</span><span class="sxs-lookup"><span data-stu-id="53ee0-148">ownerType</span></span>|[<span data-ttu-id="53ee0-149">所有者</span><span class="sxs-lookup"><span data-stu-id="53ee0-149">ownerType</span></span>](../resources/intune-devices-ownertype.md)|<span data-ttu-id="53ee0-150">设备的所有权。</span><span class="sxs-lookup"><span data-stu-id="53ee0-150">Ownership of the device.</span></span> <span data-ttu-id="53ee0-151">可以是 "公司" 或 "个人"。</span><span class="sxs-lookup"><span data-stu-id="53ee0-151">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="53ee0-152">可取值为：`unknown`、`company`、`personal`。</span><span class="sxs-lookup"><span data-stu-id="53ee0-152">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="53ee0-153">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="53ee0-153">managedDeviceOwnerType</span></span>|[<span data-ttu-id="53ee0-154">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="53ee0-154">managedDeviceOwnerType</span></span>](../resources/intune-shared-manageddeviceownertype.md)|<span data-ttu-id="53ee0-155">设备的所有权。</span><span class="sxs-lookup"><span data-stu-id="53ee0-155">Ownership of the device.</span></span> <span data-ttu-id="53ee0-156">可以是 "公司" 或 "个人"。</span><span class="sxs-lookup"><span data-stu-id="53ee0-156">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="53ee0-157">可取值为：`unknown`、`company`、`personal`。</span><span class="sxs-lookup"><span data-stu-id="53ee0-157">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="53ee0-158">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="53ee0-158">deviceActionResults</span></span>|<span data-ttu-id="53ee0-159">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) 集合</span><span class="sxs-lookup"><span data-stu-id="53ee0-159">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="53ee0-160">ComplexType deviceActionResult 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="53ee0-160">List of ComplexType deviceActionResult objects.</span></span> <span data-ttu-id="53ee0-161">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="53ee0-161">This property is read-only.</span></span>|
|<span data-ttu-id="53ee0-162">managementState</span><span class="sxs-lookup"><span data-stu-id="53ee0-162">managementState</span></span>|[<span data-ttu-id="53ee0-163">managementState</span><span class="sxs-lookup"><span data-stu-id="53ee0-163">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="53ee0-164">设备的管理状态。</span><span class="sxs-lookup"><span data-stu-id="53ee0-164">Management state of the device.</span></span> <span data-ttu-id="53ee0-165">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="53ee0-165">This property is read-only.</span></span> <span data-ttu-id="53ee0-166">可取值为：`managed`、`retirePending`、`retireFailed`、`wipePending`、`wipeFailed`、`unhealthy`、`deletePending`、`retireIssued`、`wipeIssued`、`wipeCanceled`、`retireCanceled`、`discovered`。</span><span class="sxs-lookup"><span data-stu-id="53ee0-166">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="53ee0-167">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="53ee0-167">enrolledDateTime</span></span>|<span data-ttu-id="53ee0-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53ee0-168">DateTimeOffset</span></span>|<span data-ttu-id="53ee0-169">设备的注册时间。</span><span class="sxs-lookup"><span data-stu-id="53ee0-169">Enrollment time of the device.</span></span> <span data-ttu-id="53ee0-170">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="53ee0-170">This property is read-only.</span></span>|
|<span data-ttu-id="53ee0-171">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="53ee0-171">lastSyncDateTime</span></span>|<span data-ttu-id="53ee0-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53ee0-172">DateTimeOffset</span></span>|<span data-ttu-id="53ee0-173">设备上次成功完成与 Intune 同步的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="53ee0-173">The date and time that the device last completed a successful sync with Intune.</span></span> <span data-ttu-id="53ee0-174">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="53ee0-174">This property is read-only.</span></span>|
|<span data-ttu-id="53ee0-175">chassisType</span><span class="sxs-lookup"><span data-stu-id="53ee0-175">chassisType</span></span>|[<span data-ttu-id="53ee0-176">chassisType</span><span class="sxs-lookup"><span data-stu-id="53ee0-176">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="53ee0-177">设备的机箱类型。</span><span class="sxs-lookup"><span data-stu-id="53ee0-177">Chassis type of the device.</span></span> <span data-ttu-id="53ee0-178">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="53ee0-178">This property is read-only.</span></span> <span data-ttu-id="53ee0-179">可取值为：`unknown`、`desktop`、`laptop`、`worksWorkstation`、`enterpriseServer`、`phone`、`tablet`、`mobileOther`、`mobileUnknown`。</span><span class="sxs-lookup"><span data-stu-id="53ee0-179">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="53ee0-180">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="53ee0-180">operatingSystem</span></span>|<span data-ttu-id="53ee0-181">字符串</span><span class="sxs-lookup"><span data-stu-id="53ee0-181">String</span></span>|<span data-ttu-id="53ee0-182">设备的操作系统。</span><span class="sxs-lookup"><span data-stu-id="53ee0-182">Operating system of the device.</span></span> <span data-ttu-id="53ee0-183">Windows、iOS 等。此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="53ee0-183">Windows, iOS, etc. This property is read-only.</span></span>|
|<span data-ttu-id="53ee0-184">deviceType</span><span class="sxs-lookup"><span data-stu-id="53ee0-184">deviceType</span></span>|[<span data-ttu-id="53ee0-185">deviceType</span><span class="sxs-lookup"><span data-stu-id="53ee0-185">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="53ee0-186">设备的平台。</span><span class="sxs-lookup"><span data-stu-id="53ee0-186">Platform of the device.</span></span> <span data-ttu-id="53ee0-187">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="53ee0-187">This property is read-only.</span></span> <span data-ttu-id="53ee0-188">可能的值为`desktop`： `windowsRT`、 `winMO6`、 `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer`、、、、、、、、、、、、、、、、 `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="53ee0-188">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="53ee0-189">complianceState</span><span class="sxs-lookup"><span data-stu-id="53ee0-189">complianceState</span></span>|[<span data-ttu-id="53ee0-190">complianceState</span><span class="sxs-lookup"><span data-stu-id="53ee0-190">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="53ee0-191">设备的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="53ee0-191">Compliance state of the device.</span></span> <span data-ttu-id="53ee0-192">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="53ee0-192">This property is read-only.</span></span> <span data-ttu-id="53ee0-193">可取值为：`unknown`、`compliant`、`noncompliant`、`conflict`、`error`、`inGracePeriod`、`configManager`。</span><span class="sxs-lookup"><span data-stu-id="53ee0-193">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="53ee0-194">jailBroken</span><span class="sxs-lookup"><span data-stu-id="53ee0-194">jailBroken</span></span>|<span data-ttu-id="53ee0-195">字符串</span><span class="sxs-lookup"><span data-stu-id="53ee0-195">String</span></span>|<span data-ttu-id="53ee0-196">设备是否已越狱或取得 root 权限。</span><span class="sxs-lookup"><span data-stu-id="53ee0-196">whether the device is jail broken or rooted.</span></span> <span data-ttu-id="53ee0-197">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="53ee0-197">This property is read-only.</span></span>|
|<span data-ttu-id="53ee0-198">managementAgent</span><span class="sxs-lookup"><span data-stu-id="53ee0-198">managementAgent</span></span>|[<span data-ttu-id="53ee0-199">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="53ee0-199">managementAgentType</span></span>](../resources/intune-devices-managementagenttype.md)|<span data-ttu-id="53ee0-200">设备的管理通道。</span><span class="sxs-lookup"><span data-stu-id="53ee0-200">Management channel of the device.</span></span> <span data-ttu-id="53ee0-201">Intune、EAS 等。此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="53ee0-201">Intune, EAS, etc. This property is read-only.</span></span> <span data-ttu-id="53ee0-202">可取值为：`eas`、`mdm`、`easMdm`、`intuneClient`、`easIntuneClient`、`configurationManagerClient`、`configurationManagerClientMdm`、`configurationManagerClientMdmEas`、`unknown`、`jamf`、`googleCloudDevicePolicyController`、`microsoft365ManagedMdm`。</span><span class="sxs-lookup"><span data-stu-id="53ee0-202">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span></span>|
|<span data-ttu-id="53ee0-203">osVersion</span><span class="sxs-lookup"><span data-stu-id="53ee0-203">osVersion</span></span>|<span data-ttu-id="53ee0-204">字符串</span><span class="sxs-lookup"><span data-stu-id="53ee0-204">String</span></span>|<span data-ttu-id="53ee0-205">设备的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="53ee0-205">Operating system version of the device.</span></span> <span data-ttu-id="53ee0-206">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="53ee0-206">This property is read-only.</span></span>|
|<span data-ttu-id="53ee0-207">easActivated</span><span class="sxs-lookup"><span data-stu-id="53ee0-207">easActivated</span></span>|<span data-ttu-id="53ee0-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="53ee0-208">Boolean</span></span>|<span data-ttu-id="53ee0-209">设备是否已激活 Exchange ActiveSync。</span><span class="sxs-lookup"><span data-stu-id="53ee0-209">Whether the device is Exchange ActiveSync activated.</span></span> <span data-ttu-id="53ee0-210">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="53ee0-210">This property is read-only.</span></span>|
|<span data-ttu-id="53ee0-211">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="53ee0-211">easDeviceId</span></span>|<span data-ttu-id="53ee0-212">String</span><span class="sxs-lookup"><span data-stu-id="53ee0-212">String</span></span>|<span data-ttu-id="53ee0-213">设备的 Exchange ActiveSync ID。</span><span class="sxs-lookup"><span data-stu-id="53ee0-213">Exchange ActiveSync Id of the device.</span></span> <span data-ttu-id="53ee0-214">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="53ee0-214">This property is read-only.</span></span>|
|<span data-ttu-id="53ee0-215">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="53ee0-215">easActivationDateTime</span></span>|<span data-ttu-id="53ee0-216">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53ee0-216">DateTimeOffset</span></span>|<span data-ttu-id="53ee0-217">设备的 Exchange ActivationSync 激活时间。</span><span class="sxs-lookup"><span data-stu-id="53ee0-217">Exchange ActivationSync activation time of the device.</span></span> <span data-ttu-id="53ee0-218">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="53ee0-218">This property is read-only.</span></span>|
|<span data-ttu-id="53ee0-219">aadRegistered</span><span class="sxs-lookup"><span data-stu-id="53ee0-219">aadRegistered</span></span>|<span data-ttu-id="53ee0-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="53ee0-220">Boolean</span></span>|<span data-ttu-id="53ee0-221">设备是否已注册 Azure Active Directory。</span><span class="sxs-lookup"><span data-stu-id="53ee0-221">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="53ee0-222">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="53ee0-222">This property is read-only.</span></span>|
|<span data-ttu-id="53ee0-223">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="53ee0-223">azureADRegistered</span></span>|<span data-ttu-id="53ee0-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="53ee0-224">Boolean</span></span>|<span data-ttu-id="53ee0-225">设备是否已注册 Azure Active Directory。</span><span class="sxs-lookup"><span data-stu-id="53ee0-225">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="53ee0-226">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="53ee0-226">This property is read-only.</span></span>|
|<span data-ttu-id="53ee0-227">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="53ee0-227">deviceEnrollmentType</span></span>|[<span data-ttu-id="53ee0-228">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="53ee0-228">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="53ee0-229">设备的注册类型。</span><span class="sxs-lookup"><span data-stu-id="53ee0-229">Enrollment type of the device.</span></span> <span data-ttu-id="53ee0-230">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="53ee0-230">This property is read-only.</span></span> <span data-ttu-id="53ee0-231">可取值为：`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement`、`appleUserEnrollment`、`appleUserEnrollmentWithServiceAccount`。</span><span class="sxs-lookup"><span data-stu-id="53ee0-231">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`.</span></span>|
|<span data-ttu-id="53ee0-232">lostModeState</span><span class="sxs-lookup"><span data-stu-id="53ee0-232">lostModeState</span></span>|[<span data-ttu-id="53ee0-233">lostModeState</span><span class="sxs-lookup"><span data-stu-id="53ee0-233">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="53ee0-234">指示是否已启用或禁用了丢失模式。</span><span class="sxs-lookup"><span data-stu-id="53ee0-234">Indicates if Lost mode is enabled or disabled.</span></span> <span data-ttu-id="53ee0-235">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="53ee0-235">This property is read-only.</span></span> <span data-ttu-id="53ee0-236">可取值为：`disabled`、`enabled`。</span><span class="sxs-lookup"><span data-stu-id="53ee0-236">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="53ee0-237">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="53ee0-237">activationLockBypassCode</span></span>|<span data-ttu-id="53ee0-238">字符串</span><span class="sxs-lookup"><span data-stu-id="53ee0-238">String</span></span>|<span data-ttu-id="53ee0-239">允许绕过设备上的激活锁的代码。</span><span class="sxs-lookup"><span data-stu-id="53ee0-239">Code that allows the Activation Lock on a device to be bypassed.</span></span> <span data-ttu-id="53ee0-240">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="53ee0-240">This property is read-only.</span></span>|
|<span data-ttu-id="53ee0-241">emailAddress</span><span class="sxs-lookup"><span data-stu-id="53ee0-241">emailAddress</span></span>|<span data-ttu-id="53ee0-242">字符串</span><span class="sxs-lookup"><span data-stu-id="53ee0-242">String</span></span>|<span data-ttu-id="53ee0-243">与设备关联的用户的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="53ee0-243">Email(s) for the user associated with the device.</span></span> <span data-ttu-id="53ee0-244">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="53ee0-244">This property is read-only.</span></span>|
|<span data-ttu-id="53ee0-245">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="53ee0-245">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="53ee0-246">字符串</span><span class="sxs-lookup"><span data-stu-id="53ee0-246">String</span></span>|<span data-ttu-id="53ee0-247">Azure Active Directory 设备的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="53ee0-247">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="53ee0-248">只读。</span><span class="sxs-lookup"><span data-stu-id="53ee0-248">Read only.</span></span> <span data-ttu-id="53ee0-249">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="53ee0-249">This property is read-only.</span></span>|
|<span data-ttu-id="53ee0-250">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="53ee0-250">azureADDeviceId</span></span>|<span data-ttu-id="53ee0-251">字符串</span><span class="sxs-lookup"><span data-stu-id="53ee0-251">String</span></span>|<span data-ttu-id="53ee0-252">Azure Active Directory 设备的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="53ee0-252">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="53ee0-253">只读。</span><span class="sxs-lookup"><span data-stu-id="53ee0-253">Read only.</span></span> <span data-ttu-id="53ee0-254">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="53ee0-254">This property is read-only.</span></span>|
|<span data-ttu-id="53ee0-255">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="53ee0-255">deviceRegistrationState</span></span>|[<span data-ttu-id="53ee0-256">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="53ee0-256">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="53ee0-257">设备注册状态。</span><span class="sxs-lookup"><span data-stu-id="53ee0-257">Device registration state.</span></span> <span data-ttu-id="53ee0-258">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="53ee0-258">This property is read-only.</span></span> <span data-ttu-id="53ee0-259">可取值为：`notRegistered`、`registered`、`revoked`、`keyConflict`、`approvalPending`、`certificateReset`、`notRegisteredPendingEnrollment`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="53ee0-259">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="53ee0-260">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="53ee0-260">deviceCategoryDisplayName</span></span>|<span data-ttu-id="53ee0-261">字符串</span><span class="sxs-lookup"><span data-stu-id="53ee0-261">String</span></span>|<span data-ttu-id="53ee0-262">设备类别显示名称。</span><span class="sxs-lookup"><span data-stu-id="53ee0-262">Device category display name.</span></span> <span data-ttu-id="53ee0-263">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="53ee0-263">This property is read-only.</span></span>|
|<span data-ttu-id="53ee0-264">isSupervised</span><span class="sxs-lookup"><span data-stu-id="53ee0-264">isSupervised</span></span>|<span data-ttu-id="53ee0-265">Boolean</span><span class="sxs-lookup"><span data-stu-id="53ee0-265">Boolean</span></span>|<span data-ttu-id="53ee0-266">设备监督状态。</span><span class="sxs-lookup"><span data-stu-id="53ee0-266">Device supervised status.</span></span> <span data-ttu-id="53ee0-267">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="53ee0-267">This property is read-only.</span></span>|
|<span data-ttu-id="53ee0-268">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="53ee0-268">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="53ee0-269">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53ee0-269">DateTimeOffset</span></span>|<span data-ttu-id="53ee0-270">设备上次与 Exchange 联系的时间。</span><span class="sxs-lookup"><span data-stu-id="53ee0-270">Last time the device contacted Exchange.</span></span> <span data-ttu-id="53ee0-271">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="53ee0-271">This property is read-only.</span></span>|
|<span data-ttu-id="53ee0-272">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="53ee0-272">exchangeAccessState</span></span>|[<span data-ttu-id="53ee0-273">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="53ee0-273">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="53ee0-274">Exchange 中设备的访问状态。</span><span class="sxs-lookup"><span data-stu-id="53ee0-274">The Access State of the device in Exchange.</span></span> <span data-ttu-id="53ee0-275">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="53ee0-275">This property is read-only.</span></span> <span data-ttu-id="53ee0-276">可取值为：`none`、`unknown`、`allowed`、`blocked`、`quarantined`。</span><span class="sxs-lookup"><span data-stu-id="53ee0-276">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="53ee0-277">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="53ee0-277">exchangeAccessStateReason</span></span>|[<span data-ttu-id="53ee0-278">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="53ee0-278">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="53ee0-279">Exchange 中设备访问状态的出现原因。</span><span class="sxs-lookup"><span data-stu-id="53ee0-279">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="53ee0-280">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="53ee0-280">This property is read-only.</span></span> <span data-ttu-id="53ee0-281">可取值为：`none`、`unknown`、`exchangeGlobalRule`、`exchangeIndividualRule`、`exchangeDeviceRule`、`exchangeUpgrade`、`exchangeMailboxPolicy`、`other`、`compliant`、`notCompliant`、`notEnrolled`、`unknownLocation`、`mfaRequired`、`azureADBlockDueToAccessPolicy`、`compromisedPassword`、`deviceNotKnownWithManagedApp`。</span><span class="sxs-lookup"><span data-stu-id="53ee0-281">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="53ee0-282">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="53ee0-282">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="53ee0-283">字符串</span><span class="sxs-lookup"><span data-stu-id="53ee0-283">String</span></span>|<span data-ttu-id="53ee0-284">允许与设备建立远程协助会话的 URL。</span><span class="sxs-lookup"><span data-stu-id="53ee0-284">Url that allows a Remote Assistance session to be established with the device.</span></span> <span data-ttu-id="53ee0-285">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="53ee0-285">This property is read-only.</span></span>|
|<span data-ttu-id="53ee0-286">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="53ee0-286">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="53ee0-287">String</span><span class="sxs-lookup"><span data-stu-id="53ee0-287">String</span></span>|<span data-ttu-id="53ee0-288">用于在创建远程协助会话对象时识别问题的错误字符串。</span><span class="sxs-lookup"><span data-stu-id="53ee0-288">An error string that identifies issues when creating Remote Assistance session objects.</span></span> <span data-ttu-id="53ee0-289">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="53ee0-289">This property is read-only.</span></span>|
|<span data-ttu-id="53ee0-290">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="53ee0-290">isEncrypted</span></span>|<span data-ttu-id="53ee0-291">Boolean</span><span class="sxs-lookup"><span data-stu-id="53ee0-291">Boolean</span></span>|<span data-ttu-id="53ee0-292">设备加密状态。</span><span class="sxs-lookup"><span data-stu-id="53ee0-292">Device encryption status.</span></span> <span data-ttu-id="53ee0-293">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="53ee0-293">This property is read-only.</span></span>|
|<span data-ttu-id="53ee0-294">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="53ee0-294">userPrincipalName</span></span>|<span data-ttu-id="53ee0-295">字符串</span><span class="sxs-lookup"><span data-stu-id="53ee0-295">String</span></span>|<span data-ttu-id="53ee0-296">设备用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="53ee0-296">Device user principal name.</span></span> <span data-ttu-id="53ee0-297">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="53ee0-297">This property is read-only.</span></span>|
|<span data-ttu-id="53ee0-298">model</span><span class="sxs-lookup"><span data-stu-id="53ee0-298">model</span></span>|<span data-ttu-id="53ee0-299">字符串</span><span class="sxs-lookup"><span data-stu-id="53ee0-299">String</span></span>|<span data-ttu-id="53ee0-300">设备的模型。</span><span class="sxs-lookup"><span data-stu-id="53ee0-300">Model of the device.</span></span> <span data-ttu-id="53ee0-301">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="53ee0-301">This property is read-only.</span></span>|
|<span data-ttu-id="53ee0-302">manufacturer</span><span class="sxs-lookup"><span data-stu-id="53ee0-302">manufacturer</span></span>|<span data-ttu-id="53ee0-303">字符串</span><span class="sxs-lookup"><span data-stu-id="53ee0-303">String</span></span>|<span data-ttu-id="53ee0-304">设备的制造商。</span><span class="sxs-lookup"><span data-stu-id="53ee0-304">Manufacturer of the device.</span></span> <span data-ttu-id="53ee0-305">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="53ee0-305">This property is read-only.</span></span>|
|<span data-ttu-id="53ee0-306">imei</span><span class="sxs-lookup"><span data-stu-id="53ee0-306">imei</span></span>|<span data-ttu-id="53ee0-307">字符串</span><span class="sxs-lookup"><span data-stu-id="53ee0-307">String</span></span>|<span data-ttu-id="53ee0-308">IMEI.</span><span class="sxs-lookup"><span data-stu-id="53ee0-308">IMEI.</span></span> <span data-ttu-id="53ee0-309">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="53ee0-309">This property is read-only.</span></span>|
|<span data-ttu-id="53ee0-310">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="53ee0-310">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="53ee0-311">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53ee0-311">DateTimeOffset</span></span>|<span data-ttu-id="53ee0-312">设备符合性宽限期到期时的日期时间。</span><span class="sxs-lookup"><span data-stu-id="53ee0-312">The DateTime when device compliance grace period expires.</span></span> <span data-ttu-id="53ee0-313">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="53ee0-313">This property is read-only.</span></span>|
|<span data-ttu-id="53ee0-314">serialNumber</span><span class="sxs-lookup"><span data-stu-id="53ee0-314">serialNumber</span></span>|<span data-ttu-id="53ee0-315">字符串</span><span class="sxs-lookup"><span data-stu-id="53ee0-315">String</span></span>|<span data-ttu-id="53ee0-316">SerialNumber.</span><span class="sxs-lookup"><span data-stu-id="53ee0-316">SerialNumber.</span></span> <span data-ttu-id="53ee0-317">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="53ee0-317">This property is read-only.</span></span>|
|<span data-ttu-id="53ee0-318">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="53ee0-318">phoneNumber</span></span>|<span data-ttu-id="53ee0-319">String</span><span class="sxs-lookup"><span data-stu-id="53ee0-319">String</span></span>|<span data-ttu-id="53ee0-320">设备的电话号码。</span><span class="sxs-lookup"><span data-stu-id="53ee0-320">Phone number of the device.</span></span> <span data-ttu-id="53ee0-321">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="53ee0-321">This property is read-only.</span></span>|
|<span data-ttu-id="53ee0-322">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="53ee0-322">androidSecurityPatchLevel</span></span>|<span data-ttu-id="53ee0-323">字符串</span><span class="sxs-lookup"><span data-stu-id="53ee0-323">String</span></span>|<span data-ttu-id="53ee0-324">Android 安全修补程序级别。</span><span class="sxs-lookup"><span data-stu-id="53ee0-324">Android security patch level.</span></span> <span data-ttu-id="53ee0-325">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="53ee0-325">This property is read-only.</span></span>|
|<span data-ttu-id="53ee0-326">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="53ee0-326">userDisplayName</span></span>|<span data-ttu-id="53ee0-327">String</span><span class="sxs-lookup"><span data-stu-id="53ee0-327">String</span></span>|<span data-ttu-id="53ee0-328">用户显示名称。</span><span class="sxs-lookup"><span data-stu-id="53ee0-328">User display name.</span></span> <span data-ttu-id="53ee0-329">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="53ee0-329">This property is read-only.</span></span>|
|<span data-ttu-id="53ee0-330">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="53ee0-330">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="53ee0-331">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="53ee0-331">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="53ee0-332">ConfigrMgr 客户端启用的功能。</span><span class="sxs-lookup"><span data-stu-id="53ee0-332">ConfigrMgr client enabled features.</span></span> <span data-ttu-id="53ee0-333">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="53ee0-333">This property is read-only.</span></span>|
|<span data-ttu-id="53ee0-334">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="53ee0-334">wiFiMacAddress</span></span>|<span data-ttu-id="53ee0-335">字符串</span><span class="sxs-lookup"><span data-stu-id="53ee0-335">String</span></span>|<span data-ttu-id="53ee0-336">Wi-fi MAC。</span><span class="sxs-lookup"><span data-stu-id="53ee0-336">Wi-Fi MAC.</span></span> <span data-ttu-id="53ee0-337">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="53ee0-337">This property is read-only.</span></span>|
|<span data-ttu-id="53ee0-338">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="53ee0-338">deviceHealthAttestationState</span></span>|[<span data-ttu-id="53ee0-339">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="53ee0-339">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="53ee0-340">设备运行状况证明状态。</span><span class="sxs-lookup"><span data-stu-id="53ee0-340">The device health attestation state.</span></span> <span data-ttu-id="53ee0-341">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="53ee0-341">This property is read-only.</span></span>|
|<span data-ttu-id="53ee0-342">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="53ee0-342">subscriberCarrier</span></span>|<span data-ttu-id="53ee0-343">字符串</span><span class="sxs-lookup"><span data-stu-id="53ee0-343">String</span></span>|<span data-ttu-id="53ee0-344">订阅者运营商。</span><span class="sxs-lookup"><span data-stu-id="53ee0-344">Subscriber Carrier.</span></span> <span data-ttu-id="53ee0-345">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="53ee0-345">This property is read-only.</span></span>|
|<span data-ttu-id="53ee0-346">meid</span><span class="sxs-lookup"><span data-stu-id="53ee0-346">meid</span></span>|<span data-ttu-id="53ee0-347">字符串</span><span class="sxs-lookup"><span data-stu-id="53ee0-347">String</span></span>|<span data-ttu-id="53ee0-348">MEID.</span><span class="sxs-lookup"><span data-stu-id="53ee0-348">MEID.</span></span> <span data-ttu-id="53ee0-349">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="53ee0-349">This property is read-only.</span></span>|
|<span data-ttu-id="53ee0-350">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="53ee0-350">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="53ee0-351">Int64</span><span class="sxs-lookup"><span data-stu-id="53ee0-351">Int64</span></span>|<span data-ttu-id="53ee0-352">总存储量（以字节为单位）。</span><span class="sxs-lookup"><span data-stu-id="53ee0-352">Total Storage in Bytes.</span></span> <span data-ttu-id="53ee0-353">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="53ee0-353">This property is read-only.</span></span>|
|<span data-ttu-id="53ee0-354">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="53ee0-354">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="53ee0-355">Int64</span><span class="sxs-lookup"><span data-stu-id="53ee0-355">Int64</span></span>|<span data-ttu-id="53ee0-356">以字节为单位的可用存储空间。</span><span class="sxs-lookup"><span data-stu-id="53ee0-356">Free Storage in Bytes.</span></span> <span data-ttu-id="53ee0-357">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="53ee0-357">This property is read-only.</span></span>|
|<span data-ttu-id="53ee0-358">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="53ee0-358">managedDeviceName</span></span>|<span data-ttu-id="53ee0-359">String</span><span class="sxs-lookup"><span data-stu-id="53ee0-359">String</span></span>|<span data-ttu-id="53ee0-360">用于识别设备的自动生成的名称。</span><span class="sxs-lookup"><span data-stu-id="53ee0-360">Automatically generated name to identify a device.</span></span> <span data-ttu-id="53ee0-361">可以覆盖为用户友好名称。</span><span class="sxs-lookup"><span data-stu-id="53ee0-361">Can be overwritten to a user friendly name.</span></span>|
|<span data-ttu-id="53ee0-362">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="53ee0-362">partnerReportedThreatState</span></span>|[<span data-ttu-id="53ee0-363">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="53ee0-363">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="53ee0-364">指示帐户和设备正在使用移动威胁防护合作伙伴时设备的威胁状态。</span><span class="sxs-lookup"><span data-stu-id="53ee0-364">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="53ee0-365">只读。</span><span class="sxs-lookup"><span data-stu-id="53ee0-365">Read Only.</span></span> <span data-ttu-id="53ee0-366">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="53ee0-366">This property is read-only.</span></span> <span data-ttu-id="53ee0-367">可取值为：`unknown`、`activated`、`deactivated`、`secured`、`lowSeverity`、`mediumSeverity`、`highSeverity`、`unresponsive`、`compromised`、`misconfigured`。</span><span class="sxs-lookup"><span data-stu-id="53ee0-367">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="53ee0-368">retireAfterDateTime</span><span class="sxs-lookup"><span data-stu-id="53ee0-368">retireAfterDateTime</span></span>|<span data-ttu-id="53ee0-369">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53ee0-369">DateTimeOffset</span></span>|<span data-ttu-id="53ee0-370">指示当设备因计划操作而自动停用的时间。</span><span class="sxs-lookup"><span data-stu-id="53ee0-370">Indicates the time after when a device will be auto retired because of scheduled action.</span></span> <span data-ttu-id="53ee0-371">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="53ee0-371">This property is read-only.</span></span>|
|<span data-ttu-id="53ee0-372">usersLoggedOn</span><span class="sxs-lookup"><span data-stu-id="53ee0-372">usersLoggedOn</span></span>|<span data-ttu-id="53ee0-373">[loggedOnUser](../resources/intune-devices-loggedonuser.md)集合</span><span class="sxs-lookup"><span data-stu-id="53ee0-373">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="53ee0-374">指示设备的上次登录用户。</span><span class="sxs-lookup"><span data-stu-id="53ee0-374">Indicates the last logged on users of a device.</span></span> <span data-ttu-id="53ee0-375">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="53ee0-375">This property is read-only.</span></span>|
|<span data-ttu-id="53ee0-376">preferMdmOverGroupPolicyAppliedDateTime</span><span class="sxs-lookup"><span data-stu-id="53ee0-376">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="53ee0-377">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53ee0-377">DateTimeOffset</span></span>|<span data-ttu-id="53ee0-378">报告设置了 preferMdmOverGroupPolicy 设置的 DateTime。</span><span class="sxs-lookup"><span data-stu-id="53ee0-378">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="53ee0-379">设置后，如果存在冲突，Intune MDM 设置将覆盖组策略设置。</span><span class="sxs-lookup"><span data-stu-id="53ee0-379">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="53ee0-380">只读。</span><span class="sxs-lookup"><span data-stu-id="53ee0-380">Read Only.</span></span> <span data-ttu-id="53ee0-381">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="53ee0-381">This property is read-only.</span></span>|
|<span data-ttu-id="53ee0-382">autopilotEnrolled</span><span class="sxs-lookup"><span data-stu-id="53ee0-382">autopilotEnrolled</span></span>|<span data-ttu-id="53ee0-383">Boolean</span><span class="sxs-lookup"><span data-stu-id="53ee0-383">Boolean</span></span>|<span data-ttu-id="53ee0-384">如果托管设备是通过自动引导注册的，则报告。</span><span class="sxs-lookup"><span data-stu-id="53ee0-384">Reports if the managed device is enrolled via auto-pilot.</span></span> <span data-ttu-id="53ee0-385">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="53ee0-385">This property is read-only.</span></span>|
|<span data-ttu-id="53ee0-386">requireUserEnrollmentApproval</span><span class="sxs-lookup"><span data-stu-id="53ee0-386">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="53ee0-387">Boolean</span><span class="sxs-lookup"><span data-stu-id="53ee0-387">Boolean</span></span>|<span data-ttu-id="53ee0-388">如果托管 iOS 设备是用户审批注册，则报告。</span><span class="sxs-lookup"><span data-stu-id="53ee0-388">Reports if the managed iOS device is user approval enrollment.</span></span> <span data-ttu-id="53ee0-389">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="53ee0-389">This property is read-only.</span></span>|
|<span data-ttu-id="53ee0-390">managementCertificateExpirationDate</span><span class="sxs-lookup"><span data-stu-id="53ee0-390">managementCertificateExpirationDate</span></span>|<span data-ttu-id="53ee0-391">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53ee0-391">DateTimeOffset</span></span>|<span data-ttu-id="53ee0-392">报告设备管理证书到期日期。</span><span class="sxs-lookup"><span data-stu-id="53ee0-392">Reports device management certificate expiration date.</span></span> <span data-ttu-id="53ee0-393">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="53ee0-393">This property is read-only.</span></span>|
|<span data-ttu-id="53ee0-394">iccid</span><span class="sxs-lookup"><span data-stu-id="53ee0-394">iccid</span></span>|<span data-ttu-id="53ee0-395">字符串</span><span class="sxs-lookup"><span data-stu-id="53ee0-395">String</span></span>|<span data-ttu-id="53ee0-396">集成的电路卡标识符，它是 SIM 卡的唯一标识号。</span><span class="sxs-lookup"><span data-stu-id="53ee0-396">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span> <span data-ttu-id="53ee0-397">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="53ee0-397">This property is read-only.</span></span>|
|<span data-ttu-id="53ee0-398">udid</span><span class="sxs-lookup"><span data-stu-id="53ee0-398">udid</span></span>|<span data-ttu-id="53ee0-399">字符串</span><span class="sxs-lookup"><span data-stu-id="53ee0-399">String</span></span>|<span data-ttu-id="53ee0-400">IOS 和 macOS 设备的唯一设备标识符。</span><span class="sxs-lookup"><span data-stu-id="53ee0-400">Unique Device Identifier for iOS and macOS devices.</span></span> <span data-ttu-id="53ee0-401">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="53ee0-401">This property is read-only.</span></span>|
|<span data-ttu-id="53ee0-402">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="53ee0-402">roleScopeTagIds</span></span>|<span data-ttu-id="53ee0-403">String 集合</span><span class="sxs-lookup"><span data-stu-id="53ee0-403">String collection</span></span>|<span data-ttu-id="53ee0-404">此设备实例的范围标记 Id 的列表。</span><span class="sxs-lookup"><span data-stu-id="53ee0-404">List of Scope Tag IDs for this Device instance.</span></span>|
|<span data-ttu-id="53ee0-405">windowsActiveMalwareCount</span><span class="sxs-lookup"><span data-stu-id="53ee0-405">windowsActiveMalwareCount</span></span>|<span data-ttu-id="53ee0-406">Int32</span><span class="sxs-lookup"><span data-stu-id="53ee0-406">Int32</span></span>|<span data-ttu-id="53ee0-407">此 windows 设备的活动恶意软件的计数。</span><span class="sxs-lookup"><span data-stu-id="53ee0-407">Count of active malware for this windows device.</span></span> <span data-ttu-id="53ee0-408">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="53ee0-408">This property is read-only.</span></span>|
|<span data-ttu-id="53ee0-409">windowsRemediatedMalwareCount</span><span class="sxs-lookup"><span data-stu-id="53ee0-409">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="53ee0-410">Int32</span><span class="sxs-lookup"><span data-stu-id="53ee0-410">Int32</span></span>|<span data-ttu-id="53ee0-411">此 windows 设备的修正的恶意软件的计数。</span><span class="sxs-lookup"><span data-stu-id="53ee0-411">Count of remediated malware for this windows device.</span></span> <span data-ttu-id="53ee0-412">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="53ee0-412">This property is read-only.</span></span>|
|<span data-ttu-id="53ee0-413">notes</span><span class="sxs-lookup"><span data-stu-id="53ee0-413">notes</span></span>|<span data-ttu-id="53ee0-414">字符串</span><span class="sxs-lookup"><span data-stu-id="53ee0-414">String</span></span>|<span data-ttu-id="53ee0-415">IT 管理员创建的设备上的注释</span><span class="sxs-lookup"><span data-stu-id="53ee0-415">Notes on the device created by IT Admin</span></span>|
|<span data-ttu-id="53ee0-416">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="53ee0-416">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="53ee0-417">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="53ee0-417">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="53ee0-418">Configuration manager 客户端运行状况状态，仅对由 MDM/ConfigMgr 代理管理的设备有效</span><span class="sxs-lookup"><span data-stu-id="53ee0-418">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent</span></span>|
|<span data-ttu-id="53ee0-419">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="53ee0-419">configurationManagerClientInformation</span></span>|[<span data-ttu-id="53ee0-420">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="53ee0-420">configurationManagerClientInformation</span></span>](../resources/intune-devices-configurationmanagerclientinformation.md)|<span data-ttu-id="53ee0-421">Configuration manager 客户端信息，仅对受 ConfigMgr 代理管理、duel 管理或三方管理的设备有效</span><span class="sxs-lookup"><span data-stu-id="53ee0-421">Configuration manager client information, valid only for devices managed, duel-managed or tri-managed by ConfigMgr Agent</span></span>|



## <a name="response"></a><span data-ttu-id="53ee0-422">响应</span><span class="sxs-lookup"><span data-stu-id="53ee0-422">Response</span></span>
<span data-ttu-id="53ee0-423">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [managedDevice](../resources/intune-devices-manageddevice.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="53ee0-423">If successful, this method returns a `200 OK` response code and an updated [managedDevice](../resources/intune-devices-manageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53ee0-424">示例</span><span class="sxs-lookup"><span data-stu-id="53ee0-424">Example</span></span>

### <a name="request"></a><span data-ttu-id="53ee0-425">请求</span><span class="sxs-lookup"><span data-stu-id="53ee0-425">Request</span></span>
<span data-ttu-id="53ee0-426">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="53ee0-426">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}
Content-type: application/json
Content-length: 7513

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
    "clientIdentifier": "Client Identifier value"
  }
}
```

### <a name="response"></a><span data-ttu-id="53ee0-427">响应</span><span class="sxs-lookup"><span data-stu-id="53ee0-427">Response</span></span>
<span data-ttu-id="53ee0-p167">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="53ee0-p167">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 7562

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
    "clientIdentifier": "Client Identifier value"
  }
}
```






