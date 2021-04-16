---
title: 更新 windowsManagedDevice
description: 更新 windowsManagedDevice 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 48a90be42f02ef49a8e9dd045aa70d2cbdbe74a5
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51867873"
---
# <a name="update-windowsmanageddevice"></a><span data-ttu-id="00586-103">更新 windowsManagedDevice</span><span class="sxs-lookup"><span data-stu-id="00586-103">Update windowsManagedDevice</span></span>

<span data-ttu-id="00586-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="00586-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="00586-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="00586-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="00586-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="00586-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="00586-107">更新 [windowsManagedDevice 对象](../resources/intune-devices-windowsmanageddevice.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="00586-107">Update the properties of a [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="00586-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="00586-108">Prerequisites</span></span>
<span data-ttu-id="00586-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="00586-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00586-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="00586-111">Permission type</span></span>|<span data-ttu-id="00586-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="00586-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="00586-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="00586-113">Delegated (work or school account)</span></span>|<span data-ttu-id="00586-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00586-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="00586-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="00586-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="00586-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="00586-116">Not supported.</span></span>|
|<span data-ttu-id="00586-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="00586-117">Application</span></span>|<span data-ttu-id="00586-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00586-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="00586-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="00586-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="00586-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="00586-120">Request headers</span></span>
|<span data-ttu-id="00586-121">标头</span><span class="sxs-lookup"><span data-stu-id="00586-121">Header</span></span>|<span data-ttu-id="00586-122">值</span><span class="sxs-lookup"><span data-stu-id="00586-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="00586-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="00586-123">Authorization</span></span>|<span data-ttu-id="00586-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="00586-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="00586-125">接受</span><span class="sxs-lookup"><span data-stu-id="00586-125">Accept</span></span>|<span data-ttu-id="00586-126">application/json</span><span class="sxs-lookup"><span data-stu-id="00586-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="00586-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="00586-127">Request body</span></span>
<span data-ttu-id="00586-128">在请求正文中，提供 [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="00586-128">In the request body, supply a JSON representation for the [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object.</span></span>

<span data-ttu-id="00586-129">下表显示创建 [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="00586-129">The following table shows the properties that are required when you create the [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md).</span></span>

|<span data-ttu-id="00586-130">属性</span><span class="sxs-lookup"><span data-stu-id="00586-130">Property</span></span>|<span data-ttu-id="00586-131">类型</span><span class="sxs-lookup"><span data-stu-id="00586-131">Type</span></span>|<span data-ttu-id="00586-132">说明</span><span class="sxs-lookup"><span data-stu-id="00586-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00586-133">id</span><span class="sxs-lookup"><span data-stu-id="00586-133">id</span></span>|<span data-ttu-id="00586-134">String</span><span class="sxs-lookup"><span data-stu-id="00586-134">String</span></span>|<span data-ttu-id="00586-135">设备的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="00586-135">Unique Identifier for the device.</span></span> <span data-ttu-id="00586-136">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="00586-136">This property is read-only.</span></span> <span data-ttu-id="00586-137">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="00586-137">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="00586-138">userId</span><span class="sxs-lookup"><span data-stu-id="00586-138">userId</span></span>|<span data-ttu-id="00586-139">String</span><span class="sxs-lookup"><span data-stu-id="00586-139">String</span></span>|<span data-ttu-id="00586-140">与设备关联的用户的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="00586-140">Unique Identifier for the user associated with the device.</span></span> <span data-ttu-id="00586-141">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="00586-141">This property is read-only.</span></span> <span data-ttu-id="00586-142">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="00586-142">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="00586-143">deviceName</span><span class="sxs-lookup"><span data-stu-id="00586-143">deviceName</span></span>|<span data-ttu-id="00586-144">String</span><span class="sxs-lookup"><span data-stu-id="00586-144">String</span></span>|<span data-ttu-id="00586-145">设备的名称。</span><span class="sxs-lookup"><span data-stu-id="00586-145">Name of the device.</span></span> <span data-ttu-id="00586-146">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="00586-146">This property is read-only.</span></span> <span data-ttu-id="00586-147">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="00586-147">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="00586-148">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="00586-148">hardwareInformation</span></span>|[<span data-ttu-id="00586-149">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="00586-149">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="00586-150">设备的硬向详细信息。</span><span class="sxs-lookup"><span data-stu-id="00586-150">The hardward details for the device.</span></span>  <span data-ttu-id="00586-151">包括存储空间、制造商、序列号等信息。此属性为只读。</span><span class="sxs-lookup"><span data-stu-id="00586-151">Includes information such as storage space, manufacturer, serial number, etc. This property is read-only.</span></span> <span data-ttu-id="00586-152">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="00586-152">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="00586-153">ownerType</span><span class="sxs-lookup"><span data-stu-id="00586-153">ownerType</span></span>|[<span data-ttu-id="00586-154">ownerType</span><span class="sxs-lookup"><span data-stu-id="00586-154">ownerType</span></span>](../resources/intune-shared-ownertype.md)|<span data-ttu-id="00586-155">设备的所有权。</span><span class="sxs-lookup"><span data-stu-id="00586-155">Ownership of the device.</span></span> <span data-ttu-id="00586-156">可以是"company"或"personal"继承自 [managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="00586-156">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="00586-157">可取值为：`unknown`、`company`、`personal`。</span><span class="sxs-lookup"><span data-stu-id="00586-157">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="00586-158">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="00586-158">managedDeviceOwnerType</span></span>|[<span data-ttu-id="00586-159">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="00586-159">managedDeviceOwnerType</span></span>](../resources/intune-shared-manageddeviceownertype.md)|<span data-ttu-id="00586-160">设备的所有权。</span><span class="sxs-lookup"><span data-stu-id="00586-160">Ownership of the device.</span></span> <span data-ttu-id="00586-161">可以是"company"或"personal"继承自 [managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="00586-161">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="00586-162">可取值为：`unknown`、`company`、`personal`。</span><span class="sxs-lookup"><span data-stu-id="00586-162">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="00586-163">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="00586-163">deviceActionResults</span></span>|<span data-ttu-id="00586-164">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) 集合</span><span class="sxs-lookup"><span data-stu-id="00586-164">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="00586-165">ComplexType deviceActionResult 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="00586-165">List of ComplexType deviceActionResult objects.</span></span> <span data-ttu-id="00586-166">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="00586-166">This property is read-only.</span></span> <span data-ttu-id="00586-167">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="00586-167">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="00586-168">managementState</span><span class="sxs-lookup"><span data-stu-id="00586-168">managementState</span></span>|[<span data-ttu-id="00586-169">managementState</span><span class="sxs-lookup"><span data-stu-id="00586-169">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="00586-170">设备的管理状态。</span><span class="sxs-lookup"><span data-stu-id="00586-170">Management state of the device.</span></span> <span data-ttu-id="00586-171">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="00586-171">This property is read-only.</span></span> <span data-ttu-id="00586-172">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="00586-172">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="00586-173">可取值为：`managed`、`retirePending`、`retireFailed`、`wipePending`、`wipeFailed`、`unhealthy`、`deletePending`、`retireIssued`、`wipeIssued`、`wipeCanceled`、`retireCanceled`、`discovered`。</span><span class="sxs-lookup"><span data-stu-id="00586-173">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="00586-174">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="00586-174">enrolledDateTime</span></span>|<span data-ttu-id="00586-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00586-175">DateTimeOffset</span></span>|<span data-ttu-id="00586-176">设备的注册时间。</span><span class="sxs-lookup"><span data-stu-id="00586-176">Enrollment time of the device.</span></span> <span data-ttu-id="00586-177">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="00586-177">This property is read-only.</span></span> <span data-ttu-id="00586-178">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="00586-178">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="00586-179">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="00586-179">lastSyncDateTime</span></span>|<span data-ttu-id="00586-180">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00586-180">DateTimeOffset</span></span>|<span data-ttu-id="00586-181">设备上次成功完成与 Intune 同步的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="00586-181">The date and time that the device last completed a successful sync with Intune.</span></span> <span data-ttu-id="00586-182">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="00586-182">This property is read-only.</span></span> <span data-ttu-id="00586-183">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="00586-183">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="00586-184">chassisType</span><span class="sxs-lookup"><span data-stu-id="00586-184">chassisType</span></span>|[<span data-ttu-id="00586-185">chassisType</span><span class="sxs-lookup"><span data-stu-id="00586-185">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="00586-186">设备的机架类型。</span><span class="sxs-lookup"><span data-stu-id="00586-186">Chassis type of the device.</span></span> <span data-ttu-id="00586-187">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="00586-187">This property is read-only.</span></span> <span data-ttu-id="00586-188">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="00586-188">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="00586-189">可取值为：`unknown`、`desktop`、`laptop`、`worksWorkstation`、`enterpriseServer`、`phone`、`tablet`、`mobileOther`、`mobileUnknown`。</span><span class="sxs-lookup"><span data-stu-id="00586-189">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="00586-190">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="00586-190">operatingSystem</span></span>|<span data-ttu-id="00586-191">String</span><span class="sxs-lookup"><span data-stu-id="00586-191">String</span></span>|<span data-ttu-id="00586-192">设备的操作系统。</span><span class="sxs-lookup"><span data-stu-id="00586-192">Operating system of the device.</span></span> <span data-ttu-id="00586-193">Windows、iOS 等。此属性为只读。</span><span class="sxs-lookup"><span data-stu-id="00586-193">Windows, iOS, etc. This property is read-only.</span></span> <span data-ttu-id="00586-194">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="00586-194">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="00586-195">deviceType</span><span class="sxs-lookup"><span data-stu-id="00586-195">deviceType</span></span>|[<span data-ttu-id="00586-196">deviceType</span><span class="sxs-lookup"><span data-stu-id="00586-196">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="00586-197">设备平台。</span><span class="sxs-lookup"><span data-stu-id="00586-197">Platform of the device.</span></span> <span data-ttu-id="00586-198">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="00586-198">This property is read-only.</span></span> <span data-ttu-id="00586-199">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="00586-199">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="00586-200">可能的值是 `desktop` `windowsRT` `winMO6` ：、、、、、、、、、、 `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `windows10x` `androidnGMS` `linux` `blackberry` `palm` `unknown` `cloudPC` 、</span><span class="sxs-lookup"><span data-stu-id="00586-200">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `androidnGMS`, `linux`, `blackberry`, `palm`, `unknown`, `cloudPC`.</span></span>|
|<span data-ttu-id="00586-201">complianceState</span><span class="sxs-lookup"><span data-stu-id="00586-201">complianceState</span></span>|[<span data-ttu-id="00586-202">complianceState</span><span class="sxs-lookup"><span data-stu-id="00586-202">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="00586-203">设备的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="00586-203">Compliance state of the device.</span></span> <span data-ttu-id="00586-204">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="00586-204">This property is read-only.</span></span> <span data-ttu-id="00586-205">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="00586-205">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="00586-206">可取值为：`unknown`、`compliant`、`noncompliant`、`conflict`、`error`、`inGracePeriod`、`configManager`。</span><span class="sxs-lookup"><span data-stu-id="00586-206">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="00586-207">jailBroken</span><span class="sxs-lookup"><span data-stu-id="00586-207">jailBroken</span></span>|<span data-ttu-id="00586-208">String</span><span class="sxs-lookup"><span data-stu-id="00586-208">String</span></span>|<span data-ttu-id="00586-209">设备是否已越狱或取得 root 权限。</span><span class="sxs-lookup"><span data-stu-id="00586-209">whether the device is jail broken or rooted.</span></span> <span data-ttu-id="00586-210">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="00586-210">This property is read-only.</span></span> <span data-ttu-id="00586-211">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="00586-211">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="00586-212">managementAgent</span><span class="sxs-lookup"><span data-stu-id="00586-212">managementAgent</span></span>|[<span data-ttu-id="00586-213">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="00586-213">managementAgentType</span></span>](../resources/intune-shared-managementagenttype.md)|<span data-ttu-id="00586-214">设备的管理通道。</span><span class="sxs-lookup"><span data-stu-id="00586-214">Management channel of the device.</span></span> <span data-ttu-id="00586-215">Intune、EAS 等此属性为只读。</span><span class="sxs-lookup"><span data-stu-id="00586-215">Intune, EAS, etc. This property is read-only.</span></span> <span data-ttu-id="00586-216">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="00586-216">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="00586-217">可能的值是：`eas`、`mdm`、`easMdm`、`intuneClient`、`easIntuneClient`、`configurationManagerClient`、`configurationManagerClientMdm`、`configurationManagerClientMdmEas`、`unknown`、`jamf`、`googleCloudDevicePolicyController`、`microsoft365ManagedMdm`、`msSense`。</span><span class="sxs-lookup"><span data-stu-id="00586-217">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`, `msSense`.</span></span>|
|<span data-ttu-id="00586-218">osVersion</span><span class="sxs-lookup"><span data-stu-id="00586-218">osVersion</span></span>|<span data-ttu-id="00586-219">String</span><span class="sxs-lookup"><span data-stu-id="00586-219">String</span></span>|<span data-ttu-id="00586-220">设备的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="00586-220">Operating system version of the device.</span></span> <span data-ttu-id="00586-221">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="00586-221">This property is read-only.</span></span> <span data-ttu-id="00586-222">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="00586-222">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="00586-223">easActivated</span><span class="sxs-lookup"><span data-stu-id="00586-223">easActivated</span></span>|<span data-ttu-id="00586-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="00586-224">Boolean</span></span>|<span data-ttu-id="00586-225">设备是否已激活 Exchange ActiveSync。</span><span class="sxs-lookup"><span data-stu-id="00586-225">Whether the device is Exchange ActiveSync activated.</span></span> <span data-ttu-id="00586-226">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="00586-226">This property is read-only.</span></span> <span data-ttu-id="00586-227">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="00586-227">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="00586-228">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="00586-228">easDeviceId</span></span>|<span data-ttu-id="00586-229">String</span><span class="sxs-lookup"><span data-stu-id="00586-229">String</span></span>|<span data-ttu-id="00586-230">设备的 Exchange ActiveSync ID。</span><span class="sxs-lookup"><span data-stu-id="00586-230">Exchange ActiveSync Id of the device.</span></span> <span data-ttu-id="00586-231">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="00586-231">This property is read-only.</span></span> <span data-ttu-id="00586-232">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="00586-232">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="00586-233">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="00586-233">easActivationDateTime</span></span>|<span data-ttu-id="00586-234">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00586-234">DateTimeOffset</span></span>|<span data-ttu-id="00586-235">设备的 Exchange ActivationSync 激活时间。</span><span class="sxs-lookup"><span data-stu-id="00586-235">Exchange ActivationSync activation time of the device.</span></span> <span data-ttu-id="00586-236">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="00586-236">This property is read-only.</span></span> <span data-ttu-id="00586-237">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="00586-237">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="00586-238">aadRegistered</span><span class="sxs-lookup"><span data-stu-id="00586-238">aadRegistered</span></span>|<span data-ttu-id="00586-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="00586-239">Boolean</span></span>|<span data-ttu-id="00586-240">设备是否已注册 Azure Active Directory。</span><span class="sxs-lookup"><span data-stu-id="00586-240">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="00586-241">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="00586-241">This property is read-only.</span></span> <span data-ttu-id="00586-242">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="00586-242">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="00586-243">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="00586-243">azureADRegistered</span></span>|<span data-ttu-id="00586-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="00586-244">Boolean</span></span>|<span data-ttu-id="00586-245">设备是否已注册 Azure Active Directory。</span><span class="sxs-lookup"><span data-stu-id="00586-245">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="00586-246">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="00586-246">This property is read-only.</span></span> <span data-ttu-id="00586-247">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="00586-247">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="00586-248">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="00586-248">deviceEnrollmentType</span></span>|[<span data-ttu-id="00586-249">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="00586-249">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="00586-250">设备的注册类型。</span><span class="sxs-lookup"><span data-stu-id="00586-250">Enrollment type of the device.</span></span> <span data-ttu-id="00586-251">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="00586-251">This property is read-only.</span></span> <span data-ttu-id="00586-252">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="00586-252">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="00586-253">可能的值是 `unknown` `userEnrollment` `deviceEnrollmentManager` ：、、、、、、、、、 `appleBulkWithUser` `appleBulkWithoutUser` `windowsAzureADJoin` `windowsBulkUserless` `windowsAutoEnrollment` `windowsBulkAzureDomainJoin` `windowsCoManagement` `windowsAzureADJoinUsingDeviceAuth` `appleUserEnrollment` `appleUserEnrollmentWithServiceAccount` `azureAdJoinUsingAzureVmExtension` `androidEnterpriseDedicatedDevice` `androidEnterpriseFullyManaged` `androidEnterpriseCorporateWorkProfile` 。</span><span class="sxs-lookup"><span data-stu-id="00586-253">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `windowsAzureADJoinUsingDeviceAuth`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`, `azureAdJoinUsingAzureVmExtension`, `androidEnterpriseDedicatedDevice`, `androidEnterpriseFullyManaged`, `androidEnterpriseCorporateWorkProfile`.</span></span>|
|<span data-ttu-id="00586-254">lostModeState</span><span class="sxs-lookup"><span data-stu-id="00586-254">lostModeState</span></span>|[<span data-ttu-id="00586-255">lostModeState</span><span class="sxs-lookup"><span data-stu-id="00586-255">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="00586-256">指示是启用还是禁用丢失模式。</span><span class="sxs-lookup"><span data-stu-id="00586-256">Indicates if Lost mode is enabled or disabled.</span></span> <span data-ttu-id="00586-257">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="00586-257">This property is read-only.</span></span> <span data-ttu-id="00586-258">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="00586-258">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="00586-259">可取值为：`disabled`、`enabled`。</span><span class="sxs-lookup"><span data-stu-id="00586-259">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="00586-260">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="00586-260">activationLockBypassCode</span></span>|<span data-ttu-id="00586-261">String</span><span class="sxs-lookup"><span data-stu-id="00586-261">String</span></span>|<span data-ttu-id="00586-262">允许绕过设备上的激活锁的代码。</span><span class="sxs-lookup"><span data-stu-id="00586-262">Code that allows the Activation Lock on a device to be bypassed.</span></span> <span data-ttu-id="00586-263">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="00586-263">This property is read-only.</span></span> <span data-ttu-id="00586-264">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="00586-264">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="00586-265">emailAddress</span><span class="sxs-lookup"><span data-stu-id="00586-265">emailAddress</span></span>|<span data-ttu-id="00586-266">String</span><span class="sxs-lookup"><span data-stu-id="00586-266">String</span></span>|<span data-ttu-id="00586-267">电子邮件 () 设备关联的用户的邮箱。</span><span class="sxs-lookup"><span data-stu-id="00586-267">Email(s) for the user associated with the device.</span></span> <span data-ttu-id="00586-268">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="00586-268">This property is read-only.</span></span> <span data-ttu-id="00586-269">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="00586-269">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="00586-270">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="00586-270">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="00586-271">String</span><span class="sxs-lookup"><span data-stu-id="00586-271">String</span></span>|<span data-ttu-id="00586-272">Azure Active Directory 设备的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="00586-272">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="00586-273">只读。</span><span class="sxs-lookup"><span data-stu-id="00586-273">Read only.</span></span> <span data-ttu-id="00586-274">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="00586-274">This property is read-only.</span></span> <span data-ttu-id="00586-275">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="00586-275">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="00586-276">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="00586-276">azureADDeviceId</span></span>|<span data-ttu-id="00586-277">String</span><span class="sxs-lookup"><span data-stu-id="00586-277">String</span></span>|<span data-ttu-id="00586-278">Azure Active Directory 设备的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="00586-278">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="00586-279">只读。</span><span class="sxs-lookup"><span data-stu-id="00586-279">Read only.</span></span> <span data-ttu-id="00586-280">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="00586-280">This property is read-only.</span></span> <span data-ttu-id="00586-281">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="00586-281">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="00586-282">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="00586-282">deviceRegistrationState</span></span>|[<span data-ttu-id="00586-283">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="00586-283">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="00586-284">设备注册状态。</span><span class="sxs-lookup"><span data-stu-id="00586-284">Device registration state.</span></span> <span data-ttu-id="00586-285">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="00586-285">This property is read-only.</span></span> <span data-ttu-id="00586-286">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="00586-286">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="00586-287">可取值为：`notRegistered`、`registered`、`revoked`、`keyConflict`、`approvalPending`、`certificateReset`、`notRegisteredPendingEnrollment`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="00586-287">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="00586-288">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="00586-288">deviceCategoryDisplayName</span></span>|<span data-ttu-id="00586-289">String</span><span class="sxs-lookup"><span data-stu-id="00586-289">String</span></span>|<span data-ttu-id="00586-290">设备类别显示名称。</span><span class="sxs-lookup"><span data-stu-id="00586-290">Device category display name.</span></span> <span data-ttu-id="00586-291">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="00586-291">This property is read-only.</span></span> <span data-ttu-id="00586-292">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="00586-292">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="00586-293">isSupervised</span><span class="sxs-lookup"><span data-stu-id="00586-293">isSupervised</span></span>|<span data-ttu-id="00586-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="00586-294">Boolean</span></span>|<span data-ttu-id="00586-295">设备监督状态。</span><span class="sxs-lookup"><span data-stu-id="00586-295">Device supervised status.</span></span> <span data-ttu-id="00586-296">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="00586-296">This property is read-only.</span></span> <span data-ttu-id="00586-297">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="00586-297">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="00586-298">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="00586-298">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="00586-299">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00586-299">DateTimeOffset</span></span>|<span data-ttu-id="00586-300">设备上次与 Exchange 联系的时间。</span><span class="sxs-lookup"><span data-stu-id="00586-300">Last time the device contacted Exchange.</span></span> <span data-ttu-id="00586-301">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="00586-301">This property is read-only.</span></span> <span data-ttu-id="00586-302">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="00586-302">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="00586-303">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="00586-303">exchangeAccessState</span></span>|[<span data-ttu-id="00586-304">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="00586-304">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="00586-305">Exchange 中设备的访问状态。</span><span class="sxs-lookup"><span data-stu-id="00586-305">The Access State of the device in Exchange.</span></span> <span data-ttu-id="00586-306">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="00586-306">This property is read-only.</span></span> <span data-ttu-id="00586-307">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="00586-307">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="00586-308">可取值为：`none`、`unknown`、`allowed`、`blocked`、`quarantined`。</span><span class="sxs-lookup"><span data-stu-id="00586-308">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="00586-309">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="00586-309">exchangeAccessStateReason</span></span>|[<span data-ttu-id="00586-310">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="00586-310">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="00586-311">Exchange 中设备访问状态的出现原因。</span><span class="sxs-lookup"><span data-stu-id="00586-311">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="00586-312">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="00586-312">This property is read-only.</span></span> <span data-ttu-id="00586-313">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="00586-313">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="00586-314">可取值为：`none`、`unknown`、`exchangeGlobalRule`、`exchangeIndividualRule`、`exchangeDeviceRule`、`exchangeUpgrade`、`exchangeMailboxPolicy`、`other`、`compliant`、`notCompliant`、`notEnrolled`、`unknownLocation`、`mfaRequired`、`azureADBlockDueToAccessPolicy`、`compromisedPassword`、`deviceNotKnownWithManagedApp`。</span><span class="sxs-lookup"><span data-stu-id="00586-314">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="00586-315">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="00586-315">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="00586-316">String</span><span class="sxs-lookup"><span data-stu-id="00586-316">String</span></span>|<span data-ttu-id="00586-317">允许与设备建立远程协助会话的 URL。</span><span class="sxs-lookup"><span data-stu-id="00586-317">Url that allows a Remote Assistance session to be established with the device.</span></span> <span data-ttu-id="00586-318">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="00586-318">This property is read-only.</span></span> <span data-ttu-id="00586-319">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="00586-319">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="00586-320">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="00586-320">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="00586-321">String</span><span class="sxs-lookup"><span data-stu-id="00586-321">String</span></span>|<span data-ttu-id="00586-322">用于在创建远程协助会话对象时识别问题的错误字符串。</span><span class="sxs-lookup"><span data-stu-id="00586-322">An error string that identifies issues when creating Remote Assistance session objects.</span></span> <span data-ttu-id="00586-323">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="00586-323">This property is read-only.</span></span> <span data-ttu-id="00586-324">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="00586-324">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="00586-325">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="00586-325">isEncrypted</span></span>|<span data-ttu-id="00586-326">Boolean</span><span class="sxs-lookup"><span data-stu-id="00586-326">Boolean</span></span>|<span data-ttu-id="00586-327">设备加密状态。</span><span class="sxs-lookup"><span data-stu-id="00586-327">Device encryption status.</span></span> <span data-ttu-id="00586-328">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="00586-328">This property is read-only.</span></span> <span data-ttu-id="00586-329">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="00586-329">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="00586-330">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="00586-330">userPrincipalName</span></span>|<span data-ttu-id="00586-331">String</span><span class="sxs-lookup"><span data-stu-id="00586-331">String</span></span>|<span data-ttu-id="00586-332">设备用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="00586-332">Device user principal name.</span></span> <span data-ttu-id="00586-333">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="00586-333">This property is read-only.</span></span> <span data-ttu-id="00586-334">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="00586-334">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="00586-335">model</span><span class="sxs-lookup"><span data-stu-id="00586-335">model</span></span>|<span data-ttu-id="00586-336">String</span><span class="sxs-lookup"><span data-stu-id="00586-336">String</span></span>|<span data-ttu-id="00586-337">设备型号。</span><span class="sxs-lookup"><span data-stu-id="00586-337">Model of the device.</span></span> <span data-ttu-id="00586-338">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="00586-338">This property is read-only.</span></span> <span data-ttu-id="00586-339">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="00586-339">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="00586-340">manufacturer</span><span class="sxs-lookup"><span data-stu-id="00586-340">manufacturer</span></span>|<span data-ttu-id="00586-341">String</span><span class="sxs-lookup"><span data-stu-id="00586-341">String</span></span>|<span data-ttu-id="00586-342">设备的制造商。</span><span class="sxs-lookup"><span data-stu-id="00586-342">Manufacturer of the device.</span></span> <span data-ttu-id="00586-343">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="00586-343">This property is read-only.</span></span> <span data-ttu-id="00586-344">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="00586-344">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="00586-345">imei</span><span class="sxs-lookup"><span data-stu-id="00586-345">imei</span></span>|<span data-ttu-id="00586-346">String</span><span class="sxs-lookup"><span data-stu-id="00586-346">String</span></span>|<span data-ttu-id="00586-347">IMEI。</span><span class="sxs-lookup"><span data-stu-id="00586-347">IMEI.</span></span> <span data-ttu-id="00586-348">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="00586-348">This property is read-only.</span></span> <span data-ttu-id="00586-349">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="00586-349">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="00586-350">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="00586-350">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="00586-351">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00586-351">DateTimeOffset</span></span>|<span data-ttu-id="00586-352">设备合规性宽限期到期的 DateTime。</span><span class="sxs-lookup"><span data-stu-id="00586-352">The DateTime when device compliance grace period expires.</span></span> <span data-ttu-id="00586-353">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="00586-353">This property is read-only.</span></span> <span data-ttu-id="00586-354">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="00586-354">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="00586-355">serialNumber</span><span class="sxs-lookup"><span data-stu-id="00586-355">serialNumber</span></span>|<span data-ttu-id="00586-356">String</span><span class="sxs-lookup"><span data-stu-id="00586-356">String</span></span>|<span data-ttu-id="00586-357">SerialNumber。</span><span class="sxs-lookup"><span data-stu-id="00586-357">SerialNumber.</span></span> <span data-ttu-id="00586-358">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="00586-358">This property is read-only.</span></span> <span data-ttu-id="00586-359">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="00586-359">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="00586-360">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="00586-360">phoneNumber</span></span>|<span data-ttu-id="00586-361">String</span><span class="sxs-lookup"><span data-stu-id="00586-361">String</span></span>|<span data-ttu-id="00586-362">设备的电话号码。</span><span class="sxs-lookup"><span data-stu-id="00586-362">Phone number of the device.</span></span> <span data-ttu-id="00586-363">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="00586-363">This property is read-only.</span></span> <span data-ttu-id="00586-364">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="00586-364">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="00586-365">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="00586-365">androidSecurityPatchLevel</span></span>|<span data-ttu-id="00586-366">String</span><span class="sxs-lookup"><span data-stu-id="00586-366">String</span></span>|<span data-ttu-id="00586-367">Android 安全修补程序级别。</span><span class="sxs-lookup"><span data-stu-id="00586-367">Android security patch level.</span></span> <span data-ttu-id="00586-368">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="00586-368">This property is read-only.</span></span> <span data-ttu-id="00586-369">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="00586-369">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="00586-370">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="00586-370">userDisplayName</span></span>|<span data-ttu-id="00586-371">String</span><span class="sxs-lookup"><span data-stu-id="00586-371">String</span></span>|<span data-ttu-id="00586-372">用户显示名称。</span><span class="sxs-lookup"><span data-stu-id="00586-372">User display name.</span></span> <span data-ttu-id="00586-373">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="00586-373">This property is read-only.</span></span> <span data-ttu-id="00586-374">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="00586-374">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="00586-375">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="00586-375">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="00586-376">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="00586-376">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="00586-377">ConfigrMgr 客户端启用的功能。</span><span class="sxs-lookup"><span data-stu-id="00586-377">ConfigrMgr client enabled features.</span></span> <span data-ttu-id="00586-378">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="00586-378">This property is read-only.</span></span> <span data-ttu-id="00586-379">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="00586-379">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="00586-380">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="00586-380">wiFiMacAddress</span></span>|<span data-ttu-id="00586-381">String</span><span class="sxs-lookup"><span data-stu-id="00586-381">String</span></span>|<span data-ttu-id="00586-382">Wi-Fi MAC。</span><span class="sxs-lookup"><span data-stu-id="00586-382">Wi-Fi MAC.</span></span> <span data-ttu-id="00586-383">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="00586-383">This property is read-only.</span></span> <span data-ttu-id="00586-384">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="00586-384">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="00586-385">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="00586-385">deviceHealthAttestationState</span></span>|[<span data-ttu-id="00586-386">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="00586-386">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="00586-387">设备运行状况证明状态。</span><span class="sxs-lookup"><span data-stu-id="00586-387">The device health attestation state.</span></span> <span data-ttu-id="00586-388">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="00586-388">This property is read-only.</span></span> <span data-ttu-id="00586-389">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="00586-389">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="00586-390">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="00586-390">subscriberCarrier</span></span>|<span data-ttu-id="00586-391">String</span><span class="sxs-lookup"><span data-stu-id="00586-391">String</span></span>|<span data-ttu-id="00586-392">订阅者运营商。</span><span class="sxs-lookup"><span data-stu-id="00586-392">Subscriber Carrier.</span></span> <span data-ttu-id="00586-393">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="00586-393">This property is read-only.</span></span> <span data-ttu-id="00586-394">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="00586-394">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="00586-395">meid</span><span class="sxs-lookup"><span data-stu-id="00586-395">meid</span></span>|<span data-ttu-id="00586-396">String</span><span class="sxs-lookup"><span data-stu-id="00586-396">String</span></span>|<span data-ttu-id="00586-397">MEID。</span><span class="sxs-lookup"><span data-stu-id="00586-397">MEID.</span></span> <span data-ttu-id="00586-398">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="00586-398">This property is read-only.</span></span> <span data-ttu-id="00586-399">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="00586-399">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="00586-400">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="00586-400">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="00586-401">Int64</span><span class="sxs-lookup"><span data-stu-id="00586-401">Int64</span></span>|<span data-ttu-id="00586-402">总存储（以字节为单位）。</span><span class="sxs-lookup"><span data-stu-id="00586-402">Total Storage in Bytes.</span></span> <span data-ttu-id="00586-403">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="00586-403">This property is read-only.</span></span> <span data-ttu-id="00586-404">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="00586-404">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="00586-405">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="00586-405">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="00586-406">Int64</span><span class="sxs-lookup"><span data-stu-id="00586-406">Int64</span></span>|<span data-ttu-id="00586-407">可用存储空间（以字节为单位）。</span><span class="sxs-lookup"><span data-stu-id="00586-407">Free Storage in Bytes.</span></span> <span data-ttu-id="00586-408">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="00586-408">This property is read-only.</span></span> <span data-ttu-id="00586-409">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="00586-409">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="00586-410">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="00586-410">managedDeviceName</span></span>|<span data-ttu-id="00586-411">String</span><span class="sxs-lookup"><span data-stu-id="00586-411">String</span></span>|<span data-ttu-id="00586-412">用于识别设备的自动生成的名称。</span><span class="sxs-lookup"><span data-stu-id="00586-412">Automatically generated name to identify a device.</span></span> <span data-ttu-id="00586-413">可以覆盖为用户友好名称。</span><span class="sxs-lookup"><span data-stu-id="00586-413">Can be overwritten to a user friendly name.</span></span> <span data-ttu-id="00586-414">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="00586-414">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="00586-415">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="00586-415">partnerReportedThreatState</span></span>|[<span data-ttu-id="00586-416">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="00586-416">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="00586-417">指示帐户和设备正在使用移动威胁防护合作伙伴时设备的威胁状态。</span><span class="sxs-lookup"><span data-stu-id="00586-417">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="00586-418">只读。</span><span class="sxs-lookup"><span data-stu-id="00586-418">Read Only.</span></span> <span data-ttu-id="00586-419">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="00586-419">This property is read-only.</span></span> <span data-ttu-id="00586-420">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="00586-420">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="00586-421">可取值为：`unknown`、`activated`、`deactivated`、`secured`、`lowSeverity`、`mediumSeverity`、`highSeverity`、`unresponsive`、`compromised`、`misconfigured`。</span><span class="sxs-lookup"><span data-stu-id="00586-421">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="00586-422">retireAfterDateTime</span><span class="sxs-lookup"><span data-stu-id="00586-422">retireAfterDateTime</span></span>|<span data-ttu-id="00586-423">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00586-423">DateTimeOffset</span></span>|<span data-ttu-id="00586-424">指示设备因计划操作而自动停用的时间。</span><span class="sxs-lookup"><span data-stu-id="00586-424">Indicates the time after when a device will be auto retired because of scheduled action.</span></span> <span data-ttu-id="00586-425">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="00586-425">This property is read-only.</span></span> <span data-ttu-id="00586-426">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="00586-426">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="00586-427">usersLoggedOn</span><span class="sxs-lookup"><span data-stu-id="00586-427">usersLoggedOn</span></span>|<span data-ttu-id="00586-428">[loggedOnUser](../resources/intune-devices-loggedonuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="00586-428">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="00586-429">指示设备上最后一次登录的用户。</span><span class="sxs-lookup"><span data-stu-id="00586-429">Indicates the last logged on users of a device.</span></span> <span data-ttu-id="00586-430">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="00586-430">This property is read-only.</span></span> <span data-ttu-id="00586-431">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="00586-431">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="00586-432">preferMdmOverGroupPolicyAppliedDateTime</span><span class="sxs-lookup"><span data-stu-id="00586-432">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="00586-433">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00586-433">DateTimeOffset</span></span>|<span data-ttu-id="00586-434">报告 DateTime 设置了 preferMdmOverGroupPolicy 设置。</span><span class="sxs-lookup"><span data-stu-id="00586-434">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="00586-435">设置后，如果存在冲突，Intune MDM 设置将覆盖组策略设置。</span><span class="sxs-lookup"><span data-stu-id="00586-435">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="00586-436">只读。</span><span class="sxs-lookup"><span data-stu-id="00586-436">Read Only.</span></span> <span data-ttu-id="00586-437">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="00586-437">This property is read-only.</span></span> <span data-ttu-id="00586-438">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="00586-438">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="00586-439">autopilotEnrolled</span><span class="sxs-lookup"><span data-stu-id="00586-439">autopilotEnrolled</span></span>|<span data-ttu-id="00586-440">Boolean</span><span class="sxs-lookup"><span data-stu-id="00586-440">Boolean</span></span>|<span data-ttu-id="00586-441">报告托管设备是否通过自动试点注册。</span><span class="sxs-lookup"><span data-stu-id="00586-441">Reports if the managed device is enrolled via auto-pilot.</span></span> <span data-ttu-id="00586-442">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="00586-442">This property is read-only.</span></span> <span data-ttu-id="00586-443">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="00586-443">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="00586-444">requireUserEnrollmentApproval</span><span class="sxs-lookup"><span data-stu-id="00586-444">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="00586-445">Boolean</span><span class="sxs-lookup"><span data-stu-id="00586-445">Boolean</span></span>|<span data-ttu-id="00586-446">报告托管 iOS 设备是否注册用户审批。</span><span class="sxs-lookup"><span data-stu-id="00586-446">Reports if the managed iOS device is user approval enrollment.</span></span> <span data-ttu-id="00586-447">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="00586-447">This property is read-only.</span></span> <span data-ttu-id="00586-448">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="00586-448">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="00586-449">managementCertificateExpirationDate</span><span class="sxs-lookup"><span data-stu-id="00586-449">managementCertificateExpirationDate</span></span>|<span data-ttu-id="00586-450">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00586-450">DateTimeOffset</span></span>|<span data-ttu-id="00586-451">报告设备管理证书到期日期。</span><span class="sxs-lookup"><span data-stu-id="00586-451">Reports device management certificate expiration date.</span></span> <span data-ttu-id="00586-452">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="00586-452">This property is read-only.</span></span> <span data-ttu-id="00586-453">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="00586-453">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="00586-454">iccid</span><span class="sxs-lookup"><span data-stu-id="00586-454">iccid</span></span>|<span data-ttu-id="00586-455">String</span><span class="sxs-lookup"><span data-stu-id="00586-455">String</span></span>|<span data-ttu-id="00586-456">集成的电路卡标识符，它是 SIM 卡的唯一标识号。</span><span class="sxs-lookup"><span data-stu-id="00586-456">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span> <span data-ttu-id="00586-457">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="00586-457">This property is read-only.</span></span> <span data-ttu-id="00586-458">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="00586-458">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="00586-459">udid</span><span class="sxs-lookup"><span data-stu-id="00586-459">udid</span></span>|<span data-ttu-id="00586-460">String</span><span class="sxs-lookup"><span data-stu-id="00586-460">String</span></span>|<span data-ttu-id="00586-461">iOS 和 macOS 设备的唯一设备标识符。</span><span class="sxs-lookup"><span data-stu-id="00586-461">Unique Device Identifier for iOS and macOS devices.</span></span> <span data-ttu-id="00586-462">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="00586-462">This property is read-only.</span></span> <span data-ttu-id="00586-463">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="00586-463">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="00586-464">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="00586-464">roleScopeTagIds</span></span>|<span data-ttu-id="00586-465">String 集合</span><span class="sxs-lookup"><span data-stu-id="00586-465">String collection</span></span>|<span data-ttu-id="00586-466">此设备实例的范围标记标识列表。</span><span class="sxs-lookup"><span data-stu-id="00586-466">List of Scope Tag IDs for this Device instance.</span></span> <span data-ttu-id="00586-467">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="00586-467">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="00586-468">windowsActiveMalwareCount</span><span class="sxs-lookup"><span data-stu-id="00586-468">windowsActiveMalwareCount</span></span>|<span data-ttu-id="00586-469">Int32</span><span class="sxs-lookup"><span data-stu-id="00586-469">Int32</span></span>|<span data-ttu-id="00586-470">此 Windows 设备的活动恶意软件计数。</span><span class="sxs-lookup"><span data-stu-id="00586-470">Count of active malware for this windows device.</span></span> <span data-ttu-id="00586-471">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="00586-471">This property is read-only.</span></span> <span data-ttu-id="00586-472">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="00586-472">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="00586-473">windowsRemediatedMalwareCount</span><span class="sxs-lookup"><span data-stu-id="00586-473">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="00586-474">Int32</span><span class="sxs-lookup"><span data-stu-id="00586-474">Int32</span></span>|<span data-ttu-id="00586-475">此 Windows 设备的已修复恶意软件计数。</span><span class="sxs-lookup"><span data-stu-id="00586-475">Count of remediated malware for this windows device.</span></span> <span data-ttu-id="00586-476">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="00586-476">This property is read-only.</span></span> <span data-ttu-id="00586-477">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="00586-477">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="00586-478">notes</span><span class="sxs-lookup"><span data-stu-id="00586-478">notes</span></span>|<span data-ttu-id="00586-479">String</span><span class="sxs-lookup"><span data-stu-id="00586-479">String</span></span>|<span data-ttu-id="00586-480">由 IT 管理员创建的设备的备注 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="00586-480">Notes on the device created by IT Admin Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="00586-481">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="00586-481">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="00586-482">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="00586-482">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="00586-483">配置管理器客户端运行状况状态，仅对 MDM/ConfigMgr 代理管理的设备有效。继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="00586-483">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="00586-484">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="00586-484">configurationManagerClientInformation</span></span>|[<span data-ttu-id="00586-485">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="00586-485">configurationManagerClientInformation</span></span>](../resources/intune-devices-configurationmanagerclientinformation.md)|<span data-ttu-id="00586-486">配置管理器客户端信息，仅对由 ConfigMgr 代理托管、duel 托管或三管理的设备有效。继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="00586-486">Configuration manager client information, valid only for devices managed, duel-managed or tri-managed by ConfigMgr Agent Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="00586-487">ethernetMacAddress</span><span class="sxs-lookup"><span data-stu-id="00586-487">ethernetMacAddress</span></span>|<span data-ttu-id="00586-488">String</span><span class="sxs-lookup"><span data-stu-id="00586-488">String</span></span>|<span data-ttu-id="00586-489">以太网 MAC。</span><span class="sxs-lookup"><span data-stu-id="00586-489">Ethernet MAC.</span></span> <span data-ttu-id="00586-490">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="00586-490">This property is read-only.</span></span> <span data-ttu-id="00586-491">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="00586-491">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="00586-492">physicalMemoryInBytes</span><span class="sxs-lookup"><span data-stu-id="00586-492">physicalMemoryInBytes</span></span>|<span data-ttu-id="00586-493">Int64</span><span class="sxs-lookup"><span data-stu-id="00586-493">Int64</span></span>|<span data-ttu-id="00586-494">内存总量（以字节为单位）。</span><span class="sxs-lookup"><span data-stu-id="00586-494">Total Memory in Bytes.</span></span> <span data-ttu-id="00586-495">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="00586-495">This property is read-only.</span></span> <span data-ttu-id="00586-496">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="00586-496">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="00586-497">processorArchitecture</span><span class="sxs-lookup"><span data-stu-id="00586-497">processorArchitecture</span></span>|[<span data-ttu-id="00586-498">managedDeviceArchitecture</span><span class="sxs-lookup"><span data-stu-id="00586-498">managedDeviceArchitecture</span></span>](../resources/intune-devices-manageddevicearchitecture.md)|<span data-ttu-id="00586-499">处理器体系结构。</span><span class="sxs-lookup"><span data-stu-id="00586-499">Processor architecture.</span></span> <span data-ttu-id="00586-500">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="00586-500">This property is read-only.</span></span> <span data-ttu-id="00586-501">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="00586-501">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="00586-502">可取值为：`unknown`、`x86`、`x64`、`arm`、`arM64`。</span><span class="sxs-lookup"><span data-stu-id="00586-502">Possible values are: `unknown`, `x86`, `x64`, `arm`, `arM64`.</span></span>|
|<span data-ttu-id="00586-503">specificationVersion</span><span class="sxs-lookup"><span data-stu-id="00586-503">specificationVersion</span></span>|<span data-ttu-id="00586-504">String</span><span class="sxs-lookup"><span data-stu-id="00586-504">String</span></span>|<span data-ttu-id="00586-505">规范版本。</span><span class="sxs-lookup"><span data-stu-id="00586-505">Specification version.</span></span> <span data-ttu-id="00586-506">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="00586-506">This property is read-only.</span></span> <span data-ttu-id="00586-507">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="00586-507">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="00586-508">joinType</span><span class="sxs-lookup"><span data-stu-id="00586-508">joinType</span></span>|[<span data-ttu-id="00586-509">joinType</span><span class="sxs-lookup"><span data-stu-id="00586-509">joinType</span></span>](../resources/intune-devices-jointype.md)|<span data-ttu-id="00586-510">设备加入类型 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="00586-510">Device join type Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="00586-511">可取值为：`unknown`、`azureADJoined`、`azureADRegistered`、`hybridAzureADJoined`。</span><span class="sxs-lookup"><span data-stu-id="00586-511">Possible values are: `unknown`, `azureADJoined`, `azureADRegistered`, `hybridAzureADJoined`.</span></span>|
|<span data-ttu-id="00586-512">skuFamily</span><span class="sxs-lookup"><span data-stu-id="00586-512">skuFamily</span></span>|<span data-ttu-id="00586-513">String</span><span class="sxs-lookup"><span data-stu-id="00586-513">String</span></span>|<span data-ttu-id="00586-514">设备 sku 系列 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="00586-514">Device sku family Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="00586-515">skuNumber</span><span class="sxs-lookup"><span data-stu-id="00586-515">skuNumber</span></span>|<span data-ttu-id="00586-516">Int32</span><span class="sxs-lookup"><span data-stu-id="00586-516">Int32</span></span>|<span data-ttu-id="00586-517">设备 sku 号，另请参阅 https://docs.microsoft.com/windows/win32/api/sysinfoapi/nf-sysinfoapi-getproductinfo ：。</span><span class="sxs-lookup"><span data-stu-id="00586-517">Device sku number, see also: https://docs.microsoft.com/windows/win32/api/sysinfoapi/nf-sysinfoapi-getproductinfo.</span></span> <span data-ttu-id="00586-518">有效值为 0 到 2147483647。</span><span class="sxs-lookup"><span data-stu-id="00586-518">Valid values 0 to 2147483647.</span></span> <span data-ttu-id="00586-519">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="00586-519">This property is read-only.</span></span> <span data-ttu-id="00586-520">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="00586-520">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="00586-521">managementFeatures</span><span class="sxs-lookup"><span data-stu-id="00586-521">managementFeatures</span></span>|[<span data-ttu-id="00586-522">managedDeviceManagementFeatures</span><span class="sxs-lookup"><span data-stu-id="00586-522">managedDeviceManagementFeatures</span></span>](../resources/intune-devices-manageddevicemanagementfeatures.md)|<span data-ttu-id="00586-523">设备管理功能 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="00586-523">Device management features Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="00586-524">可取值为：`none`、`microsoftManagedDesktop`。</span><span class="sxs-lookup"><span data-stu-id="00586-524">Possible values are: `none`, `microsoftManagedDesktop`.</span></span>|



## <a name="response"></a><span data-ttu-id="00586-525">响应</span><span class="sxs-lookup"><span data-stu-id="00586-525">Response</span></span>
<span data-ttu-id="00586-526">如果成功，此方法在响应正文中返回 响应代码和更新 `200 OK` 的 [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="00586-526">If successful, this method returns a `200 OK` response code and an updated [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00586-527">示例</span><span class="sxs-lookup"><span data-stu-id="00586-527">Example</span></span>

### <a name="request"></a><span data-ttu-id="00586-528">请求</span><span class="sxs-lookup"><span data-stu-id="00586-528">Request</span></span>
<span data-ttu-id="00586-529">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="00586-529">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}
Content-type: application/json
Content-length: 8564

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
  "managementFeatures": "microsoftManagedDesktop"
}
```

### <a name="response"></a><span data-ttu-id="00586-530">响应</span><span class="sxs-lookup"><span data-stu-id="00586-530">Response</span></span>
<span data-ttu-id="00586-p175">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="00586-p175">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 8613

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
  "managementFeatures": "microsoftManagedDesktop"
}
```




