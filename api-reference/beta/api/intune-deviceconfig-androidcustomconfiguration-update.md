---
title: 更新 androidCustomConfiguration
description: 更新 androidCustomConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 333c7baadc94699ffa59260b269782382a5d017e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51126705"
---
# <a name="update-androidcustomconfiguration"></a><span data-ttu-id="87244-103">更新 androidCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="87244-103">Update androidCustomConfiguration</span></span>

<span data-ttu-id="87244-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="87244-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="87244-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="87244-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="87244-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="87244-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="87244-107">更新 [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="87244-107">Update the properties of a [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="87244-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="87244-108">Prerequisites</span></span>
<span data-ttu-id="87244-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="87244-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87244-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="87244-111">Permission type</span></span>|<span data-ttu-id="87244-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="87244-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="87244-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="87244-113">Delegated (work or school account)</span></span>|<span data-ttu-id="87244-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87244-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="87244-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="87244-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="87244-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="87244-116">Not supported.</span></span>|
|<span data-ttu-id="87244-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="87244-117">Application</span></span>|<span data-ttu-id="87244-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87244-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="87244-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="87244-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="87244-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="87244-120">Request headers</span></span>
|<span data-ttu-id="87244-121">标头</span><span class="sxs-lookup"><span data-stu-id="87244-121">Header</span></span>|<span data-ttu-id="87244-122">值</span><span class="sxs-lookup"><span data-stu-id="87244-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="87244-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="87244-123">Authorization</span></span>|<span data-ttu-id="87244-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="87244-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="87244-125">接受</span><span class="sxs-lookup"><span data-stu-id="87244-125">Accept</span></span>|<span data-ttu-id="87244-126">application/json</span><span class="sxs-lookup"><span data-stu-id="87244-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="87244-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="87244-127">Request body</span></span>
<span data-ttu-id="87244-128">在请求正文中，提供 [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="87244-128">In the request body, supply a JSON representation for the [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object.</span></span>

<span data-ttu-id="87244-129">下表显示了创建 [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="87244-129">The following table shows the properties that are required when you create the [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md).</span></span>

|<span data-ttu-id="87244-130">属性</span><span class="sxs-lookup"><span data-stu-id="87244-130">Property</span></span>|<span data-ttu-id="87244-131">类型</span><span class="sxs-lookup"><span data-stu-id="87244-131">Type</span></span>|<span data-ttu-id="87244-132">说明</span><span class="sxs-lookup"><span data-stu-id="87244-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="87244-133">id</span><span class="sxs-lookup"><span data-stu-id="87244-133">id</span></span>|<span data-ttu-id="87244-134">String</span><span class="sxs-lookup"><span data-stu-id="87244-134">String</span></span>|<span data-ttu-id="87244-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="87244-135">Key of the entity.</span></span> <span data-ttu-id="87244-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="87244-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87244-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="87244-137">lastModifiedDateTime</span></span>|<span data-ttu-id="87244-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="87244-138">DateTimeOffset</span></span>|<span data-ttu-id="87244-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="87244-139">DateTime the object was last modified.</span></span> <span data-ttu-id="87244-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="87244-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87244-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="87244-141">roleScopeTagIds</span></span>|<span data-ttu-id="87244-142">String collection</span><span class="sxs-lookup"><span data-stu-id="87244-142">String collection</span></span>|<span data-ttu-id="87244-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="87244-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="87244-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="87244-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87244-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="87244-145">supportsScopeTags</span></span>|<span data-ttu-id="87244-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="87244-146">Boolean</span></span>|<span data-ttu-id="87244-147">指示基础设备配置是否支持分配范围标记。</span><span class="sxs-lookup"><span data-stu-id="87244-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="87244-148">当此值为 false 且实体对作用域用户不可见时，不允许分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="87244-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="87244-149">这适用于在 Silverlight 中创建的旧版策略，可通过在 Azure 门户中删除和重新创建策略来解决。</span><span class="sxs-lookup"><span data-stu-id="87244-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="87244-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="87244-150">This property is read-only.</span></span> <span data-ttu-id="87244-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="87244-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87244-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="87244-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="87244-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="87244-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="87244-154">此策略的操作系统版本适用性。</span><span class="sxs-lookup"><span data-stu-id="87244-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="87244-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="87244-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87244-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="87244-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="87244-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="87244-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="87244-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="87244-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="87244-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="87244-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87244-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="87244-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="87244-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="87244-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="87244-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="87244-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="87244-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="87244-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87244-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="87244-164">createdDateTime</span></span>|<span data-ttu-id="87244-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="87244-165">DateTimeOffset</span></span>|<span data-ttu-id="87244-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="87244-166">DateTime the object was created.</span></span> <span data-ttu-id="87244-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="87244-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87244-168">说明</span><span class="sxs-lookup"><span data-stu-id="87244-168">description</span></span>|<span data-ttu-id="87244-169">String</span><span class="sxs-lookup"><span data-stu-id="87244-169">String</span></span>|<span data-ttu-id="87244-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="87244-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="87244-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="87244-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87244-172">displayName</span><span class="sxs-lookup"><span data-stu-id="87244-172">displayName</span></span>|<span data-ttu-id="87244-173">String</span><span class="sxs-lookup"><span data-stu-id="87244-173">String</span></span>|<span data-ttu-id="87244-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="87244-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="87244-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="87244-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87244-176">version</span><span class="sxs-lookup"><span data-stu-id="87244-176">version</span></span>|<span data-ttu-id="87244-177">Int32</span><span class="sxs-lookup"><span data-stu-id="87244-177">Int32</span></span>|<span data-ttu-id="87244-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="87244-178">Version of the device configuration.</span></span> <span data-ttu-id="87244-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="87244-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87244-180">omaSettings</span><span class="sxs-lookup"><span data-stu-id="87244-180">omaSettings</span></span>|<span data-ttu-id="87244-181">[omaSetting](../resources/intune-deviceconfig-omasetting.md) 集合</span><span class="sxs-lookup"><span data-stu-id="87244-181">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="87244-182">OMA 设置。</span><span class="sxs-lookup"><span data-stu-id="87244-182">OMA settings.</span></span> <span data-ttu-id="87244-183">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="87244-183">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="87244-184">响应</span><span class="sxs-lookup"><span data-stu-id="87244-184">Response</span></span>
<span data-ttu-id="87244-185">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="87244-185">If successful, this method returns a `200 OK` response code and an updated [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87244-186">示例</span><span class="sxs-lookup"><span data-stu-id="87244-186">Example</span></span>

### <a name="request"></a><span data-ttu-id="87244-187">请求</span><span class="sxs-lookup"><span data-stu-id="87244-187">Request</span></span>
<span data-ttu-id="87244-188">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="87244-188">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1269

{
  "@odata.type": "#microsoft.graph.androidCustomConfiguration",
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
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSetting",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value",
      "isEncrypted": true
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="87244-189">响应</span><span class="sxs-lookup"><span data-stu-id="87244-189">Response</span></span>
<span data-ttu-id="87244-p114">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="87244-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1441

{
  "@odata.type": "#microsoft.graph.androidCustomConfiguration",
  "id": "619b5e6d-5e6d-619b-6d5e-9b616d5e9b61",
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
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSetting",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value",
      "isEncrypted": true
    }
  ]
}
```




