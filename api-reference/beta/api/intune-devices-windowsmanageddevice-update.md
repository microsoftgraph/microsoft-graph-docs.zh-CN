---
title: 更新 windowsManagedDevice
description: 更新 windowsManagedDevice 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f9964304f08a5013c8e03c80c8e79fb44e5e89ca
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48708177"
---
# <a name="update-windowsmanageddevice"></a><span data-ttu-id="dc15f-103">更新 windowsManagedDevice</span><span class="sxs-lookup"><span data-stu-id="dc15f-103">Update windowsManagedDevice</span></span>

<span data-ttu-id="dc15f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dc15f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dc15f-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="dc15f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dc15f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="dc15f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dc15f-107">更新 [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="dc15f-107">Update the properties of a [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dc15f-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="dc15f-108">Prerequisites</span></span>
<span data-ttu-id="dc15f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dc15f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc15f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="dc15f-111">Permission type</span></span>|<span data-ttu-id="dc15f-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="dc15f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dc15f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dc15f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dc15f-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc15f-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="dc15f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dc15f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dc15f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="dc15f-116">Not supported.</span></span>|
|<span data-ttu-id="dc15f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="dc15f-117">Application</span></span>|<span data-ttu-id="dc15f-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc15f-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dc15f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dc15f-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="dc15f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="dc15f-120">Request headers</span></span>
|<span data-ttu-id="dc15f-121">标头</span><span class="sxs-lookup"><span data-stu-id="dc15f-121">Header</span></span>|<span data-ttu-id="dc15f-122">值</span><span class="sxs-lookup"><span data-stu-id="dc15f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dc15f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="dc15f-123">Authorization</span></span>|<span data-ttu-id="dc15f-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="dc15f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dc15f-125">接受</span><span class="sxs-lookup"><span data-stu-id="dc15f-125">Accept</span></span>|<span data-ttu-id="dc15f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dc15f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc15f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="dc15f-127">Request body</span></span>
<span data-ttu-id="dc15f-128">在请求正文中，提供 [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dc15f-128">In the request body, supply a JSON representation for the [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object.</span></span>

<span data-ttu-id="dc15f-129">下表显示创建 [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="dc15f-129">The following table shows the properties that are required when you create the [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md).</span></span>

|<span data-ttu-id="dc15f-130">属性</span><span class="sxs-lookup"><span data-stu-id="dc15f-130">Property</span></span>|<span data-ttu-id="dc15f-131">类型</span><span class="sxs-lookup"><span data-stu-id="dc15f-131">Type</span></span>|<span data-ttu-id="dc15f-132">说明</span><span class="sxs-lookup"><span data-stu-id="dc15f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc15f-133">id</span><span class="sxs-lookup"><span data-stu-id="dc15f-133">id</span></span>|<span data-ttu-id="dc15f-134">String</span><span class="sxs-lookup"><span data-stu-id="dc15f-134">String</span></span>|<span data-ttu-id="dc15f-135">设备的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="dc15f-135">Unique Identifier for the device.</span></span> <span data-ttu-id="dc15f-136">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="dc15f-136">This property is read-only.</span></span> <span data-ttu-id="dc15f-137">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="dc15f-137">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="dc15f-138">userId</span><span class="sxs-lookup"><span data-stu-id="dc15f-138">userId</span></span>|<span data-ttu-id="dc15f-139">String</span><span class="sxs-lookup"><span data-stu-id="dc15f-139">String</span></span>|<span data-ttu-id="dc15f-140">与设备关联的用户的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="dc15f-140">Unique Identifier for the user associated with the device.</span></span> <span data-ttu-id="dc15f-141">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="dc15f-141">This property is read-only.</span></span> <span data-ttu-id="dc15f-142">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="dc15f-142">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="dc15f-143">deviceName</span><span class="sxs-lookup"><span data-stu-id="dc15f-143">deviceName</span></span>|<span data-ttu-id="dc15f-144">String</span><span class="sxs-lookup"><span data-stu-id="dc15f-144">String</span></span>|<span data-ttu-id="dc15f-145">设备的名称。</span><span class="sxs-lookup"><span data-stu-id="dc15f-145">Name of the device.</span></span> <span data-ttu-id="dc15f-146">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="dc15f-146">This property is read-only.</span></span> <span data-ttu-id="dc15f-147">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="dc15f-147">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="dc15f-148">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="dc15f-148">hardwareInformation</span></span>|[<span data-ttu-id="dc15f-149">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="dc15f-149">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="dc15f-150">设备的 hardward 详细信息。</span><span class="sxs-lookup"><span data-stu-id="dc15f-150">The hardward details for the device.</span></span>  <span data-ttu-id="dc15f-151">包括存储空间、制造商、序列号等信息。此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="dc15f-151">Includes information such as storage space, manufacturer, serial number, etc. This property is read-only.</span></span> <span data-ttu-id="dc15f-152">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="dc15f-152">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="dc15f-153">所有者</span><span class="sxs-lookup"><span data-stu-id="dc15f-153">ownerType</span></span>|[<span data-ttu-id="dc15f-154">所有者</span><span class="sxs-lookup"><span data-stu-id="dc15f-154">ownerType</span></span>](../resources/intune-shared-ownertype.md)|<span data-ttu-id="dc15f-155">设备的所有权。</span><span class="sxs-lookup"><span data-stu-id="dc15f-155">Ownership of the device.</span></span> <span data-ttu-id="dc15f-156">可以是从 [ManagedDevice](../resources/intune-devices-manageddevice.md)继承的 "公司" 或 "个人"。</span><span class="sxs-lookup"><span data-stu-id="dc15f-156">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="dc15f-157">可取值为：`unknown`、`company`、`personal`。</span><span class="sxs-lookup"><span data-stu-id="dc15f-157">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="dc15f-158">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="dc15f-158">managedDeviceOwnerType</span></span>|[<span data-ttu-id="dc15f-159">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="dc15f-159">managedDeviceOwnerType</span></span>](../resources/intune-shared-manageddeviceownertype.md)|<span data-ttu-id="dc15f-160">设备的所有权。</span><span class="sxs-lookup"><span data-stu-id="dc15f-160">Ownership of the device.</span></span> <span data-ttu-id="dc15f-161">可以是从 [ManagedDevice](../resources/intune-devices-manageddevice.md)继承的 "公司" 或 "个人"。</span><span class="sxs-lookup"><span data-stu-id="dc15f-161">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="dc15f-162">可取值为：`unknown`、`company`、`personal`。</span><span class="sxs-lookup"><span data-stu-id="dc15f-162">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="dc15f-163">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="dc15f-163">deviceActionResults</span></span>|<span data-ttu-id="dc15f-164">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) 集合</span><span class="sxs-lookup"><span data-stu-id="dc15f-164">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="dc15f-165">ComplexType deviceActionResult 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="dc15f-165">List of ComplexType deviceActionResult objects.</span></span> <span data-ttu-id="dc15f-166">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="dc15f-166">This property is read-only.</span></span> <span data-ttu-id="dc15f-167">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="dc15f-167">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="dc15f-168">managementState</span><span class="sxs-lookup"><span data-stu-id="dc15f-168">managementState</span></span>|[<span data-ttu-id="dc15f-169">managementState</span><span class="sxs-lookup"><span data-stu-id="dc15f-169">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="dc15f-170">设备的管理状态。</span><span class="sxs-lookup"><span data-stu-id="dc15f-170">Management state of the device.</span></span> <span data-ttu-id="dc15f-171">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="dc15f-171">This property is read-only.</span></span> <span data-ttu-id="dc15f-172">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="dc15f-172">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="dc15f-173">可取值为：`managed`、`retirePending`、`retireFailed`、`wipePending`、`wipeFailed`、`unhealthy`、`deletePending`、`retireIssued`、`wipeIssued`、`wipeCanceled`、`retireCanceled`、`discovered`。</span><span class="sxs-lookup"><span data-stu-id="dc15f-173">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="dc15f-174">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="dc15f-174">enrolledDateTime</span></span>|<span data-ttu-id="dc15f-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dc15f-175">DateTimeOffset</span></span>|<span data-ttu-id="dc15f-176">设备的注册时间。</span><span class="sxs-lookup"><span data-stu-id="dc15f-176">Enrollment time of the device.</span></span> <span data-ttu-id="dc15f-177">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="dc15f-177">This property is read-only.</span></span> <span data-ttu-id="dc15f-178">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="dc15f-178">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="dc15f-179">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="dc15f-179">lastSyncDateTime</span></span>|<span data-ttu-id="dc15f-180">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dc15f-180">DateTimeOffset</span></span>|<span data-ttu-id="dc15f-181">设备上次成功完成与 Intune 同步的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="dc15f-181">The date and time that the device last completed a successful sync with Intune.</span></span> <span data-ttu-id="dc15f-182">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="dc15f-182">This property is read-only.</span></span> <span data-ttu-id="dc15f-183">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="dc15f-183">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="dc15f-184">chassisType</span><span class="sxs-lookup"><span data-stu-id="dc15f-184">chassisType</span></span>|[<span data-ttu-id="dc15f-185">chassisType</span><span class="sxs-lookup"><span data-stu-id="dc15f-185">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="dc15f-186">设备的机箱类型。</span><span class="sxs-lookup"><span data-stu-id="dc15f-186">Chassis type of the device.</span></span> <span data-ttu-id="dc15f-187">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="dc15f-187">This property is read-only.</span></span> <span data-ttu-id="dc15f-188">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="dc15f-188">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="dc15f-189">可取值为：`unknown`、`desktop`、`laptop`、`worksWorkstation`、`enterpriseServer`、`phone`、`tablet`、`mobileOther`、`mobileUnknown`。</span><span class="sxs-lookup"><span data-stu-id="dc15f-189">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="dc15f-190">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="dc15f-190">operatingSystem</span></span>|<span data-ttu-id="dc15f-191">String</span><span class="sxs-lookup"><span data-stu-id="dc15f-191">String</span></span>|<span data-ttu-id="dc15f-192">设备的操作系统。</span><span class="sxs-lookup"><span data-stu-id="dc15f-192">Operating system of the device.</span></span> <span data-ttu-id="dc15f-193">Windows、iOS 等。此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="dc15f-193">Windows, iOS, etc. This property is read-only.</span></span> <span data-ttu-id="dc15f-194">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="dc15f-194">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="dc15f-195">deviceType</span><span class="sxs-lookup"><span data-stu-id="dc15f-195">deviceType</span></span>|[<span data-ttu-id="dc15f-196">deviceType</span><span class="sxs-lookup"><span data-stu-id="dc15f-196">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="dc15f-197">设备的平台。</span><span class="sxs-lookup"><span data-stu-id="dc15f-197">Platform of the device.</span></span> <span data-ttu-id="dc15f-198">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="dc15f-198">This property is read-only.</span></span> <span data-ttu-id="dc15f-199">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="dc15f-199">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="dc15f-200">可能的值为：、、、、、、、、、、、、、、、、、、、、、、、、 `desktop` `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `windows10x` `androidnGMS` `cloudPC` `blackberry` `palm` `unknown` 。</span><span class="sxs-lookup"><span data-stu-id="dc15f-200">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `androidnGMS`, `cloudPC`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="dc15f-201">complianceState</span><span class="sxs-lookup"><span data-stu-id="dc15f-201">complianceState</span></span>|[<span data-ttu-id="dc15f-202">complianceState</span><span class="sxs-lookup"><span data-stu-id="dc15f-202">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="dc15f-203">设备的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="dc15f-203">Compliance state of the device.</span></span> <span data-ttu-id="dc15f-204">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="dc15f-204">This property is read-only.</span></span> <span data-ttu-id="dc15f-205">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="dc15f-205">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="dc15f-206">可取值为：`unknown`、`compliant`、`noncompliant`、`conflict`、`error`、`inGracePeriod`、`configManager`。</span><span class="sxs-lookup"><span data-stu-id="dc15f-206">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="dc15f-207">jailBroken</span><span class="sxs-lookup"><span data-stu-id="dc15f-207">jailBroken</span></span>|<span data-ttu-id="dc15f-208">String</span><span class="sxs-lookup"><span data-stu-id="dc15f-208">String</span></span>|<span data-ttu-id="dc15f-209">设备是否已越狱或取得 root 权限。</span><span class="sxs-lookup"><span data-stu-id="dc15f-209">whether the device is jail broken or rooted.</span></span> <span data-ttu-id="dc15f-210">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="dc15f-210">This property is read-only.</span></span> <span data-ttu-id="dc15f-211">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="dc15f-211">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="dc15f-212">managementAgent</span><span class="sxs-lookup"><span data-stu-id="dc15f-212">managementAgent</span></span>|[<span data-ttu-id="dc15f-213">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="dc15f-213">managementAgentType</span></span>](../resources/intune-shared-managementagenttype.md)|<span data-ttu-id="dc15f-214">设备的管理通道。</span><span class="sxs-lookup"><span data-stu-id="dc15f-214">Management channel of the device.</span></span> <span data-ttu-id="dc15f-215">Intune、EAS 等。此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="dc15f-215">Intune, EAS, etc. This property is read-only.</span></span> <span data-ttu-id="dc15f-216">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="dc15f-216">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="dc15f-217">可取值为：`eas`、`mdm`、`easMdm`、`intuneClient`、`easIntuneClient`、`configurationManagerClient`、`configurationManagerClientMdm`、`configurationManagerClientMdmEas`、`unknown`、`jamf`、`googleCloudDevicePolicyController`、`microsoft365ManagedMdm`。</span><span class="sxs-lookup"><span data-stu-id="dc15f-217">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span></span>|
|<span data-ttu-id="dc15f-218">osVersion</span><span class="sxs-lookup"><span data-stu-id="dc15f-218">osVersion</span></span>|<span data-ttu-id="dc15f-219">String</span><span class="sxs-lookup"><span data-stu-id="dc15f-219">String</span></span>|<span data-ttu-id="dc15f-220">设备的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="dc15f-220">Operating system version of the device.</span></span> <span data-ttu-id="dc15f-221">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="dc15f-221">This property is read-only.</span></span> <span data-ttu-id="dc15f-222">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="dc15f-222">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="dc15f-223">easActivated</span><span class="sxs-lookup"><span data-stu-id="dc15f-223">easActivated</span></span>|<span data-ttu-id="dc15f-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc15f-224">Boolean</span></span>|<span data-ttu-id="dc15f-225">设备是否已激活 Exchange ActiveSync。</span><span class="sxs-lookup"><span data-stu-id="dc15f-225">Whether the device is Exchange ActiveSync activated.</span></span> <span data-ttu-id="dc15f-226">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="dc15f-226">This property is read-only.</span></span> <span data-ttu-id="dc15f-227">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="dc15f-227">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="dc15f-228">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="dc15f-228">easDeviceId</span></span>|<span data-ttu-id="dc15f-229">String</span><span class="sxs-lookup"><span data-stu-id="dc15f-229">String</span></span>|<span data-ttu-id="dc15f-230">设备的 Exchange ActiveSync ID。</span><span class="sxs-lookup"><span data-stu-id="dc15f-230">Exchange ActiveSync Id of the device.</span></span> <span data-ttu-id="dc15f-231">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="dc15f-231">This property is read-only.</span></span> <span data-ttu-id="dc15f-232">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="dc15f-232">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="dc15f-233">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="dc15f-233">easActivationDateTime</span></span>|<span data-ttu-id="dc15f-234">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dc15f-234">DateTimeOffset</span></span>|<span data-ttu-id="dc15f-235">设备的 Exchange ActivationSync 激活时间。</span><span class="sxs-lookup"><span data-stu-id="dc15f-235">Exchange ActivationSync activation time of the device.</span></span> <span data-ttu-id="dc15f-236">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="dc15f-236">This property is read-only.</span></span> <span data-ttu-id="dc15f-237">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="dc15f-237">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="dc15f-238">aadRegistered</span><span class="sxs-lookup"><span data-stu-id="dc15f-238">aadRegistered</span></span>|<span data-ttu-id="dc15f-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc15f-239">Boolean</span></span>|<span data-ttu-id="dc15f-240">设备是否已注册 Azure Active Directory。</span><span class="sxs-lookup"><span data-stu-id="dc15f-240">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="dc15f-241">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="dc15f-241">This property is read-only.</span></span> <span data-ttu-id="dc15f-242">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="dc15f-242">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="dc15f-243">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="dc15f-243">azureADRegistered</span></span>|<span data-ttu-id="dc15f-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc15f-244">Boolean</span></span>|<span data-ttu-id="dc15f-245">设备是否已注册 Azure Active Directory。</span><span class="sxs-lookup"><span data-stu-id="dc15f-245">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="dc15f-246">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="dc15f-246">This property is read-only.</span></span> <span data-ttu-id="dc15f-247">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="dc15f-247">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="dc15f-248">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="dc15f-248">deviceEnrollmentType</span></span>|[<span data-ttu-id="dc15f-249">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="dc15f-249">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="dc15f-250">设备的注册类型。</span><span class="sxs-lookup"><span data-stu-id="dc15f-250">Enrollment type of the device.</span></span> <span data-ttu-id="dc15f-251">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="dc15f-251">This property is read-only.</span></span> <span data-ttu-id="dc15f-252">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="dc15f-252">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="dc15f-253">可取值为：`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement`、`appleUserEnrollment`、`appleUserEnrollmentWithServiceAccount`、`azureAdJoinUsingAzureVmExtension`、`androidEnterpriseDedicatedDevice`、`androidEnterpriseFullyManaged`、`androidEnterpriseCorporateWorkProfile`。</span><span class="sxs-lookup"><span data-stu-id="dc15f-253">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`, `azureAdJoinUsingAzureVmExtension`, `androidEnterpriseDedicatedDevice`, `androidEnterpriseFullyManaged`, `androidEnterpriseCorporateWorkProfile`.</span></span>|
|<span data-ttu-id="dc15f-254">lostModeState</span><span class="sxs-lookup"><span data-stu-id="dc15f-254">lostModeState</span></span>|[<span data-ttu-id="dc15f-255">lostModeState</span><span class="sxs-lookup"><span data-stu-id="dc15f-255">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="dc15f-256">指示是否已启用或禁用了丢失模式。</span><span class="sxs-lookup"><span data-stu-id="dc15f-256">Indicates if Lost mode is enabled or disabled.</span></span> <span data-ttu-id="dc15f-257">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="dc15f-257">This property is read-only.</span></span> <span data-ttu-id="dc15f-258">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="dc15f-258">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="dc15f-259">可取值为：`disabled`、`enabled`。</span><span class="sxs-lookup"><span data-stu-id="dc15f-259">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="dc15f-260">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="dc15f-260">activationLockBypassCode</span></span>|<span data-ttu-id="dc15f-261">String</span><span class="sxs-lookup"><span data-stu-id="dc15f-261">String</span></span>|<span data-ttu-id="dc15f-262">允许绕过设备上的激活锁的代码。</span><span class="sxs-lookup"><span data-stu-id="dc15f-262">Code that allows the Activation Lock on a device to be bypassed.</span></span> <span data-ttu-id="dc15f-263">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="dc15f-263">This property is read-only.</span></span> <span data-ttu-id="dc15f-264">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="dc15f-264">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="dc15f-265">emailAddress</span><span class="sxs-lookup"><span data-stu-id="dc15f-265">emailAddress</span></span>|<span data-ttu-id="dc15f-266">String</span><span class="sxs-lookup"><span data-stu-id="dc15f-266">String</span></span>|<span data-ttu-id="dc15f-267">与设备关联的用户的电子邮件 (s) 。</span><span class="sxs-lookup"><span data-stu-id="dc15f-267">Email(s) for the user associated with the device.</span></span> <span data-ttu-id="dc15f-268">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="dc15f-268">This property is read-only.</span></span> <span data-ttu-id="dc15f-269">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="dc15f-269">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="dc15f-270">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="dc15f-270">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="dc15f-271">String</span><span class="sxs-lookup"><span data-stu-id="dc15f-271">String</span></span>|<span data-ttu-id="dc15f-272">Azure Active Directory 设备的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="dc15f-272">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="dc15f-273">只读。</span><span class="sxs-lookup"><span data-stu-id="dc15f-273">Read only.</span></span> <span data-ttu-id="dc15f-274">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="dc15f-274">This property is read-only.</span></span> <span data-ttu-id="dc15f-275">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="dc15f-275">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="dc15f-276">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="dc15f-276">azureADDeviceId</span></span>|<span data-ttu-id="dc15f-277">String</span><span class="sxs-lookup"><span data-stu-id="dc15f-277">String</span></span>|<span data-ttu-id="dc15f-278">Azure Active Directory 设备的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="dc15f-278">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="dc15f-279">只读。</span><span class="sxs-lookup"><span data-stu-id="dc15f-279">Read only.</span></span> <span data-ttu-id="dc15f-280">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="dc15f-280">This property is read-only.</span></span> <span data-ttu-id="dc15f-281">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="dc15f-281">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="dc15f-282">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="dc15f-282">deviceRegistrationState</span></span>|[<span data-ttu-id="dc15f-283">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="dc15f-283">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="dc15f-284">设备注册状态。</span><span class="sxs-lookup"><span data-stu-id="dc15f-284">Device registration state.</span></span> <span data-ttu-id="dc15f-285">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="dc15f-285">This property is read-only.</span></span> <span data-ttu-id="dc15f-286">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="dc15f-286">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="dc15f-287">可取值为：`notRegistered`、`registered`、`revoked`、`keyConflict`、`approvalPending`、`certificateReset`、`notRegisteredPendingEnrollment`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="dc15f-287">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="dc15f-288">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="dc15f-288">deviceCategoryDisplayName</span></span>|<span data-ttu-id="dc15f-289">String</span><span class="sxs-lookup"><span data-stu-id="dc15f-289">String</span></span>|<span data-ttu-id="dc15f-290">设备类别显示名称。</span><span class="sxs-lookup"><span data-stu-id="dc15f-290">Device category display name.</span></span> <span data-ttu-id="dc15f-291">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="dc15f-291">This property is read-only.</span></span> <span data-ttu-id="dc15f-292">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="dc15f-292">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="dc15f-293">isSupervised</span><span class="sxs-lookup"><span data-stu-id="dc15f-293">isSupervised</span></span>|<span data-ttu-id="dc15f-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc15f-294">Boolean</span></span>|<span data-ttu-id="dc15f-295">设备监督状态。</span><span class="sxs-lookup"><span data-stu-id="dc15f-295">Device supervised status.</span></span> <span data-ttu-id="dc15f-296">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="dc15f-296">This property is read-only.</span></span> <span data-ttu-id="dc15f-297">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="dc15f-297">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="dc15f-298">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="dc15f-298">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="dc15f-299">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dc15f-299">DateTimeOffset</span></span>|<span data-ttu-id="dc15f-300">设备上次与 Exchange 联系的时间。</span><span class="sxs-lookup"><span data-stu-id="dc15f-300">Last time the device contacted Exchange.</span></span> <span data-ttu-id="dc15f-301">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="dc15f-301">This property is read-only.</span></span> <span data-ttu-id="dc15f-302">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="dc15f-302">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="dc15f-303">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="dc15f-303">exchangeAccessState</span></span>|[<span data-ttu-id="dc15f-304">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="dc15f-304">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="dc15f-305">Exchange 中设备的访问状态。</span><span class="sxs-lookup"><span data-stu-id="dc15f-305">The Access State of the device in Exchange.</span></span> <span data-ttu-id="dc15f-306">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="dc15f-306">This property is read-only.</span></span> <span data-ttu-id="dc15f-307">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="dc15f-307">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="dc15f-308">可取值为：`none`、`unknown`、`allowed`、`blocked`、`quarantined`。</span><span class="sxs-lookup"><span data-stu-id="dc15f-308">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="dc15f-309">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="dc15f-309">exchangeAccessStateReason</span></span>|[<span data-ttu-id="dc15f-310">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="dc15f-310">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="dc15f-311">Exchange 中设备访问状态的出现原因。</span><span class="sxs-lookup"><span data-stu-id="dc15f-311">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="dc15f-312">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="dc15f-312">This property is read-only.</span></span> <span data-ttu-id="dc15f-313">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="dc15f-313">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="dc15f-314">可取值为：`none`、`unknown`、`exchangeGlobalRule`、`exchangeIndividualRule`、`exchangeDeviceRule`、`exchangeUpgrade`、`exchangeMailboxPolicy`、`other`、`compliant`、`notCompliant`、`notEnrolled`、`unknownLocation`、`mfaRequired`、`azureADBlockDueToAccessPolicy`、`compromisedPassword`、`deviceNotKnownWithManagedApp`。</span><span class="sxs-lookup"><span data-stu-id="dc15f-314">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="dc15f-315">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="dc15f-315">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="dc15f-316">String</span><span class="sxs-lookup"><span data-stu-id="dc15f-316">String</span></span>|<span data-ttu-id="dc15f-317">允许与设备建立远程协助会话的 URL。</span><span class="sxs-lookup"><span data-stu-id="dc15f-317">Url that allows a Remote Assistance session to be established with the device.</span></span> <span data-ttu-id="dc15f-318">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="dc15f-318">This property is read-only.</span></span> <span data-ttu-id="dc15f-319">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="dc15f-319">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="dc15f-320">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="dc15f-320">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="dc15f-321">String</span><span class="sxs-lookup"><span data-stu-id="dc15f-321">String</span></span>|<span data-ttu-id="dc15f-322">用于在创建远程协助会话对象时识别问题的错误字符串。</span><span class="sxs-lookup"><span data-stu-id="dc15f-322">An error string that identifies issues when creating Remote Assistance session objects.</span></span> <span data-ttu-id="dc15f-323">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="dc15f-323">This property is read-only.</span></span> <span data-ttu-id="dc15f-324">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="dc15f-324">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="dc15f-325">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="dc15f-325">isEncrypted</span></span>|<span data-ttu-id="dc15f-326">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc15f-326">Boolean</span></span>|<span data-ttu-id="dc15f-327">设备加密状态。</span><span class="sxs-lookup"><span data-stu-id="dc15f-327">Device encryption status.</span></span> <span data-ttu-id="dc15f-328">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="dc15f-328">This property is read-only.</span></span> <span data-ttu-id="dc15f-329">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="dc15f-329">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="dc15f-330">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="dc15f-330">userPrincipalName</span></span>|<span data-ttu-id="dc15f-331">String</span><span class="sxs-lookup"><span data-stu-id="dc15f-331">String</span></span>|<span data-ttu-id="dc15f-332">设备用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="dc15f-332">Device user principal name.</span></span> <span data-ttu-id="dc15f-333">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="dc15f-333">This property is read-only.</span></span> <span data-ttu-id="dc15f-334">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="dc15f-334">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="dc15f-335">model</span><span class="sxs-lookup"><span data-stu-id="dc15f-335">model</span></span>|<span data-ttu-id="dc15f-336">String</span><span class="sxs-lookup"><span data-stu-id="dc15f-336">String</span></span>|<span data-ttu-id="dc15f-337">设备的模型。</span><span class="sxs-lookup"><span data-stu-id="dc15f-337">Model of the device.</span></span> <span data-ttu-id="dc15f-338">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="dc15f-338">This property is read-only.</span></span> <span data-ttu-id="dc15f-339">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="dc15f-339">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="dc15f-340">manufacturer</span><span class="sxs-lookup"><span data-stu-id="dc15f-340">manufacturer</span></span>|<span data-ttu-id="dc15f-341">String</span><span class="sxs-lookup"><span data-stu-id="dc15f-341">String</span></span>|<span data-ttu-id="dc15f-342">设备的制造商。</span><span class="sxs-lookup"><span data-stu-id="dc15f-342">Manufacturer of the device.</span></span> <span data-ttu-id="dc15f-343">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="dc15f-343">This property is read-only.</span></span> <span data-ttu-id="dc15f-344">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="dc15f-344">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="dc15f-345">imei</span><span class="sxs-lookup"><span data-stu-id="dc15f-345">imei</span></span>|<span data-ttu-id="dc15f-346">String</span><span class="sxs-lookup"><span data-stu-id="dc15f-346">String</span></span>|<span data-ttu-id="dc15f-347">IMEI.</span><span class="sxs-lookup"><span data-stu-id="dc15f-347">IMEI.</span></span> <span data-ttu-id="dc15f-348">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="dc15f-348">This property is read-only.</span></span> <span data-ttu-id="dc15f-349">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="dc15f-349">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="dc15f-350">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="dc15f-350">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="dc15f-351">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dc15f-351">DateTimeOffset</span></span>|<span data-ttu-id="dc15f-352">设备符合性宽限期到期时的日期时间。</span><span class="sxs-lookup"><span data-stu-id="dc15f-352">The DateTime when device compliance grace period expires.</span></span> <span data-ttu-id="dc15f-353">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="dc15f-353">This property is read-only.</span></span> <span data-ttu-id="dc15f-354">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="dc15f-354">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="dc15f-355">serialNumber</span><span class="sxs-lookup"><span data-stu-id="dc15f-355">serialNumber</span></span>|<span data-ttu-id="dc15f-356">String</span><span class="sxs-lookup"><span data-stu-id="dc15f-356">String</span></span>|<span data-ttu-id="dc15f-357">SerialNumber.</span><span class="sxs-lookup"><span data-stu-id="dc15f-357">SerialNumber.</span></span> <span data-ttu-id="dc15f-358">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="dc15f-358">This property is read-only.</span></span> <span data-ttu-id="dc15f-359">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="dc15f-359">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="dc15f-360">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="dc15f-360">phoneNumber</span></span>|<span data-ttu-id="dc15f-361">String</span><span class="sxs-lookup"><span data-stu-id="dc15f-361">String</span></span>|<span data-ttu-id="dc15f-362">设备的电话号码。</span><span class="sxs-lookup"><span data-stu-id="dc15f-362">Phone number of the device.</span></span> <span data-ttu-id="dc15f-363">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="dc15f-363">This property is read-only.</span></span> <span data-ttu-id="dc15f-364">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="dc15f-364">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="dc15f-365">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="dc15f-365">androidSecurityPatchLevel</span></span>|<span data-ttu-id="dc15f-366">String</span><span class="sxs-lookup"><span data-stu-id="dc15f-366">String</span></span>|<span data-ttu-id="dc15f-367">Android 安全修补程序级别。</span><span class="sxs-lookup"><span data-stu-id="dc15f-367">Android security patch level.</span></span> <span data-ttu-id="dc15f-368">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="dc15f-368">This property is read-only.</span></span> <span data-ttu-id="dc15f-369">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="dc15f-369">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="dc15f-370">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="dc15f-370">userDisplayName</span></span>|<span data-ttu-id="dc15f-371">String</span><span class="sxs-lookup"><span data-stu-id="dc15f-371">String</span></span>|<span data-ttu-id="dc15f-372">用户显示名称。</span><span class="sxs-lookup"><span data-stu-id="dc15f-372">User display name.</span></span> <span data-ttu-id="dc15f-373">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="dc15f-373">This property is read-only.</span></span> <span data-ttu-id="dc15f-374">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="dc15f-374">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="dc15f-375">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="dc15f-375">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="dc15f-376">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="dc15f-376">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="dc15f-377">ConfigrMgr 客户端启用的功能。</span><span class="sxs-lookup"><span data-stu-id="dc15f-377">ConfigrMgr client enabled features.</span></span> <span data-ttu-id="dc15f-378">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="dc15f-378">This property is read-only.</span></span> <span data-ttu-id="dc15f-379">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="dc15f-379">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="dc15f-380">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="dc15f-380">wiFiMacAddress</span></span>|<span data-ttu-id="dc15f-381">String</span><span class="sxs-lookup"><span data-stu-id="dc15f-381">String</span></span>|<span data-ttu-id="dc15f-382">Wi-Fi MAC。</span><span class="sxs-lookup"><span data-stu-id="dc15f-382">Wi-Fi MAC.</span></span> <span data-ttu-id="dc15f-383">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="dc15f-383">This property is read-only.</span></span> <span data-ttu-id="dc15f-384">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="dc15f-384">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="dc15f-385">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="dc15f-385">deviceHealthAttestationState</span></span>|[<span data-ttu-id="dc15f-386">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="dc15f-386">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="dc15f-387">设备运行状况证明状态。</span><span class="sxs-lookup"><span data-stu-id="dc15f-387">The device health attestation state.</span></span> <span data-ttu-id="dc15f-388">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="dc15f-388">This property is read-only.</span></span> <span data-ttu-id="dc15f-389">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="dc15f-389">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="dc15f-390">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="dc15f-390">subscriberCarrier</span></span>|<span data-ttu-id="dc15f-391">String</span><span class="sxs-lookup"><span data-stu-id="dc15f-391">String</span></span>|<span data-ttu-id="dc15f-392">订阅者运营商。</span><span class="sxs-lookup"><span data-stu-id="dc15f-392">Subscriber Carrier.</span></span> <span data-ttu-id="dc15f-393">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="dc15f-393">This property is read-only.</span></span> <span data-ttu-id="dc15f-394">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="dc15f-394">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="dc15f-395">meid</span><span class="sxs-lookup"><span data-stu-id="dc15f-395">meid</span></span>|<span data-ttu-id="dc15f-396">String</span><span class="sxs-lookup"><span data-stu-id="dc15f-396">String</span></span>|<span data-ttu-id="dc15f-397">MEID.</span><span class="sxs-lookup"><span data-stu-id="dc15f-397">MEID.</span></span> <span data-ttu-id="dc15f-398">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="dc15f-398">This property is read-only.</span></span> <span data-ttu-id="dc15f-399">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="dc15f-399">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="dc15f-400">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="dc15f-400">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="dc15f-401">Int64</span><span class="sxs-lookup"><span data-stu-id="dc15f-401">Int64</span></span>|<span data-ttu-id="dc15f-402">总存储量（以字节为单位）。</span><span class="sxs-lookup"><span data-stu-id="dc15f-402">Total Storage in Bytes.</span></span> <span data-ttu-id="dc15f-403">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="dc15f-403">This property is read-only.</span></span> <span data-ttu-id="dc15f-404">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="dc15f-404">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="dc15f-405">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="dc15f-405">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="dc15f-406">Int64</span><span class="sxs-lookup"><span data-stu-id="dc15f-406">Int64</span></span>|<span data-ttu-id="dc15f-407">以字节为单位的可用存储空间。</span><span class="sxs-lookup"><span data-stu-id="dc15f-407">Free Storage in Bytes.</span></span> <span data-ttu-id="dc15f-408">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="dc15f-408">This property is read-only.</span></span> <span data-ttu-id="dc15f-409">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="dc15f-409">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="dc15f-410">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="dc15f-410">managedDeviceName</span></span>|<span data-ttu-id="dc15f-411">String</span><span class="sxs-lookup"><span data-stu-id="dc15f-411">String</span></span>|<span data-ttu-id="dc15f-412">用于识别设备的自动生成的名称。</span><span class="sxs-lookup"><span data-stu-id="dc15f-412">Automatically generated name to identify a device.</span></span> <span data-ttu-id="dc15f-413">可以覆盖为用户友好名称。</span><span class="sxs-lookup"><span data-stu-id="dc15f-413">Can be overwritten to a user friendly name.</span></span> <span data-ttu-id="dc15f-414">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="dc15f-414">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="dc15f-415">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="dc15f-415">partnerReportedThreatState</span></span>|[<span data-ttu-id="dc15f-416">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="dc15f-416">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="dc15f-417">指示帐户和设备正在使用移动威胁防护合作伙伴时设备的威胁状态。</span><span class="sxs-lookup"><span data-stu-id="dc15f-417">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="dc15f-418">只读。</span><span class="sxs-lookup"><span data-stu-id="dc15f-418">Read Only.</span></span> <span data-ttu-id="dc15f-419">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="dc15f-419">This property is read-only.</span></span> <span data-ttu-id="dc15f-420">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="dc15f-420">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="dc15f-421">可取值为：`unknown`、`activated`、`deactivated`、`secured`、`lowSeverity`、`mediumSeverity`、`highSeverity`、`unresponsive`、`compromised`、`misconfigured`。</span><span class="sxs-lookup"><span data-stu-id="dc15f-421">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="dc15f-422">retireAfterDateTime</span><span class="sxs-lookup"><span data-stu-id="dc15f-422">retireAfterDateTime</span></span>|<span data-ttu-id="dc15f-423">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dc15f-423">DateTimeOffset</span></span>|<span data-ttu-id="dc15f-424">指示当设备因计划操作而自动停用的时间。</span><span class="sxs-lookup"><span data-stu-id="dc15f-424">Indicates the time after when a device will be auto retired because of scheduled action.</span></span> <span data-ttu-id="dc15f-425">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="dc15f-425">This property is read-only.</span></span> <span data-ttu-id="dc15f-426">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="dc15f-426">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="dc15f-427">usersLoggedOn</span><span class="sxs-lookup"><span data-stu-id="dc15f-427">usersLoggedOn</span></span>|<span data-ttu-id="dc15f-428">[loggedOnUser](../resources/intune-devices-loggedonuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="dc15f-428">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="dc15f-429">指示设备的上次登录用户。</span><span class="sxs-lookup"><span data-stu-id="dc15f-429">Indicates the last logged on users of a device.</span></span> <span data-ttu-id="dc15f-430">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="dc15f-430">This property is read-only.</span></span> <span data-ttu-id="dc15f-431">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="dc15f-431">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="dc15f-432">preferMdmOverGroupPolicyAppliedDateTime</span><span class="sxs-lookup"><span data-stu-id="dc15f-432">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="dc15f-433">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dc15f-433">DateTimeOffset</span></span>|<span data-ttu-id="dc15f-434">报告设置了 preferMdmOverGroupPolicy 设置的 DateTime。</span><span class="sxs-lookup"><span data-stu-id="dc15f-434">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="dc15f-435">设置后，如果存在冲突，Intune MDM 设置将覆盖组策略设置。</span><span class="sxs-lookup"><span data-stu-id="dc15f-435">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="dc15f-436">只读。</span><span class="sxs-lookup"><span data-stu-id="dc15f-436">Read Only.</span></span> <span data-ttu-id="dc15f-437">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="dc15f-437">This property is read-only.</span></span> <span data-ttu-id="dc15f-438">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="dc15f-438">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="dc15f-439">autopilotEnrolled</span><span class="sxs-lookup"><span data-stu-id="dc15f-439">autopilotEnrolled</span></span>|<span data-ttu-id="dc15f-440">布尔</span><span class="sxs-lookup"><span data-stu-id="dc15f-440">Boolean</span></span>|<span data-ttu-id="dc15f-441">如果托管设备是通过自动引导注册的，则报告。</span><span class="sxs-lookup"><span data-stu-id="dc15f-441">Reports if the managed device is enrolled via auto-pilot.</span></span> <span data-ttu-id="dc15f-442">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="dc15f-442">This property is read-only.</span></span> <span data-ttu-id="dc15f-443">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="dc15f-443">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="dc15f-444">requireUserEnrollmentApproval</span><span class="sxs-lookup"><span data-stu-id="dc15f-444">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="dc15f-445">布尔</span><span class="sxs-lookup"><span data-stu-id="dc15f-445">Boolean</span></span>|<span data-ttu-id="dc15f-446">如果托管 iOS 设备是用户审批注册，则报告。</span><span class="sxs-lookup"><span data-stu-id="dc15f-446">Reports if the managed iOS device is user approval enrollment.</span></span> <span data-ttu-id="dc15f-447">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="dc15f-447">This property is read-only.</span></span> <span data-ttu-id="dc15f-448">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="dc15f-448">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="dc15f-449">managementCertificateExpirationDate</span><span class="sxs-lookup"><span data-stu-id="dc15f-449">managementCertificateExpirationDate</span></span>|<span data-ttu-id="dc15f-450">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dc15f-450">DateTimeOffset</span></span>|<span data-ttu-id="dc15f-451">报告设备管理证书到期日期。</span><span class="sxs-lookup"><span data-stu-id="dc15f-451">Reports device management certificate expiration date.</span></span> <span data-ttu-id="dc15f-452">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="dc15f-452">This property is read-only.</span></span> <span data-ttu-id="dc15f-453">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="dc15f-453">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="dc15f-454">iccid</span><span class="sxs-lookup"><span data-stu-id="dc15f-454">iccid</span></span>|<span data-ttu-id="dc15f-455">String</span><span class="sxs-lookup"><span data-stu-id="dc15f-455">String</span></span>|<span data-ttu-id="dc15f-456">集成的电路卡标识符，它是 SIM 卡的唯一标识号。</span><span class="sxs-lookup"><span data-stu-id="dc15f-456">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span> <span data-ttu-id="dc15f-457">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="dc15f-457">This property is read-only.</span></span> <span data-ttu-id="dc15f-458">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="dc15f-458">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="dc15f-459">udid</span><span class="sxs-lookup"><span data-stu-id="dc15f-459">udid</span></span>|<span data-ttu-id="dc15f-460">String</span><span class="sxs-lookup"><span data-stu-id="dc15f-460">String</span></span>|<span data-ttu-id="dc15f-461">IOS 和 macOS 设备的唯一设备标识符。</span><span class="sxs-lookup"><span data-stu-id="dc15f-461">Unique Device Identifier for iOS and macOS devices.</span></span> <span data-ttu-id="dc15f-462">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="dc15f-462">This property is read-only.</span></span> <span data-ttu-id="dc15f-463">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="dc15f-463">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="dc15f-464">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="dc15f-464">roleScopeTagIds</span></span>|<span data-ttu-id="dc15f-465">String collection</span><span class="sxs-lookup"><span data-stu-id="dc15f-465">String collection</span></span>|<span data-ttu-id="dc15f-466">此设备实例的范围标记 Id 的列表。</span><span class="sxs-lookup"><span data-stu-id="dc15f-466">List of Scope Tag IDs for this Device instance.</span></span> <span data-ttu-id="dc15f-467">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="dc15f-467">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="dc15f-468">windowsActiveMalwareCount</span><span class="sxs-lookup"><span data-stu-id="dc15f-468">windowsActiveMalwareCount</span></span>|<span data-ttu-id="dc15f-469">Int32</span><span class="sxs-lookup"><span data-stu-id="dc15f-469">Int32</span></span>|<span data-ttu-id="dc15f-470">此 windows 设备的活动恶意软件的计数。</span><span class="sxs-lookup"><span data-stu-id="dc15f-470">Count of active malware for this windows device.</span></span> <span data-ttu-id="dc15f-471">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="dc15f-471">This property is read-only.</span></span> <span data-ttu-id="dc15f-472">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="dc15f-472">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="dc15f-473">windowsRemediatedMalwareCount</span><span class="sxs-lookup"><span data-stu-id="dc15f-473">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="dc15f-474">Int32</span><span class="sxs-lookup"><span data-stu-id="dc15f-474">Int32</span></span>|<span data-ttu-id="dc15f-475">此 windows 设备的修正的恶意软件的计数。</span><span class="sxs-lookup"><span data-stu-id="dc15f-475">Count of remediated malware for this windows device.</span></span> <span data-ttu-id="dc15f-476">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="dc15f-476">This property is read-only.</span></span> <span data-ttu-id="dc15f-477">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="dc15f-477">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="dc15f-478">notes</span><span class="sxs-lookup"><span data-stu-id="dc15f-478">notes</span></span>|<span data-ttu-id="dc15f-479">String</span><span class="sxs-lookup"><span data-stu-id="dc15f-479">String</span></span>|<span data-ttu-id="dc15f-480">由 IT 管理员创建的设备上的注释继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="dc15f-480">Notes on the device created by IT Admin Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="dc15f-481">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="dc15f-481">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="dc15f-482">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="dc15f-482">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="dc15f-483">Configuration manager 客户端运行状况状态，仅适用于从[ManagedDevice](../resources/intune-devices-manageddevice.md)继承的 MDM/ConfigMgr 代理所管理的设备</span><span class="sxs-lookup"><span data-stu-id="dc15f-483">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="dc15f-484">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="dc15f-484">configurationManagerClientInformation</span></span>|[<span data-ttu-id="dc15f-485">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="dc15f-485">configurationManagerClientInformation</span></span>](../resources/intune-devices-configurationmanagerclientinformation.md)|<span data-ttu-id="dc15f-486">Configuration manager 客户端信息，仅对由[ManagedDevice](../resources/intune-devices-manageddevice.md)继承的 ConfigMgr 代理、duel 管理或三方管理的设备有效</span><span class="sxs-lookup"><span data-stu-id="dc15f-486">Configuration manager client information, valid only for devices managed, duel-managed or tri-managed by ConfigMgr Agent Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="dc15f-487">ethernetMacAddress</span><span class="sxs-lookup"><span data-stu-id="dc15f-487">ethernetMacAddress</span></span>|<span data-ttu-id="dc15f-488">String</span><span class="sxs-lookup"><span data-stu-id="dc15f-488">String</span></span>|<span data-ttu-id="dc15f-489">以太网 MAC。</span><span class="sxs-lookup"><span data-stu-id="dc15f-489">Ethernet MAC.</span></span> <span data-ttu-id="dc15f-490">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="dc15f-490">This property is read-only.</span></span> <span data-ttu-id="dc15f-491">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="dc15f-491">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="dc15f-492">physicalMemoryInBytes</span><span class="sxs-lookup"><span data-stu-id="dc15f-492">physicalMemoryInBytes</span></span>|<span data-ttu-id="dc15f-493">Int64</span><span class="sxs-lookup"><span data-stu-id="dc15f-493">Int64</span></span>|<span data-ttu-id="dc15f-494">内存总量（以字节为单位）。</span><span class="sxs-lookup"><span data-stu-id="dc15f-494">Total Memory in Bytes.</span></span> <span data-ttu-id="dc15f-495">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="dc15f-495">This property is read-only.</span></span> <span data-ttu-id="dc15f-496">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="dc15f-496">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="dc15f-497">processorArchitecture</span><span class="sxs-lookup"><span data-stu-id="dc15f-497">processorArchitecture</span></span>|[<span data-ttu-id="dc15f-498">managedDeviceArchitecture</span><span class="sxs-lookup"><span data-stu-id="dc15f-498">managedDeviceArchitecture</span></span>](../resources/intune-devices-manageddevicearchitecture.md)|<span data-ttu-id="dc15f-499">处理器体系结构。</span><span class="sxs-lookup"><span data-stu-id="dc15f-499">Processor architecture.</span></span> <span data-ttu-id="dc15f-500">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="dc15f-500">This property is read-only.</span></span> <span data-ttu-id="dc15f-501">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="dc15f-501">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="dc15f-502">可取值为：`unknown`、`x86`、`x64`、`arm`、`arM64`。</span><span class="sxs-lookup"><span data-stu-id="dc15f-502">Possible values are: `unknown`, `x86`, `x64`, `arm`, `arM64`.</span></span>|
|<span data-ttu-id="dc15f-503">specificationVersion</span><span class="sxs-lookup"><span data-stu-id="dc15f-503">specificationVersion</span></span>|<span data-ttu-id="dc15f-504">String</span><span class="sxs-lookup"><span data-stu-id="dc15f-504">String</span></span>|<span data-ttu-id="dc15f-505">规范版本。</span><span class="sxs-lookup"><span data-stu-id="dc15f-505">Specification version.</span></span> <span data-ttu-id="dc15f-506">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="dc15f-506">This property is read-only.</span></span> <span data-ttu-id="dc15f-507">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="dc15f-507">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="dc15f-508">joinType</span><span class="sxs-lookup"><span data-stu-id="dc15f-508">joinType</span></span>|[<span data-ttu-id="dc15f-509">joinType</span><span class="sxs-lookup"><span data-stu-id="dc15f-509">joinType</span></span>](../resources/intune-devices-jointype.md)|<span data-ttu-id="dc15f-510">从 [ManagedDevice](../resources/intune-devices-manageddevice.md)继承的设备联接类型。</span><span class="sxs-lookup"><span data-stu-id="dc15f-510">Device join type Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="dc15f-511">可取值为：`unknown`、`azureADJoined`、`azureADRegistered`、`hybridAzureADJoined`。</span><span class="sxs-lookup"><span data-stu-id="dc15f-511">Possible values are: `unknown`, `azureADJoined`, `azureADRegistered`, `hybridAzureADJoined`.</span></span>|
|<span data-ttu-id="dc15f-512">skuFamily</span><span class="sxs-lookup"><span data-stu-id="dc15f-512">skuFamily</span></span>|<span data-ttu-id="dc15f-513">String</span><span class="sxs-lookup"><span data-stu-id="dc15f-513">String</span></span>|<span data-ttu-id="dc15f-514">从[ManagedDevice](../resources/intune-devices-manageddevice.md)继承的设备 sku 系列</span><span class="sxs-lookup"><span data-stu-id="dc15f-514">Device sku family Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="dc15f-515">skuNumber</span><span class="sxs-lookup"><span data-stu-id="dc15f-515">skuNumber</span></span>|<span data-ttu-id="dc15f-516">Int32</span><span class="sxs-lookup"><span data-stu-id="dc15f-516">Int32</span></span>|<span data-ttu-id="dc15f-517">设备 sku 编号，另请参阅： https://docs.microsoft.com/windows/win32/api/sysinfoapi/nf-sysinfoapi-getproductinfo 。</span><span class="sxs-lookup"><span data-stu-id="dc15f-517">Device sku number, see also: https://docs.microsoft.com/windows/win32/api/sysinfoapi/nf-sysinfoapi-getproductinfo.</span></span> <span data-ttu-id="dc15f-518">有效的值为0到2147483647。</span><span class="sxs-lookup"><span data-stu-id="dc15f-518">Valid values 0 to 2147483647.</span></span> <span data-ttu-id="dc15f-519">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="dc15f-519">This property is read-only.</span></span> <span data-ttu-id="dc15f-520">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="dc15f-520">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="dc15f-521">managementFeatures</span><span class="sxs-lookup"><span data-stu-id="dc15f-521">managementFeatures</span></span>|[<span data-ttu-id="dc15f-522">managedDeviceManagementFeatures</span><span class="sxs-lookup"><span data-stu-id="dc15f-522">managedDeviceManagementFeatures</span></span>](../resources/intune-devices-manageddevicemanagementfeatures.md)|<span data-ttu-id="dc15f-523">从 [ManagedDevice](../resources/intune-devices-manageddevice.md)继承的设备管理功能。</span><span class="sxs-lookup"><span data-stu-id="dc15f-523">Device management features Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="dc15f-524">可取值为：`none`、`microsoftManagedDesktop`。</span><span class="sxs-lookup"><span data-stu-id="dc15f-524">Possible values are: `none`, `microsoftManagedDesktop`.</span></span>|



## <a name="response"></a><span data-ttu-id="dc15f-525">响应</span><span class="sxs-lookup"><span data-stu-id="dc15f-525">Response</span></span>
<span data-ttu-id="dc15f-526">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="dc15f-526">If successful, this method returns a `200 OK` response code and an updated [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dc15f-527">示例</span><span class="sxs-lookup"><span data-stu-id="dc15f-527">Example</span></span>

### <a name="request"></a><span data-ttu-id="dc15f-528">请求</span><span class="sxs-lookup"><span data-stu-id="dc15f-528">Request</span></span>
<span data-ttu-id="dc15f-529">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="dc15f-529">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="dc15f-530">响应</span><span class="sxs-lookup"><span data-stu-id="dc15f-530">Response</span></span>
<span data-ttu-id="dc15f-p175">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="dc15f-p175">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





