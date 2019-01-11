---
title: 创建 windowsManagedDevice
description: 创建新的 windowsManagedDevice 对象。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e23b24365d30954c4da1597ca9d7c14c554a73ae
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842656"
---
# <a name="create-windowsmanageddevice"></a><span data-ttu-id="9f270-103">创建 windowsManagedDevice</span><span class="sxs-lookup"><span data-stu-id="9f270-103">Create windowsManagedDevice</span></span>

> <span data-ttu-id="9f270-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="9f270-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9f270-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9f270-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9f270-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="9f270-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9f270-107">创建新的[windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9f270-107">Create a new [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9f270-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="9f270-108">Prerequisites</span></span>
<span data-ttu-id="9f270-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="9f270-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f270-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9f270-111">Permission type</span></span>|<span data-ttu-id="9f270-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9f270-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9f270-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9f270-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9f270-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f270-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="9f270-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9f270-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f270-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9f270-116">Not supported.</span></span>|
|<span data-ttu-id="9f270-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9f270-117">Application</span></span>|<span data-ttu-id="9f270-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="9f270-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9f270-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9f270-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices
POST /deviceManagement/managedDevices
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices
```

## <a name="request-headers"></a><span data-ttu-id="9f270-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9f270-120">Request headers</span></span>
|<span data-ttu-id="9f270-121">标头</span><span class="sxs-lookup"><span data-stu-id="9f270-121">Header</span></span>|<span data-ttu-id="9f270-122">值</span><span class="sxs-lookup"><span data-stu-id="9f270-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9f270-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f270-123">Authorization</span></span>|<span data-ttu-id="9f270-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9f270-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9f270-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9f270-125">Accept</span></span>|<span data-ttu-id="9f270-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9f270-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f270-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9f270-127">Request body</span></span>
<span data-ttu-id="9f270-128">在请求正文中，提供 windowsManagedDevice 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9f270-128">In the request body, supply a JSON representation for the windowsManagedDevice object.</span></span>

<span data-ttu-id="9f270-129">下表显示时创建 windowsManagedDevice 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="9f270-129">The following table shows the properties that are required when you create the windowsManagedDevice.</span></span>

|<span data-ttu-id="9f270-130">属性</span><span class="sxs-lookup"><span data-stu-id="9f270-130">Property</span></span>|<span data-ttu-id="9f270-131">类型</span><span class="sxs-lookup"><span data-stu-id="9f270-131">Type</span></span>|<span data-ttu-id="9f270-132">说明</span><span class="sxs-lookup"><span data-stu-id="9f270-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f270-133">id</span><span class="sxs-lookup"><span data-stu-id="9f270-133">id</span></span>|<span data-ttu-id="9f270-134">字符串</span><span class="sxs-lookup"><span data-stu-id="9f270-134">String</span></span>|<span data-ttu-id="9f270-135">从[managedDevice](../resources/intune-devices-manageddevice.md)设备继承的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="9f270-135">Unique Identifier for the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9f270-136">userId</span><span class="sxs-lookup"><span data-stu-id="9f270-136">userId</span></span>|<span data-ttu-id="9f270-137">String</span><span class="sxs-lookup"><span data-stu-id="9f270-137">String</span></span>|<span data-ttu-id="9f270-138">与设备继承从[managedDevice](../resources/intune-devices-manageddevice.md)关联的用户的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="9f270-138">Unique Identifier for the user associated with the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9f270-139">deviceName</span><span class="sxs-lookup"><span data-stu-id="9f270-139">deviceName</span></span>|<span data-ttu-id="9f270-140">String</span><span class="sxs-lookup"><span data-stu-id="9f270-140">String</span></span>|<span data-ttu-id="9f270-141">从[managedDevice](../resources/intune-devices-manageddevice.md)设备继承的名称</span><span class="sxs-lookup"><span data-stu-id="9f270-141">Name of the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9f270-142">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="9f270-142">hardwareInformation</span></span>|[<span data-ttu-id="9f270-143">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="9f270-143">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="9f270-144">设备 hardward 详细信息。</span><span class="sxs-lookup"><span data-stu-id="9f270-144">The hardward details for the device.</span></span>  <span data-ttu-id="9f270-145">包含信息，如存储空间、 制造商、 序列号等。继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="9f270-145">Includes information such as storage space, manufacturer, serial number, etc. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9f270-146">所有者类型</span><span class="sxs-lookup"><span data-stu-id="9f270-146">ownerType</span></span>|[<span data-ttu-id="9f270-147">所有者类型</span><span class="sxs-lookup"><span data-stu-id="9f270-147">ownerType</span></span>](../resources/intune-devices-ownertype.md)|<span data-ttu-id="9f270-148">设备的所有权。</span><span class="sxs-lookup"><span data-stu-id="9f270-148">Ownership of the device.</span></span> <span data-ttu-id="9f270-149">可以是公司或个人继承自[managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="9f270-149">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="9f270-150">可取值为：`unknown`、`company`、`personal`。</span><span class="sxs-lookup"><span data-stu-id="9f270-150">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="9f270-151">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="9f270-151">managedDeviceOwnerType</span></span>|[<span data-ttu-id="9f270-152">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="9f270-152">managedDeviceOwnerType</span></span>](../resources/intune-devices-manageddeviceownertype.md)|<span data-ttu-id="9f270-153">设备的所有权。</span><span class="sxs-lookup"><span data-stu-id="9f270-153">Ownership of the device.</span></span> <span data-ttu-id="9f270-154">可以是公司或个人继承自[managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="9f270-154">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="9f270-155">可取值为：`unknown`、`company`、`personal`。</span><span class="sxs-lookup"><span data-stu-id="9f270-155">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="9f270-156">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="9f270-156">deviceActionResults</span></span>|<span data-ttu-id="9f270-157">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9f270-157">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="9f270-158">ComplexType deviceActionResult 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="9f270-158">List of ComplexType deviceActionResult objects.</span></span> <span data-ttu-id="9f270-159">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="9f270-159">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9f270-160">管理</span><span class="sxs-lookup"><span data-stu-id="9f270-160">managementState</span></span>|[<span data-ttu-id="9f270-161">管理</span><span class="sxs-lookup"><span data-stu-id="9f270-161">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="9f270-162">管理设备的状态。</span><span class="sxs-lookup"><span data-stu-id="9f270-162">Management state of the device.</span></span> <span data-ttu-id="9f270-163">继承自[managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="9f270-163">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="9f270-164">可取值为：`managed`、`retirePending`、`retireFailed`、`wipePending`、`wipeFailed`、`unhealthy`、`deletePending`、`retireIssued`、`wipeIssued`、`wipeCanceled`、`retireCanceled`、`discovered`。</span><span class="sxs-lookup"><span data-stu-id="9f270-164">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="9f270-165">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="9f270-165">enrolledDateTime</span></span>|<span data-ttu-id="9f270-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f270-166">DateTimeOffset</span></span>|<span data-ttu-id="9f270-167">设备的注册时间。</span><span class="sxs-lookup"><span data-stu-id="9f270-167">Enrollment time of the device.</span></span> <span data-ttu-id="9f270-168">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="9f270-168">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9f270-169">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="9f270-169">lastSyncDateTime</span></span>|<span data-ttu-id="9f270-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f270-170">DateTimeOffset</span></span>|<span data-ttu-id="9f270-171">设备上次成功完成与 Intune 同步的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="9f270-171">The date and time that the device last completed a successful sync with Intune.</span></span> <span data-ttu-id="9f270-172">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="9f270-172">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9f270-173">chassisType</span><span class="sxs-lookup"><span data-stu-id="9f270-173">chassisType</span></span>|[<span data-ttu-id="9f270-174">chassisType</span><span class="sxs-lookup"><span data-stu-id="9f270-174">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="9f270-175">机箱设备的类型。</span><span class="sxs-lookup"><span data-stu-id="9f270-175">Chassis type of the device.</span></span> <span data-ttu-id="9f270-176">继承自[managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="9f270-176">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="9f270-177">可取值为：`unknown`、`desktop`、`laptop`、`worksWorkstation`、`enterpriseServer`、`phone`、`tablet`、`mobileOther`、`mobileUnknown`。</span><span class="sxs-lookup"><span data-stu-id="9f270-177">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="9f270-178">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="9f270-178">operatingSystem</span></span>|<span data-ttu-id="9f270-179">String</span><span class="sxs-lookup"><span data-stu-id="9f270-179">String</span></span>|<span data-ttu-id="9f270-180">设备的操作系统。</span><span class="sxs-lookup"><span data-stu-id="9f270-180">Operating system of the device.</span></span> <span data-ttu-id="9f270-181">Windows，iOS 等。继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="9f270-181">Windows, iOS, etc. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9f270-182">deviceType</span><span class="sxs-lookup"><span data-stu-id="9f270-182">deviceType</span></span>|[<span data-ttu-id="9f270-183">deviceType</span><span class="sxs-lookup"><span data-stu-id="9f270-183">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="9f270-184">设备的平台。</span><span class="sxs-lookup"><span data-stu-id="9f270-184">Platform of the device.</span></span> <span data-ttu-id="9f270-185">继承自[managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="9f270-185">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="9f270-186">可能的值为： `desktop`， `windowsRT`， `winMO6`， `nokia`， `windowsPhone`， `mac`， `winCE`， `winEmbedded`， `iPhone`， `iPad`， `iPod`， `android`， `iSocConsumer`， `unix`， `macMDM`， `holoLens`， `surfaceHub`， `androidForWork`， `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="9f270-186">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="9f270-187">complianceState</span><span class="sxs-lookup"><span data-stu-id="9f270-187">complianceState</span></span>|[<span data-ttu-id="9f270-188">complianceState</span><span class="sxs-lookup"><span data-stu-id="9f270-188">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="9f270-189">设备的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="9f270-189">Compliance state of the device.</span></span> <span data-ttu-id="9f270-190">继承自[managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="9f270-190">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="9f270-191">可取值为：`unknown`、`compliant`、`noncompliant`、`conflict`、`error`、`inGracePeriod`、`configManager`。</span><span class="sxs-lookup"><span data-stu-id="9f270-191">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="9f270-192">jailBroken</span><span class="sxs-lookup"><span data-stu-id="9f270-192">jailBroken</span></span>|<span data-ttu-id="9f270-193">String</span><span class="sxs-lookup"><span data-stu-id="9f270-193">String</span></span>|<span data-ttu-id="9f270-194">设备是否已越狱或取得 root 权限。</span><span class="sxs-lookup"><span data-stu-id="9f270-194">whether the device is jail broken or rooted.</span></span> <span data-ttu-id="9f270-195">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="9f270-195">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9f270-196">managementAgent</span><span class="sxs-lookup"><span data-stu-id="9f270-196">managementAgent</span></span>|[<span data-ttu-id="9f270-197">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="9f270-197">managementAgentType</span></span>](../resources/intune-devices-managementagenttype.md)|<span data-ttu-id="9f270-198">设备的管理通道。</span><span class="sxs-lookup"><span data-stu-id="9f270-198">Management channel of the device.</span></span> <span data-ttu-id="9f270-199">Intune、 EAS 等。继承自[managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="9f270-199">Intune, EAS, etc. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="9f270-200">可取值为：`eas`、`mdm`、`easMdm`、`intuneClient`、`easIntuneClient`、`configurationManagerClient`、`configurationManagerClientMdm`、`configurationManagerClientMdmEas`、`unknown`、`jamf`、`googleCloudDevicePolicyController`、`microsoft365ManagedMdm`。</span><span class="sxs-lookup"><span data-stu-id="9f270-200">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span></span>|
|<span data-ttu-id="9f270-201">osVersion</span><span class="sxs-lookup"><span data-stu-id="9f270-201">osVersion</span></span>|<span data-ttu-id="9f270-202">String</span><span class="sxs-lookup"><span data-stu-id="9f270-202">String</span></span>|<span data-ttu-id="9f270-203">设备的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="9f270-203">Operating system version of the device.</span></span> <span data-ttu-id="9f270-204">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="9f270-204">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9f270-205">easActivated</span><span class="sxs-lookup"><span data-stu-id="9f270-205">easActivated</span></span>|<span data-ttu-id="9f270-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f270-206">Boolean</span></span>|<span data-ttu-id="9f270-207">设备是否已激活 Exchange ActiveSync。</span><span class="sxs-lookup"><span data-stu-id="9f270-207">Whether the device is Exchange ActiveSync activated.</span></span> <span data-ttu-id="9f270-208">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="9f270-208">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9f270-209">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="9f270-209">easDeviceId</span></span>|<span data-ttu-id="9f270-210">String</span><span class="sxs-lookup"><span data-stu-id="9f270-210">String</span></span>|<span data-ttu-id="9f270-211">设备的 Exchange ActiveSync ID。</span><span class="sxs-lookup"><span data-stu-id="9f270-211">Exchange ActiveSync Id of the device.</span></span> <span data-ttu-id="9f270-212">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="9f270-212">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9f270-213">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="9f270-213">easActivationDateTime</span></span>|<span data-ttu-id="9f270-214">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f270-214">DateTimeOffset</span></span>|<span data-ttu-id="9f270-215">设备的 Exchange ActivationSync 激活时间。</span><span class="sxs-lookup"><span data-stu-id="9f270-215">Exchange ActivationSync activation time of the device.</span></span> <span data-ttu-id="9f270-216">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="9f270-216">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9f270-217">aadRegistered</span><span class="sxs-lookup"><span data-stu-id="9f270-217">aadRegistered</span></span>|<span data-ttu-id="9f270-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f270-218">Boolean</span></span>|<span data-ttu-id="9f270-219">设备是否已注册 Azure Active Directory。</span><span class="sxs-lookup"><span data-stu-id="9f270-219">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="9f270-220">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="9f270-220">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9f270-221">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="9f270-221">azureADRegistered</span></span>|<span data-ttu-id="9f270-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f270-222">Boolean</span></span>|<span data-ttu-id="9f270-223">设备是否已注册 Azure Active Directory。</span><span class="sxs-lookup"><span data-stu-id="9f270-223">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="9f270-224">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="9f270-224">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9f270-225">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="9f270-225">deviceEnrollmentType</span></span>|[<span data-ttu-id="9f270-226">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="9f270-226">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="9f270-227">设备的注册类型。</span><span class="sxs-lookup"><span data-stu-id="9f270-227">Enrollment type of the device.</span></span> <span data-ttu-id="9f270-228">继承自[managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="9f270-228">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="9f270-229">可取值为：`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement`。</span><span class="sxs-lookup"><span data-stu-id="9f270-229">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="9f270-230">lostModeState</span><span class="sxs-lookup"><span data-stu-id="9f270-230">lostModeState</span></span>|[<span data-ttu-id="9f270-231">lostModeState</span><span class="sxs-lookup"><span data-stu-id="9f270-231">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="9f270-232">指示是否丢失的模式已启用或禁用[managedDevice](../resources/intune-devices-manageddevice.md)继承。</span><span class="sxs-lookup"><span data-stu-id="9f270-232">Indicates if Lost mode is enabled or disabled Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="9f270-233">可取值为：`disabled`、`enabled`。</span><span class="sxs-lookup"><span data-stu-id="9f270-233">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="9f270-234">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="9f270-234">activationLockBypassCode</span></span>|<span data-ttu-id="9f270-235">String</span><span class="sxs-lookup"><span data-stu-id="9f270-235">String</span></span>|<span data-ttu-id="9f270-236">允许绕过设备上的激活锁的代码。</span><span class="sxs-lookup"><span data-stu-id="9f270-236">Code that allows the Activation Lock on a device to be bypassed.</span></span> <span data-ttu-id="9f270-237">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="9f270-237">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9f270-238">emailAddress</span><span class="sxs-lookup"><span data-stu-id="9f270-238">emailAddress</span></span>|<span data-ttu-id="9f270-239">String</span><span class="sxs-lookup"><span data-stu-id="9f270-239">String</span></span>|<span data-ttu-id="9f270-240">与设备继承从[managedDevice](../resources/intune-devices-manageddevice.md)关联的用户的 email(s)</span><span class="sxs-lookup"><span data-stu-id="9f270-240">Email(s) for the user associated with the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9f270-241">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="9f270-241">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="9f270-242">String</span><span class="sxs-lookup"><span data-stu-id="9f270-242">String</span></span>|<span data-ttu-id="9f270-243">Azure Active Directory 设备的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="9f270-243">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="9f270-244">只读。</span><span class="sxs-lookup"><span data-stu-id="9f270-244">Read only.</span></span> <span data-ttu-id="9f270-245">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="9f270-245">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9f270-246">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="9f270-246">azureADDeviceId</span></span>|<span data-ttu-id="9f270-247">String</span><span class="sxs-lookup"><span data-stu-id="9f270-247">String</span></span>|<span data-ttu-id="9f270-248">Azure Active Directory 设备的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="9f270-248">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="9f270-249">只读。</span><span class="sxs-lookup"><span data-stu-id="9f270-249">Read only.</span></span> <span data-ttu-id="9f270-250">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="9f270-250">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9f270-251">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="9f270-251">deviceRegistrationState</span></span>|[<span data-ttu-id="9f270-252">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="9f270-252">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="9f270-253">设备注册状态。</span><span class="sxs-lookup"><span data-stu-id="9f270-253">Device registration state.</span></span> <span data-ttu-id="9f270-254">继承自[managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="9f270-254">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="9f270-255">可取值为：`notRegistered`、`registered`、`revoked`、`keyConflict`、`approvalPending`、`certificateReset`、`notRegisteredPendingEnrollment`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="9f270-255">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="9f270-256">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="9f270-256">deviceCategoryDisplayName</span></span>|<span data-ttu-id="9f270-257">String</span><span class="sxs-lookup"><span data-stu-id="9f270-257">String</span></span>|<span data-ttu-id="9f270-258">从[managedDevice](../resources/intune-devices-manageddevice.md)的设备类别显示名称继承</span><span class="sxs-lookup"><span data-stu-id="9f270-258">Device category display name Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9f270-259">isSupervised</span><span class="sxs-lookup"><span data-stu-id="9f270-259">isSupervised</span></span>|<span data-ttu-id="9f270-260">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f270-260">Boolean</span></span>|<span data-ttu-id="9f270-261">设备管理[managedDevice](../resources/intune-devices-manageddevice.md)状态继承</span><span class="sxs-lookup"><span data-stu-id="9f270-261">Device supervised status Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9f270-262">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="9f270-262">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="9f270-263">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f270-263">DateTimeOffset</span></span>|<span data-ttu-id="9f270-264">设备上次与 Exchange 联系的时间。</span><span class="sxs-lookup"><span data-stu-id="9f270-264">Last time the device contacted Exchange.</span></span> <span data-ttu-id="9f270-265">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="9f270-265">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9f270-266">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="9f270-266">exchangeAccessState</span></span>|[<span data-ttu-id="9f270-267">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="9f270-267">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="9f270-268">Exchange 中设备的访问状态。</span><span class="sxs-lookup"><span data-stu-id="9f270-268">The Access State of the device in Exchange.</span></span> <span data-ttu-id="9f270-269">继承自[managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="9f270-269">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="9f270-270">可取值为：`none`、`unknown`、`allowed`、`blocked`、`quarantined`。</span><span class="sxs-lookup"><span data-stu-id="9f270-270">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="9f270-271">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="9f270-271">exchangeAccessStateReason</span></span>|[<span data-ttu-id="9f270-272">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="9f270-272">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="9f270-273">Exchange 中设备访问状态的出现原因。</span><span class="sxs-lookup"><span data-stu-id="9f270-273">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="9f270-274">继承自[managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="9f270-274">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="9f270-275">可取值为：`none`、`unknown`、`exchangeGlobalRule`、`exchangeIndividualRule`、`exchangeDeviceRule`、`exchangeUpgrade`、`exchangeMailboxPolicy`、`other`、`compliant`、`notCompliant`、`notEnrolled`、`unknownLocation`、`mfaRequired`、`azureADBlockDueToAccessPolicy`、`compromisedPassword`、`deviceNotKnownWithManagedApp`。</span><span class="sxs-lookup"><span data-stu-id="9f270-275">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="9f270-276">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="9f270-276">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="9f270-277">String</span><span class="sxs-lookup"><span data-stu-id="9f270-277">String</span></span>|<span data-ttu-id="9f270-278">允许与设备建立远程协助会话的 URL。</span><span class="sxs-lookup"><span data-stu-id="9f270-278">Url that allows a Remote Assistance session to be established with the device.</span></span> <span data-ttu-id="9f270-279">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="9f270-279">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9f270-280">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="9f270-280">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="9f270-281">String</span><span class="sxs-lookup"><span data-stu-id="9f270-281">String</span></span>|<span data-ttu-id="9f270-282">用于在创建远程协助会话对象时识别问题的错误字符串。</span><span class="sxs-lookup"><span data-stu-id="9f270-282">An error string that identifies issues when creating Remote Assistance session objects.</span></span> <span data-ttu-id="9f270-283">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="9f270-283">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9f270-284">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="9f270-284">isEncrypted</span></span>|<span data-ttu-id="9f270-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f270-285">Boolean</span></span>|<span data-ttu-id="9f270-286">从[managedDevice](../resources/intune-devices-manageddevice.md)设备加密状态继承</span><span class="sxs-lookup"><span data-stu-id="9f270-286">Device encryption status Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9f270-287">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="9f270-287">userPrincipalName</span></span>|<span data-ttu-id="9f270-288">字符串</span><span class="sxs-lookup"><span data-stu-id="9f270-288">String</span></span>|<span data-ttu-id="9f270-289">设备用户主体名称继承从[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="9f270-289">Device user principal name Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9f270-290">model</span><span class="sxs-lookup"><span data-stu-id="9f270-290">model</span></span>|<span data-ttu-id="9f270-291">String</span><span class="sxs-lookup"><span data-stu-id="9f270-291">String</span></span>|<span data-ttu-id="9f270-292">从[managedDevice](../resources/intune-devices-manageddevice.md)的设备继承的型号</span><span class="sxs-lookup"><span data-stu-id="9f270-292">Model of the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9f270-293">manufacturer</span><span class="sxs-lookup"><span data-stu-id="9f270-293">manufacturer</span></span>|<span data-ttu-id="9f270-294">String</span><span class="sxs-lookup"><span data-stu-id="9f270-294">String</span></span>|<span data-ttu-id="9f270-295">从[managedDevice](../resources/intune-devices-manageddevice.md)继承设备的制造商</span><span class="sxs-lookup"><span data-stu-id="9f270-295">Manufacturer of the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9f270-296">imei</span><span class="sxs-lookup"><span data-stu-id="9f270-296">imei</span></span>|<span data-ttu-id="9f270-297">String</span><span class="sxs-lookup"><span data-stu-id="9f270-297">String</span></span>|<span data-ttu-id="9f270-298">IMEI 继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="9f270-298">IMEI Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9f270-299">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="9f270-299">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="9f270-300">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f270-300">DateTimeOffset</span></span>|<span data-ttu-id="9f270-301">当设备合规性宽限期继承从[managedDevice](../resources/intune-devices-manageddevice.md) DateTime</span><span class="sxs-lookup"><span data-stu-id="9f270-301">The DateTime when device compliance grace period expires Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9f270-302">serialNumber</span><span class="sxs-lookup"><span data-stu-id="9f270-302">serialNumber</span></span>|<span data-ttu-id="9f270-303">字符串</span><span class="sxs-lookup"><span data-stu-id="9f270-303">String</span></span>|<span data-ttu-id="9f270-304">SerialNumber 继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="9f270-304">SerialNumber Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9f270-305">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="9f270-305">phoneNumber</span></span>|<span data-ttu-id="9f270-306">String</span><span class="sxs-lookup"><span data-stu-id="9f270-306">String</span></span>|<span data-ttu-id="9f270-307">从[managedDevice](../resources/intune-devices-manageddevice.md)继承设备的电话号码</span><span class="sxs-lookup"><span data-stu-id="9f270-307">Phone number of the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9f270-308">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="9f270-308">androidSecurityPatchLevel</span></span>|<span data-ttu-id="9f270-309">String</span><span class="sxs-lookup"><span data-stu-id="9f270-309">String</span></span>|<span data-ttu-id="9f270-310">从[managedDevice](../resources/intune-devices-manageddevice.md) android 安全修补程序级别继承</span><span class="sxs-lookup"><span data-stu-id="9f270-310">Android security patch level Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9f270-311">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="9f270-311">userDisplayName</span></span>|<span data-ttu-id="9f270-312">String</span><span class="sxs-lookup"><span data-stu-id="9f270-312">String</span></span>|<span data-ttu-id="9f270-313">从[managedDevice](../resources/intune-devices-manageddevice.md)的用户显示名称继承</span><span class="sxs-lookup"><span data-stu-id="9f270-313">User display name Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9f270-314">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="9f270-314">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="9f270-315">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="9f270-315">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="9f270-316">启用功能继承[managedDevice](../resources/intune-devices-manageddevice.md) ConfigrMgr 客户端</span><span class="sxs-lookup"><span data-stu-id="9f270-316">ConfigrMgr client enabled features Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9f270-317">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="9f270-317">wiFiMacAddress</span></span>|<span data-ttu-id="9f270-318">String</span><span class="sxs-lookup"><span data-stu-id="9f270-318">String</span></span>|<span data-ttu-id="9f270-319">Wi-fi MAC 继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="9f270-319">Wi-Fi MAC Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9f270-320">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="9f270-320">deviceHealthAttestationState</span></span>|[<span data-ttu-id="9f270-321">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="9f270-321">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="9f270-322">设备运行状况证明状态。</span><span class="sxs-lookup"><span data-stu-id="9f270-322">The device health attestation state.</span></span> <span data-ttu-id="9f270-323">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="9f270-323">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9f270-324">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="9f270-324">subscriberCarrier</span></span>|<span data-ttu-id="9f270-325">String</span><span class="sxs-lookup"><span data-stu-id="9f270-325">String</span></span>|<span data-ttu-id="9f270-326">订阅者运营商继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="9f270-326">Subscriber Carrier Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9f270-327">meid</span><span class="sxs-lookup"><span data-stu-id="9f270-327">meid</span></span>|<span data-ttu-id="9f270-328">String</span><span class="sxs-lookup"><span data-stu-id="9f270-328">String</span></span>|<span data-ttu-id="9f270-329">MEID 继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="9f270-329">MEID Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9f270-330">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="9f270-330">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="9f270-331">Int64</span><span class="sxs-lookup"><span data-stu-id="9f270-331">Int64</span></span>|<span data-ttu-id="9f270-332">总存储在字节继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="9f270-332">Total Storage in Bytes Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9f270-333">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="9f270-333">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="9f270-334">Int64</span><span class="sxs-lookup"><span data-stu-id="9f270-334">Int64</span></span>|<span data-ttu-id="9f270-335">字节继承自[managedDevice](../resources/intune-devices-manageddevice.md)中的可用存储</span><span class="sxs-lookup"><span data-stu-id="9f270-335">Free Storage in Bytes Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9f270-336">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="9f270-336">managedDeviceName</span></span>|<span data-ttu-id="9f270-337">String</span><span class="sxs-lookup"><span data-stu-id="9f270-337">String</span></span>|<span data-ttu-id="9f270-338">用于识别设备的自动生成的名称。</span><span class="sxs-lookup"><span data-stu-id="9f270-338">Automatically generated name to identify a device.</span></span> <span data-ttu-id="9f270-339">可以覆盖为用户友好名称。</span><span class="sxs-lookup"><span data-stu-id="9f270-339">Can be overwritten to a user friendly name.</span></span> <span data-ttu-id="9f270-340">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="9f270-340">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9f270-341">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="9f270-341">partnerReportedThreatState</span></span>|[<span data-ttu-id="9f270-342">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="9f270-342">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="9f270-343">指示帐户和设备正在使用移动威胁防护合作伙伴时设备的威胁状态。</span><span class="sxs-lookup"><span data-stu-id="9f270-343">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="9f270-344">只读。</span><span class="sxs-lookup"><span data-stu-id="9f270-344">Read Only.</span></span> <span data-ttu-id="9f270-345">继承自[managedDevice](../resources/intune-devices-manageddevice.md)。</span><span class="sxs-lookup"><span data-stu-id="9f270-345">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="9f270-346">可取值为：`unknown`、`activated`、`deactivated`、`secured`、`lowSeverity`、`mediumSeverity`、`highSeverity`、`unresponsive`、`compromised`、`misconfigured`。</span><span class="sxs-lookup"><span data-stu-id="9f270-346">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="9f270-347">usersLoggedOn</span><span class="sxs-lookup"><span data-stu-id="9f270-347">usersLoggedOn</span></span>|<span data-ttu-id="9f270-348">[loggedOnUser](../resources/intune-devices-loggedonuser.md)集合</span><span class="sxs-lookup"><span data-stu-id="9f270-348">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="9f270-349">指示上次登录的用户从[managedDevice](../resources/intune-devices-manageddevice.md)设备继承</span><span class="sxs-lookup"><span data-stu-id="9f270-349">Indicates the last logged on users of a device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9f270-350">preferMdmOverGroupPolicyAppliedDateTime</span><span class="sxs-lookup"><span data-stu-id="9f270-350">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="9f270-351">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f270-351">DateTimeOffset</span></span>|<span data-ttu-id="9f270-352">报告 DateTime 的 preferMdmOverGroupPolicy 设置。</span><span class="sxs-lookup"><span data-stu-id="9f270-352">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="9f270-353">设置时，这些 Intune MDM 设置将覆盖组策略设置冲突时。</span><span class="sxs-lookup"><span data-stu-id="9f270-353">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="9f270-354">只读。</span><span class="sxs-lookup"><span data-stu-id="9f270-354">Read Only.</span></span> <span data-ttu-id="9f270-355">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="9f270-355">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9f270-356">autopilotEnrolled</span><span class="sxs-lookup"><span data-stu-id="9f270-356">autopilotEnrolled</span></span>|<span data-ttu-id="9f270-357">布尔</span><span class="sxs-lookup"><span data-stu-id="9f270-357">Boolean</span></span>|<span data-ttu-id="9f270-358">如果通过自动试点注册托管的设备，报告。</span><span class="sxs-lookup"><span data-stu-id="9f270-358">Reports if the managed device is enrolled via auto-pilot.</span></span> <span data-ttu-id="9f270-359">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="9f270-359">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9f270-360">requireUserEnrollmentApproval</span><span class="sxs-lookup"><span data-stu-id="9f270-360">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="9f270-361">布尔</span><span class="sxs-lookup"><span data-stu-id="9f270-361">Boolean</span></span>|<span data-ttu-id="9f270-362">报告托管的 iOS 设备是否用户审批注册。</span><span class="sxs-lookup"><span data-stu-id="9f270-362">Reports if the managed iOS device is user approval enrollment.</span></span> <span data-ttu-id="9f270-363">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="9f270-363">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9f270-364">managementCertificateExpirationDate</span><span class="sxs-lookup"><span data-stu-id="9f270-364">managementCertificateExpirationDate</span></span>|<span data-ttu-id="9f270-365">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f270-365">DateTimeOffset</span></span>|<span data-ttu-id="9f270-366">报告设备管理证书过期日期继承从[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="9f270-366">Reports device management certificate expiration date Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9f270-367">iccid</span><span class="sxs-lookup"><span data-stu-id="9f270-367">iccid</span></span>|<span data-ttu-id="9f270-368">字符串</span><span class="sxs-lookup"><span data-stu-id="9f270-368">String</span></span>|<span data-ttu-id="9f270-369">集成的电路卡标识符，它是 SIM 卡的唯一标识号。</span><span class="sxs-lookup"><span data-stu-id="9f270-369">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span> <span data-ttu-id="9f270-370">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="9f270-370">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9f270-371">udid</span><span class="sxs-lookup"><span data-stu-id="9f270-371">udid</span></span>|<span data-ttu-id="9f270-372">字符串</span><span class="sxs-lookup"><span data-stu-id="9f270-372">String</span></span>|<span data-ttu-id="9f270-373">IOS 和 macOS 设备的唯一设备标识符。</span><span class="sxs-lookup"><span data-stu-id="9f270-373">Unique Device Identifier for iOS and macOS devices.</span></span> <span data-ttu-id="9f270-374">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="9f270-374">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9f270-375">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9f270-375">roleScopeTagIds</span></span>|<span data-ttu-id="9f270-376">String 集合</span><span class="sxs-lookup"><span data-stu-id="9f270-376">String collection</span></span>|<span data-ttu-id="9f270-377">此设备实例范围标记 Id 的列表。</span><span class="sxs-lookup"><span data-stu-id="9f270-377">List of Scope Tag IDs for this Device instance.</span></span> <span data-ttu-id="9f270-378">继承自[managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="9f270-378">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9f270-379">windowsActiveMalwareCount</span><span class="sxs-lookup"><span data-stu-id="9f270-379">windowsActiveMalwareCount</span></span>|<span data-ttu-id="9f270-380">Int32</span><span class="sxs-lookup"><span data-stu-id="9f270-380">Int32</span></span>|<span data-ttu-id="9f270-381">从[managedDevice](../resources/intune-devices-manageddevice.md)此 windows 设备继承的活动恶意软件的计数</span><span class="sxs-lookup"><span data-stu-id="9f270-381">Count of active malware for this windows device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9f270-382">windowsRemediatedMalwareCount</span><span class="sxs-lookup"><span data-stu-id="9f270-382">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="9f270-383">Int32</span><span class="sxs-lookup"><span data-stu-id="9f270-383">Int32</span></span>|<span data-ttu-id="9f270-384">从[managedDevice](../resources/intune-devices-manageddevice.md)此 windows 设备继承的补救恶意软件的计数</span><span class="sxs-lookup"><span data-stu-id="9f270-384">Count of remediated malware for this windows device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9f270-385">notes</span><span class="sxs-lookup"><span data-stu-id="9f270-385">notes</span></span>|<span data-ttu-id="9f270-386">String</span><span class="sxs-lookup"><span data-stu-id="9f270-386">String</span></span>|<span data-ttu-id="9f270-387">创建从[managedDevice](../resources/intune-devices-manageddevice.md)由 IT 管理员继承的设备的说明</span><span class="sxs-lookup"><span data-stu-id="9f270-387">Notes on the device created by IT Admin Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9f270-388">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="9f270-388">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="9f270-389">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="9f270-389">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="9f270-390">配置管理器客户端健康状态，仅供设备从[managedDevice](../resources/intune-devices-manageddevice.md)由继承 MDM/ConfigMgr 代理管理</span><span class="sxs-lookup"><span data-stu-id="9f270-390">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|



## <a name="response"></a><span data-ttu-id="9f270-391">响应</span><span class="sxs-lookup"><span data-stu-id="9f270-391">Response</span></span>
<span data-ttu-id="9f270-392">如果成功，此方法返回`201 Created`响应代码和响应正文中的[windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9f270-392">If successful, this method returns a `201 Created` response code and a [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f270-393">示例</span><span class="sxs-lookup"><span data-stu-id="9f270-393">Example</span></span>
### <a name="request"></a><span data-ttu-id="9f270-394">请求</span><span class="sxs-lookup"><span data-stu-id="9f270-394">Request</span></span>
<span data-ttu-id="9f270-395">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9f270-395">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/managedDevices
Content-type: application/json
Content-length: 7173

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
    "windowsUpdateForBusiness": true
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

### <a name="response"></a><span data-ttu-id="9f270-396">响应</span><span class="sxs-lookup"><span data-stu-id="9f270-396">Response</span></span>
<span data-ttu-id="9f270-p142">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9f270-p142">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 7222

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
    "windowsUpdateForBusiness": true
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





