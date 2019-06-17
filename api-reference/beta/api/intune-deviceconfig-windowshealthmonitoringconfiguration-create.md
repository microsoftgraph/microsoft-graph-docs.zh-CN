---
title: 创建 windowsHealthMonitoringConfiguration
description: 创建新的 windowsHealthMonitoringConfiguration 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 63146c8bf18452a7d41b2beb3b1de83db9d526c0
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34961978"
---
# <a name="create-windowshealthmonitoringconfiguration"></a><span data-ttu-id="a1f13-103">创建 windowsHealthMonitoringConfiguration</span><span class="sxs-lookup"><span data-stu-id="a1f13-103">Create windowsHealthMonitoringConfiguration</span></span>

> <span data-ttu-id="a1f13-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a1f13-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a1f13-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a1f13-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1f13-106">创建新的[windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a1f13-106">Create a new [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a1f13-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="a1f13-107">Prerequisites</span></span>
<span data-ttu-id="a1f13-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a1f13-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1f13-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a1f13-110">Permission type</span></span>|<span data-ttu-id="a1f13-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a1f13-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1f13-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a1f13-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a1f13-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1f13-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a1f13-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a1f13-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1f13-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a1f13-115">Not supported.</span></span>|
|<span data-ttu-id="a1f13-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a1f13-116">Application</span></span>|<span data-ttu-id="a1f13-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="a1f13-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1f13-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a1f13-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a1f13-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a1f13-119">Request headers</span></span>
|<span data-ttu-id="a1f13-120">标头</span><span class="sxs-lookup"><span data-stu-id="a1f13-120">Header</span></span>|<span data-ttu-id="a1f13-121">值</span><span class="sxs-lookup"><span data-stu-id="a1f13-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a1f13-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a1f13-122">Authorization</span></span>|<span data-ttu-id="a1f13-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a1f13-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a1f13-124">接受</span><span class="sxs-lookup"><span data-stu-id="a1f13-124">Accept</span></span>|<span data-ttu-id="a1f13-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a1f13-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1f13-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a1f13-126">Request body</span></span>
<span data-ttu-id="a1f13-127">在请求正文中, 提供 windowsHealthMonitoringConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a1f13-127">In the request body, supply a JSON representation for the windowsHealthMonitoringConfiguration object.</span></span>

<span data-ttu-id="a1f13-128">下表显示创建 windowsHealthMonitoringConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a1f13-128">The following table shows the properties that are required when you create the windowsHealthMonitoringConfiguration.</span></span>

|<span data-ttu-id="a1f13-129">属性</span><span class="sxs-lookup"><span data-stu-id="a1f13-129">Property</span></span>|<span data-ttu-id="a1f13-130">类型</span><span class="sxs-lookup"><span data-stu-id="a1f13-130">Type</span></span>|<span data-ttu-id="a1f13-131">说明</span><span class="sxs-lookup"><span data-stu-id="a1f13-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1f13-132">id</span><span class="sxs-lookup"><span data-stu-id="a1f13-132">id</span></span>|<span data-ttu-id="a1f13-133">字符串</span><span class="sxs-lookup"><span data-stu-id="a1f13-133">String</span></span>|<span data-ttu-id="a1f13-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a1f13-134">Key of the entity.</span></span> <span data-ttu-id="a1f13-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a1f13-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a1f13-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a1f13-136">lastModifiedDateTime</span></span>|<span data-ttu-id="a1f13-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1f13-137">DateTimeOffset</span></span>|<span data-ttu-id="a1f13-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="a1f13-138">DateTime the object was last modified.</span></span> <span data-ttu-id="a1f13-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a1f13-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a1f13-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a1f13-140">roleScopeTagIds</span></span>|<span data-ttu-id="a1f13-141">String collection</span><span class="sxs-lookup"><span data-stu-id="a1f13-141">String collection</span></span>|<span data-ttu-id="a1f13-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="a1f13-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a1f13-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a1f13-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a1f13-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a1f13-144">supportsScopeTags</span></span>|<span data-ttu-id="a1f13-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="a1f13-145">Boolean</span></span>|<span data-ttu-id="a1f13-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="a1f13-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a1f13-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="a1f13-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a1f13-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="a1f13-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a1f13-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="a1f13-149">This property is read-only.</span></span> <span data-ttu-id="a1f13-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a1f13-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a1f13-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a1f13-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="a1f13-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a1f13-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="a1f13-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="a1f13-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="a1f13-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a1f13-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a1f13-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a1f13-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="a1f13-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a1f13-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="a1f13-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="a1f13-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="a1f13-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a1f13-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a1f13-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a1f13-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="a1f13-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a1f13-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="a1f13-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="a1f13-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="a1f13-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a1f13-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a1f13-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a1f13-163">createdDateTime</span></span>|<span data-ttu-id="a1f13-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1f13-164">DateTimeOffset</span></span>|<span data-ttu-id="a1f13-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="a1f13-165">DateTime the object was created.</span></span> <span data-ttu-id="a1f13-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a1f13-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a1f13-167">说明</span><span class="sxs-lookup"><span data-stu-id="a1f13-167">description</span></span>|<span data-ttu-id="a1f13-168">String</span><span class="sxs-lookup"><span data-stu-id="a1f13-168">String</span></span>|<span data-ttu-id="a1f13-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="a1f13-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a1f13-170">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a1f13-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a1f13-171">displayName</span><span class="sxs-lookup"><span data-stu-id="a1f13-171">displayName</span></span>|<span data-ttu-id="a1f13-172">String</span><span class="sxs-lookup"><span data-stu-id="a1f13-172">String</span></span>|<span data-ttu-id="a1f13-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="a1f13-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a1f13-174">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a1f13-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a1f13-175">version</span><span class="sxs-lookup"><span data-stu-id="a1f13-175">version</span></span>|<span data-ttu-id="a1f13-176">Int32</span><span class="sxs-lookup"><span data-stu-id="a1f13-176">Int32</span></span>|<span data-ttu-id="a1f13-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="a1f13-177">Version of the device configuration.</span></span> <span data-ttu-id="a1f13-178">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a1f13-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a1f13-179">allowDeviceHealthMonitoring</span><span class="sxs-lookup"><span data-stu-id="a1f13-179">allowDeviceHealthMonitoring</span></span>|[<span data-ttu-id="a1f13-180">启用</span><span class="sxs-lookup"><span data-stu-id="a1f13-180">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="a1f13-181">在设备上启用设备运行状况监视。</span><span class="sxs-lookup"><span data-stu-id="a1f13-181">Enables device health monitoring on the device.</span></span> <span data-ttu-id="a1f13-182">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="a1f13-182">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="a1f13-183">configDeviceHealthMonitoringScope</span><span class="sxs-lookup"><span data-stu-id="a1f13-183">configDeviceHealthMonitoringScope</span></span>|[<span data-ttu-id="a1f13-184">windowsHealthMonitoringScope</span><span class="sxs-lookup"><span data-stu-id="a1f13-184">windowsHealthMonitoringScope</span></span>](../resources/intune-deviceconfig-windowshealthmonitoringscope.md)|<span data-ttu-id="a1f13-185">指定从启用运行状况监视的设备收集的一组事件。</span><span class="sxs-lookup"><span data-stu-id="a1f13-185">Specifies set of events collected from the device where health monitoring is enabled.</span></span> <span data-ttu-id="a1f13-186">可取值为：`undefined`、`healthMonitoring`、`bootPerformance`。</span><span class="sxs-lookup"><span data-stu-id="a1f13-186">Possible values are: `undefined`, `healthMonitoring`, `bootPerformance`.</span></span>|
|<span data-ttu-id="a1f13-187">configDeviceHealthMonitoringCustomScope</span><span class="sxs-lookup"><span data-stu-id="a1f13-187">configDeviceHealthMonitoringCustomScope</span></span>|<span data-ttu-id="a1f13-188">String</span><span class="sxs-lookup"><span data-stu-id="a1f13-188">String</span></span>|<span data-ttu-id="a1f13-189">指定从启用运行状况监视的设备收集的自定义事件集</span><span class="sxs-lookup"><span data-stu-id="a1f13-189">Specifies custom set of events collected from the device where health monitoring is enabled</span></span>|



## <a name="response"></a><span data-ttu-id="a1f13-190">响应</span><span class="sxs-lookup"><span data-stu-id="a1f13-190">Response</span></span>
<span data-ttu-id="a1f13-191">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a1f13-191">If successful, this method returns a `201 Created` response code and a [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1f13-192">示例</span><span class="sxs-lookup"><span data-stu-id="a1f13-192">Example</span></span>

### <a name="request"></a><span data-ttu-id="a1f13-193">请求</span><span class="sxs-lookup"><span data-stu-id="a1f13-193">Request</span></span>
<span data-ttu-id="a1f13-194">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a1f13-194">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a1f13-195">响应</span><span class="sxs-lookup"><span data-stu-id="a1f13-195">Response</span></span>
<span data-ttu-id="a1f13-p115">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a1f13-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





