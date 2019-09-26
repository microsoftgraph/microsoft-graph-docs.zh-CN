---
title: 更新 androidForWorkTrustedRootCertificate
description: 更新 androidForWorkTrustedRootCertificate 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a4ea0b8e48bc10881369cfcc67bbbae7fecbad97
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37176343"
---
# <a name="update-androidforworktrustedrootcertificate"></a><span data-ttu-id="64816-103">更新 androidForWorkTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="64816-103">Update androidForWorkTrustedRootCertificate</span></span>

> <span data-ttu-id="64816-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="64816-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="64816-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="64816-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64816-106">更新[androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="64816-106">Update the properties of a [androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="64816-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="64816-107">Prerequisites</span></span>
<span data-ttu-id="64816-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="64816-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64816-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="64816-110">Permission type</span></span>|<span data-ttu-id="64816-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="64816-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="64816-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="64816-112">Delegated (work or school account)</span></span>|<span data-ttu-id="64816-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64816-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="64816-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="64816-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="64816-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="64816-115">Not supported.</span></span>|
|<span data-ttu-id="64816-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="64816-116">Application</span></span>|<span data-ttu-id="64816-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64816-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="64816-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="64816-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidForWorkEnterpriseWiFiConfiguration/rootCertificateForServerValidation
```

## <a name="request-headers"></a><span data-ttu-id="64816-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="64816-119">Request headers</span></span>
|<span data-ttu-id="64816-120">标头</span><span class="sxs-lookup"><span data-stu-id="64816-120">Header</span></span>|<span data-ttu-id="64816-121">值</span><span class="sxs-lookup"><span data-stu-id="64816-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="64816-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="64816-122">Authorization</span></span>|<span data-ttu-id="64816-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="64816-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="64816-124">接受</span><span class="sxs-lookup"><span data-stu-id="64816-124">Accept</span></span>|<span data-ttu-id="64816-125">application/json</span><span class="sxs-lookup"><span data-stu-id="64816-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="64816-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="64816-126">Request body</span></span>
<span data-ttu-id="64816-127">在请求正文中，提供[androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="64816-127">In the request body, supply a JSON representation for the [androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md) object.</span></span>

<span data-ttu-id="64816-128">下表显示创建[androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="64816-128">The following table shows the properties that are required when you create the [androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md).</span></span>

|<span data-ttu-id="64816-129">属性</span><span class="sxs-lookup"><span data-stu-id="64816-129">Property</span></span>|<span data-ttu-id="64816-130">类型</span><span class="sxs-lookup"><span data-stu-id="64816-130">Type</span></span>|<span data-ttu-id="64816-131">说明</span><span class="sxs-lookup"><span data-stu-id="64816-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64816-132">id</span><span class="sxs-lookup"><span data-stu-id="64816-132">id</span></span>|<span data-ttu-id="64816-133">字符串</span><span class="sxs-lookup"><span data-stu-id="64816-133">String</span></span>|<span data-ttu-id="64816-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="64816-134">Key of the entity.</span></span> <span data-ttu-id="64816-135">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64816-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64816-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="64816-136">lastModifiedDateTime</span></span>|<span data-ttu-id="64816-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64816-137">DateTimeOffset</span></span>|<span data-ttu-id="64816-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="64816-138">DateTime the object was last modified.</span></span> <span data-ttu-id="64816-139">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64816-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64816-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="64816-140">roleScopeTagIds</span></span>|<span data-ttu-id="64816-141">String collection</span><span class="sxs-lookup"><span data-stu-id="64816-141">String collection</span></span>|<span data-ttu-id="64816-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="64816-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="64816-143">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64816-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64816-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="64816-144">supportsScopeTags</span></span>|<span data-ttu-id="64816-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="64816-145">Boolean</span></span>|<span data-ttu-id="64816-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="64816-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="64816-147">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="64816-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="64816-148">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="64816-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="64816-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="64816-149">This property is read-only.</span></span> <span data-ttu-id="64816-150">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64816-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64816-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="64816-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="64816-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="64816-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="64816-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="64816-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="64816-154">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64816-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64816-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="64816-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="64816-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="64816-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="64816-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="64816-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="64816-158">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64816-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64816-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="64816-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="64816-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="64816-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="64816-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="64816-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="64816-162">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64816-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64816-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="64816-163">createdDateTime</span></span>|<span data-ttu-id="64816-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64816-164">DateTimeOffset</span></span>|<span data-ttu-id="64816-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="64816-165">DateTime the object was created.</span></span> <span data-ttu-id="64816-166">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64816-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64816-167">说明</span><span class="sxs-lookup"><span data-stu-id="64816-167">description</span></span>|<span data-ttu-id="64816-168">String</span><span class="sxs-lookup"><span data-stu-id="64816-168">String</span></span>|<span data-ttu-id="64816-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="64816-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="64816-170">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64816-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64816-171">displayName</span><span class="sxs-lookup"><span data-stu-id="64816-171">displayName</span></span>|<span data-ttu-id="64816-172">String</span><span class="sxs-lookup"><span data-stu-id="64816-172">String</span></span>|<span data-ttu-id="64816-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="64816-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="64816-174">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64816-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64816-175">version</span><span class="sxs-lookup"><span data-stu-id="64816-175">version</span></span>|<span data-ttu-id="64816-176">Int32</span><span class="sxs-lookup"><span data-stu-id="64816-176">Int32</span></span>|<span data-ttu-id="64816-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="64816-177">Version of the device configuration.</span></span> <span data-ttu-id="64816-178">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64816-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64816-179">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="64816-179">trustedRootCertificate</span></span>|<span data-ttu-id="64816-180">Binary</span><span class="sxs-lookup"><span data-stu-id="64816-180">Binary</span></span>|<span data-ttu-id="64816-181">受信任的根证书</span><span class="sxs-lookup"><span data-stu-id="64816-181">Trusted Root Certificate</span></span>|
|<span data-ttu-id="64816-182">certFileName</span><span class="sxs-lookup"><span data-stu-id="64816-182">certFileName</span></span>|<span data-ttu-id="64816-183">String</span><span class="sxs-lookup"><span data-stu-id="64816-183">String</span></span>|<span data-ttu-id="64816-184">要在 UI 中显示的文件名。</span><span class="sxs-lookup"><span data-stu-id="64816-184">File name to display in UI.</span></span>|



## <a name="response"></a><span data-ttu-id="64816-185">响应</span><span class="sxs-lookup"><span data-stu-id="64816-185">Response</span></span>
<span data-ttu-id="64816-186">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="64816-186">If successful, this method returns a `200 OK` response code and an updated [androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64816-187">示例</span><span class="sxs-lookup"><span data-stu-id="64816-187">Example</span></span>

### <a name="request"></a><span data-ttu-id="64816-188">请求</span><span class="sxs-lookup"><span data-stu-id="64816-188">Request</span></span>
<span data-ttu-id="64816-189">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="64816-189">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate
Content-type: application/json
Content-length: 1147

{
  "@odata.type": "#microsoft.graph.androidForWorkTrustedRootCertificate",
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

### <a name="response"></a><span data-ttu-id="64816-190">响应</span><span class="sxs-lookup"><span data-stu-id="64816-190">Response</span></span>
<span data-ttu-id="64816-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="64816-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1319

{
  "@odata.type": "#microsoft.graph.androidForWorkTrustedRootCertificate",
  "id": "2f78834c-834c-2f78-4c83-782f4c83782f",
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




