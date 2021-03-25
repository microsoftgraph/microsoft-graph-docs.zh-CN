---
title: 创建 windowsHealthMonitoringConfiguration
description: 创建新的 windowsHealthMonitoringConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d840f3a25d4fa8621a945a497030fbcdcf3d3b7d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51154910"
---
# <a name="create-windowshealthmonitoringconfiguration"></a><span data-ttu-id="dfffc-103">创建 windowsHealthMonitoringConfiguration</span><span class="sxs-lookup"><span data-stu-id="dfffc-103">Create windowsHealthMonitoringConfiguration</span></span>

<span data-ttu-id="dfffc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dfffc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dfffc-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="dfffc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dfffc-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="dfffc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dfffc-107">创建新的 [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="dfffc-107">Create a new [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dfffc-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="dfffc-108">Prerequisites</span></span>
<span data-ttu-id="dfffc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dfffc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dfffc-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="dfffc-111">Permission type</span></span>|<span data-ttu-id="dfffc-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dfffc-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dfffc-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dfffc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dfffc-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dfffc-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dfffc-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dfffc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dfffc-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="dfffc-116">Not supported.</span></span>|
|<span data-ttu-id="dfffc-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="dfffc-117">Application</span></span>|<span data-ttu-id="dfffc-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dfffc-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dfffc-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dfffc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="dfffc-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="dfffc-120">Request headers</span></span>
|<span data-ttu-id="dfffc-121">标头</span><span class="sxs-lookup"><span data-stu-id="dfffc-121">Header</span></span>|<span data-ttu-id="dfffc-122">值</span><span class="sxs-lookup"><span data-stu-id="dfffc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dfffc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="dfffc-123">Authorization</span></span>|<span data-ttu-id="dfffc-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="dfffc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dfffc-125">接受</span><span class="sxs-lookup"><span data-stu-id="dfffc-125">Accept</span></span>|<span data-ttu-id="dfffc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dfffc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dfffc-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="dfffc-127">Request body</span></span>
<span data-ttu-id="dfffc-128">在请求正文中，提供 windowsHealthMonitoringConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dfffc-128">In the request body, supply a JSON representation for the windowsHealthMonitoringConfiguration object.</span></span>

<span data-ttu-id="dfffc-129">下表显示创建 windowsHealthMonitoringConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="dfffc-129">The following table shows the properties that are required when you create the windowsHealthMonitoringConfiguration.</span></span>

|<span data-ttu-id="dfffc-130">属性</span><span class="sxs-lookup"><span data-stu-id="dfffc-130">Property</span></span>|<span data-ttu-id="dfffc-131">类型</span><span class="sxs-lookup"><span data-stu-id="dfffc-131">Type</span></span>|<span data-ttu-id="dfffc-132">说明</span><span class="sxs-lookup"><span data-stu-id="dfffc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dfffc-133">id</span><span class="sxs-lookup"><span data-stu-id="dfffc-133">id</span></span>|<span data-ttu-id="dfffc-134">String</span><span class="sxs-lookup"><span data-stu-id="dfffc-134">String</span></span>|<span data-ttu-id="dfffc-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="dfffc-135">Key of the entity.</span></span> <span data-ttu-id="dfffc-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dfffc-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dfffc-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dfffc-137">lastModifiedDateTime</span></span>|<span data-ttu-id="dfffc-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dfffc-138">DateTimeOffset</span></span>|<span data-ttu-id="dfffc-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="dfffc-139">DateTime the object was last modified.</span></span> <span data-ttu-id="dfffc-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dfffc-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dfffc-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="dfffc-141">roleScopeTagIds</span></span>|<span data-ttu-id="dfffc-142">String collection</span><span class="sxs-lookup"><span data-stu-id="dfffc-142">String collection</span></span>|<span data-ttu-id="dfffc-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="dfffc-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="dfffc-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dfffc-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dfffc-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="dfffc-145">supportsScopeTags</span></span>|<span data-ttu-id="dfffc-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="dfffc-146">Boolean</span></span>|<span data-ttu-id="dfffc-147">指示基础设备配置是否支持分配范围标记。</span><span class="sxs-lookup"><span data-stu-id="dfffc-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="dfffc-148">当此值为 false 且实体对作用域用户不可见时，不允许分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="dfffc-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="dfffc-149">这适用于在 Silverlight 中创建的旧版策略，可通过在 Azure 门户中删除和重新创建策略来解决。</span><span class="sxs-lookup"><span data-stu-id="dfffc-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="dfffc-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="dfffc-150">This property is read-only.</span></span> <span data-ttu-id="dfffc-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dfffc-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dfffc-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="dfffc-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="dfffc-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="dfffc-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="dfffc-154">此策略的操作系统版本适用性。</span><span class="sxs-lookup"><span data-stu-id="dfffc-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="dfffc-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dfffc-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dfffc-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="dfffc-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="dfffc-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="dfffc-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="dfffc-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="dfffc-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="dfffc-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dfffc-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dfffc-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="dfffc-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="dfffc-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="dfffc-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="dfffc-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="dfffc-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="dfffc-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dfffc-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dfffc-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dfffc-164">createdDateTime</span></span>|<span data-ttu-id="dfffc-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dfffc-165">DateTimeOffset</span></span>|<span data-ttu-id="dfffc-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="dfffc-166">DateTime the object was created.</span></span> <span data-ttu-id="dfffc-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dfffc-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dfffc-168">说明</span><span class="sxs-lookup"><span data-stu-id="dfffc-168">description</span></span>|<span data-ttu-id="dfffc-169">String</span><span class="sxs-lookup"><span data-stu-id="dfffc-169">String</span></span>|<span data-ttu-id="dfffc-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="dfffc-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="dfffc-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dfffc-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dfffc-172">displayName</span><span class="sxs-lookup"><span data-stu-id="dfffc-172">displayName</span></span>|<span data-ttu-id="dfffc-173">String</span><span class="sxs-lookup"><span data-stu-id="dfffc-173">String</span></span>|<span data-ttu-id="dfffc-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="dfffc-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="dfffc-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dfffc-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dfffc-176">version</span><span class="sxs-lookup"><span data-stu-id="dfffc-176">version</span></span>|<span data-ttu-id="dfffc-177">Int32</span><span class="sxs-lookup"><span data-stu-id="dfffc-177">Int32</span></span>|<span data-ttu-id="dfffc-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="dfffc-178">Version of the device configuration.</span></span> <span data-ttu-id="dfffc-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dfffc-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dfffc-180">allowDeviceHealthMonitoring</span><span class="sxs-lookup"><span data-stu-id="dfffc-180">allowDeviceHealthMonitoring</span></span>|[<span data-ttu-id="dfffc-181">enablement</span><span class="sxs-lookup"><span data-stu-id="dfffc-181">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="dfffc-182">在设备上启用设备运行状况监视。</span><span class="sxs-lookup"><span data-stu-id="dfffc-182">Enables device health monitoring on the device.</span></span> <span data-ttu-id="dfffc-183">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="dfffc-183">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="dfffc-184">configDeviceHealthMonitoringScope</span><span class="sxs-lookup"><span data-stu-id="dfffc-184">configDeviceHealthMonitoringScope</span></span>|[<span data-ttu-id="dfffc-185">windowsHealthMonitoringScope</span><span class="sxs-lookup"><span data-stu-id="dfffc-185">windowsHealthMonitoringScope</span></span>](../resources/intune-deviceconfig-windowshealthmonitoringscope.md)|<span data-ttu-id="dfffc-186">指定从启用了运行状况监视的设备收集的事件集。</span><span class="sxs-lookup"><span data-stu-id="dfffc-186">Specifies set of events collected from the device where health monitoring is enabled.</span></span> <span data-ttu-id="dfffc-187">可取值为：`undefined`、`healthMonitoring`、`bootPerformance`、`windowsUpdates`。</span><span class="sxs-lookup"><span data-stu-id="dfffc-187">Possible values are: `undefined`, `healthMonitoring`, `bootPerformance`, `windowsUpdates`.</span></span>|
|<span data-ttu-id="dfffc-188">configDeviceHealthMonitoringCustomScope</span><span class="sxs-lookup"><span data-stu-id="dfffc-188">configDeviceHealthMonitoringCustomScope</span></span>|<span data-ttu-id="dfffc-189">String</span><span class="sxs-lookup"><span data-stu-id="dfffc-189">String</span></span>|<span data-ttu-id="dfffc-190">指定从启用了运行状况监视的设备收集的自定义事件集</span><span class="sxs-lookup"><span data-stu-id="dfffc-190">Specifies custom set of events collected from the device where health monitoring is enabled</span></span>|



## <a name="response"></a><span data-ttu-id="dfffc-191">响应</span><span class="sxs-lookup"><span data-stu-id="dfffc-191">Response</span></span>
<span data-ttu-id="dfffc-192">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="dfffc-192">If successful, this method returns a `201 Created` response code and a [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dfffc-193">示例</span><span class="sxs-lookup"><span data-stu-id="dfffc-193">Example</span></span>

### <a name="request"></a><span data-ttu-id="dfffc-194">请求</span><span class="sxs-lookup"><span data-stu-id="dfffc-194">Request</span></span>
<span data-ttu-id="dfffc-195">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="dfffc-195">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1244

{
  "@odata.type": "#microsoft.graph.windowsHealthMonitoringConfiguration",
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
  "allowDeviceHealthMonitoring": "enabled",
  "configDeviceHealthMonitoringScope": "healthMonitoring",
  "configDeviceHealthMonitoringCustomScope": "Config Device Health Monitoring Custom Scope value"
}
```

### <a name="response"></a><span data-ttu-id="dfffc-196">响应</span><span class="sxs-lookup"><span data-stu-id="dfffc-196">Response</span></span>
<span data-ttu-id="dfffc-p115">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="dfffc-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1416

{
  "@odata.type": "#microsoft.graph.windowsHealthMonitoringConfiguration",
  "id": "3439bcec-bcec-3439-ecbc-3934ecbc3934",
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
  "allowDeviceHealthMonitoring": "enabled",
  "configDeviceHealthMonitoringScope": "healthMonitoring",
  "configDeviceHealthMonitoringCustomScope": "Config Device Health Monitoring Custom Scope value"
}
```




