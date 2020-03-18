---
title: 创建 windowsManagedDevice
description: 创建新的 windowsManagedDevice 对象。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 75f6393938d8dfb72fffd4d5afe2698a0fa787fb
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42813668"
---
# <a name="create-windowsmanageddevice"></a><span data-ttu-id="4267d-103">创建 windowsManagedDevice</span><span class="sxs-lookup"><span data-stu-id="4267d-103">Create windowsManagedDevice</span></span>

> <span data-ttu-id="4267d-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4267d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4267d-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4267d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4267d-106">创建新的[windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4267d-106">Create a new [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4267d-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="4267d-107">Prerequisites</span></span>
<span data-ttu-id="4267d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4267d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4267d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4267d-110">Permission type</span></span>|<span data-ttu-id="4267d-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4267d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4267d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4267d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4267d-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4267d-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="4267d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4267d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4267d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4267d-115">Not supported.</span></span>|
|<span data-ttu-id="4267d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="4267d-116">Application</span></span>|<span data-ttu-id="4267d-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4267d-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4267d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4267d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices
```

## <a name="request-headers"></a><span data-ttu-id="4267d-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4267d-119">Request headers</span></span>
|<span data-ttu-id="4267d-120">标头</span><span class="sxs-lookup"><span data-stu-id="4267d-120">Header</span></span>|<span data-ttu-id="4267d-121">值</span><span class="sxs-lookup"><span data-stu-id="4267d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4267d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4267d-122">Authorization</span></span>|<span data-ttu-id="4267d-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4267d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4267d-124">接受</span><span class="sxs-lookup"><span data-stu-id="4267d-124">Accept</span></span>|<span data-ttu-id="4267d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4267d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4267d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="4267d-126">Request body</span></span>
<span data-ttu-id="4267d-127">在请求正文中，提供 windowsManagedDevice 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4267d-127">In the request body, supply a JSON representation for the windowsManagedDevice object.</span></span>

<span data-ttu-id="4267d-128">下表显示创建 windowsManagedDevice 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="4267d-128">The following table shows the properties that are required when you create the windowsManagedDevice.</span></span>

|<span data-ttu-id="4267d-129">属性</span><span class="sxs-lookup"><span data-stu-id="4267d-129">Property</span></span>|<span data-ttu-id="4267d-130">类型</span><span class="sxs-lookup"><span data-stu-id="4267d-130">Type</span></span>|<span data-ttu-id="4267d-131">说明</span><span class="sxs-lookup"><span data-stu-id="4267d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4267d-132">id</span><span class="sxs-lookup"><span data-stu-id="4267d-132">id</span></span>|<span data-ttu-id="4267d-133">字符串</span><span class="sxs-lookup"><span data-stu-id="4267d-133">String</span></span>|<span data-ttu-id="4267d-134">设备的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="4267d-134">Unique Identifier for the device.</span></span> <span data-ttu-id="4267d-135">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4267d-135">This property is read-only.</span></span> <span data-ttu-id="4267d-136">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4267d-136">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4267d-137">userId</span><span class="sxs-lookup"><span data-stu-id="4267d-137">userId</span></span>|<span data-ttu-id="4267d-138">String</span><span class="sxs-lookup"><span data-stu-id="4267d-138">String</span></span>|<span data-ttu-id="4267d-139">与设备关联的用户的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="4267d-139">Unique Identifier for the user associated with the device.</span></span> <span data-ttu-id="4267d-140">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4267d-140">This property is read-only.</span></span> <span data-ttu-id="4267d-141">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4267d-141">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4267d-142">deviceName</span><span class="sxs-lookup"><span data-stu-id="4267d-142">deviceName</span></span>|<span data-ttu-id="4267d-143">String</span><span class="sxs-lookup"><span data-stu-id="4267d-143">String</span></span>|<span data-ttu-id="4267d-144">设备的名称。</span><span class="sxs-lookup"><span data-stu-id="4267d-144">Name of the device.</span></span> <span data-ttu-id="4267d-145">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4267d-145">This property is read-only.</span></span> <span data-ttu-id="4267d-146">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4267d-146">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4267d-147">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="4267d-147">hardwareInformation</span></span>|[<span data-ttu-id="4267d-148">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="4267d-148">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="4267d-149">设备的 hardward 详细信息。</span><span class="sxs-lookup"><span data-stu-id="4267d-149">The hardward details for the device.</span></span>  <span data-ttu-id="4267d-150">包括存储空间、制造商、序列号等信息。此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4267d-150">Includes information such as storage space, manufacturer, serial number, etc. This property is read-only.</span></span> <span data-ttu-id="4267d-151">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4267d-151">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4267d-152">所有者</span><span class="sxs-lookup"><span data-stu-id="4267d-152">ownerType</span></span>|[<span data-ttu-id="4267d-153">所有者</span><span class="sxs-lookup"><span data-stu-id="4267d-153">ownerType</span></span>](../resources/intune-shared-ownertype.md)|<span data-ttu-id="4267d-154">设备的所有权。</span><span class="sxs-lookup"><span data-stu-id="4267d-154">Ownership of the device.</span></span> <span data-ttu-id="4267d-155">可以是从[ManagedDevice](../resources/intune-devices-manageddevice.md)继承的 "公司" 或 "个人"。</span><span class="sxs-lookup"><span data-stu-id="4267d-155">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="4267d-156">可取值为：`unknown`、`company`、`personal`。</span><span class="sxs-lookup"><span data-stu-id="4267d-156">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="4267d-157">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="4267d-157">managedDeviceOwnerType</span></span>|[<span data-ttu-id="4267d-158">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="4267d-158">managedDeviceOwnerType</span></span>](../resources/intune-shared-manageddeviceownertype.md)|<span data-ttu-id="4267d-159">设备的所有权。</span><span class="sxs-lookup"><span data-stu-id="4267d-159">Ownership of the device.</span></span> <span data-ttu-id="4267d-160">可以是从[ManagedDevice](../resources/intune-devices-manageddevice.md)继承的 "公司" 或 "个人"。</span><span class="sxs-lookup"><span data-stu-id="4267d-160">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="4267d-161">可取值为：`unknown`、`company`、`personal`。</span><span class="sxs-lookup"><span data-stu-id="4267d-161">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="4267d-162">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="4267d-162">deviceActionResults</span></span>|<span data-ttu-id="4267d-163">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4267d-163">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="4267d-164">ComplexType deviceActionResult 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="4267d-164">List of ComplexType deviceActionResult objects.</span></span> <span data-ttu-id="4267d-165">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4267d-165">This property is read-only.</span></span> <span data-ttu-id="4267d-166">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4267d-166">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4267d-167">managementState</span><span class="sxs-lookup"><span data-stu-id="4267d-167">managementState</span></span>|[<span data-ttu-id="4267d-168">managementState</span><span class="sxs-lookup"><span data-stu-id="4267d-168">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="4267d-169">设备的管理状态。</span><span class="sxs-lookup"><span data-stu-id="4267d-169">Management state of the device.</span></span> <span data-ttu-id="4267d-170">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4267d-170">This property is read-only.</span></span> <span data-ttu-id="4267d-171">继承自[managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="4267d-171">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="4267d-172">可取值为：`managed`、`retirePending`、`retireFailed`、`wipePending`、`wipeFailed`、`unhealthy`、`deletePending`、`retireIssued`、`wipeIssued`、`wipeCanceled`、`retireCanceled`、`discovered`。</span><span class="sxs-lookup"><span data-stu-id="4267d-172">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="4267d-173">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="4267d-173">enrolledDateTime</span></span>|<span data-ttu-id="4267d-174">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4267d-174">DateTimeOffset</span></span>|<span data-ttu-id="4267d-175">设备的注册时间。</span><span class="sxs-lookup"><span data-stu-id="4267d-175">Enrollment time of the device.</span></span> <span data-ttu-id="4267d-176">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4267d-176">This property is read-only.</span></span> <span data-ttu-id="4267d-177">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4267d-177">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4267d-178">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="4267d-178">lastSyncDateTime</span></span>|<span data-ttu-id="4267d-179">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4267d-179">DateTimeOffset</span></span>|<span data-ttu-id="4267d-180">设备上次成功完成与 Intune 同步的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="4267d-180">The date and time that the device last completed a successful sync with Intune.</span></span> <span data-ttu-id="4267d-181">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4267d-181">This property is read-only.</span></span> <span data-ttu-id="4267d-182">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4267d-182">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4267d-183">chassisType</span><span class="sxs-lookup"><span data-stu-id="4267d-183">chassisType</span></span>|[<span data-ttu-id="4267d-184">chassisType</span><span class="sxs-lookup"><span data-stu-id="4267d-184">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="4267d-185">设备的机箱类型。</span><span class="sxs-lookup"><span data-stu-id="4267d-185">Chassis type of the device.</span></span> <span data-ttu-id="4267d-186">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4267d-186">This property is read-only.</span></span> <span data-ttu-id="4267d-187">继承自[managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="4267d-187">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="4267d-188">可取值为：`unknown`、`desktop`、`laptop`、`worksWorkstation`、`enterpriseServer`、`phone`、`tablet`、`mobileOther`、`mobileUnknown`。</span><span class="sxs-lookup"><span data-stu-id="4267d-188">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="4267d-189">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="4267d-189">operatingSystem</span></span>|<span data-ttu-id="4267d-190">String</span><span class="sxs-lookup"><span data-stu-id="4267d-190">String</span></span>|<span data-ttu-id="4267d-191">设备的操作系统。</span><span class="sxs-lookup"><span data-stu-id="4267d-191">Operating system of the device.</span></span> <span data-ttu-id="4267d-192">Windows、iOS 等。此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4267d-192">Windows, iOS, etc. This property is read-only.</span></span> <span data-ttu-id="4267d-193">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4267d-193">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4267d-194">deviceType</span><span class="sxs-lookup"><span data-stu-id="4267d-194">deviceType</span></span>|[<span data-ttu-id="4267d-195">deviceType</span><span class="sxs-lookup"><span data-stu-id="4267d-195">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="4267d-196">设备的平台。</span><span class="sxs-lookup"><span data-stu-id="4267d-196">Platform of the device.</span></span> <span data-ttu-id="4267d-197">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4267d-197">This property is read-only.</span></span> <span data-ttu-id="4267d-198">继承自[managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="4267d-198">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="4267d-199">可能的值为`desktop`： `windowsRT`、 `winMO6`、 `nokia` `windowsPhone` `mac` `winCE` `palm` `unknown`、、、、、、、、、、、、、、、、、、、、。 `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `windows10x` `blackberry`</span><span class="sxs-lookup"><span data-stu-id="4267d-199">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="4267d-200">complianceState</span><span class="sxs-lookup"><span data-stu-id="4267d-200">complianceState</span></span>|[<span data-ttu-id="4267d-201">complianceState</span><span class="sxs-lookup"><span data-stu-id="4267d-201">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="4267d-202">设备的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="4267d-202">Compliance state of the device.</span></span> <span data-ttu-id="4267d-203">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4267d-203">This property is read-only.</span></span> <span data-ttu-id="4267d-204">继承自[managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="4267d-204">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="4267d-205">可取值为：`unknown`、`compliant`、`noncompliant`、`conflict`、`error`、`inGracePeriod`、`configManager`。</span><span class="sxs-lookup"><span data-stu-id="4267d-205">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="4267d-206">jailBroken</span><span class="sxs-lookup"><span data-stu-id="4267d-206">jailBroken</span></span>|<span data-ttu-id="4267d-207">String</span><span class="sxs-lookup"><span data-stu-id="4267d-207">String</span></span>|<span data-ttu-id="4267d-208">设备是否已越狱或取得 root 权限。</span><span class="sxs-lookup"><span data-stu-id="4267d-208">whether the device is jail broken or rooted.</span></span> <span data-ttu-id="4267d-209">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4267d-209">This property is read-only.</span></span> <span data-ttu-id="4267d-210">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4267d-210">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4267d-211">managementAgent</span><span class="sxs-lookup"><span data-stu-id="4267d-211">managementAgent</span></span>|[<span data-ttu-id="4267d-212">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="4267d-212">managementAgentType</span></span>](../resources/intune-shared-managementagenttype.md)|<span data-ttu-id="4267d-213">设备的管理通道。</span><span class="sxs-lookup"><span data-stu-id="4267d-213">Management channel of the device.</span></span> <span data-ttu-id="4267d-214">Intune、EAS 等。此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4267d-214">Intune, EAS, etc. This property is read-only.</span></span> <span data-ttu-id="4267d-215">继承自[managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="4267d-215">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="4267d-216">可能的值是：`eas`、`mdm`、`easMdm`、`intuneClient`、`easIntuneClient`、`configurationManagerClient`、`configurationManagerClientMdm`、`configurationManagerClientMdmEas`、`unknown`、`jamf`、`googleCloudDevicePolicyController`、`microsoft365ManagedMdm`、`windowsManagementCloudApi`。</span><span class="sxs-lookup"><span data-stu-id="4267d-216">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`, `windowsManagementCloudApi`.</span></span>|
|<span data-ttu-id="4267d-217">osVersion</span><span class="sxs-lookup"><span data-stu-id="4267d-217">osVersion</span></span>|<span data-ttu-id="4267d-218">String</span><span class="sxs-lookup"><span data-stu-id="4267d-218">String</span></span>|<span data-ttu-id="4267d-219">设备的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="4267d-219">Operating system version of the device.</span></span> <span data-ttu-id="4267d-220">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4267d-220">This property is read-only.</span></span> <span data-ttu-id="4267d-221">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4267d-221">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4267d-222">easActivated</span><span class="sxs-lookup"><span data-stu-id="4267d-222">easActivated</span></span>|<span data-ttu-id="4267d-223">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267d-223">Boolean</span></span>|<span data-ttu-id="4267d-224">设备是否已激活 Exchange ActiveSync。</span><span class="sxs-lookup"><span data-stu-id="4267d-224">Whether the device is Exchange ActiveSync activated.</span></span> <span data-ttu-id="4267d-225">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4267d-225">This property is read-only.</span></span> <span data-ttu-id="4267d-226">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4267d-226">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4267d-227">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="4267d-227">easDeviceId</span></span>|<span data-ttu-id="4267d-228">String</span><span class="sxs-lookup"><span data-stu-id="4267d-228">String</span></span>|<span data-ttu-id="4267d-229">设备的 Exchange ActiveSync ID。</span><span class="sxs-lookup"><span data-stu-id="4267d-229">Exchange ActiveSync Id of the device.</span></span> <span data-ttu-id="4267d-230">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4267d-230">This property is read-only.</span></span> <span data-ttu-id="4267d-231">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4267d-231">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4267d-232">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="4267d-232">easActivationDateTime</span></span>|<span data-ttu-id="4267d-233">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4267d-233">DateTimeOffset</span></span>|<span data-ttu-id="4267d-234">设备的 Exchange ActivationSync 激活时间。</span><span class="sxs-lookup"><span data-stu-id="4267d-234">Exchange ActivationSync activation time of the device.</span></span> <span data-ttu-id="4267d-235">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4267d-235">This property is read-only.</span></span> <span data-ttu-id="4267d-236">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4267d-236">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4267d-237">aadRegistered</span><span class="sxs-lookup"><span data-stu-id="4267d-237">aadRegistered</span></span>|<span data-ttu-id="4267d-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="4267d-238">Boolean</span></span>|<span data-ttu-id="4267d-239">设备是否已注册 Azure Active Directory。</span><span class="sxs-lookup"><span data-stu-id="4267d-239">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="4267d-240">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4267d-240">This property is read-only.</span></span> <span data-ttu-id="4267d-241">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4267d-241">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4267d-242">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="4267d-242">azureADRegistered</span></span>|<span data-ttu-id="4267d-243">Boolean</span><span class="sxs-lookup"><span data-stu-id="4267d-243">Boolean</span></span>|<span data-ttu-id="4267d-244">设备是否已注册 Azure Active Directory。</span><span class="sxs-lookup"><span data-stu-id="4267d-244">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="4267d-245">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4267d-245">This property is read-only.</span></span> <span data-ttu-id="4267d-246">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4267d-246">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4267d-247">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="4267d-247">deviceEnrollmentType</span></span>|[<span data-ttu-id="4267d-248">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="4267d-248">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="4267d-249">设备的注册类型。</span><span class="sxs-lookup"><span data-stu-id="4267d-249">Enrollment type of the device.</span></span> <span data-ttu-id="4267d-250">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4267d-250">This property is read-only.</span></span> <span data-ttu-id="4267d-251">继承自[managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="4267d-251">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="4267d-252">可取值为：`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement`、`appleUserEnrollment`、`appleUserEnrollmentWithServiceAccount`。</span><span class="sxs-lookup"><span data-stu-id="4267d-252">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`.</span></span>|
|<span data-ttu-id="4267d-253">lostModeState</span><span class="sxs-lookup"><span data-stu-id="4267d-253">lostModeState</span></span>|[<span data-ttu-id="4267d-254">lostModeState</span><span class="sxs-lookup"><span data-stu-id="4267d-254">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="4267d-255">指示是否已启用或禁用了丢失模式。</span><span class="sxs-lookup"><span data-stu-id="4267d-255">Indicates if Lost mode is enabled or disabled.</span></span> <span data-ttu-id="4267d-256">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4267d-256">This property is read-only.</span></span> <span data-ttu-id="4267d-257">继承自[managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="4267d-257">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="4267d-258">可取值为：`disabled`、`enabled`。</span><span class="sxs-lookup"><span data-stu-id="4267d-258">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="4267d-259">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="4267d-259">activationLockBypassCode</span></span>|<span data-ttu-id="4267d-260">String</span><span class="sxs-lookup"><span data-stu-id="4267d-260">String</span></span>|<span data-ttu-id="4267d-261">允许绕过设备上的激活锁的代码。</span><span class="sxs-lookup"><span data-stu-id="4267d-261">Code that allows the Activation Lock on a device to be bypassed.</span></span> <span data-ttu-id="4267d-262">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4267d-262">This property is read-only.</span></span> <span data-ttu-id="4267d-263">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4267d-263">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4267d-264">emailAddress</span><span class="sxs-lookup"><span data-stu-id="4267d-264">emailAddress</span></span>|<span data-ttu-id="4267d-265">String</span><span class="sxs-lookup"><span data-stu-id="4267d-265">String</span></span>|<span data-ttu-id="4267d-266">与设备关联的用户的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="4267d-266">Email(s) for the user associated with the device.</span></span> <span data-ttu-id="4267d-267">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4267d-267">This property is read-only.</span></span> <span data-ttu-id="4267d-268">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4267d-268">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4267d-269">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="4267d-269">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="4267d-270">String</span><span class="sxs-lookup"><span data-stu-id="4267d-270">String</span></span>|<span data-ttu-id="4267d-271">Azure Active Directory 设备的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="4267d-271">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="4267d-272">只读。</span><span class="sxs-lookup"><span data-stu-id="4267d-272">Read only.</span></span> <span data-ttu-id="4267d-273">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4267d-273">This property is read-only.</span></span> <span data-ttu-id="4267d-274">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4267d-274">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4267d-275">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="4267d-275">azureADDeviceId</span></span>|<span data-ttu-id="4267d-276">String</span><span class="sxs-lookup"><span data-stu-id="4267d-276">String</span></span>|<span data-ttu-id="4267d-277">Azure Active Directory 设备的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="4267d-277">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="4267d-278">只读。</span><span class="sxs-lookup"><span data-stu-id="4267d-278">Read only.</span></span> <span data-ttu-id="4267d-279">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4267d-279">This property is read-only.</span></span> <span data-ttu-id="4267d-280">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4267d-280">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4267d-281">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="4267d-281">deviceRegistrationState</span></span>|[<span data-ttu-id="4267d-282">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="4267d-282">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="4267d-283">设备注册状态。</span><span class="sxs-lookup"><span data-stu-id="4267d-283">Device registration state.</span></span> <span data-ttu-id="4267d-284">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4267d-284">This property is read-only.</span></span> <span data-ttu-id="4267d-285">继承自[managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="4267d-285">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="4267d-286">可取值为：`notRegistered`、`registered`、`revoked`、`keyConflict`、`approvalPending`、`certificateReset`、`notRegisteredPendingEnrollment`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="4267d-286">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="4267d-287">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="4267d-287">deviceCategoryDisplayName</span></span>|<span data-ttu-id="4267d-288">String</span><span class="sxs-lookup"><span data-stu-id="4267d-288">String</span></span>|<span data-ttu-id="4267d-289">设备类别显示名称。</span><span class="sxs-lookup"><span data-stu-id="4267d-289">Device category display name.</span></span> <span data-ttu-id="4267d-290">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4267d-290">This property is read-only.</span></span> <span data-ttu-id="4267d-291">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4267d-291">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4267d-292">isSupervised</span><span class="sxs-lookup"><span data-stu-id="4267d-292">isSupervised</span></span>|<span data-ttu-id="4267d-293">Boolean</span><span class="sxs-lookup"><span data-stu-id="4267d-293">Boolean</span></span>|<span data-ttu-id="4267d-294">设备监督状态。</span><span class="sxs-lookup"><span data-stu-id="4267d-294">Device supervised status.</span></span> <span data-ttu-id="4267d-295">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4267d-295">This property is read-only.</span></span> <span data-ttu-id="4267d-296">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4267d-296">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4267d-297">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="4267d-297">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="4267d-298">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4267d-298">DateTimeOffset</span></span>|<span data-ttu-id="4267d-299">设备上次与 Exchange 联系的时间。</span><span class="sxs-lookup"><span data-stu-id="4267d-299">Last time the device contacted Exchange.</span></span> <span data-ttu-id="4267d-300">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4267d-300">This property is read-only.</span></span> <span data-ttu-id="4267d-301">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4267d-301">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4267d-302">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="4267d-302">exchangeAccessState</span></span>|[<span data-ttu-id="4267d-303">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="4267d-303">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="4267d-304">Exchange 中设备的访问状态。</span><span class="sxs-lookup"><span data-stu-id="4267d-304">The Access State of the device in Exchange.</span></span> <span data-ttu-id="4267d-305">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4267d-305">This property is read-only.</span></span> <span data-ttu-id="4267d-306">继承自[managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="4267d-306">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="4267d-307">可取值为：`none`、`unknown`、`allowed`、`blocked`、`quarantined`。</span><span class="sxs-lookup"><span data-stu-id="4267d-307">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="4267d-308">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="4267d-308">exchangeAccessStateReason</span></span>|[<span data-ttu-id="4267d-309">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="4267d-309">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="4267d-310">Exchange 中设备访问状态的出现原因。</span><span class="sxs-lookup"><span data-stu-id="4267d-310">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="4267d-311">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4267d-311">This property is read-only.</span></span> <span data-ttu-id="4267d-312">继承自[managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="4267d-312">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="4267d-313">可取值为：`none`、`unknown`、`exchangeGlobalRule`、`exchangeIndividualRule`、`exchangeDeviceRule`、`exchangeUpgrade`、`exchangeMailboxPolicy`、`other`、`compliant`、`notCompliant`、`notEnrolled`、`unknownLocation`、`mfaRequired`、`azureADBlockDueToAccessPolicy`、`compromisedPassword`、`deviceNotKnownWithManagedApp`。</span><span class="sxs-lookup"><span data-stu-id="4267d-313">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="4267d-314">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="4267d-314">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="4267d-315">String</span><span class="sxs-lookup"><span data-stu-id="4267d-315">String</span></span>|<span data-ttu-id="4267d-316">允许与设备建立远程协助会话的 URL。</span><span class="sxs-lookup"><span data-stu-id="4267d-316">Url that allows a Remote Assistance session to be established with the device.</span></span> <span data-ttu-id="4267d-317">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4267d-317">This property is read-only.</span></span> <span data-ttu-id="4267d-318">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4267d-318">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4267d-319">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="4267d-319">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="4267d-320">String</span><span class="sxs-lookup"><span data-stu-id="4267d-320">String</span></span>|<span data-ttu-id="4267d-321">用于在创建远程协助会话对象时识别问题的错误字符串。</span><span class="sxs-lookup"><span data-stu-id="4267d-321">An error string that identifies issues when creating Remote Assistance session objects.</span></span> <span data-ttu-id="4267d-322">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4267d-322">This property is read-only.</span></span> <span data-ttu-id="4267d-323">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4267d-323">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4267d-324">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="4267d-324">isEncrypted</span></span>|<span data-ttu-id="4267d-325">Boolean</span><span class="sxs-lookup"><span data-stu-id="4267d-325">Boolean</span></span>|<span data-ttu-id="4267d-326">设备加密状态。</span><span class="sxs-lookup"><span data-stu-id="4267d-326">Device encryption status.</span></span> <span data-ttu-id="4267d-327">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4267d-327">This property is read-only.</span></span> <span data-ttu-id="4267d-328">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4267d-328">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4267d-329">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="4267d-329">userPrincipalName</span></span>|<span data-ttu-id="4267d-330">字符串</span><span class="sxs-lookup"><span data-stu-id="4267d-330">String</span></span>|<span data-ttu-id="4267d-331">设备用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="4267d-331">Device user principal name.</span></span> <span data-ttu-id="4267d-332">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4267d-332">This property is read-only.</span></span> <span data-ttu-id="4267d-333">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4267d-333">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4267d-334">model</span><span class="sxs-lookup"><span data-stu-id="4267d-334">model</span></span>|<span data-ttu-id="4267d-335">String</span><span class="sxs-lookup"><span data-stu-id="4267d-335">String</span></span>|<span data-ttu-id="4267d-336">设备的模型。</span><span class="sxs-lookup"><span data-stu-id="4267d-336">Model of the device.</span></span> <span data-ttu-id="4267d-337">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4267d-337">This property is read-only.</span></span> <span data-ttu-id="4267d-338">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4267d-338">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4267d-339">manufacturer</span><span class="sxs-lookup"><span data-stu-id="4267d-339">manufacturer</span></span>|<span data-ttu-id="4267d-340">String</span><span class="sxs-lookup"><span data-stu-id="4267d-340">String</span></span>|<span data-ttu-id="4267d-341">设备的制造商。</span><span class="sxs-lookup"><span data-stu-id="4267d-341">Manufacturer of the device.</span></span> <span data-ttu-id="4267d-342">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4267d-342">This property is read-only.</span></span> <span data-ttu-id="4267d-343">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4267d-343">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4267d-344">imei</span><span class="sxs-lookup"><span data-stu-id="4267d-344">imei</span></span>|<span data-ttu-id="4267d-345">String</span><span class="sxs-lookup"><span data-stu-id="4267d-345">String</span></span>|<span data-ttu-id="4267d-346">IMEI.</span><span class="sxs-lookup"><span data-stu-id="4267d-346">IMEI.</span></span> <span data-ttu-id="4267d-347">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4267d-347">This property is read-only.</span></span> <span data-ttu-id="4267d-348">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4267d-348">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4267d-349">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="4267d-349">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="4267d-350">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4267d-350">DateTimeOffset</span></span>|<span data-ttu-id="4267d-351">设备符合性宽限期到期时的日期时间。</span><span class="sxs-lookup"><span data-stu-id="4267d-351">The DateTime when device compliance grace period expires.</span></span> <span data-ttu-id="4267d-352">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4267d-352">This property is read-only.</span></span> <span data-ttu-id="4267d-353">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4267d-353">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4267d-354">serialNumber</span><span class="sxs-lookup"><span data-stu-id="4267d-354">serialNumber</span></span>|<span data-ttu-id="4267d-355">字符串</span><span class="sxs-lookup"><span data-stu-id="4267d-355">String</span></span>|<span data-ttu-id="4267d-356">SerialNumber.</span><span class="sxs-lookup"><span data-stu-id="4267d-356">SerialNumber.</span></span> <span data-ttu-id="4267d-357">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4267d-357">This property is read-only.</span></span> <span data-ttu-id="4267d-358">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4267d-358">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4267d-359">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="4267d-359">phoneNumber</span></span>|<span data-ttu-id="4267d-360">String</span><span class="sxs-lookup"><span data-stu-id="4267d-360">String</span></span>|<span data-ttu-id="4267d-361">设备的电话号码。</span><span class="sxs-lookup"><span data-stu-id="4267d-361">Phone number of the device.</span></span> <span data-ttu-id="4267d-362">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4267d-362">This property is read-only.</span></span> <span data-ttu-id="4267d-363">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4267d-363">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4267d-364">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="4267d-364">androidSecurityPatchLevel</span></span>|<span data-ttu-id="4267d-365">String</span><span class="sxs-lookup"><span data-stu-id="4267d-365">String</span></span>|<span data-ttu-id="4267d-366">Android 安全修补程序级别。</span><span class="sxs-lookup"><span data-stu-id="4267d-366">Android security patch level.</span></span> <span data-ttu-id="4267d-367">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4267d-367">This property is read-only.</span></span> <span data-ttu-id="4267d-368">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4267d-368">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4267d-369">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="4267d-369">userDisplayName</span></span>|<span data-ttu-id="4267d-370">String</span><span class="sxs-lookup"><span data-stu-id="4267d-370">String</span></span>|<span data-ttu-id="4267d-371">用户显示名称。</span><span class="sxs-lookup"><span data-stu-id="4267d-371">User display name.</span></span> <span data-ttu-id="4267d-372">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4267d-372">This property is read-only.</span></span> <span data-ttu-id="4267d-373">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4267d-373">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4267d-374">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="4267d-374">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="4267d-375">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="4267d-375">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="4267d-376">ConfigrMgr 客户端启用的功能。</span><span class="sxs-lookup"><span data-stu-id="4267d-376">ConfigrMgr client enabled features.</span></span> <span data-ttu-id="4267d-377">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4267d-377">This property is read-only.</span></span> <span data-ttu-id="4267d-378">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4267d-378">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4267d-379">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="4267d-379">wiFiMacAddress</span></span>|<span data-ttu-id="4267d-380">String</span><span class="sxs-lookup"><span data-stu-id="4267d-380">String</span></span>|<span data-ttu-id="4267d-381">Wi-fi MAC。</span><span class="sxs-lookup"><span data-stu-id="4267d-381">Wi-Fi MAC.</span></span> <span data-ttu-id="4267d-382">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4267d-382">This property is read-only.</span></span> <span data-ttu-id="4267d-383">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4267d-383">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4267d-384">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="4267d-384">deviceHealthAttestationState</span></span>|[<span data-ttu-id="4267d-385">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="4267d-385">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="4267d-386">设备运行状况证明状态。</span><span class="sxs-lookup"><span data-stu-id="4267d-386">The device health attestation state.</span></span> <span data-ttu-id="4267d-387">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4267d-387">This property is read-only.</span></span> <span data-ttu-id="4267d-388">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4267d-388">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4267d-389">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="4267d-389">subscriberCarrier</span></span>|<span data-ttu-id="4267d-390">String</span><span class="sxs-lookup"><span data-stu-id="4267d-390">String</span></span>|<span data-ttu-id="4267d-391">订阅者运营商。</span><span class="sxs-lookup"><span data-stu-id="4267d-391">Subscriber Carrier.</span></span> <span data-ttu-id="4267d-392">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4267d-392">This property is read-only.</span></span> <span data-ttu-id="4267d-393">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4267d-393">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4267d-394">meid</span><span class="sxs-lookup"><span data-stu-id="4267d-394">meid</span></span>|<span data-ttu-id="4267d-395">String</span><span class="sxs-lookup"><span data-stu-id="4267d-395">String</span></span>|<span data-ttu-id="4267d-396">MEID.</span><span class="sxs-lookup"><span data-stu-id="4267d-396">MEID.</span></span> <span data-ttu-id="4267d-397">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4267d-397">This property is read-only.</span></span> <span data-ttu-id="4267d-398">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4267d-398">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4267d-399">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="4267d-399">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="4267d-400">Int64</span><span class="sxs-lookup"><span data-stu-id="4267d-400">Int64</span></span>|<span data-ttu-id="4267d-401">总存储量（以字节为单位）。</span><span class="sxs-lookup"><span data-stu-id="4267d-401">Total Storage in Bytes.</span></span> <span data-ttu-id="4267d-402">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4267d-402">This property is read-only.</span></span> <span data-ttu-id="4267d-403">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4267d-403">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4267d-404">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="4267d-404">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="4267d-405">Int64</span><span class="sxs-lookup"><span data-stu-id="4267d-405">Int64</span></span>|<span data-ttu-id="4267d-406">以字节为单位的可用存储空间。</span><span class="sxs-lookup"><span data-stu-id="4267d-406">Free Storage in Bytes.</span></span> <span data-ttu-id="4267d-407">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4267d-407">This property is read-only.</span></span> <span data-ttu-id="4267d-408">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4267d-408">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4267d-409">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="4267d-409">managedDeviceName</span></span>|<span data-ttu-id="4267d-410">String</span><span class="sxs-lookup"><span data-stu-id="4267d-410">String</span></span>|<span data-ttu-id="4267d-411">用于识别设备的自动生成的名称。</span><span class="sxs-lookup"><span data-stu-id="4267d-411">Automatically generated name to identify a device.</span></span> <span data-ttu-id="4267d-412">可以覆盖为用户友好名称。</span><span class="sxs-lookup"><span data-stu-id="4267d-412">Can be overwritten to a user friendly name.</span></span> <span data-ttu-id="4267d-413">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4267d-413">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4267d-414">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="4267d-414">partnerReportedThreatState</span></span>|[<span data-ttu-id="4267d-415">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="4267d-415">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="4267d-416">指示帐户和设备正在使用移动威胁防护合作伙伴时设备的威胁状态。</span><span class="sxs-lookup"><span data-stu-id="4267d-416">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="4267d-417">只读。</span><span class="sxs-lookup"><span data-stu-id="4267d-417">Read Only.</span></span> <span data-ttu-id="4267d-418">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4267d-418">This property is read-only.</span></span> <span data-ttu-id="4267d-419">继承自[managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="4267d-419">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="4267d-420">可取值为：`unknown`、`activated`、`deactivated`、`secured`、`lowSeverity`、`mediumSeverity`、`highSeverity`、`unresponsive`、`compromised`、`misconfigured`。</span><span class="sxs-lookup"><span data-stu-id="4267d-420">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="4267d-421">retireAfterDateTime</span><span class="sxs-lookup"><span data-stu-id="4267d-421">retireAfterDateTime</span></span>|<span data-ttu-id="4267d-422">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4267d-422">DateTimeOffset</span></span>|<span data-ttu-id="4267d-423">指示当设备因计划操作而自动停用的时间。</span><span class="sxs-lookup"><span data-stu-id="4267d-423">Indicates the time after when a device will be auto retired because of scheduled action.</span></span> <span data-ttu-id="4267d-424">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4267d-424">This property is read-only.</span></span> <span data-ttu-id="4267d-425">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4267d-425">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4267d-426">usersLoggedOn</span><span class="sxs-lookup"><span data-stu-id="4267d-426">usersLoggedOn</span></span>|<span data-ttu-id="4267d-427">[loggedOnUser](../resources/intune-devices-loggedonuser.md)集合</span><span class="sxs-lookup"><span data-stu-id="4267d-427">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="4267d-428">指示设备的上次登录用户。</span><span class="sxs-lookup"><span data-stu-id="4267d-428">Indicates the last logged on users of a device.</span></span> <span data-ttu-id="4267d-429">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4267d-429">This property is read-only.</span></span> <span data-ttu-id="4267d-430">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4267d-430">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4267d-431">preferMdmOverGroupPolicyAppliedDateTime</span><span class="sxs-lookup"><span data-stu-id="4267d-431">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="4267d-432">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4267d-432">DateTimeOffset</span></span>|<span data-ttu-id="4267d-433">报告设置了 preferMdmOverGroupPolicy 设置的 DateTime。</span><span class="sxs-lookup"><span data-stu-id="4267d-433">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="4267d-434">设置后，如果存在冲突，Intune MDM 设置将覆盖组策略设置。</span><span class="sxs-lookup"><span data-stu-id="4267d-434">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="4267d-435">只读。</span><span class="sxs-lookup"><span data-stu-id="4267d-435">Read Only.</span></span> <span data-ttu-id="4267d-436">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4267d-436">This property is read-only.</span></span> <span data-ttu-id="4267d-437">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4267d-437">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4267d-438">autopilotEnrolled</span><span class="sxs-lookup"><span data-stu-id="4267d-438">autopilotEnrolled</span></span>|<span data-ttu-id="4267d-439">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267d-439">Boolean</span></span>|<span data-ttu-id="4267d-440">如果托管设备是通过自动引导注册的，则报告。</span><span class="sxs-lookup"><span data-stu-id="4267d-440">Reports if the managed device is enrolled via auto-pilot.</span></span> <span data-ttu-id="4267d-441">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4267d-441">This property is read-only.</span></span> <span data-ttu-id="4267d-442">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4267d-442">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4267d-443">requireUserEnrollmentApproval</span><span class="sxs-lookup"><span data-stu-id="4267d-443">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="4267d-444">布尔值</span><span class="sxs-lookup"><span data-stu-id="4267d-444">Boolean</span></span>|<span data-ttu-id="4267d-445">如果托管 iOS 设备是用户审批注册，则报告。</span><span class="sxs-lookup"><span data-stu-id="4267d-445">Reports if the managed iOS device is user approval enrollment.</span></span> <span data-ttu-id="4267d-446">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4267d-446">This property is read-only.</span></span> <span data-ttu-id="4267d-447">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4267d-447">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4267d-448">managementCertificateExpirationDate</span><span class="sxs-lookup"><span data-stu-id="4267d-448">managementCertificateExpirationDate</span></span>|<span data-ttu-id="4267d-449">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4267d-449">DateTimeOffset</span></span>|<span data-ttu-id="4267d-450">报告设备管理证书到期日期。</span><span class="sxs-lookup"><span data-stu-id="4267d-450">Reports device management certificate expiration date.</span></span> <span data-ttu-id="4267d-451">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4267d-451">This property is read-only.</span></span> <span data-ttu-id="4267d-452">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4267d-452">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4267d-453">iccid</span><span class="sxs-lookup"><span data-stu-id="4267d-453">iccid</span></span>|<span data-ttu-id="4267d-454">String</span><span class="sxs-lookup"><span data-stu-id="4267d-454">String</span></span>|<span data-ttu-id="4267d-455">集成的电路卡标识符，它是 SIM 卡的唯一标识号。</span><span class="sxs-lookup"><span data-stu-id="4267d-455">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span> <span data-ttu-id="4267d-456">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4267d-456">This property is read-only.</span></span> <span data-ttu-id="4267d-457">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4267d-457">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4267d-458">udid</span><span class="sxs-lookup"><span data-stu-id="4267d-458">udid</span></span>|<span data-ttu-id="4267d-459">String</span><span class="sxs-lookup"><span data-stu-id="4267d-459">String</span></span>|<span data-ttu-id="4267d-460">IOS 和 macOS 设备的唯一设备标识符。</span><span class="sxs-lookup"><span data-stu-id="4267d-460">Unique Device Identifier for iOS and macOS devices.</span></span> <span data-ttu-id="4267d-461">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4267d-461">This property is read-only.</span></span> <span data-ttu-id="4267d-462">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4267d-462">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4267d-463">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4267d-463">roleScopeTagIds</span></span>|<span data-ttu-id="4267d-464">String collection</span><span class="sxs-lookup"><span data-stu-id="4267d-464">String collection</span></span>|<span data-ttu-id="4267d-465">此设备实例的范围标记 Id 的列表。</span><span class="sxs-lookup"><span data-stu-id="4267d-465">List of Scope Tag IDs for this Device instance.</span></span> <span data-ttu-id="4267d-466">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4267d-466">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4267d-467">windowsActiveMalwareCount</span><span class="sxs-lookup"><span data-stu-id="4267d-467">windowsActiveMalwareCount</span></span>|<span data-ttu-id="4267d-468">Int32</span><span class="sxs-lookup"><span data-stu-id="4267d-468">Int32</span></span>|<span data-ttu-id="4267d-469">此 windows 设备的活动恶意软件的计数。</span><span class="sxs-lookup"><span data-stu-id="4267d-469">Count of active malware for this windows device.</span></span> <span data-ttu-id="4267d-470">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4267d-470">This property is read-only.</span></span> <span data-ttu-id="4267d-471">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4267d-471">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4267d-472">windowsRemediatedMalwareCount</span><span class="sxs-lookup"><span data-stu-id="4267d-472">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="4267d-473">Int32</span><span class="sxs-lookup"><span data-stu-id="4267d-473">Int32</span></span>|<span data-ttu-id="4267d-474">此 windows 设备的修正的恶意软件的计数。</span><span class="sxs-lookup"><span data-stu-id="4267d-474">Count of remediated malware for this windows device.</span></span> <span data-ttu-id="4267d-475">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4267d-475">This property is read-only.</span></span> <span data-ttu-id="4267d-476">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4267d-476">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4267d-477">notes</span><span class="sxs-lookup"><span data-stu-id="4267d-477">notes</span></span>|<span data-ttu-id="4267d-478">String</span><span class="sxs-lookup"><span data-stu-id="4267d-478">String</span></span>|<span data-ttu-id="4267d-479">由 IT 管理员创建的设备上的注释继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4267d-479">Notes on the device created by IT Admin Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4267d-480">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="4267d-480">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="4267d-481">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="4267d-481">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="4267d-482">Configuration manager 客户端运行状况状态，仅适用于从[ManagedDevice](../resources/intune-devices-manageddevice.md)继承的 MDM/ConfigMgr 代理所管理的设备</span><span class="sxs-lookup"><span data-stu-id="4267d-482">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4267d-483">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="4267d-483">configurationManagerClientInformation</span></span>|[<span data-ttu-id="4267d-484">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="4267d-484">configurationManagerClientInformation</span></span>](../resources/intune-devices-configurationmanagerclientinformation.md)|<span data-ttu-id="4267d-485">Configuration manager 客户端信息，仅对由[ManagedDevice](../resources/intune-devices-manageddevice.md)继承的 ConfigMgr 代理、duel 管理或三方管理的设备有效</span><span class="sxs-lookup"><span data-stu-id="4267d-485">Configuration manager client information, valid only for devices managed, duel-managed or tri-managed by ConfigMgr Agent Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4267d-486">ethernetMacAddress</span><span class="sxs-lookup"><span data-stu-id="4267d-486">ethernetMacAddress</span></span>|<span data-ttu-id="4267d-487">String</span><span class="sxs-lookup"><span data-stu-id="4267d-487">String</span></span>|<span data-ttu-id="4267d-488">以太网 MAC。</span><span class="sxs-lookup"><span data-stu-id="4267d-488">Ethernet MAC.</span></span> <span data-ttu-id="4267d-489">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4267d-489">This property is read-only.</span></span> <span data-ttu-id="4267d-490">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4267d-490">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4267d-491">physicalMemoryInBytes</span><span class="sxs-lookup"><span data-stu-id="4267d-491">physicalMemoryInBytes</span></span>|<span data-ttu-id="4267d-492">Int64</span><span class="sxs-lookup"><span data-stu-id="4267d-492">Int64</span></span>|<span data-ttu-id="4267d-493">内存总量（以字节为单位）。</span><span class="sxs-lookup"><span data-stu-id="4267d-493">Total Memory in Bytes.</span></span> <span data-ttu-id="4267d-494">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4267d-494">This property is read-only.</span></span> <span data-ttu-id="4267d-495">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="4267d-495">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="4267d-496">processorArchitecture</span><span class="sxs-lookup"><span data-stu-id="4267d-496">processorArchitecture</span></span>|[<span data-ttu-id="4267d-497">managedDeviceArchitecture</span><span class="sxs-lookup"><span data-stu-id="4267d-497">managedDeviceArchitecture</span></span>](../resources/intune-devices-manageddevicearchitecture.md)|<span data-ttu-id="4267d-498">处理器体系结构。</span><span class="sxs-lookup"><span data-stu-id="4267d-498">Processor architecture.</span></span> <span data-ttu-id="4267d-499">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4267d-499">This property is read-only.</span></span> <span data-ttu-id="4267d-500">继承自[managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="4267d-500">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="4267d-501">可取值为：`unknown`、`x86`、`x64`、`arm`、`arM64`。</span><span class="sxs-lookup"><span data-stu-id="4267d-501">Possible values are: `unknown`, `x86`, `x64`, `arm`, `arM64`.</span></span>|



## <a name="response"></a><span data-ttu-id="4267d-502">响应</span><span class="sxs-lookup"><span data-stu-id="4267d-502">Response</span></span>
<span data-ttu-id="4267d-503">如果成功，此方法在响应`201 Created`正文中返回响应代码和[windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4267d-503">If successful, this method returns a `201 Created` response code and a [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4267d-504">示例</span><span class="sxs-lookup"><span data-stu-id="4267d-504">Example</span></span>

### <a name="request"></a><span data-ttu-id="4267d-505">请求</span><span class="sxs-lookup"><span data-stu-id="4267d-505">Request</span></span>
<span data-ttu-id="4267d-506">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4267d-506">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices
Content-type: application/json
Content-length: 7665

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
  "processorArchitecture": "x86"
}
```

### <a name="response"></a><span data-ttu-id="4267d-507">响应</span><span class="sxs-lookup"><span data-stu-id="4267d-507">Response</span></span>
<span data-ttu-id="4267d-p171">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4267d-p171">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 7714

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
  "processorArchitecture": "x86"
}
```




