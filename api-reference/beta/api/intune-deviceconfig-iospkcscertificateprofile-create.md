---
title: 创建 iosPkcsCertificateProfile
description: 创建新的 iosPkcsCertificateProfile 对象。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2cb5f93296d7117cd003d807afbdf19211d607a0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396257"
---
# <a name="create-iospkcscertificateprofile"></a><span data-ttu-id="acd10-103">创建 iosPkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="acd10-103">Create iosPkcsCertificateProfile</span></span>

> <span data-ttu-id="acd10-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="acd10-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="acd10-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="acd10-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="acd10-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="acd10-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="acd10-107">创建新的[iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="acd10-107">Create a new [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="acd10-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="acd10-108">Prerequisites</span></span>
<span data-ttu-id="acd10-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="acd10-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="acd10-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="acd10-111">Permission type</span></span>|<span data-ttu-id="acd10-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="acd10-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="acd10-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="acd10-113">Delegated (work or school account)</span></span>|<span data-ttu-id="acd10-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="acd10-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="acd10-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="acd10-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="acd10-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="acd10-116">Not supported.</span></span>|
|<span data-ttu-id="acd10-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="acd10-117">Application</span></span>|<span data-ttu-id="acd10-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="acd10-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="acd10-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="acd10-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="acd10-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="acd10-120">Request headers</span></span>
|<span data-ttu-id="acd10-121">标头</span><span class="sxs-lookup"><span data-stu-id="acd10-121">Header</span></span>|<span data-ttu-id="acd10-122">值</span><span class="sxs-lookup"><span data-stu-id="acd10-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="acd10-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="acd10-123">Authorization</span></span>|<span data-ttu-id="acd10-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="acd10-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="acd10-125">Accept</span><span class="sxs-lookup"><span data-stu-id="acd10-125">Accept</span></span>|<span data-ttu-id="acd10-126">application/json</span><span class="sxs-lookup"><span data-stu-id="acd10-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="acd10-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="acd10-127">Request body</span></span>
<span data-ttu-id="acd10-128">在请求正文中，提供 iosPkcsCertificateProfile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="acd10-128">In the request body, supply a JSON representation for the iosPkcsCertificateProfile object.</span></span>

<span data-ttu-id="acd10-129">下表显示时创建 iosPkcsCertificateProfile 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="acd10-129">The following table shows the properties that are required when you create the iosPkcsCertificateProfile.</span></span>

|<span data-ttu-id="acd10-130">属性</span><span class="sxs-lookup"><span data-stu-id="acd10-130">Property</span></span>|<span data-ttu-id="acd10-131">类型</span><span class="sxs-lookup"><span data-stu-id="acd10-131">Type</span></span>|<span data-ttu-id="acd10-132">说明</span><span class="sxs-lookup"><span data-stu-id="acd10-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="acd10-133">id</span><span class="sxs-lookup"><span data-stu-id="acd10-133">id</span></span>|<span data-ttu-id="acd10-134">String</span><span class="sxs-lookup"><span data-stu-id="acd10-134">String</span></span>|<span data-ttu-id="acd10-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="acd10-135">Key of the entity.</span></span> <span data-ttu-id="acd10-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="acd10-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="acd10-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="acd10-137">lastModifiedDateTime</span></span>|<span data-ttu-id="acd10-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="acd10-138">DateTimeOffset</span></span>|<span data-ttu-id="acd10-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="acd10-139">DateTime the object was last modified.</span></span> <span data-ttu-id="acd10-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="acd10-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="acd10-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="acd10-141">roleScopeTagIds</span></span>|<span data-ttu-id="acd10-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="acd10-142">String collection</span></span>|<span data-ttu-id="acd10-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="acd10-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="acd10-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="acd10-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="acd10-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="acd10-145">supportsScopeTags</span></span>|<span data-ttu-id="acd10-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="acd10-146">Boolean</span></span>|<span data-ttu-id="acd10-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="acd10-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="acd10-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="acd10-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="acd10-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="acd10-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="acd10-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="acd10-150">This property is read-only.</span></span> <span data-ttu-id="acd10-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="acd10-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="acd10-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="acd10-152">createdDateTime</span></span>|<span data-ttu-id="acd10-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="acd10-153">DateTimeOffset</span></span>|<span data-ttu-id="acd10-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="acd10-154">DateTime the object was created.</span></span> <span data-ttu-id="acd10-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="acd10-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="acd10-156">description</span><span class="sxs-lookup"><span data-stu-id="acd10-156">description</span></span>|<span data-ttu-id="acd10-157">String</span><span class="sxs-lookup"><span data-stu-id="acd10-157">String</span></span>|<span data-ttu-id="acd10-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="acd10-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="acd10-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="acd10-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="acd10-160">displayName</span><span class="sxs-lookup"><span data-stu-id="acd10-160">displayName</span></span>|<span data-ttu-id="acd10-161">String</span><span class="sxs-lookup"><span data-stu-id="acd10-161">String</span></span>|<span data-ttu-id="acd10-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="acd10-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="acd10-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="acd10-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="acd10-164">version</span><span class="sxs-lookup"><span data-stu-id="acd10-164">version</span></span>|<span data-ttu-id="acd10-165">Int32</span><span class="sxs-lookup"><span data-stu-id="acd10-165">Int32</span></span>|<span data-ttu-id="acd10-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="acd10-166">Version of the device configuration.</span></span> <span data-ttu-id="acd10-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="acd10-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="acd10-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="acd10-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="acd10-169">Int32</span><span class="sxs-lookup"><span data-stu-id="acd10-169">Int32</span></span>|<span data-ttu-id="acd10-170">证书续订阈值百分比。</span><span class="sxs-lookup"><span data-stu-id="acd10-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="acd10-171">有效值 1 到 99 继承自[iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="acd10-171">Valid values 1 to 99 Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="acd10-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="acd10-172">subjectNameFormat</span></span>|[<span data-ttu-id="acd10-173">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="acd10-173">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="acd10-174">证书使用者名称格式。</span><span class="sxs-lookup"><span data-stu-id="acd10-174">Certificate Subject Name Format.</span></span> <span data-ttu-id="acd10-175">继承自[iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="acd10-175">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="acd10-176">可取值为：`commonName`、`commonNameAsEmail`、`custom`、`commonNameIncludingEmail`、`commonNameAsIMEI`、`commonNameAsSerialNumber`。</span><span class="sxs-lookup"><span data-stu-id="acd10-176">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="acd10-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="acd10-177">subjectAlternativeNameType</span></span>|[<span data-ttu-id="acd10-178">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="acd10-178">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="acd10-179">证书使用者替代名称类型。</span><span class="sxs-lookup"><span data-stu-id="acd10-179">Certificate Subject Alternative Name type.</span></span> <span data-ttu-id="acd10-180">继承自[iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="acd10-180">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="acd10-181">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService`。</span><span class="sxs-lookup"><span data-stu-id="acd10-181">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="acd10-182">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="acd10-182">certificateValidityPeriodValue</span></span>|<span data-ttu-id="acd10-183">Int32</span><span class="sxs-lookup"><span data-stu-id="acd10-183">Int32</span></span>|<span data-ttu-id="acd10-184">证书有效期限的值。</span><span class="sxs-lookup"><span data-stu-id="acd10-184">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="acd10-185">继承自[iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="acd10-185">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="acd10-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="acd10-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="acd10-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="acd10-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="acd10-188">证书有效期限的小数位数。</span><span class="sxs-lookup"><span data-stu-id="acd10-188">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="acd10-189">继承自[iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="acd10-189">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="acd10-190">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="acd10-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="acd10-191">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="acd10-191">certificationAuthority</span></span>|<span data-ttu-id="acd10-192">String</span><span class="sxs-lookup"><span data-stu-id="acd10-192">String</span></span>|<span data-ttu-id="acd10-193">PKCS 证书颁发机构。</span><span class="sxs-lookup"><span data-stu-id="acd10-193">PKCS Certification Authority.</span></span>|
|<span data-ttu-id="acd10-194">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="acd10-194">certificationAuthorityName</span></span>|<span data-ttu-id="acd10-195">String</span><span class="sxs-lookup"><span data-stu-id="acd10-195">String</span></span>|<span data-ttu-id="acd10-196">PKCS 证书颁发机构的名称。</span><span class="sxs-lookup"><span data-stu-id="acd10-196">PKCS Certification Authority Name.</span></span>|
|<span data-ttu-id="acd10-197">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="acd10-197">certificateTemplateName</span></span>|<span data-ttu-id="acd10-198">String</span><span class="sxs-lookup"><span data-stu-id="acd10-198">String</span></span>|<span data-ttu-id="acd10-199">PKCS 证书模板名称。</span><span class="sxs-lookup"><span data-stu-id="acd10-199">PKCS Certificate Template Name.</span></span>|
|<span data-ttu-id="acd10-200">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="acd10-200">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="acd10-201">String</span><span class="sxs-lookup"><span data-stu-id="acd10-201">String</span></span>|<span data-ttu-id="acd10-202">定义 AAD 属性的自定义字符串。</span><span class="sxs-lookup"><span data-stu-id="acd10-202">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="acd10-203">响应</span><span class="sxs-lookup"><span data-stu-id="acd10-203">Response</span></span>
<span data-ttu-id="acd10-204">如果成功，此方法返回`201 Created`响应代码和响应正文中的[iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="acd10-204">If successful, this method returns a `201 Created` response code and a [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="acd10-205">示例</span><span class="sxs-lookup"><span data-stu-id="acd10-205">Example</span></span>

### <a name="request"></a><span data-ttu-id="acd10-206">请求</span><span class="sxs-lookup"><span data-stu-id="acd10-206">Request</span></span>
<span data-ttu-id="acd10-207">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="acd10-207">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="acd10-208">响应</span><span class="sxs-lookup"><span data-stu-id="acd10-208">Response</span></span>
<span data-ttu-id="acd10-p116">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="acd10-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




