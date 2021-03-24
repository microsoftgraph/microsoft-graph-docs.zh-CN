---
title: 更新 iosEducationDeviceConfiguration
description: 更新 iosEducationDeviceConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2974113ff057cec2c1d9e207fc7e3e26258ea28f
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51129921"
---
# <a name="update-ioseducationdeviceconfiguration"></a><span data-ttu-id="443fa-103">更新 iosEducationDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="443fa-103">Update iosEducationDeviceConfiguration</span></span>

<span data-ttu-id="443fa-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="443fa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="443fa-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="443fa-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="443fa-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="443fa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="443fa-107">更新 [iosEducationDeviceConfiguration 对象](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="443fa-107">Update the properties of a [iosEducationDeviceConfiguration](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="443fa-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="443fa-108">Prerequisites</span></span>
<span data-ttu-id="443fa-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="443fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="443fa-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="443fa-111">Permission type</span></span>|<span data-ttu-id="443fa-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="443fa-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="443fa-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="443fa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="443fa-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="443fa-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="443fa-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="443fa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="443fa-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="443fa-116">Not supported.</span></span>|
|<span data-ttu-id="443fa-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="443fa-117">Application</span></span>|<span data-ttu-id="443fa-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="443fa-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="443fa-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="443fa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="443fa-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="443fa-120">Request headers</span></span>
|<span data-ttu-id="443fa-121">标头</span><span class="sxs-lookup"><span data-stu-id="443fa-121">Header</span></span>|<span data-ttu-id="443fa-122">值</span><span class="sxs-lookup"><span data-stu-id="443fa-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="443fa-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="443fa-123">Authorization</span></span>|<span data-ttu-id="443fa-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="443fa-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="443fa-125">接受</span><span class="sxs-lookup"><span data-stu-id="443fa-125">Accept</span></span>|<span data-ttu-id="443fa-126">application/json</span><span class="sxs-lookup"><span data-stu-id="443fa-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="443fa-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="443fa-127">Request body</span></span>
<span data-ttu-id="443fa-128">在请求正文中，提供 [iosEducationDeviceConfiguration](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="443fa-128">In the request body, supply a JSON representation for the [iosEducationDeviceConfiguration](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md) object.</span></span>

<span data-ttu-id="443fa-129">下表显示创建 [iosEducationDeviceConfiguration 时所需的属性](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="443fa-129">The following table shows the properties that are required when you create the [iosEducationDeviceConfiguration](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md).</span></span>

|<span data-ttu-id="443fa-130">属性</span><span class="sxs-lookup"><span data-stu-id="443fa-130">Property</span></span>|<span data-ttu-id="443fa-131">类型</span><span class="sxs-lookup"><span data-stu-id="443fa-131">Type</span></span>|<span data-ttu-id="443fa-132">说明</span><span class="sxs-lookup"><span data-stu-id="443fa-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="443fa-133">id</span><span class="sxs-lookup"><span data-stu-id="443fa-133">id</span></span>|<span data-ttu-id="443fa-134">String</span><span class="sxs-lookup"><span data-stu-id="443fa-134">String</span></span>|<span data-ttu-id="443fa-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="443fa-135">Key of the entity.</span></span> <span data-ttu-id="443fa-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="443fa-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="443fa-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="443fa-137">lastModifiedDateTime</span></span>|<span data-ttu-id="443fa-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="443fa-138">DateTimeOffset</span></span>|<span data-ttu-id="443fa-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="443fa-139">DateTime the object was last modified.</span></span> <span data-ttu-id="443fa-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="443fa-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="443fa-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="443fa-141">roleScopeTagIds</span></span>|<span data-ttu-id="443fa-142">String collection</span><span class="sxs-lookup"><span data-stu-id="443fa-142">String collection</span></span>|<span data-ttu-id="443fa-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="443fa-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="443fa-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="443fa-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="443fa-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="443fa-145">supportsScopeTags</span></span>|<span data-ttu-id="443fa-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="443fa-146">Boolean</span></span>|<span data-ttu-id="443fa-147">指示基础设备配置是否支持分配范围标记。</span><span class="sxs-lookup"><span data-stu-id="443fa-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="443fa-148">当此值为 false 且实体对作用域用户不可见时，不允许分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="443fa-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="443fa-149">这适用于在 Silverlight 中创建的旧版策略，可通过在 Azure 门户中删除和重新创建策略来解决。</span><span class="sxs-lookup"><span data-stu-id="443fa-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="443fa-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="443fa-150">This property is read-only.</span></span> <span data-ttu-id="443fa-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="443fa-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="443fa-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="443fa-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="443fa-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="443fa-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="443fa-154">此策略的操作系统版本适用性。</span><span class="sxs-lookup"><span data-stu-id="443fa-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="443fa-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="443fa-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="443fa-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="443fa-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="443fa-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="443fa-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="443fa-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="443fa-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="443fa-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="443fa-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="443fa-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="443fa-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="443fa-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="443fa-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="443fa-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="443fa-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="443fa-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="443fa-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="443fa-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="443fa-164">createdDateTime</span></span>|<span data-ttu-id="443fa-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="443fa-165">DateTimeOffset</span></span>|<span data-ttu-id="443fa-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="443fa-166">DateTime the object was created.</span></span> <span data-ttu-id="443fa-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="443fa-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="443fa-168">说明</span><span class="sxs-lookup"><span data-stu-id="443fa-168">description</span></span>|<span data-ttu-id="443fa-169">String</span><span class="sxs-lookup"><span data-stu-id="443fa-169">String</span></span>|<span data-ttu-id="443fa-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="443fa-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="443fa-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="443fa-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="443fa-172">displayName</span><span class="sxs-lookup"><span data-stu-id="443fa-172">displayName</span></span>|<span data-ttu-id="443fa-173">String</span><span class="sxs-lookup"><span data-stu-id="443fa-173">String</span></span>|<span data-ttu-id="443fa-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="443fa-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="443fa-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="443fa-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="443fa-176">version</span><span class="sxs-lookup"><span data-stu-id="443fa-176">version</span></span>|<span data-ttu-id="443fa-177">Int32</span><span class="sxs-lookup"><span data-stu-id="443fa-177">Int32</span></span>|<span data-ttu-id="443fa-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="443fa-178">Version of the device configuration.</span></span> <span data-ttu-id="443fa-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="443fa-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="443fa-180">响应</span><span class="sxs-lookup"><span data-stu-id="443fa-180">Response</span></span>
<span data-ttu-id="443fa-181">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [iosEducationDeviceConfiguration](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="443fa-181">If successful, this method returns a `200 OK` response code and an updated [iosEducationDeviceConfiguration](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="443fa-182">示例</span><span class="sxs-lookup"><span data-stu-id="443fa-182">Example</span></span>

### <a name="request"></a><span data-ttu-id="443fa-183">请求</span><span class="sxs-lookup"><span data-stu-id="443fa-183">Request</span></span>
<span data-ttu-id="443fa-184">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="443fa-184">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1034

{
  "@odata.type": "#microsoft.graph.iosEducationDeviceConfiguration",
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

### <a name="response"></a><span data-ttu-id="443fa-185">响应</span><span class="sxs-lookup"><span data-stu-id="443fa-185">Response</span></span>
<span data-ttu-id="443fa-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="443fa-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1206

{
  "@odata.type": "#microsoft.graph.iosEducationDeviceConfiguration",
  "id": "3d563be4-3be4-3d56-e43b-563de43b563d",
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




