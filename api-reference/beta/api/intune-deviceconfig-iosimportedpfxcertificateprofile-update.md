---
title: 更新 iosImportedPFXCertificateProfile
description: 更新 iosImportedPFXCertificateProfile 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 61553c0e14af90af0ac8c456a8b596a54e9c12ab
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/09/2019
ms.locfileid: "38084319"
---
# <a name="update-iosimportedpfxcertificateprofile"></a><span data-ttu-id="86690-103">更新 iosImportedPFXCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="86690-103">Update iosImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="86690-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="86690-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="86690-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="86690-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86690-106">更新[iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="86690-106">Update the properties of a [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="86690-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="86690-107">Prerequisites</span></span>
<span data-ttu-id="86690-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="86690-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86690-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="86690-110">Permission type</span></span>|<span data-ttu-id="86690-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="86690-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="86690-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="86690-112">Delegated (work or school account)</span></span>|<span data-ttu-id="86690-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86690-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="86690-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="86690-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="86690-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="86690-115">Not supported.</span></span>|
|<span data-ttu-id="86690-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="86690-116">Application</span></span>|<span data-ttu-id="86690-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86690-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="86690-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="86690-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="86690-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="86690-119">Request headers</span></span>
|<span data-ttu-id="86690-120">标头</span><span class="sxs-lookup"><span data-stu-id="86690-120">Header</span></span>|<span data-ttu-id="86690-121">值</span><span class="sxs-lookup"><span data-stu-id="86690-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="86690-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="86690-122">Authorization</span></span>|<span data-ttu-id="86690-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="86690-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="86690-124">接受</span><span class="sxs-lookup"><span data-stu-id="86690-124">Accept</span></span>|<span data-ttu-id="86690-125">application/json</span><span class="sxs-lookup"><span data-stu-id="86690-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="86690-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="86690-126">Request body</span></span>
<span data-ttu-id="86690-127">在请求正文中，提供[iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="86690-127">In the request body, supply a JSON representation for the [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) object.</span></span>

<span data-ttu-id="86690-128">下表显示创建[iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="86690-128">The following table shows the properties that are required when you create the [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md).</span></span>

|<span data-ttu-id="86690-129">属性</span><span class="sxs-lookup"><span data-stu-id="86690-129">Property</span></span>|<span data-ttu-id="86690-130">类型</span><span class="sxs-lookup"><span data-stu-id="86690-130">Type</span></span>|<span data-ttu-id="86690-131">描述</span><span class="sxs-lookup"><span data-stu-id="86690-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86690-132">id</span><span class="sxs-lookup"><span data-stu-id="86690-132">id</span></span>|<span data-ttu-id="86690-133">字符串</span><span class="sxs-lookup"><span data-stu-id="86690-133">String</span></span>|<span data-ttu-id="86690-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="86690-134">Key of the entity.</span></span> <span data-ttu-id="86690-135">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86690-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86690-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="86690-136">lastModifiedDateTime</span></span>|<span data-ttu-id="86690-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86690-137">DateTimeOffset</span></span>|<span data-ttu-id="86690-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="86690-138">DateTime the object was last modified.</span></span> <span data-ttu-id="86690-139">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86690-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86690-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="86690-140">roleScopeTagIds</span></span>|<span data-ttu-id="86690-141">String collection</span><span class="sxs-lookup"><span data-stu-id="86690-141">String collection</span></span>|<span data-ttu-id="86690-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="86690-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="86690-143">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86690-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86690-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="86690-144">supportsScopeTags</span></span>|<span data-ttu-id="86690-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="86690-145">Boolean</span></span>|<span data-ttu-id="86690-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="86690-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="86690-147">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="86690-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="86690-148">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="86690-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="86690-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="86690-149">This property is read-only.</span></span> <span data-ttu-id="86690-150">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86690-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86690-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="86690-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="86690-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="86690-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="86690-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="86690-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="86690-154">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86690-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86690-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="86690-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="86690-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="86690-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="86690-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="86690-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="86690-158">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86690-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86690-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="86690-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="86690-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="86690-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="86690-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="86690-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="86690-162">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86690-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86690-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="86690-163">createdDateTime</span></span>|<span data-ttu-id="86690-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86690-164">DateTimeOffset</span></span>|<span data-ttu-id="86690-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="86690-165">DateTime the object was created.</span></span> <span data-ttu-id="86690-166">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86690-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86690-167">说明</span><span class="sxs-lookup"><span data-stu-id="86690-167">description</span></span>|<span data-ttu-id="86690-168">String</span><span class="sxs-lookup"><span data-stu-id="86690-168">String</span></span>|<span data-ttu-id="86690-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="86690-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="86690-170">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86690-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86690-171">displayName</span><span class="sxs-lookup"><span data-stu-id="86690-171">displayName</span></span>|<span data-ttu-id="86690-172">String</span><span class="sxs-lookup"><span data-stu-id="86690-172">String</span></span>|<span data-ttu-id="86690-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="86690-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="86690-174">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86690-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86690-175">version</span><span class="sxs-lookup"><span data-stu-id="86690-175">version</span></span>|<span data-ttu-id="86690-176">Int32</span><span class="sxs-lookup"><span data-stu-id="86690-176">Int32</span></span>|<span data-ttu-id="86690-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="86690-177">Version of the device configuration.</span></span> <span data-ttu-id="86690-178">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86690-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86690-179">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="86690-179">intendedPurpose</span></span>|[<span data-ttu-id="86690-180">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="86690-180">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="86690-181">证书配置文件的预期用途-可以为未分配、SmimeEncryption、SmimeSigning 等。可能的值为`unassigned`： `smimeEncryption`、 `smimeSigning`、 `vpn`、 `wifi`、。</span><span class="sxs-lookup"><span data-stu-id="86690-181">Intended Purpose of the Certificate Profile - which could be Unassigned, SmimeEncryption, SmimeSigning etc. Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="86690-182">响应</span><span class="sxs-lookup"><span data-stu-id="86690-182">Response</span></span>
<span data-ttu-id="86690-183">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="86690-183">If successful, this method returns a `200 OK` response code and an updated [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86690-184">示例</span><span class="sxs-lookup"><span data-stu-id="86690-184">Example</span></span>

### <a name="request"></a><span data-ttu-id="86690-185">请求</span><span class="sxs-lookup"><span data-stu-id="86690-185">Request</span></span>
<span data-ttu-id="86690-186">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="86690-186">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1076

{
  "@odata.type": "#microsoft.graph.iosImportedPFXCertificateProfile",
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
  "intendedPurpose": "smimeEncryption"
}
```

### <a name="response"></a><span data-ttu-id="86690-187">响应</span><span class="sxs-lookup"><span data-stu-id="86690-187">Response</span></span>
<span data-ttu-id="86690-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="86690-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1248

{
  "@odata.type": "#microsoft.graph.iosImportedPFXCertificateProfile",
  "id": "583b9d8c-9d8c-583b-8c9d-3b588c9d3b58",
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
  "intendedPurpose": "smimeEncryption"
}
```






