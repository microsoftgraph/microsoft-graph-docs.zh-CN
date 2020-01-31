---
title: 创建 iosUpdateConfiguration
description: 创建新的 iosUpdateConfiguration 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d6dffd868494cac581adc6be75f2ad00ac4f0a7f
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/31/2020
ms.locfileid: "41635886"
---
# <a name="create-iosupdateconfiguration"></a><span data-ttu-id="aa834-103">创建 iosUpdateConfiguration</span><span class="sxs-lookup"><span data-stu-id="aa834-103">Create iosUpdateConfiguration</span></span>

> <span data-ttu-id="aa834-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="aa834-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aa834-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="aa834-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aa834-106">创建新的 [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="aa834-106">Create a new [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aa834-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="aa834-107">Prerequisites</span></span>
<span data-ttu-id="aa834-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="aa834-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aa834-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="aa834-110">Permission type</span></span>|<span data-ttu-id="aa834-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="aa834-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aa834-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aa834-112">Delegated (work or school account)</span></span>|<span data-ttu-id="aa834-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa834-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="aa834-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aa834-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aa834-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="aa834-115">Not supported.</span></span>|
|<span data-ttu-id="aa834-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="aa834-116">Application</span></span>|<span data-ttu-id="aa834-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa834-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="aa834-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="aa834-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="aa834-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="aa834-119">Request headers</span></span>
|<span data-ttu-id="aa834-120">标头</span><span class="sxs-lookup"><span data-stu-id="aa834-120">Header</span></span>|<span data-ttu-id="aa834-121">值</span><span class="sxs-lookup"><span data-stu-id="aa834-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aa834-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="aa834-122">Authorization</span></span>|<span data-ttu-id="aa834-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="aa834-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aa834-124">接受</span><span class="sxs-lookup"><span data-stu-id="aa834-124">Accept</span></span>|<span data-ttu-id="aa834-125">application/json</span><span class="sxs-lookup"><span data-stu-id="aa834-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aa834-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="aa834-126">Request body</span></span>
<span data-ttu-id="aa834-127">在请求正文中，提供 iosUpdateConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aa834-127">In the request body, supply a JSON representation for the iosUpdateConfiguration object.</span></span>

<span data-ttu-id="aa834-128">下表显示创建 iosUpdateConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="aa834-128">The following table shows the properties that are required when you create the iosUpdateConfiguration.</span></span>

|<span data-ttu-id="aa834-129">属性</span><span class="sxs-lookup"><span data-stu-id="aa834-129">Property</span></span>|<span data-ttu-id="aa834-130">类型</span><span class="sxs-lookup"><span data-stu-id="aa834-130">Type</span></span>|<span data-ttu-id="aa834-131">Description</span><span class="sxs-lookup"><span data-stu-id="aa834-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa834-132">id</span><span class="sxs-lookup"><span data-stu-id="aa834-132">id</span></span>|<span data-ttu-id="aa834-133">字符串</span><span class="sxs-lookup"><span data-stu-id="aa834-133">String</span></span>|<span data-ttu-id="aa834-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="aa834-134">Key of the entity.</span></span> <span data-ttu-id="aa834-135">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aa834-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aa834-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="aa834-136">lastModifiedDateTime</span></span>|<span data-ttu-id="aa834-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aa834-137">DateTimeOffset</span></span>|<span data-ttu-id="aa834-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="aa834-138">DateTime the object was last modified.</span></span> <span data-ttu-id="aa834-139">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aa834-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aa834-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="aa834-140">roleScopeTagIds</span></span>|<span data-ttu-id="aa834-141">String 集合</span><span class="sxs-lookup"><span data-stu-id="aa834-141">String collection</span></span>|<span data-ttu-id="aa834-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="aa834-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="aa834-143">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aa834-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aa834-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="aa834-144">supportsScopeTags</span></span>|<span data-ttu-id="aa834-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="aa834-145">Boolean</span></span>|<span data-ttu-id="aa834-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="aa834-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="aa834-147">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="aa834-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="aa834-148">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="aa834-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="aa834-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="aa834-149">This property is read-only.</span></span> <span data-ttu-id="aa834-150">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aa834-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aa834-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="aa834-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="aa834-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="aa834-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="aa834-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="aa834-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="aa834-154">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aa834-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aa834-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="aa834-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="aa834-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="aa834-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="aa834-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="aa834-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="aa834-158">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aa834-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aa834-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="aa834-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="aa834-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="aa834-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="aa834-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="aa834-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="aa834-162">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aa834-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aa834-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="aa834-163">createdDateTime</span></span>|<span data-ttu-id="aa834-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aa834-164">DateTimeOffset</span></span>|<span data-ttu-id="aa834-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="aa834-165">DateTime the object was created.</span></span> <span data-ttu-id="aa834-166">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aa834-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aa834-167">说明</span><span class="sxs-lookup"><span data-stu-id="aa834-167">description</span></span>|<span data-ttu-id="aa834-168">String</span><span class="sxs-lookup"><span data-stu-id="aa834-168">String</span></span>|<span data-ttu-id="aa834-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="aa834-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="aa834-170">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aa834-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aa834-171">displayName</span><span class="sxs-lookup"><span data-stu-id="aa834-171">displayName</span></span>|<span data-ttu-id="aa834-172">String</span><span class="sxs-lookup"><span data-stu-id="aa834-172">String</span></span>|<span data-ttu-id="aa834-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="aa834-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="aa834-174">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aa834-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aa834-175">version</span><span class="sxs-lookup"><span data-stu-id="aa834-175">version</span></span>|<span data-ttu-id="aa834-176">Int32</span><span class="sxs-lookup"><span data-stu-id="aa834-176">Int32</span></span>|<span data-ttu-id="aa834-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="aa834-177">Version of the device configuration.</span></span> <span data-ttu-id="aa834-178">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aa834-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aa834-179">isEnabled</span><span class="sxs-lookup"><span data-stu-id="aa834-179">isEnabled</span></span>|<span data-ttu-id="aa834-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="aa834-180">Boolean</span></span>|<span data-ttu-id="aa834-181">在 UI 中是否启用了设置</span><span class="sxs-lookup"><span data-stu-id="aa834-181">Is setting enabled in UI</span></span>|
|<span data-ttu-id="aa834-182">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="aa834-182">activeHoursStart</span></span>|<span data-ttu-id="aa834-183">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="aa834-183">TimeOfDay</span></span>|<span data-ttu-id="aa834-184">使用时段开始时间（使用时段表示不应发生更新安装的时间范围）</span><span class="sxs-lookup"><span data-stu-id="aa834-184">Active Hours Start (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="aa834-185">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="aa834-185">activeHoursEnd</span></span>|<span data-ttu-id="aa834-186">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="aa834-186">TimeOfDay</span></span>|<span data-ttu-id="aa834-187">使用时段结束时间（使用时段表示不应发生更新安装的时间范围）</span><span class="sxs-lookup"><span data-stu-id="aa834-187">Active Hours End (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="aa834-188">desiredOsVersion</span><span class="sxs-lookup"><span data-stu-id="aa834-188">desiredOsVersion</span></span>|<span data-ttu-id="aa834-189">字符串</span><span class="sxs-lookup"><span data-stu-id="aa834-189">String</span></span>|<span data-ttu-id="aa834-190">如果未指定，设备将更新到最新版本的操作系统。</span><span class="sxs-lookup"><span data-stu-id="aa834-190">If left unspecified, devices will update to the latest version of the OS.</span></span>|
|<span data-ttu-id="aa834-191">scheduledInstallDays</span><span class="sxs-lookup"><span data-stu-id="aa834-191">scheduledInstallDays</span></span>|<span data-ttu-id="aa834-192">[dayOfWeek](../resources/intune-deviceconfig-dayofweek.md)集合</span><span class="sxs-lookup"><span data-stu-id="aa834-192">[dayOfWeek](../resources/intune-deviceconfig-dayofweek.md) collection</span></span>|<span data-ttu-id="aa834-193">配置为使用时段所对应的一周的某一天。</span><span class="sxs-lookup"><span data-stu-id="aa834-193">Days in week for which active hours are configured.</span></span> <span data-ttu-id="aa834-194">该集合最多可包含 7 个元素。</span><span class="sxs-lookup"><span data-stu-id="aa834-194">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="aa834-195">可取值为：`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday`。</span><span class="sxs-lookup"><span data-stu-id="aa834-195">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="aa834-196">utcTimeOffsetInMinutes</span><span class="sxs-lookup"><span data-stu-id="aa834-196">utcTimeOffsetInMinutes</span></span>|<span data-ttu-id="aa834-197">Int32</span><span class="sxs-lookup"><span data-stu-id="aa834-197">Int32</span></span>|<span data-ttu-id="aa834-198">UTC 时间偏移，用分钟表示</span><span class="sxs-lookup"><span data-stu-id="aa834-198">UTC Time Offset indicated in minutes</span></span>|
|<span data-ttu-id="aa834-199">enforcedSoftwareUpdateDelayInDays</span><span class="sxs-lookup"><span data-stu-id="aa834-199">enforcedSoftwareUpdateDelayInDays</span></span>|<span data-ttu-id="aa834-200">Int32</span><span class="sxs-lookup"><span data-stu-id="aa834-200">Int32</span></span>|<span data-ttu-id="aa834-201">软件更新在 iOS 设备中可见的天数，范围从0到90（含0到）</span><span class="sxs-lookup"><span data-stu-id="aa834-201">Days before software updates are visible to iOS devices ranging from 0 to 90 inclusive</span></span>|



## <a name="response"></a><span data-ttu-id="aa834-202">响应</span><span class="sxs-lookup"><span data-stu-id="aa834-202">Response</span></span>
<span data-ttu-id="aa834-203">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="aa834-203">If successful, this method returns a `201 Created` response code and a [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aa834-204">示例</span><span class="sxs-lookup"><span data-stu-id="aa834-204">Example</span></span>

### <a name="request"></a><span data-ttu-id="aa834-205">请求</span><span class="sxs-lookup"><span data-stu-id="aa834-205">Request</span></span>
<span data-ttu-id="aa834-206">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="aa834-206">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1306

{
  "@odata.type": "#microsoft.graph.iosUpdateConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "isEnabled": true,
  "activeHoursStart": "12:00:05.5020000",
  "activeHoursEnd": "11:59:00.8990000",
  "desiredOsVersion": "Desired Os Version value",
  "scheduledInstallDays": [
    "monday"
  ],
  "utcTimeOffsetInMinutes": 6,
  "enforcedSoftwareUpdateDelayInDays": 1
}
```

### <a name="response"></a><span data-ttu-id="aa834-207">响应</span><span class="sxs-lookup"><span data-stu-id="aa834-207">Response</span></span>
<span data-ttu-id="aa834-p114">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="aa834-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1478

{
  "@odata.type": "#microsoft.graph.iosUpdateConfiguration",
  "id": "321aef09-ef09-321a-09ef-1a3209ef1a32",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "isEnabled": true,
  "activeHoursStart": "12:00:05.5020000",
  "activeHoursEnd": "11:59:00.8990000",
  "desiredOsVersion": "Desired Os Version value",
  "scheduledInstallDays": [
    "monday"
  ],
  "utcTimeOffsetInMinutes": 6,
  "enforcedSoftwareUpdateDelayInDays": 1
}
```





