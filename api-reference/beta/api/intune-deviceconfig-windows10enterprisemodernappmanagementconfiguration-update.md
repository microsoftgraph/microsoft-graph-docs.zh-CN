---
title: 更新 windows10EnterpriseModernAppManagementConfiguration
description: 更新 windows10EnterpriseModernAppManagementConfiguration 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8a815db83e86ad5a98a03aa45235621befe04d2b
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42739920"
---
# <a name="update-windows10enterprisemodernappmanagementconfiguration"></a><span data-ttu-id="03fcf-103">更新 windows10EnterpriseModernAppManagementConfiguration</span><span class="sxs-lookup"><span data-stu-id="03fcf-103">Update windows10EnterpriseModernAppManagementConfiguration</span></span>

> <span data-ttu-id="03fcf-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="03fcf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="03fcf-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="03fcf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="03fcf-106">更新 [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="03fcf-106">Update the properties of a [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="03fcf-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="03fcf-107">Prerequisites</span></span>
<span data-ttu-id="03fcf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="03fcf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03fcf-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="03fcf-110">Permission type</span></span>|<span data-ttu-id="03fcf-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="03fcf-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="03fcf-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="03fcf-112">Delegated (work or school account)</span></span>|<span data-ttu-id="03fcf-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03fcf-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="03fcf-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="03fcf-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="03fcf-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="03fcf-115">Not supported.</span></span>|
|<span data-ttu-id="03fcf-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="03fcf-116">Application</span></span>|<span data-ttu-id="03fcf-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03fcf-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="03fcf-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="03fcf-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="03fcf-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="03fcf-119">Request headers</span></span>
|<span data-ttu-id="03fcf-120">标头</span><span class="sxs-lookup"><span data-stu-id="03fcf-120">Header</span></span>|<span data-ttu-id="03fcf-121">值</span><span class="sxs-lookup"><span data-stu-id="03fcf-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="03fcf-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="03fcf-122">Authorization</span></span>|<span data-ttu-id="03fcf-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="03fcf-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="03fcf-124">接受</span><span class="sxs-lookup"><span data-stu-id="03fcf-124">Accept</span></span>|<span data-ttu-id="03fcf-125">application/json</span><span class="sxs-lookup"><span data-stu-id="03fcf-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="03fcf-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="03fcf-126">Request body</span></span>
<span data-ttu-id="03fcf-127">在请求正文中，提供 [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="03fcf-127">In the request body, supply a JSON representation for the [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) object.</span></span>

<span data-ttu-id="03fcf-128">下表显示创建 [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="03fcf-128">The following table shows the properties that are required when you create the [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md).</span></span>

|<span data-ttu-id="03fcf-129">属性</span><span class="sxs-lookup"><span data-stu-id="03fcf-129">Property</span></span>|<span data-ttu-id="03fcf-130">类型</span><span class="sxs-lookup"><span data-stu-id="03fcf-130">Type</span></span>|<span data-ttu-id="03fcf-131">说明</span><span class="sxs-lookup"><span data-stu-id="03fcf-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03fcf-132">id</span><span class="sxs-lookup"><span data-stu-id="03fcf-132">id</span></span>|<span data-ttu-id="03fcf-133">字符串</span><span class="sxs-lookup"><span data-stu-id="03fcf-133">String</span></span>|<span data-ttu-id="03fcf-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="03fcf-134">Key of the entity.</span></span> <span data-ttu-id="03fcf-135">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="03fcf-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03fcf-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="03fcf-136">lastModifiedDateTime</span></span>|<span data-ttu-id="03fcf-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03fcf-137">DateTimeOffset</span></span>|<span data-ttu-id="03fcf-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="03fcf-138">DateTime the object was last modified.</span></span> <span data-ttu-id="03fcf-139">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="03fcf-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03fcf-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="03fcf-140">roleScopeTagIds</span></span>|<span data-ttu-id="03fcf-141">String collection</span><span class="sxs-lookup"><span data-stu-id="03fcf-141">String collection</span></span>|<span data-ttu-id="03fcf-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="03fcf-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="03fcf-143">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="03fcf-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03fcf-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="03fcf-144">supportsScopeTags</span></span>|<span data-ttu-id="03fcf-145">布尔值</span><span class="sxs-lookup"><span data-stu-id="03fcf-145">Boolean</span></span>|<span data-ttu-id="03fcf-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="03fcf-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="03fcf-147">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="03fcf-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="03fcf-148">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="03fcf-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="03fcf-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="03fcf-149">This property is read-only.</span></span> <span data-ttu-id="03fcf-150">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="03fcf-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03fcf-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="03fcf-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="03fcf-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="03fcf-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="03fcf-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="03fcf-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="03fcf-154">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="03fcf-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03fcf-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="03fcf-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="03fcf-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="03fcf-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="03fcf-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="03fcf-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="03fcf-158">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="03fcf-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03fcf-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="03fcf-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="03fcf-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="03fcf-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="03fcf-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="03fcf-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="03fcf-162">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="03fcf-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03fcf-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="03fcf-163">createdDateTime</span></span>|<span data-ttu-id="03fcf-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03fcf-164">DateTimeOffset</span></span>|<span data-ttu-id="03fcf-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="03fcf-165">DateTime the object was created.</span></span> <span data-ttu-id="03fcf-166">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="03fcf-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03fcf-167">说明</span><span class="sxs-lookup"><span data-stu-id="03fcf-167">description</span></span>|<span data-ttu-id="03fcf-168">String</span><span class="sxs-lookup"><span data-stu-id="03fcf-168">String</span></span>|<span data-ttu-id="03fcf-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="03fcf-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="03fcf-170">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="03fcf-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03fcf-171">displayName</span><span class="sxs-lookup"><span data-stu-id="03fcf-171">displayName</span></span>|<span data-ttu-id="03fcf-172">String</span><span class="sxs-lookup"><span data-stu-id="03fcf-172">String</span></span>|<span data-ttu-id="03fcf-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="03fcf-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="03fcf-174">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="03fcf-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03fcf-175">version</span><span class="sxs-lookup"><span data-stu-id="03fcf-175">version</span></span>|<span data-ttu-id="03fcf-176">Int32</span><span class="sxs-lookup"><span data-stu-id="03fcf-176">Int32</span></span>|<span data-ttu-id="03fcf-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="03fcf-177">Version of the device configuration.</span></span> <span data-ttu-id="03fcf-178">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="03fcf-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03fcf-179">uninstallBuiltInApps</span><span class="sxs-lookup"><span data-stu-id="03fcf-179">uninstallBuiltInApps</span></span>|<span data-ttu-id="03fcf-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="03fcf-180">Boolean</span></span>|<span data-ttu-id="03fcf-181">指示是否卸载内置 Windows 应用的固定列表。</span><span class="sxs-lookup"><span data-stu-id="03fcf-181">Indicates whether or not to uninstall a fixed list of built-in Windows apps.</span></span>|



## <a name="response"></a><span data-ttu-id="03fcf-182">响应</span><span class="sxs-lookup"><span data-stu-id="03fcf-182">Response</span></span>
<span data-ttu-id="03fcf-183">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="03fcf-183">If successful, this method returns a `200 OK` response code and an updated [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03fcf-184">示例</span><span class="sxs-lookup"><span data-stu-id="03fcf-184">Example</span></span>

### <a name="request"></a><span data-ttu-id="03fcf-185">请求</span><span class="sxs-lookup"><span data-stu-id="03fcf-185">Request</span></span>
<span data-ttu-id="03fcf-186">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="03fcf-186">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1087

{
  "@odata.type": "#microsoft.graph.windows10EnterpriseModernAppManagementConfiguration",
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
  "uninstallBuiltInApps": true
}
```

### <a name="response"></a><span data-ttu-id="03fcf-187">响应</span><span class="sxs-lookup"><span data-stu-id="03fcf-187">Response</span></span>
<span data-ttu-id="03fcf-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="03fcf-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1259

{
  "@odata.type": "#microsoft.graph.windows10EnterpriseModernAppManagementConfiguration",
  "id": "d6577687-7687-d657-8776-57d6877657d6",
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
  "uninstallBuiltInApps": true
}
```




