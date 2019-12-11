---
title: 更新 macOSTrustedRootCertificate
description: 更新 macOSTrustedRootCertificate 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 06372c8ae973bd673de37711926ceed4c557aca9
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39948175"
---
# <a name="update-macostrustedrootcertificate"></a><span data-ttu-id="c9263-103">更新 macOSTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="c9263-103">Update macOSTrustedRootCertificate</span></span>

> <span data-ttu-id="c9263-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c9263-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c9263-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c9263-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c9263-106">更新[macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c9263-106">Update the properties of a [macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c9263-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="c9263-107">Prerequisites</span></span>
<span data-ttu-id="c9263-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c9263-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9263-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c9263-110">Permission type</span></span>|<span data-ttu-id="c9263-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c9263-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c9263-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c9263-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c9263-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9263-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c9263-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c9263-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c9263-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c9263-115">Not supported.</span></span>|
|<span data-ttu-id="c9263-116">Application</span><span class="sxs-lookup"><span data-stu-id="c9263-116">Application</span></span>|<span data-ttu-id="c9263-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9263-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c9263-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c9263-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSEnterpriseWiFiConfiguration/rootCertificateForServerValidation
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/microsoft.graph.macOSScepCertificateProfile/rootCertificate
```

## <a name="request-headers"></a><span data-ttu-id="c9263-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c9263-119">Request headers</span></span>
|<span data-ttu-id="c9263-120">标头</span><span class="sxs-lookup"><span data-stu-id="c9263-120">Header</span></span>|<span data-ttu-id="c9263-121">值</span><span class="sxs-lookup"><span data-stu-id="c9263-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c9263-122">授权</span><span class="sxs-lookup"><span data-stu-id="c9263-122">Authorization</span></span>|<span data-ttu-id="c9263-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c9263-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c9263-124">接受</span><span class="sxs-lookup"><span data-stu-id="c9263-124">Accept</span></span>|<span data-ttu-id="c9263-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c9263-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c9263-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c9263-126">Request body</span></span>
<span data-ttu-id="c9263-127">在请求正文中，提供[macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c9263-127">In the request body, supply a JSON representation for the [macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md) object.</span></span>

<span data-ttu-id="c9263-128">下表显示创建[macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c9263-128">The following table shows the properties that are required when you create the [macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md).</span></span>

|<span data-ttu-id="c9263-129">属性</span><span class="sxs-lookup"><span data-stu-id="c9263-129">Property</span></span>|<span data-ttu-id="c9263-130">类型</span><span class="sxs-lookup"><span data-stu-id="c9263-130">Type</span></span>|<span data-ttu-id="c9263-131">说明</span><span class="sxs-lookup"><span data-stu-id="c9263-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9263-132">id</span><span class="sxs-lookup"><span data-stu-id="c9263-132">id</span></span>|<span data-ttu-id="c9263-133">字符串</span><span class="sxs-lookup"><span data-stu-id="c9263-133">String</span></span>|<span data-ttu-id="c9263-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c9263-134">Key of the entity.</span></span> <span data-ttu-id="c9263-135">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c9263-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9263-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c9263-136">lastModifiedDateTime</span></span>|<span data-ttu-id="c9263-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9263-137">DateTimeOffset</span></span>|<span data-ttu-id="c9263-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c9263-138">DateTime the object was last modified.</span></span> <span data-ttu-id="c9263-139">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c9263-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9263-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c9263-140">roleScopeTagIds</span></span>|<span data-ttu-id="c9263-141">String collection</span><span class="sxs-lookup"><span data-stu-id="c9263-141">String collection</span></span>|<span data-ttu-id="c9263-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="c9263-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c9263-143">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c9263-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9263-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c9263-144">supportsScopeTags</span></span>|<span data-ttu-id="c9263-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9263-145">Boolean</span></span>|<span data-ttu-id="c9263-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="c9263-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c9263-147">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="c9263-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c9263-148">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="c9263-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c9263-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c9263-149">This property is read-only.</span></span> <span data-ttu-id="c9263-150">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c9263-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9263-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c9263-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="c9263-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c9263-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="c9263-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="c9263-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="c9263-154">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c9263-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9263-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c9263-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="c9263-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c9263-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="c9263-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="c9263-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="c9263-158">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c9263-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9263-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c9263-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="c9263-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c9263-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="c9263-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="c9263-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="c9263-162">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c9263-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9263-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c9263-163">createdDateTime</span></span>|<span data-ttu-id="c9263-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9263-164">DateTimeOffset</span></span>|<span data-ttu-id="c9263-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c9263-165">DateTime the object was created.</span></span> <span data-ttu-id="c9263-166">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c9263-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9263-167">说明</span><span class="sxs-lookup"><span data-stu-id="c9263-167">description</span></span>|<span data-ttu-id="c9263-168">String</span><span class="sxs-lookup"><span data-stu-id="c9263-168">String</span></span>|<span data-ttu-id="c9263-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="c9263-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c9263-170">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c9263-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9263-171">displayName</span><span class="sxs-lookup"><span data-stu-id="c9263-171">displayName</span></span>|<span data-ttu-id="c9263-172">String</span><span class="sxs-lookup"><span data-stu-id="c9263-172">String</span></span>|<span data-ttu-id="c9263-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="c9263-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c9263-174">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c9263-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9263-175">version</span><span class="sxs-lookup"><span data-stu-id="c9263-175">version</span></span>|<span data-ttu-id="c9263-176">Int32</span><span class="sxs-lookup"><span data-stu-id="c9263-176">Int32</span></span>|<span data-ttu-id="c9263-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="c9263-177">Version of the device configuration.</span></span> <span data-ttu-id="c9263-178">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c9263-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9263-179">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="c9263-179">trustedRootCertificate</span></span>|<span data-ttu-id="c9263-180">Binary</span><span class="sxs-lookup"><span data-stu-id="c9263-180">Binary</span></span>|<span data-ttu-id="c9263-181">受信任的根证书。</span><span class="sxs-lookup"><span data-stu-id="c9263-181">Trusted Root Certificate.</span></span>|
|<span data-ttu-id="c9263-182">certFileName</span><span class="sxs-lookup"><span data-stu-id="c9263-182">certFileName</span></span>|<span data-ttu-id="c9263-183">字符串</span><span class="sxs-lookup"><span data-stu-id="c9263-183">String</span></span>|<span data-ttu-id="c9263-184">要在 UI 中显示的文件名。</span><span class="sxs-lookup"><span data-stu-id="c9263-184">File name to display in UI.</span></span>|



## <a name="response"></a><span data-ttu-id="c9263-185">响应</span><span class="sxs-lookup"><span data-stu-id="c9263-185">Response</span></span>
<span data-ttu-id="c9263-186">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c9263-186">If successful, this method returns a `200 OK` response code and an updated [macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9263-187">示例</span><span class="sxs-lookup"><span data-stu-id="c9263-187">Example</span></span>

### <a name="request"></a><span data-ttu-id="c9263-188">请求</span><span class="sxs-lookup"><span data-stu-id="c9263-188">Request</span></span>
<span data-ttu-id="c9263-189">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c9263-189">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c9263-190">响应</span><span class="sxs-lookup"><span data-stu-id="c9263-190">Response</span></span>
<span data-ttu-id="c9263-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c9263-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





