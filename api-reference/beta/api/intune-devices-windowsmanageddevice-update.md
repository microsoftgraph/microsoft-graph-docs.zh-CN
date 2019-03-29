---
title: 更新 windowsManagedDevice
description: 更新 windowsManagedDevice 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e1fd03350e06b467713ee1338e62f58cab45b44a
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30962552"
---
# <a name="update-windowsmanageddevice"></a><span data-ttu-id="d81bd-103">更新 windowsManagedDevice</span><span class="sxs-lookup"><span data-stu-id="d81bd-103">Update windowsManagedDevice</span></span>

> <span data-ttu-id="d81bd-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d81bd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d81bd-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d81bd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d81bd-106">更新[windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d81bd-106">Update the properties of a [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d81bd-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="d81bd-107">Prerequisites</span></span>
<span data-ttu-id="d81bd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d81bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d81bd-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d81bd-110">Permission type</span></span>|<span data-ttu-id="d81bd-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d81bd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d81bd-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d81bd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d81bd-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d81bd-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="d81bd-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d81bd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d81bd-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d81bd-115">Not supported.</span></span>|
|<span data-ttu-id="d81bd-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d81bd-116">Application</span></span>|<span data-ttu-id="d81bd-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="d81bd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d81bd-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d81bd-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="d81bd-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="d81bd-119">Request headers</span></span>
|<span data-ttu-id="d81bd-120">标头</span><span class="sxs-lookup"><span data-stu-id="d81bd-120">Header</span></span>|<span data-ttu-id="d81bd-121">值</span><span class="sxs-lookup"><span data-stu-id="d81bd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d81bd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d81bd-122">Authorization</span></span>|<span data-ttu-id="d81bd-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d81bd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d81bd-124">接受</span><span class="sxs-lookup"><span data-stu-id="d81bd-124">Accept</span></span>|<span data-ttu-id="d81bd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d81bd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d81bd-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d81bd-126">Request body</span></span>
<span data-ttu-id="d81bd-127">在请求正文中, 提供[windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d81bd-127">In the request body, supply a JSON representation for the [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object.</span></span>

<span data-ttu-id="d81bd-128">下表显示创建[windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d81bd-128">The following table shows the properties that are required when you create the [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md).</span></span>

|<span data-ttu-id="d81bd-129">属性</span><span class="sxs-lookup"><span data-stu-id="d81bd-129">Property</span></span>|<span data-ttu-id="d81bd-130">类型</span><span class="sxs-lookup"><span data-stu-id="d81bd-130">Type</span></span>|<span data-ttu-id="d81bd-131">说明</span><span class="sxs-lookup"><span data-stu-id="d81bd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d81bd-132">id</span><span class="sxs-lookup"><span data-stu-id="d81bd-132">id</span></span>|<span data-ttu-id="d81bd-133">String</span><span class="sxs-lookup"><span data-stu-id="d81bd-133">String</span></span>|<span data-ttu-id="d81bd-134">继承自[managedDevice](../resources/intune-devices-manageddevice.md)的设备的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="d81bd-134">Unique Identifier for the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d81bd-135">userId</span><span class="sxs-lookup"><span data-stu-id="d81bd-135">userId</span></span>|<span data-ttu-id="d81bd-136">String</span><span class="sxs-lookup"><span data-stu-id="d81bd-136">String</span></span>|<span data-ttu-id="d81bd-137">与继承自[managedDevice](../resources/intune-devices-manageddevice.md)的设备关联的用户的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="d81bd-137">Unique Identifier for the user associated with the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d81bd-138">deviceName</span><span class="sxs-lookup"><span data-stu-id="d81bd-138">deviceName</span></span>|<span data-ttu-id="d81bd-139">String</span><span class="sxs-lookup"><span data-stu-id="d81bd-139">String</span></span>|<span data-ttu-id="d81bd-140">继承自[managedDevice](../resources/intune-devices-manageddevice.md)的设备的名称</span><span class="sxs-lookup"><span data-stu-id="d81bd-140">Name of the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d81bd-141">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="d81bd-141">hardwareInformation</span></span>|[<span data-ttu-id="d81bd-142">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="d81bd-142">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="d81bd-143">设备的 hardward 详细信息。</span><span class="sxs-lookup"><span data-stu-id="d81bd-143">The hardward details for the device.</span></span>  <span data-ttu-id="d81bd-144">包括存储空间、制造商、序列号等信息。继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d81bd-144">Includes information such as storage space, manufacturer, serial number, etc. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d81bd-145">所有者</span><span class="sxs-lookup"><span data-stu-id="d81bd-145">ownerType</span></span>|[<span data-ttu-id="d81bd-146">所有者</span><span class="sxs-lookup"><span data-stu-id="d81bd-146">ownerType</span></span>](../resources/intune-devices-ownertype.md)|<span data-ttu-id="d81bd-147">设备的所有权。</span><span class="sxs-lookup"><span data-stu-id="d81bd-147">Ownership of the device.</span></span> <span data-ttu-id="d81bd-148">可以是从[managedDevice](../resources/intune-devices-manageddevice.md)继承的 "公司" 或 "个人"。</span><span class="sxs-lookup"><span data-stu-id="d81bd-148">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="d81bd-149">可取值为：`unknown`、`company`、`personal`。</span><span class="sxs-lookup"><span data-stu-id="d81bd-149">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="d81bd-150">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="d81bd-150">managedDeviceOwnerType</span></span>|[<span data-ttu-id="d81bd-151">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="d81bd-151">managedDeviceOwnerType</span></span>](../resources/intune-devices-manageddeviceownertype.md)|<span data-ttu-id="d81bd-152">设备的所有权。</span><span class="sxs-lookup"><span data-stu-id="d81bd-152">Ownership of the device.</span></span> <span data-ttu-id="d81bd-153">可以是从[managedDevice](../resources/intune-devices-manageddevice.md)继承的 "公司" 或 "个人"。</span><span class="sxs-lookup"><span data-stu-id="d81bd-153">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="d81bd-154">可取值为：`unknown`、`company`、`personal`。</span><span class="sxs-lookup"><span data-stu-id="d81bd-154">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="d81bd-155">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="d81bd-155">deviceActionResults</span></span>|<span data-ttu-id="d81bd-156">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d81bd-156">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="d81bd-157">ComplexType deviceActionResult 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="d81bd-157">List of ComplexType deviceActionResult objects.</span></span> <span data-ttu-id="d81bd-158">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d81bd-158">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d81bd-159">managementState</span><span class="sxs-lookup"><span data-stu-id="d81bd-159">managementState</span></span>|[<span data-ttu-id="d81bd-160">managementState</span><span class="sxs-lookup"><span data-stu-id="d81bd-160">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="d81bd-161">设备的管理状态。</span><span class="sxs-lookup"><span data-stu-id="d81bd-161">Management state of the device.</span></span> <span data-ttu-id="d81bd-162">继承自[managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="d81bd-162">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="d81bd-163">可取值为：`managed`、`retirePending`、`retireFailed`、`wipePending`、`wipeFailed`、`unhealthy`、`deletePending`、`retireIssued`、`wipeIssued`、`wipeCanceled`、`retireCanceled`、`discovered`。</span><span class="sxs-lookup"><span data-stu-id="d81bd-163">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="d81bd-164">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="d81bd-164">enrolledDateTime</span></span>|<span data-ttu-id="d81bd-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d81bd-165">DateTimeOffset</span></span>|<span data-ttu-id="d81bd-166">设备的注册时间。</span><span class="sxs-lookup"><span data-stu-id="d81bd-166">Enrollment time of the device.</span></span> <span data-ttu-id="d81bd-167">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d81bd-167">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d81bd-168">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="d81bd-168">lastSyncDateTime</span></span>|<span data-ttu-id="d81bd-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d81bd-169">DateTimeOffset</span></span>|<span data-ttu-id="d81bd-170">设备上次成功完成与 Intune 同步的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="d81bd-170">The date and time that the device last completed a successful sync with Intune.</span></span> <span data-ttu-id="d81bd-171">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d81bd-171">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d81bd-172">chassisType</span><span class="sxs-lookup"><span data-stu-id="d81bd-172">chassisType</span></span>|[<span data-ttu-id="d81bd-173">chassisType</span><span class="sxs-lookup"><span data-stu-id="d81bd-173">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="d81bd-174">设备的机箱类型。</span><span class="sxs-lookup"><span data-stu-id="d81bd-174">Chassis type of the device.</span></span> <span data-ttu-id="d81bd-175">继承自[managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="d81bd-175">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="d81bd-176">可取值为：`unknown`、`desktop`、`laptop`、`worksWorkstation`、`enterpriseServer`、`phone`、`tablet`、`mobileOther`、`mobileUnknown`。</span><span class="sxs-lookup"><span data-stu-id="d81bd-176">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="d81bd-177">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="d81bd-177">operatingSystem</span></span>|<span data-ttu-id="d81bd-178">String</span><span class="sxs-lookup"><span data-stu-id="d81bd-178">String</span></span>|<span data-ttu-id="d81bd-179">设备的操作系统。</span><span class="sxs-lookup"><span data-stu-id="d81bd-179">Operating system of the device.</span></span> <span data-ttu-id="d81bd-180">Windows、iOS 等。继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d81bd-180">Windows, iOS, etc. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d81bd-181">deviceType</span><span class="sxs-lookup"><span data-stu-id="d81bd-181">deviceType</span></span>|[<span data-ttu-id="d81bd-182">deviceType</span><span class="sxs-lookup"><span data-stu-id="d81bd-182">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="d81bd-183">设备的平台。</span><span class="sxs-lookup"><span data-stu-id="d81bd-183">Platform of the device.</span></span> <span data-ttu-id="d81bd-184">继承自[managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="d81bd-184">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="d81bd-185">可能的值为`desktop`: `windowsRT`、 `winMO6`、 `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer`、、、、、、、、、、、、、、、、 `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="d81bd-185">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="d81bd-186">complianceState</span><span class="sxs-lookup"><span data-stu-id="d81bd-186">complianceState</span></span>|[<span data-ttu-id="d81bd-187">complianceState</span><span class="sxs-lookup"><span data-stu-id="d81bd-187">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="d81bd-188">设备的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="d81bd-188">Compliance state of the device.</span></span> <span data-ttu-id="d81bd-189">继承自[managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="d81bd-189">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="d81bd-190">可取值为：`unknown`、`compliant`、`noncompliant`、`conflict`、`error`、`inGracePeriod`、`configManager`。</span><span class="sxs-lookup"><span data-stu-id="d81bd-190">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="d81bd-191">jailBroken</span><span class="sxs-lookup"><span data-stu-id="d81bd-191">jailBroken</span></span>|<span data-ttu-id="d81bd-192">String</span><span class="sxs-lookup"><span data-stu-id="d81bd-192">String</span></span>|<span data-ttu-id="d81bd-193">设备是否已越狱或取得 root 权限。</span><span class="sxs-lookup"><span data-stu-id="d81bd-193">whether the device is jail broken or rooted.</span></span> <span data-ttu-id="d81bd-194">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d81bd-194">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d81bd-195">managementAgent</span><span class="sxs-lookup"><span data-stu-id="d81bd-195">managementAgent</span></span>|[<span data-ttu-id="d81bd-196">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="d81bd-196">managementAgentType</span></span>](../resources/intune-devices-managementagenttype.md)|<span data-ttu-id="d81bd-197">设备的管理通道。</span><span class="sxs-lookup"><span data-stu-id="d81bd-197">Management channel of the device.</span></span> <span data-ttu-id="d81bd-198">Intune、EAS 等。继承自[managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="d81bd-198">Intune, EAS, etc. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="d81bd-199">可取值为：`eas`、`mdm`、`easMdm`、`intuneClient`、`easIntuneClient`、`configurationManagerClient`、`configurationManagerClientMdm`、`configurationManagerClientMdmEas`、`unknown`、`jamf`、`googleCloudDevicePolicyController`、`microsoft365ManagedMdm`。</span><span class="sxs-lookup"><span data-stu-id="d81bd-199">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span></span>|
|<span data-ttu-id="d81bd-200">osVersion</span><span class="sxs-lookup"><span data-stu-id="d81bd-200">osVersion</span></span>|<span data-ttu-id="d81bd-201">String</span><span class="sxs-lookup"><span data-stu-id="d81bd-201">String</span></span>|<span data-ttu-id="d81bd-202">设备的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="d81bd-202">Operating system version of the device.</span></span> <span data-ttu-id="d81bd-203">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d81bd-203">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d81bd-204">easActivated</span><span class="sxs-lookup"><span data-stu-id="d81bd-204">easActivated</span></span>|<span data-ttu-id="d81bd-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="d81bd-205">Boolean</span></span>|<span data-ttu-id="d81bd-206">设备是否已激活 Exchange ActiveSync。</span><span class="sxs-lookup"><span data-stu-id="d81bd-206">Whether the device is Exchange ActiveSync activated.</span></span> <span data-ttu-id="d81bd-207">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d81bd-207">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d81bd-208">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="d81bd-208">easDeviceId</span></span>|<span data-ttu-id="d81bd-209">String</span><span class="sxs-lookup"><span data-stu-id="d81bd-209">String</span></span>|<span data-ttu-id="d81bd-210">设备的 Exchange ActiveSync ID。</span><span class="sxs-lookup"><span data-stu-id="d81bd-210">Exchange ActiveSync Id of the device.</span></span> <span data-ttu-id="d81bd-211">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d81bd-211">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d81bd-212">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="d81bd-212">easActivationDateTime</span></span>|<span data-ttu-id="d81bd-213">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d81bd-213">DateTimeOffset</span></span>|<span data-ttu-id="d81bd-214">设备的 Exchange ActivationSync 激活时间。</span><span class="sxs-lookup"><span data-stu-id="d81bd-214">Exchange ActivationSync activation time of the device.</span></span> <span data-ttu-id="d81bd-215">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d81bd-215">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d81bd-216">aadRegistered</span><span class="sxs-lookup"><span data-stu-id="d81bd-216">aadRegistered</span></span>|<span data-ttu-id="d81bd-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="d81bd-217">Boolean</span></span>|<span data-ttu-id="d81bd-218">设备是否已注册 Azure Active Directory。</span><span class="sxs-lookup"><span data-stu-id="d81bd-218">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="d81bd-219">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d81bd-219">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d81bd-220">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="d81bd-220">azureADRegistered</span></span>|<span data-ttu-id="d81bd-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="d81bd-221">Boolean</span></span>|<span data-ttu-id="d81bd-222">设备是否已注册 Azure Active Directory。</span><span class="sxs-lookup"><span data-stu-id="d81bd-222">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="d81bd-223">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d81bd-223">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d81bd-224">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="d81bd-224">deviceEnrollmentType</span></span>|[<span data-ttu-id="d81bd-225">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="d81bd-225">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="d81bd-226">设备的注册类型。</span><span class="sxs-lookup"><span data-stu-id="d81bd-226">Enrollment type of the device.</span></span> <span data-ttu-id="d81bd-227">继承自[managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="d81bd-227">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="d81bd-228">可取值为：`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement`。</span><span class="sxs-lookup"><span data-stu-id="d81bd-228">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="d81bd-229">lostModeState</span><span class="sxs-lookup"><span data-stu-id="d81bd-229">lostModeState</span></span>|[<span data-ttu-id="d81bd-230">lostModeState</span><span class="sxs-lookup"><span data-stu-id="d81bd-230">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="d81bd-231">指示是否已启用或禁用从[managedDevice](../resources/intune-devices-manageddevice.md)继承的已丢失模式。</span><span class="sxs-lookup"><span data-stu-id="d81bd-231">Indicates if Lost mode is enabled or disabled Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="d81bd-232">可取值为：`disabled`、`enabled`。</span><span class="sxs-lookup"><span data-stu-id="d81bd-232">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="d81bd-233">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="d81bd-233">activationLockBypassCode</span></span>|<span data-ttu-id="d81bd-234">String</span><span class="sxs-lookup"><span data-stu-id="d81bd-234">String</span></span>|<span data-ttu-id="d81bd-235">允许绕过设备上的激活锁的代码。</span><span class="sxs-lookup"><span data-stu-id="d81bd-235">Code that allows the Activation Lock on a device to be bypassed.</span></span> <span data-ttu-id="d81bd-236">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d81bd-236">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d81bd-237">emailAddress</span><span class="sxs-lookup"><span data-stu-id="d81bd-237">emailAddress</span></span>|<span data-ttu-id="d81bd-238">String</span><span class="sxs-lookup"><span data-stu-id="d81bd-238">String</span></span>|<span data-ttu-id="d81bd-239">与从[managedDevice](../resources/intune-devices-manageddevice.md)继承的设备关联的用户的电子邮件</span><span class="sxs-lookup"><span data-stu-id="d81bd-239">Email(s) for the user associated with the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d81bd-240">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="d81bd-240">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="d81bd-241">String</span><span class="sxs-lookup"><span data-stu-id="d81bd-241">String</span></span>|<span data-ttu-id="d81bd-242">Azure Active Directory 设备的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="d81bd-242">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="d81bd-243">只读。</span><span class="sxs-lookup"><span data-stu-id="d81bd-243">Read only.</span></span> <span data-ttu-id="d81bd-244">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d81bd-244">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d81bd-245">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="d81bd-245">azureADDeviceId</span></span>|<span data-ttu-id="d81bd-246">String</span><span class="sxs-lookup"><span data-stu-id="d81bd-246">String</span></span>|<span data-ttu-id="d81bd-247">Azure Active Directory 设备的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="d81bd-247">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="d81bd-248">只读。</span><span class="sxs-lookup"><span data-stu-id="d81bd-248">Read only.</span></span> <span data-ttu-id="d81bd-249">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d81bd-249">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d81bd-250">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="d81bd-250">deviceRegistrationState</span></span>|[<span data-ttu-id="d81bd-251">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="d81bd-251">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="d81bd-252">设备注册状态。</span><span class="sxs-lookup"><span data-stu-id="d81bd-252">Device registration state.</span></span> <span data-ttu-id="d81bd-253">继承自[managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="d81bd-253">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="d81bd-254">可取值为：`notRegistered`、`registered`、`revoked`、`keyConflict`、`approvalPending`、`certificateReset`、`notRegisteredPendingEnrollment`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="d81bd-254">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="d81bd-255">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="d81bd-255">deviceCategoryDisplayName</span></span>|<span data-ttu-id="d81bd-256">String</span><span class="sxs-lookup"><span data-stu-id="d81bd-256">String</span></span>|<span data-ttu-id="d81bd-257">继承自[managedDevice](../resources/intune-devices-manageddevice.md)的设备类别显示名称</span><span class="sxs-lookup"><span data-stu-id="d81bd-257">Device category display name Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d81bd-258">isSupervised</span><span class="sxs-lookup"><span data-stu-id="d81bd-258">isSupervised</span></span>|<span data-ttu-id="d81bd-259">Boolean</span><span class="sxs-lookup"><span data-stu-id="d81bd-259">Boolean</span></span>|<span data-ttu-id="d81bd-260">从[managedDevice](../resources/intune-devices-manageddevice.md)继承的设备监督状态</span><span class="sxs-lookup"><span data-stu-id="d81bd-260">Device supervised status Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d81bd-261">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="d81bd-261">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="d81bd-262">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d81bd-262">DateTimeOffset</span></span>|<span data-ttu-id="d81bd-263">设备上次与 Exchange 联系的时间。</span><span class="sxs-lookup"><span data-stu-id="d81bd-263">Last time the device contacted Exchange.</span></span> <span data-ttu-id="d81bd-264">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d81bd-264">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d81bd-265">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="d81bd-265">exchangeAccessState</span></span>|[<span data-ttu-id="d81bd-266">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="d81bd-266">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="d81bd-267">Exchange 中设备的访问状态。</span><span class="sxs-lookup"><span data-stu-id="d81bd-267">The Access State of the device in Exchange.</span></span> <span data-ttu-id="d81bd-268">继承自[managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="d81bd-268">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="d81bd-269">可取值为：`none`、`unknown`、`allowed`、`blocked`、`quarantined`。</span><span class="sxs-lookup"><span data-stu-id="d81bd-269">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="d81bd-270">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="d81bd-270">exchangeAccessStateReason</span></span>|[<span data-ttu-id="d81bd-271">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="d81bd-271">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="d81bd-272">Exchange 中设备访问状态的出现原因。</span><span class="sxs-lookup"><span data-stu-id="d81bd-272">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="d81bd-273">继承自[managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="d81bd-273">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="d81bd-274">可取值为：`none`、`unknown`、`exchangeGlobalRule`、`exchangeIndividualRule`、`exchangeDeviceRule`、`exchangeUpgrade`、`exchangeMailboxPolicy`、`other`、`compliant`、`notCompliant`、`notEnrolled`、`unknownLocation`、`mfaRequired`、`azureADBlockDueToAccessPolicy`、`compromisedPassword`、`deviceNotKnownWithManagedApp`。</span><span class="sxs-lookup"><span data-stu-id="d81bd-274">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="d81bd-275">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="d81bd-275">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="d81bd-276">String</span><span class="sxs-lookup"><span data-stu-id="d81bd-276">String</span></span>|<span data-ttu-id="d81bd-277">允许与设备建立远程协助会话的 URL。</span><span class="sxs-lookup"><span data-stu-id="d81bd-277">Url that allows a Remote Assistance session to be established with the device.</span></span> <span data-ttu-id="d81bd-278">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d81bd-278">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d81bd-279">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="d81bd-279">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="d81bd-280">String</span><span class="sxs-lookup"><span data-stu-id="d81bd-280">String</span></span>|<span data-ttu-id="d81bd-281">用于在创建远程协助会话对象时识别问题的错误字符串。</span><span class="sxs-lookup"><span data-stu-id="d81bd-281">An error string that identifies issues when creating Remote Assistance session objects.</span></span> <span data-ttu-id="d81bd-282">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d81bd-282">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d81bd-283">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="d81bd-283">isEncrypted</span></span>|<span data-ttu-id="d81bd-284">Boolean</span><span class="sxs-lookup"><span data-stu-id="d81bd-284">Boolean</span></span>|<span data-ttu-id="d81bd-285">从[managedDevice](../resources/intune-devices-manageddevice.md)继承的设备加密状态</span><span class="sxs-lookup"><span data-stu-id="d81bd-285">Device encryption status Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d81bd-286">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d81bd-286">userPrincipalName</span></span>|<span data-ttu-id="d81bd-287">String</span><span class="sxs-lookup"><span data-stu-id="d81bd-287">String</span></span>|<span data-ttu-id="d81bd-288">从[managedDevice](../resources/intune-devices-manageddevice.md)继承的设备用户主体名称</span><span class="sxs-lookup"><span data-stu-id="d81bd-288">Device user principal name Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d81bd-289">model</span><span class="sxs-lookup"><span data-stu-id="d81bd-289">model</span></span>|<span data-ttu-id="d81bd-290">String</span><span class="sxs-lookup"><span data-stu-id="d81bd-290">String</span></span>|<span data-ttu-id="d81bd-291">继承自[managedDevice](../resources/intune-devices-manageddevice.md)的设备的模型</span><span class="sxs-lookup"><span data-stu-id="d81bd-291">Model of the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d81bd-292">manufacturer</span><span class="sxs-lookup"><span data-stu-id="d81bd-292">manufacturer</span></span>|<span data-ttu-id="d81bd-293">String</span><span class="sxs-lookup"><span data-stu-id="d81bd-293">String</span></span>|<span data-ttu-id="d81bd-294">继承自[managedDevice](../resources/intune-devices-manageddevice.md)的设备的制造商</span><span class="sxs-lookup"><span data-stu-id="d81bd-294">Manufacturer of the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d81bd-295">imei</span><span class="sxs-lookup"><span data-stu-id="d81bd-295">imei</span></span>|<span data-ttu-id="d81bd-296">String</span><span class="sxs-lookup"><span data-stu-id="d81bd-296">String</span></span>|<span data-ttu-id="d81bd-297">从[managedDevice](../resources/intune-devices-manageddevice.md)继承的 IMEI</span><span class="sxs-lookup"><span data-stu-id="d81bd-297">IMEI Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d81bd-298">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="d81bd-298">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="d81bd-299">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d81bd-299">DateTimeOffset</span></span>|<span data-ttu-id="d81bd-300">设备符合性宽限期过期时间从[managedDevice](../resources/intune-devices-manageddevice.md)继承的日期/时间</span><span class="sxs-lookup"><span data-stu-id="d81bd-300">The DateTime when device compliance grace period expires Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d81bd-301">serialNumber</span><span class="sxs-lookup"><span data-stu-id="d81bd-301">serialNumber</span></span>|<span data-ttu-id="d81bd-302">字符串</span><span class="sxs-lookup"><span data-stu-id="d81bd-302">String</span></span>|<span data-ttu-id="d81bd-303">SerialNumber 继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d81bd-303">SerialNumber Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d81bd-304">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="d81bd-304">phoneNumber</span></span>|<span data-ttu-id="d81bd-305">String</span><span class="sxs-lookup"><span data-stu-id="d81bd-305">String</span></span>|<span data-ttu-id="d81bd-306">继承自[managedDevice](../resources/intune-devices-manageddevice.md)的设备的电话号码</span><span class="sxs-lookup"><span data-stu-id="d81bd-306">Phone number of the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d81bd-307">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="d81bd-307">androidSecurityPatchLevel</span></span>|<span data-ttu-id="d81bd-308">String</span><span class="sxs-lookup"><span data-stu-id="d81bd-308">String</span></span>|<span data-ttu-id="d81bd-309">从[managedDevice](../resources/intune-devices-manageddevice.md)继承的 Android 安全修补程序级别</span><span class="sxs-lookup"><span data-stu-id="d81bd-309">Android security patch level Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d81bd-310">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="d81bd-310">userDisplayName</span></span>|<span data-ttu-id="d81bd-311">String</span><span class="sxs-lookup"><span data-stu-id="d81bd-311">String</span></span>|<span data-ttu-id="d81bd-312">从[managedDevice](../resources/intune-devices-manageddevice.md)继承的用户显示名称</span><span class="sxs-lookup"><span data-stu-id="d81bd-312">User display name Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d81bd-313">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="d81bd-313">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="d81bd-314">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="d81bd-314">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="d81bd-315">继承自[managedDevice](../resources/intune-devices-manageddevice.md)的 ConfigrMgr 客户端启用的功能</span><span class="sxs-lookup"><span data-stu-id="d81bd-315">ConfigrMgr client enabled features Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d81bd-316">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="d81bd-316">wiFiMacAddress</span></span>|<span data-ttu-id="d81bd-317">String</span><span class="sxs-lookup"><span data-stu-id="d81bd-317">String</span></span>|<span data-ttu-id="d81bd-318">从[managedDevice](../resources/intune-devices-manageddevice.md)继承的 wi-fi MAC</span><span class="sxs-lookup"><span data-stu-id="d81bd-318">Wi-Fi MAC Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d81bd-319">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="d81bd-319">deviceHealthAttestationState</span></span>|[<span data-ttu-id="d81bd-320">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="d81bd-320">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="d81bd-321">设备运行状况证明状态。</span><span class="sxs-lookup"><span data-stu-id="d81bd-321">The device health attestation state.</span></span> <span data-ttu-id="d81bd-322">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d81bd-322">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d81bd-323">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="d81bd-323">subscriberCarrier</span></span>|<span data-ttu-id="d81bd-324">String</span><span class="sxs-lookup"><span data-stu-id="d81bd-324">String</span></span>|<span data-ttu-id="d81bd-325">从[managedDevice](../resources/intune-devices-manageddevice.md)继承的订阅者运营商</span><span class="sxs-lookup"><span data-stu-id="d81bd-325">Subscriber Carrier Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d81bd-326">meid</span><span class="sxs-lookup"><span data-stu-id="d81bd-326">meid</span></span>|<span data-ttu-id="d81bd-327">String</span><span class="sxs-lookup"><span data-stu-id="d81bd-327">String</span></span>|<span data-ttu-id="d81bd-328">MEID 继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d81bd-328">MEID Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d81bd-329">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="d81bd-329">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="d81bd-330">Int64</span><span class="sxs-lookup"><span data-stu-id="d81bd-330">Int64</span></span>|<span data-ttu-id="d81bd-331">从[managedDevice](../resources/intune-devices-manageddevice.md)继承的总存储量 (以字节为单位)</span><span class="sxs-lookup"><span data-stu-id="d81bd-331">Total Storage in Bytes Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d81bd-332">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="d81bd-332">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="d81bd-333">Int64</span><span class="sxs-lookup"><span data-stu-id="d81bd-333">Int64</span></span>|<span data-ttu-id="d81bd-334">从[managedDevice](../resources/intune-devices-manageddevice.md)继承的可用存储量 (以字节为单位)</span><span class="sxs-lookup"><span data-stu-id="d81bd-334">Free Storage in Bytes Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d81bd-335">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="d81bd-335">managedDeviceName</span></span>|<span data-ttu-id="d81bd-336">String</span><span class="sxs-lookup"><span data-stu-id="d81bd-336">String</span></span>|<span data-ttu-id="d81bd-337">用于识别设备的自动生成的名称。</span><span class="sxs-lookup"><span data-stu-id="d81bd-337">Automatically generated name to identify a device.</span></span> <span data-ttu-id="d81bd-338">可以覆盖为用户友好名称。</span><span class="sxs-lookup"><span data-stu-id="d81bd-338">Can be overwritten to a user friendly name.</span></span> <span data-ttu-id="d81bd-339">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d81bd-339">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d81bd-340">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="d81bd-340">partnerReportedThreatState</span></span>|[<span data-ttu-id="d81bd-341">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="d81bd-341">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="d81bd-342">指示帐户和设备正在使用移动威胁防护合作伙伴时设备的威胁状态。</span><span class="sxs-lookup"><span data-stu-id="d81bd-342">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="d81bd-343">只读。</span><span class="sxs-lookup"><span data-stu-id="d81bd-343">Read Only.</span></span> <span data-ttu-id="d81bd-344">继承自[managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="d81bd-344">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="d81bd-345">可取值为：`unknown`、`activated`、`deactivated`、`secured`、`lowSeverity`、`mediumSeverity`、`highSeverity`、`unresponsive`、`compromised`、`misconfigured`。</span><span class="sxs-lookup"><span data-stu-id="d81bd-345">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="d81bd-346">usersLoggedOn</span><span class="sxs-lookup"><span data-stu-id="d81bd-346">usersLoggedOn</span></span>|<span data-ttu-id="d81bd-347">[loggedOnUser](../resources/intune-devices-loggedonuser.md)集合</span><span class="sxs-lookup"><span data-stu-id="d81bd-347">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="d81bd-348">指示从[managedDevice](../resources/intune-devices-manageddevice.md)继承的设备的上次登录用户</span><span class="sxs-lookup"><span data-stu-id="d81bd-348">Indicates the last logged on users of a device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d81bd-349">preferMdmOverGroupPolicyAppliedDateTime</span><span class="sxs-lookup"><span data-stu-id="d81bd-349">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="d81bd-350">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d81bd-350">DateTimeOffset</span></span>|<span data-ttu-id="d81bd-351">报告设置了 preferMdmOverGroupPolicy 设置的 DateTime。</span><span class="sxs-lookup"><span data-stu-id="d81bd-351">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="d81bd-352">设置后, 如果存在冲突, Intune MDM 设置将覆盖组策略设置。</span><span class="sxs-lookup"><span data-stu-id="d81bd-352">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="d81bd-353">只读。</span><span class="sxs-lookup"><span data-stu-id="d81bd-353">Read Only.</span></span> <span data-ttu-id="d81bd-354">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d81bd-354">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d81bd-355">autopilotEnrolled</span><span class="sxs-lookup"><span data-stu-id="d81bd-355">autopilotEnrolled</span></span>|<span data-ttu-id="d81bd-356">Boolean</span><span class="sxs-lookup"><span data-stu-id="d81bd-356">Boolean</span></span>|<span data-ttu-id="d81bd-357">如果托管设备是通过自动引导注册的, 则报告。</span><span class="sxs-lookup"><span data-stu-id="d81bd-357">Reports if the managed device is enrolled via auto-pilot.</span></span> <span data-ttu-id="d81bd-358">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d81bd-358">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d81bd-359">requireUserEnrollmentApproval</span><span class="sxs-lookup"><span data-stu-id="d81bd-359">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="d81bd-360">Boolean</span><span class="sxs-lookup"><span data-stu-id="d81bd-360">Boolean</span></span>|<span data-ttu-id="d81bd-361">如果托管 iOS 设备是用户审批注册, 则报告。</span><span class="sxs-lookup"><span data-stu-id="d81bd-361">Reports if the managed iOS device is user approval enrollment.</span></span> <span data-ttu-id="d81bd-362">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d81bd-362">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d81bd-363">managementCertificateExpirationDate</span><span class="sxs-lookup"><span data-stu-id="d81bd-363">managementCertificateExpirationDate</span></span>|<span data-ttu-id="d81bd-364">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d81bd-364">DateTimeOffset</span></span>|<span data-ttu-id="d81bd-365">报告设备管理证书到期日期继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d81bd-365">Reports device management certificate expiration date Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d81bd-366">iccid</span><span class="sxs-lookup"><span data-stu-id="d81bd-366">iccid</span></span>|<span data-ttu-id="d81bd-367">String</span><span class="sxs-lookup"><span data-stu-id="d81bd-367">String</span></span>|<span data-ttu-id="d81bd-368">集成的电路卡标识符, 它是 SIM 卡的唯一标识号。</span><span class="sxs-lookup"><span data-stu-id="d81bd-368">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span> <span data-ttu-id="d81bd-369">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d81bd-369">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d81bd-370">udid</span><span class="sxs-lookup"><span data-stu-id="d81bd-370">udid</span></span>|<span data-ttu-id="d81bd-371">String</span><span class="sxs-lookup"><span data-stu-id="d81bd-371">String</span></span>|<span data-ttu-id="d81bd-372">iOS 和 macOS 设备的唯一设备标识符。</span><span class="sxs-lookup"><span data-stu-id="d81bd-372">Unique Device Identifier for iOS and macOS devices.</span></span> <span data-ttu-id="d81bd-373">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d81bd-373">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d81bd-374">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d81bd-374">roleScopeTagIds</span></span>|<span data-ttu-id="d81bd-375">String 集合</span><span class="sxs-lookup"><span data-stu-id="d81bd-375">String collection</span></span>|<span data-ttu-id="d81bd-376">此设备实例的范围标记 id 的列表。</span><span class="sxs-lookup"><span data-stu-id="d81bd-376">List of Scope Tag IDs for this Device instance.</span></span> <span data-ttu-id="d81bd-377">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d81bd-377">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d81bd-378">windowsActiveMalwareCount</span><span class="sxs-lookup"><span data-stu-id="d81bd-378">windowsActiveMalwareCount</span></span>|<span data-ttu-id="d81bd-379">Int32</span><span class="sxs-lookup"><span data-stu-id="d81bd-379">Int32</span></span>|<span data-ttu-id="d81bd-380">从[managedDevice](../resources/intune-devices-manageddevice.md)继承的此 windows 设备的活动恶意软件的计数</span><span class="sxs-lookup"><span data-stu-id="d81bd-380">Count of active malware for this windows device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d81bd-381">windowsRemediatedMalwareCount</span><span class="sxs-lookup"><span data-stu-id="d81bd-381">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="d81bd-382">Int32</span><span class="sxs-lookup"><span data-stu-id="d81bd-382">Int32</span></span>|<span data-ttu-id="d81bd-383">从[managedDevice](../resources/intune-devices-manageddevice.md)继承的此 windows 设备的修正的恶意软件的计数</span><span class="sxs-lookup"><span data-stu-id="d81bd-383">Count of remediated malware for this windows device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d81bd-384">notes</span><span class="sxs-lookup"><span data-stu-id="d81bd-384">notes</span></span>|<span data-ttu-id="d81bd-385">String</span><span class="sxs-lookup"><span data-stu-id="d81bd-385">String</span></span>|<span data-ttu-id="d81bd-386">由 IT 管理员创建的设备上的注释继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d81bd-386">Notes on the device created by IT Admin Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d81bd-387">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="d81bd-387">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="d81bd-388">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="d81bd-388">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="d81bd-389">Configuration manager 客户端运行状况状态, 仅适用于从[managedDevice](../resources/intune-devices-manageddevice.md)继承的 MDM/ConfigMgr 代理所管理的设备</span><span class="sxs-lookup"><span data-stu-id="d81bd-389">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|



## <a name="response"></a><span data-ttu-id="d81bd-390">响应</span><span class="sxs-lookup"><span data-stu-id="d81bd-390">Response</span></span>
<span data-ttu-id="d81bd-391">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d81bd-391">If successful, this method returns a `200 OK` response code and an updated [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d81bd-392">示例</span><span class="sxs-lookup"><span data-stu-id="d81bd-392">Example</span></span>

### <a name="request"></a><span data-ttu-id="d81bd-393">请求</span><span class="sxs-lookup"><span data-stu-id="d81bd-393">Request</span></span>
<span data-ttu-id="d81bd-394">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d81bd-394">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/users/{usersId}/managedDevices/{managedDeviceId}
Content-type: application/json
Content-length: 7231

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

### <a name="response"></a><span data-ttu-id="d81bd-395">响应</span><span class="sxs-lookup"><span data-stu-id="d81bd-395">Response</span></span>
<span data-ttu-id="d81bd-p141">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d81bd-p141">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 7280

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




