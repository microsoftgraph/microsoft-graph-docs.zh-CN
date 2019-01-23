---
title: 创建 androidPkcsCertificateProfile
description: 创建新的 androidPkcsCertificateProfile 对象。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9efcf4361d168cd44bbbe16da43941d3ed1215f5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395172"
---
# <a name="create-androidpkcscertificateprofile"></a><span data-ttu-id="28e01-103">创建 androidPkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="28e01-103">Create androidPkcsCertificateProfile</span></span>

> <span data-ttu-id="28e01-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="28e01-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="28e01-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="28e01-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="28e01-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="28e01-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="28e01-107">创建新的[androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="28e01-107">Create a new [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="28e01-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="28e01-108">Prerequisites</span></span>
<span data-ttu-id="28e01-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="28e01-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="28e01-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="28e01-111">Permission type</span></span>|<span data-ttu-id="28e01-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="28e01-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="28e01-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="28e01-113">Delegated (work or school account)</span></span>|<span data-ttu-id="28e01-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28e01-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="28e01-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="28e01-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="28e01-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="28e01-116">Not supported.</span></span>|
|<span data-ttu-id="28e01-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="28e01-117">Application</span></span>|<span data-ttu-id="28e01-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="28e01-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="28e01-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="28e01-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="28e01-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="28e01-120">Request headers</span></span>
|<span data-ttu-id="28e01-121">标头</span><span class="sxs-lookup"><span data-stu-id="28e01-121">Header</span></span>|<span data-ttu-id="28e01-122">值</span><span class="sxs-lookup"><span data-stu-id="28e01-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="28e01-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="28e01-123">Authorization</span></span>|<span data-ttu-id="28e01-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="28e01-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="28e01-125">Accept</span><span class="sxs-lookup"><span data-stu-id="28e01-125">Accept</span></span>|<span data-ttu-id="28e01-126">application/json</span><span class="sxs-lookup"><span data-stu-id="28e01-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="28e01-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="28e01-127">Request body</span></span>
<span data-ttu-id="28e01-128">在请求正文中，提供 androidPkcsCertificateProfile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="28e01-128">In the request body, supply a JSON representation for the androidPkcsCertificateProfile object.</span></span>

<span data-ttu-id="28e01-129">下表显示时创建 androidPkcsCertificateProfile 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="28e01-129">The following table shows the properties that are required when you create the androidPkcsCertificateProfile.</span></span>

|<span data-ttu-id="28e01-130">属性</span><span class="sxs-lookup"><span data-stu-id="28e01-130">Property</span></span>|<span data-ttu-id="28e01-131">类型</span><span class="sxs-lookup"><span data-stu-id="28e01-131">Type</span></span>|<span data-ttu-id="28e01-132">说明</span><span class="sxs-lookup"><span data-stu-id="28e01-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28e01-133">id</span><span class="sxs-lookup"><span data-stu-id="28e01-133">id</span></span>|<span data-ttu-id="28e01-134">String</span><span class="sxs-lookup"><span data-stu-id="28e01-134">String</span></span>|<span data-ttu-id="28e01-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="28e01-135">Key of the entity.</span></span> <span data-ttu-id="28e01-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="28e01-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="28e01-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="28e01-137">lastModifiedDateTime</span></span>|<span data-ttu-id="28e01-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="28e01-138">DateTimeOffset</span></span>|<span data-ttu-id="28e01-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="28e01-139">DateTime the object was last modified.</span></span> <span data-ttu-id="28e01-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="28e01-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="28e01-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="28e01-141">roleScopeTagIds</span></span>|<span data-ttu-id="28e01-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="28e01-142">String collection</span></span>|<span data-ttu-id="28e01-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="28e01-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="28e01-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="28e01-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="28e01-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="28e01-145">supportsScopeTags</span></span>|<span data-ttu-id="28e01-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="28e01-146">Boolean</span></span>|<span data-ttu-id="28e01-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="28e01-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="28e01-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="28e01-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="28e01-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="28e01-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="28e01-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="28e01-150">This property is read-only.</span></span> <span data-ttu-id="28e01-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="28e01-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="28e01-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="28e01-152">createdDateTime</span></span>|<span data-ttu-id="28e01-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="28e01-153">DateTimeOffset</span></span>|<span data-ttu-id="28e01-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="28e01-154">DateTime the object was created.</span></span> <span data-ttu-id="28e01-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="28e01-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="28e01-156">description</span><span class="sxs-lookup"><span data-stu-id="28e01-156">description</span></span>|<span data-ttu-id="28e01-157">String</span><span class="sxs-lookup"><span data-stu-id="28e01-157">String</span></span>|<span data-ttu-id="28e01-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="28e01-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="28e01-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="28e01-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="28e01-160">displayName</span><span class="sxs-lookup"><span data-stu-id="28e01-160">displayName</span></span>|<span data-ttu-id="28e01-161">String</span><span class="sxs-lookup"><span data-stu-id="28e01-161">String</span></span>|<span data-ttu-id="28e01-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="28e01-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="28e01-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="28e01-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="28e01-164">version</span><span class="sxs-lookup"><span data-stu-id="28e01-164">version</span></span>|<span data-ttu-id="28e01-165">Int32</span><span class="sxs-lookup"><span data-stu-id="28e01-165">Int32</span></span>|<span data-ttu-id="28e01-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="28e01-166">Version of the device configuration.</span></span> <span data-ttu-id="28e01-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="28e01-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="28e01-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="28e01-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="28e01-169">Int32</span><span class="sxs-lookup"><span data-stu-id="28e01-169">Int32</span></span>|<span data-ttu-id="28e01-170">证书续订阈值百分比。</span><span class="sxs-lookup"><span data-stu-id="28e01-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="28e01-171">有效值 1 到 99 继承自[androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="28e01-171">Valid values 1 to 99 Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="28e01-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="28e01-172">subjectNameFormat</span></span>|[<span data-ttu-id="28e01-173">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="28e01-173">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="28e01-174">证书使用者名称格式。</span><span class="sxs-lookup"><span data-stu-id="28e01-174">Certificate Subject Name Format.</span></span> <span data-ttu-id="28e01-175">继承自[androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="28e01-175">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="28e01-176">可取值为：`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId`。</span><span class="sxs-lookup"><span data-stu-id="28e01-176">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="28e01-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="28e01-177">subjectAlternativeNameType</span></span>|[<span data-ttu-id="28e01-178">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="28e01-178">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="28e01-179">证书使用者替代名称类型。</span><span class="sxs-lookup"><span data-stu-id="28e01-179">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="28e01-180">继承自[androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="28e01-180">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="28e01-181">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService`。</span><span class="sxs-lookup"><span data-stu-id="28e01-181">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="28e01-182">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="28e01-182">certificateValidityPeriodValue</span></span>|<span data-ttu-id="28e01-183">Int32</span><span class="sxs-lookup"><span data-stu-id="28e01-183">Int32</span></span>|<span data-ttu-id="28e01-184">证书有效期限的值。</span><span class="sxs-lookup"><span data-stu-id="28e01-184">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="28e01-185">继承自[androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="28e01-185">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="28e01-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="28e01-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="28e01-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="28e01-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="28e01-188">证书有效期限的小数位数。</span><span class="sxs-lookup"><span data-stu-id="28e01-188">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="28e01-189">继承自[androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="28e01-189">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="28e01-190">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="28e01-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="28e01-191">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="28e01-191">extendedKeyUsages</span></span>|<span data-ttu-id="28e01-192">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)集合</span><span class="sxs-lookup"><span data-stu-id="28e01-192">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="28e01-193">扩展的密钥用法 (EKU) 设置。</span><span class="sxs-lookup"><span data-stu-id="28e01-193">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="28e01-194">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="28e01-194">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="28e01-195">继承自[androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="28e01-195">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="28e01-196">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="28e01-196">certificationAuthority</span></span>|<span data-ttu-id="28e01-197">String</span><span class="sxs-lookup"><span data-stu-id="28e01-197">String</span></span>|<span data-ttu-id="28e01-198">PKCS 证书颁发机构</span><span class="sxs-lookup"><span data-stu-id="28e01-198">PKCS Certification Authority</span></span>|
|<span data-ttu-id="28e01-199">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="28e01-199">certificationAuthorityName</span></span>|<span data-ttu-id="28e01-200">String</span><span class="sxs-lookup"><span data-stu-id="28e01-200">String</span></span>|<span data-ttu-id="28e01-201">PKCS 证书颁发机构名称</span><span class="sxs-lookup"><span data-stu-id="28e01-201">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="28e01-202">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="28e01-202">certificateTemplateName</span></span>|<span data-ttu-id="28e01-203">String</span><span class="sxs-lookup"><span data-stu-id="28e01-203">String</span></span>|<span data-ttu-id="28e01-204">PKCS 证书模板名称</span><span class="sxs-lookup"><span data-stu-id="28e01-204">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="28e01-205">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="28e01-205">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="28e01-206">String</span><span class="sxs-lookup"><span data-stu-id="28e01-206">String</span></span>|<span data-ttu-id="28e01-207">定义 AAD 属性的自定义字符串。</span><span class="sxs-lookup"><span data-stu-id="28e01-207">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="28e01-208">响应</span><span class="sxs-lookup"><span data-stu-id="28e01-208">Response</span></span>
<span data-ttu-id="28e01-209">如果成功，此方法返回`201 Created`响应代码和响应正文中的[androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="28e01-209">If successful, this method returns a `201 Created` response code and a [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28e01-210">示例</span><span class="sxs-lookup"><span data-stu-id="28e01-210">Example</span></span>

### <a name="request"></a><span data-ttu-id="28e01-211">请求</span><span class="sxs-lookup"><span data-stu-id="28e01-211">Request</span></span>
<span data-ttu-id="28e01-212">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="28e01-212">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 958

{
  "@odata.type": "#microsoft.graph.androidPkcsCertificateProfile",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "renewalThresholdPercentage": 10,
  "subjectNameFormat": "commonNameIncludingEmail",
  "subjectAlternativeNameType": "emailAddress",
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
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```

### <a name="response"></a><span data-ttu-id="28e01-213">响应</span><span class="sxs-lookup"><span data-stu-id="28e01-213">Response</span></span>
<span data-ttu-id="28e01-p117">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="28e01-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1130

{
  "@odata.type": "#microsoft.graph.androidPkcsCertificateProfile",
  "id": "bb55705b-705b-bb55-5b70-55bb5b7055bb",
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
  "subjectAlternativeNameType": "emailAddress",
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
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```




