---
title: 更新 unsupportedDeviceConfiguration
description: 更新 unsupportedDeviceConfiguration 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 12f69f531b5a388a008529722f4105c9af708232
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42741495"
---
# <a name="update-unsupporteddeviceconfiguration"></a><span data-ttu-id="e5b9e-103">更新 unsupportedDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="e5b9e-103">Update unsupportedDeviceConfiguration</span></span>

> <span data-ttu-id="e5b9e-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e5b9e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e5b9e-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e5b9e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5b9e-106">更新[unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e5b9e-106">Update the properties of a [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e5b9e-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="e5b9e-107">Prerequisites</span></span>
<span data-ttu-id="e5b9e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e5b9e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5b9e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e5b9e-110">Permission type</span></span>|<span data-ttu-id="e5b9e-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e5b9e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e5b9e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e5b9e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e5b9e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5b9e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e5b9e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e5b9e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e5b9e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e5b9e-115">Not supported.</span></span>|
|<span data-ttu-id="e5b9e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="e5b9e-116">Application</span></span>|<span data-ttu-id="e5b9e-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5b9e-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e5b9e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e5b9e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="e5b9e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="e5b9e-119">Request headers</span></span>
|<span data-ttu-id="e5b9e-120">标头</span><span class="sxs-lookup"><span data-stu-id="e5b9e-120">Header</span></span>|<span data-ttu-id="e5b9e-121">值</span><span class="sxs-lookup"><span data-stu-id="e5b9e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e5b9e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e5b9e-122">Authorization</span></span>|<span data-ttu-id="e5b9e-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e5b9e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e5b9e-124">接受</span><span class="sxs-lookup"><span data-stu-id="e5b9e-124">Accept</span></span>|<span data-ttu-id="e5b9e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e5b9e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e5b9e-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="e5b9e-126">Request body</span></span>
<span data-ttu-id="e5b9e-127">在请求正文中，提供[unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e5b9e-127">In the request body, supply a JSON representation for the [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) object.</span></span>

<span data-ttu-id="e5b9e-128">下表显示创建[unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e5b9e-128">The following table shows the properties that are required when you create the [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md).</span></span>

|<span data-ttu-id="e5b9e-129">属性</span><span class="sxs-lookup"><span data-stu-id="e5b9e-129">Property</span></span>|<span data-ttu-id="e5b9e-130">类型</span><span class="sxs-lookup"><span data-stu-id="e5b9e-130">Type</span></span>|<span data-ttu-id="e5b9e-131">说明</span><span class="sxs-lookup"><span data-stu-id="e5b9e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5b9e-132">id</span><span class="sxs-lookup"><span data-stu-id="e5b9e-132">id</span></span>|<span data-ttu-id="e5b9e-133">字符串</span><span class="sxs-lookup"><span data-stu-id="e5b9e-133">String</span></span>|<span data-ttu-id="e5b9e-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e5b9e-134">Key of the entity.</span></span> <span data-ttu-id="e5b9e-135">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e5b9e-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e5b9e-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e5b9e-136">lastModifiedDateTime</span></span>|<span data-ttu-id="e5b9e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e5b9e-137">DateTimeOffset</span></span>|<span data-ttu-id="e5b9e-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="e5b9e-138">DateTime the object was last modified.</span></span> <span data-ttu-id="e5b9e-139">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e5b9e-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e5b9e-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e5b9e-140">roleScopeTagIds</span></span>|<span data-ttu-id="e5b9e-141">String collection</span><span class="sxs-lookup"><span data-stu-id="e5b9e-141">String collection</span></span>|<span data-ttu-id="e5b9e-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="e5b9e-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e5b9e-143">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e5b9e-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e5b9e-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="e5b9e-144">supportsScopeTags</span></span>|<span data-ttu-id="e5b9e-145">布尔值</span><span class="sxs-lookup"><span data-stu-id="e5b9e-145">Boolean</span></span>|<span data-ttu-id="e5b9e-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="e5b9e-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="e5b9e-147">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="e5b9e-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="e5b9e-148">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="e5b9e-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="e5b9e-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="e5b9e-149">This property is read-only.</span></span> <span data-ttu-id="e5b9e-150">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e5b9e-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e5b9e-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="e5b9e-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="e5b9e-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="e5b9e-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="e5b9e-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="e5b9e-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="e5b9e-154">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e5b9e-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e5b9e-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="e5b9e-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="e5b9e-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="e5b9e-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="e5b9e-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="e5b9e-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="e5b9e-158">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e5b9e-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e5b9e-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="e5b9e-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="e5b9e-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="e5b9e-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="e5b9e-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="e5b9e-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="e5b9e-162">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e5b9e-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e5b9e-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e5b9e-163">createdDateTime</span></span>|<span data-ttu-id="e5b9e-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e5b9e-164">DateTimeOffset</span></span>|<span data-ttu-id="e5b9e-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="e5b9e-165">DateTime the object was created.</span></span> <span data-ttu-id="e5b9e-166">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e5b9e-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e5b9e-167">说明</span><span class="sxs-lookup"><span data-stu-id="e5b9e-167">description</span></span>|<span data-ttu-id="e5b9e-168">String</span><span class="sxs-lookup"><span data-stu-id="e5b9e-168">String</span></span>|<span data-ttu-id="e5b9e-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="e5b9e-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e5b9e-170">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e5b9e-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e5b9e-171">displayName</span><span class="sxs-lookup"><span data-stu-id="e5b9e-171">displayName</span></span>|<span data-ttu-id="e5b9e-172">String</span><span class="sxs-lookup"><span data-stu-id="e5b9e-172">String</span></span>|<span data-ttu-id="e5b9e-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="e5b9e-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e5b9e-174">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e5b9e-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e5b9e-175">version</span><span class="sxs-lookup"><span data-stu-id="e5b9e-175">version</span></span>|<span data-ttu-id="e5b9e-176">Int32</span><span class="sxs-lookup"><span data-stu-id="e5b9e-176">Int32</span></span>|<span data-ttu-id="e5b9e-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="e5b9e-177">Version of the device configuration.</span></span> <span data-ttu-id="e5b9e-178">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e5b9e-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e5b9e-179">originalEntityTypeName</span><span class="sxs-lookup"><span data-stu-id="e5b9e-179">originalEntityTypeName</span></span>|<span data-ttu-id="e5b9e-180">String</span><span class="sxs-lookup"><span data-stu-id="e5b9e-180">String</span></span>|<span data-ttu-id="e5b9e-181">将以其他方式返回的实体的类型。</span><span class="sxs-lookup"><span data-stu-id="e5b9e-181">The type of entity that would be returned otherwise.</span></span>|
|<span data-ttu-id="e5b9e-182">详细信息</span><span class="sxs-lookup"><span data-stu-id="e5b9e-182">details</span></span>|<span data-ttu-id="e5b9e-183">[unsupportedDeviceConfigurationDetail](../resources/intune-deviceconfig-unsupporteddeviceconfigurationdetail.md)集合</span><span class="sxs-lookup"><span data-stu-id="e5b9e-183">[unsupportedDeviceConfigurationDetail](../resources/intune-deviceconfig-unsupporteddeviceconfigurationdetail.md) collection</span></span>|<span data-ttu-id="e5b9e-184">描述实体不受支持的原因的详细信息。</span><span class="sxs-lookup"><span data-stu-id="e5b9e-184">Details describing why the entity is unsupported.</span></span> <span data-ttu-id="e5b9e-185">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="e5b9e-185">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="e5b9e-186">响应</span><span class="sxs-lookup"><span data-stu-id="e5b9e-186">Response</span></span>
<span data-ttu-id="e5b9e-187">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e5b9e-187">If successful, this method returns a `200 OK` response code and an updated [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5b9e-188">示例</span><span class="sxs-lookup"><span data-stu-id="e5b9e-188">Example</span></span>

### <a name="request"></a><span data-ttu-id="e5b9e-189">请求</span><span class="sxs-lookup"><span data-stu-id="e5b9e-189">Request</span></span>
<span data-ttu-id="e5b9e-190">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e5b9e-190">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1291

{
  "@odata.type": "#microsoft.graph.unsupportedDeviceConfiguration",
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
  "originalEntityTypeName": "Original Entity Type Name value",
  "details": [
    {
      "@odata.type": "microsoft.graph.unsupportedDeviceConfigurationDetail",
      "message": "Message value",
      "propertyName": "Property Name value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="e5b9e-191">响应</span><span class="sxs-lookup"><span data-stu-id="e5b9e-191">Response</span></span>
<span data-ttu-id="e5b9e-p114">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e5b9e-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1463

{
  "@odata.type": "#microsoft.graph.unsupportedDeviceConfiguration",
  "id": "f80d6fc8-6fc8-f80d-c86f-0df8c86f0df8",
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
  "originalEntityTypeName": "Original Entity Type Name value",
  "details": [
    {
      "@odata.type": "microsoft.graph.unsupportedDeviceConfigurationDetail",
      "message": "Message value",
      "propertyName": "Property Name value"
    }
  ]
}
```




