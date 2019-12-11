---
title: 创建 windowsManagedDevice
description: 创建新的 windowsManagedDevice 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e410bc5dbda16c30a4f9bed9e95aa85ffc1dfd05
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39944291"
---
# <a name="create-windowsmanageddevice"></a><span data-ttu-id="5e53f-103">创建 windowsManagedDevice</span><span class="sxs-lookup"><span data-stu-id="5e53f-103">Create windowsManagedDevice</span></span>

> <span data-ttu-id="5e53f-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5e53f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5e53f-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5e53f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5e53f-106">创建新的[windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md)对象。</span><span class="sxs-lookup"><span data-stu-id="5e53f-106">Create a new [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5e53f-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="5e53f-107">Prerequisites</span></span>
<span data-ttu-id="5e53f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5e53f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e53f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="5e53f-110">Permission type</span></span>|<span data-ttu-id="5e53f-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5e53f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5e53f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5e53f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5e53f-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e53f-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="5e53f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5e53f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5e53f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="5e53f-115">Not supported.</span></span>|
|<span data-ttu-id="5e53f-116">Application</span><span class="sxs-lookup"><span data-stu-id="5e53f-116">Application</span></span>|<span data-ttu-id="5e53f-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e53f-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5e53f-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5e53f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices
```

## <a name="request-headers"></a><span data-ttu-id="5e53f-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="5e53f-119">Request headers</span></span>
|<span data-ttu-id="5e53f-120">标头</span><span class="sxs-lookup"><span data-stu-id="5e53f-120">Header</span></span>|<span data-ttu-id="5e53f-121">值</span><span class="sxs-lookup"><span data-stu-id="5e53f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5e53f-122">授权</span><span class="sxs-lookup"><span data-stu-id="5e53f-122">Authorization</span></span>|<span data-ttu-id="5e53f-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5e53f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5e53f-124">接受</span><span class="sxs-lookup"><span data-stu-id="5e53f-124">Accept</span></span>|<span data-ttu-id="5e53f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5e53f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5e53f-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="5e53f-126">Request body</span></span>
<span data-ttu-id="5e53f-127">在请求正文中，提供 windowsManagedDevice 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5e53f-127">In the request body, supply a JSON representation for the windowsManagedDevice object.</span></span>

<span data-ttu-id="5e53f-128">下表显示创建 windowsManagedDevice 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="5e53f-128">The following table shows the properties that are required when you create the windowsManagedDevice.</span></span>

|<span data-ttu-id="5e53f-129">属性</span><span class="sxs-lookup"><span data-stu-id="5e53f-129">Property</span></span>|<span data-ttu-id="5e53f-130">类型</span><span class="sxs-lookup"><span data-stu-id="5e53f-130">Type</span></span>|<span data-ttu-id="5e53f-131">说明</span><span class="sxs-lookup"><span data-stu-id="5e53f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e53f-132">id</span><span class="sxs-lookup"><span data-stu-id="5e53f-132">id</span></span>|<span data-ttu-id="5e53f-133">字符串</span><span class="sxs-lookup"><span data-stu-id="5e53f-133">String</span></span>|<span data-ttu-id="5e53f-134">设备的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="5e53f-134">Unique Identifier for the device.</span></span> <span data-ttu-id="5e53f-135">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5e53f-135">This property is read-only.</span></span> <span data-ttu-id="5e53f-136">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="5e53f-136">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="5e53f-137">userId</span><span class="sxs-lookup"><span data-stu-id="5e53f-137">userId</span></span>|<span data-ttu-id="5e53f-138">String</span><span class="sxs-lookup"><span data-stu-id="5e53f-138">String</span></span>|<span data-ttu-id="5e53f-139">与设备关联的用户的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="5e53f-139">Unique Identifier for the user associated with the device.</span></span> <span data-ttu-id="5e53f-140">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5e53f-140">This property is read-only.</span></span> <span data-ttu-id="5e53f-141">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="5e53f-141">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="5e53f-142">deviceName</span><span class="sxs-lookup"><span data-stu-id="5e53f-142">deviceName</span></span>|<span data-ttu-id="5e53f-143">字符串</span><span class="sxs-lookup"><span data-stu-id="5e53f-143">String</span></span>|<span data-ttu-id="5e53f-144">设备的名称。</span><span class="sxs-lookup"><span data-stu-id="5e53f-144">Name of the device.</span></span> <span data-ttu-id="5e53f-145">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5e53f-145">This property is read-only.</span></span> <span data-ttu-id="5e53f-146">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="5e53f-146">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="5e53f-147">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="5e53f-147">hardwareInformation</span></span>|[<span data-ttu-id="5e53f-148">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="5e53f-148">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="5e53f-149">设备的 hardward 详细信息。</span><span class="sxs-lookup"><span data-stu-id="5e53f-149">The hardward details for the device.</span></span>  <span data-ttu-id="5e53f-150">包括存储空间、制造商、序列号等信息。此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5e53f-150">Includes information such as storage space, manufacturer, serial number, etc. This property is read-only.</span></span> <span data-ttu-id="5e53f-151">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="5e53f-151">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="5e53f-152">所有者</span><span class="sxs-lookup"><span data-stu-id="5e53f-152">ownerType</span></span>|[<span data-ttu-id="5e53f-153">所有者</span><span class="sxs-lookup"><span data-stu-id="5e53f-153">ownerType</span></span>](../resources/intune-shared-ownertype.md)|<span data-ttu-id="5e53f-154">设备的所有权。</span><span class="sxs-lookup"><span data-stu-id="5e53f-154">Ownership of the device.</span></span> <span data-ttu-id="5e53f-155">可以是从[ManagedDevice](../resources/intune-devices-manageddevice.md)继承的 "公司" 或 "个人"。</span><span class="sxs-lookup"><span data-stu-id="5e53f-155">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="5e53f-156">可取值为：`unknown`、`company`、`personal`。</span><span class="sxs-lookup"><span data-stu-id="5e53f-156">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="5e53f-157">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="5e53f-157">managedDeviceOwnerType</span></span>|[<span data-ttu-id="5e53f-158">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="5e53f-158">managedDeviceOwnerType</span></span>](../resources/intune-shared-manageddeviceownertype.md)|<span data-ttu-id="5e53f-159">设备的所有权。</span><span class="sxs-lookup"><span data-stu-id="5e53f-159">Ownership of the device.</span></span> <span data-ttu-id="5e53f-160">可以是从[ManagedDevice](../resources/intune-devices-manageddevice.md)继承的 "公司" 或 "个人"。</span><span class="sxs-lookup"><span data-stu-id="5e53f-160">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="5e53f-161">可取值为：`unknown`、`company`、`personal`。</span><span class="sxs-lookup"><span data-stu-id="5e53f-161">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="5e53f-162">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="5e53f-162">deviceActionResults</span></span>|<span data-ttu-id="5e53f-163">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5e53f-163">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="5e53f-164">ComplexType deviceActionResult 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="5e53f-164">List of ComplexType deviceActionResult objects.</span></span> <span data-ttu-id="5e53f-165">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5e53f-165">This property is read-only.</span></span> <span data-ttu-id="5e53f-166">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="5e53f-166">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="5e53f-167">managementState</span><span class="sxs-lookup"><span data-stu-id="5e53f-167">managementState</span></span>|[<span data-ttu-id="5e53f-168">managementState</span><span class="sxs-lookup"><span data-stu-id="5e53f-168">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="5e53f-169">设备的管理状态。</span><span class="sxs-lookup"><span data-stu-id="5e53f-169">Management state of the device.</span></span> <span data-ttu-id="5e53f-170">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5e53f-170">This property is read-only.</span></span> <span data-ttu-id="5e53f-171">继承自[managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="5e53f-171">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="5e53f-172">可取值为：`managed`、`retirePending`、`retireFailed`、`wipePending`、`wipeFailed`、`unhealthy`、`deletePending`、`retireIssued`、`wipeIssued`、`wipeCanceled`、`retireCanceled`、`discovered`。</span><span class="sxs-lookup"><span data-stu-id="5e53f-172">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="5e53f-173">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="5e53f-173">enrolledDateTime</span></span>|<span data-ttu-id="5e53f-174">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e53f-174">DateTimeOffset</span></span>|<span data-ttu-id="5e53f-175">设备的注册时间。</span><span class="sxs-lookup"><span data-stu-id="5e53f-175">Enrollment time of the device.</span></span> <span data-ttu-id="5e53f-176">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5e53f-176">This property is read-only.</span></span> <span data-ttu-id="5e53f-177">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="5e53f-177">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="5e53f-178">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="5e53f-178">lastSyncDateTime</span></span>|<span data-ttu-id="5e53f-179">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e53f-179">DateTimeOffset</span></span>|<span data-ttu-id="5e53f-180">设备上次成功完成与 Intune 同步的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="5e53f-180">The date and time that the device last completed a successful sync with Intune.</span></span> <span data-ttu-id="5e53f-181">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5e53f-181">This property is read-only.</span></span> <span data-ttu-id="5e53f-182">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="5e53f-182">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="5e53f-183">chassisType</span><span class="sxs-lookup"><span data-stu-id="5e53f-183">chassisType</span></span>|[<span data-ttu-id="5e53f-184">chassisType</span><span class="sxs-lookup"><span data-stu-id="5e53f-184">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="5e53f-185">设备的机箱类型。</span><span class="sxs-lookup"><span data-stu-id="5e53f-185">Chassis type of the device.</span></span> <span data-ttu-id="5e53f-186">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5e53f-186">This property is read-only.</span></span> <span data-ttu-id="5e53f-187">继承自[managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="5e53f-187">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="5e53f-188">可取值为：`unknown`、`desktop`、`laptop`、`worksWorkstation`、`enterpriseServer`、`phone`、`tablet`、`mobileOther`、`mobileUnknown`。</span><span class="sxs-lookup"><span data-stu-id="5e53f-188">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="5e53f-189">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="5e53f-189">operatingSystem</span></span>|<span data-ttu-id="5e53f-190">字符串</span><span class="sxs-lookup"><span data-stu-id="5e53f-190">String</span></span>|<span data-ttu-id="5e53f-191">设备的操作系统。</span><span class="sxs-lookup"><span data-stu-id="5e53f-191">Operating system of the device.</span></span> <span data-ttu-id="5e53f-192">Windows、iOS 等。此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5e53f-192">Windows, iOS, etc. This property is read-only.</span></span> <span data-ttu-id="5e53f-193">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="5e53f-193">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="5e53f-194">deviceType</span><span class="sxs-lookup"><span data-stu-id="5e53f-194">deviceType</span></span>|[<span data-ttu-id="5e53f-195">deviceType</span><span class="sxs-lookup"><span data-stu-id="5e53f-195">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="5e53f-196">设备的平台。</span><span class="sxs-lookup"><span data-stu-id="5e53f-196">Platform of the device.</span></span> <span data-ttu-id="5e53f-197">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5e53f-197">This property is read-only.</span></span> <span data-ttu-id="5e53f-198">继承自[managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="5e53f-198">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="5e53f-199">可能的值为`desktop`： `windowsRT`、 `winMO6`、 `nokia` `windowsPhone` `mac` `winCE` `palm` `unknown`、、、、、、、、、、、、、、、、、、、。 `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `blackberry`</span><span class="sxs-lookup"><span data-stu-id="5e53f-199">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="5e53f-200">complianceState</span><span class="sxs-lookup"><span data-stu-id="5e53f-200">complianceState</span></span>|[<span data-ttu-id="5e53f-201">complianceState</span><span class="sxs-lookup"><span data-stu-id="5e53f-201">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="5e53f-202">设备的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="5e53f-202">Compliance state of the device.</span></span> <span data-ttu-id="5e53f-203">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5e53f-203">This property is read-only.</span></span> <span data-ttu-id="5e53f-204">继承自[managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="5e53f-204">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="5e53f-205">可取值为：`unknown`、`compliant`、`noncompliant`、`conflict`、`error`、`inGracePeriod`、`configManager`。</span><span class="sxs-lookup"><span data-stu-id="5e53f-205">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="5e53f-206">jailBroken</span><span class="sxs-lookup"><span data-stu-id="5e53f-206">jailBroken</span></span>|<span data-ttu-id="5e53f-207">String</span><span class="sxs-lookup"><span data-stu-id="5e53f-207">String</span></span>|<span data-ttu-id="5e53f-208">设备是否已越狱或取得 root 权限。</span><span class="sxs-lookup"><span data-stu-id="5e53f-208">whether the device is jail broken or rooted.</span></span> <span data-ttu-id="5e53f-209">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5e53f-209">This property is read-only.</span></span> <span data-ttu-id="5e53f-210">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="5e53f-210">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="5e53f-211">managementAgent</span><span class="sxs-lookup"><span data-stu-id="5e53f-211">managementAgent</span></span>|[<span data-ttu-id="5e53f-212">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="5e53f-212">managementAgentType</span></span>](../resources/intune-shared-managementagenttype.md)|<span data-ttu-id="5e53f-213">设备的管理通道。</span><span class="sxs-lookup"><span data-stu-id="5e53f-213">Management channel of the device.</span></span> <span data-ttu-id="5e53f-214">Intune、EAS 等。此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5e53f-214">Intune, EAS, etc. This property is read-only.</span></span> <span data-ttu-id="5e53f-215">继承自[managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="5e53f-215">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="5e53f-216">可取值为：`eas`、`mdm`、`easMdm`、`intuneClient`、`easIntuneClient`、`configurationManagerClient`、`configurationManagerClientMdm`、`configurationManagerClientMdmEas`、`unknown`、`jamf`、`googleCloudDevicePolicyController`、`microsoft365ManagedMdm`。</span><span class="sxs-lookup"><span data-stu-id="5e53f-216">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span></span>|
|<span data-ttu-id="5e53f-217">osVersion</span><span class="sxs-lookup"><span data-stu-id="5e53f-217">osVersion</span></span>|<span data-ttu-id="5e53f-218">String</span><span class="sxs-lookup"><span data-stu-id="5e53f-218">String</span></span>|<span data-ttu-id="5e53f-219">设备的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="5e53f-219">Operating system version of the device.</span></span> <span data-ttu-id="5e53f-220">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5e53f-220">This property is read-only.</span></span> <span data-ttu-id="5e53f-221">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="5e53f-221">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="5e53f-222">easActivated</span><span class="sxs-lookup"><span data-stu-id="5e53f-222">easActivated</span></span>|<span data-ttu-id="5e53f-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="5e53f-223">Boolean</span></span>|<span data-ttu-id="5e53f-224">设备是否已激活 Exchange ActiveSync。</span><span class="sxs-lookup"><span data-stu-id="5e53f-224">Whether the device is Exchange ActiveSync activated.</span></span> <span data-ttu-id="5e53f-225">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5e53f-225">This property is read-only.</span></span> <span data-ttu-id="5e53f-226">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="5e53f-226">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="5e53f-227">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="5e53f-227">easDeviceId</span></span>|<span data-ttu-id="5e53f-228">字符串</span><span class="sxs-lookup"><span data-stu-id="5e53f-228">String</span></span>|<span data-ttu-id="5e53f-229">设备的 Exchange ActiveSync ID。</span><span class="sxs-lookup"><span data-stu-id="5e53f-229">Exchange ActiveSync Id of the device.</span></span> <span data-ttu-id="5e53f-230">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5e53f-230">This property is read-only.</span></span> <span data-ttu-id="5e53f-231">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="5e53f-231">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="5e53f-232">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="5e53f-232">easActivationDateTime</span></span>|<span data-ttu-id="5e53f-233">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e53f-233">DateTimeOffset</span></span>|<span data-ttu-id="5e53f-234">设备的 Exchange ActivationSync 激活时间。</span><span class="sxs-lookup"><span data-stu-id="5e53f-234">Exchange ActivationSync activation time of the device.</span></span> <span data-ttu-id="5e53f-235">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5e53f-235">This property is read-only.</span></span> <span data-ttu-id="5e53f-236">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="5e53f-236">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="5e53f-237">aadRegistered</span><span class="sxs-lookup"><span data-stu-id="5e53f-237">aadRegistered</span></span>|<span data-ttu-id="5e53f-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="5e53f-238">Boolean</span></span>|<span data-ttu-id="5e53f-239">设备是否已注册 Azure Active Directory。</span><span class="sxs-lookup"><span data-stu-id="5e53f-239">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="5e53f-240">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5e53f-240">This property is read-only.</span></span> <span data-ttu-id="5e53f-241">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="5e53f-241">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="5e53f-242">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="5e53f-242">azureADRegistered</span></span>|<span data-ttu-id="5e53f-243">Boolean</span><span class="sxs-lookup"><span data-stu-id="5e53f-243">Boolean</span></span>|<span data-ttu-id="5e53f-244">设备是否已注册 Azure Active Directory。</span><span class="sxs-lookup"><span data-stu-id="5e53f-244">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="5e53f-245">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5e53f-245">This property is read-only.</span></span> <span data-ttu-id="5e53f-246">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="5e53f-246">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="5e53f-247">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="5e53f-247">deviceEnrollmentType</span></span>|[<span data-ttu-id="5e53f-248">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="5e53f-248">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="5e53f-249">设备的注册类型。</span><span class="sxs-lookup"><span data-stu-id="5e53f-249">Enrollment type of the device.</span></span> <span data-ttu-id="5e53f-250">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5e53f-250">This property is read-only.</span></span> <span data-ttu-id="5e53f-251">继承自[managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="5e53f-251">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="5e53f-252">可取值为：`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement`、`appleUserEnrollment`、`appleUserEnrollmentWithServiceAccount`。</span><span class="sxs-lookup"><span data-stu-id="5e53f-252">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`.</span></span>|
|<span data-ttu-id="5e53f-253">lostModeState</span><span class="sxs-lookup"><span data-stu-id="5e53f-253">lostModeState</span></span>|[<span data-ttu-id="5e53f-254">lostModeState</span><span class="sxs-lookup"><span data-stu-id="5e53f-254">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="5e53f-255">指示是否已启用或禁用了丢失模式。</span><span class="sxs-lookup"><span data-stu-id="5e53f-255">Indicates if Lost mode is enabled or disabled.</span></span> <span data-ttu-id="5e53f-256">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5e53f-256">This property is read-only.</span></span> <span data-ttu-id="5e53f-257">继承自[managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="5e53f-257">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="5e53f-258">可取值为：`disabled`、`enabled`。</span><span class="sxs-lookup"><span data-stu-id="5e53f-258">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="5e53f-259">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="5e53f-259">activationLockBypassCode</span></span>|<span data-ttu-id="5e53f-260">字符串</span><span class="sxs-lookup"><span data-stu-id="5e53f-260">String</span></span>|<span data-ttu-id="5e53f-261">允许绕过设备上的激活锁的代码。</span><span class="sxs-lookup"><span data-stu-id="5e53f-261">Code that allows the Activation Lock on a device to be bypassed.</span></span> <span data-ttu-id="5e53f-262">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5e53f-262">This property is read-only.</span></span> <span data-ttu-id="5e53f-263">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="5e53f-263">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="5e53f-264">emailAddress</span><span class="sxs-lookup"><span data-stu-id="5e53f-264">emailAddress</span></span>|<span data-ttu-id="5e53f-265">字符串</span><span class="sxs-lookup"><span data-stu-id="5e53f-265">String</span></span>|<span data-ttu-id="5e53f-266">与设备关联的用户的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="5e53f-266">Email(s) for the user associated with the device.</span></span> <span data-ttu-id="5e53f-267">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5e53f-267">This property is read-only.</span></span> <span data-ttu-id="5e53f-268">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="5e53f-268">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="5e53f-269">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="5e53f-269">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="5e53f-270">字符串</span><span class="sxs-lookup"><span data-stu-id="5e53f-270">String</span></span>|<span data-ttu-id="5e53f-271">Azure Active Directory 设备的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="5e53f-271">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="5e53f-272">只读。</span><span class="sxs-lookup"><span data-stu-id="5e53f-272">Read only.</span></span> <span data-ttu-id="5e53f-273">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5e53f-273">This property is read-only.</span></span> <span data-ttu-id="5e53f-274">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="5e53f-274">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="5e53f-275">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="5e53f-275">azureADDeviceId</span></span>|<span data-ttu-id="5e53f-276">字符串</span><span class="sxs-lookup"><span data-stu-id="5e53f-276">String</span></span>|<span data-ttu-id="5e53f-277">Azure Active Directory 设备的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="5e53f-277">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="5e53f-278">只读。</span><span class="sxs-lookup"><span data-stu-id="5e53f-278">Read only.</span></span> <span data-ttu-id="5e53f-279">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5e53f-279">This property is read-only.</span></span> <span data-ttu-id="5e53f-280">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="5e53f-280">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="5e53f-281">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="5e53f-281">deviceRegistrationState</span></span>|[<span data-ttu-id="5e53f-282">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="5e53f-282">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="5e53f-283">设备注册状态。</span><span class="sxs-lookup"><span data-stu-id="5e53f-283">Device registration state.</span></span> <span data-ttu-id="5e53f-284">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5e53f-284">This property is read-only.</span></span> <span data-ttu-id="5e53f-285">继承自[managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="5e53f-285">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="5e53f-286">可取值为：`notRegistered`、`registered`、`revoked`、`keyConflict`、`approvalPending`、`certificateReset`、`notRegisteredPendingEnrollment`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="5e53f-286">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="5e53f-287">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="5e53f-287">deviceCategoryDisplayName</span></span>|<span data-ttu-id="5e53f-288">字符串</span><span class="sxs-lookup"><span data-stu-id="5e53f-288">String</span></span>|<span data-ttu-id="5e53f-289">设备类别显示名称。</span><span class="sxs-lookup"><span data-stu-id="5e53f-289">Device category display name.</span></span> <span data-ttu-id="5e53f-290">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5e53f-290">This property is read-only.</span></span> <span data-ttu-id="5e53f-291">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="5e53f-291">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="5e53f-292">isSupervised</span><span class="sxs-lookup"><span data-stu-id="5e53f-292">isSupervised</span></span>|<span data-ttu-id="5e53f-293">Boolean</span><span class="sxs-lookup"><span data-stu-id="5e53f-293">Boolean</span></span>|<span data-ttu-id="5e53f-294">设备监督状态。</span><span class="sxs-lookup"><span data-stu-id="5e53f-294">Device supervised status.</span></span> <span data-ttu-id="5e53f-295">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5e53f-295">This property is read-only.</span></span> <span data-ttu-id="5e53f-296">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="5e53f-296">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="5e53f-297">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="5e53f-297">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="5e53f-298">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e53f-298">DateTimeOffset</span></span>|<span data-ttu-id="5e53f-299">设备上次与 Exchange 联系的时间。</span><span class="sxs-lookup"><span data-stu-id="5e53f-299">Last time the device contacted Exchange.</span></span> <span data-ttu-id="5e53f-300">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5e53f-300">This property is read-only.</span></span> <span data-ttu-id="5e53f-301">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="5e53f-301">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="5e53f-302">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="5e53f-302">exchangeAccessState</span></span>|[<span data-ttu-id="5e53f-303">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="5e53f-303">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="5e53f-304">Exchange 中设备的访问状态。</span><span class="sxs-lookup"><span data-stu-id="5e53f-304">The Access State of the device in Exchange.</span></span> <span data-ttu-id="5e53f-305">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5e53f-305">This property is read-only.</span></span> <span data-ttu-id="5e53f-306">继承自[managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="5e53f-306">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="5e53f-307">可取值为：`none`、`unknown`、`allowed`、`blocked`、`quarantined`。</span><span class="sxs-lookup"><span data-stu-id="5e53f-307">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="5e53f-308">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="5e53f-308">exchangeAccessStateReason</span></span>|[<span data-ttu-id="5e53f-309">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="5e53f-309">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="5e53f-310">Exchange 中设备访问状态的出现原因。</span><span class="sxs-lookup"><span data-stu-id="5e53f-310">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="5e53f-311">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5e53f-311">This property is read-only.</span></span> <span data-ttu-id="5e53f-312">继承自[managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="5e53f-312">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="5e53f-313">可取值为：`none`、`unknown`、`exchangeGlobalRule`、`exchangeIndividualRule`、`exchangeDeviceRule`、`exchangeUpgrade`、`exchangeMailboxPolicy`、`other`、`compliant`、`notCompliant`、`notEnrolled`、`unknownLocation`、`mfaRequired`、`azureADBlockDueToAccessPolicy`、`compromisedPassword`、`deviceNotKnownWithManagedApp`。</span><span class="sxs-lookup"><span data-stu-id="5e53f-313">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="5e53f-314">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="5e53f-314">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="5e53f-315">字符串</span><span class="sxs-lookup"><span data-stu-id="5e53f-315">String</span></span>|<span data-ttu-id="5e53f-316">允许与设备建立远程协助会话的 URL。</span><span class="sxs-lookup"><span data-stu-id="5e53f-316">Url that allows a Remote Assistance session to be established with the device.</span></span> <span data-ttu-id="5e53f-317">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5e53f-317">This property is read-only.</span></span> <span data-ttu-id="5e53f-318">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="5e53f-318">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="5e53f-319">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="5e53f-319">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="5e53f-320">String</span><span class="sxs-lookup"><span data-stu-id="5e53f-320">String</span></span>|<span data-ttu-id="5e53f-321">用于在创建远程协助会话对象时识别问题的错误字符串。</span><span class="sxs-lookup"><span data-stu-id="5e53f-321">An error string that identifies issues when creating Remote Assistance session objects.</span></span> <span data-ttu-id="5e53f-322">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5e53f-322">This property is read-only.</span></span> <span data-ttu-id="5e53f-323">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="5e53f-323">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="5e53f-324">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="5e53f-324">isEncrypted</span></span>|<span data-ttu-id="5e53f-325">Boolean</span><span class="sxs-lookup"><span data-stu-id="5e53f-325">Boolean</span></span>|<span data-ttu-id="5e53f-326">设备加密状态。</span><span class="sxs-lookup"><span data-stu-id="5e53f-326">Device encryption status.</span></span> <span data-ttu-id="5e53f-327">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5e53f-327">This property is read-only.</span></span> <span data-ttu-id="5e53f-328">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="5e53f-328">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="5e53f-329">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="5e53f-329">userPrincipalName</span></span>|<span data-ttu-id="5e53f-330">字符串</span><span class="sxs-lookup"><span data-stu-id="5e53f-330">String</span></span>|<span data-ttu-id="5e53f-331">设备用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="5e53f-331">Device user principal name.</span></span> <span data-ttu-id="5e53f-332">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5e53f-332">This property is read-only.</span></span> <span data-ttu-id="5e53f-333">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="5e53f-333">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="5e53f-334">model</span><span class="sxs-lookup"><span data-stu-id="5e53f-334">model</span></span>|<span data-ttu-id="5e53f-335">字符串</span><span class="sxs-lookup"><span data-stu-id="5e53f-335">String</span></span>|<span data-ttu-id="5e53f-336">设备的模型。</span><span class="sxs-lookup"><span data-stu-id="5e53f-336">Model of the device.</span></span> <span data-ttu-id="5e53f-337">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5e53f-337">This property is read-only.</span></span> <span data-ttu-id="5e53f-338">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="5e53f-338">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="5e53f-339">manufacturer</span><span class="sxs-lookup"><span data-stu-id="5e53f-339">manufacturer</span></span>|<span data-ttu-id="5e53f-340">字符串</span><span class="sxs-lookup"><span data-stu-id="5e53f-340">String</span></span>|<span data-ttu-id="5e53f-341">设备的制造商。</span><span class="sxs-lookup"><span data-stu-id="5e53f-341">Manufacturer of the device.</span></span> <span data-ttu-id="5e53f-342">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5e53f-342">This property is read-only.</span></span> <span data-ttu-id="5e53f-343">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="5e53f-343">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="5e53f-344">imei</span><span class="sxs-lookup"><span data-stu-id="5e53f-344">imei</span></span>|<span data-ttu-id="5e53f-345">字符串</span><span class="sxs-lookup"><span data-stu-id="5e53f-345">String</span></span>|<span data-ttu-id="5e53f-346">IMEI.</span><span class="sxs-lookup"><span data-stu-id="5e53f-346">IMEI.</span></span> <span data-ttu-id="5e53f-347">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5e53f-347">This property is read-only.</span></span> <span data-ttu-id="5e53f-348">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="5e53f-348">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="5e53f-349">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="5e53f-349">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="5e53f-350">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e53f-350">DateTimeOffset</span></span>|<span data-ttu-id="5e53f-351">设备符合性宽限期到期时的日期时间。</span><span class="sxs-lookup"><span data-stu-id="5e53f-351">The DateTime when device compliance grace period expires.</span></span> <span data-ttu-id="5e53f-352">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5e53f-352">This property is read-only.</span></span> <span data-ttu-id="5e53f-353">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="5e53f-353">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="5e53f-354">serialNumber</span><span class="sxs-lookup"><span data-stu-id="5e53f-354">serialNumber</span></span>|<span data-ttu-id="5e53f-355">字符串</span><span class="sxs-lookup"><span data-stu-id="5e53f-355">String</span></span>|<span data-ttu-id="5e53f-356">SerialNumber.</span><span class="sxs-lookup"><span data-stu-id="5e53f-356">SerialNumber.</span></span> <span data-ttu-id="5e53f-357">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5e53f-357">This property is read-only.</span></span> <span data-ttu-id="5e53f-358">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="5e53f-358">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="5e53f-359">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="5e53f-359">phoneNumber</span></span>|<span data-ttu-id="5e53f-360">字符串</span><span class="sxs-lookup"><span data-stu-id="5e53f-360">String</span></span>|<span data-ttu-id="5e53f-361">设备的电话号码。</span><span class="sxs-lookup"><span data-stu-id="5e53f-361">Phone number of the device.</span></span> <span data-ttu-id="5e53f-362">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5e53f-362">This property is read-only.</span></span> <span data-ttu-id="5e53f-363">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="5e53f-363">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="5e53f-364">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="5e53f-364">androidSecurityPatchLevel</span></span>|<span data-ttu-id="5e53f-365">字符串</span><span class="sxs-lookup"><span data-stu-id="5e53f-365">String</span></span>|<span data-ttu-id="5e53f-366">Android 安全修补程序级别。</span><span class="sxs-lookup"><span data-stu-id="5e53f-366">Android security patch level.</span></span> <span data-ttu-id="5e53f-367">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5e53f-367">This property is read-only.</span></span> <span data-ttu-id="5e53f-368">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="5e53f-368">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="5e53f-369">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="5e53f-369">userDisplayName</span></span>|<span data-ttu-id="5e53f-370">String</span><span class="sxs-lookup"><span data-stu-id="5e53f-370">String</span></span>|<span data-ttu-id="5e53f-371">用户显示名称。</span><span class="sxs-lookup"><span data-stu-id="5e53f-371">User display name.</span></span> <span data-ttu-id="5e53f-372">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5e53f-372">This property is read-only.</span></span> <span data-ttu-id="5e53f-373">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="5e53f-373">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="5e53f-374">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="5e53f-374">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="5e53f-375">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="5e53f-375">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="5e53f-376">ConfigrMgr 客户端启用的功能。</span><span class="sxs-lookup"><span data-stu-id="5e53f-376">ConfigrMgr client enabled features.</span></span> <span data-ttu-id="5e53f-377">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5e53f-377">This property is read-only.</span></span> <span data-ttu-id="5e53f-378">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="5e53f-378">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="5e53f-379">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="5e53f-379">wiFiMacAddress</span></span>|<span data-ttu-id="5e53f-380">字符串</span><span class="sxs-lookup"><span data-stu-id="5e53f-380">String</span></span>|<span data-ttu-id="5e53f-381">Wi-fi MAC。</span><span class="sxs-lookup"><span data-stu-id="5e53f-381">Wi-Fi MAC.</span></span> <span data-ttu-id="5e53f-382">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5e53f-382">This property is read-only.</span></span> <span data-ttu-id="5e53f-383">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="5e53f-383">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="5e53f-384">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="5e53f-384">deviceHealthAttestationState</span></span>|[<span data-ttu-id="5e53f-385">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="5e53f-385">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="5e53f-386">设备运行状况证明状态。</span><span class="sxs-lookup"><span data-stu-id="5e53f-386">The device health attestation state.</span></span> <span data-ttu-id="5e53f-387">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5e53f-387">This property is read-only.</span></span> <span data-ttu-id="5e53f-388">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="5e53f-388">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="5e53f-389">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="5e53f-389">subscriberCarrier</span></span>|<span data-ttu-id="5e53f-390">字符串</span><span class="sxs-lookup"><span data-stu-id="5e53f-390">String</span></span>|<span data-ttu-id="5e53f-391">订阅者运营商。</span><span class="sxs-lookup"><span data-stu-id="5e53f-391">Subscriber Carrier.</span></span> <span data-ttu-id="5e53f-392">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5e53f-392">This property is read-only.</span></span> <span data-ttu-id="5e53f-393">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="5e53f-393">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="5e53f-394">meid</span><span class="sxs-lookup"><span data-stu-id="5e53f-394">meid</span></span>|<span data-ttu-id="5e53f-395">字符串</span><span class="sxs-lookup"><span data-stu-id="5e53f-395">String</span></span>|<span data-ttu-id="5e53f-396">MEID.</span><span class="sxs-lookup"><span data-stu-id="5e53f-396">MEID.</span></span> <span data-ttu-id="5e53f-397">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5e53f-397">This property is read-only.</span></span> <span data-ttu-id="5e53f-398">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="5e53f-398">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="5e53f-399">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="5e53f-399">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="5e53f-400">Int64</span><span class="sxs-lookup"><span data-stu-id="5e53f-400">Int64</span></span>|<span data-ttu-id="5e53f-401">总存储量（以字节为单位）。</span><span class="sxs-lookup"><span data-stu-id="5e53f-401">Total Storage in Bytes.</span></span> <span data-ttu-id="5e53f-402">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5e53f-402">This property is read-only.</span></span> <span data-ttu-id="5e53f-403">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="5e53f-403">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="5e53f-404">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="5e53f-404">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="5e53f-405">Int64</span><span class="sxs-lookup"><span data-stu-id="5e53f-405">Int64</span></span>|<span data-ttu-id="5e53f-406">以字节为单位的可用存储空间。</span><span class="sxs-lookup"><span data-stu-id="5e53f-406">Free Storage in Bytes.</span></span> <span data-ttu-id="5e53f-407">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5e53f-407">This property is read-only.</span></span> <span data-ttu-id="5e53f-408">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="5e53f-408">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="5e53f-409">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="5e53f-409">managedDeviceName</span></span>|<span data-ttu-id="5e53f-410">String</span><span class="sxs-lookup"><span data-stu-id="5e53f-410">String</span></span>|<span data-ttu-id="5e53f-411">用于识别设备的自动生成的名称。</span><span class="sxs-lookup"><span data-stu-id="5e53f-411">Automatically generated name to identify a device.</span></span> <span data-ttu-id="5e53f-412">可以覆盖为用户友好名称。</span><span class="sxs-lookup"><span data-stu-id="5e53f-412">Can be overwritten to a user friendly name.</span></span> <span data-ttu-id="5e53f-413">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="5e53f-413">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="5e53f-414">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="5e53f-414">partnerReportedThreatState</span></span>|[<span data-ttu-id="5e53f-415">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="5e53f-415">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="5e53f-416">指示帐户和设备正在使用移动威胁防护合作伙伴时设备的威胁状态。</span><span class="sxs-lookup"><span data-stu-id="5e53f-416">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="5e53f-417">只读。</span><span class="sxs-lookup"><span data-stu-id="5e53f-417">Read Only.</span></span> <span data-ttu-id="5e53f-418">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5e53f-418">This property is read-only.</span></span> <span data-ttu-id="5e53f-419">继承自[managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="5e53f-419">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="5e53f-420">可取值为：`unknown`、`activated`、`deactivated`、`secured`、`lowSeverity`、`mediumSeverity`、`highSeverity`、`unresponsive`、`compromised`、`misconfigured`。</span><span class="sxs-lookup"><span data-stu-id="5e53f-420">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="5e53f-421">retireAfterDateTime</span><span class="sxs-lookup"><span data-stu-id="5e53f-421">retireAfterDateTime</span></span>|<span data-ttu-id="5e53f-422">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e53f-422">DateTimeOffset</span></span>|<span data-ttu-id="5e53f-423">指示当设备因计划操作而自动停用的时间。</span><span class="sxs-lookup"><span data-stu-id="5e53f-423">Indicates the time after when a device will be auto retired because of scheduled action.</span></span> <span data-ttu-id="5e53f-424">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5e53f-424">This property is read-only.</span></span> <span data-ttu-id="5e53f-425">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="5e53f-425">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="5e53f-426">usersLoggedOn</span><span class="sxs-lookup"><span data-stu-id="5e53f-426">usersLoggedOn</span></span>|<span data-ttu-id="5e53f-427">[loggedOnUser](../resources/intune-devices-loggedonuser.md)集合</span><span class="sxs-lookup"><span data-stu-id="5e53f-427">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="5e53f-428">指示设备的上次登录用户。</span><span class="sxs-lookup"><span data-stu-id="5e53f-428">Indicates the last logged on users of a device.</span></span> <span data-ttu-id="5e53f-429">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5e53f-429">This property is read-only.</span></span> <span data-ttu-id="5e53f-430">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="5e53f-430">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="5e53f-431">preferMdmOverGroupPolicyAppliedDateTime</span><span class="sxs-lookup"><span data-stu-id="5e53f-431">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="5e53f-432">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e53f-432">DateTimeOffset</span></span>|<span data-ttu-id="5e53f-433">报告设置了 preferMdmOverGroupPolicy 设置的 DateTime。</span><span class="sxs-lookup"><span data-stu-id="5e53f-433">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="5e53f-434">设置后，如果存在冲突，Intune MDM 设置将覆盖组策略设置。</span><span class="sxs-lookup"><span data-stu-id="5e53f-434">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="5e53f-435">只读。</span><span class="sxs-lookup"><span data-stu-id="5e53f-435">Read Only.</span></span> <span data-ttu-id="5e53f-436">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5e53f-436">This property is read-only.</span></span> <span data-ttu-id="5e53f-437">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="5e53f-437">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="5e53f-438">autopilotEnrolled</span><span class="sxs-lookup"><span data-stu-id="5e53f-438">autopilotEnrolled</span></span>|<span data-ttu-id="5e53f-439">Boolean</span><span class="sxs-lookup"><span data-stu-id="5e53f-439">Boolean</span></span>|<span data-ttu-id="5e53f-440">如果托管设备是通过自动引导注册的，则报告。</span><span class="sxs-lookup"><span data-stu-id="5e53f-440">Reports if the managed device is enrolled via auto-pilot.</span></span> <span data-ttu-id="5e53f-441">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5e53f-441">This property is read-only.</span></span> <span data-ttu-id="5e53f-442">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="5e53f-442">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="5e53f-443">requireUserEnrollmentApproval</span><span class="sxs-lookup"><span data-stu-id="5e53f-443">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="5e53f-444">Boolean</span><span class="sxs-lookup"><span data-stu-id="5e53f-444">Boolean</span></span>|<span data-ttu-id="5e53f-445">如果托管 iOS 设备是用户审批注册，则报告。</span><span class="sxs-lookup"><span data-stu-id="5e53f-445">Reports if the managed iOS device is user approval enrollment.</span></span> <span data-ttu-id="5e53f-446">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5e53f-446">This property is read-only.</span></span> <span data-ttu-id="5e53f-447">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="5e53f-447">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="5e53f-448">managementCertificateExpirationDate</span><span class="sxs-lookup"><span data-stu-id="5e53f-448">managementCertificateExpirationDate</span></span>|<span data-ttu-id="5e53f-449">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e53f-449">DateTimeOffset</span></span>|<span data-ttu-id="5e53f-450">报告设备管理证书到期日期。</span><span class="sxs-lookup"><span data-stu-id="5e53f-450">Reports device management certificate expiration date.</span></span> <span data-ttu-id="5e53f-451">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5e53f-451">This property is read-only.</span></span> <span data-ttu-id="5e53f-452">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="5e53f-452">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="5e53f-453">iccid</span><span class="sxs-lookup"><span data-stu-id="5e53f-453">iccid</span></span>|<span data-ttu-id="5e53f-454">字符串</span><span class="sxs-lookup"><span data-stu-id="5e53f-454">String</span></span>|<span data-ttu-id="5e53f-455">集成的电路卡标识符，它是 SIM 卡的唯一标识号。</span><span class="sxs-lookup"><span data-stu-id="5e53f-455">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span> <span data-ttu-id="5e53f-456">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5e53f-456">This property is read-only.</span></span> <span data-ttu-id="5e53f-457">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="5e53f-457">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="5e53f-458">udid</span><span class="sxs-lookup"><span data-stu-id="5e53f-458">udid</span></span>|<span data-ttu-id="5e53f-459">字符串</span><span class="sxs-lookup"><span data-stu-id="5e53f-459">String</span></span>|<span data-ttu-id="5e53f-460">IOS 和 macOS 设备的唯一设备标识符。</span><span class="sxs-lookup"><span data-stu-id="5e53f-460">Unique Device Identifier for iOS and macOS devices.</span></span> <span data-ttu-id="5e53f-461">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5e53f-461">This property is read-only.</span></span> <span data-ttu-id="5e53f-462">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="5e53f-462">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="5e53f-463">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5e53f-463">roleScopeTagIds</span></span>|<span data-ttu-id="5e53f-464">String collection</span><span class="sxs-lookup"><span data-stu-id="5e53f-464">String collection</span></span>|<span data-ttu-id="5e53f-465">此设备实例的范围标记 Id 的列表。</span><span class="sxs-lookup"><span data-stu-id="5e53f-465">List of Scope Tag IDs for this Device instance.</span></span> <span data-ttu-id="5e53f-466">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="5e53f-466">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="5e53f-467">windowsActiveMalwareCount</span><span class="sxs-lookup"><span data-stu-id="5e53f-467">windowsActiveMalwareCount</span></span>|<span data-ttu-id="5e53f-468">Int32</span><span class="sxs-lookup"><span data-stu-id="5e53f-468">Int32</span></span>|<span data-ttu-id="5e53f-469">此 windows 设备的活动恶意软件的计数。</span><span class="sxs-lookup"><span data-stu-id="5e53f-469">Count of active malware for this windows device.</span></span> <span data-ttu-id="5e53f-470">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5e53f-470">This property is read-only.</span></span> <span data-ttu-id="5e53f-471">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="5e53f-471">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="5e53f-472">windowsRemediatedMalwareCount</span><span class="sxs-lookup"><span data-stu-id="5e53f-472">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="5e53f-473">Int32</span><span class="sxs-lookup"><span data-stu-id="5e53f-473">Int32</span></span>|<span data-ttu-id="5e53f-474">此 windows 设备的修正的恶意软件的计数。</span><span class="sxs-lookup"><span data-stu-id="5e53f-474">Count of remediated malware for this windows device.</span></span> <span data-ttu-id="5e53f-475">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5e53f-475">This property is read-only.</span></span> <span data-ttu-id="5e53f-476">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="5e53f-476">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="5e53f-477">notes</span><span class="sxs-lookup"><span data-stu-id="5e53f-477">notes</span></span>|<span data-ttu-id="5e53f-478">String</span><span class="sxs-lookup"><span data-stu-id="5e53f-478">String</span></span>|<span data-ttu-id="5e53f-479">由 IT 管理员创建的设备上的注释继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="5e53f-479">Notes on the device created by IT Admin Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="5e53f-480">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="5e53f-480">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="5e53f-481">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="5e53f-481">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="5e53f-482">Configuration manager 客户端运行状况状态，仅适用于从[ManagedDevice](../resources/intune-devices-manageddevice.md)继承的 MDM/ConfigMgr 代理所管理的设备</span><span class="sxs-lookup"><span data-stu-id="5e53f-482">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="5e53f-483">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="5e53f-483">configurationManagerClientInformation</span></span>|[<span data-ttu-id="5e53f-484">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="5e53f-484">configurationManagerClientInformation</span></span>](../resources/intune-devices-configurationmanagerclientinformation.md)|<span data-ttu-id="5e53f-485">Configuration manager 客户端信息，仅对由[ManagedDevice](../resources/intune-devices-manageddevice.md)继承的 ConfigMgr 代理、duel 管理或三方管理的设备有效</span><span class="sxs-lookup"><span data-stu-id="5e53f-485">Configuration manager client information, valid only for devices managed, duel-managed or tri-managed by ConfigMgr Agent Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="5e53f-486">ethernetMacAddress</span><span class="sxs-lookup"><span data-stu-id="5e53f-486">ethernetMacAddress</span></span>|<span data-ttu-id="5e53f-487">字符串</span><span class="sxs-lookup"><span data-stu-id="5e53f-487">String</span></span>|<span data-ttu-id="5e53f-488">以太网 MAC。</span><span class="sxs-lookup"><span data-stu-id="5e53f-488">Ethernet MAC.</span></span> <span data-ttu-id="5e53f-489">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5e53f-489">This property is read-only.</span></span> <span data-ttu-id="5e53f-490">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="5e53f-490">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="5e53f-491">physicalMemoryInBytes</span><span class="sxs-lookup"><span data-stu-id="5e53f-491">physicalMemoryInBytes</span></span>|<span data-ttu-id="5e53f-492">Int64</span><span class="sxs-lookup"><span data-stu-id="5e53f-492">Int64</span></span>|<span data-ttu-id="5e53f-493">内存总量（以字节为单位）。</span><span class="sxs-lookup"><span data-stu-id="5e53f-493">Total Memory in Bytes.</span></span> <span data-ttu-id="5e53f-494">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5e53f-494">This property is read-only.</span></span> <span data-ttu-id="5e53f-495">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="5e53f-495">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="5e53f-496">processorArchitecture</span><span class="sxs-lookup"><span data-stu-id="5e53f-496">processorArchitecture</span></span>|[<span data-ttu-id="5e53f-497">managedDeviceArchitecture</span><span class="sxs-lookup"><span data-stu-id="5e53f-497">managedDeviceArchitecture</span></span>](../resources/intune-devices-manageddevicearchitecture.md)|<span data-ttu-id="5e53f-498">处理器体系结构。</span><span class="sxs-lookup"><span data-stu-id="5e53f-498">Processor architecture.</span></span> <span data-ttu-id="5e53f-499">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5e53f-499">This property is read-only.</span></span> <span data-ttu-id="5e53f-500">继承自[managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="5e53f-500">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="5e53f-501">可取值为：`unknown`、`x86`、`x64`、`arm`、`arM64`。</span><span class="sxs-lookup"><span data-stu-id="5e53f-501">Possible values are: `unknown`, `x86`, `x64`, `arm`, `arM64`.</span></span>|



## <a name="response"></a><span data-ttu-id="5e53f-502">响应</span><span class="sxs-lookup"><span data-stu-id="5e53f-502">Response</span></span>
<span data-ttu-id="5e53f-503">如果成功，此方法在响应`201 Created`正文中返回响应代码和[windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md)对象。</span><span class="sxs-lookup"><span data-stu-id="5e53f-503">If successful, this method returns a `201 Created` response code and a [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5e53f-504">示例</span><span class="sxs-lookup"><span data-stu-id="5e53f-504">Example</span></span>

### <a name="request"></a><span data-ttu-id="5e53f-505">请求</span><span class="sxs-lookup"><span data-stu-id="5e53f-505">Request</span></span>
<span data-ttu-id="5e53f-506">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5e53f-506">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices
Content-type: application/json
Content-length: 7641

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
  },
  "ethernetMacAddress": "Ethernet Mac Address value",
  "physicalMemoryInBytes": 5,
  "processorArchitecture": "x86"
}
```

### <a name="response"></a><span data-ttu-id="5e53f-507">响应</span><span class="sxs-lookup"><span data-stu-id="5e53f-507">Response</span></span>
<span data-ttu-id="5e53f-p171">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5e53f-p171">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 7690

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
  },
  "ethernetMacAddress": "Ethernet Mac Address value",
  "physicalMemoryInBytes": 5,
  "processorArchitecture": "x86"
}
```





