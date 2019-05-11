---
title: 创建 iosPkcsCertificateProfile
description: 创建新的 iosPkcsCertificateProfile 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a3d455b4626d2ee316c8523509bfe3bce3e429cf
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33923417"
---
# <a name="create-iospkcscertificateprofile"></a><span data-ttu-id="43870-103">创建 iosPkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="43870-103">Create iosPkcsCertificateProfile</span></span>

> <span data-ttu-id="43870-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="43870-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="43870-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="43870-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="43870-106">创建新的[iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="43870-106">Create a new [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="43870-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="43870-107">Prerequisites</span></span>
<span data-ttu-id="43870-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="43870-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="43870-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="43870-110">Permission type</span></span>|<span data-ttu-id="43870-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="43870-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="43870-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="43870-112">Delegated (work or school account)</span></span>|<span data-ttu-id="43870-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43870-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="43870-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="43870-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="43870-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="43870-115">Not supported.</span></span>|
|<span data-ttu-id="43870-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="43870-116">Application</span></span>|<span data-ttu-id="43870-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="43870-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="43870-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="43870-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="43870-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="43870-119">Request headers</span></span>
|<span data-ttu-id="43870-120">标头</span><span class="sxs-lookup"><span data-stu-id="43870-120">Header</span></span>|<span data-ttu-id="43870-121">值</span><span class="sxs-lookup"><span data-stu-id="43870-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="43870-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="43870-122">Authorization</span></span>|<span data-ttu-id="43870-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="43870-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="43870-124">接受</span><span class="sxs-lookup"><span data-stu-id="43870-124">Accept</span></span>|<span data-ttu-id="43870-125">application/json</span><span class="sxs-lookup"><span data-stu-id="43870-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="43870-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="43870-126">Request body</span></span>
<span data-ttu-id="43870-127">在请求正文中, 提供 iosPkcsCertificateProfile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="43870-127">In the request body, supply a JSON representation for the iosPkcsCertificateProfile object.</span></span>

<span data-ttu-id="43870-128">下表显示创建 iosPkcsCertificateProfile 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="43870-128">The following table shows the properties that are required when you create the iosPkcsCertificateProfile.</span></span>

|<span data-ttu-id="43870-129">属性</span><span class="sxs-lookup"><span data-stu-id="43870-129">Property</span></span>|<span data-ttu-id="43870-130">类型</span><span class="sxs-lookup"><span data-stu-id="43870-130">Type</span></span>|<span data-ttu-id="43870-131">说明</span><span class="sxs-lookup"><span data-stu-id="43870-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43870-132">id</span><span class="sxs-lookup"><span data-stu-id="43870-132">id</span></span>|<span data-ttu-id="43870-133">字符串</span><span class="sxs-lookup"><span data-stu-id="43870-133">String</span></span>|<span data-ttu-id="43870-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="43870-134">Key of the entity.</span></span> <span data-ttu-id="43870-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="43870-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="43870-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="43870-136">lastModifiedDateTime</span></span>|<span data-ttu-id="43870-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="43870-137">DateTimeOffset</span></span>|<span data-ttu-id="43870-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="43870-138">DateTime the object was last modified.</span></span> <span data-ttu-id="43870-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="43870-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="43870-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="43870-140">roleScopeTagIds</span></span>|<span data-ttu-id="43870-141">String collection</span><span class="sxs-lookup"><span data-stu-id="43870-141">String collection</span></span>|<span data-ttu-id="43870-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="43870-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="43870-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="43870-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="43870-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="43870-144">supportsScopeTags</span></span>|<span data-ttu-id="43870-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="43870-145">Boolean</span></span>|<span data-ttu-id="43870-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="43870-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="43870-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="43870-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="43870-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="43870-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="43870-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="43870-149">This property is read-only.</span></span> <span data-ttu-id="43870-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="43870-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="43870-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="43870-151">createdDateTime</span></span>|<span data-ttu-id="43870-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="43870-152">DateTimeOffset</span></span>|<span data-ttu-id="43870-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="43870-153">DateTime the object was created.</span></span> <span data-ttu-id="43870-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="43870-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="43870-155">说明</span><span class="sxs-lookup"><span data-stu-id="43870-155">description</span></span>|<span data-ttu-id="43870-156">String</span><span class="sxs-lookup"><span data-stu-id="43870-156">String</span></span>|<span data-ttu-id="43870-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="43870-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="43870-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="43870-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="43870-159">displayName</span><span class="sxs-lookup"><span data-stu-id="43870-159">displayName</span></span>|<span data-ttu-id="43870-160">String</span><span class="sxs-lookup"><span data-stu-id="43870-160">String</span></span>|<span data-ttu-id="43870-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="43870-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="43870-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="43870-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="43870-163">version</span><span class="sxs-lookup"><span data-stu-id="43870-163">version</span></span>|<span data-ttu-id="43870-164">Int32</span><span class="sxs-lookup"><span data-stu-id="43870-164">Int32</span></span>|<span data-ttu-id="43870-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="43870-165">Version of the device configuration.</span></span> <span data-ttu-id="43870-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="43870-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="43870-167">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="43870-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="43870-168">Int32</span><span class="sxs-lookup"><span data-stu-id="43870-168">Int32</span></span>|<span data-ttu-id="43870-169">证书续订阈值百分比。</span><span class="sxs-lookup"><span data-stu-id="43870-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="43870-170">从[IosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)继承的有效值1到99</span><span class="sxs-lookup"><span data-stu-id="43870-170">Valid values 1 to 99 Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="43870-171">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="43870-171">subjectNameFormat</span></span>|[<span data-ttu-id="43870-172">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="43870-172">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="43870-173">证书使用者名称格式。</span><span class="sxs-lookup"><span data-stu-id="43870-173">Certificate Subject Name Format.</span></span> <span data-ttu-id="43870-174">继承自[iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="43870-174">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="43870-175">可取值为：`commonName`、`commonNameAsEmail`、`custom`、`commonNameIncludingEmail`、`commonNameAsIMEI`、`commonNameAsSerialNumber`。</span><span class="sxs-lookup"><span data-stu-id="43870-175">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="43870-176">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="43870-176">subjectAlternativeNameType</span></span>|[<span data-ttu-id="43870-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="43870-177">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="43870-178">证书使用者备用名称类型。</span><span class="sxs-lookup"><span data-stu-id="43870-178">Certificate Subject Alternative Name type.</span></span> <span data-ttu-id="43870-179">继承自[iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="43870-179">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="43870-180">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService`。</span><span class="sxs-lookup"><span data-stu-id="43870-180">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="43870-181">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="43870-181">certificateValidityPeriodValue</span></span>|<span data-ttu-id="43870-182">Int32</span><span class="sxs-lookup"><span data-stu-id="43870-182">Int32</span></span>|<span data-ttu-id="43870-183">证书有效期限的值。</span><span class="sxs-lookup"><span data-stu-id="43870-183">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="43870-184">继承自[iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="43870-184">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="43870-185">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="43870-185">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="43870-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="43870-186">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="43870-187">证书有效期的小数位数。</span><span class="sxs-lookup"><span data-stu-id="43870-187">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="43870-188">继承自[iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="43870-188">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="43870-189">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="43870-189">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="43870-190">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="43870-190">certificationAuthority</span></span>|<span data-ttu-id="43870-191">String</span><span class="sxs-lookup"><span data-stu-id="43870-191">String</span></span>|<span data-ttu-id="43870-192">PKCS 证书颁发机构。</span><span class="sxs-lookup"><span data-stu-id="43870-192">PKCS Certification Authority.</span></span>|
|<span data-ttu-id="43870-193">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="43870-193">certificationAuthorityName</span></span>|<span data-ttu-id="43870-194">String</span><span class="sxs-lookup"><span data-stu-id="43870-194">String</span></span>|<span data-ttu-id="43870-195">PKCS 证书颁发机构名称。</span><span class="sxs-lookup"><span data-stu-id="43870-195">PKCS Certification Authority Name.</span></span>|
|<span data-ttu-id="43870-196">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="43870-196">certificateTemplateName</span></span>|<span data-ttu-id="43870-197">String</span><span class="sxs-lookup"><span data-stu-id="43870-197">String</span></span>|<span data-ttu-id="43870-198">PKCS 证书模板名称。</span><span class="sxs-lookup"><span data-stu-id="43870-198">PKCS Certificate Template Name.</span></span>|
|<span data-ttu-id="43870-199">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="43870-199">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="43870-200">String</span><span class="sxs-lookup"><span data-stu-id="43870-200">String</span></span>|<span data-ttu-id="43870-201">定义 AAD 属性的自定义字符串。</span><span class="sxs-lookup"><span data-stu-id="43870-201">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="43870-202">响应</span><span class="sxs-lookup"><span data-stu-id="43870-202">Response</span></span>
<span data-ttu-id="43870-203">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="43870-203">If successful, this method returns a `201 Created` response code and a [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="43870-204">示例</span><span class="sxs-lookup"><span data-stu-id="43870-204">Example</span></span>

### <a name="request"></a><span data-ttu-id="43870-205">请求</span><span class="sxs-lookup"><span data-stu-id="43870-205">Request</span></span>
<span data-ttu-id="43870-206">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="43870-206">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 761

{
  "@odata.type": "#microsoft.graph.iosPkcsCertificateProfile",
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
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```

### <a name="response"></a><span data-ttu-id="43870-207">响应</span><span class="sxs-lookup"><span data-stu-id="43870-207">Response</span></span>
<span data-ttu-id="43870-p115">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="43870-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 933

{
  "@odata.type": "#microsoft.graph.iosPkcsCertificateProfile",
  "id": "ed0264dd-64dd-ed02-dd64-02eddd6402ed",
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
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```




