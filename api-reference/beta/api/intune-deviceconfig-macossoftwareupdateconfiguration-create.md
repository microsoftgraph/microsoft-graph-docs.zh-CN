---
title: 创建 macOSSoftwareUpdateConfiguration
description: 创建新的 macOSSoftwareUpdateConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0e7d58e0543daaefe92d21e5081332d12391b41c
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51132644"
---
# <a name="create-macossoftwareupdateconfiguration"></a><span data-ttu-id="56848-103">创建 macOSSoftwareUpdateConfiguration</span><span class="sxs-lookup"><span data-stu-id="56848-103">Create macOSSoftwareUpdateConfiguration</span></span>

<span data-ttu-id="56848-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="56848-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="56848-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="56848-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="56848-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="56848-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="56848-107">创建新的 [macOSSoftwareUpdateConfiguration](../resources/intune-deviceconfig-macossoftwareupdateconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="56848-107">Create a new [macOSSoftwareUpdateConfiguration](../resources/intune-deviceconfig-macossoftwareupdateconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="56848-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="56848-108">Prerequisites</span></span>
<span data-ttu-id="56848-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="56848-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56848-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="56848-111">Permission type</span></span>|<span data-ttu-id="56848-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="56848-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="56848-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="56848-113">Delegated (work or school account)</span></span>|<span data-ttu-id="56848-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56848-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="56848-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="56848-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="56848-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="56848-116">Not supported.</span></span>|
|<span data-ttu-id="56848-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="56848-117">Application</span></span>|<span data-ttu-id="56848-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56848-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="56848-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="56848-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="56848-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="56848-120">Request headers</span></span>
|<span data-ttu-id="56848-121">标头</span><span class="sxs-lookup"><span data-stu-id="56848-121">Header</span></span>|<span data-ttu-id="56848-122">值</span><span class="sxs-lookup"><span data-stu-id="56848-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="56848-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="56848-123">Authorization</span></span>|<span data-ttu-id="56848-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="56848-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="56848-125">接受</span><span class="sxs-lookup"><span data-stu-id="56848-125">Accept</span></span>|<span data-ttu-id="56848-126">application/json</span><span class="sxs-lookup"><span data-stu-id="56848-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="56848-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="56848-127">Request body</span></span>
<span data-ttu-id="56848-128">在请求正文中，提供 macOSSoftwareUpdateConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="56848-128">In the request body, supply a JSON representation for the macOSSoftwareUpdateConfiguration object.</span></span>

<span data-ttu-id="56848-129">下表显示创建 macOSSoftwareUpdateConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="56848-129">The following table shows the properties that are required when you create the macOSSoftwareUpdateConfiguration.</span></span>

|<span data-ttu-id="56848-130">属性</span><span class="sxs-lookup"><span data-stu-id="56848-130">Property</span></span>|<span data-ttu-id="56848-131">类型</span><span class="sxs-lookup"><span data-stu-id="56848-131">Type</span></span>|<span data-ttu-id="56848-132">说明</span><span class="sxs-lookup"><span data-stu-id="56848-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56848-133">id</span><span class="sxs-lookup"><span data-stu-id="56848-133">id</span></span>|<span data-ttu-id="56848-134">String</span><span class="sxs-lookup"><span data-stu-id="56848-134">String</span></span>|<span data-ttu-id="56848-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="56848-135">Key of the entity.</span></span> <span data-ttu-id="56848-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="56848-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="56848-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="56848-137">lastModifiedDateTime</span></span>|<span data-ttu-id="56848-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="56848-138">DateTimeOffset</span></span>|<span data-ttu-id="56848-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="56848-139">DateTime the object was last modified.</span></span> <span data-ttu-id="56848-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="56848-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="56848-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="56848-141">roleScopeTagIds</span></span>|<span data-ttu-id="56848-142">String collection</span><span class="sxs-lookup"><span data-stu-id="56848-142">String collection</span></span>|<span data-ttu-id="56848-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="56848-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="56848-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="56848-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="56848-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="56848-145">supportsScopeTags</span></span>|<span data-ttu-id="56848-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="56848-146">Boolean</span></span>|<span data-ttu-id="56848-147">指示基础设备配置是否支持分配范围标记。</span><span class="sxs-lookup"><span data-stu-id="56848-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="56848-148">当此值为 false 且实体对作用域用户不可见时，不允许分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="56848-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="56848-149">这适用于在 Silverlight 中创建的旧版策略，可通过在 Azure 门户中删除和重新创建策略来解决。</span><span class="sxs-lookup"><span data-stu-id="56848-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="56848-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="56848-150">This property is read-only.</span></span> <span data-ttu-id="56848-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="56848-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="56848-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="56848-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="56848-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="56848-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="56848-154">此策略的操作系统版本适用性。</span><span class="sxs-lookup"><span data-stu-id="56848-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="56848-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="56848-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="56848-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="56848-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="56848-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="56848-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="56848-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="56848-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="56848-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="56848-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="56848-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="56848-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="56848-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="56848-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="56848-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="56848-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="56848-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="56848-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="56848-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="56848-164">createdDateTime</span></span>|<span data-ttu-id="56848-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="56848-165">DateTimeOffset</span></span>|<span data-ttu-id="56848-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="56848-166">DateTime the object was created.</span></span> <span data-ttu-id="56848-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="56848-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="56848-168">说明</span><span class="sxs-lookup"><span data-stu-id="56848-168">description</span></span>|<span data-ttu-id="56848-169">String</span><span class="sxs-lookup"><span data-stu-id="56848-169">String</span></span>|<span data-ttu-id="56848-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="56848-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="56848-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="56848-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="56848-172">displayName</span><span class="sxs-lookup"><span data-stu-id="56848-172">displayName</span></span>|<span data-ttu-id="56848-173">String</span><span class="sxs-lookup"><span data-stu-id="56848-173">String</span></span>|<span data-ttu-id="56848-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="56848-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="56848-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="56848-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="56848-176">version</span><span class="sxs-lookup"><span data-stu-id="56848-176">version</span></span>|<span data-ttu-id="56848-177">Int32</span><span class="sxs-lookup"><span data-stu-id="56848-177">Int32</span></span>|<span data-ttu-id="56848-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="56848-178">Version of the device configuration.</span></span> <span data-ttu-id="56848-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="56848-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="56848-180">criticalUpdateBehavior</span><span class="sxs-lookup"><span data-stu-id="56848-180">criticalUpdateBehavior</span></span>|[<span data-ttu-id="56848-181">macOSSoftwareUpdateBehavior</span><span class="sxs-lookup"><span data-stu-id="56848-181">macOSSoftwareUpdateBehavior</span></span>](../resources/intune-deviceconfig-macossoftwareupdatebehavior.md)|<span data-ttu-id="56848-182">关键更新的更新行为。</span><span class="sxs-lookup"><span data-stu-id="56848-182">Update behavior for critical updates.</span></span> <span data-ttu-id="56848-183">可取值为：`notConfigured`、`default`。</span><span class="sxs-lookup"><span data-stu-id="56848-183">Possible values are: `notConfigured`, `default`.</span></span>|
|<span data-ttu-id="56848-184">configDataUpdateBehavior</span><span class="sxs-lookup"><span data-stu-id="56848-184">configDataUpdateBehavior</span></span>|[<span data-ttu-id="56848-185">macOSSoftwareUpdateBehavior</span><span class="sxs-lookup"><span data-stu-id="56848-185">macOSSoftwareUpdateBehavior</span></span>](../resources/intune-deviceconfig-macossoftwareupdatebehavior.md)|<span data-ttu-id="56848-186">配置文件更新的更新行为。</span><span class="sxs-lookup"><span data-stu-id="56848-186">Update behavior for configuration data file updates.</span></span> <span data-ttu-id="56848-187">可取值为：`notConfigured`、`default`。</span><span class="sxs-lookup"><span data-stu-id="56848-187">Possible values are: `notConfigured`, `default`.</span></span>|
|<span data-ttu-id="56848-188">firmwareUpdateBehavior</span><span class="sxs-lookup"><span data-stu-id="56848-188">firmwareUpdateBehavior</span></span>|[<span data-ttu-id="56848-189">macOSSoftwareUpdateBehavior</span><span class="sxs-lookup"><span data-stu-id="56848-189">macOSSoftwareUpdateBehavior</span></span>](../resources/intune-deviceconfig-macossoftwareupdatebehavior.md)|<span data-ttu-id="56848-190">固件更新的更新行为。</span><span class="sxs-lookup"><span data-stu-id="56848-190">Update behavior for firmware updates.</span></span> <span data-ttu-id="56848-191">可取值为：`notConfigured`、`default`。</span><span class="sxs-lookup"><span data-stu-id="56848-191">Possible values are: `notConfigured`, `default`.</span></span>|
|<span data-ttu-id="56848-192">allOtherUpdateBehavior</span><span class="sxs-lookup"><span data-stu-id="56848-192">allOtherUpdateBehavior</span></span>|[<span data-ttu-id="56848-193">macOSSoftwareUpdateBehavior</span><span class="sxs-lookup"><span data-stu-id="56848-193">macOSSoftwareUpdateBehavior</span></span>](../resources/intune-deviceconfig-macossoftwareupdatebehavior.md)|<span data-ttu-id="56848-194">所有其他更新的更新行为。</span><span class="sxs-lookup"><span data-stu-id="56848-194">Update behavior for all other updates.</span></span> <span data-ttu-id="56848-195">可取值为：`notConfigured`、`default`。</span><span class="sxs-lookup"><span data-stu-id="56848-195">Possible values are: `notConfigured`, `default`.</span></span>|
|<span data-ttu-id="56848-196">updateScheduleType</span><span class="sxs-lookup"><span data-stu-id="56848-196">updateScheduleType</span></span>|[<span data-ttu-id="56848-197">macOSSoftwareUpdateScheduleType</span><span class="sxs-lookup"><span data-stu-id="56848-197">macOSSoftwareUpdateScheduleType</span></span>](../resources/intune-deviceconfig-macossoftwareupdatescheduletype.md)|<span data-ttu-id="56848-198">更新计划类型。</span><span class="sxs-lookup"><span data-stu-id="56848-198">Update schedule type.</span></span> <span data-ttu-id="56848-199">可取值为：`alwaysUpdate`、`updateDuringTimeWindows`、`updateOutsideOfTimeWindows`。</span><span class="sxs-lookup"><span data-stu-id="56848-199">Possible values are: `alwaysUpdate`, `updateDuringTimeWindows`, `updateOutsideOfTimeWindows`.</span></span>|
|<span data-ttu-id="56848-200">customUpdateTimeWindows</span><span class="sxs-lookup"><span data-stu-id="56848-200">customUpdateTimeWindows</span></span>|<span data-ttu-id="56848-201">[customUpdateTimeWindow](../resources/intune-deviceconfig-customupdatetimewindow.md) 集合</span><span class="sxs-lookup"><span data-stu-id="56848-201">[customUpdateTimeWindow](../resources/intune-deviceconfig-customupdatetimewindow.md) collection</span></span>|<span data-ttu-id="56848-202">允许或阻止更新的自定义时间窗口。</span><span class="sxs-lookup"><span data-stu-id="56848-202">Custom Time windows when updates will be allowed or blocked.</span></span> <span data-ttu-id="56848-203">此集合最多可包含 20 个元素。</span><span class="sxs-lookup"><span data-stu-id="56848-203">This collection can contain a maximum of 20 elements.</span></span>|
|<span data-ttu-id="56848-204">updateTimeWindowUtcOffsetInMinutes</span><span class="sxs-lookup"><span data-stu-id="56848-204">updateTimeWindowUtcOffsetInMinutes</span></span>|<span data-ttu-id="56848-205">Int32</span><span class="sxs-lookup"><span data-stu-id="56848-205">Int32</span></span>|<span data-ttu-id="56848-206">指示每个更新时间窗口的 UTC 偏移的分钟数</span><span class="sxs-lookup"><span data-stu-id="56848-206">Minutes indicating UTC offset for each update time window</span></span>|



## <a name="response"></a><span data-ttu-id="56848-207">响应</span><span class="sxs-lookup"><span data-stu-id="56848-207">Response</span></span>
<span data-ttu-id="56848-208">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [macOSSoftwareUpdateConfiguration](../resources/intune-deviceconfig-macossoftwareupdateconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="56848-208">If successful, this method returns a `201 Created` response code and a [macOSSoftwareUpdateConfiguration](../resources/intune-deviceconfig-macossoftwareupdateconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="56848-209">示例</span><span class="sxs-lookup"><span data-stu-id="56848-209">Example</span></span>

### <a name="request"></a><span data-ttu-id="56848-210">请求</span><span class="sxs-lookup"><span data-stu-id="56848-210">Request</span></span>
<span data-ttu-id="56848-211">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="56848-211">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1542

{
  "@odata.type": "#microsoft.graph.macOSSoftwareUpdateConfiguration",
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
  "criticalUpdateBehavior": "default",
  "configDataUpdateBehavior": "default",
  "firmwareUpdateBehavior": "default",
  "allOtherUpdateBehavior": "default",
  "updateScheduleType": "updateDuringTimeWindows",
  "customUpdateTimeWindows": [
    {
      "@odata.type": "microsoft.graph.customUpdateTimeWindow",
      "startDay": "monday",
      "endDay": "monday",
      "startTime": "12:03:30.2730000",
      "endTime": "12:03:02.3740000"
    }
  ],
  "updateTimeWindowUtcOffsetInMinutes": 2
}
```

### <a name="response"></a><span data-ttu-id="56848-212">响应</span><span class="sxs-lookup"><span data-stu-id="56848-212">Response</span></span>
<span data-ttu-id="56848-p119">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="56848-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1714

{
  "@odata.type": "#microsoft.graph.macOSSoftwareUpdateConfiguration",
  "id": "b8e467ac-67ac-b8e4-ac67-e4b8ac67e4b8",
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
  "criticalUpdateBehavior": "default",
  "configDataUpdateBehavior": "default",
  "firmwareUpdateBehavior": "default",
  "allOtherUpdateBehavior": "default",
  "updateScheduleType": "updateDuringTimeWindows",
  "customUpdateTimeWindows": [
    {
      "@odata.type": "microsoft.graph.customUpdateTimeWindow",
      "startDay": "monday",
      "endDay": "monday",
      "startTime": "12:03:30.2730000",
      "endTime": "12:03:02.3740000"
    }
  ],
  "updateTimeWindowUtcOffsetInMinutes": 2
}
```




