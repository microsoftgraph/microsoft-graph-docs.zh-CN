---
title: 更新 windowsManagedDevice
description: 更新 windowsManagedDevice 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 70bb270f578f26a14e90882f73b6db61604b875a
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158812"
---
# <a name="update-windowsmanageddevice"></a><span data-ttu-id="c463e-103">更新 windowsManagedDevice</span><span class="sxs-lookup"><span data-stu-id="c463e-103">Update windowsManagedDevice</span></span>

<span data-ttu-id="c463e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c463e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c463e-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c463e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c463e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c463e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c463e-107">更新 [windowsManagedDevice 对象](../resources/intune-devices-windowsmanageddevice.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="c463e-107">Update the properties of a [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c463e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="c463e-108">Prerequisites</span></span>
<span data-ttu-id="c463e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c463e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c463e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c463e-111">Permission type</span></span>|<span data-ttu-id="c463e-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c463e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c463e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c463e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c463e-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c463e-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="c463e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c463e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c463e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c463e-116">Not supported.</span></span>|
|<span data-ttu-id="c463e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c463e-117">Application</span></span>|<span data-ttu-id="c463e-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c463e-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c463e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c463e-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="c463e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c463e-120">Request headers</span></span>
|<span data-ttu-id="c463e-121">标头</span><span class="sxs-lookup"><span data-stu-id="c463e-121">Header</span></span>|<span data-ttu-id="c463e-122">值</span><span class="sxs-lookup"><span data-stu-id="c463e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c463e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c463e-123">Authorization</span></span>|<span data-ttu-id="c463e-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c463e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c463e-125">接受</span><span class="sxs-lookup"><span data-stu-id="c463e-125">Accept</span></span>|<span data-ttu-id="c463e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c463e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c463e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c463e-127">Request body</span></span>
<span data-ttu-id="c463e-128">在请求正文中，提供 [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c463e-128">In the request body, supply a JSON representation for the [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object.</span></span>

<span data-ttu-id="c463e-129">下表显示创建 [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c463e-129">The following table shows the properties that are required when you create the [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md).</span></span>

|<span data-ttu-id="c463e-130">属性</span><span class="sxs-lookup"><span data-stu-id="c463e-130">Property</span></span>|<span data-ttu-id="c463e-131">类型</span><span class="sxs-lookup"><span data-stu-id="c463e-131">Type</span></span>|<span data-ttu-id="c463e-132">说明</span><span class="sxs-lookup"><span data-stu-id="c463e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c463e-133">id</span><span class="sxs-lookup"><span data-stu-id="c463e-133">id</span></span>|<span data-ttu-id="c463e-134">String</span><span class="sxs-lookup"><span data-stu-id="c463e-134">String</span></span>|<span data-ttu-id="c463e-135">设备的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="c463e-135">Unique Identifier for the device.</span></span> <span data-ttu-id="c463e-136">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c463e-136">This property is read-only.</span></span> <span data-ttu-id="c463e-137">继承自 [managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c463e-137">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="c463e-138">userId</span><span class="sxs-lookup"><span data-stu-id="c463e-138">userId</span></span>|<span data-ttu-id="c463e-139">String</span><span class="sxs-lookup"><span data-stu-id="c463e-139">String</span></span>|<span data-ttu-id="c463e-140">与设备关联的用户的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="c463e-140">Unique Identifier for the user associated with the device.</span></span> <span data-ttu-id="c463e-141">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c463e-141">This property is read-only.</span></span> <span data-ttu-id="c463e-142">继承自 [managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c463e-142">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="c463e-143">deviceName</span><span class="sxs-lookup"><span data-stu-id="c463e-143">deviceName</span></span>|<span data-ttu-id="c463e-144">String</span><span class="sxs-lookup"><span data-stu-id="c463e-144">String</span></span>|<span data-ttu-id="c463e-145">设备的名称。</span><span class="sxs-lookup"><span data-stu-id="c463e-145">Name of the device.</span></span> <span data-ttu-id="c463e-146">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c463e-146">This property is read-only.</span></span> <span data-ttu-id="c463e-147">继承自 [managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c463e-147">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="c463e-148">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="c463e-148">hardwareInformation</span></span>|[<span data-ttu-id="c463e-149">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="c463e-149">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="c463e-150">设备的硬性详细信息。</span><span class="sxs-lookup"><span data-stu-id="c463e-150">The hardward details for the device.</span></span>  <span data-ttu-id="c463e-151">包括存储空间、制造商、序列号等信息。此属性为只读。</span><span class="sxs-lookup"><span data-stu-id="c463e-151">Includes information such as storage space, manufacturer, serial number, etc. This property is read-only.</span></span> <span data-ttu-id="c463e-152">继承自 [managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c463e-152">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="c463e-153">ownerType</span><span class="sxs-lookup"><span data-stu-id="c463e-153">ownerType</span></span>|[<span data-ttu-id="c463e-154">ownerType</span><span class="sxs-lookup"><span data-stu-id="c463e-154">ownerType</span></span>](../resources/intune-shared-ownertype.md)|<span data-ttu-id="c463e-155">设备的所有权。</span><span class="sxs-lookup"><span data-stu-id="c463e-155">Ownership of the device.</span></span> <span data-ttu-id="c463e-156">可以是"company"或"personal"继承自 [managedDevice](../resources/intune-shared-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="c463e-156">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-shared-manageddevice.md).</span></span> <span data-ttu-id="c463e-157">可取值为：`unknown`、`company`、`personal`。</span><span class="sxs-lookup"><span data-stu-id="c463e-157">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="c463e-158">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="c463e-158">managedDeviceOwnerType</span></span>|[<span data-ttu-id="c463e-159">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="c463e-159">managedDeviceOwnerType</span></span>](../resources/intune-shared-manageddeviceownertype.md)|<span data-ttu-id="c463e-160">设备的所有权。</span><span class="sxs-lookup"><span data-stu-id="c463e-160">Ownership of the device.</span></span> <span data-ttu-id="c463e-161">可以是"company"或"personal"继承自 [managedDevice](../resources/intune-shared-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="c463e-161">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-shared-manageddevice.md).</span></span> <span data-ttu-id="c463e-162">可取值为：`unknown`、`company`、`personal`。</span><span class="sxs-lookup"><span data-stu-id="c463e-162">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="c463e-163">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="c463e-163">deviceActionResults</span></span>|<span data-ttu-id="c463e-164">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c463e-164">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="c463e-165">ComplexType deviceActionResult 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="c463e-165">List of ComplexType deviceActionResult objects.</span></span> <span data-ttu-id="c463e-166">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c463e-166">This property is read-only.</span></span> <span data-ttu-id="c463e-167">继承自 [managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c463e-167">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="c463e-168">managementState</span><span class="sxs-lookup"><span data-stu-id="c463e-168">managementState</span></span>|[<span data-ttu-id="c463e-169">managementState</span><span class="sxs-lookup"><span data-stu-id="c463e-169">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="c463e-170">设备的管理状态。</span><span class="sxs-lookup"><span data-stu-id="c463e-170">Management state of the device.</span></span> <span data-ttu-id="c463e-171">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c463e-171">This property is read-only.</span></span> <span data-ttu-id="c463e-172">继承自 [managedDevice](../resources/intune-shared-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="c463e-172">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md).</span></span> <span data-ttu-id="c463e-173">可取值为：`managed`、`retirePending`、`retireFailed`、`wipePending`、`wipeFailed`、`unhealthy`、`deletePending`、`retireIssued`、`wipeIssued`、`wipeCanceled`、`retireCanceled`、`discovered`。</span><span class="sxs-lookup"><span data-stu-id="c463e-173">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="c463e-174">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="c463e-174">enrolledDateTime</span></span>|<span data-ttu-id="c463e-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c463e-175">DateTimeOffset</span></span>|<span data-ttu-id="c463e-176">设备的注册时间。</span><span class="sxs-lookup"><span data-stu-id="c463e-176">Enrollment time of the device.</span></span> <span data-ttu-id="c463e-177">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c463e-177">This property is read-only.</span></span> <span data-ttu-id="c463e-178">继承自 [managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c463e-178">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="c463e-179">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="c463e-179">lastSyncDateTime</span></span>|<span data-ttu-id="c463e-180">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c463e-180">DateTimeOffset</span></span>|<span data-ttu-id="c463e-181">设备上次成功完成与 Intune 同步的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="c463e-181">The date and time that the device last completed a successful sync with Intune.</span></span> <span data-ttu-id="c463e-182">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c463e-182">This property is read-only.</span></span> <span data-ttu-id="c463e-183">继承自 [managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c463e-183">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="c463e-184">chassisType</span><span class="sxs-lookup"><span data-stu-id="c463e-184">chassisType</span></span>|[<span data-ttu-id="c463e-185">chassisType</span><span class="sxs-lookup"><span data-stu-id="c463e-185">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="c463e-186">设备的机架类型。</span><span class="sxs-lookup"><span data-stu-id="c463e-186">Chassis type of the device.</span></span> <span data-ttu-id="c463e-187">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c463e-187">This property is read-only.</span></span> <span data-ttu-id="c463e-188">继承自 [managedDevice](../resources/intune-shared-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="c463e-188">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md).</span></span> <span data-ttu-id="c463e-189">可取值为：`unknown`、`desktop`、`laptop`、`worksWorkstation`、`enterpriseServer`、`phone`、`tablet`、`mobileOther`、`mobileUnknown`。</span><span class="sxs-lookup"><span data-stu-id="c463e-189">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="c463e-190">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="c463e-190">operatingSystem</span></span>|<span data-ttu-id="c463e-191">String</span><span class="sxs-lookup"><span data-stu-id="c463e-191">String</span></span>|<span data-ttu-id="c463e-192">设备的操作系统。</span><span class="sxs-lookup"><span data-stu-id="c463e-192">Operating system of the device.</span></span> <span data-ttu-id="c463e-193">Windows、iOS 等此属性为只读。</span><span class="sxs-lookup"><span data-stu-id="c463e-193">Windows, iOS, etc. This property is read-only.</span></span> <span data-ttu-id="c463e-194">继承自 [managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c463e-194">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="c463e-195">deviceType</span><span class="sxs-lookup"><span data-stu-id="c463e-195">deviceType</span></span>|[<span data-ttu-id="c463e-196">deviceType</span><span class="sxs-lookup"><span data-stu-id="c463e-196">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="c463e-197">设备平台。</span><span class="sxs-lookup"><span data-stu-id="c463e-197">Platform of the device.</span></span> <span data-ttu-id="c463e-198">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c463e-198">This property is read-only.</span></span> <span data-ttu-id="c463e-199">继承自 [managedDevice](../resources/intune-shared-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="c463e-199">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md).</span></span> <span data-ttu-id="c463e-200">可能的值是： `desktop` ， ， ， ， ， ， ， `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` ， `android` `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `windows10x` `androidnGMS` `linux` `blackberry` `palm` `unknown` `cloudPC` 。</span><span class="sxs-lookup"><span data-stu-id="c463e-200">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `androidnGMS`, `linux`, `blackberry`, `palm`, `unknown`, `cloudPC`.</span></span>|
|<span data-ttu-id="c463e-201">complianceState</span><span class="sxs-lookup"><span data-stu-id="c463e-201">complianceState</span></span>|[<span data-ttu-id="c463e-202">complianceState</span><span class="sxs-lookup"><span data-stu-id="c463e-202">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="c463e-203">设备的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="c463e-203">Compliance state of the device.</span></span> <span data-ttu-id="c463e-204">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c463e-204">This property is read-only.</span></span> <span data-ttu-id="c463e-205">继承自 [managedDevice](../resources/intune-shared-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="c463e-205">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md).</span></span> <span data-ttu-id="c463e-206">可取值为：`unknown`、`compliant`、`noncompliant`、`conflict`、`error`、`inGracePeriod`、`configManager`。</span><span class="sxs-lookup"><span data-stu-id="c463e-206">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="c463e-207">jailBroken</span><span class="sxs-lookup"><span data-stu-id="c463e-207">jailBroken</span></span>|<span data-ttu-id="c463e-208">String</span><span class="sxs-lookup"><span data-stu-id="c463e-208">String</span></span>|<span data-ttu-id="c463e-209">设备是否已越狱或取得 root 权限。</span><span class="sxs-lookup"><span data-stu-id="c463e-209">whether the device is jail broken or rooted.</span></span> <span data-ttu-id="c463e-210">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c463e-210">This property is read-only.</span></span> <span data-ttu-id="c463e-211">继承自 [managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c463e-211">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="c463e-212">managementAgent</span><span class="sxs-lookup"><span data-stu-id="c463e-212">managementAgent</span></span>|[<span data-ttu-id="c463e-213">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="c463e-213">managementAgentType</span></span>](../resources/intune-shared-managementagenttype.md)|<span data-ttu-id="c463e-214">设备的管理通道。</span><span class="sxs-lookup"><span data-stu-id="c463e-214">Management channel of the device.</span></span> <span data-ttu-id="c463e-215">Intune、EAS 等此属性为只读。</span><span class="sxs-lookup"><span data-stu-id="c463e-215">Intune, EAS, etc. This property is read-only.</span></span> <span data-ttu-id="c463e-216">继承自 [managedDevice](../resources/intune-shared-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="c463e-216">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md).</span></span> <span data-ttu-id="c463e-217">可取值为：`eas`、`mdm`、`easMdm`、`intuneClient`、`easIntuneClient`、`configurationManagerClient`、`configurationManagerClientMdm`、`configurationManagerClientMdmEas`、`unknown`、`jamf`、`googleCloudDevicePolicyController`、`microsoft365ManagedMdm`。</span><span class="sxs-lookup"><span data-stu-id="c463e-217">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span></span>|
|<span data-ttu-id="c463e-218">osVersion</span><span class="sxs-lookup"><span data-stu-id="c463e-218">osVersion</span></span>|<span data-ttu-id="c463e-219">String</span><span class="sxs-lookup"><span data-stu-id="c463e-219">String</span></span>|<span data-ttu-id="c463e-220">设备的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="c463e-220">Operating system version of the device.</span></span> <span data-ttu-id="c463e-221">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c463e-221">This property is read-only.</span></span> <span data-ttu-id="c463e-222">继承自 [managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c463e-222">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="c463e-223">easActivated</span><span class="sxs-lookup"><span data-stu-id="c463e-223">easActivated</span></span>|<span data-ttu-id="c463e-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="c463e-224">Boolean</span></span>|<span data-ttu-id="c463e-225">设备是否已激活 Exchange ActiveSync。</span><span class="sxs-lookup"><span data-stu-id="c463e-225">Whether the device is Exchange ActiveSync activated.</span></span> <span data-ttu-id="c463e-226">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c463e-226">This property is read-only.</span></span> <span data-ttu-id="c463e-227">继承自 [managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c463e-227">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="c463e-228">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="c463e-228">easDeviceId</span></span>|<span data-ttu-id="c463e-229">String</span><span class="sxs-lookup"><span data-stu-id="c463e-229">String</span></span>|<span data-ttu-id="c463e-230">设备的 Exchange ActiveSync ID。</span><span class="sxs-lookup"><span data-stu-id="c463e-230">Exchange ActiveSync Id of the device.</span></span> <span data-ttu-id="c463e-231">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c463e-231">This property is read-only.</span></span> <span data-ttu-id="c463e-232">继承自 [managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c463e-232">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="c463e-233">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="c463e-233">easActivationDateTime</span></span>|<span data-ttu-id="c463e-234">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c463e-234">DateTimeOffset</span></span>|<span data-ttu-id="c463e-235">设备的 Exchange ActivationSync 激活时间。</span><span class="sxs-lookup"><span data-stu-id="c463e-235">Exchange ActivationSync activation time of the device.</span></span> <span data-ttu-id="c463e-236">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c463e-236">This property is read-only.</span></span> <span data-ttu-id="c463e-237">继承自 [managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c463e-237">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="c463e-238">aadRegistered</span><span class="sxs-lookup"><span data-stu-id="c463e-238">aadRegistered</span></span>|<span data-ttu-id="c463e-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="c463e-239">Boolean</span></span>|<span data-ttu-id="c463e-240">设备是否已注册 Azure Active Directory。</span><span class="sxs-lookup"><span data-stu-id="c463e-240">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="c463e-241">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c463e-241">This property is read-only.</span></span> <span data-ttu-id="c463e-242">继承自 [managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c463e-242">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="c463e-243">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="c463e-243">azureADRegistered</span></span>|<span data-ttu-id="c463e-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="c463e-244">Boolean</span></span>|<span data-ttu-id="c463e-245">设备是否已注册 Azure Active Directory。</span><span class="sxs-lookup"><span data-stu-id="c463e-245">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="c463e-246">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c463e-246">This property is read-only.</span></span> <span data-ttu-id="c463e-247">继承自 [managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c463e-247">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="c463e-248">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="c463e-248">deviceEnrollmentType</span></span>|[<span data-ttu-id="c463e-249">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="c463e-249">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="c463e-250">设备的注册类型。</span><span class="sxs-lookup"><span data-stu-id="c463e-250">Enrollment type of the device.</span></span> <span data-ttu-id="c463e-251">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c463e-251">This property is read-only.</span></span> <span data-ttu-id="c463e-252">继承自 [managedDevice](../resources/intune-shared-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="c463e-252">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md).</span></span> <span data-ttu-id="c463e-253">可取值为：`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement`、`appleUserEnrollment`、`appleUserEnrollmentWithServiceAccount`、`azureAdJoinUsingAzureVmExtension`、`androidEnterpriseDedicatedDevice`、`androidEnterpriseFullyManaged`、`androidEnterpriseCorporateWorkProfile`。</span><span class="sxs-lookup"><span data-stu-id="c463e-253">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`, `azureAdJoinUsingAzureVmExtension`, `androidEnterpriseDedicatedDevice`, `androidEnterpriseFullyManaged`, `androidEnterpriseCorporateWorkProfile`.</span></span>|
|<span data-ttu-id="c463e-254">lostModeState</span><span class="sxs-lookup"><span data-stu-id="c463e-254">lostModeState</span></span>|[<span data-ttu-id="c463e-255">lostModeState</span><span class="sxs-lookup"><span data-stu-id="c463e-255">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="c463e-256">指示是否启用或禁用"丢失"模式。</span><span class="sxs-lookup"><span data-stu-id="c463e-256">Indicates if Lost mode is enabled or disabled.</span></span> <span data-ttu-id="c463e-257">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c463e-257">This property is read-only.</span></span> <span data-ttu-id="c463e-258">继承自 [managedDevice](../resources/intune-shared-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="c463e-258">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md).</span></span> <span data-ttu-id="c463e-259">可取值为：`disabled`、`enabled`。</span><span class="sxs-lookup"><span data-stu-id="c463e-259">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="c463e-260">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="c463e-260">activationLockBypassCode</span></span>|<span data-ttu-id="c463e-261">String</span><span class="sxs-lookup"><span data-stu-id="c463e-261">String</span></span>|<span data-ttu-id="c463e-262">允许绕过设备上的激活锁的代码。</span><span class="sxs-lookup"><span data-stu-id="c463e-262">Code that allows the Activation Lock on a device to be bypassed.</span></span> <span data-ttu-id="c463e-263">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c463e-263">This property is read-only.</span></span> <span data-ttu-id="c463e-264">继承自 [managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c463e-264">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="c463e-265">emailAddress</span><span class="sxs-lookup"><span data-stu-id="c463e-265">emailAddress</span></span>|<span data-ttu-id="c463e-266">String</span><span class="sxs-lookup"><span data-stu-id="c463e-266">String</span></span>|<span data-ttu-id="c463e-267">电子邮件 () 设备关联的用户的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="c463e-267">Email(s) for the user associated with the device.</span></span> <span data-ttu-id="c463e-268">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c463e-268">This property is read-only.</span></span> <span data-ttu-id="c463e-269">继承自 [managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c463e-269">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="c463e-270">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="c463e-270">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="c463e-271">String</span><span class="sxs-lookup"><span data-stu-id="c463e-271">String</span></span>|<span data-ttu-id="c463e-272">Azure Active Directory 设备的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="c463e-272">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="c463e-273">只读。</span><span class="sxs-lookup"><span data-stu-id="c463e-273">Read only.</span></span> <span data-ttu-id="c463e-274">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c463e-274">This property is read-only.</span></span> <span data-ttu-id="c463e-275">继承自 [managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c463e-275">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="c463e-276">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="c463e-276">azureADDeviceId</span></span>|<span data-ttu-id="c463e-277">String</span><span class="sxs-lookup"><span data-stu-id="c463e-277">String</span></span>|<span data-ttu-id="c463e-278">Azure Active Directory 设备的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="c463e-278">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="c463e-279">只读。</span><span class="sxs-lookup"><span data-stu-id="c463e-279">Read only.</span></span> <span data-ttu-id="c463e-280">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c463e-280">This property is read-only.</span></span> <span data-ttu-id="c463e-281">继承自 [managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c463e-281">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="c463e-282">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="c463e-282">deviceRegistrationState</span></span>|[<span data-ttu-id="c463e-283">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="c463e-283">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="c463e-284">设备注册状态。</span><span class="sxs-lookup"><span data-stu-id="c463e-284">Device registration state.</span></span> <span data-ttu-id="c463e-285">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c463e-285">This property is read-only.</span></span> <span data-ttu-id="c463e-286">继承自 [managedDevice](../resources/intune-shared-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="c463e-286">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md).</span></span> <span data-ttu-id="c463e-287">可取值为：`notRegistered`、`registered`、`revoked`、`keyConflict`、`approvalPending`、`certificateReset`、`notRegisteredPendingEnrollment`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="c463e-287">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="c463e-288">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="c463e-288">deviceCategoryDisplayName</span></span>|<span data-ttu-id="c463e-289">String</span><span class="sxs-lookup"><span data-stu-id="c463e-289">String</span></span>|<span data-ttu-id="c463e-290">设备类别显示名称。</span><span class="sxs-lookup"><span data-stu-id="c463e-290">Device category display name.</span></span> <span data-ttu-id="c463e-291">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c463e-291">This property is read-only.</span></span> <span data-ttu-id="c463e-292">继承自 [managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c463e-292">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="c463e-293">isSupervised</span><span class="sxs-lookup"><span data-stu-id="c463e-293">isSupervised</span></span>|<span data-ttu-id="c463e-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="c463e-294">Boolean</span></span>|<span data-ttu-id="c463e-295">设备监督状态。</span><span class="sxs-lookup"><span data-stu-id="c463e-295">Device supervised status.</span></span> <span data-ttu-id="c463e-296">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c463e-296">This property is read-only.</span></span> <span data-ttu-id="c463e-297">继承自 [managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c463e-297">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="c463e-298">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="c463e-298">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="c463e-299">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c463e-299">DateTimeOffset</span></span>|<span data-ttu-id="c463e-300">设备上次与 Exchange 联系的时间。</span><span class="sxs-lookup"><span data-stu-id="c463e-300">Last time the device contacted Exchange.</span></span> <span data-ttu-id="c463e-301">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c463e-301">This property is read-only.</span></span> <span data-ttu-id="c463e-302">继承自 [managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c463e-302">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="c463e-303">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="c463e-303">exchangeAccessState</span></span>|[<span data-ttu-id="c463e-304">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="c463e-304">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="c463e-305">Exchange 中设备的访问状态。</span><span class="sxs-lookup"><span data-stu-id="c463e-305">The Access State of the device in Exchange.</span></span> <span data-ttu-id="c463e-306">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c463e-306">This property is read-only.</span></span> <span data-ttu-id="c463e-307">继承自 [managedDevice](../resources/intune-shared-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="c463e-307">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md).</span></span> <span data-ttu-id="c463e-308">可取值为：`none`、`unknown`、`allowed`、`blocked`、`quarantined`。</span><span class="sxs-lookup"><span data-stu-id="c463e-308">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="c463e-309">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="c463e-309">exchangeAccessStateReason</span></span>|[<span data-ttu-id="c463e-310">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="c463e-310">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="c463e-311">Exchange 中设备访问状态的出现原因。</span><span class="sxs-lookup"><span data-stu-id="c463e-311">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="c463e-312">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c463e-312">This property is read-only.</span></span> <span data-ttu-id="c463e-313">继承自 [managedDevice](../resources/intune-shared-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="c463e-313">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md).</span></span> <span data-ttu-id="c463e-314">可取值为：`none`、`unknown`、`exchangeGlobalRule`、`exchangeIndividualRule`、`exchangeDeviceRule`、`exchangeUpgrade`、`exchangeMailboxPolicy`、`other`、`compliant`、`notCompliant`、`notEnrolled`、`unknownLocation`、`mfaRequired`、`azureADBlockDueToAccessPolicy`、`compromisedPassword`、`deviceNotKnownWithManagedApp`。</span><span class="sxs-lookup"><span data-stu-id="c463e-314">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="c463e-315">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="c463e-315">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="c463e-316">String</span><span class="sxs-lookup"><span data-stu-id="c463e-316">String</span></span>|<span data-ttu-id="c463e-317">允许与设备建立远程协助会话的 URL。</span><span class="sxs-lookup"><span data-stu-id="c463e-317">Url that allows a Remote Assistance session to be established with the device.</span></span> <span data-ttu-id="c463e-318">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c463e-318">This property is read-only.</span></span> <span data-ttu-id="c463e-319">继承自 [managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c463e-319">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="c463e-320">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="c463e-320">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="c463e-321">String</span><span class="sxs-lookup"><span data-stu-id="c463e-321">String</span></span>|<span data-ttu-id="c463e-322">用于在创建远程协助会话对象时识别问题的错误字符串。</span><span class="sxs-lookup"><span data-stu-id="c463e-322">An error string that identifies issues when creating Remote Assistance session objects.</span></span> <span data-ttu-id="c463e-323">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c463e-323">This property is read-only.</span></span> <span data-ttu-id="c463e-324">继承自 [managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c463e-324">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="c463e-325">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="c463e-325">isEncrypted</span></span>|<span data-ttu-id="c463e-326">Boolean</span><span class="sxs-lookup"><span data-stu-id="c463e-326">Boolean</span></span>|<span data-ttu-id="c463e-327">设备加密状态。</span><span class="sxs-lookup"><span data-stu-id="c463e-327">Device encryption status.</span></span> <span data-ttu-id="c463e-328">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c463e-328">This property is read-only.</span></span> <span data-ttu-id="c463e-329">继承自 [managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c463e-329">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="c463e-330">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c463e-330">userPrincipalName</span></span>|<span data-ttu-id="c463e-331">String</span><span class="sxs-lookup"><span data-stu-id="c463e-331">String</span></span>|<span data-ttu-id="c463e-332">设备用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="c463e-332">Device user principal name.</span></span> <span data-ttu-id="c463e-333">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c463e-333">This property is read-only.</span></span> <span data-ttu-id="c463e-334">继承自 [managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c463e-334">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="c463e-335">model</span><span class="sxs-lookup"><span data-stu-id="c463e-335">model</span></span>|<span data-ttu-id="c463e-336">String</span><span class="sxs-lookup"><span data-stu-id="c463e-336">String</span></span>|<span data-ttu-id="c463e-337">设备型号。</span><span class="sxs-lookup"><span data-stu-id="c463e-337">Model of the device.</span></span> <span data-ttu-id="c463e-338">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c463e-338">This property is read-only.</span></span> <span data-ttu-id="c463e-339">继承自 [managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c463e-339">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="c463e-340">manufacturer</span><span class="sxs-lookup"><span data-stu-id="c463e-340">manufacturer</span></span>|<span data-ttu-id="c463e-341">String</span><span class="sxs-lookup"><span data-stu-id="c463e-341">String</span></span>|<span data-ttu-id="c463e-342">设备的制造商。</span><span class="sxs-lookup"><span data-stu-id="c463e-342">Manufacturer of the device.</span></span> <span data-ttu-id="c463e-343">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c463e-343">This property is read-only.</span></span> <span data-ttu-id="c463e-344">继承自 [managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c463e-344">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="c463e-345">imei</span><span class="sxs-lookup"><span data-stu-id="c463e-345">imei</span></span>|<span data-ttu-id="c463e-346">String</span><span class="sxs-lookup"><span data-stu-id="c463e-346">String</span></span>|<span data-ttu-id="c463e-347">IMEI。</span><span class="sxs-lookup"><span data-stu-id="c463e-347">IMEI.</span></span> <span data-ttu-id="c463e-348">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c463e-348">This property is read-only.</span></span> <span data-ttu-id="c463e-349">继承自 [managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c463e-349">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="c463e-350">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="c463e-350">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="c463e-351">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c463e-351">DateTimeOffset</span></span>|<span data-ttu-id="c463e-352">设备合规性宽限期到期的 DateTime。</span><span class="sxs-lookup"><span data-stu-id="c463e-352">The DateTime when device compliance grace period expires.</span></span> <span data-ttu-id="c463e-353">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c463e-353">This property is read-only.</span></span> <span data-ttu-id="c463e-354">继承自 [managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c463e-354">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="c463e-355">serialNumber</span><span class="sxs-lookup"><span data-stu-id="c463e-355">serialNumber</span></span>|<span data-ttu-id="c463e-356">String</span><span class="sxs-lookup"><span data-stu-id="c463e-356">String</span></span>|<span data-ttu-id="c463e-357">SerialNumber。</span><span class="sxs-lookup"><span data-stu-id="c463e-357">SerialNumber.</span></span> <span data-ttu-id="c463e-358">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c463e-358">This property is read-only.</span></span> <span data-ttu-id="c463e-359">继承自 [managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c463e-359">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="c463e-360">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="c463e-360">phoneNumber</span></span>|<span data-ttu-id="c463e-361">String</span><span class="sxs-lookup"><span data-stu-id="c463e-361">String</span></span>|<span data-ttu-id="c463e-362">设备的电话号码。</span><span class="sxs-lookup"><span data-stu-id="c463e-362">Phone number of the device.</span></span> <span data-ttu-id="c463e-363">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c463e-363">This property is read-only.</span></span> <span data-ttu-id="c463e-364">继承自 [managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c463e-364">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="c463e-365">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="c463e-365">androidSecurityPatchLevel</span></span>|<span data-ttu-id="c463e-366">String</span><span class="sxs-lookup"><span data-stu-id="c463e-366">String</span></span>|<span data-ttu-id="c463e-367">Android 安全修补程序级别。</span><span class="sxs-lookup"><span data-stu-id="c463e-367">Android security patch level.</span></span> <span data-ttu-id="c463e-368">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c463e-368">This property is read-only.</span></span> <span data-ttu-id="c463e-369">继承自 [managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c463e-369">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="c463e-370">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="c463e-370">userDisplayName</span></span>|<span data-ttu-id="c463e-371">String</span><span class="sxs-lookup"><span data-stu-id="c463e-371">String</span></span>|<span data-ttu-id="c463e-372">用户显示名称。</span><span class="sxs-lookup"><span data-stu-id="c463e-372">User display name.</span></span> <span data-ttu-id="c463e-373">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c463e-373">This property is read-only.</span></span> <span data-ttu-id="c463e-374">继承自 [managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c463e-374">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="c463e-375">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="c463e-375">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="c463e-376">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="c463e-376">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="c463e-377">ConfigrMgr 客户端启用的功能。</span><span class="sxs-lookup"><span data-stu-id="c463e-377">ConfigrMgr client enabled features.</span></span> <span data-ttu-id="c463e-378">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c463e-378">This property is read-only.</span></span> <span data-ttu-id="c463e-379">继承自 [managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c463e-379">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="c463e-380">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="c463e-380">wiFiMacAddress</span></span>|<span data-ttu-id="c463e-381">String</span><span class="sxs-lookup"><span data-stu-id="c463e-381">String</span></span>|<span data-ttu-id="c463e-382">Wi-Fi MAC。</span><span class="sxs-lookup"><span data-stu-id="c463e-382">Wi-Fi MAC.</span></span> <span data-ttu-id="c463e-383">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c463e-383">This property is read-only.</span></span> <span data-ttu-id="c463e-384">继承自 [managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c463e-384">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="c463e-385">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="c463e-385">deviceHealthAttestationState</span></span>|[<span data-ttu-id="c463e-386">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="c463e-386">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="c463e-387">设备运行状况证明状态。</span><span class="sxs-lookup"><span data-stu-id="c463e-387">The device health attestation state.</span></span> <span data-ttu-id="c463e-388">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c463e-388">This property is read-only.</span></span> <span data-ttu-id="c463e-389">继承自 [managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c463e-389">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="c463e-390">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="c463e-390">subscriberCarrier</span></span>|<span data-ttu-id="c463e-391">String</span><span class="sxs-lookup"><span data-stu-id="c463e-391">String</span></span>|<span data-ttu-id="c463e-392">订阅者运营商。</span><span class="sxs-lookup"><span data-stu-id="c463e-392">Subscriber Carrier.</span></span> <span data-ttu-id="c463e-393">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c463e-393">This property is read-only.</span></span> <span data-ttu-id="c463e-394">继承自 [managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c463e-394">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="c463e-395">meid</span><span class="sxs-lookup"><span data-stu-id="c463e-395">meid</span></span>|<span data-ttu-id="c463e-396">String</span><span class="sxs-lookup"><span data-stu-id="c463e-396">String</span></span>|<span data-ttu-id="c463e-397">MEID。</span><span class="sxs-lookup"><span data-stu-id="c463e-397">MEID.</span></span> <span data-ttu-id="c463e-398">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c463e-398">This property is read-only.</span></span> <span data-ttu-id="c463e-399">继承自 [managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c463e-399">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="c463e-400">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="c463e-400">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="c463e-401">Int64</span><span class="sxs-lookup"><span data-stu-id="c463e-401">Int64</span></span>|<span data-ttu-id="c463e-402">总存储量（以字节为单位）。</span><span class="sxs-lookup"><span data-stu-id="c463e-402">Total Storage in Bytes.</span></span> <span data-ttu-id="c463e-403">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c463e-403">This property is read-only.</span></span> <span data-ttu-id="c463e-404">继承自 [managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c463e-404">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="c463e-405">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="c463e-405">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="c463e-406">Int64</span><span class="sxs-lookup"><span data-stu-id="c463e-406">Int64</span></span>|<span data-ttu-id="c463e-407">可用存储空间（以字节为单位）。</span><span class="sxs-lookup"><span data-stu-id="c463e-407">Free Storage in Bytes.</span></span> <span data-ttu-id="c463e-408">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c463e-408">This property is read-only.</span></span> <span data-ttu-id="c463e-409">继承自 [managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c463e-409">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="c463e-410">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="c463e-410">managedDeviceName</span></span>|<span data-ttu-id="c463e-411">String</span><span class="sxs-lookup"><span data-stu-id="c463e-411">String</span></span>|<span data-ttu-id="c463e-412">用于识别设备的自动生成的名称。</span><span class="sxs-lookup"><span data-stu-id="c463e-412">Automatically generated name to identify a device.</span></span> <span data-ttu-id="c463e-413">可以覆盖为用户友好名称。</span><span class="sxs-lookup"><span data-stu-id="c463e-413">Can be overwritten to a user friendly name.</span></span> <span data-ttu-id="c463e-414">继承自 [managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c463e-414">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="c463e-415">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="c463e-415">partnerReportedThreatState</span></span>|[<span data-ttu-id="c463e-416">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="c463e-416">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="c463e-417">指示帐户和设备正在使用移动威胁防护合作伙伴时设备的威胁状态。</span><span class="sxs-lookup"><span data-stu-id="c463e-417">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="c463e-418">只读。</span><span class="sxs-lookup"><span data-stu-id="c463e-418">Read Only.</span></span> <span data-ttu-id="c463e-419">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c463e-419">This property is read-only.</span></span> <span data-ttu-id="c463e-420">继承自 [managedDevice](../resources/intune-shared-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="c463e-420">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md).</span></span> <span data-ttu-id="c463e-421">可取值为：`unknown`、`activated`、`deactivated`、`secured`、`lowSeverity`、`mediumSeverity`、`highSeverity`、`unresponsive`、`compromised`、`misconfigured`。</span><span class="sxs-lookup"><span data-stu-id="c463e-421">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="c463e-422">retireAfterDateTime</span><span class="sxs-lookup"><span data-stu-id="c463e-422">retireAfterDateTime</span></span>|<span data-ttu-id="c463e-423">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c463e-423">DateTimeOffset</span></span>|<span data-ttu-id="c463e-424">指示由于计划操作而自动停用设备的时间。</span><span class="sxs-lookup"><span data-stu-id="c463e-424">Indicates the time after when a device will be auto retired because of scheduled action.</span></span> <span data-ttu-id="c463e-425">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c463e-425">This property is read-only.</span></span> <span data-ttu-id="c463e-426">继承自 [managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c463e-426">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="c463e-427">usersLoggedOn</span><span class="sxs-lookup"><span data-stu-id="c463e-427">usersLoggedOn</span></span>|<span data-ttu-id="c463e-428">[loggedOnUser](../resources/intune-devices-loggedonuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c463e-428">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="c463e-429">指示最后一次登录设备的用户。</span><span class="sxs-lookup"><span data-stu-id="c463e-429">Indicates the last logged on users of a device.</span></span> <span data-ttu-id="c463e-430">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c463e-430">This property is read-only.</span></span> <span data-ttu-id="c463e-431">继承自 [managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c463e-431">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="c463e-432">preferMdmOverGroupPolicyAppliedDateTime</span><span class="sxs-lookup"><span data-stu-id="c463e-432">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="c463e-433">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c463e-433">DateTimeOffset</span></span>|<span data-ttu-id="c463e-434">报告设置了 preferMdmOverGroupPolicy 设置的 DateTime。</span><span class="sxs-lookup"><span data-stu-id="c463e-434">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="c463e-435">设置后，如果发生冲突，Intune MDM 设置将覆盖组策略设置。</span><span class="sxs-lookup"><span data-stu-id="c463e-435">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="c463e-436">只读。</span><span class="sxs-lookup"><span data-stu-id="c463e-436">Read Only.</span></span> <span data-ttu-id="c463e-437">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c463e-437">This property is read-only.</span></span> <span data-ttu-id="c463e-438">继承自 [managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c463e-438">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="c463e-439">autopilotEnrolled</span><span class="sxs-lookup"><span data-stu-id="c463e-439">autopilotEnrolled</span></span>|<span data-ttu-id="c463e-440">布尔</span><span class="sxs-lookup"><span data-stu-id="c463e-440">Boolean</span></span>|<span data-ttu-id="c463e-441">报告托管设备是否通过自动试点注册。</span><span class="sxs-lookup"><span data-stu-id="c463e-441">Reports if the managed device is enrolled via auto-pilot.</span></span> <span data-ttu-id="c463e-442">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c463e-442">This property is read-only.</span></span> <span data-ttu-id="c463e-443">继承自 [managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c463e-443">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="c463e-444">requireUserEnrollmentApproval</span><span class="sxs-lookup"><span data-stu-id="c463e-444">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="c463e-445">布尔</span><span class="sxs-lookup"><span data-stu-id="c463e-445">Boolean</span></span>|<span data-ttu-id="c463e-446">报告托管 iOS 设备是用户审批注册。</span><span class="sxs-lookup"><span data-stu-id="c463e-446">Reports if the managed iOS device is user approval enrollment.</span></span> <span data-ttu-id="c463e-447">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c463e-447">This property is read-only.</span></span> <span data-ttu-id="c463e-448">继承自 [managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c463e-448">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="c463e-449">managementCertificateExpirationDate</span><span class="sxs-lookup"><span data-stu-id="c463e-449">managementCertificateExpirationDate</span></span>|<span data-ttu-id="c463e-450">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c463e-450">DateTimeOffset</span></span>|<span data-ttu-id="c463e-451">报告设备管理证书到期日期。</span><span class="sxs-lookup"><span data-stu-id="c463e-451">Reports device management certificate expiration date.</span></span> <span data-ttu-id="c463e-452">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c463e-452">This property is read-only.</span></span> <span data-ttu-id="c463e-453">继承自 [managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c463e-453">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="c463e-454">iccid</span><span class="sxs-lookup"><span data-stu-id="c463e-454">iccid</span></span>|<span data-ttu-id="c463e-455">String</span><span class="sxs-lookup"><span data-stu-id="c463e-455">String</span></span>|<span data-ttu-id="c463e-456">集成的电路卡标识符，它是 SIM 卡的唯一标识号。</span><span class="sxs-lookup"><span data-stu-id="c463e-456">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span> <span data-ttu-id="c463e-457">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c463e-457">This property is read-only.</span></span> <span data-ttu-id="c463e-458">继承自 [managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c463e-458">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="c463e-459">udid</span><span class="sxs-lookup"><span data-stu-id="c463e-459">udid</span></span>|<span data-ttu-id="c463e-460">String</span><span class="sxs-lookup"><span data-stu-id="c463e-460">String</span></span>|<span data-ttu-id="c463e-461">iOS 和 macOS 设备的唯一设备标识符。</span><span class="sxs-lookup"><span data-stu-id="c463e-461">Unique Device Identifier for iOS and macOS devices.</span></span> <span data-ttu-id="c463e-462">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c463e-462">This property is read-only.</span></span> <span data-ttu-id="c463e-463">继承自 [managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c463e-463">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="c463e-464">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c463e-464">roleScopeTagIds</span></span>|<span data-ttu-id="c463e-465">字符串集合</span><span class="sxs-lookup"><span data-stu-id="c463e-465">String collection</span></span>|<span data-ttu-id="c463e-466">此设备实例的范围标记标识列表。</span><span class="sxs-lookup"><span data-stu-id="c463e-466">List of Scope Tag IDs for this Device instance.</span></span> <span data-ttu-id="c463e-467">继承自 [managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c463e-467">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="c463e-468">windowsActiveMalwareCount</span><span class="sxs-lookup"><span data-stu-id="c463e-468">windowsActiveMalwareCount</span></span>|<span data-ttu-id="c463e-469">Int32</span><span class="sxs-lookup"><span data-stu-id="c463e-469">Int32</span></span>|<span data-ttu-id="c463e-470">此 Windows 设备的活动恶意软件计数。</span><span class="sxs-lookup"><span data-stu-id="c463e-470">Count of active malware for this windows device.</span></span> <span data-ttu-id="c463e-471">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c463e-471">This property is read-only.</span></span> <span data-ttu-id="c463e-472">继承自 [managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c463e-472">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="c463e-473">windowsRemediatedMalwareCount</span><span class="sxs-lookup"><span data-stu-id="c463e-473">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="c463e-474">Int32</span><span class="sxs-lookup"><span data-stu-id="c463e-474">Int32</span></span>|<span data-ttu-id="c463e-475">此 Windows 设备的已修复恶意软件计数。</span><span class="sxs-lookup"><span data-stu-id="c463e-475">Count of remediated malware for this windows device.</span></span> <span data-ttu-id="c463e-476">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c463e-476">This property is read-only.</span></span> <span data-ttu-id="c463e-477">继承自 [managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c463e-477">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="c463e-478">notes</span><span class="sxs-lookup"><span data-stu-id="c463e-478">notes</span></span>|<span data-ttu-id="c463e-479">String</span><span class="sxs-lookup"><span data-stu-id="c463e-479">String</span></span>|<span data-ttu-id="c463e-480">IT 管理员创建的设备上备注 继承自 [managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c463e-480">Notes on the device created by IT Admin Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="c463e-481">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="c463e-481">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="c463e-482">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="c463e-482">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="c463e-483">配置管理器客户端运行状况状态，仅对 MDM/ConfigMgr 代理管理的设备有效。继承自 [managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c463e-483">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="c463e-484">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="c463e-484">configurationManagerClientInformation</span></span>|[<span data-ttu-id="c463e-485">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="c463e-485">configurationManagerClientInformation</span></span>](../resources/intune-devices-configurationmanagerclientinformation.md)|<span data-ttu-id="c463e-486">配置管理器客户端信息，仅对由 ConfigMgr 代理托管、duel 托管或三管理的设备有效。继承自 [managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c463e-486">Configuration manager client information, valid only for devices managed, duel-managed or tri-managed by ConfigMgr Agent Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="c463e-487">ethernetMacAddress</span><span class="sxs-lookup"><span data-stu-id="c463e-487">ethernetMacAddress</span></span>|<span data-ttu-id="c463e-488">String</span><span class="sxs-lookup"><span data-stu-id="c463e-488">String</span></span>|<span data-ttu-id="c463e-489">以太网 MAC。</span><span class="sxs-lookup"><span data-stu-id="c463e-489">Ethernet MAC.</span></span> <span data-ttu-id="c463e-490">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c463e-490">This property is read-only.</span></span> <span data-ttu-id="c463e-491">继承自 [managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c463e-491">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="c463e-492">physicalMemoryInBytes</span><span class="sxs-lookup"><span data-stu-id="c463e-492">physicalMemoryInBytes</span></span>|<span data-ttu-id="c463e-493">Int64</span><span class="sxs-lookup"><span data-stu-id="c463e-493">Int64</span></span>|<span data-ttu-id="c463e-494">总内存（以字节为单位）。</span><span class="sxs-lookup"><span data-stu-id="c463e-494">Total Memory in Bytes.</span></span> <span data-ttu-id="c463e-495">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c463e-495">This property is read-only.</span></span> <span data-ttu-id="c463e-496">继承自 [managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c463e-496">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="c463e-497">processorArchitecture</span><span class="sxs-lookup"><span data-stu-id="c463e-497">processorArchitecture</span></span>|[<span data-ttu-id="c463e-498">managedDeviceArchitecture</span><span class="sxs-lookup"><span data-stu-id="c463e-498">managedDeviceArchitecture</span></span>](../resources/intune-devices-manageddevicearchitecture.md)|<span data-ttu-id="c463e-499">处理器体系结构。</span><span class="sxs-lookup"><span data-stu-id="c463e-499">Processor architecture.</span></span> <span data-ttu-id="c463e-500">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c463e-500">This property is read-only.</span></span> <span data-ttu-id="c463e-501">继承自 [managedDevice](../resources/intune-shared-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="c463e-501">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md).</span></span> <span data-ttu-id="c463e-502">可取值为：`unknown`、`x86`、`x64`、`arm`、`arM64`。</span><span class="sxs-lookup"><span data-stu-id="c463e-502">Possible values are: `unknown`, `x86`, `x64`, `arm`, `arM64`.</span></span>|
|<span data-ttu-id="c463e-503">specificationVersion</span><span class="sxs-lookup"><span data-stu-id="c463e-503">specificationVersion</span></span>|<span data-ttu-id="c463e-504">String</span><span class="sxs-lookup"><span data-stu-id="c463e-504">String</span></span>|<span data-ttu-id="c463e-505">规范版本。</span><span class="sxs-lookup"><span data-stu-id="c463e-505">Specification version.</span></span> <span data-ttu-id="c463e-506">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c463e-506">This property is read-only.</span></span> <span data-ttu-id="c463e-507">继承自 [managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c463e-507">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="c463e-508">joinType</span><span class="sxs-lookup"><span data-stu-id="c463e-508">joinType</span></span>|[<span data-ttu-id="c463e-509">joinType</span><span class="sxs-lookup"><span data-stu-id="c463e-509">joinType</span></span>](../resources/intune-devices-jointype.md)|<span data-ttu-id="c463e-510">设备加入类型 继承自 [managedDevice](../resources/intune-shared-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="c463e-510">Device join type Inherited from [managedDevice](../resources/intune-shared-manageddevice.md).</span></span> <span data-ttu-id="c463e-511">可取值为：`unknown`、`azureADJoined`、`azureADRegistered`、`hybridAzureADJoined`。</span><span class="sxs-lookup"><span data-stu-id="c463e-511">Possible values are: `unknown`, `azureADJoined`, `azureADRegistered`, `hybridAzureADJoined`.</span></span>|
|<span data-ttu-id="c463e-512">skuFamily</span><span class="sxs-lookup"><span data-stu-id="c463e-512">skuFamily</span></span>|<span data-ttu-id="c463e-513">String</span><span class="sxs-lookup"><span data-stu-id="c463e-513">String</span></span>|<span data-ttu-id="c463e-514">设备 sku 系列 继承自 [managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c463e-514">Device sku family Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="c463e-515">skuNumber</span><span class="sxs-lookup"><span data-stu-id="c463e-515">skuNumber</span></span>|<span data-ttu-id="c463e-516">Int32</span><span class="sxs-lookup"><span data-stu-id="c463e-516">Int32</span></span>|<span data-ttu-id="c463e-517">设备 sku 号，另请参阅： https://docs.microsoft.com/windows/win32/api/sysinfoapi/nf-sysinfoapi-getproductinfo 。</span><span class="sxs-lookup"><span data-stu-id="c463e-517">Device sku number, see also: https://docs.microsoft.com/windows/win32/api/sysinfoapi/nf-sysinfoapi-getproductinfo.</span></span> <span data-ttu-id="c463e-518">有效值为 0 到 2147483647。</span><span class="sxs-lookup"><span data-stu-id="c463e-518">Valid values 0 to 2147483647.</span></span> <span data-ttu-id="c463e-519">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c463e-519">This property is read-only.</span></span> <span data-ttu-id="c463e-520">继承自 [managedDevice](../resources/intune-shared-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c463e-520">Inherited from [managedDevice](../resources/intune-shared-manageddevice.md)</span></span>|
|<span data-ttu-id="c463e-521">managementFeatures</span><span class="sxs-lookup"><span data-stu-id="c463e-521">managementFeatures</span></span>|[<span data-ttu-id="c463e-522">managedDeviceManagementFeatures</span><span class="sxs-lookup"><span data-stu-id="c463e-522">managedDeviceManagementFeatures</span></span>](../resources/intune-devices-manageddevicemanagementfeatures.md)|<span data-ttu-id="c463e-523">设备管理功能 继承自 [managedDevice](../resources/intune-shared-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="c463e-523">Device management features Inherited from [managedDevice](../resources/intune-shared-manageddevice.md).</span></span> <span data-ttu-id="c463e-524">可取值为：`none`、`microsoftManagedDesktop`。</span><span class="sxs-lookup"><span data-stu-id="c463e-524">Possible values are: `none`, `microsoftManagedDesktop`.</span></span>|



## <a name="response"></a><span data-ttu-id="c463e-525">响应</span><span class="sxs-lookup"><span data-stu-id="c463e-525">Response</span></span>
<span data-ttu-id="c463e-526">如果成功，此方法在响应正文中返回响应 `200 OK` 代码和更新的 [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c463e-526">If successful, this method returns a `200 OK` response code and an updated [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c463e-527">示例</span><span class="sxs-lookup"><span data-stu-id="c463e-527">Example</span></span>

### <a name="request"></a><span data-ttu-id="c463e-528">请求</span><span class="sxs-lookup"><span data-stu-id="c463e-528">Request</span></span>
<span data-ttu-id="c463e-529">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c463e-529">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}
Content-type: application/json
Content-length: 8115

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
    "subnetAddress": "Subnet Address value"
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

### <a name="response"></a><span data-ttu-id="c463e-530">响应</span><span class="sxs-lookup"><span data-stu-id="c463e-530">Response</span></span>
<span data-ttu-id="c463e-p175">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c463e-p175">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 8164

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
    "subnetAddress": "Subnet Address value"
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




