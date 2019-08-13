---
title: 创建 windowsManagedDevice
description: 创建新的 windowsManagedDevice 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7cad94fca4ee7e3876329c43aab7f81d63aef801
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36309910"
---
# <a name="create-windowsmanageddevice"></a><span data-ttu-id="bdf99-103">创建 windowsManagedDevice</span><span class="sxs-lookup"><span data-stu-id="bdf99-103">Create windowsManagedDevice</span></span>

> <span data-ttu-id="bdf99-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bdf99-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bdf99-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bdf99-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bdf99-106">创建新的[windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md)对象。</span><span class="sxs-lookup"><span data-stu-id="bdf99-106">Create a new [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bdf99-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="bdf99-107">Prerequisites</span></span>
<span data-ttu-id="bdf99-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bdf99-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bdf99-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="bdf99-110">Permission type</span></span>|<span data-ttu-id="bdf99-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="bdf99-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bdf99-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bdf99-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bdf99-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bdf99-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="bdf99-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bdf99-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bdf99-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="bdf99-115">Not supported.</span></span>|
|<span data-ttu-id="bdf99-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="bdf99-116">Application</span></span>|<span data-ttu-id="bdf99-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bdf99-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bdf99-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bdf99-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices
```

## <a name="request-headers"></a><span data-ttu-id="bdf99-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="bdf99-119">Request headers</span></span>
|<span data-ttu-id="bdf99-120">标头</span><span class="sxs-lookup"><span data-stu-id="bdf99-120">Header</span></span>|<span data-ttu-id="bdf99-121">值</span><span class="sxs-lookup"><span data-stu-id="bdf99-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bdf99-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bdf99-122">Authorization</span></span>|<span data-ttu-id="bdf99-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="bdf99-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bdf99-124">接受</span><span class="sxs-lookup"><span data-stu-id="bdf99-124">Accept</span></span>|<span data-ttu-id="bdf99-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bdf99-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bdf99-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="bdf99-126">Request body</span></span>
<span data-ttu-id="bdf99-127">在请求正文中, 提供 windowsManagedDevice 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bdf99-127">In the request body, supply a JSON representation for the windowsManagedDevice object.</span></span>

<span data-ttu-id="bdf99-128">下表显示创建 windowsManagedDevice 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="bdf99-128">The following table shows the properties that are required when you create the windowsManagedDevice.</span></span>

|<span data-ttu-id="bdf99-129">属性</span><span class="sxs-lookup"><span data-stu-id="bdf99-129">Property</span></span>|<span data-ttu-id="bdf99-130">类型</span><span class="sxs-lookup"><span data-stu-id="bdf99-130">Type</span></span>|<span data-ttu-id="bdf99-131">说明</span><span class="sxs-lookup"><span data-stu-id="bdf99-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bdf99-132">id</span><span class="sxs-lookup"><span data-stu-id="bdf99-132">id</span></span>|<span data-ttu-id="bdf99-133">字符串</span><span class="sxs-lookup"><span data-stu-id="bdf99-133">String</span></span>|<span data-ttu-id="bdf99-134">继承自[managedDevice](../resources/intune-devices-manageddevice.md)的设备的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="bdf99-134">Unique Identifier for the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="bdf99-135">userId</span><span class="sxs-lookup"><span data-stu-id="bdf99-135">userId</span></span>|<span data-ttu-id="bdf99-136">String</span><span class="sxs-lookup"><span data-stu-id="bdf99-136">String</span></span>|<span data-ttu-id="bdf99-137">与继承自[managedDevice](../resources/intune-devices-manageddevice.md)的设备关联的用户的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="bdf99-137">Unique Identifier for the user associated with the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="bdf99-138">deviceName</span><span class="sxs-lookup"><span data-stu-id="bdf99-138">deviceName</span></span>|<span data-ttu-id="bdf99-139">String</span><span class="sxs-lookup"><span data-stu-id="bdf99-139">String</span></span>|<span data-ttu-id="bdf99-140">继承自[managedDevice](../resources/intune-devices-manageddevice.md)的设备的名称</span><span class="sxs-lookup"><span data-stu-id="bdf99-140">Name of the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="bdf99-141">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="bdf99-141">hardwareInformation</span></span>|[<span data-ttu-id="bdf99-142">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="bdf99-142">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="bdf99-143">设备的 hardward 详细信息。</span><span class="sxs-lookup"><span data-stu-id="bdf99-143">The hardward details for the device.</span></span>  <span data-ttu-id="bdf99-144">包括存储空间、制造商、序列号等信息。继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="bdf99-144">Includes information such as storage space, manufacturer, serial number, etc. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="bdf99-145">所有者</span><span class="sxs-lookup"><span data-stu-id="bdf99-145">ownerType</span></span>|[<span data-ttu-id="bdf99-146">所有者</span><span class="sxs-lookup"><span data-stu-id="bdf99-146">ownerType</span></span>](../resources/intune-devices-ownertype.md)|<span data-ttu-id="bdf99-147">设备的所有权。</span><span class="sxs-lookup"><span data-stu-id="bdf99-147">Ownership of the device.</span></span> <span data-ttu-id="bdf99-148">可以是从[ManagedDevice](../resources/intune-devices-manageddevice.md)继承的 "公司" 或 "个人"。</span><span class="sxs-lookup"><span data-stu-id="bdf99-148">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="bdf99-149">可取值为：`unknown`、`company`、`personal`。</span><span class="sxs-lookup"><span data-stu-id="bdf99-149">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="bdf99-150">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="bdf99-150">managedDeviceOwnerType</span></span>|[<span data-ttu-id="bdf99-151">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="bdf99-151">managedDeviceOwnerType</span></span>](../resources/intune-devices-manageddeviceownertype.md)|<span data-ttu-id="bdf99-152">设备的所有权。</span><span class="sxs-lookup"><span data-stu-id="bdf99-152">Ownership of the device.</span></span> <span data-ttu-id="bdf99-153">可以是从[ManagedDevice](../resources/intune-devices-manageddevice.md)继承的 "公司" 或 "个人"。</span><span class="sxs-lookup"><span data-stu-id="bdf99-153">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="bdf99-154">可取值为：`unknown`、`company`、`personal`。</span><span class="sxs-lookup"><span data-stu-id="bdf99-154">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="bdf99-155">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="bdf99-155">deviceActionResults</span></span>|<span data-ttu-id="bdf99-156">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) 集合</span><span class="sxs-lookup"><span data-stu-id="bdf99-156">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="bdf99-157">ComplexType deviceActionResult 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="bdf99-157">List of ComplexType deviceActionResult objects.</span></span> <span data-ttu-id="bdf99-158">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="bdf99-158">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="bdf99-159">managementState</span><span class="sxs-lookup"><span data-stu-id="bdf99-159">managementState</span></span>|[<span data-ttu-id="bdf99-160">managementState</span><span class="sxs-lookup"><span data-stu-id="bdf99-160">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="bdf99-161">设备的管理状态。</span><span class="sxs-lookup"><span data-stu-id="bdf99-161">Management state of the device.</span></span> <span data-ttu-id="bdf99-162">继承自[managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="bdf99-162">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="bdf99-163">可取值为：`managed`、`retirePending`、`retireFailed`、`wipePending`、`wipeFailed`、`unhealthy`、`deletePending`、`retireIssued`、`wipeIssued`、`wipeCanceled`、`retireCanceled`、`discovered`。</span><span class="sxs-lookup"><span data-stu-id="bdf99-163">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="bdf99-164">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="bdf99-164">enrolledDateTime</span></span>|<span data-ttu-id="bdf99-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bdf99-165">DateTimeOffset</span></span>|<span data-ttu-id="bdf99-166">设备的注册时间。</span><span class="sxs-lookup"><span data-stu-id="bdf99-166">Enrollment time of the device.</span></span> <span data-ttu-id="bdf99-167">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="bdf99-167">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="bdf99-168">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="bdf99-168">lastSyncDateTime</span></span>|<span data-ttu-id="bdf99-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bdf99-169">DateTimeOffset</span></span>|<span data-ttu-id="bdf99-170">设备上次成功完成与 Intune 同步的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="bdf99-170">The date and time that the device last completed a successful sync with Intune.</span></span> <span data-ttu-id="bdf99-171">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="bdf99-171">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="bdf99-172">chassisType</span><span class="sxs-lookup"><span data-stu-id="bdf99-172">chassisType</span></span>|[<span data-ttu-id="bdf99-173">chassisType</span><span class="sxs-lookup"><span data-stu-id="bdf99-173">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="bdf99-174">设备的机箱类型。</span><span class="sxs-lookup"><span data-stu-id="bdf99-174">Chassis type of the device.</span></span> <span data-ttu-id="bdf99-175">继承自[managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="bdf99-175">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="bdf99-176">可取值为：`unknown`、`desktop`、`laptop`、`worksWorkstation`、`enterpriseServer`、`phone`、`tablet`、`mobileOther`、`mobileUnknown`。</span><span class="sxs-lookup"><span data-stu-id="bdf99-176">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="bdf99-177">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="bdf99-177">operatingSystem</span></span>|<span data-ttu-id="bdf99-178">String</span><span class="sxs-lookup"><span data-stu-id="bdf99-178">String</span></span>|<span data-ttu-id="bdf99-179">设备的操作系统。</span><span class="sxs-lookup"><span data-stu-id="bdf99-179">Operating system of the device.</span></span> <span data-ttu-id="bdf99-180">Windows、iOS 等。继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="bdf99-180">Windows, iOS, etc. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="bdf99-181">deviceType</span><span class="sxs-lookup"><span data-stu-id="bdf99-181">deviceType</span></span>|[<span data-ttu-id="bdf99-182">deviceType</span><span class="sxs-lookup"><span data-stu-id="bdf99-182">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="bdf99-183">设备的平台。</span><span class="sxs-lookup"><span data-stu-id="bdf99-183">Platform of the device.</span></span> <span data-ttu-id="bdf99-184">继承自[managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="bdf99-184">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="bdf99-185">可能的值为`desktop`: `windowsRT`、 `winMO6`、 `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer`、、、、、、、、、、、、、、、、 `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="bdf99-185">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="bdf99-186">complianceState</span><span class="sxs-lookup"><span data-stu-id="bdf99-186">complianceState</span></span>|[<span data-ttu-id="bdf99-187">complianceState</span><span class="sxs-lookup"><span data-stu-id="bdf99-187">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="bdf99-188">设备的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="bdf99-188">Compliance state of the device.</span></span> <span data-ttu-id="bdf99-189">继承自[managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="bdf99-189">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="bdf99-190">可取值为：`unknown`、`compliant`、`noncompliant`、`conflict`、`error`、`inGracePeriod`、`configManager`。</span><span class="sxs-lookup"><span data-stu-id="bdf99-190">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="bdf99-191">jailBroken</span><span class="sxs-lookup"><span data-stu-id="bdf99-191">jailBroken</span></span>|<span data-ttu-id="bdf99-192">String</span><span class="sxs-lookup"><span data-stu-id="bdf99-192">String</span></span>|<span data-ttu-id="bdf99-193">设备是否已越狱或取得 root 权限。</span><span class="sxs-lookup"><span data-stu-id="bdf99-193">whether the device is jail broken or rooted.</span></span> <span data-ttu-id="bdf99-194">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="bdf99-194">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="bdf99-195">managementAgent</span><span class="sxs-lookup"><span data-stu-id="bdf99-195">managementAgent</span></span>|[<span data-ttu-id="bdf99-196">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="bdf99-196">managementAgentType</span></span>](../resources/intune-devices-managementagenttype.md)|<span data-ttu-id="bdf99-197">设备的管理通道。</span><span class="sxs-lookup"><span data-stu-id="bdf99-197">Management channel of the device.</span></span> <span data-ttu-id="bdf99-198">Intune、EAS 等。继承自[managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="bdf99-198">Intune, EAS, etc. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="bdf99-199">可取值为：`eas`、`mdm`、`easMdm`、`intuneClient`、`easIntuneClient`、`configurationManagerClient`、`configurationManagerClientMdm`、`configurationManagerClientMdmEas`、`unknown`、`jamf`、`googleCloudDevicePolicyController`、`microsoft365ManagedMdm`。</span><span class="sxs-lookup"><span data-stu-id="bdf99-199">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span></span>|
|<span data-ttu-id="bdf99-200">osVersion</span><span class="sxs-lookup"><span data-stu-id="bdf99-200">osVersion</span></span>|<span data-ttu-id="bdf99-201">String</span><span class="sxs-lookup"><span data-stu-id="bdf99-201">String</span></span>|<span data-ttu-id="bdf99-202">设备的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="bdf99-202">Operating system version of the device.</span></span> <span data-ttu-id="bdf99-203">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="bdf99-203">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="bdf99-204">easActivated</span><span class="sxs-lookup"><span data-stu-id="bdf99-204">easActivated</span></span>|<span data-ttu-id="bdf99-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="bdf99-205">Boolean</span></span>|<span data-ttu-id="bdf99-206">设备是否已激活 Exchange ActiveSync。</span><span class="sxs-lookup"><span data-stu-id="bdf99-206">Whether the device is Exchange ActiveSync activated.</span></span> <span data-ttu-id="bdf99-207">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="bdf99-207">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="bdf99-208">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="bdf99-208">easDeviceId</span></span>|<span data-ttu-id="bdf99-209">String</span><span class="sxs-lookup"><span data-stu-id="bdf99-209">String</span></span>|<span data-ttu-id="bdf99-210">设备的 Exchange ActiveSync ID。</span><span class="sxs-lookup"><span data-stu-id="bdf99-210">Exchange ActiveSync Id of the device.</span></span> <span data-ttu-id="bdf99-211">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="bdf99-211">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="bdf99-212">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="bdf99-212">easActivationDateTime</span></span>|<span data-ttu-id="bdf99-213">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bdf99-213">DateTimeOffset</span></span>|<span data-ttu-id="bdf99-214">设备的 Exchange ActivationSync 激活时间。</span><span class="sxs-lookup"><span data-stu-id="bdf99-214">Exchange ActivationSync activation time of the device.</span></span> <span data-ttu-id="bdf99-215">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="bdf99-215">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="bdf99-216">aadRegistered</span><span class="sxs-lookup"><span data-stu-id="bdf99-216">aadRegistered</span></span>|<span data-ttu-id="bdf99-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="bdf99-217">Boolean</span></span>|<span data-ttu-id="bdf99-218">设备是否已注册 Azure Active Directory。</span><span class="sxs-lookup"><span data-stu-id="bdf99-218">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="bdf99-219">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="bdf99-219">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="bdf99-220">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="bdf99-220">azureADRegistered</span></span>|<span data-ttu-id="bdf99-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="bdf99-221">Boolean</span></span>|<span data-ttu-id="bdf99-222">设备是否已注册 Azure Active Directory。</span><span class="sxs-lookup"><span data-stu-id="bdf99-222">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="bdf99-223">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="bdf99-223">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="bdf99-224">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="bdf99-224">deviceEnrollmentType</span></span>|[<span data-ttu-id="bdf99-225">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="bdf99-225">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="bdf99-226">设备的注册类型。</span><span class="sxs-lookup"><span data-stu-id="bdf99-226">Enrollment type of the device.</span></span> <span data-ttu-id="bdf99-227">继承自[managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="bdf99-227">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="bdf99-228">可取值为：`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement`。</span><span class="sxs-lookup"><span data-stu-id="bdf99-228">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="bdf99-229">lostModeState</span><span class="sxs-lookup"><span data-stu-id="bdf99-229">lostModeState</span></span>|[<span data-ttu-id="bdf99-230">lostModeState</span><span class="sxs-lookup"><span data-stu-id="bdf99-230">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="bdf99-231">指示是否已启用或禁用从[ManagedDevice](../resources/intune-devices-manageddevice.md)继承的已丢失模式。</span><span class="sxs-lookup"><span data-stu-id="bdf99-231">Indicates if Lost mode is enabled or disabled Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="bdf99-232">可取值为：`disabled`、`enabled`。</span><span class="sxs-lookup"><span data-stu-id="bdf99-232">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="bdf99-233">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="bdf99-233">activationLockBypassCode</span></span>|<span data-ttu-id="bdf99-234">String</span><span class="sxs-lookup"><span data-stu-id="bdf99-234">String</span></span>|<span data-ttu-id="bdf99-235">允许绕过设备上的激活锁的代码。</span><span class="sxs-lookup"><span data-stu-id="bdf99-235">Code that allows the Activation Lock on a device to be bypassed.</span></span> <span data-ttu-id="bdf99-236">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="bdf99-236">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="bdf99-237">emailAddress</span><span class="sxs-lookup"><span data-stu-id="bdf99-237">emailAddress</span></span>|<span data-ttu-id="bdf99-238">String</span><span class="sxs-lookup"><span data-stu-id="bdf99-238">String</span></span>|<span data-ttu-id="bdf99-239">与从[ManagedDevice](../resources/intune-devices-manageddevice.md)继承的设备关联的用户的电子邮件</span><span class="sxs-lookup"><span data-stu-id="bdf99-239">Email(s) for the user associated with the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="bdf99-240">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="bdf99-240">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="bdf99-241">String</span><span class="sxs-lookup"><span data-stu-id="bdf99-241">String</span></span>|<span data-ttu-id="bdf99-242">Azure Active Directory 设备的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="bdf99-242">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="bdf99-243">只读。</span><span class="sxs-lookup"><span data-stu-id="bdf99-243">Read only.</span></span> <span data-ttu-id="bdf99-244">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="bdf99-244">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="bdf99-245">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="bdf99-245">azureADDeviceId</span></span>|<span data-ttu-id="bdf99-246">String</span><span class="sxs-lookup"><span data-stu-id="bdf99-246">String</span></span>|<span data-ttu-id="bdf99-247">Azure Active Directory 设备的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="bdf99-247">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="bdf99-248">只读。</span><span class="sxs-lookup"><span data-stu-id="bdf99-248">Read only.</span></span> <span data-ttu-id="bdf99-249">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="bdf99-249">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="bdf99-250">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="bdf99-250">deviceRegistrationState</span></span>|[<span data-ttu-id="bdf99-251">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="bdf99-251">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="bdf99-252">设备注册状态。</span><span class="sxs-lookup"><span data-stu-id="bdf99-252">Device registration state.</span></span> <span data-ttu-id="bdf99-253">继承自[managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="bdf99-253">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="bdf99-254">可取值为：`notRegistered`、`registered`、`revoked`、`keyConflict`、`approvalPending`、`certificateReset`、`notRegisteredPendingEnrollment`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="bdf99-254">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="bdf99-255">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="bdf99-255">deviceCategoryDisplayName</span></span>|<span data-ttu-id="bdf99-256">String</span><span class="sxs-lookup"><span data-stu-id="bdf99-256">String</span></span>|<span data-ttu-id="bdf99-257">继承自[managedDevice](../resources/intune-devices-manageddevice.md)的设备类别显示名称</span><span class="sxs-lookup"><span data-stu-id="bdf99-257">Device category display name Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="bdf99-258">isSupervised</span><span class="sxs-lookup"><span data-stu-id="bdf99-258">isSupervised</span></span>|<span data-ttu-id="bdf99-259">Boolean</span><span class="sxs-lookup"><span data-stu-id="bdf99-259">Boolean</span></span>|<span data-ttu-id="bdf99-260">从[ManagedDevice](../resources/intune-devices-manageddevice.md)继承的设备监督状态</span><span class="sxs-lookup"><span data-stu-id="bdf99-260">Device supervised status Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="bdf99-261">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="bdf99-261">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="bdf99-262">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bdf99-262">DateTimeOffset</span></span>|<span data-ttu-id="bdf99-263">设备上次与 Exchange 联系的时间。</span><span class="sxs-lookup"><span data-stu-id="bdf99-263">Last time the device contacted Exchange.</span></span> <span data-ttu-id="bdf99-264">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="bdf99-264">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="bdf99-265">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="bdf99-265">exchangeAccessState</span></span>|[<span data-ttu-id="bdf99-266">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="bdf99-266">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="bdf99-267">Exchange 中设备的访问状态。</span><span class="sxs-lookup"><span data-stu-id="bdf99-267">The Access State of the device in Exchange.</span></span> <span data-ttu-id="bdf99-268">继承自[managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="bdf99-268">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="bdf99-269">可取值为：`none`、`unknown`、`allowed`、`blocked`、`quarantined`。</span><span class="sxs-lookup"><span data-stu-id="bdf99-269">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="bdf99-270">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="bdf99-270">exchangeAccessStateReason</span></span>|[<span data-ttu-id="bdf99-271">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="bdf99-271">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="bdf99-272">Exchange 中设备访问状态的出现原因。</span><span class="sxs-lookup"><span data-stu-id="bdf99-272">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="bdf99-273">继承自[managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="bdf99-273">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="bdf99-274">可取值为：`none`、`unknown`、`exchangeGlobalRule`、`exchangeIndividualRule`、`exchangeDeviceRule`、`exchangeUpgrade`、`exchangeMailboxPolicy`、`other`、`compliant`、`notCompliant`、`notEnrolled`、`unknownLocation`、`mfaRequired`、`azureADBlockDueToAccessPolicy`、`compromisedPassword`、`deviceNotKnownWithManagedApp`。</span><span class="sxs-lookup"><span data-stu-id="bdf99-274">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="bdf99-275">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="bdf99-275">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="bdf99-276">String</span><span class="sxs-lookup"><span data-stu-id="bdf99-276">String</span></span>|<span data-ttu-id="bdf99-277">允许与设备建立远程协助会话的 URL。</span><span class="sxs-lookup"><span data-stu-id="bdf99-277">Url that allows a Remote Assistance session to be established with the device.</span></span> <span data-ttu-id="bdf99-278">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="bdf99-278">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="bdf99-279">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="bdf99-279">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="bdf99-280">String</span><span class="sxs-lookup"><span data-stu-id="bdf99-280">String</span></span>|<span data-ttu-id="bdf99-281">用于在创建远程协助会话对象时识别问题的错误字符串。</span><span class="sxs-lookup"><span data-stu-id="bdf99-281">An error string that identifies issues when creating Remote Assistance session objects.</span></span> <span data-ttu-id="bdf99-282">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="bdf99-282">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="bdf99-283">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="bdf99-283">isEncrypted</span></span>|<span data-ttu-id="bdf99-284">Boolean</span><span class="sxs-lookup"><span data-stu-id="bdf99-284">Boolean</span></span>|<span data-ttu-id="bdf99-285">从[ManagedDevice](../resources/intune-devices-manageddevice.md)继承的设备加密状态</span><span class="sxs-lookup"><span data-stu-id="bdf99-285">Device encryption status Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="bdf99-286">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="bdf99-286">userPrincipalName</span></span>|<span data-ttu-id="bdf99-287">String</span><span class="sxs-lookup"><span data-stu-id="bdf99-287">String</span></span>|<span data-ttu-id="bdf99-288">从[ManagedDevice](../resources/intune-devices-manageddevice.md)继承的设备用户主体名称</span><span class="sxs-lookup"><span data-stu-id="bdf99-288">Device user principal name Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="bdf99-289">model</span><span class="sxs-lookup"><span data-stu-id="bdf99-289">model</span></span>|<span data-ttu-id="bdf99-290">String</span><span class="sxs-lookup"><span data-stu-id="bdf99-290">String</span></span>|<span data-ttu-id="bdf99-291">继承自[managedDevice](../resources/intune-devices-manageddevice.md)的设备的模型</span><span class="sxs-lookup"><span data-stu-id="bdf99-291">Model of the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="bdf99-292">manufacturer</span><span class="sxs-lookup"><span data-stu-id="bdf99-292">manufacturer</span></span>|<span data-ttu-id="bdf99-293">String</span><span class="sxs-lookup"><span data-stu-id="bdf99-293">String</span></span>|<span data-ttu-id="bdf99-294">继承自[managedDevice](../resources/intune-devices-manageddevice.md)的设备的制造商</span><span class="sxs-lookup"><span data-stu-id="bdf99-294">Manufacturer of the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="bdf99-295">imei</span><span class="sxs-lookup"><span data-stu-id="bdf99-295">imei</span></span>|<span data-ttu-id="bdf99-296">String</span><span class="sxs-lookup"><span data-stu-id="bdf99-296">String</span></span>|<span data-ttu-id="bdf99-297">从[ManagedDevice](../resources/intune-devices-manageddevice.md)继承的 IMEI</span><span class="sxs-lookup"><span data-stu-id="bdf99-297">IMEI Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="bdf99-298">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="bdf99-298">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="bdf99-299">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bdf99-299">DateTimeOffset</span></span>|<span data-ttu-id="bdf99-300">设备符合性宽限期过期时间从[ManagedDevice](../resources/intune-devices-manageddevice.md)继承的日期/时间</span><span class="sxs-lookup"><span data-stu-id="bdf99-300">The DateTime when device compliance grace period expires Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="bdf99-301">serialNumber</span><span class="sxs-lookup"><span data-stu-id="bdf99-301">serialNumber</span></span>|<span data-ttu-id="bdf99-302">字符串</span><span class="sxs-lookup"><span data-stu-id="bdf99-302">String</span></span>|<span data-ttu-id="bdf99-303">SerialNumber 继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="bdf99-303">SerialNumber Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="bdf99-304">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="bdf99-304">phoneNumber</span></span>|<span data-ttu-id="bdf99-305">String</span><span class="sxs-lookup"><span data-stu-id="bdf99-305">String</span></span>|<span data-ttu-id="bdf99-306">继承自[managedDevice](../resources/intune-devices-manageddevice.md)的设备的电话号码</span><span class="sxs-lookup"><span data-stu-id="bdf99-306">Phone number of the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="bdf99-307">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="bdf99-307">androidSecurityPatchLevel</span></span>|<span data-ttu-id="bdf99-308">String</span><span class="sxs-lookup"><span data-stu-id="bdf99-308">String</span></span>|<span data-ttu-id="bdf99-309">从[ManagedDevice](../resources/intune-devices-manageddevice.md)继承的 Android 安全修补程序级别</span><span class="sxs-lookup"><span data-stu-id="bdf99-309">Android security patch level Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="bdf99-310">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="bdf99-310">userDisplayName</span></span>|<span data-ttu-id="bdf99-311">String</span><span class="sxs-lookup"><span data-stu-id="bdf99-311">String</span></span>|<span data-ttu-id="bdf99-312">从[ManagedDevice](../resources/intune-devices-manageddevice.md)继承的用户显示名称</span><span class="sxs-lookup"><span data-stu-id="bdf99-312">User display name Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="bdf99-313">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="bdf99-313">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="bdf99-314">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="bdf99-314">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="bdf99-315">继承自[managedDevice](../resources/intune-devices-manageddevice.md)的 ConfigrMgr 客户端启用的功能</span><span class="sxs-lookup"><span data-stu-id="bdf99-315">ConfigrMgr client enabled features Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="bdf99-316">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="bdf99-316">wiFiMacAddress</span></span>|<span data-ttu-id="bdf99-317">String</span><span class="sxs-lookup"><span data-stu-id="bdf99-317">String</span></span>|<span data-ttu-id="bdf99-318">从[ManagedDevice](../resources/intune-devices-manageddevice.md)继承的 wi-fi MAC</span><span class="sxs-lookup"><span data-stu-id="bdf99-318">Wi-Fi MAC Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="bdf99-319">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="bdf99-319">deviceHealthAttestationState</span></span>|[<span data-ttu-id="bdf99-320">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="bdf99-320">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="bdf99-321">设备运行状况证明状态。</span><span class="sxs-lookup"><span data-stu-id="bdf99-321">The device health attestation state.</span></span> <span data-ttu-id="bdf99-322">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="bdf99-322">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="bdf99-323">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="bdf99-323">subscriberCarrier</span></span>|<span data-ttu-id="bdf99-324">String</span><span class="sxs-lookup"><span data-stu-id="bdf99-324">String</span></span>|<span data-ttu-id="bdf99-325">从[ManagedDevice](../resources/intune-devices-manageddevice.md)继承的订阅者运营商</span><span class="sxs-lookup"><span data-stu-id="bdf99-325">Subscriber Carrier Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="bdf99-326">meid</span><span class="sxs-lookup"><span data-stu-id="bdf99-326">meid</span></span>|<span data-ttu-id="bdf99-327">String</span><span class="sxs-lookup"><span data-stu-id="bdf99-327">String</span></span>|<span data-ttu-id="bdf99-328">MEID 继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="bdf99-328">MEID Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="bdf99-329">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="bdf99-329">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="bdf99-330">Int64</span><span class="sxs-lookup"><span data-stu-id="bdf99-330">Int64</span></span>|<span data-ttu-id="bdf99-331">从[ManagedDevice](../resources/intune-devices-manageddevice.md)继承的总存储量 (以字节为单位)</span><span class="sxs-lookup"><span data-stu-id="bdf99-331">Total Storage in Bytes Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="bdf99-332">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="bdf99-332">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="bdf99-333">Int64</span><span class="sxs-lookup"><span data-stu-id="bdf99-333">Int64</span></span>|<span data-ttu-id="bdf99-334">从[ManagedDevice](../resources/intune-devices-manageddevice.md)继承的可用存储量 (以字节为单位)</span><span class="sxs-lookup"><span data-stu-id="bdf99-334">Free Storage in Bytes Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="bdf99-335">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="bdf99-335">managedDeviceName</span></span>|<span data-ttu-id="bdf99-336">String</span><span class="sxs-lookup"><span data-stu-id="bdf99-336">String</span></span>|<span data-ttu-id="bdf99-337">用于识别设备的自动生成的名称。</span><span class="sxs-lookup"><span data-stu-id="bdf99-337">Automatically generated name to identify a device.</span></span> <span data-ttu-id="bdf99-338">可以覆盖为用户友好名称。</span><span class="sxs-lookup"><span data-stu-id="bdf99-338">Can be overwritten to a user friendly name.</span></span> <span data-ttu-id="bdf99-339">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="bdf99-339">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="bdf99-340">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="bdf99-340">partnerReportedThreatState</span></span>|[<span data-ttu-id="bdf99-341">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="bdf99-341">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="bdf99-342">指示帐户和设备正在使用移动威胁防护合作伙伴时设备的威胁状态。</span><span class="sxs-lookup"><span data-stu-id="bdf99-342">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="bdf99-343">只读。</span><span class="sxs-lookup"><span data-stu-id="bdf99-343">Read Only.</span></span> <span data-ttu-id="bdf99-344">继承自[managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="bdf99-344">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="bdf99-345">可取值为：`unknown`、`activated`、`deactivated`、`secured`、`lowSeverity`、`mediumSeverity`、`highSeverity`、`unresponsive`、`compromised`、`misconfigured`。</span><span class="sxs-lookup"><span data-stu-id="bdf99-345">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="bdf99-346">retireAfterDateTime</span><span class="sxs-lookup"><span data-stu-id="bdf99-346">retireAfterDateTime</span></span>|<span data-ttu-id="bdf99-347">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bdf99-347">DateTimeOffset</span></span>|<span data-ttu-id="bdf99-348">指示当设备因计划操作而自动停用的时间。</span><span class="sxs-lookup"><span data-stu-id="bdf99-348">Indicates the time after when a device will be auto retired because of scheduled action.</span></span> <span data-ttu-id="bdf99-349">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="bdf99-349">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="bdf99-350">usersLoggedOn</span><span class="sxs-lookup"><span data-stu-id="bdf99-350">usersLoggedOn</span></span>|<span data-ttu-id="bdf99-351">[loggedOnUser](../resources/intune-devices-loggedonuser.md)集合</span><span class="sxs-lookup"><span data-stu-id="bdf99-351">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="bdf99-352">指示从[ManagedDevice](../resources/intune-devices-manageddevice.md)继承的设备的上次登录用户</span><span class="sxs-lookup"><span data-stu-id="bdf99-352">Indicates the last logged on users of a device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="bdf99-353">preferMdmOverGroupPolicyAppliedDateTime</span><span class="sxs-lookup"><span data-stu-id="bdf99-353">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="bdf99-354">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bdf99-354">DateTimeOffset</span></span>|<span data-ttu-id="bdf99-355">报告设置了 preferMdmOverGroupPolicy 设置的 DateTime。</span><span class="sxs-lookup"><span data-stu-id="bdf99-355">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="bdf99-356">设置后, 如果存在冲突, Intune MDM 设置将覆盖组策略设置。</span><span class="sxs-lookup"><span data-stu-id="bdf99-356">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="bdf99-357">只读。</span><span class="sxs-lookup"><span data-stu-id="bdf99-357">Read Only.</span></span> <span data-ttu-id="bdf99-358">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="bdf99-358">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="bdf99-359">autopilotEnrolled</span><span class="sxs-lookup"><span data-stu-id="bdf99-359">autopilotEnrolled</span></span>|<span data-ttu-id="bdf99-360">Boolean</span><span class="sxs-lookup"><span data-stu-id="bdf99-360">Boolean</span></span>|<span data-ttu-id="bdf99-361">如果托管设备是通过自动引导注册的, 则报告。</span><span class="sxs-lookup"><span data-stu-id="bdf99-361">Reports if the managed device is enrolled via auto-pilot.</span></span> <span data-ttu-id="bdf99-362">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="bdf99-362">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="bdf99-363">requireUserEnrollmentApproval</span><span class="sxs-lookup"><span data-stu-id="bdf99-363">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="bdf99-364">Boolean</span><span class="sxs-lookup"><span data-stu-id="bdf99-364">Boolean</span></span>|<span data-ttu-id="bdf99-365">如果托管 iOS 设备是用户审批注册, 则报告。</span><span class="sxs-lookup"><span data-stu-id="bdf99-365">Reports if the managed iOS device is user approval enrollment.</span></span> <span data-ttu-id="bdf99-366">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="bdf99-366">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="bdf99-367">managementCertificateExpirationDate</span><span class="sxs-lookup"><span data-stu-id="bdf99-367">managementCertificateExpirationDate</span></span>|<span data-ttu-id="bdf99-368">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bdf99-368">DateTimeOffset</span></span>|<span data-ttu-id="bdf99-369">报告设备管理证书到期日期继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="bdf99-369">Reports device management certificate expiration date Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="bdf99-370">iccid</span><span class="sxs-lookup"><span data-stu-id="bdf99-370">iccid</span></span>|<span data-ttu-id="bdf99-371">String</span><span class="sxs-lookup"><span data-stu-id="bdf99-371">String</span></span>|<span data-ttu-id="bdf99-372">集成的电路卡标识符, 它是 SIM 卡的唯一标识号。</span><span class="sxs-lookup"><span data-stu-id="bdf99-372">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span> <span data-ttu-id="bdf99-373">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="bdf99-373">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="bdf99-374">udid</span><span class="sxs-lookup"><span data-stu-id="bdf99-374">udid</span></span>|<span data-ttu-id="bdf99-375">String</span><span class="sxs-lookup"><span data-stu-id="bdf99-375">String</span></span>|<span data-ttu-id="bdf99-376">IOS 和 macOS 设备的唯一设备标识符。</span><span class="sxs-lookup"><span data-stu-id="bdf99-376">Unique Device Identifier for iOS and macOS devices.</span></span> <span data-ttu-id="bdf99-377">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="bdf99-377">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="bdf99-378">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="bdf99-378">roleScopeTagIds</span></span>|<span data-ttu-id="bdf99-379">String collection</span><span class="sxs-lookup"><span data-stu-id="bdf99-379">String collection</span></span>|<span data-ttu-id="bdf99-380">此设备实例的范围标记 Id 的列表。</span><span class="sxs-lookup"><span data-stu-id="bdf99-380">List of Scope Tag IDs for this Device instance.</span></span> <span data-ttu-id="bdf99-381">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="bdf99-381">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="bdf99-382">windowsActiveMalwareCount</span><span class="sxs-lookup"><span data-stu-id="bdf99-382">windowsActiveMalwareCount</span></span>|<span data-ttu-id="bdf99-383">Int32</span><span class="sxs-lookup"><span data-stu-id="bdf99-383">Int32</span></span>|<span data-ttu-id="bdf99-384">从[ManagedDevice](../resources/intune-devices-manageddevice.md)继承的此 windows 设备的活动恶意软件的计数</span><span class="sxs-lookup"><span data-stu-id="bdf99-384">Count of active malware for this windows device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="bdf99-385">windowsRemediatedMalwareCount</span><span class="sxs-lookup"><span data-stu-id="bdf99-385">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="bdf99-386">Int32</span><span class="sxs-lookup"><span data-stu-id="bdf99-386">Int32</span></span>|<span data-ttu-id="bdf99-387">从[ManagedDevice](../resources/intune-devices-manageddevice.md)继承的此 windows 设备的修正的恶意软件的计数</span><span class="sxs-lookup"><span data-stu-id="bdf99-387">Count of remediated malware for this windows device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="bdf99-388">notes</span><span class="sxs-lookup"><span data-stu-id="bdf99-388">notes</span></span>|<span data-ttu-id="bdf99-389">String</span><span class="sxs-lookup"><span data-stu-id="bdf99-389">String</span></span>|<span data-ttu-id="bdf99-390">由 IT 管理员创建的设备上的注释继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="bdf99-390">Notes on the device created by IT Admin Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="bdf99-391">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="bdf99-391">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="bdf99-392">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="bdf99-392">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="bdf99-393">Configuration manager 客户端运行状况状态, 仅适用于从[ManagedDevice](../resources/intune-devices-manageddevice.md)继承的 MDM/ConfigMgr 代理所管理的设备</span><span class="sxs-lookup"><span data-stu-id="bdf99-393">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="bdf99-394">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="bdf99-394">configurationManagerClientInformation</span></span>|[<span data-ttu-id="bdf99-395">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="bdf99-395">configurationManagerClientInformation</span></span>](../resources/intune-devices-configurationmanagerclientinformation.md)|<span data-ttu-id="bdf99-396">Configuration manager 客户端信息, 仅对由[ManagedDevice](../resources/intune-devices-manageddevice.md)继承的 ConfigMgr 代理、duel 管理或三方管理的设备有效</span><span class="sxs-lookup"><span data-stu-id="bdf99-396">Configuration manager client information, valid only for devices managed, duel-managed or tri-managed by ConfigMgr Agent Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|



## <a name="response"></a><span data-ttu-id="bdf99-397">响应</span><span class="sxs-lookup"><span data-stu-id="bdf99-397">Response</span></span>
<span data-ttu-id="bdf99-398">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md)对象。</span><span class="sxs-lookup"><span data-stu-id="bdf99-398">If successful, this method returns a `201 Created` response code and a [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bdf99-399">示例</span><span class="sxs-lookup"><span data-stu-id="bdf99-399">Example</span></span>

### <a name="request"></a><span data-ttu-id="bdf99-400">请求</span><span class="sxs-lookup"><span data-stu-id="bdf99-400">Request</span></span>
<span data-ttu-id="bdf99-401">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bdf99-401">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices
Content-type: application/json
Content-length: 7520

{
  "@odata.type": "#microsoft.graph.windowsManagedDevice",
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

### <a name="response"></a><span data-ttu-id="bdf99-402">响应</span><span class="sxs-lookup"><span data-stu-id="bdf99-402">Response</span></span>
<span data-ttu-id="bdf99-p142">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bdf99-p142">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 7569

{
  "@odata.type": "#microsoft.graph.windowsManagedDevice",
  "id": "97842b67-2b67-9784-672b-8497672b8497",
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






