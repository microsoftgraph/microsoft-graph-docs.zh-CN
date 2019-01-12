---
title: 创建 iosScepCertificateProfile
description: 创建新的 iosScepCertificateProfile 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ef9955b876ae43cacd163968ddbfb8f72b91f9ef
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27924977"
---
# <a name="create-iosscepcertificateprofile"></a><span data-ttu-id="8479e-103">创建 iosScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="8479e-103">Create iosScepCertificateProfile</span></span>

> <span data-ttu-id="8479e-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="8479e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8479e-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8479e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8479e-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="8479e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8479e-107">创建新的[iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8479e-107">Create a new [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8479e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="8479e-108">Prerequisites</span></span>
<span data-ttu-id="8479e-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="8479e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8479e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="8479e-111">Permission type</span></span>|<span data-ttu-id="8479e-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8479e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8479e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8479e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8479e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8479e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8479e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8479e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8479e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8479e-116">Not supported.</span></span>|
|<span data-ttu-id="8479e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="8479e-117">Application</span></span>|<span data-ttu-id="8479e-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="8479e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8479e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8479e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="8479e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="8479e-120">Request headers</span></span>
|<span data-ttu-id="8479e-121">标头</span><span class="sxs-lookup"><span data-stu-id="8479e-121">Header</span></span>|<span data-ttu-id="8479e-122">值</span><span class="sxs-lookup"><span data-stu-id="8479e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8479e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8479e-123">Authorization</span></span>|<span data-ttu-id="8479e-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8479e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8479e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8479e-125">Accept</span></span>|<span data-ttu-id="8479e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8479e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8479e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="8479e-127">Request body</span></span>
<span data-ttu-id="8479e-128">在请求正文中，提供 iosScepCertificateProfile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8479e-128">In the request body, supply a JSON representation for the iosScepCertificateProfile object.</span></span>

<span data-ttu-id="8479e-129">下表显示时创建 iosScepCertificateProfile 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="8479e-129">The following table shows the properties that are required when you create the iosScepCertificateProfile.</span></span>

|<span data-ttu-id="8479e-130">属性</span><span class="sxs-lookup"><span data-stu-id="8479e-130">Property</span></span>|<span data-ttu-id="8479e-131">类型</span><span class="sxs-lookup"><span data-stu-id="8479e-131">Type</span></span>|<span data-ttu-id="8479e-132">说明</span><span class="sxs-lookup"><span data-stu-id="8479e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8479e-133">id</span><span class="sxs-lookup"><span data-stu-id="8479e-133">id</span></span>|<span data-ttu-id="8479e-134">String</span><span class="sxs-lookup"><span data-stu-id="8479e-134">String</span></span>|<span data-ttu-id="8479e-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="8479e-135">Key of the entity.</span></span> <span data-ttu-id="8479e-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8479e-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8479e-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8479e-137">lastModifiedDateTime</span></span>|<span data-ttu-id="8479e-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8479e-138">DateTimeOffset</span></span>|<span data-ttu-id="8479e-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="8479e-139">DateTime the object was last modified.</span></span> <span data-ttu-id="8479e-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8479e-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8479e-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8479e-141">roleScopeTagIds</span></span>|<span data-ttu-id="8479e-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="8479e-142">String collection</span></span>|<span data-ttu-id="8479e-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="8479e-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="8479e-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8479e-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8479e-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="8479e-145">supportsScopeTags</span></span>|<span data-ttu-id="8479e-146">布尔</span><span class="sxs-lookup"><span data-stu-id="8479e-146">Boolean</span></span>|<span data-ttu-id="8479e-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="8479e-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="8479e-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="8479e-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="8479e-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="8479e-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="8479e-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8479e-150">This property is read-only.</span></span> <span data-ttu-id="8479e-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8479e-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8479e-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8479e-152">createdDateTime</span></span>|<span data-ttu-id="8479e-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8479e-153">DateTimeOffset</span></span>|<span data-ttu-id="8479e-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="8479e-154">DateTime the object was created.</span></span> <span data-ttu-id="8479e-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8479e-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8479e-156">description</span><span class="sxs-lookup"><span data-stu-id="8479e-156">description</span></span>|<span data-ttu-id="8479e-157">String</span><span class="sxs-lookup"><span data-stu-id="8479e-157">String</span></span>|<span data-ttu-id="8479e-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="8479e-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8479e-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8479e-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8479e-160">displayName</span><span class="sxs-lookup"><span data-stu-id="8479e-160">displayName</span></span>|<span data-ttu-id="8479e-161">String</span><span class="sxs-lookup"><span data-stu-id="8479e-161">String</span></span>|<span data-ttu-id="8479e-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="8479e-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8479e-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8479e-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8479e-164">version</span><span class="sxs-lookup"><span data-stu-id="8479e-164">version</span></span>|<span data-ttu-id="8479e-165">Int32</span><span class="sxs-lookup"><span data-stu-id="8479e-165">Int32</span></span>|<span data-ttu-id="8479e-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="8479e-166">Version of the device configuration.</span></span> <span data-ttu-id="8479e-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8479e-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8479e-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="8479e-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="8479e-169">Int32</span><span class="sxs-lookup"><span data-stu-id="8479e-169">Int32</span></span>|<span data-ttu-id="8479e-170">证书续订阈值百分比。</span><span class="sxs-lookup"><span data-stu-id="8479e-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="8479e-171">有效值 1 到 99 继承自[iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="8479e-171">Valid values 1 to 99 Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="8479e-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="8479e-172">subjectNameFormat</span></span>|[<span data-ttu-id="8479e-173">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="8479e-173">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="8479e-174">证书使用者名称格式。</span><span class="sxs-lookup"><span data-stu-id="8479e-174">Certificate Subject Name Format.</span></span> <span data-ttu-id="8479e-175">继承自[iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="8479e-175">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="8479e-176">可取值为：`commonName`、`commonNameAsEmail`、`custom`、`commonNameIncludingEmail`、`commonNameAsIMEI`、`commonNameAsSerialNumber`。</span><span class="sxs-lookup"><span data-stu-id="8479e-176">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="8479e-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="8479e-177">subjectAlternativeNameType</span></span>|[<span data-ttu-id="8479e-178">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="8479e-178">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="8479e-179">证书使用者替代名称类型。</span><span class="sxs-lookup"><span data-stu-id="8479e-179">Certificate Subject Alternative Name type.</span></span> <span data-ttu-id="8479e-180">继承自[iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="8479e-180">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="8479e-181">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService`。</span><span class="sxs-lookup"><span data-stu-id="8479e-181">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="8479e-182">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="8479e-182">certificateValidityPeriodValue</span></span>|<span data-ttu-id="8479e-183">Int32</span><span class="sxs-lookup"><span data-stu-id="8479e-183">Int32</span></span>|<span data-ttu-id="8479e-184">证书有效期限的值。</span><span class="sxs-lookup"><span data-stu-id="8479e-184">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="8479e-185">继承自[iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="8479e-185">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="8479e-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="8479e-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="8479e-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="8479e-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="8479e-188">证书有效期限的小数位数。</span><span class="sxs-lookup"><span data-stu-id="8479e-188">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="8479e-189">继承自[iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="8479e-189">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="8479e-190">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="8479e-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="8479e-191">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="8479e-191">scepServerUrls</span></span>|<span data-ttu-id="8479e-192">String 集合</span><span class="sxs-lookup"><span data-stu-id="8479e-192">String collection</span></span>|<span data-ttu-id="8479e-193">SCEP 服务器 Url(s)。</span><span class="sxs-lookup"><span data-stu-id="8479e-193">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="8479e-194">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="8479e-194">subjectNameFormatString</span></span>|<span data-ttu-id="8479e-195">字符串</span><span class="sxs-lookup"><span data-stu-id="8479e-195">String</span></span>|<span data-ttu-id="8479e-196">自定义格式使用 SubjectNameFormat = 自定义。</span><span class="sxs-lookup"><span data-stu-id="8479e-196">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="8479e-197">示例： CN = {{EmailAddress}} E = {{EmailAddress}}，OU = 企业用户，O = Contoso Corporation L = 雷德蒙德，ST = WA，C = US</span><span class="sxs-lookup"><span data-stu-id="8479e-197">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="8479e-198">keyUsage</span><span class="sxs-lookup"><span data-stu-id="8479e-198">keyUsage</span></span>|[<span data-ttu-id="8479e-199">keyUsages</span><span class="sxs-lookup"><span data-stu-id="8479e-199">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="8479e-200">SCEP 密钥用法。</span><span class="sxs-lookup"><span data-stu-id="8479e-200">SCEP Key Usage.</span></span> <span data-ttu-id="8479e-201">可取值为：`keyEncipherment`、`digitalSignature`。</span><span class="sxs-lookup"><span data-stu-id="8479e-201">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="8479e-202">keySize</span><span class="sxs-lookup"><span data-stu-id="8479e-202">keySize</span></span>|[<span data-ttu-id="8479e-203">keySize</span><span class="sxs-lookup"><span data-stu-id="8479e-203">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="8479e-204">SCEP 密钥大小。</span><span class="sxs-lookup"><span data-stu-id="8479e-204">SCEP Key Size.</span></span> <span data-ttu-id="8479e-205">可取值为：`size1024`、`size2048`。</span><span class="sxs-lookup"><span data-stu-id="8479e-205">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="8479e-206">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="8479e-206">extendedKeyUsages</span></span>|<span data-ttu-id="8479e-207">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)集合</span><span class="sxs-lookup"><span data-stu-id="8479e-207">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="8479e-208">扩展的密钥用法 (EKU) 设置。</span><span class="sxs-lookup"><span data-stu-id="8479e-208">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="8479e-209">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="8479e-209">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="8479e-210">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="8479e-210">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="8479e-211">字符串</span><span class="sxs-lookup"><span data-stu-id="8479e-211">String</span></span>|<span data-ttu-id="8479e-212">定义 AAD 属性的自定义字符串。</span><span class="sxs-lookup"><span data-stu-id="8479e-212">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="8479e-213">certificateStore</span><span class="sxs-lookup"><span data-stu-id="8479e-213">certificateStore</span></span>|[<span data-ttu-id="8479e-214">certificateStore</span><span class="sxs-lookup"><span data-stu-id="8479e-214">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="8479e-215">目标存储证书。</span><span class="sxs-lookup"><span data-stu-id="8479e-215">Target store certificate.</span></span> <span data-ttu-id="8479e-216">可取值为：`user`、`machine`。</span><span class="sxs-lookup"><span data-stu-id="8479e-216">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="8479e-217">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="8479e-217">customSubjectAlternativeNames</span></span>|<span data-ttu-id="8479e-218">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)集合</span><span class="sxs-lookup"><span data-stu-id="8479e-218">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="8479e-219">自定义主题 Alterantive 名称设置。</span><span class="sxs-lookup"><span data-stu-id="8479e-219">Custom Subject Alterantive Name Settings.</span></span> <span data-ttu-id="8479e-220">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="8479e-220">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="8479e-221">响应</span><span class="sxs-lookup"><span data-stu-id="8479e-221">Response</span></span>
<span data-ttu-id="8479e-222">如果成功，此方法返回`201 Created`响应代码和响应正文中的[iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8479e-222">If successful, this method returns a `201 Created` response code and a [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8479e-223">示例</span><span class="sxs-lookup"><span data-stu-id="8479e-223">Example</span></span>
### <a name="request"></a><span data-ttu-id="8479e-224">请求</span><span class="sxs-lookup"><span data-stu-id="8479e-224">Request</span></span>
<span data-ttu-id="8479e-225">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8479e-225">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1223

{
  "@odata.type": "#microsoft.graph.iosScepCertificateProfile",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "certificateStore": "machine",
  "customSubjectAlternativeNames": [
    {
      "@odata.type": "microsoft.graph.customSubjectAlternativeName",
      "sanType": "emailAddress",
      "name": "Name value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="8479e-226">响应</span><span class="sxs-lookup"><span data-stu-id="8479e-226">Response</span></span>
<span data-ttu-id="8479e-p122">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8479e-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1331

{
  "@odata.type": "#microsoft.graph.iosScepCertificateProfile",
  "id": "0deb8dbf-8dbf-0deb-bf8d-eb0dbf8deb0d",
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
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "certificateStore": "machine",
  "customSubjectAlternativeNames": [
    {
      "@odata.type": "microsoft.graph.customSubjectAlternativeName",
      "sanType": "emailAddress",
      "name": "Name value"
    }
  ]
}
```





