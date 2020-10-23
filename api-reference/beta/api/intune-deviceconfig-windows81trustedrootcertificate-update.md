---
title: 更新 windows81TrustedRootCertificate
description: 更新 windows81TrustedRootCertificate 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5f6f4a15094a7795127105cbd77ef45414085c30
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48723523"
---
# <a name="update-windows81trustedrootcertificate"></a><span data-ttu-id="c9c86-103">更新 windows81TrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="c9c86-103">Update windows81TrustedRootCertificate</span></span>

<span data-ttu-id="c9c86-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c9c86-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c9c86-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c9c86-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c9c86-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c9c86-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c9c86-107">更新 [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c9c86-107">Update the properties of a [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c9c86-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="c9c86-108">Prerequisites</span></span>
<span data-ttu-id="c9c86-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c9c86-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9c86-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c9c86-111">Permission type</span></span>|<span data-ttu-id="c9c86-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c9c86-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c9c86-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c9c86-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c9c86-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9c86-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c9c86-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c9c86-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c9c86-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c9c86-116">Not supported.</span></span>|
|<span data-ttu-id="c9c86-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c9c86-117">Application</span></span>|<span data-ttu-id="c9c86-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9c86-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c9c86-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c9c86-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificateForClientValidation
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows81SCEPCertificateProfile/rootCertificate
```

## <a name="request-headers"></a><span data-ttu-id="c9c86-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c9c86-120">Request headers</span></span>
|<span data-ttu-id="c9c86-121">标头</span><span class="sxs-lookup"><span data-stu-id="c9c86-121">Header</span></span>|<span data-ttu-id="c9c86-122">值</span><span class="sxs-lookup"><span data-stu-id="c9c86-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c9c86-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c9c86-123">Authorization</span></span>|<span data-ttu-id="c9c86-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c9c86-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c9c86-125">接受</span><span class="sxs-lookup"><span data-stu-id="c9c86-125">Accept</span></span>|<span data-ttu-id="c9c86-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c9c86-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c9c86-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c9c86-127">Request body</span></span>
<span data-ttu-id="c9c86-128">在请求正文中，提供 [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c9c86-128">In the request body, supply a JSON representation for the [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) object.</span></span>

<span data-ttu-id="c9c86-129">下表显示创建 [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c9c86-129">The following table shows the properties that are required when you create the [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md).</span></span>

|<span data-ttu-id="c9c86-130">属性</span><span class="sxs-lookup"><span data-stu-id="c9c86-130">Property</span></span>|<span data-ttu-id="c9c86-131">类型</span><span class="sxs-lookup"><span data-stu-id="c9c86-131">Type</span></span>|<span data-ttu-id="c9c86-132">说明</span><span class="sxs-lookup"><span data-stu-id="c9c86-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9c86-133">id</span><span class="sxs-lookup"><span data-stu-id="c9c86-133">id</span></span>|<span data-ttu-id="c9c86-134">String</span><span class="sxs-lookup"><span data-stu-id="c9c86-134">String</span></span>|<span data-ttu-id="c9c86-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c9c86-135">Key of the entity.</span></span> <span data-ttu-id="c9c86-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c9c86-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9c86-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c9c86-137">lastModifiedDateTime</span></span>|<span data-ttu-id="c9c86-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9c86-138">DateTimeOffset</span></span>|<span data-ttu-id="c9c86-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c9c86-139">DateTime the object was last modified.</span></span> <span data-ttu-id="c9c86-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c9c86-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9c86-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c9c86-141">roleScopeTagIds</span></span>|<span data-ttu-id="c9c86-142">String collection</span><span class="sxs-lookup"><span data-stu-id="c9c86-142">String collection</span></span>|<span data-ttu-id="c9c86-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="c9c86-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c9c86-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c9c86-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9c86-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c9c86-145">supportsScopeTags</span></span>|<span data-ttu-id="c9c86-146">布尔</span><span class="sxs-lookup"><span data-stu-id="c9c86-146">Boolean</span></span>|<span data-ttu-id="c9c86-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="c9c86-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c9c86-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="c9c86-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c9c86-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="c9c86-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c9c86-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c9c86-150">This property is read-only.</span></span> <span data-ttu-id="c9c86-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c9c86-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9c86-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c9c86-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="c9c86-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c9c86-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="c9c86-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="c9c86-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="c9c86-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c9c86-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9c86-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c9c86-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="c9c86-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c9c86-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="c9c86-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="c9c86-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="c9c86-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c9c86-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9c86-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c9c86-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="c9c86-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c9c86-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="c9c86-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="c9c86-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="c9c86-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c9c86-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9c86-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c9c86-164">createdDateTime</span></span>|<span data-ttu-id="c9c86-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9c86-165">DateTimeOffset</span></span>|<span data-ttu-id="c9c86-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c9c86-166">DateTime the object was created.</span></span> <span data-ttu-id="c9c86-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c9c86-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9c86-168">说明</span><span class="sxs-lookup"><span data-stu-id="c9c86-168">description</span></span>|<span data-ttu-id="c9c86-169">String</span><span class="sxs-lookup"><span data-stu-id="c9c86-169">String</span></span>|<span data-ttu-id="c9c86-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="c9c86-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c9c86-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c9c86-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9c86-172">displayName</span><span class="sxs-lookup"><span data-stu-id="c9c86-172">displayName</span></span>|<span data-ttu-id="c9c86-173">String</span><span class="sxs-lookup"><span data-stu-id="c9c86-173">String</span></span>|<span data-ttu-id="c9c86-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="c9c86-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c9c86-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c9c86-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9c86-176">version</span><span class="sxs-lookup"><span data-stu-id="c9c86-176">version</span></span>|<span data-ttu-id="c9c86-177">Int32</span><span class="sxs-lookup"><span data-stu-id="c9c86-177">Int32</span></span>|<span data-ttu-id="c9c86-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="c9c86-178">Version of the device configuration.</span></span> <span data-ttu-id="c9c86-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c9c86-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9c86-180">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="c9c86-180">trustedRootCertificate</span></span>|<span data-ttu-id="c9c86-181">Binary</span><span class="sxs-lookup"><span data-stu-id="c9c86-181">Binary</span></span>|<span data-ttu-id="c9c86-182">受信任的根证书</span><span class="sxs-lookup"><span data-stu-id="c9c86-182">Trusted Root Certificate</span></span>|
|<span data-ttu-id="c9c86-183">certFileName</span><span class="sxs-lookup"><span data-stu-id="c9c86-183">certFileName</span></span>|<span data-ttu-id="c9c86-184">String</span><span class="sxs-lookup"><span data-stu-id="c9c86-184">String</span></span>|<span data-ttu-id="c9c86-185">要在 UI 中显示的文件名。</span><span class="sxs-lookup"><span data-stu-id="c9c86-185">File name to display in UI.</span></span>|
|<span data-ttu-id="c9c86-186">destinationStore</span><span class="sxs-lookup"><span data-stu-id="c9c86-186">destinationStore</span></span>|[<span data-ttu-id="c9c86-187">certificateDestinationStore</span><span class="sxs-lookup"><span data-stu-id="c9c86-187">certificateDestinationStore</span></span>](../resources/intune-deviceconfig-certificatedestinationstore.md)|<span data-ttu-id="c9c86-188">受信任的根证书的目标存储位置。</span><span class="sxs-lookup"><span data-stu-id="c9c86-188">Destination store location for the Trusted Root Certificate.</span></span> <span data-ttu-id="c9c86-189">可取值为：`computerCertStoreRoot`、`computerCertStoreIntermediate`、`userCertStoreIntermediate`。</span><span class="sxs-lookup"><span data-stu-id="c9c86-189">Possible values are: `computerCertStoreRoot`, `computerCertStoreIntermediate`, `userCertStoreIntermediate`.</span></span>|



## <a name="response"></a><span data-ttu-id="c9c86-190">响应</span><span class="sxs-lookup"><span data-stu-id="c9c86-190">Response</span></span>
<span data-ttu-id="c9c86-191">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c9c86-191">If successful, this method returns a `200 OK` response code and an updated [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9c86-192">示例</span><span class="sxs-lookup"><span data-stu-id="c9c86-192">Example</span></span>

### <a name="request"></a><span data-ttu-id="c9c86-193">请求</span><span class="sxs-lookup"><span data-stu-id="c9c86-193">Request</span></span>
<span data-ttu-id="c9c86-194">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c9c86-194">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c9c86-195">响应</span><span class="sxs-lookup"><span data-stu-id="c9c86-195">Response</span></span>
<span data-ttu-id="c9c86-p114">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c9c86-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





