---
title: 创建 windows10EnterpriseModernAppManagementConfiguration
description: 创建新的 windows10EnterpriseModernAppManagementConfiguration 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d02be4307980c806701b8c7d2e6cdad7d7d0ed3f
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37182741"
---
# <a name="create-windows10enterprisemodernappmanagementconfiguration"></a><span data-ttu-id="be32f-103">创建 windows10EnterpriseModernAppManagementConfiguration</span><span class="sxs-lookup"><span data-stu-id="be32f-103">Create windows10EnterpriseModernAppManagementConfiguration</span></span>

> <span data-ttu-id="be32f-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="be32f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="be32f-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="be32f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="be32f-106">创建新的 [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="be32f-106">Create a new [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="be32f-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="be32f-107">Prerequisites</span></span>
<span data-ttu-id="be32f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="be32f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be32f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="be32f-110">Permission type</span></span>|<span data-ttu-id="be32f-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="be32f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="be32f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="be32f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="be32f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be32f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="be32f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="be32f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="be32f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="be32f-115">Not supported.</span></span>|
|<span data-ttu-id="be32f-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="be32f-116">Application</span></span>|<span data-ttu-id="be32f-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be32f-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="be32f-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="be32f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="be32f-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="be32f-119">Request headers</span></span>
|<span data-ttu-id="be32f-120">标头</span><span class="sxs-lookup"><span data-stu-id="be32f-120">Header</span></span>|<span data-ttu-id="be32f-121">值</span><span class="sxs-lookup"><span data-stu-id="be32f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="be32f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="be32f-122">Authorization</span></span>|<span data-ttu-id="be32f-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="be32f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="be32f-124">接受</span><span class="sxs-lookup"><span data-stu-id="be32f-124">Accept</span></span>|<span data-ttu-id="be32f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="be32f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="be32f-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="be32f-126">Request body</span></span>
<span data-ttu-id="be32f-127">在请求正文中，提供 windows10EnterpriseModernAppManagementConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="be32f-127">In the request body, supply a JSON representation for the windows10EnterpriseModernAppManagementConfiguration object.</span></span>

<span data-ttu-id="be32f-128">下表显示创建 windows10EnterpriseModernAppManagementConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="be32f-128">The following table shows the properties that are required when you create the windows10EnterpriseModernAppManagementConfiguration.</span></span>

|<span data-ttu-id="be32f-129">属性</span><span class="sxs-lookup"><span data-stu-id="be32f-129">Property</span></span>|<span data-ttu-id="be32f-130">类型</span><span class="sxs-lookup"><span data-stu-id="be32f-130">Type</span></span>|<span data-ttu-id="be32f-131">说明</span><span class="sxs-lookup"><span data-stu-id="be32f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be32f-132">id</span><span class="sxs-lookup"><span data-stu-id="be32f-132">id</span></span>|<span data-ttu-id="be32f-133">字符串</span><span class="sxs-lookup"><span data-stu-id="be32f-133">String</span></span>|<span data-ttu-id="be32f-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="be32f-134">Key of the entity.</span></span> <span data-ttu-id="be32f-135">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="be32f-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="be32f-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="be32f-136">lastModifiedDateTime</span></span>|<span data-ttu-id="be32f-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be32f-137">DateTimeOffset</span></span>|<span data-ttu-id="be32f-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="be32f-138">DateTime the object was last modified.</span></span> <span data-ttu-id="be32f-139">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="be32f-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="be32f-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="be32f-140">roleScopeTagIds</span></span>|<span data-ttu-id="be32f-141">String collection</span><span class="sxs-lookup"><span data-stu-id="be32f-141">String collection</span></span>|<span data-ttu-id="be32f-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="be32f-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="be32f-143">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="be32f-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="be32f-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="be32f-144">supportsScopeTags</span></span>|<span data-ttu-id="be32f-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="be32f-145">Boolean</span></span>|<span data-ttu-id="be32f-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="be32f-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="be32f-147">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="be32f-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="be32f-148">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="be32f-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="be32f-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="be32f-149">This property is read-only.</span></span> <span data-ttu-id="be32f-150">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="be32f-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="be32f-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="be32f-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="be32f-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="be32f-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="be32f-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="be32f-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="be32f-154">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="be32f-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="be32f-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="be32f-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="be32f-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="be32f-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="be32f-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="be32f-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="be32f-158">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="be32f-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="be32f-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="be32f-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="be32f-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="be32f-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="be32f-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="be32f-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="be32f-162">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="be32f-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="be32f-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="be32f-163">createdDateTime</span></span>|<span data-ttu-id="be32f-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be32f-164">DateTimeOffset</span></span>|<span data-ttu-id="be32f-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="be32f-165">DateTime the object was created.</span></span> <span data-ttu-id="be32f-166">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="be32f-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="be32f-167">说明</span><span class="sxs-lookup"><span data-stu-id="be32f-167">description</span></span>|<span data-ttu-id="be32f-168">String</span><span class="sxs-lookup"><span data-stu-id="be32f-168">String</span></span>|<span data-ttu-id="be32f-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="be32f-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="be32f-170">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="be32f-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="be32f-171">displayName</span><span class="sxs-lookup"><span data-stu-id="be32f-171">displayName</span></span>|<span data-ttu-id="be32f-172">String</span><span class="sxs-lookup"><span data-stu-id="be32f-172">String</span></span>|<span data-ttu-id="be32f-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="be32f-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="be32f-174">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="be32f-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="be32f-175">version</span><span class="sxs-lookup"><span data-stu-id="be32f-175">version</span></span>|<span data-ttu-id="be32f-176">Int32</span><span class="sxs-lookup"><span data-stu-id="be32f-176">Int32</span></span>|<span data-ttu-id="be32f-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="be32f-177">Version of the device configuration.</span></span> <span data-ttu-id="be32f-178">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="be32f-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="be32f-179">uninstallBuiltInApps</span><span class="sxs-lookup"><span data-stu-id="be32f-179">uninstallBuiltInApps</span></span>|<span data-ttu-id="be32f-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="be32f-180">Boolean</span></span>|<span data-ttu-id="be32f-181">指示是否卸载内置 Windows 应用的固定列表。</span><span class="sxs-lookup"><span data-stu-id="be32f-181">Indicates whether or not to uninstall a fixed list of built-in Windows apps.</span></span>|



## <a name="response"></a><span data-ttu-id="be32f-182">响应</span><span class="sxs-lookup"><span data-stu-id="be32f-182">Response</span></span>
<span data-ttu-id="be32f-183">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="be32f-183">If successful, this method returns a `201 Created` response code and a [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="be32f-184">示例</span><span class="sxs-lookup"><span data-stu-id="be32f-184">Example</span></span>

### <a name="request"></a><span data-ttu-id="be32f-185">请求</span><span class="sxs-lookup"><span data-stu-id="be32f-185">Request</span></span>
<span data-ttu-id="be32f-186">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="be32f-186">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="be32f-187">响应</span><span class="sxs-lookup"><span data-stu-id="be32f-187">Response</span></span>
<span data-ttu-id="be32f-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="be32f-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




