---
title: 更新 windowsPhone81TrustedRootCertificate
description: 更新 windowsPhone81TrustedRootCertificate 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e718391c07a0b4e1698b2671501a6ef5b12cd2e0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47972390"
---
# <a name="update-windowsphone81trustedrootcertificate"></a><span data-ttu-id="a46da-103">更新 windowsPhone81TrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="a46da-103">Update windowsPhone81TrustedRootCertificate</span></span>

<span data-ttu-id="a46da-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a46da-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a46da-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a46da-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a46da-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a46da-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a46da-107">更新 [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a46da-107">Update the properties of a [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a46da-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="a46da-108">Prerequisites</span></span>
<span data-ttu-id="a46da-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a46da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a46da-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a46da-111">Permission type</span></span>|<span data-ttu-id="a46da-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a46da-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a46da-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a46da-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a46da-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a46da-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a46da-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a46da-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a46da-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a46da-116">Not supported.</span></span>|
|<span data-ttu-id="a46da-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a46da-117">Application</span></span>|<span data-ttu-id="a46da-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a46da-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a46da-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a46da-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/microsoft.graph.windowsPhone81SCEPCertificateProfile/rootCertificate
```

## <a name="request-headers"></a><span data-ttu-id="a46da-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a46da-120">Request headers</span></span>
|<span data-ttu-id="a46da-121">标头</span><span class="sxs-lookup"><span data-stu-id="a46da-121">Header</span></span>|<span data-ttu-id="a46da-122">值</span><span class="sxs-lookup"><span data-stu-id="a46da-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a46da-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a46da-123">Authorization</span></span>|<span data-ttu-id="a46da-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a46da-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a46da-125">接受</span><span class="sxs-lookup"><span data-stu-id="a46da-125">Accept</span></span>|<span data-ttu-id="a46da-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a46da-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a46da-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a46da-127">Request body</span></span>
<span data-ttu-id="a46da-128">在请求正文中，提供 [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a46da-128">In the request body, supply a JSON representation for the [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) object.</span></span>

<span data-ttu-id="a46da-129">下表显示创建 [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a46da-129">The following table shows the properties that are required when you create the [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md).</span></span>

|<span data-ttu-id="a46da-130">属性</span><span class="sxs-lookup"><span data-stu-id="a46da-130">Property</span></span>|<span data-ttu-id="a46da-131">类型</span><span class="sxs-lookup"><span data-stu-id="a46da-131">Type</span></span>|<span data-ttu-id="a46da-132">说明</span><span class="sxs-lookup"><span data-stu-id="a46da-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a46da-133">id</span><span class="sxs-lookup"><span data-stu-id="a46da-133">id</span></span>|<span data-ttu-id="a46da-134">String</span><span class="sxs-lookup"><span data-stu-id="a46da-134">String</span></span>|<span data-ttu-id="a46da-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a46da-135">Key of the entity.</span></span> <span data-ttu-id="a46da-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a46da-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a46da-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a46da-137">lastModifiedDateTime</span></span>|<span data-ttu-id="a46da-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a46da-138">DateTimeOffset</span></span>|<span data-ttu-id="a46da-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="a46da-139">DateTime the object was last modified.</span></span> <span data-ttu-id="a46da-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a46da-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a46da-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a46da-141">roleScopeTagIds</span></span>|<span data-ttu-id="a46da-142">String collection</span><span class="sxs-lookup"><span data-stu-id="a46da-142">String collection</span></span>|<span data-ttu-id="a46da-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="a46da-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a46da-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a46da-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a46da-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a46da-145">supportsScopeTags</span></span>|<span data-ttu-id="a46da-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="a46da-146">Boolean</span></span>|<span data-ttu-id="a46da-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="a46da-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a46da-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="a46da-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a46da-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="a46da-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a46da-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="a46da-150">This property is read-only.</span></span> <span data-ttu-id="a46da-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a46da-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a46da-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a46da-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="a46da-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a46da-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="a46da-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="a46da-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="a46da-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a46da-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a46da-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a46da-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="a46da-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a46da-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="a46da-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="a46da-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="a46da-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a46da-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a46da-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a46da-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="a46da-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a46da-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="a46da-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="a46da-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="a46da-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a46da-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a46da-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a46da-164">createdDateTime</span></span>|<span data-ttu-id="a46da-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a46da-165">DateTimeOffset</span></span>|<span data-ttu-id="a46da-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="a46da-166">DateTime the object was created.</span></span> <span data-ttu-id="a46da-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a46da-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a46da-168">description</span><span class="sxs-lookup"><span data-stu-id="a46da-168">description</span></span>|<span data-ttu-id="a46da-169">String</span><span class="sxs-lookup"><span data-stu-id="a46da-169">String</span></span>|<span data-ttu-id="a46da-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="a46da-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a46da-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a46da-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a46da-172">displayName</span><span class="sxs-lookup"><span data-stu-id="a46da-172">displayName</span></span>|<span data-ttu-id="a46da-173">String</span><span class="sxs-lookup"><span data-stu-id="a46da-173">String</span></span>|<span data-ttu-id="a46da-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="a46da-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a46da-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a46da-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a46da-176">version</span><span class="sxs-lookup"><span data-stu-id="a46da-176">version</span></span>|<span data-ttu-id="a46da-177">Int32</span><span class="sxs-lookup"><span data-stu-id="a46da-177">Int32</span></span>|<span data-ttu-id="a46da-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="a46da-178">Version of the device configuration.</span></span> <span data-ttu-id="a46da-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a46da-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a46da-180">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="a46da-180">trustedRootCertificate</span></span>|<span data-ttu-id="a46da-181">Binary</span><span class="sxs-lookup"><span data-stu-id="a46da-181">Binary</span></span>|<span data-ttu-id="a46da-182">受信任的根证书</span><span class="sxs-lookup"><span data-stu-id="a46da-182">Trusted Root Certificate</span></span>|
|<span data-ttu-id="a46da-183">certFileName</span><span class="sxs-lookup"><span data-stu-id="a46da-183">certFileName</span></span>|<span data-ttu-id="a46da-184">String</span><span class="sxs-lookup"><span data-stu-id="a46da-184">String</span></span>|<span data-ttu-id="a46da-185">要在 UI 中显示的文件名。</span><span class="sxs-lookup"><span data-stu-id="a46da-185">File name to display in UI.</span></span>|



## <a name="response"></a><span data-ttu-id="a46da-186">响应</span><span class="sxs-lookup"><span data-stu-id="a46da-186">Response</span></span>
<span data-ttu-id="a46da-187">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a46da-187">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a46da-188">示例</span><span class="sxs-lookup"><span data-stu-id="a46da-188">Example</span></span>

### <a name="request"></a><span data-ttu-id="a46da-189">请求</span><span class="sxs-lookup"><span data-stu-id="a46da-189">Request</span></span>
<span data-ttu-id="a46da-190">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a46da-190">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/microsoft.graph.windowsPhone81SCEPCertificateProfile/rootCertificate
Content-type: application/json
Content-length: 1147

{
  "@odata.type": "#microsoft.graph.windowsPhone81TrustedRootCertificate",
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

### <a name="response"></a><span data-ttu-id="a46da-191">响应</span><span class="sxs-lookup"><span data-stu-id="a46da-191">Response</span></span>
<span data-ttu-id="a46da-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a46da-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1319

{
  "@odata.type": "#microsoft.graph.windowsPhone81TrustedRootCertificate",
  "id": "6316bf01-bf01-6316-01bf-166301bf1663",
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






