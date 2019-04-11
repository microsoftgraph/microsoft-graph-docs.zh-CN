---
title: 更新 macOSImportedPFXCertificateProfile
description: 更新 macOSImportedPFXCertificateProfile 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1bdf83aa5fca824ed0180c630a69f80502cae559
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31804821"
---
# <a name="update-macosimportedpfxcertificateprofile"></a><span data-ttu-id="3891b-103">更新 macOSImportedPFXCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="3891b-103">Update macOSImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="3891b-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3891b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3891b-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3891b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3891b-106">更新[macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="3891b-106">Update the properties of a [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3891b-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="3891b-107">Prerequisites</span></span>
<span data-ttu-id="3891b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3891b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3891b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="3891b-110">Permission type</span></span>|<span data-ttu-id="3891b-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3891b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3891b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3891b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3891b-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3891b-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3891b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3891b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3891b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3891b-115">Not supported.</span></span>|
|<span data-ttu-id="3891b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="3891b-116">Application</span></span>|<span data-ttu-id="3891b-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="3891b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3891b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3891b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="3891b-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="3891b-119">Request headers</span></span>
|<span data-ttu-id="3891b-120">标头</span><span class="sxs-lookup"><span data-stu-id="3891b-120">Header</span></span>|<span data-ttu-id="3891b-121">值</span><span class="sxs-lookup"><span data-stu-id="3891b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3891b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3891b-122">Authorization</span></span>|<span data-ttu-id="3891b-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3891b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3891b-124">接受</span><span class="sxs-lookup"><span data-stu-id="3891b-124">Accept</span></span>|<span data-ttu-id="3891b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3891b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3891b-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="3891b-126">Request body</span></span>
<span data-ttu-id="3891b-127">在请求正文中, 提供[macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3891b-127">In the request body, supply a JSON representation for the [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) object.</span></span>

<span data-ttu-id="3891b-128">下表显示创建[macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3891b-128">The following table shows the properties that are required when you create the [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md).</span></span>

|<span data-ttu-id="3891b-129">属性</span><span class="sxs-lookup"><span data-stu-id="3891b-129">Property</span></span>|<span data-ttu-id="3891b-130">类型</span><span class="sxs-lookup"><span data-stu-id="3891b-130">Type</span></span>|<span data-ttu-id="3891b-131">说明</span><span class="sxs-lookup"><span data-stu-id="3891b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3891b-132">id</span><span class="sxs-lookup"><span data-stu-id="3891b-132">id</span></span>|<span data-ttu-id="3891b-133">String</span><span class="sxs-lookup"><span data-stu-id="3891b-133">String</span></span>|<span data-ttu-id="3891b-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="3891b-134">Key of the entity.</span></span> <span data-ttu-id="3891b-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3891b-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3891b-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3891b-136">lastModifiedDateTime</span></span>|<span data-ttu-id="3891b-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3891b-137">DateTimeOffset</span></span>|<span data-ttu-id="3891b-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="3891b-138">DateTime the object was last modified.</span></span> <span data-ttu-id="3891b-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3891b-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3891b-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3891b-140">roleScopeTagIds</span></span>|<span data-ttu-id="3891b-141">String 集合</span><span class="sxs-lookup"><span data-stu-id="3891b-141">String collection</span></span>|<span data-ttu-id="3891b-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="3891b-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="3891b-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3891b-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3891b-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="3891b-144">supportsScopeTags</span></span>|<span data-ttu-id="3891b-145">布尔值</span><span class="sxs-lookup"><span data-stu-id="3891b-145">Boolean</span></span>|<span data-ttu-id="3891b-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="3891b-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="3891b-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="3891b-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="3891b-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="3891b-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="3891b-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="3891b-149">This property is read-only.</span></span> <span data-ttu-id="3891b-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3891b-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3891b-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3891b-151">createdDateTime</span></span>|<span data-ttu-id="3891b-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3891b-152">DateTimeOffset</span></span>|<span data-ttu-id="3891b-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="3891b-153">DateTime the object was created.</span></span> <span data-ttu-id="3891b-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3891b-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3891b-155">description</span><span class="sxs-lookup"><span data-stu-id="3891b-155">description</span></span>|<span data-ttu-id="3891b-156">String</span><span class="sxs-lookup"><span data-stu-id="3891b-156">String</span></span>|<span data-ttu-id="3891b-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="3891b-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3891b-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3891b-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3891b-159">displayName</span><span class="sxs-lookup"><span data-stu-id="3891b-159">displayName</span></span>|<span data-ttu-id="3891b-160">String</span><span class="sxs-lookup"><span data-stu-id="3891b-160">String</span></span>|<span data-ttu-id="3891b-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="3891b-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3891b-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3891b-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3891b-163">version</span><span class="sxs-lookup"><span data-stu-id="3891b-163">version</span></span>|<span data-ttu-id="3891b-164">Int32</span><span class="sxs-lookup"><span data-stu-id="3891b-164">Int32</span></span>|<span data-ttu-id="3891b-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="3891b-165">Version of the device configuration.</span></span> <span data-ttu-id="3891b-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3891b-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3891b-167">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="3891b-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="3891b-168">Int32</span><span class="sxs-lookup"><span data-stu-id="3891b-168">Int32</span></span>|<span data-ttu-id="3891b-169">证书续订阈值百分比。</span><span class="sxs-lookup"><span data-stu-id="3891b-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="3891b-170">继承自[macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="3891b-170">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="3891b-171">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="3891b-171">subjectNameFormat</span></span>|[<span data-ttu-id="3891b-172">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="3891b-172">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="3891b-173">证书使用者名称格式。</span><span class="sxs-lookup"><span data-stu-id="3891b-173">Certificate Subject Name Format.</span></span> <span data-ttu-id="3891b-174">继承自[macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="3891b-174">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="3891b-175">可取值为：`commonName`、`commonNameAsEmail`、`custom`、`commonNameIncludingEmail`、`commonNameAsIMEI`、`commonNameAsSerialNumber`。</span><span class="sxs-lookup"><span data-stu-id="3891b-175">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="3891b-176">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="3891b-176">subjectAlternativeNameType</span></span>|[<span data-ttu-id="3891b-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="3891b-177">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="3891b-178">证书使用者备用名称类型。</span><span class="sxs-lookup"><span data-stu-id="3891b-178">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="3891b-179">继承自[macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="3891b-179">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="3891b-180">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute` 或 `domainNameService`。</span><span class="sxs-lookup"><span data-stu-id="3891b-180">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="3891b-181">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="3891b-181">certificateValidityPeriodValue</span></span>|<span data-ttu-id="3891b-182">Int32</span><span class="sxs-lookup"><span data-stu-id="3891b-182">Int32</span></span>|<span data-ttu-id="3891b-183">证书有效期限的值。</span><span class="sxs-lookup"><span data-stu-id="3891b-183">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="3891b-184">继承自[macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="3891b-184">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="3891b-185">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="3891b-185">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="3891b-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="3891b-186">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="3891b-187">证书有效期的小数位数。</span><span class="sxs-lookup"><span data-stu-id="3891b-187">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="3891b-188">继承自[macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="3891b-188">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="3891b-189">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="3891b-189">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="3891b-190">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="3891b-190">intendedPurpose</span></span>|[<span data-ttu-id="3891b-191">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="3891b-191">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="3891b-192">尚未记录。</span><span class="sxs-lookup"><span data-stu-id="3891b-192">Not yet documented.</span></span> <span data-ttu-id="3891b-193">可取值为：`unassigned`、`smimeEncryption`、`smimeSigning`、`vpn` 或 `wifi`。</span><span class="sxs-lookup"><span data-stu-id="3891b-193">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="3891b-194">响应</span><span class="sxs-lookup"><span data-stu-id="3891b-194">Response</span></span>
<span data-ttu-id="3891b-195">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="3891b-195">If successful, this method returns a `200 OK` response code and an updated [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3891b-196">示例</span><span class="sxs-lookup"><span data-stu-id="3891b-196">Example</span></span>

### <a name="request"></a><span data-ttu-id="3891b-197">请求</span><span class="sxs-lookup"><span data-stu-id="3891b-197">Request</span></span>
<span data-ttu-id="3891b-198">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3891b-198">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 524

{
  "@odata.type": "#microsoft.graph.macOSImportedPFXCertificateProfile",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "renewalThresholdPercentage": 10,
  "subjectNameFormat": "commonNameAsEmail",
  "subjectAlternativeNameType": "emailAddress",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "intendedPurpose": "smimeEncryption"
}
```

### <a name="response"></a><span data-ttu-id="3891b-199">响应</span><span class="sxs-lookup"><span data-stu-id="3891b-199">Response</span></span>
<span data-ttu-id="3891b-p116">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3891b-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 696

{
  "@odata.type": "#microsoft.graph.macOSImportedPFXCertificateProfile",
  "id": "4175bd8c-bd8c-4175-8cbd-75418cbd7541",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "renewalThresholdPercentage": 10,
  "subjectNameFormat": "commonNameAsEmail",
  "subjectAlternativeNameType": "emailAddress",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "intendedPurpose": "smimeEncryption"
}
```





