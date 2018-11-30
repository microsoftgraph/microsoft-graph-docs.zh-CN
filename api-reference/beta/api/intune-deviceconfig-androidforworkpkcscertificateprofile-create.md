---
title: 创建 androidForWorkPkcsCertificateProfile
description: 创建新的 androidForWorkPkcsCertificateProfile 对象。
ms.openlocfilehash: 6beae61dc6125aa1dd9b6b182c49c6af0a1163df
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048336"
---
# <a name="create-androidforworkpkcscertificateprofile"></a><span data-ttu-id="cf277-103">创建 androidForWorkPkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="cf277-103">Create androidForWorkPkcsCertificateProfile</span></span>

> <span data-ttu-id="cf277-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="cf277-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cf277-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="cf277-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cf277-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="cf277-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cf277-107">创建新的[androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="cf277-107">Create a new [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cf277-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="cf277-108">Prerequisites</span></span>
<span data-ttu-id="cf277-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="cf277-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf277-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="cf277-111">Permission type</span></span>|<span data-ttu-id="cf277-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="cf277-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cf277-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cf277-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cf277-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf277-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cf277-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cf277-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cf277-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="cf277-116">Not supported.</span></span>|
|<span data-ttu-id="cf277-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="cf277-117">Application</span></span>|<span data-ttu-id="cf277-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="cf277-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cf277-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cf277-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="cf277-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="cf277-120">Request headers</span></span>
|<span data-ttu-id="cf277-121">标头</span><span class="sxs-lookup"><span data-stu-id="cf277-121">Header</span></span>|<span data-ttu-id="cf277-122">值</span><span class="sxs-lookup"><span data-stu-id="cf277-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cf277-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cf277-123">Authorization</span></span>|<span data-ttu-id="cf277-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="cf277-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cf277-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cf277-125">Accept</span></span>|<span data-ttu-id="cf277-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cf277-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf277-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="cf277-127">Request body</span></span>
<span data-ttu-id="cf277-128">在请求正文中，提供 androidForWorkPkcsCertificateProfile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cf277-128">In the request body, supply a JSON representation for the androidForWorkPkcsCertificateProfile object.</span></span>

<span data-ttu-id="cf277-129">下表显示时创建 androidForWorkPkcsCertificateProfile 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="cf277-129">The following table shows the properties that are required when you create the androidForWorkPkcsCertificateProfile.</span></span>

|<span data-ttu-id="cf277-130">属性</span><span class="sxs-lookup"><span data-stu-id="cf277-130">Property</span></span>|<span data-ttu-id="cf277-131">类型</span><span class="sxs-lookup"><span data-stu-id="cf277-131">Type</span></span>|<span data-ttu-id="cf277-132">说明</span><span class="sxs-lookup"><span data-stu-id="cf277-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf277-133">id</span><span class="sxs-lookup"><span data-stu-id="cf277-133">id</span></span>|<span data-ttu-id="cf277-134">String</span><span class="sxs-lookup"><span data-stu-id="cf277-134">String</span></span>|<span data-ttu-id="cf277-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="cf277-135">Key of the entity.</span></span> <span data-ttu-id="cf277-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cf277-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cf277-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cf277-137">lastModifiedDateTime</span></span>|<span data-ttu-id="cf277-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf277-138">DateTimeOffset</span></span>|<span data-ttu-id="cf277-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="cf277-139">DateTime the object was last modified.</span></span> <span data-ttu-id="cf277-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cf277-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cf277-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="cf277-141">roleScopeTagIds</span></span>|<span data-ttu-id="cf277-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="cf277-142">String collection</span></span>|<span data-ttu-id="cf277-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="cf277-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="cf277-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cf277-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cf277-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="cf277-145">supportsScopeTags</span></span>|<span data-ttu-id="cf277-146">布尔</span><span class="sxs-lookup"><span data-stu-id="cf277-146">Boolean</span></span>|<span data-ttu-id="cf277-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="cf277-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="cf277-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="cf277-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="cf277-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="cf277-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="cf277-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="cf277-150">This property is read-only.</span></span> <span data-ttu-id="cf277-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cf277-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cf277-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cf277-152">createdDateTime</span></span>|<span data-ttu-id="cf277-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf277-153">DateTimeOffset</span></span>|<span data-ttu-id="cf277-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="cf277-154">DateTime the object was created.</span></span> <span data-ttu-id="cf277-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cf277-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cf277-156">description</span><span class="sxs-lookup"><span data-stu-id="cf277-156">description</span></span>|<span data-ttu-id="cf277-157">String</span><span class="sxs-lookup"><span data-stu-id="cf277-157">String</span></span>|<span data-ttu-id="cf277-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="cf277-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="cf277-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cf277-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cf277-160">displayName</span><span class="sxs-lookup"><span data-stu-id="cf277-160">displayName</span></span>|<span data-ttu-id="cf277-161">String</span><span class="sxs-lookup"><span data-stu-id="cf277-161">String</span></span>|<span data-ttu-id="cf277-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="cf277-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="cf277-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cf277-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cf277-164">version</span><span class="sxs-lookup"><span data-stu-id="cf277-164">version</span></span>|<span data-ttu-id="cf277-165">Int32</span><span class="sxs-lookup"><span data-stu-id="cf277-165">Int32</span></span>|<span data-ttu-id="cf277-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="cf277-166">Version of the device configuration.</span></span> <span data-ttu-id="cf277-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cf277-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cf277-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="cf277-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="cf277-169">Int32</span><span class="sxs-lookup"><span data-stu-id="cf277-169">Int32</span></span>|<span data-ttu-id="cf277-170">证书续订阈值百分比。</span><span class="sxs-lookup"><span data-stu-id="cf277-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="cf277-171">有效值 1 到 99 继承自[androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="cf277-171">Valid values 1 to 99 Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="cf277-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="cf277-172">subjectNameFormat</span></span>|[<span data-ttu-id="cf277-173">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="cf277-173">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="cf277-174">证书使用者名称格式。</span><span class="sxs-lookup"><span data-stu-id="cf277-174">Certificate Subject Name Format.</span></span> <span data-ttu-id="cf277-175">继承自[androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="cf277-175">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="cf277-176">可取值为：`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId`。</span><span class="sxs-lookup"><span data-stu-id="cf277-176">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="cf277-177">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="cf277-177">certificateValidityPeriodValue</span></span>|<span data-ttu-id="cf277-178">Int32</span><span class="sxs-lookup"><span data-stu-id="cf277-178">Int32</span></span>|<span data-ttu-id="cf277-179">证书有效期限的值。</span><span class="sxs-lookup"><span data-stu-id="cf277-179">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="cf277-180">继承自[androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="cf277-180">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="cf277-181">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="cf277-181">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="cf277-182">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="cf277-182">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="cf277-183">证书有效期限的小数位数。</span><span class="sxs-lookup"><span data-stu-id="cf277-183">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="cf277-184">继承自[androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="cf277-184">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="cf277-185">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="cf277-185">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="cf277-186">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="cf277-186">extendedKeyUsages</span></span>|<span data-ttu-id="cf277-187">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)集合</span><span class="sxs-lookup"><span data-stu-id="cf277-187">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="cf277-188">扩展的密钥用法 (EKU) 设置。</span><span class="sxs-lookup"><span data-stu-id="cf277-188">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="cf277-189">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="cf277-189">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="cf277-190">继承自[androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="cf277-190">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="cf277-191">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="cf277-191">certificationAuthority</span></span>|<span data-ttu-id="cf277-192">字符串</span><span class="sxs-lookup"><span data-stu-id="cf277-192">String</span></span>|<span data-ttu-id="cf277-193">PKCS 证书颁发机构</span><span class="sxs-lookup"><span data-stu-id="cf277-193">PKCS Certification Authority</span></span>|
|<span data-ttu-id="cf277-194">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="cf277-194">certificationAuthorityName</span></span>|<span data-ttu-id="cf277-195">字符串</span><span class="sxs-lookup"><span data-stu-id="cf277-195">String</span></span>|<span data-ttu-id="cf277-196">PKCS 证书颁发机构名称</span><span class="sxs-lookup"><span data-stu-id="cf277-196">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="cf277-197">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="cf277-197">certificateTemplateName</span></span>|<span data-ttu-id="cf277-198">字符串</span><span class="sxs-lookup"><span data-stu-id="cf277-198">String</span></span>|<span data-ttu-id="cf277-199">PKCS 证书模板名称</span><span class="sxs-lookup"><span data-stu-id="cf277-199">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="cf277-200">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="cf277-200">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="cf277-201">字符串</span><span class="sxs-lookup"><span data-stu-id="cf277-201">String</span></span>|<span data-ttu-id="cf277-202">定义 AAD 属性的自定义字符串。</span><span class="sxs-lookup"><span data-stu-id="cf277-202">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="cf277-203">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="cf277-203">subjectAlternativeNameType</span></span>|[<span data-ttu-id="cf277-204">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="cf277-204">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="cf277-205">证书使用者替代名称类型。</span><span class="sxs-lookup"><span data-stu-id="cf277-205">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="cf277-206">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService`。</span><span class="sxs-lookup"><span data-stu-id="cf277-206">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|



## <a name="response"></a><span data-ttu-id="cf277-207">响应</span><span class="sxs-lookup"><span data-stu-id="cf277-207">Response</span></span>
<span data-ttu-id="cf277-208">如果成功，此方法返回`201 Created`响应代码和响应正文中的[androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="cf277-208">If successful, this method returns a `201 Created` response code and a [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf277-209">示例</span><span class="sxs-lookup"><span data-stu-id="cf277-209">Example</span></span>
### <a name="request"></a><span data-ttu-id="cf277-210">请求</span><span class="sxs-lookup"><span data-stu-id="cf277-210">Request</span></span>
<span data-ttu-id="cf277-211">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cf277-211">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1029

{
  "@odata.type": "#microsoft.graph.androidForWorkPkcsCertificateProfile",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "renewalThresholdPercentage": 10,
  "subjectNameFormat": "commonNameIncludingEmail",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "subjectAlternativeNameType": "emailAddress"
}
```

### <a name="response"></a><span data-ttu-id="cf277-212">响应</span><span class="sxs-lookup"><span data-stu-id="cf277-212">Response</span></span>
<span data-ttu-id="cf277-p117">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cf277-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1137

{
  "@odata.type": "#microsoft.graph.androidForWorkPkcsCertificateProfile",
  "id": "0a2d7691-7691-0a2d-9176-2d0a91762d0a",
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
  "subjectNameFormat": "commonNameIncludingEmail",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "subjectAlternativeNameType": "emailAddress"
}
```





