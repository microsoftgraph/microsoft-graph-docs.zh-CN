---
title: 更新 iosDerivedCredentialAuthenticationConfiguration
description: 更新 iosDerivedCredentialAuthenticationConfiguration 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 95bb856650c2b5fb3e71d1126c62425385185996
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37533929"
---
# <a name="update-iosderivedcredentialauthenticationconfiguration"></a><span data-ttu-id="a6c64-103">更新 iosDerivedCredentialAuthenticationConfiguration</span><span class="sxs-lookup"><span data-stu-id="a6c64-103">Update iosDerivedCredentialAuthenticationConfiguration</span></span>

> <span data-ttu-id="a6c64-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a6c64-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a6c64-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a6c64-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6c64-106">更新[iosDerivedCredentialAuthenticationConfiguration](../resources/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a6c64-106">Update the properties of a [iosDerivedCredentialAuthenticationConfiguration](../resources/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a6c64-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="a6c64-107">Prerequisites</span></span>
<span data-ttu-id="a6c64-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a6c64-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6c64-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a6c64-110">Permission type</span></span>|<span data-ttu-id="a6c64-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a6c64-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a6c64-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a6c64-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a6c64-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6c64-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a6c64-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a6c64-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a6c64-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a6c64-115">Not supported.</span></span>|
|<span data-ttu-id="a6c64-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a6c64-116">Application</span></span>|<span data-ttu-id="a6c64-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6c64-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a6c64-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a6c64-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="a6c64-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a6c64-119">Request headers</span></span>
|<span data-ttu-id="a6c64-120">标头</span><span class="sxs-lookup"><span data-stu-id="a6c64-120">Header</span></span>|<span data-ttu-id="a6c64-121">值</span><span class="sxs-lookup"><span data-stu-id="a6c64-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a6c64-122">授权</span><span class="sxs-lookup"><span data-stu-id="a6c64-122">Authorization</span></span>|<span data-ttu-id="a6c64-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a6c64-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a6c64-124">接受</span><span class="sxs-lookup"><span data-stu-id="a6c64-124">Accept</span></span>|<span data-ttu-id="a6c64-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a6c64-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6c64-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a6c64-126">Request body</span></span>
<span data-ttu-id="a6c64-127">在请求正文中，提供[iosDerivedCredentialAuthenticationConfiguration](../resources/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a6c64-127">In the request body, supply a JSON representation for the [iosDerivedCredentialAuthenticationConfiguration](../resources/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration.md) object.</span></span>

<span data-ttu-id="a6c64-128">下表显示创建[iosDerivedCredentialAuthenticationConfiguration](../resources/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a6c64-128">The following table shows the properties that are required when you create the [iosDerivedCredentialAuthenticationConfiguration](../resources/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration.md).</span></span>

|<span data-ttu-id="a6c64-129">属性</span><span class="sxs-lookup"><span data-stu-id="a6c64-129">Property</span></span>|<span data-ttu-id="a6c64-130">类型</span><span class="sxs-lookup"><span data-stu-id="a6c64-130">Type</span></span>|<span data-ttu-id="a6c64-131">说明</span><span class="sxs-lookup"><span data-stu-id="a6c64-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6c64-132">id</span><span class="sxs-lookup"><span data-stu-id="a6c64-132">id</span></span>|<span data-ttu-id="a6c64-133">字符串</span><span class="sxs-lookup"><span data-stu-id="a6c64-133">String</span></span>|<span data-ttu-id="a6c64-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a6c64-134">Key of the entity.</span></span> <span data-ttu-id="a6c64-135">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a6c64-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6c64-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a6c64-136">lastModifiedDateTime</span></span>|<span data-ttu-id="a6c64-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a6c64-137">DateTimeOffset</span></span>|<span data-ttu-id="a6c64-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="a6c64-138">DateTime the object was last modified.</span></span> <span data-ttu-id="a6c64-139">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a6c64-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6c64-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a6c64-140">roleScopeTagIds</span></span>|<span data-ttu-id="a6c64-141">String 集合</span><span class="sxs-lookup"><span data-stu-id="a6c64-141">String collection</span></span>|<span data-ttu-id="a6c64-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="a6c64-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a6c64-143">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a6c64-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6c64-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a6c64-144">supportsScopeTags</span></span>|<span data-ttu-id="a6c64-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="a6c64-145">Boolean</span></span>|<span data-ttu-id="a6c64-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="a6c64-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a6c64-147">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="a6c64-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a6c64-148">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="a6c64-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a6c64-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="a6c64-149">This property is read-only.</span></span> <span data-ttu-id="a6c64-150">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a6c64-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6c64-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a6c64-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="a6c64-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a6c64-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="a6c64-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="a6c64-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="a6c64-154">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a6c64-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6c64-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a6c64-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="a6c64-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a6c64-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="a6c64-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="a6c64-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="a6c64-158">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a6c64-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6c64-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a6c64-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="a6c64-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a6c64-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="a6c64-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="a6c64-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="a6c64-162">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a6c64-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6c64-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a6c64-163">createdDateTime</span></span>|<span data-ttu-id="a6c64-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a6c64-164">DateTimeOffset</span></span>|<span data-ttu-id="a6c64-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="a6c64-165">DateTime the object was created.</span></span> <span data-ttu-id="a6c64-166">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a6c64-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6c64-167">说明</span><span class="sxs-lookup"><span data-stu-id="a6c64-167">description</span></span>|<span data-ttu-id="a6c64-168">String</span><span class="sxs-lookup"><span data-stu-id="a6c64-168">String</span></span>|<span data-ttu-id="a6c64-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="a6c64-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a6c64-170">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a6c64-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6c64-171">displayName</span><span class="sxs-lookup"><span data-stu-id="a6c64-171">displayName</span></span>|<span data-ttu-id="a6c64-172">String</span><span class="sxs-lookup"><span data-stu-id="a6c64-172">String</span></span>|<span data-ttu-id="a6c64-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="a6c64-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a6c64-174">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a6c64-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6c64-175">version</span><span class="sxs-lookup"><span data-stu-id="a6c64-175">version</span></span>|<span data-ttu-id="a6c64-176">Int32</span><span class="sxs-lookup"><span data-stu-id="a6c64-176">Int32</span></span>|<span data-ttu-id="a6c64-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="a6c64-177">Version of the device configuration.</span></span> <span data-ttu-id="a6c64-178">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a6c64-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="a6c64-179">响应</span><span class="sxs-lookup"><span data-stu-id="a6c64-179">Response</span></span>
<span data-ttu-id="a6c64-180">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[iosDerivedCredentialAuthenticationConfiguration](../resources/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a6c64-180">If successful, this method returns a `200 OK` response code and an updated [iosDerivedCredentialAuthenticationConfiguration](../resources/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6c64-181">示例</span><span class="sxs-lookup"><span data-stu-id="a6c64-181">Example</span></span>

### <a name="request"></a><span data-ttu-id="a6c64-182">请求</span><span class="sxs-lookup"><span data-stu-id="a6c64-182">Request</span></span>
<span data-ttu-id="a6c64-183">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a6c64-183">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1050

{
  "@odata.type": "#microsoft.graph.iosDerivedCredentialAuthenticationConfiguration",
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
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="a6c64-184">响应</span><span class="sxs-lookup"><span data-stu-id="a6c64-184">Response</span></span>
<span data-ttu-id="a6c64-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a6c64-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1222

{
  "@odata.type": "#microsoft.graph.iosDerivedCredentialAuthenticationConfiguration",
  "id": "01713f58-3f58-0171-583f-7101583f7101",
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
  "version": 7
}
```






