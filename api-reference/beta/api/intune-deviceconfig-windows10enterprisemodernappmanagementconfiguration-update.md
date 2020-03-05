---
title: 更新 windows10EnterpriseModernAppManagementConfiguration
description: 更新 windows10EnterpriseModernAppManagementConfiguration 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6a7762896d0d61f99c942037a9d38807e2b0a6d6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42479980"
---
# <a name="update-windows10enterprisemodernappmanagementconfiguration"></a><span data-ttu-id="3088d-103">更新 windows10EnterpriseModernAppManagementConfiguration</span><span class="sxs-lookup"><span data-stu-id="3088d-103">Update windows10EnterpriseModernAppManagementConfiguration</span></span>

<span data-ttu-id="3088d-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="3088d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3088d-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3088d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3088d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3088d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3088d-107">更新 [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="3088d-107">Update the properties of a [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3088d-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="3088d-108">Prerequisites</span></span>
<span data-ttu-id="3088d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3088d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3088d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="3088d-111">Permission type</span></span>|<span data-ttu-id="3088d-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3088d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3088d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3088d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3088d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3088d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3088d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3088d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3088d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3088d-116">Not supported.</span></span>|
|<span data-ttu-id="3088d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="3088d-117">Application</span></span>|<span data-ttu-id="3088d-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3088d-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3088d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3088d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="3088d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="3088d-120">Request headers</span></span>
|<span data-ttu-id="3088d-121">标头</span><span class="sxs-lookup"><span data-stu-id="3088d-121">Header</span></span>|<span data-ttu-id="3088d-122">值</span><span class="sxs-lookup"><span data-stu-id="3088d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3088d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3088d-123">Authorization</span></span>|<span data-ttu-id="3088d-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3088d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3088d-125">接受</span><span class="sxs-lookup"><span data-stu-id="3088d-125">Accept</span></span>|<span data-ttu-id="3088d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3088d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3088d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3088d-127">Request body</span></span>
<span data-ttu-id="3088d-128">在请求正文中，提供 [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3088d-128">In the request body, supply a JSON representation for the [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) object.</span></span>

<span data-ttu-id="3088d-129">下表显示创建 [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3088d-129">The following table shows the properties that are required when you create the [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md).</span></span>

|<span data-ttu-id="3088d-130">属性</span><span class="sxs-lookup"><span data-stu-id="3088d-130">Property</span></span>|<span data-ttu-id="3088d-131">类型</span><span class="sxs-lookup"><span data-stu-id="3088d-131">Type</span></span>|<span data-ttu-id="3088d-132">说明</span><span class="sxs-lookup"><span data-stu-id="3088d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3088d-133">id</span><span class="sxs-lookup"><span data-stu-id="3088d-133">id</span></span>|<span data-ttu-id="3088d-134">字符串</span><span class="sxs-lookup"><span data-stu-id="3088d-134">String</span></span>|<span data-ttu-id="3088d-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="3088d-135">Key of the entity.</span></span> <span data-ttu-id="3088d-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3088d-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3088d-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3088d-137">lastModifiedDateTime</span></span>|<span data-ttu-id="3088d-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3088d-138">DateTimeOffset</span></span>|<span data-ttu-id="3088d-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="3088d-139">DateTime the object was last modified.</span></span> <span data-ttu-id="3088d-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3088d-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3088d-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3088d-141">roleScopeTagIds</span></span>|<span data-ttu-id="3088d-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="3088d-142">String collection</span></span>|<span data-ttu-id="3088d-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="3088d-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="3088d-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3088d-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3088d-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="3088d-145">supportsScopeTags</span></span>|<span data-ttu-id="3088d-146">布尔</span><span class="sxs-lookup"><span data-stu-id="3088d-146">Boolean</span></span>|<span data-ttu-id="3088d-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="3088d-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="3088d-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="3088d-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="3088d-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="3088d-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="3088d-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="3088d-150">This property is read-only.</span></span> <span data-ttu-id="3088d-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3088d-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3088d-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="3088d-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="3088d-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="3088d-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="3088d-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="3088d-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="3088d-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3088d-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3088d-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="3088d-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="3088d-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="3088d-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="3088d-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="3088d-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="3088d-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3088d-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3088d-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="3088d-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="3088d-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="3088d-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="3088d-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="3088d-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="3088d-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3088d-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3088d-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3088d-164">createdDateTime</span></span>|<span data-ttu-id="3088d-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3088d-165">DateTimeOffset</span></span>|<span data-ttu-id="3088d-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="3088d-166">DateTime the object was created.</span></span> <span data-ttu-id="3088d-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3088d-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3088d-168">说明</span><span class="sxs-lookup"><span data-stu-id="3088d-168">description</span></span>|<span data-ttu-id="3088d-169">String</span><span class="sxs-lookup"><span data-stu-id="3088d-169">String</span></span>|<span data-ttu-id="3088d-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="3088d-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3088d-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3088d-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3088d-172">displayName</span><span class="sxs-lookup"><span data-stu-id="3088d-172">displayName</span></span>|<span data-ttu-id="3088d-173">String</span><span class="sxs-lookup"><span data-stu-id="3088d-173">String</span></span>|<span data-ttu-id="3088d-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="3088d-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3088d-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3088d-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3088d-176">version</span><span class="sxs-lookup"><span data-stu-id="3088d-176">version</span></span>|<span data-ttu-id="3088d-177">Int32</span><span class="sxs-lookup"><span data-stu-id="3088d-177">Int32</span></span>|<span data-ttu-id="3088d-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="3088d-178">Version of the device configuration.</span></span> <span data-ttu-id="3088d-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3088d-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3088d-180">uninstallBuiltInApps</span><span class="sxs-lookup"><span data-stu-id="3088d-180">uninstallBuiltInApps</span></span>|<span data-ttu-id="3088d-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="3088d-181">Boolean</span></span>|<span data-ttu-id="3088d-182">指示是否卸载内置 Windows 应用的固定列表。</span><span class="sxs-lookup"><span data-stu-id="3088d-182">Indicates whether or not to uninstall a fixed list of built-in Windows apps.</span></span>|



## <a name="response"></a><span data-ttu-id="3088d-183">响应</span><span class="sxs-lookup"><span data-stu-id="3088d-183">Response</span></span>
<span data-ttu-id="3088d-184">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3088d-184">If successful, this method returns a `200 OK` response code and an updated [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3088d-185">示例</span><span class="sxs-lookup"><span data-stu-id="3088d-185">Example</span></span>

### <a name="request"></a><span data-ttu-id="3088d-186">请求</span><span class="sxs-lookup"><span data-stu-id="3088d-186">Request</span></span>
<span data-ttu-id="3088d-187">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3088d-187">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3088d-188">响应</span><span class="sxs-lookup"><span data-stu-id="3088d-188">Response</span></span>
<span data-ttu-id="3088d-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3088d-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





