---
title: 创建 windows81TrustedRootCertificate
description: 创建新的 windows81TrustedRootCertificate 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1800f1ceb020e1ba5f3b7af9643a7f5e40991735
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51147250"
---
# <a name="create-windows81trustedrootcertificate"></a><span data-ttu-id="f4bc1-103">创建 windows81TrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="f4bc1-103">Create windows81TrustedRootCertificate</span></span>

<span data-ttu-id="f4bc1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4bc1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f4bc1-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f4bc1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f4bc1-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f4bc1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4bc1-107">创建新的 [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f4bc1-107">Create a new [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f4bc1-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="f4bc1-108">Prerequisites</span></span>
<span data-ttu-id="f4bc1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f4bc1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4bc1-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f4bc1-111">Permission type</span></span>|<span data-ttu-id="f4bc1-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f4bc1-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f4bc1-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f4bc1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f4bc1-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4bc1-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f4bc1-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f4bc1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f4bc1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f4bc1-116">Not supported.</span></span>|
|<span data-ttu-id="f4bc1-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f4bc1-117">Application</span></span>|<span data-ttu-id="f4bc1-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4bc1-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f4bc1-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f4bc1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation
```

## <a name="request-headers"></a><span data-ttu-id="f4bc1-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f4bc1-120">Request headers</span></span>
|<span data-ttu-id="f4bc1-121">标头</span><span class="sxs-lookup"><span data-stu-id="f4bc1-121">Header</span></span>|<span data-ttu-id="f4bc1-122">值</span><span class="sxs-lookup"><span data-stu-id="f4bc1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f4bc1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f4bc1-123">Authorization</span></span>|<span data-ttu-id="f4bc1-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f4bc1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f4bc1-125">接受</span><span class="sxs-lookup"><span data-stu-id="f4bc1-125">Accept</span></span>|<span data-ttu-id="f4bc1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f4bc1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4bc1-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f4bc1-127">Request body</span></span>
<span data-ttu-id="f4bc1-128">在请求正文中，提供 windows81TrustedRootCertificate 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f4bc1-128">In the request body, supply a JSON representation for the windows81TrustedRootCertificate object.</span></span>

<span data-ttu-id="f4bc1-129">下表显示创建 windows81TrustedRootCertificate 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f4bc1-129">The following table shows the properties that are required when you create the windows81TrustedRootCertificate.</span></span>

|<span data-ttu-id="f4bc1-130">属性</span><span class="sxs-lookup"><span data-stu-id="f4bc1-130">Property</span></span>|<span data-ttu-id="f4bc1-131">类型</span><span class="sxs-lookup"><span data-stu-id="f4bc1-131">Type</span></span>|<span data-ttu-id="f4bc1-132">说明</span><span class="sxs-lookup"><span data-stu-id="f4bc1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4bc1-133">id</span><span class="sxs-lookup"><span data-stu-id="f4bc1-133">id</span></span>|<span data-ttu-id="f4bc1-134">String</span><span class="sxs-lookup"><span data-stu-id="f4bc1-134">String</span></span>|<span data-ttu-id="f4bc1-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f4bc1-135">Key of the entity.</span></span> <span data-ttu-id="f4bc1-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4bc1-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4bc1-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f4bc1-137">lastModifiedDateTime</span></span>|<span data-ttu-id="f4bc1-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4bc1-138">DateTimeOffset</span></span>|<span data-ttu-id="f4bc1-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f4bc1-139">DateTime the object was last modified.</span></span> <span data-ttu-id="f4bc1-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4bc1-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4bc1-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f4bc1-141">roleScopeTagIds</span></span>|<span data-ttu-id="f4bc1-142">String collection</span><span class="sxs-lookup"><span data-stu-id="f4bc1-142">String collection</span></span>|<span data-ttu-id="f4bc1-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="f4bc1-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f4bc1-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4bc1-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4bc1-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f4bc1-145">supportsScopeTags</span></span>|<span data-ttu-id="f4bc1-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4bc1-146">Boolean</span></span>|<span data-ttu-id="f4bc1-147">指示基础设备配置是否支持分配范围标记。</span><span class="sxs-lookup"><span data-stu-id="f4bc1-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f4bc1-148">当此值为 false 且实体对作用域用户不可见时，不允许分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="f4bc1-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f4bc1-149">这适用于在 Silverlight 中创建的旧版策略，可通过在 Azure 门户中删除和重新创建策略来解决。</span><span class="sxs-lookup"><span data-stu-id="f4bc1-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f4bc1-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="f4bc1-150">This property is read-only.</span></span> <span data-ttu-id="f4bc1-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4bc1-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4bc1-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f4bc1-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="f4bc1-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f4bc1-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="f4bc1-154">此策略的操作系统版本适用性。</span><span class="sxs-lookup"><span data-stu-id="f4bc1-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="f4bc1-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4bc1-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4bc1-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f4bc1-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="f4bc1-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f4bc1-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="f4bc1-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="f4bc1-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="f4bc1-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4bc1-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4bc1-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f4bc1-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="f4bc1-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f4bc1-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="f4bc1-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="f4bc1-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="f4bc1-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4bc1-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4bc1-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f4bc1-164">createdDateTime</span></span>|<span data-ttu-id="f4bc1-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4bc1-165">DateTimeOffset</span></span>|<span data-ttu-id="f4bc1-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f4bc1-166">DateTime the object was created.</span></span> <span data-ttu-id="f4bc1-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4bc1-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4bc1-168">说明</span><span class="sxs-lookup"><span data-stu-id="f4bc1-168">description</span></span>|<span data-ttu-id="f4bc1-169">String</span><span class="sxs-lookup"><span data-stu-id="f4bc1-169">String</span></span>|<span data-ttu-id="f4bc1-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="f4bc1-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f4bc1-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4bc1-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4bc1-172">displayName</span><span class="sxs-lookup"><span data-stu-id="f4bc1-172">displayName</span></span>|<span data-ttu-id="f4bc1-173">String</span><span class="sxs-lookup"><span data-stu-id="f4bc1-173">String</span></span>|<span data-ttu-id="f4bc1-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="f4bc1-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f4bc1-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4bc1-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4bc1-176">version</span><span class="sxs-lookup"><span data-stu-id="f4bc1-176">version</span></span>|<span data-ttu-id="f4bc1-177">Int32</span><span class="sxs-lookup"><span data-stu-id="f4bc1-177">Int32</span></span>|<span data-ttu-id="f4bc1-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="f4bc1-178">Version of the device configuration.</span></span> <span data-ttu-id="f4bc1-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4bc1-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4bc1-180">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="f4bc1-180">trustedRootCertificate</span></span>|<span data-ttu-id="f4bc1-181">Binary</span><span class="sxs-lookup"><span data-stu-id="f4bc1-181">Binary</span></span>|<span data-ttu-id="f4bc1-182">受信任的根证书</span><span class="sxs-lookup"><span data-stu-id="f4bc1-182">Trusted Root Certificate</span></span>|
|<span data-ttu-id="f4bc1-183">certFileName</span><span class="sxs-lookup"><span data-stu-id="f4bc1-183">certFileName</span></span>|<span data-ttu-id="f4bc1-184">String</span><span class="sxs-lookup"><span data-stu-id="f4bc1-184">String</span></span>|<span data-ttu-id="f4bc1-185">要显示在 UI 中的文件名。</span><span class="sxs-lookup"><span data-stu-id="f4bc1-185">File name to display in UI.</span></span>|
|<span data-ttu-id="f4bc1-186">destinationStore</span><span class="sxs-lookup"><span data-stu-id="f4bc1-186">destinationStore</span></span>|[<span data-ttu-id="f4bc1-187">certificateDestinationStore</span><span class="sxs-lookup"><span data-stu-id="f4bc1-187">certificateDestinationStore</span></span>](../resources/intune-shared-certificatedestinationstore.md)|<span data-ttu-id="f4bc1-188">受信任根证书的目标存储位置。</span><span class="sxs-lookup"><span data-stu-id="f4bc1-188">Destination store location for the Trusted Root Certificate.</span></span> <span data-ttu-id="f4bc1-189">可取值为：`computerCertStoreRoot`、`computerCertStoreIntermediate`、`userCertStoreIntermediate`。</span><span class="sxs-lookup"><span data-stu-id="f4bc1-189">Possible values are: `computerCertStoreRoot`, `computerCertStoreIntermediate`, `userCertStoreIntermediate`.</span></span>|



## <a name="response"></a><span data-ttu-id="f4bc1-190">响应</span><span class="sxs-lookup"><span data-stu-id="f4bc1-190">Response</span></span>
<span data-ttu-id="f4bc1-191">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f4bc1-191">If successful, this method returns a `201 Created` response code and a [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4bc1-192">示例</span><span class="sxs-lookup"><span data-stu-id="f4bc1-192">Example</span></span>

### <a name="request"></a><span data-ttu-id="f4bc1-193">请求</span><span class="sxs-lookup"><span data-stu-id="f4bc1-193">Request</span></span>
<span data-ttu-id="f4bc1-194">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f4bc1-194">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation
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

### <a name="response"></a><span data-ttu-id="f4bc1-195">响应</span><span class="sxs-lookup"><span data-stu-id="f4bc1-195">Response</span></span>
<span data-ttu-id="f4bc1-p114">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f4bc1-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




