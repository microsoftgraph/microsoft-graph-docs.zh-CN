---
title: 创建 windowsManagedDevice
description: 创建新的 windowsManagedDevice 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fc1f6e9576e85a70de0bec0a9c86e14d4688afc0
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52662975"
---
# <a name="create-windowsmanageddevice"></a><span data-ttu-id="921f7-103">创建 windowsManagedDevice</span><span class="sxs-lookup"><span data-stu-id="921f7-103">Create windowsManagedDevice</span></span>

<span data-ttu-id="921f7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="921f7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="921f7-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="921f7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="921f7-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="921f7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="921f7-107">创建新的 [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="921f7-107">Create a new [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="921f7-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="921f7-108">Prerequisites</span></span>
<span data-ttu-id="921f7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="921f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="921f7-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="921f7-111">Permission type</span></span>|<span data-ttu-id="921f7-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="921f7-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="921f7-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="921f7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="921f7-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="921f7-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="921f7-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="921f7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="921f7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="921f7-116">Not supported.</span></span>|
|<span data-ttu-id="921f7-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="921f7-117">Application</span></span>|<span data-ttu-id="921f7-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="921f7-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="921f7-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="921f7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices
POST /deviceManagement/comanagedDevices
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices
```

## <a name="request-headers"></a><span data-ttu-id="921f7-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="921f7-120">Request headers</span></span>
|<span data-ttu-id="921f7-121">标头</span><span class="sxs-lookup"><span data-stu-id="921f7-121">Header</span></span>|<span data-ttu-id="921f7-122">值</span><span class="sxs-lookup"><span data-stu-id="921f7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="921f7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="921f7-123">Authorization</span></span>|<span data-ttu-id="921f7-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="921f7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="921f7-125">接受</span><span class="sxs-lookup"><span data-stu-id="921f7-125">Accept</span></span>|<span data-ttu-id="921f7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="921f7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="921f7-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="921f7-127">Request body</span></span>
<span data-ttu-id="921f7-128">在请求正文中，提供 windowsManagedDevice 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="921f7-128">In the request body, supply a JSON representation for the windowsManagedDevice object.</span></span>

<span data-ttu-id="921f7-129">下表显示创建 windowsManagedDevice 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="921f7-129">The following table shows the properties that are required when you create the windowsManagedDevice.</span></span>

|<span data-ttu-id="921f7-130">属性</span><span class="sxs-lookup"><span data-stu-id="921f7-130">Property</span></span>|<span data-ttu-id="921f7-131">类型</span><span class="sxs-lookup"><span data-stu-id="921f7-131">Type</span></span>|<span data-ttu-id="921f7-132">说明</span><span class="sxs-lookup"><span data-stu-id="921f7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="921f7-133">id</span><span class="sxs-lookup"><span data-stu-id="921f7-133">id</span></span>|<span data-ttu-id="921f7-134">String</span><span class="sxs-lookup"><span data-stu-id="921f7-134">String</span></span>|<span data-ttu-id="921f7-135">设备的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="921f7-135">Unique Identifier for the device.</span></span> <span data-ttu-id="921f7-136">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="921f7-136">This property is read-only.</span></span> <span data-ttu-id="921f7-137">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="921f7-137">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="921f7-138">userId</span><span class="sxs-lookup"><span data-stu-id="921f7-138">userId</span></span>|<span data-ttu-id="921f7-139">String</span><span class="sxs-lookup"><span data-stu-id="921f7-139">String</span></span>|<span data-ttu-id="921f7-140">与设备关联的用户的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="921f7-140">Unique Identifier for the user associated with the device.</span></span> <span data-ttu-id="921f7-141">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="921f7-141">This property is read-only.</span></span> <span data-ttu-id="921f7-142">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="921f7-142">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="921f7-143">deviceName</span><span class="sxs-lookup"><span data-stu-id="921f7-143">deviceName</span></span>|<span data-ttu-id="921f7-144">String</span><span class="sxs-lookup"><span data-stu-id="921f7-144">String</span></span>|<span data-ttu-id="921f7-145">设备的名称。</span><span class="sxs-lookup"><span data-stu-id="921f7-145">Name of the device.</span></span> <span data-ttu-id="921f7-146">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="921f7-146">This property is read-only.</span></span> <span data-ttu-id="921f7-147">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="921f7-147">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="921f7-148">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="921f7-148">hardwareInformation</span></span>|[<span data-ttu-id="921f7-149">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="921f7-149">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="921f7-150">设备的硬向详细信息。</span><span class="sxs-lookup"><span data-stu-id="921f7-150">The hardward details for the device.</span></span>  <span data-ttu-id="921f7-151">包括存储空间、制造商、序列号等信息。此属性为只读。</span><span class="sxs-lookup"><span data-stu-id="921f7-151">Includes information such as storage space, manufacturer, serial number, etc. This property is read-only.</span></span> <span data-ttu-id="921f7-152">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="921f7-152">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="921f7-153">ownerType</span><span class="sxs-lookup"><span data-stu-id="921f7-153">ownerType</span></span>|[<span data-ttu-id="921f7-154">ownerType</span><span class="sxs-lookup"><span data-stu-id="921f7-154">ownerType</span></span>](../resources/intune-shared-ownertype.md)|<span data-ttu-id="921f7-155">设备的所有权。</span><span class="sxs-lookup"><span data-stu-id="921f7-155">Ownership of the device.</span></span> <span data-ttu-id="921f7-156">可以是"company"或"personal"继承自 [managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="921f7-156">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="921f7-157">可取值为：`unknown`、`company`、`personal`。</span><span class="sxs-lookup"><span data-stu-id="921f7-157">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="921f7-158">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="921f7-158">managedDeviceOwnerType</span></span>|[<span data-ttu-id="921f7-159">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="921f7-159">managedDeviceOwnerType</span></span>](../resources/intune-shared-manageddeviceownertype.md)|<span data-ttu-id="921f7-160">设备的所有权。</span><span class="sxs-lookup"><span data-stu-id="921f7-160">Ownership of the device.</span></span> <span data-ttu-id="921f7-161">可以是"company"或"personal"继承自 [managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="921f7-161">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="921f7-162">可取值为：`unknown`、`company`、`personal`。</span><span class="sxs-lookup"><span data-stu-id="921f7-162">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="921f7-163">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="921f7-163">deviceActionResults</span></span>|<span data-ttu-id="921f7-164">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) 集合</span><span class="sxs-lookup"><span data-stu-id="921f7-164">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="921f7-165">ComplexType deviceActionResult 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="921f7-165">List of ComplexType deviceActionResult objects.</span></span> <span data-ttu-id="921f7-166">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="921f7-166">This property is read-only.</span></span> <span data-ttu-id="921f7-167">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="921f7-167">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="921f7-168">managementState</span><span class="sxs-lookup"><span data-stu-id="921f7-168">managementState</span></span>|[<span data-ttu-id="921f7-169">managementState</span><span class="sxs-lookup"><span data-stu-id="921f7-169">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="921f7-170">设备的管理状态。</span><span class="sxs-lookup"><span data-stu-id="921f7-170">Management state of the device.</span></span> <span data-ttu-id="921f7-171">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="921f7-171">This property is read-only.</span></span> <span data-ttu-id="921f7-172">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="921f7-172">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="921f7-173">可取值为：`managed`、`retirePending`、`retireFailed`、`wipePending`、`wipeFailed`、`unhealthy`、`deletePending`、`retireIssued`、`wipeIssued`、`wipeCanceled`、`retireCanceled`、`discovered`。</span><span class="sxs-lookup"><span data-stu-id="921f7-173">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="921f7-174">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="921f7-174">enrolledDateTime</span></span>|<span data-ttu-id="921f7-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="921f7-175">DateTimeOffset</span></span>|<span data-ttu-id="921f7-176">设备的注册时间。</span><span class="sxs-lookup"><span data-stu-id="921f7-176">Enrollment time of the device.</span></span> <span data-ttu-id="921f7-177">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="921f7-177">This property is read-only.</span></span> <span data-ttu-id="921f7-178">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="921f7-178">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="921f7-179">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="921f7-179">lastSyncDateTime</span></span>|<span data-ttu-id="921f7-180">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="921f7-180">DateTimeOffset</span></span>|<span data-ttu-id="921f7-181">设备上次成功完成与 Intune 同步的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="921f7-181">The date and time that the device last completed a successful sync with Intune.</span></span> <span data-ttu-id="921f7-182">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="921f7-182">This property is read-only.</span></span> <span data-ttu-id="921f7-183">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="921f7-183">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="921f7-184">chassisType</span><span class="sxs-lookup"><span data-stu-id="921f7-184">chassisType</span></span>|[<span data-ttu-id="921f7-185">chassisType</span><span class="sxs-lookup"><span data-stu-id="921f7-185">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="921f7-186">设备的机架类型。</span><span class="sxs-lookup"><span data-stu-id="921f7-186">Chassis type of the device.</span></span> <span data-ttu-id="921f7-187">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="921f7-187">This property is read-only.</span></span> <span data-ttu-id="921f7-188">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="921f7-188">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="921f7-189">可取值为：`unknown`、`desktop`、`laptop`、`worksWorkstation`、`enterpriseServer`、`phone`、`tablet`、`mobileOther`、`mobileUnknown`。</span><span class="sxs-lookup"><span data-stu-id="921f7-189">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="921f7-190">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="921f7-190">operatingSystem</span></span>|<span data-ttu-id="921f7-191">String</span><span class="sxs-lookup"><span data-stu-id="921f7-191">String</span></span>|<span data-ttu-id="921f7-192">设备的操作系统。</span><span class="sxs-lookup"><span data-stu-id="921f7-192">Operating system of the device.</span></span> <span data-ttu-id="921f7-193">Windows、iOS 等。此属性为只读。</span><span class="sxs-lookup"><span data-stu-id="921f7-193">Windows, iOS, etc. This property is read-only.</span></span> <span data-ttu-id="921f7-194">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="921f7-194">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="921f7-195">deviceType</span><span class="sxs-lookup"><span data-stu-id="921f7-195">deviceType</span></span>|[<span data-ttu-id="921f7-196">deviceType</span><span class="sxs-lookup"><span data-stu-id="921f7-196">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="921f7-197">设备平台。</span><span class="sxs-lookup"><span data-stu-id="921f7-197">Platform of the device.</span></span> <span data-ttu-id="921f7-198">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="921f7-198">This property is read-only.</span></span> <span data-ttu-id="921f7-199">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="921f7-199">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="921f7-200">可能的值是 `desktop` `windowsRT` `winMO6` ：、、、、、、、、、、 `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `windows10x` `androidnGMS` `chromeOS` `linux` `blackberry` `palm` `unknown` `cloudPC` 、</span><span class="sxs-lookup"><span data-stu-id="921f7-200">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `androidnGMS`, `chromeOS`, `linux`, `blackberry`, `palm`, `unknown`, `cloudPC`.</span></span>|
|<span data-ttu-id="921f7-201">complianceState</span><span class="sxs-lookup"><span data-stu-id="921f7-201">complianceState</span></span>|[<span data-ttu-id="921f7-202">complianceState</span><span class="sxs-lookup"><span data-stu-id="921f7-202">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="921f7-203">设备的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="921f7-203">Compliance state of the device.</span></span> <span data-ttu-id="921f7-204">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="921f7-204">This property is read-only.</span></span> <span data-ttu-id="921f7-205">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="921f7-205">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="921f7-206">可取值为：`unknown`、`compliant`、`noncompliant`、`conflict`、`error`、`inGracePeriod`、`configManager`。</span><span class="sxs-lookup"><span data-stu-id="921f7-206">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="921f7-207">jailBroken</span><span class="sxs-lookup"><span data-stu-id="921f7-207">jailBroken</span></span>|<span data-ttu-id="921f7-208">String</span><span class="sxs-lookup"><span data-stu-id="921f7-208">String</span></span>|<span data-ttu-id="921f7-209">设备是否已越狱或取得 root 权限。</span><span class="sxs-lookup"><span data-stu-id="921f7-209">whether the device is jail broken or rooted.</span></span> <span data-ttu-id="921f7-210">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="921f7-210">This property is read-only.</span></span> <span data-ttu-id="921f7-211">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="921f7-211">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="921f7-212">managementAgent</span><span class="sxs-lookup"><span data-stu-id="921f7-212">managementAgent</span></span>|[<span data-ttu-id="921f7-213">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="921f7-213">managementAgentType</span></span>](../resources/intune-shared-managementagenttype.md)|<span data-ttu-id="921f7-214">设备的管理通道。</span><span class="sxs-lookup"><span data-stu-id="921f7-214">Management channel of the device.</span></span> <span data-ttu-id="921f7-215">Intune、EAS 等此属性为只读。</span><span class="sxs-lookup"><span data-stu-id="921f7-215">Intune, EAS, etc. This property is read-only.</span></span> <span data-ttu-id="921f7-216">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="921f7-216">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="921f7-217">可能的值是 `eas` `mdm` `easMdm` ：、、、、、、、、、、 `intuneClient` `easIntuneClient` `configurationManagerClient` `configurationManagerClientMdm` `configurationManagerClientMdmEas` `unknown` `jamf` `googleCloudDevicePolicyController` `microsoft365ManagedMdm` `msSense` `intuneAosp` 。</span><span class="sxs-lookup"><span data-stu-id="921f7-217">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`, `msSense`, `intuneAosp`.</span></span>|
|<span data-ttu-id="921f7-218">osVersion</span><span class="sxs-lookup"><span data-stu-id="921f7-218">osVersion</span></span>|<span data-ttu-id="921f7-219">String</span><span class="sxs-lookup"><span data-stu-id="921f7-219">String</span></span>|<span data-ttu-id="921f7-220">设备的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="921f7-220">Operating system version of the device.</span></span> <span data-ttu-id="921f7-221">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="921f7-221">This property is read-only.</span></span> <span data-ttu-id="921f7-222">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="921f7-222">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="921f7-223">easActivated</span><span class="sxs-lookup"><span data-stu-id="921f7-223">easActivated</span></span>|<span data-ttu-id="921f7-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="921f7-224">Boolean</span></span>|<span data-ttu-id="921f7-225">设备是否已激活 Exchange ActiveSync。</span><span class="sxs-lookup"><span data-stu-id="921f7-225">Whether the device is Exchange ActiveSync activated.</span></span> <span data-ttu-id="921f7-226">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="921f7-226">This property is read-only.</span></span> <span data-ttu-id="921f7-227">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="921f7-227">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="921f7-228">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="921f7-228">easDeviceId</span></span>|<span data-ttu-id="921f7-229">String</span><span class="sxs-lookup"><span data-stu-id="921f7-229">String</span></span>|<span data-ttu-id="921f7-230">设备的 Exchange ActiveSync ID。</span><span class="sxs-lookup"><span data-stu-id="921f7-230">Exchange ActiveSync Id of the device.</span></span> <span data-ttu-id="921f7-231">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="921f7-231">This property is read-only.</span></span> <span data-ttu-id="921f7-232">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="921f7-232">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="921f7-233">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="921f7-233">easActivationDateTime</span></span>|<span data-ttu-id="921f7-234">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="921f7-234">DateTimeOffset</span></span>|<span data-ttu-id="921f7-235">设备的 Exchange ActivationSync 激活时间。</span><span class="sxs-lookup"><span data-stu-id="921f7-235">Exchange ActivationSync activation time of the device.</span></span> <span data-ttu-id="921f7-236">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="921f7-236">This property is read-only.</span></span> <span data-ttu-id="921f7-237">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="921f7-237">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="921f7-238">aadRegistered</span><span class="sxs-lookup"><span data-stu-id="921f7-238">aadRegistered</span></span>|<span data-ttu-id="921f7-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="921f7-239">Boolean</span></span>|<span data-ttu-id="921f7-240">设备是否已注册 Azure Active Directory。</span><span class="sxs-lookup"><span data-stu-id="921f7-240">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="921f7-241">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="921f7-241">This property is read-only.</span></span> <span data-ttu-id="921f7-242">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="921f7-242">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="921f7-243">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="921f7-243">azureADRegistered</span></span>|<span data-ttu-id="921f7-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="921f7-244">Boolean</span></span>|<span data-ttu-id="921f7-245">设备是否已注册 Azure Active Directory。</span><span class="sxs-lookup"><span data-stu-id="921f7-245">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="921f7-246">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="921f7-246">This property is read-only.</span></span> <span data-ttu-id="921f7-247">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="921f7-247">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="921f7-248">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="921f7-248">deviceEnrollmentType</span></span>|[<span data-ttu-id="921f7-249">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="921f7-249">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="921f7-250">设备的注册类型。</span><span class="sxs-lookup"><span data-stu-id="921f7-250">Enrollment type of the device.</span></span> <span data-ttu-id="921f7-251">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="921f7-251">This property is read-only.</span></span> <span data-ttu-id="921f7-252">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="921f7-252">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="921f7-253">可能的值是 `unknown` `userEnrollment` `deviceEnrollmentManager` ：、、、、、、、、、 `appleBulkWithUser` `appleBulkWithoutUser` `windowsAzureADJoin` `windowsBulkUserless` `windowsAutoEnrollment` `windowsBulkAzureDomainJoin` `windowsCoManagement` `windowsAzureADJoinUsingDeviceAuth` `appleUserEnrollment` `appleUserEnrollmentWithServiceAccount` `azureAdJoinUsingAzureVmExtension` `androidEnterpriseDedicatedDevice` `androidEnterpriseFullyManaged` `androidEnterpriseCorporateWorkProfile` 。</span><span class="sxs-lookup"><span data-stu-id="921f7-253">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `windowsAzureADJoinUsingDeviceAuth`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`, `azureAdJoinUsingAzureVmExtension`, `androidEnterpriseDedicatedDevice`, `androidEnterpriseFullyManaged`, `androidEnterpriseCorporateWorkProfile`.</span></span>|
|<span data-ttu-id="921f7-254">lostModeState</span><span class="sxs-lookup"><span data-stu-id="921f7-254">lostModeState</span></span>|[<span data-ttu-id="921f7-255">lostModeState</span><span class="sxs-lookup"><span data-stu-id="921f7-255">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="921f7-256">指示是启用还是禁用丢失模式。</span><span class="sxs-lookup"><span data-stu-id="921f7-256">Indicates if Lost mode is enabled or disabled.</span></span> <span data-ttu-id="921f7-257">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="921f7-257">This property is read-only.</span></span> <span data-ttu-id="921f7-258">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="921f7-258">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="921f7-259">可取值为：`disabled`、`enabled`。</span><span class="sxs-lookup"><span data-stu-id="921f7-259">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="921f7-260">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="921f7-260">activationLockBypassCode</span></span>|<span data-ttu-id="921f7-261">String</span><span class="sxs-lookup"><span data-stu-id="921f7-261">String</span></span>|<span data-ttu-id="921f7-262">允许绕过设备上的激活锁的代码。</span><span class="sxs-lookup"><span data-stu-id="921f7-262">Code that allows the Activation Lock on a device to be bypassed.</span></span> <span data-ttu-id="921f7-263">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="921f7-263">This property is read-only.</span></span> <span data-ttu-id="921f7-264">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="921f7-264">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="921f7-265">emailAddress</span><span class="sxs-lookup"><span data-stu-id="921f7-265">emailAddress</span></span>|<span data-ttu-id="921f7-266">String</span><span class="sxs-lookup"><span data-stu-id="921f7-266">String</span></span>|<span data-ttu-id="921f7-267">电子邮件 () 设备关联的用户的邮箱。</span><span class="sxs-lookup"><span data-stu-id="921f7-267">Email(s) for the user associated with the device.</span></span> <span data-ttu-id="921f7-268">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="921f7-268">This property is read-only.</span></span> <span data-ttu-id="921f7-269">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="921f7-269">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="921f7-270">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="921f7-270">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="921f7-271">String</span><span class="sxs-lookup"><span data-stu-id="921f7-271">String</span></span>|<span data-ttu-id="921f7-272">Azure Active Directory 设备的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="921f7-272">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="921f7-273">只读。</span><span class="sxs-lookup"><span data-stu-id="921f7-273">Read only.</span></span> <span data-ttu-id="921f7-274">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="921f7-274">This property is read-only.</span></span> <span data-ttu-id="921f7-275">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="921f7-275">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="921f7-276">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="921f7-276">azureADDeviceId</span></span>|<span data-ttu-id="921f7-277">String</span><span class="sxs-lookup"><span data-stu-id="921f7-277">String</span></span>|<span data-ttu-id="921f7-278">Azure Active Directory 设备的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="921f7-278">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="921f7-279">只读。</span><span class="sxs-lookup"><span data-stu-id="921f7-279">Read only.</span></span> <span data-ttu-id="921f7-280">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="921f7-280">This property is read-only.</span></span> <span data-ttu-id="921f7-281">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="921f7-281">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="921f7-282">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="921f7-282">deviceRegistrationState</span></span>|[<span data-ttu-id="921f7-283">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="921f7-283">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="921f7-284">设备注册状态。</span><span class="sxs-lookup"><span data-stu-id="921f7-284">Device registration state.</span></span> <span data-ttu-id="921f7-285">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="921f7-285">This property is read-only.</span></span> <span data-ttu-id="921f7-286">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="921f7-286">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="921f7-287">可取值为：`notRegistered`、`registered`、`revoked`、`keyConflict`、`approvalPending`、`certificateReset`、`notRegisteredPendingEnrollment`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="921f7-287">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="921f7-288">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="921f7-288">deviceCategoryDisplayName</span></span>|<span data-ttu-id="921f7-289">String</span><span class="sxs-lookup"><span data-stu-id="921f7-289">String</span></span>|<span data-ttu-id="921f7-290">设备类别显示名称。</span><span class="sxs-lookup"><span data-stu-id="921f7-290">Device category display name.</span></span> <span data-ttu-id="921f7-291">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="921f7-291">This property is read-only.</span></span> <span data-ttu-id="921f7-292">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="921f7-292">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="921f7-293">isSupervised</span><span class="sxs-lookup"><span data-stu-id="921f7-293">isSupervised</span></span>|<span data-ttu-id="921f7-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="921f7-294">Boolean</span></span>|<span data-ttu-id="921f7-295">设备监督状态。</span><span class="sxs-lookup"><span data-stu-id="921f7-295">Device supervised status.</span></span> <span data-ttu-id="921f7-296">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="921f7-296">This property is read-only.</span></span> <span data-ttu-id="921f7-297">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="921f7-297">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="921f7-298">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="921f7-298">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="921f7-299">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="921f7-299">DateTimeOffset</span></span>|<span data-ttu-id="921f7-300">设备上次与 Exchange 联系的时间。</span><span class="sxs-lookup"><span data-stu-id="921f7-300">Last time the device contacted Exchange.</span></span> <span data-ttu-id="921f7-301">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="921f7-301">This property is read-only.</span></span> <span data-ttu-id="921f7-302">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="921f7-302">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="921f7-303">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="921f7-303">exchangeAccessState</span></span>|[<span data-ttu-id="921f7-304">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="921f7-304">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="921f7-305">Exchange 中设备的访问状态。</span><span class="sxs-lookup"><span data-stu-id="921f7-305">The Access State of the device in Exchange.</span></span> <span data-ttu-id="921f7-306">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="921f7-306">This property is read-only.</span></span> <span data-ttu-id="921f7-307">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="921f7-307">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="921f7-308">可取值为：`none`、`unknown`、`allowed`、`blocked`、`quarantined`。</span><span class="sxs-lookup"><span data-stu-id="921f7-308">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="921f7-309">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="921f7-309">exchangeAccessStateReason</span></span>|[<span data-ttu-id="921f7-310">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="921f7-310">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="921f7-311">Exchange 中设备访问状态的出现原因。</span><span class="sxs-lookup"><span data-stu-id="921f7-311">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="921f7-312">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="921f7-312">This property is read-only.</span></span> <span data-ttu-id="921f7-313">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="921f7-313">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="921f7-314">可取值为：`none`、`unknown`、`exchangeGlobalRule`、`exchangeIndividualRule`、`exchangeDeviceRule`、`exchangeUpgrade`、`exchangeMailboxPolicy`、`other`、`compliant`、`notCompliant`、`notEnrolled`、`unknownLocation`、`mfaRequired`、`azureADBlockDueToAccessPolicy`、`compromisedPassword`、`deviceNotKnownWithManagedApp`。</span><span class="sxs-lookup"><span data-stu-id="921f7-314">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="921f7-315">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="921f7-315">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="921f7-316">String</span><span class="sxs-lookup"><span data-stu-id="921f7-316">String</span></span>|<span data-ttu-id="921f7-317">允许与设备建立远程协助会话的 URL。</span><span class="sxs-lookup"><span data-stu-id="921f7-317">Url that allows a Remote Assistance session to be established with the device.</span></span> <span data-ttu-id="921f7-318">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="921f7-318">This property is read-only.</span></span> <span data-ttu-id="921f7-319">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="921f7-319">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="921f7-320">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="921f7-320">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="921f7-321">String</span><span class="sxs-lookup"><span data-stu-id="921f7-321">String</span></span>|<span data-ttu-id="921f7-322">用于在创建远程协助会话对象时识别问题的错误字符串。</span><span class="sxs-lookup"><span data-stu-id="921f7-322">An error string that identifies issues when creating Remote Assistance session objects.</span></span> <span data-ttu-id="921f7-323">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="921f7-323">This property is read-only.</span></span> <span data-ttu-id="921f7-324">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="921f7-324">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="921f7-325">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="921f7-325">isEncrypted</span></span>|<span data-ttu-id="921f7-326">Boolean</span><span class="sxs-lookup"><span data-stu-id="921f7-326">Boolean</span></span>|<span data-ttu-id="921f7-327">设备加密状态。</span><span class="sxs-lookup"><span data-stu-id="921f7-327">Device encryption status.</span></span> <span data-ttu-id="921f7-328">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="921f7-328">This property is read-only.</span></span> <span data-ttu-id="921f7-329">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="921f7-329">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="921f7-330">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="921f7-330">userPrincipalName</span></span>|<span data-ttu-id="921f7-331">String</span><span class="sxs-lookup"><span data-stu-id="921f7-331">String</span></span>|<span data-ttu-id="921f7-332">设备用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="921f7-332">Device user principal name.</span></span> <span data-ttu-id="921f7-333">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="921f7-333">This property is read-only.</span></span> <span data-ttu-id="921f7-334">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="921f7-334">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="921f7-335">model</span><span class="sxs-lookup"><span data-stu-id="921f7-335">model</span></span>|<span data-ttu-id="921f7-336">String</span><span class="sxs-lookup"><span data-stu-id="921f7-336">String</span></span>|<span data-ttu-id="921f7-337">设备型号。</span><span class="sxs-lookup"><span data-stu-id="921f7-337">Model of the device.</span></span> <span data-ttu-id="921f7-338">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="921f7-338">This property is read-only.</span></span> <span data-ttu-id="921f7-339">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="921f7-339">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="921f7-340">manufacturer</span><span class="sxs-lookup"><span data-stu-id="921f7-340">manufacturer</span></span>|<span data-ttu-id="921f7-341">String</span><span class="sxs-lookup"><span data-stu-id="921f7-341">String</span></span>|<span data-ttu-id="921f7-342">设备的制造商。</span><span class="sxs-lookup"><span data-stu-id="921f7-342">Manufacturer of the device.</span></span> <span data-ttu-id="921f7-343">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="921f7-343">This property is read-only.</span></span> <span data-ttu-id="921f7-344">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="921f7-344">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="921f7-345">imei</span><span class="sxs-lookup"><span data-stu-id="921f7-345">imei</span></span>|<span data-ttu-id="921f7-346">String</span><span class="sxs-lookup"><span data-stu-id="921f7-346">String</span></span>|<span data-ttu-id="921f7-347">IMEI。</span><span class="sxs-lookup"><span data-stu-id="921f7-347">IMEI.</span></span> <span data-ttu-id="921f7-348">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="921f7-348">This property is read-only.</span></span> <span data-ttu-id="921f7-349">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="921f7-349">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="921f7-350">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="921f7-350">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="921f7-351">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="921f7-351">DateTimeOffset</span></span>|<span data-ttu-id="921f7-352">设备合规性宽限期到期的 DateTime。</span><span class="sxs-lookup"><span data-stu-id="921f7-352">The DateTime when device compliance grace period expires.</span></span> <span data-ttu-id="921f7-353">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="921f7-353">This property is read-only.</span></span> <span data-ttu-id="921f7-354">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="921f7-354">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="921f7-355">serialNumber</span><span class="sxs-lookup"><span data-stu-id="921f7-355">serialNumber</span></span>|<span data-ttu-id="921f7-356">String</span><span class="sxs-lookup"><span data-stu-id="921f7-356">String</span></span>|<span data-ttu-id="921f7-357">SerialNumber。</span><span class="sxs-lookup"><span data-stu-id="921f7-357">SerialNumber.</span></span> <span data-ttu-id="921f7-358">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="921f7-358">This property is read-only.</span></span> <span data-ttu-id="921f7-359">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="921f7-359">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="921f7-360">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="921f7-360">phoneNumber</span></span>|<span data-ttu-id="921f7-361">String</span><span class="sxs-lookup"><span data-stu-id="921f7-361">String</span></span>|<span data-ttu-id="921f7-362">电话设备的数量。</span><span class="sxs-lookup"><span data-stu-id="921f7-362">Phone number of the device.</span></span> <span data-ttu-id="921f7-363">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="921f7-363">This property is read-only.</span></span> <span data-ttu-id="921f7-364">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="921f7-364">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="921f7-365">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="921f7-365">androidSecurityPatchLevel</span></span>|<span data-ttu-id="921f7-366">String</span><span class="sxs-lookup"><span data-stu-id="921f7-366">String</span></span>|<span data-ttu-id="921f7-367">Android 安全修补程序级别。</span><span class="sxs-lookup"><span data-stu-id="921f7-367">Android security patch level.</span></span> <span data-ttu-id="921f7-368">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="921f7-368">This property is read-only.</span></span> <span data-ttu-id="921f7-369">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="921f7-369">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="921f7-370">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="921f7-370">userDisplayName</span></span>|<span data-ttu-id="921f7-371">String</span><span class="sxs-lookup"><span data-stu-id="921f7-371">String</span></span>|<span data-ttu-id="921f7-372">用户显示名称。</span><span class="sxs-lookup"><span data-stu-id="921f7-372">User display name.</span></span> <span data-ttu-id="921f7-373">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="921f7-373">This property is read-only.</span></span> <span data-ttu-id="921f7-374">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="921f7-374">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="921f7-375">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="921f7-375">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="921f7-376">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="921f7-376">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="921f7-377">ConfigrMgr 客户端启用的功能。</span><span class="sxs-lookup"><span data-stu-id="921f7-377">ConfigrMgr client enabled features.</span></span> <span data-ttu-id="921f7-378">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="921f7-378">This property is read-only.</span></span> <span data-ttu-id="921f7-379">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="921f7-379">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="921f7-380">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="921f7-380">wiFiMacAddress</span></span>|<span data-ttu-id="921f7-381">String</span><span class="sxs-lookup"><span data-stu-id="921f7-381">String</span></span>|<span data-ttu-id="921f7-382">Wi-Fi MAC。</span><span class="sxs-lookup"><span data-stu-id="921f7-382">Wi-Fi MAC.</span></span> <span data-ttu-id="921f7-383">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="921f7-383">This property is read-only.</span></span> <span data-ttu-id="921f7-384">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="921f7-384">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="921f7-385">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="921f7-385">deviceHealthAttestationState</span></span>|[<span data-ttu-id="921f7-386">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="921f7-386">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="921f7-387">设备运行状况证明状态。</span><span class="sxs-lookup"><span data-stu-id="921f7-387">The device health attestation state.</span></span> <span data-ttu-id="921f7-388">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="921f7-388">This property is read-only.</span></span> <span data-ttu-id="921f7-389">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="921f7-389">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="921f7-390">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="921f7-390">subscriberCarrier</span></span>|<span data-ttu-id="921f7-391">String</span><span class="sxs-lookup"><span data-stu-id="921f7-391">String</span></span>|<span data-ttu-id="921f7-392">订阅者运营商。</span><span class="sxs-lookup"><span data-stu-id="921f7-392">Subscriber Carrier.</span></span> <span data-ttu-id="921f7-393">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="921f7-393">This property is read-only.</span></span> <span data-ttu-id="921f7-394">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="921f7-394">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="921f7-395">meid</span><span class="sxs-lookup"><span data-stu-id="921f7-395">meid</span></span>|<span data-ttu-id="921f7-396">String</span><span class="sxs-lookup"><span data-stu-id="921f7-396">String</span></span>|<span data-ttu-id="921f7-397">MEID。</span><span class="sxs-lookup"><span data-stu-id="921f7-397">MEID.</span></span> <span data-ttu-id="921f7-398">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="921f7-398">This property is read-only.</span></span> <span data-ttu-id="921f7-399">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="921f7-399">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="921f7-400">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="921f7-400">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="921f7-401">Int64</span><span class="sxs-lookup"><span data-stu-id="921f7-401">Int64</span></span>|<span data-ttu-id="921f7-402">总存储字节数。</span><span class="sxs-lookup"><span data-stu-id="921f7-402">Total Storage in Bytes.</span></span> <span data-ttu-id="921f7-403">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="921f7-403">This property is read-only.</span></span> <span data-ttu-id="921f7-404">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="921f7-404">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="921f7-405">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="921f7-405">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="921f7-406">Int64</span><span class="sxs-lookup"><span data-stu-id="921f7-406">Int64</span></span>|<span data-ttu-id="921f7-407">可用存储字节为单位。</span><span class="sxs-lookup"><span data-stu-id="921f7-407">Free Storage in Bytes.</span></span> <span data-ttu-id="921f7-408">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="921f7-408">This property is read-only.</span></span> <span data-ttu-id="921f7-409">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="921f7-409">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="921f7-410">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="921f7-410">managedDeviceName</span></span>|<span data-ttu-id="921f7-411">String</span><span class="sxs-lookup"><span data-stu-id="921f7-411">String</span></span>|<span data-ttu-id="921f7-412">用于识别设备的自动生成的名称。</span><span class="sxs-lookup"><span data-stu-id="921f7-412">Automatically generated name to identify a device.</span></span> <span data-ttu-id="921f7-413">可以覆盖为用户友好名称。</span><span class="sxs-lookup"><span data-stu-id="921f7-413">Can be overwritten to a user friendly name.</span></span> <span data-ttu-id="921f7-414">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="921f7-414">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="921f7-415">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="921f7-415">partnerReportedThreatState</span></span>|[<span data-ttu-id="921f7-416">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="921f7-416">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="921f7-417">指示帐户和设备正在使用移动威胁防护合作伙伴时设备的威胁状态。</span><span class="sxs-lookup"><span data-stu-id="921f7-417">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="921f7-418">只读。</span><span class="sxs-lookup"><span data-stu-id="921f7-418">Read Only.</span></span> <span data-ttu-id="921f7-419">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="921f7-419">This property is read-only.</span></span> <span data-ttu-id="921f7-420">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="921f7-420">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="921f7-421">可取值为：`unknown`、`activated`、`deactivated`、`secured`、`lowSeverity`、`mediumSeverity`、`highSeverity`、`unresponsive`、`compromised`、`misconfigured`。</span><span class="sxs-lookup"><span data-stu-id="921f7-421">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="921f7-422">retireAfterDateTime</span><span class="sxs-lookup"><span data-stu-id="921f7-422">retireAfterDateTime</span></span>|<span data-ttu-id="921f7-423">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="921f7-423">DateTimeOffset</span></span>|<span data-ttu-id="921f7-424">指示设备因计划操作而自动停用的时间。</span><span class="sxs-lookup"><span data-stu-id="921f7-424">Indicates the time after when a device will be auto retired because of scheduled action.</span></span> <span data-ttu-id="921f7-425">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="921f7-425">This property is read-only.</span></span> <span data-ttu-id="921f7-426">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="921f7-426">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="921f7-427">usersLoggedOn</span><span class="sxs-lookup"><span data-stu-id="921f7-427">usersLoggedOn</span></span>|<span data-ttu-id="921f7-428">[loggedOnUser](../resources/intune-devices-loggedonuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="921f7-428">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="921f7-429">指示设备上最后一次登录的用户。</span><span class="sxs-lookup"><span data-stu-id="921f7-429">Indicates the last logged on users of a device.</span></span> <span data-ttu-id="921f7-430">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="921f7-430">This property is read-only.</span></span> <span data-ttu-id="921f7-431">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="921f7-431">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="921f7-432">preferMdmOverGroupPolicyAppliedDateTime</span><span class="sxs-lookup"><span data-stu-id="921f7-432">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="921f7-433">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="921f7-433">DateTimeOffset</span></span>|<span data-ttu-id="921f7-434">报告 DateTime 设置了 preferMdmOverGroupPolicy 设置。</span><span class="sxs-lookup"><span data-stu-id="921f7-434">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="921f7-435">设置后，如果存在冲突，Intune MDM 设置将覆盖组策略设置。</span><span class="sxs-lookup"><span data-stu-id="921f7-435">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="921f7-436">只读。</span><span class="sxs-lookup"><span data-stu-id="921f7-436">Read Only.</span></span> <span data-ttu-id="921f7-437">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="921f7-437">This property is read-only.</span></span> <span data-ttu-id="921f7-438">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="921f7-438">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="921f7-439">autopilotEnrolled</span><span class="sxs-lookup"><span data-stu-id="921f7-439">autopilotEnrolled</span></span>|<span data-ttu-id="921f7-440">布尔值</span><span class="sxs-lookup"><span data-stu-id="921f7-440">Boolean</span></span>|<span data-ttu-id="921f7-441">报告托管设备是否通过自动试点注册。</span><span class="sxs-lookup"><span data-stu-id="921f7-441">Reports if the managed device is enrolled via auto-pilot.</span></span> <span data-ttu-id="921f7-442">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="921f7-442">This property is read-only.</span></span> <span data-ttu-id="921f7-443">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="921f7-443">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="921f7-444">requireUserEnrollmentApproval</span><span class="sxs-lookup"><span data-stu-id="921f7-444">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="921f7-445">布尔值</span><span class="sxs-lookup"><span data-stu-id="921f7-445">Boolean</span></span>|<span data-ttu-id="921f7-446">报告托管 iOS 设备是否注册用户审批。</span><span class="sxs-lookup"><span data-stu-id="921f7-446">Reports if the managed iOS device is user approval enrollment.</span></span> <span data-ttu-id="921f7-447">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="921f7-447">This property is read-only.</span></span> <span data-ttu-id="921f7-448">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="921f7-448">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="921f7-449">managementCertificateExpirationDate</span><span class="sxs-lookup"><span data-stu-id="921f7-449">managementCertificateExpirationDate</span></span>|<span data-ttu-id="921f7-450">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="921f7-450">DateTimeOffset</span></span>|<span data-ttu-id="921f7-451">报告设备管理证书到期日期。</span><span class="sxs-lookup"><span data-stu-id="921f7-451">Reports device management certificate expiration date.</span></span> <span data-ttu-id="921f7-452">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="921f7-452">This property is read-only.</span></span> <span data-ttu-id="921f7-453">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="921f7-453">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="921f7-454">iccid</span><span class="sxs-lookup"><span data-stu-id="921f7-454">iccid</span></span>|<span data-ttu-id="921f7-455">String</span><span class="sxs-lookup"><span data-stu-id="921f7-455">String</span></span>|<span data-ttu-id="921f7-456">集成的电路卡标识符，它是 SIM 卡的唯一标识号。</span><span class="sxs-lookup"><span data-stu-id="921f7-456">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span> <span data-ttu-id="921f7-457">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="921f7-457">This property is read-only.</span></span> <span data-ttu-id="921f7-458">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="921f7-458">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="921f7-459">udid</span><span class="sxs-lookup"><span data-stu-id="921f7-459">udid</span></span>|<span data-ttu-id="921f7-460">String</span><span class="sxs-lookup"><span data-stu-id="921f7-460">String</span></span>|<span data-ttu-id="921f7-461">iOS 和 macOS 设备的唯一设备标识符。</span><span class="sxs-lookup"><span data-stu-id="921f7-461">Unique Device Identifier for iOS and macOS devices.</span></span> <span data-ttu-id="921f7-462">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="921f7-462">This property is read-only.</span></span> <span data-ttu-id="921f7-463">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="921f7-463">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="921f7-464">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="921f7-464">roleScopeTagIds</span></span>|<span data-ttu-id="921f7-465">String collection</span><span class="sxs-lookup"><span data-stu-id="921f7-465">String collection</span></span>|<span data-ttu-id="921f7-466">此设备实例的范围标记标识列表。</span><span class="sxs-lookup"><span data-stu-id="921f7-466">List of Scope Tag IDs for this Device instance.</span></span> <span data-ttu-id="921f7-467">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="921f7-467">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="921f7-468">windowsActiveMalwareCount</span><span class="sxs-lookup"><span data-stu-id="921f7-468">windowsActiveMalwareCount</span></span>|<span data-ttu-id="921f7-469">Int32</span><span class="sxs-lookup"><span data-stu-id="921f7-469">Int32</span></span>|<span data-ttu-id="921f7-470">此 Windows 设备的活动恶意软件计数。</span><span class="sxs-lookup"><span data-stu-id="921f7-470">Count of active malware for this windows device.</span></span> <span data-ttu-id="921f7-471">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="921f7-471">This property is read-only.</span></span> <span data-ttu-id="921f7-472">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="921f7-472">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="921f7-473">windowsRemediatedMalwareCount</span><span class="sxs-lookup"><span data-stu-id="921f7-473">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="921f7-474">Int32</span><span class="sxs-lookup"><span data-stu-id="921f7-474">Int32</span></span>|<span data-ttu-id="921f7-475">此 Windows 设备的已修复恶意软件计数。</span><span class="sxs-lookup"><span data-stu-id="921f7-475">Count of remediated malware for this windows device.</span></span> <span data-ttu-id="921f7-476">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="921f7-476">This property is read-only.</span></span> <span data-ttu-id="921f7-477">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="921f7-477">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="921f7-478">notes</span><span class="sxs-lookup"><span data-stu-id="921f7-478">notes</span></span>|<span data-ttu-id="921f7-479">String</span><span class="sxs-lookup"><span data-stu-id="921f7-479">String</span></span>|<span data-ttu-id="921f7-480">由 IT 管理员创建的设备的备注 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="921f7-480">Notes on the device created by IT Admin Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="921f7-481">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="921f7-481">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="921f7-482">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="921f7-482">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="921f7-483">配置管理器客户端运行状况状态，仅对 MDM/ConfigMgr 代理管理的设备有效。继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="921f7-483">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="921f7-484">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="921f7-484">configurationManagerClientInformation</span></span>|[<span data-ttu-id="921f7-485">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="921f7-485">configurationManagerClientInformation</span></span>](../resources/intune-devices-configurationmanagerclientinformation.md)|<span data-ttu-id="921f7-486">配置管理器客户端信息，仅对由 ConfigMgr 代理托管、duel 托管或三管理的设备有效。继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="921f7-486">Configuration manager client information, valid only for devices managed, duel-managed or tri-managed by ConfigMgr Agent Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="921f7-487">ethernetMacAddress</span><span class="sxs-lookup"><span data-stu-id="921f7-487">ethernetMacAddress</span></span>|<span data-ttu-id="921f7-488">String</span><span class="sxs-lookup"><span data-stu-id="921f7-488">String</span></span>|<span data-ttu-id="921f7-489">以太网 MAC。</span><span class="sxs-lookup"><span data-stu-id="921f7-489">Ethernet MAC.</span></span> <span data-ttu-id="921f7-490">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="921f7-490">This property is read-only.</span></span> <span data-ttu-id="921f7-491">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="921f7-491">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="921f7-492">physicalMemoryInBytes</span><span class="sxs-lookup"><span data-stu-id="921f7-492">physicalMemoryInBytes</span></span>|<span data-ttu-id="921f7-493">Int64</span><span class="sxs-lookup"><span data-stu-id="921f7-493">Int64</span></span>|<span data-ttu-id="921f7-494">内存总量（以字节为单位）。</span><span class="sxs-lookup"><span data-stu-id="921f7-494">Total Memory in Bytes.</span></span> <span data-ttu-id="921f7-495">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="921f7-495">This property is read-only.</span></span> <span data-ttu-id="921f7-496">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="921f7-496">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="921f7-497">processorArchitecture</span><span class="sxs-lookup"><span data-stu-id="921f7-497">processorArchitecture</span></span>|[<span data-ttu-id="921f7-498">managedDeviceArchitecture</span><span class="sxs-lookup"><span data-stu-id="921f7-498">managedDeviceArchitecture</span></span>](../resources/intune-devices-manageddevicearchitecture.md)|<span data-ttu-id="921f7-499">处理器体系结构。</span><span class="sxs-lookup"><span data-stu-id="921f7-499">Processor architecture.</span></span> <span data-ttu-id="921f7-500">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="921f7-500">This property is read-only.</span></span> <span data-ttu-id="921f7-501">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="921f7-501">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="921f7-502">可取值为：`unknown`、`x86`、`x64`、`arm`、`arM64`。</span><span class="sxs-lookup"><span data-stu-id="921f7-502">Possible values are: `unknown`, `x86`, `x64`, `arm`, `arM64`.</span></span>|
|<span data-ttu-id="921f7-503">specificationVersion</span><span class="sxs-lookup"><span data-stu-id="921f7-503">specificationVersion</span></span>|<span data-ttu-id="921f7-504">String</span><span class="sxs-lookup"><span data-stu-id="921f7-504">String</span></span>|<span data-ttu-id="921f7-505">规范版本。</span><span class="sxs-lookup"><span data-stu-id="921f7-505">Specification version.</span></span> <span data-ttu-id="921f7-506">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="921f7-506">This property is read-only.</span></span> <span data-ttu-id="921f7-507">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="921f7-507">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="921f7-508">joinType</span><span class="sxs-lookup"><span data-stu-id="921f7-508">joinType</span></span>|[<span data-ttu-id="921f7-509">joinType</span><span class="sxs-lookup"><span data-stu-id="921f7-509">joinType</span></span>](../resources/intune-devices-jointype.md)|<span data-ttu-id="921f7-510">设备加入类型 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="921f7-510">Device join type Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="921f7-511">可取值为：`unknown`、`azureADJoined`、`azureADRegistered`、`hybridAzureADJoined`。</span><span class="sxs-lookup"><span data-stu-id="921f7-511">Possible values are: `unknown`, `azureADJoined`, `azureADRegistered`, `hybridAzureADJoined`.</span></span>|
|<span data-ttu-id="921f7-512">skuFamily</span><span class="sxs-lookup"><span data-stu-id="921f7-512">skuFamily</span></span>|<span data-ttu-id="921f7-513">String</span><span class="sxs-lookup"><span data-stu-id="921f7-513">String</span></span>|<span data-ttu-id="921f7-514">设备 sku 系列 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="921f7-514">Device sku family Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="921f7-515">skuNumber</span><span class="sxs-lookup"><span data-stu-id="921f7-515">skuNumber</span></span>|<span data-ttu-id="921f7-516">Int32</span><span class="sxs-lookup"><span data-stu-id="921f7-516">Int32</span></span>|<span data-ttu-id="921f7-517">设备 sku 号，另请参阅 https://docs.microsoft.com/windows/win32/api/sysinfoapi/nf-sysinfoapi-getproductinfo ：。</span><span class="sxs-lookup"><span data-stu-id="921f7-517">Device sku number, see also: https://docs.microsoft.com/windows/win32/api/sysinfoapi/nf-sysinfoapi-getproductinfo.</span></span> <span data-ttu-id="921f7-518">有效值为 0 到 2147483647。</span><span class="sxs-lookup"><span data-stu-id="921f7-518">Valid values 0 to 2147483647.</span></span> <span data-ttu-id="921f7-519">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="921f7-519">This property is read-only.</span></span> <span data-ttu-id="921f7-520">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="921f7-520">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="921f7-521">managementFeatures</span><span class="sxs-lookup"><span data-stu-id="921f7-521">managementFeatures</span></span>|[<span data-ttu-id="921f7-522">managedDeviceManagementFeatures</span><span class="sxs-lookup"><span data-stu-id="921f7-522">managedDeviceManagementFeatures</span></span>](../resources/intune-devices-manageddevicemanagementfeatures.md)|<span data-ttu-id="921f7-523">设备管理功能 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="921f7-523">Device management features Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="921f7-524">可取值为：`none`、`microsoftManagedDesktop`。</span><span class="sxs-lookup"><span data-stu-id="921f7-524">Possible values are: `none`, `microsoftManagedDesktop`.</span></span>|
|<span data-ttu-id="921f7-525">chromeOSDeviceInfo</span><span class="sxs-lookup"><span data-stu-id="921f7-525">chromeOSDeviceInfo</span></span>|<span data-ttu-id="921f7-526">[chromeOSDeviceProperty](../resources/intune-devices-chromeosdeviceproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="921f7-526">[chromeOSDeviceProperty](../resources/intune-devices-chromeosdeviceproperty.md) collection</span></span>|<span data-ttu-id="921f7-527">ChromeOS 设备的属性列表。</span><span class="sxs-lookup"><span data-stu-id="921f7-527">List of properties of the ChromeOS Device.</span></span> <span data-ttu-id="921f7-528">继承自 [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="921f7-528">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|



## <a name="response"></a><span data-ttu-id="921f7-529">响应</span><span class="sxs-lookup"><span data-stu-id="921f7-529">Response</span></span>
<span data-ttu-id="921f7-530">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="921f7-530">If successful, this method returns a `201 Created` response code and a [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="921f7-531">示例</span><span class="sxs-lookup"><span data-stu-id="921f7-531">Example</span></span>

### <a name="request"></a><span data-ttu-id="921f7-532">请求</span><span class="sxs-lookup"><span data-stu-id="921f7-532">Request</span></span>
<span data-ttu-id="921f7-533">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="921f7-533">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices
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
  "managementFeatures": "microsoftManagedDesktop",
  "chromeOSDeviceInfo": [
    {
      "@odata.type": "microsoft.graph.chromeOSDeviceProperty",
      "name": "Name value",
      "value": "Value value",
      "valueType": "Value Type value",
      "updatable": true
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="921f7-534">响应</span><span class="sxs-lookup"><span data-stu-id="921f7-534">Response</span></span>
<span data-ttu-id="921f7-p176">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="921f7-p176">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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
  "managementFeatures": "microsoftManagedDesktop",
  "chromeOSDeviceInfo": [
    {
      "@odata.type": "microsoft.graph.chromeOSDeviceProperty",
      "name": "Name value",
      "value": "Value value",
      "valueType": "Value Type value",
      "updatable": true
    }
  ]
}
```




