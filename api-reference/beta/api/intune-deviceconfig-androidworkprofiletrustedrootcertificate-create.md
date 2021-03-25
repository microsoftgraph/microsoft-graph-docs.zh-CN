---
title: 创建 androidWorkProfileTrustedRootCertificate
description: 创建新的 androidWorkProfileTrustedRootCertificate 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2d64040452817d7278e774280db4b2cef2a65e59
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51151653"
---
# <a name="create-androidworkprofiletrustedrootcertificate"></a><span data-ttu-id="d0f12-103">创建 androidWorkProfileTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="d0f12-103">Create androidWorkProfileTrustedRootCertificate</span></span>

<span data-ttu-id="d0f12-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d0f12-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d0f12-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d0f12-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d0f12-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d0f12-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d0f12-107">创建新的 [androidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d0f12-107">Create a new [androidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d0f12-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="d0f12-108">Prerequisites</span></span>
<span data-ttu-id="d0f12-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d0f12-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0f12-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d0f12-111">Permission type</span></span>|<span data-ttu-id="d0f12-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d0f12-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d0f12-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d0f12-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d0f12-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0f12-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d0f12-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d0f12-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d0f12-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d0f12-116">Not supported.</span></span>|
|<span data-ttu-id="d0f12-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d0f12-117">Application</span></span>|<span data-ttu-id="d0f12-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0f12-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d0f12-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d0f12-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d0f12-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d0f12-120">Request headers</span></span>
|<span data-ttu-id="d0f12-121">标头</span><span class="sxs-lookup"><span data-stu-id="d0f12-121">Header</span></span>|<span data-ttu-id="d0f12-122">值</span><span class="sxs-lookup"><span data-stu-id="d0f12-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d0f12-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d0f12-123">Authorization</span></span>|<span data-ttu-id="d0f12-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d0f12-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d0f12-125">接受</span><span class="sxs-lookup"><span data-stu-id="d0f12-125">Accept</span></span>|<span data-ttu-id="d0f12-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d0f12-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d0f12-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d0f12-127">Request body</span></span>
<span data-ttu-id="d0f12-128">在请求正文中，提供 androidWorkProfileTrustedRootCertificate 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d0f12-128">In the request body, supply a JSON representation for the androidWorkProfileTrustedRootCertificate object.</span></span>

<span data-ttu-id="d0f12-129">下表显示创建 androidWorkProfileTrustedRootCertificate 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d0f12-129">The following table shows the properties that are required when you create the androidWorkProfileTrustedRootCertificate.</span></span>

|<span data-ttu-id="d0f12-130">属性</span><span class="sxs-lookup"><span data-stu-id="d0f12-130">Property</span></span>|<span data-ttu-id="d0f12-131">类型</span><span class="sxs-lookup"><span data-stu-id="d0f12-131">Type</span></span>|<span data-ttu-id="d0f12-132">说明</span><span class="sxs-lookup"><span data-stu-id="d0f12-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0f12-133">id</span><span class="sxs-lookup"><span data-stu-id="d0f12-133">id</span></span>|<span data-ttu-id="d0f12-134">String</span><span class="sxs-lookup"><span data-stu-id="d0f12-134">String</span></span>|<span data-ttu-id="d0f12-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d0f12-135">Key of the entity.</span></span> <span data-ttu-id="d0f12-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d0f12-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0f12-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d0f12-137">lastModifiedDateTime</span></span>|<span data-ttu-id="d0f12-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0f12-138">DateTimeOffset</span></span>|<span data-ttu-id="d0f12-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="d0f12-139">DateTime the object was last modified.</span></span> <span data-ttu-id="d0f12-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d0f12-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0f12-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d0f12-141">roleScopeTagIds</span></span>|<span data-ttu-id="d0f12-142">String collection</span><span class="sxs-lookup"><span data-stu-id="d0f12-142">String collection</span></span>|<span data-ttu-id="d0f12-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="d0f12-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d0f12-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d0f12-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0f12-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d0f12-145">supportsScopeTags</span></span>|<span data-ttu-id="d0f12-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0f12-146">Boolean</span></span>|<span data-ttu-id="d0f12-147">指示基础设备配置是否支持分配范围标记。</span><span class="sxs-lookup"><span data-stu-id="d0f12-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d0f12-148">当此值为 false 且实体对作用域用户不可见时，不允许分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="d0f12-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d0f12-149">这适用于在 Silverlight 中创建的旧版策略，可通过在 Azure 门户中删除和重新创建策略来解决。</span><span class="sxs-lookup"><span data-stu-id="d0f12-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d0f12-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="d0f12-150">This property is read-only.</span></span> <span data-ttu-id="d0f12-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d0f12-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0f12-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d0f12-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="d0f12-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d0f12-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="d0f12-154">此策略的操作系统版本适用性。</span><span class="sxs-lookup"><span data-stu-id="d0f12-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="d0f12-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d0f12-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0f12-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d0f12-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="d0f12-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d0f12-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="d0f12-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="d0f12-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="d0f12-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d0f12-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0f12-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="d0f12-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="d0f12-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="d0f12-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="d0f12-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="d0f12-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="d0f12-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d0f12-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0f12-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d0f12-164">createdDateTime</span></span>|<span data-ttu-id="d0f12-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0f12-165">DateTimeOffset</span></span>|<span data-ttu-id="d0f12-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="d0f12-166">DateTime the object was created.</span></span> <span data-ttu-id="d0f12-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d0f12-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0f12-168">说明</span><span class="sxs-lookup"><span data-stu-id="d0f12-168">description</span></span>|<span data-ttu-id="d0f12-169">String</span><span class="sxs-lookup"><span data-stu-id="d0f12-169">String</span></span>|<span data-ttu-id="d0f12-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="d0f12-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d0f12-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d0f12-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0f12-172">displayName</span><span class="sxs-lookup"><span data-stu-id="d0f12-172">displayName</span></span>|<span data-ttu-id="d0f12-173">String</span><span class="sxs-lookup"><span data-stu-id="d0f12-173">String</span></span>|<span data-ttu-id="d0f12-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="d0f12-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d0f12-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d0f12-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0f12-176">version</span><span class="sxs-lookup"><span data-stu-id="d0f12-176">version</span></span>|<span data-ttu-id="d0f12-177">Int32</span><span class="sxs-lookup"><span data-stu-id="d0f12-177">Int32</span></span>|<span data-ttu-id="d0f12-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="d0f12-178">Version of the device configuration.</span></span> <span data-ttu-id="d0f12-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d0f12-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0f12-180">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="d0f12-180">trustedRootCertificate</span></span>|<span data-ttu-id="d0f12-181">Binary</span><span class="sxs-lookup"><span data-stu-id="d0f12-181">Binary</span></span>|<span data-ttu-id="d0f12-182">受信任的根证书</span><span class="sxs-lookup"><span data-stu-id="d0f12-182">Trusted Root Certificate</span></span>|
|<span data-ttu-id="d0f12-183">certFileName</span><span class="sxs-lookup"><span data-stu-id="d0f12-183">certFileName</span></span>|<span data-ttu-id="d0f12-184">String</span><span class="sxs-lookup"><span data-stu-id="d0f12-184">String</span></span>|<span data-ttu-id="d0f12-185">要显示在 UI 中的文件名。</span><span class="sxs-lookup"><span data-stu-id="d0f12-185">File name to display in UI.</span></span>|



## <a name="response"></a><span data-ttu-id="d0f12-186">响应</span><span class="sxs-lookup"><span data-stu-id="d0f12-186">Response</span></span>
<span data-ttu-id="d0f12-187">如果成功，此方法在响应正文 `201 Created` 中返回 响应代码和 [androidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d0f12-187">If successful, this method returns a `201 Created` response code and a [androidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d0f12-188">示例</span><span class="sxs-lookup"><span data-stu-id="d0f12-188">Example</span></span>

### <a name="request"></a><span data-ttu-id="d0f12-189">请求</span><span class="sxs-lookup"><span data-stu-id="d0f12-189">Request</span></span>
<span data-ttu-id="d0f12-190">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d0f12-190">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="d0f12-191">响应</span><span class="sxs-lookup"><span data-stu-id="d0f12-191">Response</span></span>
<span data-ttu-id="d0f12-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d0f12-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




