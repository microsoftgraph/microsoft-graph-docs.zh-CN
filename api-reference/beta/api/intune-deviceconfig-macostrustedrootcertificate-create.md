---
title: 创建 macOSTrustedRootCertificate
description: 创建新的 macOSTrustedRootCertificate 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 19a6ef8607199425691cb635c912bbd825382f38
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792778"
---
# <a name="create-macostrustedrootcertificate"></a><span data-ttu-id="e0546-103">创建 macOSTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="e0546-103">Create macOSTrustedRootCertificate</span></span>

<span data-ttu-id="e0546-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e0546-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e0546-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e0546-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e0546-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e0546-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e0546-107">创建新的[macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e0546-107">Create a new [macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e0546-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="e0546-108">Prerequisites</span></span>
<span data-ttu-id="e0546-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="e0546-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="e0546-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0546-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0546-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e0546-111">Permission type</span></span>|<span data-ttu-id="e0546-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e0546-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e0546-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e0546-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e0546-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0546-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e0546-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e0546-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e0546-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e0546-116">Not supported.</span></span>|
|<span data-ttu-id="e0546-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e0546-117">Application</span></span>|<span data-ttu-id="e0546-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0546-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e0546-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e0546-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSEnterpriseWiFiConfiguration/rootCertificatesForServerValidation
```

## <a name="request-headers"></a><span data-ttu-id="e0546-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e0546-120">Request headers</span></span>
|<span data-ttu-id="e0546-121">标头</span><span class="sxs-lookup"><span data-stu-id="e0546-121">Header</span></span>|<span data-ttu-id="e0546-122">值</span><span class="sxs-lookup"><span data-stu-id="e0546-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e0546-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e0546-123">Authorization</span></span>|<span data-ttu-id="e0546-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e0546-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e0546-125">接受</span><span class="sxs-lookup"><span data-stu-id="e0546-125">Accept</span></span>|<span data-ttu-id="e0546-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e0546-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e0546-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e0546-127">Request body</span></span>
<span data-ttu-id="e0546-128">在请求正文中，提供 macOSTrustedRootCertificate 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e0546-128">In the request body, supply a JSON representation for the macOSTrustedRootCertificate object.</span></span>

<span data-ttu-id="e0546-129">下表显示创建 macOSTrustedRootCertificate 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e0546-129">The following table shows the properties that are required when you create the macOSTrustedRootCertificate.</span></span>

|<span data-ttu-id="e0546-130">属性</span><span class="sxs-lookup"><span data-stu-id="e0546-130">Property</span></span>|<span data-ttu-id="e0546-131">类型</span><span class="sxs-lookup"><span data-stu-id="e0546-131">Type</span></span>|<span data-ttu-id="e0546-132">说明</span><span class="sxs-lookup"><span data-stu-id="e0546-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0546-133">id</span><span class="sxs-lookup"><span data-stu-id="e0546-133">id</span></span>|<span data-ttu-id="e0546-134">字符串</span><span class="sxs-lookup"><span data-stu-id="e0546-134">String</span></span>|<span data-ttu-id="e0546-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e0546-135">Key of the entity.</span></span> <span data-ttu-id="e0546-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e0546-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0546-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e0546-137">lastModifiedDateTime</span></span>|<span data-ttu-id="e0546-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0546-138">DateTimeOffset</span></span>|<span data-ttu-id="e0546-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="e0546-139">DateTime the object was last modified.</span></span> <span data-ttu-id="e0546-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e0546-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0546-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e0546-141">roleScopeTagIds</span></span>|<span data-ttu-id="e0546-142">String collection</span><span class="sxs-lookup"><span data-stu-id="e0546-142">String collection</span></span>|<span data-ttu-id="e0546-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="e0546-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e0546-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e0546-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0546-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="e0546-145">supportsScopeTags</span></span>|<span data-ttu-id="e0546-146">布尔值</span><span class="sxs-lookup"><span data-stu-id="e0546-146">Boolean</span></span>|<span data-ttu-id="e0546-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="e0546-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="e0546-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="e0546-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="e0546-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="e0546-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="e0546-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="e0546-150">This property is read-only.</span></span> <span data-ttu-id="e0546-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e0546-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0546-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="e0546-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="e0546-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="e0546-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="e0546-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="e0546-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="e0546-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e0546-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0546-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="e0546-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="e0546-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="e0546-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="e0546-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="e0546-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="e0546-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e0546-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0546-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="e0546-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="e0546-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="e0546-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="e0546-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="e0546-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="e0546-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e0546-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0546-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e0546-164">createdDateTime</span></span>|<span data-ttu-id="e0546-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0546-165">DateTimeOffset</span></span>|<span data-ttu-id="e0546-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="e0546-166">DateTime the object was created.</span></span> <span data-ttu-id="e0546-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e0546-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0546-168">说明</span><span class="sxs-lookup"><span data-stu-id="e0546-168">description</span></span>|<span data-ttu-id="e0546-169">String</span><span class="sxs-lookup"><span data-stu-id="e0546-169">String</span></span>|<span data-ttu-id="e0546-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="e0546-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e0546-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e0546-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0546-172">displayName</span><span class="sxs-lookup"><span data-stu-id="e0546-172">displayName</span></span>|<span data-ttu-id="e0546-173">String</span><span class="sxs-lookup"><span data-stu-id="e0546-173">String</span></span>|<span data-ttu-id="e0546-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="e0546-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e0546-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e0546-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0546-176">version</span><span class="sxs-lookup"><span data-stu-id="e0546-176">version</span></span>|<span data-ttu-id="e0546-177">Int32</span><span class="sxs-lookup"><span data-stu-id="e0546-177">Int32</span></span>|<span data-ttu-id="e0546-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="e0546-178">Version of the device configuration.</span></span> <span data-ttu-id="e0546-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e0546-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0546-180">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="e0546-180">trustedRootCertificate</span></span>|<span data-ttu-id="e0546-181">Binary</span><span class="sxs-lookup"><span data-stu-id="e0546-181">Binary</span></span>|<span data-ttu-id="e0546-182">受信任的根证书。</span><span class="sxs-lookup"><span data-stu-id="e0546-182">Trusted Root Certificate.</span></span>|
|<span data-ttu-id="e0546-183">certFileName</span><span class="sxs-lookup"><span data-stu-id="e0546-183">certFileName</span></span>|<span data-ttu-id="e0546-184">String</span><span class="sxs-lookup"><span data-stu-id="e0546-184">String</span></span>|<span data-ttu-id="e0546-185">要在 UI 中显示的文件名。</span><span class="sxs-lookup"><span data-stu-id="e0546-185">File name to display in UI.</span></span>|



## <a name="response"></a><span data-ttu-id="e0546-186">响应</span><span class="sxs-lookup"><span data-stu-id="e0546-186">Response</span></span>
<span data-ttu-id="e0546-187">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和[macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e0546-187">If successful, this method returns a `201 Created` response code and a [macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0546-188">示例</span><span class="sxs-lookup"><span data-stu-id="e0546-188">Example</span></span>

### <a name="request"></a><span data-ttu-id="e0546-189">请求</span><span class="sxs-lookup"><span data-stu-id="e0546-189">Request</span></span>
<span data-ttu-id="e0546-190">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e0546-190">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSEnterpriseWiFiConfiguration/rootCertificatesForServerValidation
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

### <a name="response"></a><span data-ttu-id="e0546-191">响应</span><span class="sxs-lookup"><span data-stu-id="e0546-191">Response</span></span>
<span data-ttu-id="e0546-192">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="e0546-192">Here is an example of the response.</span></span> <span data-ttu-id="e0546-193">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="e0546-193">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="e0546-194">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="e0546-194">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



