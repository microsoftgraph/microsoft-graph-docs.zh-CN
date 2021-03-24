---
title: 更新 windows81TrustedRootCertificate
description: 更新 windows81TrustedRootCertificate 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3414bb0619f08d91c1ad3ab0dad5ef8dd485d821
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51147201"
---
# <a name="update-windows81trustedrootcertificate"></a><span data-ttu-id="fc5c4-103">更新 windows81TrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="fc5c4-103">Update windows81TrustedRootCertificate</span></span>

<span data-ttu-id="fc5c4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc5c4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fc5c4-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fc5c4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fc5c4-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fc5c4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc5c4-107">更新 [windows81TrustedRootCertificate 对象](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="fc5c4-107">Update the properties of a [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fc5c4-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="fc5c4-108">Prerequisites</span></span>
<span data-ttu-id="fc5c4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fc5c4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc5c4-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="fc5c4-111">Permission type</span></span>|<span data-ttu-id="fc5c4-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fc5c4-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fc5c4-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fc5c4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fc5c4-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc5c4-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fc5c4-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fc5c4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fc5c4-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="fc5c4-116">Not supported.</span></span>|
|<span data-ttu-id="fc5c4-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="fc5c4-117">Application</span></span>|<span data-ttu-id="fc5c4-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc5c4-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fc5c4-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fc5c4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificateForClientValidation
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows81SCEPCertificateProfile/rootCertificate
```

## <a name="request-headers"></a><span data-ttu-id="fc5c4-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="fc5c4-120">Request headers</span></span>
|<span data-ttu-id="fc5c4-121">标头</span><span class="sxs-lookup"><span data-stu-id="fc5c4-121">Header</span></span>|<span data-ttu-id="fc5c4-122">值</span><span class="sxs-lookup"><span data-stu-id="fc5c4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fc5c4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fc5c4-123">Authorization</span></span>|<span data-ttu-id="fc5c4-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="fc5c4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fc5c4-125">接受</span><span class="sxs-lookup"><span data-stu-id="fc5c4-125">Accept</span></span>|<span data-ttu-id="fc5c4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fc5c4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fc5c4-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="fc5c4-127">Request body</span></span>
<span data-ttu-id="fc5c4-128">在请求正文中，提供 [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fc5c4-128">In the request body, supply a JSON representation for the [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) object.</span></span>

<span data-ttu-id="fc5c4-129">下表显示创建 [windows81TrustedRootCertificate 时所需的属性](../resources/intune-deviceconfig-windows81trustedrootcertificate.md)。</span><span class="sxs-lookup"><span data-stu-id="fc5c4-129">The following table shows the properties that are required when you create the [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md).</span></span>

|<span data-ttu-id="fc5c4-130">属性</span><span class="sxs-lookup"><span data-stu-id="fc5c4-130">Property</span></span>|<span data-ttu-id="fc5c4-131">类型</span><span class="sxs-lookup"><span data-stu-id="fc5c4-131">Type</span></span>|<span data-ttu-id="fc5c4-132">说明</span><span class="sxs-lookup"><span data-stu-id="fc5c4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc5c4-133">id</span><span class="sxs-lookup"><span data-stu-id="fc5c4-133">id</span></span>|<span data-ttu-id="fc5c4-134">String</span><span class="sxs-lookup"><span data-stu-id="fc5c4-134">String</span></span>|<span data-ttu-id="fc5c4-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="fc5c4-135">Key of the entity.</span></span> <span data-ttu-id="fc5c4-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fc5c4-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fc5c4-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fc5c4-137">lastModifiedDateTime</span></span>|<span data-ttu-id="fc5c4-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fc5c4-138">DateTimeOffset</span></span>|<span data-ttu-id="fc5c4-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="fc5c4-139">DateTime the object was last modified.</span></span> <span data-ttu-id="fc5c4-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fc5c4-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fc5c4-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="fc5c4-141">roleScopeTagIds</span></span>|<span data-ttu-id="fc5c4-142">String collection</span><span class="sxs-lookup"><span data-stu-id="fc5c4-142">String collection</span></span>|<span data-ttu-id="fc5c4-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="fc5c4-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="fc5c4-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fc5c4-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fc5c4-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="fc5c4-145">supportsScopeTags</span></span>|<span data-ttu-id="fc5c4-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc5c4-146">Boolean</span></span>|<span data-ttu-id="fc5c4-147">指示基础设备配置是否支持分配范围标记。</span><span class="sxs-lookup"><span data-stu-id="fc5c4-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="fc5c4-148">当此值为 false 且实体对作用域用户不可见时，不允许分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="fc5c4-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="fc5c4-149">这适用于在 Silverlight 中创建的旧版策略，可通过在 Azure 门户中删除和重新创建策略来解决。</span><span class="sxs-lookup"><span data-stu-id="fc5c4-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="fc5c4-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="fc5c4-150">This property is read-only.</span></span> <span data-ttu-id="fc5c4-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fc5c4-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fc5c4-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="fc5c4-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="fc5c4-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="fc5c4-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="fc5c4-154">此策略的操作系统版本适用性。</span><span class="sxs-lookup"><span data-stu-id="fc5c4-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="fc5c4-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fc5c4-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fc5c4-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="fc5c4-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="fc5c4-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="fc5c4-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="fc5c4-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="fc5c4-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="fc5c4-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fc5c4-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fc5c4-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="fc5c4-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="fc5c4-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="fc5c4-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="fc5c4-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="fc5c4-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="fc5c4-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fc5c4-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fc5c4-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fc5c4-164">createdDateTime</span></span>|<span data-ttu-id="fc5c4-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fc5c4-165">DateTimeOffset</span></span>|<span data-ttu-id="fc5c4-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="fc5c4-166">DateTime the object was created.</span></span> <span data-ttu-id="fc5c4-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fc5c4-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fc5c4-168">说明</span><span class="sxs-lookup"><span data-stu-id="fc5c4-168">description</span></span>|<span data-ttu-id="fc5c4-169">String</span><span class="sxs-lookup"><span data-stu-id="fc5c4-169">String</span></span>|<span data-ttu-id="fc5c4-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="fc5c4-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="fc5c4-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fc5c4-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fc5c4-172">displayName</span><span class="sxs-lookup"><span data-stu-id="fc5c4-172">displayName</span></span>|<span data-ttu-id="fc5c4-173">String</span><span class="sxs-lookup"><span data-stu-id="fc5c4-173">String</span></span>|<span data-ttu-id="fc5c4-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="fc5c4-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="fc5c4-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fc5c4-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fc5c4-176">version</span><span class="sxs-lookup"><span data-stu-id="fc5c4-176">version</span></span>|<span data-ttu-id="fc5c4-177">Int32</span><span class="sxs-lookup"><span data-stu-id="fc5c4-177">Int32</span></span>|<span data-ttu-id="fc5c4-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="fc5c4-178">Version of the device configuration.</span></span> <span data-ttu-id="fc5c4-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fc5c4-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fc5c4-180">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="fc5c4-180">trustedRootCertificate</span></span>|<span data-ttu-id="fc5c4-181">Binary</span><span class="sxs-lookup"><span data-stu-id="fc5c4-181">Binary</span></span>|<span data-ttu-id="fc5c4-182">受信任的根证书</span><span class="sxs-lookup"><span data-stu-id="fc5c4-182">Trusted Root Certificate</span></span>|
|<span data-ttu-id="fc5c4-183">certFileName</span><span class="sxs-lookup"><span data-stu-id="fc5c4-183">certFileName</span></span>|<span data-ttu-id="fc5c4-184">String</span><span class="sxs-lookup"><span data-stu-id="fc5c4-184">String</span></span>|<span data-ttu-id="fc5c4-185">要显示在 UI 中的文件名。</span><span class="sxs-lookup"><span data-stu-id="fc5c4-185">File name to display in UI.</span></span>|
|<span data-ttu-id="fc5c4-186">destinationStore</span><span class="sxs-lookup"><span data-stu-id="fc5c4-186">destinationStore</span></span>|[<span data-ttu-id="fc5c4-187">certificateDestinationStore</span><span class="sxs-lookup"><span data-stu-id="fc5c4-187">certificateDestinationStore</span></span>](../resources/intune-shared-certificatedestinationstore.md)|<span data-ttu-id="fc5c4-188">受信任根证书的目标存储位置。</span><span class="sxs-lookup"><span data-stu-id="fc5c4-188">Destination store location for the Trusted Root Certificate.</span></span> <span data-ttu-id="fc5c4-189">可取值为：`computerCertStoreRoot`、`computerCertStoreIntermediate`、`userCertStoreIntermediate`。</span><span class="sxs-lookup"><span data-stu-id="fc5c4-189">Possible values are: `computerCertStoreRoot`, `computerCertStoreIntermediate`, `userCertStoreIntermediate`.</span></span>|



## <a name="response"></a><span data-ttu-id="fc5c4-190">响应</span><span class="sxs-lookup"><span data-stu-id="fc5c4-190">Response</span></span>
<span data-ttu-id="fc5c4-191">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fc5c4-191">If successful, this method returns a `200 OK` response code and an updated [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc5c4-192">示例</span><span class="sxs-lookup"><span data-stu-id="fc5c4-192">Example</span></span>

### <a name="request"></a><span data-ttu-id="fc5c4-193">请求</span><span class="sxs-lookup"><span data-stu-id="fc5c4-193">Request</span></span>
<span data-ttu-id="fc5c4-194">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fc5c4-194">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificateForClientValidation
Content-type: application/json
Content-length: 1198

{
  "@odata.type": "#microsoft.graph.windows81TrustedRootCertificate",
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
  "certFileName": "Cert File Name value",
  "destinationStore": "computerCertStoreIntermediate"
}
```

### <a name="response"></a><span data-ttu-id="fc5c4-195">响应</span><span class="sxs-lookup"><span data-stu-id="fc5c4-195">Response</span></span>
<span data-ttu-id="fc5c4-p114">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fc5c4-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1370

{
  "@odata.type": "#microsoft.graph.windows81TrustedRootCertificate",
  "id": "3fb588f9-88f9-3fb5-f988-b53ff988b53f",
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
  "certFileName": "Cert File Name value",
  "destinationStore": "computerCertStoreIntermediate"
}
```




