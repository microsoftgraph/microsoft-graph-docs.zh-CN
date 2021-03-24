---
title: 更新 macOSTrustedRootCertificate
description: 更新 macOSTrustedRootCertificate 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3f96e5ad8349cd2d0268fd5987fab69398f83881
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51131195"
---
# <a name="update-macostrustedrootcertificate"></a><span data-ttu-id="51b42-103">更新 macOSTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="51b42-103">Update macOSTrustedRootCertificate</span></span>

<span data-ttu-id="51b42-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="51b42-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="51b42-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="51b42-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="51b42-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="51b42-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51b42-107">更新 [macOSTrustedRootCertificate 对象](../resources/intune-deviceconfig-macostrustedrootcertificate.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="51b42-107">Update the properties of a [macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="51b42-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="51b42-108">Prerequisites</span></span>
<span data-ttu-id="51b42-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="51b42-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51b42-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="51b42-111">Permission type</span></span>|<span data-ttu-id="51b42-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="51b42-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51b42-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="51b42-113">Delegated (work or school account)</span></span>|<span data-ttu-id="51b42-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51b42-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="51b42-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="51b42-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51b42-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="51b42-116">Not supported.</span></span>|
|<span data-ttu-id="51b42-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="51b42-117">Application</span></span>|<span data-ttu-id="51b42-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51b42-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="51b42-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="51b42-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSEnterpriseWiFiConfiguration/rootCertificateForServerValidation
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSEnterpriseWiFiConfiguration/rootCertificatesForServerValidation/{macOSTrustedRootCertificateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/microsoft.graph.macOSScepCertificateProfile/rootCertificate
```

## <a name="request-headers"></a><span data-ttu-id="51b42-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="51b42-120">Request headers</span></span>
|<span data-ttu-id="51b42-121">标头</span><span class="sxs-lookup"><span data-stu-id="51b42-121">Header</span></span>|<span data-ttu-id="51b42-122">值</span><span class="sxs-lookup"><span data-stu-id="51b42-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="51b42-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="51b42-123">Authorization</span></span>|<span data-ttu-id="51b42-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="51b42-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="51b42-125">接受</span><span class="sxs-lookup"><span data-stu-id="51b42-125">Accept</span></span>|<span data-ttu-id="51b42-126">application/json</span><span class="sxs-lookup"><span data-stu-id="51b42-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="51b42-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="51b42-127">Request body</span></span>
<span data-ttu-id="51b42-128">在请求正文中，提供 [macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="51b42-128">In the request body, supply a JSON representation for the [macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md) object.</span></span>

<span data-ttu-id="51b42-129">下表显示创建 [macOSTrustedRootCertificate 时所需的属性](../resources/intune-deviceconfig-macostrustedrootcertificate.md)。</span><span class="sxs-lookup"><span data-stu-id="51b42-129">The following table shows the properties that are required when you create the [macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md).</span></span>

|<span data-ttu-id="51b42-130">属性</span><span class="sxs-lookup"><span data-stu-id="51b42-130">Property</span></span>|<span data-ttu-id="51b42-131">类型</span><span class="sxs-lookup"><span data-stu-id="51b42-131">Type</span></span>|<span data-ttu-id="51b42-132">说明</span><span class="sxs-lookup"><span data-stu-id="51b42-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51b42-133">id</span><span class="sxs-lookup"><span data-stu-id="51b42-133">id</span></span>|<span data-ttu-id="51b42-134">String</span><span class="sxs-lookup"><span data-stu-id="51b42-134">String</span></span>|<span data-ttu-id="51b42-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="51b42-135">Key of the entity.</span></span> <span data-ttu-id="51b42-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="51b42-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51b42-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="51b42-137">lastModifiedDateTime</span></span>|<span data-ttu-id="51b42-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51b42-138">DateTimeOffset</span></span>|<span data-ttu-id="51b42-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="51b42-139">DateTime the object was last modified.</span></span> <span data-ttu-id="51b42-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="51b42-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51b42-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="51b42-141">roleScopeTagIds</span></span>|<span data-ttu-id="51b42-142">String collection</span><span class="sxs-lookup"><span data-stu-id="51b42-142">String collection</span></span>|<span data-ttu-id="51b42-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="51b42-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="51b42-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="51b42-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51b42-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="51b42-145">supportsScopeTags</span></span>|<span data-ttu-id="51b42-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="51b42-146">Boolean</span></span>|<span data-ttu-id="51b42-147">指示基础设备配置是否支持分配范围标记。</span><span class="sxs-lookup"><span data-stu-id="51b42-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="51b42-148">当此值为 false 且实体对作用域用户不可见时，不允许分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="51b42-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="51b42-149">这适用于在 Silverlight 中创建的旧版策略，可通过在 Azure 门户中删除和重新创建策略来解决。</span><span class="sxs-lookup"><span data-stu-id="51b42-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="51b42-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="51b42-150">This property is read-only.</span></span> <span data-ttu-id="51b42-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="51b42-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51b42-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="51b42-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="51b42-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="51b42-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="51b42-154">此策略的操作系统版本适用性。</span><span class="sxs-lookup"><span data-stu-id="51b42-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="51b42-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="51b42-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51b42-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="51b42-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="51b42-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="51b42-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="51b42-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="51b42-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="51b42-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="51b42-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51b42-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="51b42-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="51b42-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="51b42-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="51b42-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="51b42-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="51b42-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="51b42-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51b42-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="51b42-164">createdDateTime</span></span>|<span data-ttu-id="51b42-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51b42-165">DateTimeOffset</span></span>|<span data-ttu-id="51b42-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="51b42-166">DateTime the object was created.</span></span> <span data-ttu-id="51b42-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="51b42-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51b42-168">说明</span><span class="sxs-lookup"><span data-stu-id="51b42-168">description</span></span>|<span data-ttu-id="51b42-169">String</span><span class="sxs-lookup"><span data-stu-id="51b42-169">String</span></span>|<span data-ttu-id="51b42-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="51b42-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="51b42-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="51b42-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51b42-172">displayName</span><span class="sxs-lookup"><span data-stu-id="51b42-172">displayName</span></span>|<span data-ttu-id="51b42-173">String</span><span class="sxs-lookup"><span data-stu-id="51b42-173">String</span></span>|<span data-ttu-id="51b42-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="51b42-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="51b42-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="51b42-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51b42-176">version</span><span class="sxs-lookup"><span data-stu-id="51b42-176">version</span></span>|<span data-ttu-id="51b42-177">Int32</span><span class="sxs-lookup"><span data-stu-id="51b42-177">Int32</span></span>|<span data-ttu-id="51b42-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="51b42-178">Version of the device configuration.</span></span> <span data-ttu-id="51b42-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="51b42-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51b42-180">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="51b42-180">trustedRootCertificate</span></span>|<span data-ttu-id="51b42-181">Binary</span><span class="sxs-lookup"><span data-stu-id="51b42-181">Binary</span></span>|<span data-ttu-id="51b42-182">受信任的根证书。</span><span class="sxs-lookup"><span data-stu-id="51b42-182">Trusted Root Certificate.</span></span>|
|<span data-ttu-id="51b42-183">certFileName</span><span class="sxs-lookup"><span data-stu-id="51b42-183">certFileName</span></span>|<span data-ttu-id="51b42-184">String</span><span class="sxs-lookup"><span data-stu-id="51b42-184">String</span></span>|<span data-ttu-id="51b42-185">要显示在 UI 中的文件名。</span><span class="sxs-lookup"><span data-stu-id="51b42-185">File name to display in UI.</span></span>|



## <a name="response"></a><span data-ttu-id="51b42-186">响应</span><span class="sxs-lookup"><span data-stu-id="51b42-186">Response</span></span>
<span data-ttu-id="51b42-187">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="51b42-187">If successful, this method returns a `200 OK` response code and an updated [macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51b42-188">示例</span><span class="sxs-lookup"><span data-stu-id="51b42-188">Example</span></span>

### <a name="request"></a><span data-ttu-id="51b42-189">请求</span><span class="sxs-lookup"><span data-stu-id="51b42-189">Request</span></span>
<span data-ttu-id="51b42-190">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="51b42-190">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation
Content-type: application/json
Content-length: 1138

{
  "@odata.type": "#microsoft.graph.macOSTrustedRootCertificate",
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
  "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
  "certFileName": "Cert File Name value"
}
```

### <a name="response"></a><span data-ttu-id="51b42-191">响应</span><span class="sxs-lookup"><span data-stu-id="51b42-191">Response</span></span>
<span data-ttu-id="51b42-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="51b42-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1310

{
  "@odata.type": "#microsoft.graph.macOSTrustedRootCertificate",
  "id": "c5fac954-c954-c5fa-54c9-fac554c9fac5",
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
  "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
  "certFileName": "Cert File Name value"
}
```




