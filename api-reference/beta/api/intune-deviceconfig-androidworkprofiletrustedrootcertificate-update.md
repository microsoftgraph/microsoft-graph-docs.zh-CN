---
title: 更新 androidWorkProfileTrustedRootCertificate
description: 更新 androidWorkProfileTrustedRootCertificate 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ab74f91843d6fb1ee267ca24b10773393d28e3e8
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39949901"
---
# <a name="update-androidworkprofiletrustedrootcertificate"></a><span data-ttu-id="9a8af-103">更新 androidWorkProfileTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="9a8af-103">Update androidWorkProfileTrustedRootCertificate</span></span>

> <span data-ttu-id="9a8af-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9a8af-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9a8af-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9a8af-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9a8af-106">更新[androidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9a8af-106">Update the properties of a [androidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9a8af-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="9a8af-107">Prerequisites</span></span>
<span data-ttu-id="9a8af-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9a8af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a8af-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="9a8af-110">Permission type</span></span>|<span data-ttu-id="9a8af-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9a8af-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9a8af-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9a8af-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9a8af-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a8af-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9a8af-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9a8af-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9a8af-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9a8af-115">Not supported.</span></span>|
|<span data-ttu-id="9a8af-116">Application</span><span class="sxs-lookup"><span data-stu-id="9a8af-116">Application</span></span>|<span data-ttu-id="9a8af-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a8af-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9a8af-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9a8af-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidWorkProfileCertificateProfileBase/rootCertificate
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidWorkProfileEnterpriseWiFiConfiguration/rootCertificateForServerValidation
```

## <a name="request-headers"></a><span data-ttu-id="9a8af-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="9a8af-119">Request headers</span></span>
|<span data-ttu-id="9a8af-120">标头</span><span class="sxs-lookup"><span data-stu-id="9a8af-120">Header</span></span>|<span data-ttu-id="9a8af-121">值</span><span class="sxs-lookup"><span data-stu-id="9a8af-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9a8af-122">授权</span><span class="sxs-lookup"><span data-stu-id="9a8af-122">Authorization</span></span>|<span data-ttu-id="9a8af-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9a8af-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9a8af-124">接受</span><span class="sxs-lookup"><span data-stu-id="9a8af-124">Accept</span></span>|<span data-ttu-id="9a8af-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9a8af-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9a8af-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="9a8af-126">Request body</span></span>
<span data-ttu-id="9a8af-127">在请求正文中，提供[androidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9a8af-127">In the request body, supply a JSON representation for the [androidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md) object.</span></span>

<span data-ttu-id="9a8af-128">下表显示创建[androidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="9a8af-128">The following table shows the properties that are required when you create the [androidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md).</span></span>

|<span data-ttu-id="9a8af-129">属性</span><span class="sxs-lookup"><span data-stu-id="9a8af-129">Property</span></span>|<span data-ttu-id="9a8af-130">类型</span><span class="sxs-lookup"><span data-stu-id="9a8af-130">Type</span></span>|<span data-ttu-id="9a8af-131">说明</span><span class="sxs-lookup"><span data-stu-id="9a8af-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a8af-132">id</span><span class="sxs-lookup"><span data-stu-id="9a8af-132">id</span></span>|<span data-ttu-id="9a8af-133">字符串</span><span class="sxs-lookup"><span data-stu-id="9a8af-133">String</span></span>|<span data-ttu-id="9a8af-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="9a8af-134">Key of the entity.</span></span> <span data-ttu-id="9a8af-135">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9a8af-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9a8af-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9a8af-136">lastModifiedDateTime</span></span>|<span data-ttu-id="9a8af-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a8af-137">DateTimeOffset</span></span>|<span data-ttu-id="9a8af-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="9a8af-138">DateTime the object was last modified.</span></span> <span data-ttu-id="9a8af-139">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9a8af-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9a8af-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9a8af-140">roleScopeTagIds</span></span>|<span data-ttu-id="9a8af-141">String collection</span><span class="sxs-lookup"><span data-stu-id="9a8af-141">String collection</span></span>|<span data-ttu-id="9a8af-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="9a8af-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9a8af-143">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9a8af-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9a8af-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="9a8af-144">supportsScopeTags</span></span>|<span data-ttu-id="9a8af-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="9a8af-145">Boolean</span></span>|<span data-ttu-id="9a8af-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="9a8af-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="9a8af-147">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="9a8af-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="9a8af-148">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="9a8af-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="9a8af-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9a8af-149">This property is read-only.</span></span> <span data-ttu-id="9a8af-150">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9a8af-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9a8af-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="9a8af-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="9a8af-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="9a8af-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="9a8af-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="9a8af-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="9a8af-154">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9a8af-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9a8af-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="9a8af-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="9a8af-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="9a8af-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="9a8af-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="9a8af-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="9a8af-158">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9a8af-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9a8af-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="9a8af-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="9a8af-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="9a8af-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="9a8af-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="9a8af-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="9a8af-162">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9a8af-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9a8af-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9a8af-163">createdDateTime</span></span>|<span data-ttu-id="9a8af-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a8af-164">DateTimeOffset</span></span>|<span data-ttu-id="9a8af-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="9a8af-165">DateTime the object was created.</span></span> <span data-ttu-id="9a8af-166">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9a8af-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9a8af-167">说明</span><span class="sxs-lookup"><span data-stu-id="9a8af-167">description</span></span>|<span data-ttu-id="9a8af-168">String</span><span class="sxs-lookup"><span data-stu-id="9a8af-168">String</span></span>|<span data-ttu-id="9a8af-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="9a8af-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9a8af-170">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9a8af-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9a8af-171">displayName</span><span class="sxs-lookup"><span data-stu-id="9a8af-171">displayName</span></span>|<span data-ttu-id="9a8af-172">String</span><span class="sxs-lookup"><span data-stu-id="9a8af-172">String</span></span>|<span data-ttu-id="9a8af-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="9a8af-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9a8af-174">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9a8af-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9a8af-175">version</span><span class="sxs-lookup"><span data-stu-id="9a8af-175">version</span></span>|<span data-ttu-id="9a8af-176">Int32</span><span class="sxs-lookup"><span data-stu-id="9a8af-176">Int32</span></span>|<span data-ttu-id="9a8af-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="9a8af-177">Version of the device configuration.</span></span> <span data-ttu-id="9a8af-178">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9a8af-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9a8af-179">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="9a8af-179">trustedRootCertificate</span></span>|<span data-ttu-id="9a8af-180">Binary</span><span class="sxs-lookup"><span data-stu-id="9a8af-180">Binary</span></span>|<span data-ttu-id="9a8af-181">受信任的根证书</span><span class="sxs-lookup"><span data-stu-id="9a8af-181">Trusted Root Certificate</span></span>|
|<span data-ttu-id="9a8af-182">certFileName</span><span class="sxs-lookup"><span data-stu-id="9a8af-182">certFileName</span></span>|<span data-ttu-id="9a8af-183">字符串</span><span class="sxs-lookup"><span data-stu-id="9a8af-183">String</span></span>|<span data-ttu-id="9a8af-184">要在 UI 中显示的文件名。</span><span class="sxs-lookup"><span data-stu-id="9a8af-184">File name to display in UI.</span></span>|



## <a name="response"></a><span data-ttu-id="9a8af-185">响应</span><span class="sxs-lookup"><span data-stu-id="9a8af-185">Response</span></span>
<span data-ttu-id="9a8af-186">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[androidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9a8af-186">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9a8af-187">示例</span><span class="sxs-lookup"><span data-stu-id="9a8af-187">Example</span></span>

### <a name="request"></a><span data-ttu-id="9a8af-188">请求</span><span class="sxs-lookup"><span data-stu-id="9a8af-188">Request</span></span>
<span data-ttu-id="9a8af-189">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9a8af-189">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate
Content-type: application/json
Content-length: 1151

{
  "@odata.type": "#microsoft.graph.androidWorkProfileTrustedRootCertificate",
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

### <a name="response"></a><span data-ttu-id="9a8af-190">响应</span><span class="sxs-lookup"><span data-stu-id="9a8af-190">Response</span></span>
<span data-ttu-id="9a8af-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9a8af-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1323

{
  "@odata.type": "#microsoft.graph.androidWorkProfileTrustedRootCertificate",
  "id": "37cc7454-7454-37cc-5474-cc375474cc37",
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





