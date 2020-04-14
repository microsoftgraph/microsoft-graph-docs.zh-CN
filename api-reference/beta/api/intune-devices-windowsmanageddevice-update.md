---
title: 更新 windowsManagedDevice
description: 更新 windowsManagedDevice 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f7d0f3c30a8a434b595bb1c05393d53e601ba1a2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43378381"
---
# <a name="update-windowsmanageddevice"></a><span data-ttu-id="6efa5-103">更新 windowsManagedDevice</span><span class="sxs-lookup"><span data-stu-id="6efa5-103">Update windowsManagedDevice</span></span>

<span data-ttu-id="6efa5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6efa5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6efa5-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6efa5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6efa5-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6efa5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6efa5-107">更新[windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6efa5-107">Update the properties of a [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6efa5-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="6efa5-108">Prerequisites</span></span>
<span data-ttu-id="6efa5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6efa5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6efa5-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6efa5-111">Permission type</span></span>|<span data-ttu-id="6efa5-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6efa5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6efa5-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6efa5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6efa5-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6efa5-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="6efa5-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6efa5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6efa5-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6efa5-116">Not supported.</span></span>|
|<span data-ttu-id="6efa5-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="6efa5-117">Application</span></span>|<span data-ttu-id="6efa5-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6efa5-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6efa5-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6efa5-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="6efa5-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6efa5-120">Request headers</span></span>
|<span data-ttu-id="6efa5-121">标头</span><span class="sxs-lookup"><span data-stu-id="6efa5-121">Header</span></span>|<span data-ttu-id="6efa5-122">值</span><span class="sxs-lookup"><span data-stu-id="6efa5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6efa5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6efa5-123">Authorization</span></span>|<span data-ttu-id="6efa5-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6efa5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6efa5-125">接受</span><span class="sxs-lookup"><span data-stu-id="6efa5-125">Accept</span></span>|<span data-ttu-id="6efa5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6efa5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6efa5-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6efa5-127">Request body</span></span>
<span data-ttu-id="6efa5-128">在请求正文中，提供[windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6efa5-128">In the request body, supply a JSON representation for the [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object.</span></span>

<span data-ttu-id="6efa5-129">下表显示创建[windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6efa5-129">The following table shows the properties that are required when you create the [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md).</span></span>

|<span data-ttu-id="6efa5-130">属性</span><span class="sxs-lookup"><span data-stu-id="6efa5-130">Property</span></span>|<span data-ttu-id="6efa5-131">类型</span><span class="sxs-lookup"><span data-stu-id="6efa5-131">Type</span></span>|<span data-ttu-id="6efa5-132">说明</span><span class="sxs-lookup"><span data-stu-id="6efa5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6efa5-133">id</span><span class="sxs-lookup"><span data-stu-id="6efa5-133">id</span></span>|<span data-ttu-id="6efa5-134">字符串</span><span class="sxs-lookup"><span data-stu-id="6efa5-134">String</span></span>|<span data-ttu-id="6efa5-135">设备的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="6efa5-135">Unique Identifier for the device.</span></span> <span data-ttu-id="6efa5-136">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6efa5-136">This property is read-only.</span></span> <span data-ttu-id="6efa5-137">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6efa5-137">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6efa5-138">userId</span><span class="sxs-lookup"><span data-stu-id="6efa5-138">userId</span></span>|<span data-ttu-id="6efa5-139">String</span><span class="sxs-lookup"><span data-stu-id="6efa5-139">String</span></span>|<span data-ttu-id="6efa5-140">与设备关联的用户的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="6efa5-140">Unique Identifier for the user associated with the device.</span></span> <span data-ttu-id="6efa5-141">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6efa5-141">This property is read-only.</span></span> <span data-ttu-id="6efa5-142">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6efa5-142">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6efa5-143">deviceName</span><span class="sxs-lookup"><span data-stu-id="6efa5-143">deviceName</span></span>|<span data-ttu-id="6efa5-144">字符串</span><span class="sxs-lookup"><span data-stu-id="6efa5-144">String</span></span>|<span data-ttu-id="6efa5-145">设备的名称。</span><span class="sxs-lookup"><span data-stu-id="6efa5-145">Name of the device.</span></span> <span data-ttu-id="6efa5-146">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6efa5-146">This property is read-only.</span></span> <span data-ttu-id="6efa5-147">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6efa5-147">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6efa5-148">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="6efa5-148">hardwareInformation</span></span>|[<span data-ttu-id="6efa5-149">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="6efa5-149">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="6efa5-150">设备的 hardward 详细信息。</span><span class="sxs-lookup"><span data-stu-id="6efa5-150">The hardward details for the device.</span></span>  <span data-ttu-id="6efa5-151">包括存储空间、制造商、序列号等信息。此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6efa5-151">Includes information such as storage space, manufacturer, serial number, etc. This property is read-only.</span></span> <span data-ttu-id="6efa5-152">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6efa5-152">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6efa5-153">所有者</span><span class="sxs-lookup"><span data-stu-id="6efa5-153">ownerType</span></span>|[<span data-ttu-id="6efa5-154">所有者</span><span class="sxs-lookup"><span data-stu-id="6efa5-154">ownerType</span></span>](../resources/intune-shared-ownertype.md)|<span data-ttu-id="6efa5-155">设备的所有权。</span><span class="sxs-lookup"><span data-stu-id="6efa5-155">Ownership of the device.</span></span> <span data-ttu-id="6efa5-156">可以是从[ManagedDevice](../resources/intune-devices-manageddevice.md)继承的 "公司" 或 "个人"。</span><span class="sxs-lookup"><span data-stu-id="6efa5-156">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="6efa5-157">可取值为：`unknown`、`company`、`personal`。</span><span class="sxs-lookup"><span data-stu-id="6efa5-157">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="6efa5-158">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="6efa5-158">managedDeviceOwnerType</span></span>|[<span data-ttu-id="6efa5-159">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="6efa5-159">managedDeviceOwnerType</span></span>](../resources/intune-shared-manageddeviceownertype.md)|<span data-ttu-id="6efa5-160">设备的所有权。</span><span class="sxs-lookup"><span data-stu-id="6efa5-160">Ownership of the device.</span></span> <span data-ttu-id="6efa5-161">可以是从[ManagedDevice](../resources/intune-devices-manageddevice.md)继承的 "公司" 或 "个人"。</span><span class="sxs-lookup"><span data-stu-id="6efa5-161">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="6efa5-162">可取值为：`unknown`、`company`、`personal`。</span><span class="sxs-lookup"><span data-stu-id="6efa5-162">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="6efa5-163">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="6efa5-163">deviceActionResults</span></span>|<span data-ttu-id="6efa5-164">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6efa5-164">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="6efa5-165">ComplexType deviceActionResult 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="6efa5-165">List of ComplexType deviceActionResult objects.</span></span> <span data-ttu-id="6efa5-166">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6efa5-166">This property is read-only.</span></span> <span data-ttu-id="6efa5-167">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6efa5-167">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6efa5-168">managementState</span><span class="sxs-lookup"><span data-stu-id="6efa5-168">managementState</span></span>|[<span data-ttu-id="6efa5-169">managementState</span><span class="sxs-lookup"><span data-stu-id="6efa5-169">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="6efa5-170">设备的管理状态。</span><span class="sxs-lookup"><span data-stu-id="6efa5-170">Management state of the device.</span></span> <span data-ttu-id="6efa5-171">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6efa5-171">This property is read-only.</span></span> <span data-ttu-id="6efa5-172">继承自[managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="6efa5-172">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="6efa5-173">可取值为：`managed`、`retirePending`、`retireFailed`、`wipePending`、`wipeFailed`、`unhealthy`、`deletePending`、`retireIssued`、`wipeIssued`、`wipeCanceled`、`retireCanceled`、`discovered`。</span><span class="sxs-lookup"><span data-stu-id="6efa5-173">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="6efa5-174">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="6efa5-174">enrolledDateTime</span></span>|<span data-ttu-id="6efa5-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6efa5-175">DateTimeOffset</span></span>|<span data-ttu-id="6efa5-176">设备的注册时间。</span><span class="sxs-lookup"><span data-stu-id="6efa5-176">Enrollment time of the device.</span></span> <span data-ttu-id="6efa5-177">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6efa5-177">This property is read-only.</span></span> <span data-ttu-id="6efa5-178">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6efa5-178">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6efa5-179">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="6efa5-179">lastSyncDateTime</span></span>|<span data-ttu-id="6efa5-180">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6efa5-180">DateTimeOffset</span></span>|<span data-ttu-id="6efa5-181">设备上次成功完成与 Intune 同步的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="6efa5-181">The date and time that the device last completed a successful sync with Intune.</span></span> <span data-ttu-id="6efa5-182">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6efa5-182">This property is read-only.</span></span> <span data-ttu-id="6efa5-183">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6efa5-183">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6efa5-184">chassisType</span><span class="sxs-lookup"><span data-stu-id="6efa5-184">chassisType</span></span>|[<span data-ttu-id="6efa5-185">chassisType</span><span class="sxs-lookup"><span data-stu-id="6efa5-185">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="6efa5-186">设备的机箱类型。</span><span class="sxs-lookup"><span data-stu-id="6efa5-186">Chassis type of the device.</span></span> <span data-ttu-id="6efa5-187">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6efa5-187">This property is read-only.</span></span> <span data-ttu-id="6efa5-188">继承自[managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="6efa5-188">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="6efa5-189">可取值为：`unknown`、`desktop`、`laptop`、`worksWorkstation`、`enterpriseServer`、`phone`、`tablet`、`mobileOther`、`mobileUnknown`。</span><span class="sxs-lookup"><span data-stu-id="6efa5-189">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="6efa5-190">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="6efa5-190">operatingSystem</span></span>|<span data-ttu-id="6efa5-191">字符串</span><span class="sxs-lookup"><span data-stu-id="6efa5-191">String</span></span>|<span data-ttu-id="6efa5-192">设备的操作系统。</span><span class="sxs-lookup"><span data-stu-id="6efa5-192">Operating system of the device.</span></span> <span data-ttu-id="6efa5-193">Windows、iOS 等。此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6efa5-193">Windows, iOS, etc. This property is read-only.</span></span> <span data-ttu-id="6efa5-194">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6efa5-194">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6efa5-195">deviceType</span><span class="sxs-lookup"><span data-stu-id="6efa5-195">deviceType</span></span>|[<span data-ttu-id="6efa5-196">deviceType</span><span class="sxs-lookup"><span data-stu-id="6efa5-196">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="6efa5-197">设备的平台。</span><span class="sxs-lookup"><span data-stu-id="6efa5-197">Platform of the device.</span></span> <span data-ttu-id="6efa5-198">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6efa5-198">This property is read-only.</span></span> <span data-ttu-id="6efa5-199">继承自[managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="6efa5-199">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="6efa5-200">可能的值为`desktop`： `windowsRT`、 `winMO6`、 `nokia` `windowsPhone` `mac` `winCE` `palm` `unknown`、、、、、、、、、、、、、、、、、、、、。 `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `windows10x` `blackberry`</span><span class="sxs-lookup"><span data-stu-id="6efa5-200">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="6efa5-201">complianceState</span><span class="sxs-lookup"><span data-stu-id="6efa5-201">complianceState</span></span>|[<span data-ttu-id="6efa5-202">complianceState</span><span class="sxs-lookup"><span data-stu-id="6efa5-202">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="6efa5-203">设备的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="6efa5-203">Compliance state of the device.</span></span> <span data-ttu-id="6efa5-204">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6efa5-204">This property is read-only.</span></span> <span data-ttu-id="6efa5-205">继承自[managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="6efa5-205">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="6efa5-206">可取值为：`unknown`、`compliant`、`noncompliant`、`conflict`、`error`、`inGracePeriod`、`configManager`。</span><span class="sxs-lookup"><span data-stu-id="6efa5-206">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="6efa5-207">jailBroken</span><span class="sxs-lookup"><span data-stu-id="6efa5-207">jailBroken</span></span>|<span data-ttu-id="6efa5-208">String</span><span class="sxs-lookup"><span data-stu-id="6efa5-208">String</span></span>|<span data-ttu-id="6efa5-209">设备是否已越狱或取得 root 权限。</span><span class="sxs-lookup"><span data-stu-id="6efa5-209">whether the device is jail broken or rooted.</span></span> <span data-ttu-id="6efa5-210">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6efa5-210">This property is read-only.</span></span> <span data-ttu-id="6efa5-211">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6efa5-211">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6efa5-212">managementAgent</span><span class="sxs-lookup"><span data-stu-id="6efa5-212">managementAgent</span></span>|[<span data-ttu-id="6efa5-213">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="6efa5-213">managementAgentType</span></span>](../resources/intune-shared-managementagenttype.md)|<span data-ttu-id="6efa5-214">设备的管理通道。</span><span class="sxs-lookup"><span data-stu-id="6efa5-214">Management channel of the device.</span></span> <span data-ttu-id="6efa5-215">Intune、EAS 等。此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6efa5-215">Intune, EAS, etc. This property is read-only.</span></span> <span data-ttu-id="6efa5-216">继承自[managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="6efa5-216">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="6efa5-217">可能的值是：`eas`、`mdm`、`easMdm`、`intuneClient`、`easIntuneClient`、`configurationManagerClient`、`configurationManagerClientMdm`、`configurationManagerClientMdmEas`、`unknown`、`jamf`、`googleCloudDevicePolicyController`、`microsoft365ManagedMdm`、`windowsManagementCloudApi`。</span><span class="sxs-lookup"><span data-stu-id="6efa5-217">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`, `windowsManagementCloudApi`.</span></span>|
|<span data-ttu-id="6efa5-218">osVersion</span><span class="sxs-lookup"><span data-stu-id="6efa5-218">osVersion</span></span>|<span data-ttu-id="6efa5-219">String</span><span class="sxs-lookup"><span data-stu-id="6efa5-219">String</span></span>|<span data-ttu-id="6efa5-220">设备的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="6efa5-220">Operating system version of the device.</span></span> <span data-ttu-id="6efa5-221">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6efa5-221">This property is read-only.</span></span> <span data-ttu-id="6efa5-222">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6efa5-222">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6efa5-223">easActivated</span><span class="sxs-lookup"><span data-stu-id="6efa5-223">easActivated</span></span>|<span data-ttu-id="6efa5-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="6efa5-224">Boolean</span></span>|<span data-ttu-id="6efa5-225">设备是否已激活 Exchange ActiveSync。</span><span class="sxs-lookup"><span data-stu-id="6efa5-225">Whether the device is Exchange ActiveSync activated.</span></span> <span data-ttu-id="6efa5-226">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6efa5-226">This property is read-only.</span></span> <span data-ttu-id="6efa5-227">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6efa5-227">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6efa5-228">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="6efa5-228">easDeviceId</span></span>|<span data-ttu-id="6efa5-229">字符串</span><span class="sxs-lookup"><span data-stu-id="6efa5-229">String</span></span>|<span data-ttu-id="6efa5-230">设备的 Exchange ActiveSync ID。</span><span class="sxs-lookup"><span data-stu-id="6efa5-230">Exchange ActiveSync Id of the device.</span></span> <span data-ttu-id="6efa5-231">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6efa5-231">This property is read-only.</span></span> <span data-ttu-id="6efa5-232">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6efa5-232">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6efa5-233">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="6efa5-233">easActivationDateTime</span></span>|<span data-ttu-id="6efa5-234">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6efa5-234">DateTimeOffset</span></span>|<span data-ttu-id="6efa5-235">设备的 Exchange ActivationSync 激活时间。</span><span class="sxs-lookup"><span data-stu-id="6efa5-235">Exchange ActivationSync activation time of the device.</span></span> <span data-ttu-id="6efa5-236">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6efa5-236">This property is read-only.</span></span> <span data-ttu-id="6efa5-237">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6efa5-237">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6efa5-238">aadRegistered</span><span class="sxs-lookup"><span data-stu-id="6efa5-238">aadRegistered</span></span>|<span data-ttu-id="6efa5-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="6efa5-239">Boolean</span></span>|<span data-ttu-id="6efa5-240">设备是否已注册 Azure Active Directory。</span><span class="sxs-lookup"><span data-stu-id="6efa5-240">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="6efa5-241">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6efa5-241">This property is read-only.</span></span> <span data-ttu-id="6efa5-242">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6efa5-242">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6efa5-243">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="6efa5-243">azureADRegistered</span></span>|<span data-ttu-id="6efa5-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="6efa5-244">Boolean</span></span>|<span data-ttu-id="6efa5-245">设备是否已注册 Azure Active Directory。</span><span class="sxs-lookup"><span data-stu-id="6efa5-245">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="6efa5-246">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6efa5-246">This property is read-only.</span></span> <span data-ttu-id="6efa5-247">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6efa5-247">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6efa5-248">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="6efa5-248">deviceEnrollmentType</span></span>|[<span data-ttu-id="6efa5-249">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="6efa5-249">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="6efa5-250">设备的注册类型。</span><span class="sxs-lookup"><span data-stu-id="6efa5-250">Enrollment type of the device.</span></span> <span data-ttu-id="6efa5-251">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6efa5-251">This property is read-only.</span></span> <span data-ttu-id="6efa5-252">继承自[managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="6efa5-252">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="6efa5-253">可能的值是：`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement`、`appleUserEnrollment`、`appleUserEnrollmentWithServiceAccount`、`azureAdJoinUsingAzureVmExtension`。</span><span class="sxs-lookup"><span data-stu-id="6efa5-253">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`, `azureAdJoinUsingAzureVmExtension`.</span></span>|
|<span data-ttu-id="6efa5-254">lostModeState</span><span class="sxs-lookup"><span data-stu-id="6efa5-254">lostModeState</span></span>|[<span data-ttu-id="6efa5-255">lostModeState</span><span class="sxs-lookup"><span data-stu-id="6efa5-255">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="6efa5-256">指示是否已启用或禁用了丢失模式。</span><span class="sxs-lookup"><span data-stu-id="6efa5-256">Indicates if Lost mode is enabled or disabled.</span></span> <span data-ttu-id="6efa5-257">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6efa5-257">This property is read-only.</span></span> <span data-ttu-id="6efa5-258">继承自[managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="6efa5-258">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="6efa5-259">可取值为：`disabled`、`enabled`。</span><span class="sxs-lookup"><span data-stu-id="6efa5-259">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="6efa5-260">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="6efa5-260">activationLockBypassCode</span></span>|<span data-ttu-id="6efa5-261">字符串</span><span class="sxs-lookup"><span data-stu-id="6efa5-261">String</span></span>|<span data-ttu-id="6efa5-262">允许绕过设备上的激活锁的代码。</span><span class="sxs-lookup"><span data-stu-id="6efa5-262">Code that allows the Activation Lock on a device to be bypassed.</span></span> <span data-ttu-id="6efa5-263">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6efa5-263">This property is read-only.</span></span> <span data-ttu-id="6efa5-264">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6efa5-264">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6efa5-265">emailAddress</span><span class="sxs-lookup"><span data-stu-id="6efa5-265">emailAddress</span></span>|<span data-ttu-id="6efa5-266">字符串</span><span class="sxs-lookup"><span data-stu-id="6efa5-266">String</span></span>|<span data-ttu-id="6efa5-267">与设备关联的用户的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="6efa5-267">Email(s) for the user associated with the device.</span></span> <span data-ttu-id="6efa5-268">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6efa5-268">This property is read-only.</span></span> <span data-ttu-id="6efa5-269">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6efa5-269">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6efa5-270">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="6efa5-270">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="6efa5-271">字符串</span><span class="sxs-lookup"><span data-stu-id="6efa5-271">String</span></span>|<span data-ttu-id="6efa5-272">Azure Active Directory 设备的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="6efa5-272">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="6efa5-273">只读。</span><span class="sxs-lookup"><span data-stu-id="6efa5-273">Read only.</span></span> <span data-ttu-id="6efa5-274">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6efa5-274">This property is read-only.</span></span> <span data-ttu-id="6efa5-275">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6efa5-275">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6efa5-276">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="6efa5-276">azureADDeviceId</span></span>|<span data-ttu-id="6efa5-277">字符串</span><span class="sxs-lookup"><span data-stu-id="6efa5-277">String</span></span>|<span data-ttu-id="6efa5-278">Azure Active Directory 设备的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="6efa5-278">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="6efa5-279">只读。</span><span class="sxs-lookup"><span data-stu-id="6efa5-279">Read only.</span></span> <span data-ttu-id="6efa5-280">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6efa5-280">This property is read-only.</span></span> <span data-ttu-id="6efa5-281">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6efa5-281">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6efa5-282">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="6efa5-282">deviceRegistrationState</span></span>|[<span data-ttu-id="6efa5-283">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="6efa5-283">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="6efa5-284">设备注册状态。</span><span class="sxs-lookup"><span data-stu-id="6efa5-284">Device registration state.</span></span> <span data-ttu-id="6efa5-285">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6efa5-285">This property is read-only.</span></span> <span data-ttu-id="6efa5-286">继承自[managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="6efa5-286">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="6efa5-287">可取值为：`notRegistered`、`registered`、`revoked`、`keyConflict`、`approvalPending`、`certificateReset`、`notRegisteredPendingEnrollment`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="6efa5-287">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="6efa5-288">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="6efa5-288">deviceCategoryDisplayName</span></span>|<span data-ttu-id="6efa5-289">字符串</span><span class="sxs-lookup"><span data-stu-id="6efa5-289">String</span></span>|<span data-ttu-id="6efa5-290">设备类别显示名称。</span><span class="sxs-lookup"><span data-stu-id="6efa5-290">Device category display name.</span></span> <span data-ttu-id="6efa5-291">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6efa5-291">This property is read-only.</span></span> <span data-ttu-id="6efa5-292">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6efa5-292">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6efa5-293">isSupervised</span><span class="sxs-lookup"><span data-stu-id="6efa5-293">isSupervised</span></span>|<span data-ttu-id="6efa5-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="6efa5-294">Boolean</span></span>|<span data-ttu-id="6efa5-295">设备监督状态。</span><span class="sxs-lookup"><span data-stu-id="6efa5-295">Device supervised status.</span></span> <span data-ttu-id="6efa5-296">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6efa5-296">This property is read-only.</span></span> <span data-ttu-id="6efa5-297">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6efa5-297">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6efa5-298">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="6efa5-298">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="6efa5-299">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6efa5-299">DateTimeOffset</span></span>|<span data-ttu-id="6efa5-300">设备上次与 Exchange 联系的时间。</span><span class="sxs-lookup"><span data-stu-id="6efa5-300">Last time the device contacted Exchange.</span></span> <span data-ttu-id="6efa5-301">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6efa5-301">This property is read-only.</span></span> <span data-ttu-id="6efa5-302">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6efa5-302">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6efa5-303">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="6efa5-303">exchangeAccessState</span></span>|[<span data-ttu-id="6efa5-304">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="6efa5-304">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="6efa5-305">Exchange 中设备的访问状态。</span><span class="sxs-lookup"><span data-stu-id="6efa5-305">The Access State of the device in Exchange.</span></span> <span data-ttu-id="6efa5-306">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6efa5-306">This property is read-only.</span></span> <span data-ttu-id="6efa5-307">继承自[managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="6efa5-307">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="6efa5-308">可取值为：`none`、`unknown`、`allowed`、`blocked`、`quarantined`。</span><span class="sxs-lookup"><span data-stu-id="6efa5-308">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="6efa5-309">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="6efa5-309">exchangeAccessStateReason</span></span>|[<span data-ttu-id="6efa5-310">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="6efa5-310">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="6efa5-311">Exchange 中设备访问状态的出现原因。</span><span class="sxs-lookup"><span data-stu-id="6efa5-311">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="6efa5-312">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6efa5-312">This property is read-only.</span></span> <span data-ttu-id="6efa5-313">继承自[managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="6efa5-313">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="6efa5-314">可取值为：`none`、`unknown`、`exchangeGlobalRule`、`exchangeIndividualRule`、`exchangeDeviceRule`、`exchangeUpgrade`、`exchangeMailboxPolicy`、`other`、`compliant`、`notCompliant`、`notEnrolled`、`unknownLocation`、`mfaRequired`、`azureADBlockDueToAccessPolicy`、`compromisedPassword`、`deviceNotKnownWithManagedApp`。</span><span class="sxs-lookup"><span data-stu-id="6efa5-314">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="6efa5-315">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="6efa5-315">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="6efa5-316">字符串</span><span class="sxs-lookup"><span data-stu-id="6efa5-316">String</span></span>|<span data-ttu-id="6efa5-317">允许与设备建立远程协助会话的 URL。</span><span class="sxs-lookup"><span data-stu-id="6efa5-317">Url that allows a Remote Assistance session to be established with the device.</span></span> <span data-ttu-id="6efa5-318">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6efa5-318">This property is read-only.</span></span> <span data-ttu-id="6efa5-319">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6efa5-319">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6efa5-320">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="6efa5-320">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="6efa5-321">String</span><span class="sxs-lookup"><span data-stu-id="6efa5-321">String</span></span>|<span data-ttu-id="6efa5-322">用于在创建远程协助会话对象时识别问题的错误字符串。</span><span class="sxs-lookup"><span data-stu-id="6efa5-322">An error string that identifies issues when creating Remote Assistance session objects.</span></span> <span data-ttu-id="6efa5-323">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6efa5-323">This property is read-only.</span></span> <span data-ttu-id="6efa5-324">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6efa5-324">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6efa5-325">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="6efa5-325">isEncrypted</span></span>|<span data-ttu-id="6efa5-326">Boolean</span><span class="sxs-lookup"><span data-stu-id="6efa5-326">Boolean</span></span>|<span data-ttu-id="6efa5-327">设备加密状态。</span><span class="sxs-lookup"><span data-stu-id="6efa5-327">Device encryption status.</span></span> <span data-ttu-id="6efa5-328">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6efa5-328">This property is read-only.</span></span> <span data-ttu-id="6efa5-329">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6efa5-329">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6efa5-330">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="6efa5-330">userPrincipalName</span></span>|<span data-ttu-id="6efa5-331">字符串</span><span class="sxs-lookup"><span data-stu-id="6efa5-331">String</span></span>|<span data-ttu-id="6efa5-332">设备用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="6efa5-332">Device user principal name.</span></span> <span data-ttu-id="6efa5-333">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6efa5-333">This property is read-only.</span></span> <span data-ttu-id="6efa5-334">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6efa5-334">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6efa5-335">model</span><span class="sxs-lookup"><span data-stu-id="6efa5-335">model</span></span>|<span data-ttu-id="6efa5-336">字符串</span><span class="sxs-lookup"><span data-stu-id="6efa5-336">String</span></span>|<span data-ttu-id="6efa5-337">设备的模型。</span><span class="sxs-lookup"><span data-stu-id="6efa5-337">Model of the device.</span></span> <span data-ttu-id="6efa5-338">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6efa5-338">This property is read-only.</span></span> <span data-ttu-id="6efa5-339">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6efa5-339">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6efa5-340">manufacturer</span><span class="sxs-lookup"><span data-stu-id="6efa5-340">manufacturer</span></span>|<span data-ttu-id="6efa5-341">字符串</span><span class="sxs-lookup"><span data-stu-id="6efa5-341">String</span></span>|<span data-ttu-id="6efa5-342">设备的制造商。</span><span class="sxs-lookup"><span data-stu-id="6efa5-342">Manufacturer of the device.</span></span> <span data-ttu-id="6efa5-343">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6efa5-343">This property is read-only.</span></span> <span data-ttu-id="6efa5-344">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6efa5-344">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6efa5-345">imei</span><span class="sxs-lookup"><span data-stu-id="6efa5-345">imei</span></span>|<span data-ttu-id="6efa5-346">字符串</span><span class="sxs-lookup"><span data-stu-id="6efa5-346">String</span></span>|<span data-ttu-id="6efa5-347">IMEI.</span><span class="sxs-lookup"><span data-stu-id="6efa5-347">IMEI.</span></span> <span data-ttu-id="6efa5-348">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6efa5-348">This property is read-only.</span></span> <span data-ttu-id="6efa5-349">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6efa5-349">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6efa5-350">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="6efa5-350">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="6efa5-351">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6efa5-351">DateTimeOffset</span></span>|<span data-ttu-id="6efa5-352">设备符合性宽限期到期时的日期时间。</span><span class="sxs-lookup"><span data-stu-id="6efa5-352">The DateTime when device compliance grace period expires.</span></span> <span data-ttu-id="6efa5-353">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6efa5-353">This property is read-only.</span></span> <span data-ttu-id="6efa5-354">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6efa5-354">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6efa5-355">serialNumber</span><span class="sxs-lookup"><span data-stu-id="6efa5-355">serialNumber</span></span>|<span data-ttu-id="6efa5-356">字符串</span><span class="sxs-lookup"><span data-stu-id="6efa5-356">String</span></span>|<span data-ttu-id="6efa5-357">SerialNumber.</span><span class="sxs-lookup"><span data-stu-id="6efa5-357">SerialNumber.</span></span> <span data-ttu-id="6efa5-358">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6efa5-358">This property is read-only.</span></span> <span data-ttu-id="6efa5-359">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6efa5-359">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6efa5-360">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="6efa5-360">phoneNumber</span></span>|<span data-ttu-id="6efa5-361">字符串</span><span class="sxs-lookup"><span data-stu-id="6efa5-361">String</span></span>|<span data-ttu-id="6efa5-362">设备的电话号码。</span><span class="sxs-lookup"><span data-stu-id="6efa5-362">Phone number of the device.</span></span> <span data-ttu-id="6efa5-363">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6efa5-363">This property is read-only.</span></span> <span data-ttu-id="6efa5-364">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6efa5-364">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6efa5-365">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="6efa5-365">androidSecurityPatchLevel</span></span>|<span data-ttu-id="6efa5-366">字符串</span><span class="sxs-lookup"><span data-stu-id="6efa5-366">String</span></span>|<span data-ttu-id="6efa5-367">Android 安全修补程序级别。</span><span class="sxs-lookup"><span data-stu-id="6efa5-367">Android security patch level.</span></span> <span data-ttu-id="6efa5-368">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6efa5-368">This property is read-only.</span></span> <span data-ttu-id="6efa5-369">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6efa5-369">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6efa5-370">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="6efa5-370">userDisplayName</span></span>|<span data-ttu-id="6efa5-371">String</span><span class="sxs-lookup"><span data-stu-id="6efa5-371">String</span></span>|<span data-ttu-id="6efa5-372">用户显示名称。</span><span class="sxs-lookup"><span data-stu-id="6efa5-372">User display name.</span></span> <span data-ttu-id="6efa5-373">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6efa5-373">This property is read-only.</span></span> <span data-ttu-id="6efa5-374">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6efa5-374">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6efa5-375">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="6efa5-375">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="6efa5-376">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="6efa5-376">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="6efa5-377">ConfigrMgr 客户端启用的功能。</span><span class="sxs-lookup"><span data-stu-id="6efa5-377">ConfigrMgr client enabled features.</span></span> <span data-ttu-id="6efa5-378">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6efa5-378">This property is read-only.</span></span> <span data-ttu-id="6efa5-379">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6efa5-379">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6efa5-380">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="6efa5-380">wiFiMacAddress</span></span>|<span data-ttu-id="6efa5-381">字符串</span><span class="sxs-lookup"><span data-stu-id="6efa5-381">String</span></span>|<span data-ttu-id="6efa5-382">Wi-fi MAC。</span><span class="sxs-lookup"><span data-stu-id="6efa5-382">Wi-Fi MAC.</span></span> <span data-ttu-id="6efa5-383">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6efa5-383">This property is read-only.</span></span> <span data-ttu-id="6efa5-384">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6efa5-384">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6efa5-385">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="6efa5-385">deviceHealthAttestationState</span></span>|[<span data-ttu-id="6efa5-386">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="6efa5-386">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="6efa5-387">设备运行状况证明状态。</span><span class="sxs-lookup"><span data-stu-id="6efa5-387">The device health attestation state.</span></span> <span data-ttu-id="6efa5-388">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6efa5-388">This property is read-only.</span></span> <span data-ttu-id="6efa5-389">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6efa5-389">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6efa5-390">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="6efa5-390">subscriberCarrier</span></span>|<span data-ttu-id="6efa5-391">字符串</span><span class="sxs-lookup"><span data-stu-id="6efa5-391">String</span></span>|<span data-ttu-id="6efa5-392">订阅者运营商。</span><span class="sxs-lookup"><span data-stu-id="6efa5-392">Subscriber Carrier.</span></span> <span data-ttu-id="6efa5-393">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6efa5-393">This property is read-only.</span></span> <span data-ttu-id="6efa5-394">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6efa5-394">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6efa5-395">meid</span><span class="sxs-lookup"><span data-stu-id="6efa5-395">meid</span></span>|<span data-ttu-id="6efa5-396">字符串</span><span class="sxs-lookup"><span data-stu-id="6efa5-396">String</span></span>|<span data-ttu-id="6efa5-397">MEID.</span><span class="sxs-lookup"><span data-stu-id="6efa5-397">MEID.</span></span> <span data-ttu-id="6efa5-398">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6efa5-398">This property is read-only.</span></span> <span data-ttu-id="6efa5-399">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6efa5-399">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6efa5-400">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="6efa5-400">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="6efa5-401">Int64</span><span class="sxs-lookup"><span data-stu-id="6efa5-401">Int64</span></span>|<span data-ttu-id="6efa5-402">总存储量（以字节为单位）。</span><span class="sxs-lookup"><span data-stu-id="6efa5-402">Total Storage in Bytes.</span></span> <span data-ttu-id="6efa5-403">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6efa5-403">This property is read-only.</span></span> <span data-ttu-id="6efa5-404">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6efa5-404">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6efa5-405">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="6efa5-405">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="6efa5-406">Int64</span><span class="sxs-lookup"><span data-stu-id="6efa5-406">Int64</span></span>|<span data-ttu-id="6efa5-407">以字节为单位的可用存储空间。</span><span class="sxs-lookup"><span data-stu-id="6efa5-407">Free Storage in Bytes.</span></span> <span data-ttu-id="6efa5-408">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6efa5-408">This property is read-only.</span></span> <span data-ttu-id="6efa5-409">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6efa5-409">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6efa5-410">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="6efa5-410">managedDeviceName</span></span>|<span data-ttu-id="6efa5-411">String</span><span class="sxs-lookup"><span data-stu-id="6efa5-411">String</span></span>|<span data-ttu-id="6efa5-412">用于识别设备的自动生成的名称。</span><span class="sxs-lookup"><span data-stu-id="6efa5-412">Automatically generated name to identify a device.</span></span> <span data-ttu-id="6efa5-413">可以覆盖为用户友好名称。</span><span class="sxs-lookup"><span data-stu-id="6efa5-413">Can be overwritten to a user friendly name.</span></span> <span data-ttu-id="6efa5-414">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6efa5-414">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6efa5-415">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="6efa5-415">partnerReportedThreatState</span></span>|[<span data-ttu-id="6efa5-416">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="6efa5-416">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="6efa5-417">指示帐户和设备正在使用移动威胁防护合作伙伴时设备的威胁状态。</span><span class="sxs-lookup"><span data-stu-id="6efa5-417">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="6efa5-418">只读。</span><span class="sxs-lookup"><span data-stu-id="6efa5-418">Read Only.</span></span> <span data-ttu-id="6efa5-419">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6efa5-419">This property is read-only.</span></span> <span data-ttu-id="6efa5-420">继承自[managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="6efa5-420">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="6efa5-421">可取值为：`unknown`、`activated`、`deactivated`、`secured`、`lowSeverity`、`mediumSeverity`、`highSeverity`、`unresponsive`、`compromised`、`misconfigured`。</span><span class="sxs-lookup"><span data-stu-id="6efa5-421">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="6efa5-422">retireAfterDateTime</span><span class="sxs-lookup"><span data-stu-id="6efa5-422">retireAfterDateTime</span></span>|<span data-ttu-id="6efa5-423">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6efa5-423">DateTimeOffset</span></span>|<span data-ttu-id="6efa5-424">指示当设备因计划操作而自动停用的时间。</span><span class="sxs-lookup"><span data-stu-id="6efa5-424">Indicates the time after when a device will be auto retired because of scheduled action.</span></span> <span data-ttu-id="6efa5-425">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6efa5-425">This property is read-only.</span></span> <span data-ttu-id="6efa5-426">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6efa5-426">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6efa5-427">usersLoggedOn</span><span class="sxs-lookup"><span data-stu-id="6efa5-427">usersLoggedOn</span></span>|<span data-ttu-id="6efa5-428">[loggedOnUser](../resources/intune-devices-loggedonuser.md)集合</span><span class="sxs-lookup"><span data-stu-id="6efa5-428">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="6efa5-429">指示设备的上次登录用户。</span><span class="sxs-lookup"><span data-stu-id="6efa5-429">Indicates the last logged on users of a device.</span></span> <span data-ttu-id="6efa5-430">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6efa5-430">This property is read-only.</span></span> <span data-ttu-id="6efa5-431">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6efa5-431">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6efa5-432">preferMdmOverGroupPolicyAppliedDateTime</span><span class="sxs-lookup"><span data-stu-id="6efa5-432">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="6efa5-433">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6efa5-433">DateTimeOffset</span></span>|<span data-ttu-id="6efa5-434">报告设置了 preferMdmOverGroupPolicy 设置的 DateTime。</span><span class="sxs-lookup"><span data-stu-id="6efa5-434">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="6efa5-435">设置后，如果存在冲突，Intune MDM 设置将覆盖组策略设置。</span><span class="sxs-lookup"><span data-stu-id="6efa5-435">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="6efa5-436">只读。</span><span class="sxs-lookup"><span data-stu-id="6efa5-436">Read Only.</span></span> <span data-ttu-id="6efa5-437">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6efa5-437">This property is read-only.</span></span> <span data-ttu-id="6efa5-438">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6efa5-438">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6efa5-439">autopilotEnrolled</span><span class="sxs-lookup"><span data-stu-id="6efa5-439">autopilotEnrolled</span></span>|<span data-ttu-id="6efa5-440">Boolean</span><span class="sxs-lookup"><span data-stu-id="6efa5-440">Boolean</span></span>|<span data-ttu-id="6efa5-441">如果托管设备是通过自动引导注册的，则报告。</span><span class="sxs-lookup"><span data-stu-id="6efa5-441">Reports if the managed device is enrolled via auto-pilot.</span></span> <span data-ttu-id="6efa5-442">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6efa5-442">This property is read-only.</span></span> <span data-ttu-id="6efa5-443">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6efa5-443">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6efa5-444">requireUserEnrollmentApproval</span><span class="sxs-lookup"><span data-stu-id="6efa5-444">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="6efa5-445">Boolean</span><span class="sxs-lookup"><span data-stu-id="6efa5-445">Boolean</span></span>|<span data-ttu-id="6efa5-446">如果托管 iOS 设备是用户审批注册，则报告。</span><span class="sxs-lookup"><span data-stu-id="6efa5-446">Reports if the managed iOS device is user approval enrollment.</span></span> <span data-ttu-id="6efa5-447">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6efa5-447">This property is read-only.</span></span> <span data-ttu-id="6efa5-448">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6efa5-448">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6efa5-449">managementCertificateExpirationDate</span><span class="sxs-lookup"><span data-stu-id="6efa5-449">managementCertificateExpirationDate</span></span>|<span data-ttu-id="6efa5-450">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6efa5-450">DateTimeOffset</span></span>|<span data-ttu-id="6efa5-451">报告设备管理证书到期日期。</span><span class="sxs-lookup"><span data-stu-id="6efa5-451">Reports device management certificate expiration date.</span></span> <span data-ttu-id="6efa5-452">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6efa5-452">This property is read-only.</span></span> <span data-ttu-id="6efa5-453">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6efa5-453">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6efa5-454">iccid</span><span class="sxs-lookup"><span data-stu-id="6efa5-454">iccid</span></span>|<span data-ttu-id="6efa5-455">字符串</span><span class="sxs-lookup"><span data-stu-id="6efa5-455">String</span></span>|<span data-ttu-id="6efa5-456">集成的电路卡标识符，它是 SIM 卡的唯一标识号。</span><span class="sxs-lookup"><span data-stu-id="6efa5-456">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span> <span data-ttu-id="6efa5-457">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6efa5-457">This property is read-only.</span></span> <span data-ttu-id="6efa5-458">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6efa5-458">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6efa5-459">udid</span><span class="sxs-lookup"><span data-stu-id="6efa5-459">udid</span></span>|<span data-ttu-id="6efa5-460">字符串</span><span class="sxs-lookup"><span data-stu-id="6efa5-460">String</span></span>|<span data-ttu-id="6efa5-461">IOS 和 macOS 设备的唯一设备标识符。</span><span class="sxs-lookup"><span data-stu-id="6efa5-461">Unique Device Identifier for iOS and macOS devices.</span></span> <span data-ttu-id="6efa5-462">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6efa5-462">This property is read-only.</span></span> <span data-ttu-id="6efa5-463">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6efa5-463">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6efa5-464">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6efa5-464">roleScopeTagIds</span></span>|<span data-ttu-id="6efa5-465">String 集合</span><span class="sxs-lookup"><span data-stu-id="6efa5-465">String collection</span></span>|<span data-ttu-id="6efa5-466">此设备实例的范围标记 Id 的列表。</span><span class="sxs-lookup"><span data-stu-id="6efa5-466">List of Scope Tag IDs for this Device instance.</span></span> <span data-ttu-id="6efa5-467">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6efa5-467">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6efa5-468">windowsActiveMalwareCount</span><span class="sxs-lookup"><span data-stu-id="6efa5-468">windowsActiveMalwareCount</span></span>|<span data-ttu-id="6efa5-469">Int32</span><span class="sxs-lookup"><span data-stu-id="6efa5-469">Int32</span></span>|<span data-ttu-id="6efa5-470">此 windows 设备的活动恶意软件的计数。</span><span class="sxs-lookup"><span data-stu-id="6efa5-470">Count of active malware for this windows device.</span></span> <span data-ttu-id="6efa5-471">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6efa5-471">This property is read-only.</span></span> <span data-ttu-id="6efa5-472">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6efa5-472">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6efa5-473">windowsRemediatedMalwareCount</span><span class="sxs-lookup"><span data-stu-id="6efa5-473">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="6efa5-474">Int32</span><span class="sxs-lookup"><span data-stu-id="6efa5-474">Int32</span></span>|<span data-ttu-id="6efa5-475">此 windows 设备的修正的恶意软件的计数。</span><span class="sxs-lookup"><span data-stu-id="6efa5-475">Count of remediated malware for this windows device.</span></span> <span data-ttu-id="6efa5-476">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6efa5-476">This property is read-only.</span></span> <span data-ttu-id="6efa5-477">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6efa5-477">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6efa5-478">notes</span><span class="sxs-lookup"><span data-stu-id="6efa5-478">notes</span></span>|<span data-ttu-id="6efa5-479">String</span><span class="sxs-lookup"><span data-stu-id="6efa5-479">String</span></span>|<span data-ttu-id="6efa5-480">由 IT 管理员创建的设备上的注释继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6efa5-480">Notes on the device created by IT Admin Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6efa5-481">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="6efa5-481">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="6efa5-482">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="6efa5-482">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="6efa5-483">Configuration manager 客户端运行状况状态，仅适用于从[ManagedDevice](../resources/intune-devices-manageddevice.md)继承的 MDM/ConfigMgr 代理所管理的设备</span><span class="sxs-lookup"><span data-stu-id="6efa5-483">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6efa5-484">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="6efa5-484">configurationManagerClientInformation</span></span>|[<span data-ttu-id="6efa5-485">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="6efa5-485">configurationManagerClientInformation</span></span>](../resources/intune-devices-configurationmanagerclientinformation.md)|<span data-ttu-id="6efa5-486">Configuration manager 客户端信息，仅对由[ManagedDevice](../resources/intune-devices-manageddevice.md)继承的 ConfigMgr 代理、duel 管理或三方管理的设备有效</span><span class="sxs-lookup"><span data-stu-id="6efa5-486">Configuration manager client information, valid only for devices managed, duel-managed or tri-managed by ConfigMgr Agent Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6efa5-487">ethernetMacAddress</span><span class="sxs-lookup"><span data-stu-id="6efa5-487">ethernetMacAddress</span></span>|<span data-ttu-id="6efa5-488">字符串</span><span class="sxs-lookup"><span data-stu-id="6efa5-488">String</span></span>|<span data-ttu-id="6efa5-489">以太网 MAC。</span><span class="sxs-lookup"><span data-stu-id="6efa5-489">Ethernet MAC.</span></span> <span data-ttu-id="6efa5-490">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6efa5-490">This property is read-only.</span></span> <span data-ttu-id="6efa5-491">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6efa5-491">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6efa5-492">physicalMemoryInBytes</span><span class="sxs-lookup"><span data-stu-id="6efa5-492">physicalMemoryInBytes</span></span>|<span data-ttu-id="6efa5-493">Int64</span><span class="sxs-lookup"><span data-stu-id="6efa5-493">Int64</span></span>|<span data-ttu-id="6efa5-494">内存总量（以字节为单位）。</span><span class="sxs-lookup"><span data-stu-id="6efa5-494">Total Memory in Bytes.</span></span> <span data-ttu-id="6efa5-495">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6efa5-495">This property is read-only.</span></span> <span data-ttu-id="6efa5-496">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6efa5-496">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6efa5-497">processorArchitecture</span><span class="sxs-lookup"><span data-stu-id="6efa5-497">processorArchitecture</span></span>|[<span data-ttu-id="6efa5-498">managedDeviceArchitecture</span><span class="sxs-lookup"><span data-stu-id="6efa5-498">managedDeviceArchitecture</span></span>](../resources/intune-devices-manageddevicearchitecture.md)|<span data-ttu-id="6efa5-499">处理器体系结构。</span><span class="sxs-lookup"><span data-stu-id="6efa5-499">Processor architecture.</span></span> <span data-ttu-id="6efa5-500">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6efa5-500">This property is read-only.</span></span> <span data-ttu-id="6efa5-501">继承自[managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="6efa5-501">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="6efa5-502">可取值为：`unknown`、`x86`、`x64`、`arm`、`arM64`。</span><span class="sxs-lookup"><span data-stu-id="6efa5-502">Possible values are: `unknown`, `x86`, `x64`, `arm`, `arM64`.</span></span>|
|<span data-ttu-id="6efa5-503">specificationVersion</span><span class="sxs-lookup"><span data-stu-id="6efa5-503">specificationVersion</span></span>|<span data-ttu-id="6efa5-504">字符串</span><span class="sxs-lookup"><span data-stu-id="6efa5-504">String</span></span>|<span data-ttu-id="6efa5-505">规范版本。</span><span class="sxs-lookup"><span data-stu-id="6efa5-505">Specification version.</span></span> <span data-ttu-id="6efa5-506">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6efa5-506">This property is read-only.</span></span> <span data-ttu-id="6efa5-507">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6efa5-507">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|



## <a name="response"></a><span data-ttu-id="6efa5-508">响应</span><span class="sxs-lookup"><span data-stu-id="6efa5-508">Response</span></span>
<span data-ttu-id="6efa5-509">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6efa5-509">If successful, this method returns a `200 OK` response code and an updated [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6efa5-510">示例</span><span class="sxs-lookup"><span data-stu-id="6efa5-510">Example</span></span>

### <a name="request"></a><span data-ttu-id="6efa5-511">请求</span><span class="sxs-lookup"><span data-stu-id="6efa5-511">Request</span></span>
<span data-ttu-id="6efa5-512">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6efa5-512">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}
Content-type: application/json
Content-length: 7723

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
    "clientIdentifier": "Client Identifier value",
    "isBlocked": true
  },
  "ethernetMacAddress": "Ethernet Mac Address value",
  "physicalMemoryInBytes": 5,
  "processorArchitecture": "x86",
  "specificationVersion": "Specification Version value"
}
```

### <a name="response"></a><span data-ttu-id="6efa5-513">响应</span><span class="sxs-lookup"><span data-stu-id="6efa5-513">Response</span></span>
<span data-ttu-id="6efa5-p172">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6efa5-p172">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 7772

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
    "clientIdentifier": "Client Identifier value",
    "isBlocked": true
  },
  "ethernetMacAddress": "Ethernet Mac Address value",
  "physicalMemoryInBytes": 5,
  "processorArchitecture": "x86",
  "specificationVersion": "Specification Version value"
}
```



