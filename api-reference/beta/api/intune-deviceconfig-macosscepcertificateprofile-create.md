---
title: 创建 macOSScepCertificateProfile
description: 创建新的 macOSScepCertificateProfile 对象。
author: tfitzmac
ms.openlocfilehash: 30d6ea30d2fb7eaa9a3603f46143d8015e593eeb
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27355354"
---
# <a name="create-macosscepcertificateprofile"></a><span data-ttu-id="e6d87-103">创建 macOSScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="e6d87-103">Create macOSScepCertificateProfile</span></span>

> <span data-ttu-id="e6d87-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e6d87-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e6d87-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e6d87-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e6d87-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e6d87-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e6d87-107">创建新的[macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e6d87-107">Create a new [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e6d87-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="e6d87-108">Prerequisites</span></span>
<span data-ttu-id="e6d87-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="e6d87-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e6d87-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e6d87-111">Permission type</span></span>|<span data-ttu-id="e6d87-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e6d87-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e6d87-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e6d87-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e6d87-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6d87-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e6d87-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e6d87-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e6d87-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e6d87-116">Not supported.</span></span>|
|<span data-ttu-id="e6d87-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e6d87-117">Application</span></span>|<span data-ttu-id="e6d87-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="e6d87-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e6d87-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e6d87-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="e6d87-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e6d87-120">Request headers</span></span>
|<span data-ttu-id="e6d87-121">标头</span><span class="sxs-lookup"><span data-stu-id="e6d87-121">Header</span></span>|<span data-ttu-id="e6d87-122">值</span><span class="sxs-lookup"><span data-stu-id="e6d87-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e6d87-123">授权</span><span class="sxs-lookup"><span data-stu-id="e6d87-123">Authorization</span></span>|<span data-ttu-id="e6d87-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e6d87-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e6d87-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e6d87-125">Accept</span></span>|<span data-ttu-id="e6d87-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e6d87-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e6d87-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e6d87-127">Request body</span></span>
<span data-ttu-id="e6d87-128">在请求正文中，提供 macOSScepCertificateProfile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e6d87-128">In the request body, supply a JSON representation for the macOSScepCertificateProfile object.</span></span>

<span data-ttu-id="e6d87-129">下表显示时创建 macOSScepCertificateProfile 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e6d87-129">The following table shows the properties that are required when you create the macOSScepCertificateProfile.</span></span>

|<span data-ttu-id="e6d87-130">属性</span><span class="sxs-lookup"><span data-stu-id="e6d87-130">Property</span></span>|<span data-ttu-id="e6d87-131">类型</span><span class="sxs-lookup"><span data-stu-id="e6d87-131">Type</span></span>|<span data-ttu-id="e6d87-132">说明</span><span class="sxs-lookup"><span data-stu-id="e6d87-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6d87-133">id</span><span class="sxs-lookup"><span data-stu-id="e6d87-133">id</span></span>|<span data-ttu-id="e6d87-134">String</span><span class="sxs-lookup"><span data-stu-id="e6d87-134">String</span></span>|<span data-ttu-id="e6d87-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e6d87-135">Key of the entity.</span></span> <span data-ttu-id="e6d87-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e6d87-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e6d87-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e6d87-137">lastModifiedDateTime</span></span>|<span data-ttu-id="e6d87-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e6d87-138">DateTimeOffset</span></span>|<span data-ttu-id="e6d87-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="e6d87-139">DateTime the object was last modified.</span></span> <span data-ttu-id="e6d87-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e6d87-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e6d87-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e6d87-141">roleScopeTagIds</span></span>|<span data-ttu-id="e6d87-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="e6d87-142">String collection</span></span>|<span data-ttu-id="e6d87-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="e6d87-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e6d87-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e6d87-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e6d87-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="e6d87-145">supportsScopeTags</span></span>|<span data-ttu-id="e6d87-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="e6d87-146">Boolean</span></span>|<span data-ttu-id="e6d87-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="e6d87-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="e6d87-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="e6d87-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="e6d87-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="e6d87-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="e6d87-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="e6d87-150">This property is read-only.</span></span> <span data-ttu-id="e6d87-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e6d87-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e6d87-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e6d87-152">createdDateTime</span></span>|<span data-ttu-id="e6d87-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e6d87-153">DateTimeOffset</span></span>|<span data-ttu-id="e6d87-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="e6d87-154">DateTime the object was created.</span></span> <span data-ttu-id="e6d87-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e6d87-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e6d87-156">description</span><span class="sxs-lookup"><span data-stu-id="e6d87-156">description</span></span>|<span data-ttu-id="e6d87-157">String</span><span class="sxs-lookup"><span data-stu-id="e6d87-157">String</span></span>|<span data-ttu-id="e6d87-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="e6d87-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e6d87-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e6d87-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e6d87-160">displayName</span><span class="sxs-lookup"><span data-stu-id="e6d87-160">displayName</span></span>|<span data-ttu-id="e6d87-161">String</span><span class="sxs-lookup"><span data-stu-id="e6d87-161">String</span></span>|<span data-ttu-id="e6d87-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="e6d87-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e6d87-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e6d87-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e6d87-164">version</span><span class="sxs-lookup"><span data-stu-id="e6d87-164">version</span></span>|<span data-ttu-id="e6d87-165">Int32</span><span class="sxs-lookup"><span data-stu-id="e6d87-165">Int32</span></span>|<span data-ttu-id="e6d87-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="e6d87-166">Version of the device configuration.</span></span> <span data-ttu-id="e6d87-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e6d87-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e6d87-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="e6d87-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="e6d87-169">Int32</span><span class="sxs-lookup"><span data-stu-id="e6d87-169">Int32</span></span>|<span data-ttu-id="e6d87-170">证书续订阈值百分比。</span><span class="sxs-lookup"><span data-stu-id="e6d87-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="e6d87-171">继承自[macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="e6d87-171">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="e6d87-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="e6d87-172">subjectNameFormat</span></span>|[<span data-ttu-id="e6d87-173">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="e6d87-173">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="e6d87-174">证书使用者名称格式。</span><span class="sxs-lookup"><span data-stu-id="e6d87-174">Certificate Subject Name Format.</span></span> <span data-ttu-id="e6d87-175">继承自[macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="e6d87-175">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="e6d87-176">可取值为：`commonName`、`commonNameAsEmail`、`custom`、`commonNameIncludingEmail`、`commonNameAsIMEI`、`commonNameAsSerialNumber`。</span><span class="sxs-lookup"><span data-stu-id="e6d87-176">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="e6d87-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="e6d87-177">subjectAlternativeNameType</span></span>|[<span data-ttu-id="e6d87-178">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="e6d87-178">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="e6d87-179">证书使用者替代名称类型。</span><span class="sxs-lookup"><span data-stu-id="e6d87-179">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="e6d87-180">继承自[macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="e6d87-180">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="e6d87-181">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService`。</span><span class="sxs-lookup"><span data-stu-id="e6d87-181">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="e6d87-182">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="e6d87-182">certificateValidityPeriodValue</span></span>|<span data-ttu-id="e6d87-183">Int32</span><span class="sxs-lookup"><span data-stu-id="e6d87-183">Int32</span></span>|<span data-ttu-id="e6d87-184">证书有效期限的值。</span><span class="sxs-lookup"><span data-stu-id="e6d87-184">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="e6d87-185">继承自[macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="e6d87-185">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="e6d87-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="e6d87-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="e6d87-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="e6d87-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="e6d87-188">证书有效期限的小数位数。</span><span class="sxs-lookup"><span data-stu-id="e6d87-188">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="e6d87-189">继承自[macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="e6d87-189">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="e6d87-190">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="e6d87-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="e6d87-191">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="e6d87-191">scepServerUrls</span></span>|<span data-ttu-id="e6d87-192">String 集合</span><span class="sxs-lookup"><span data-stu-id="e6d87-192">String collection</span></span>|<span data-ttu-id="e6d87-193">SCEP 服务器 Url(s)。</span><span class="sxs-lookup"><span data-stu-id="e6d87-193">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="e6d87-194">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="e6d87-194">subjectNameFormatString</span></span>|<span data-ttu-id="e6d87-195">字符串</span><span class="sxs-lookup"><span data-stu-id="e6d87-195">String</span></span>|<span data-ttu-id="e6d87-196">自定义格式使用 SubjectNameFormat = 自定义。</span><span class="sxs-lookup"><span data-stu-id="e6d87-196">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="e6d87-197">示例： CN = {{EmailAddress}} E = {{EmailAddress}}，OU = 企业用户，O = Contoso Corporation L = 雷德蒙德，ST = WA，C = US</span><span class="sxs-lookup"><span data-stu-id="e6d87-197">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="e6d87-198">keyUsage</span><span class="sxs-lookup"><span data-stu-id="e6d87-198">keyUsage</span></span>|[<span data-ttu-id="e6d87-199">keyUsages</span><span class="sxs-lookup"><span data-stu-id="e6d87-199">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="e6d87-200">SCEP 密钥用法。</span><span class="sxs-lookup"><span data-stu-id="e6d87-200">SCEP Key Usage.</span></span> <span data-ttu-id="e6d87-201">可取值为：`keyEncipherment`、`digitalSignature`。</span><span class="sxs-lookup"><span data-stu-id="e6d87-201">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="e6d87-202">keySize</span><span class="sxs-lookup"><span data-stu-id="e6d87-202">keySize</span></span>|[<span data-ttu-id="e6d87-203">keySize</span><span class="sxs-lookup"><span data-stu-id="e6d87-203">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="e6d87-204">SCEP 密钥大小。</span><span class="sxs-lookup"><span data-stu-id="e6d87-204">SCEP Key Size.</span></span> <span data-ttu-id="e6d87-205">可取值为：`size1024`、`size2048`。</span><span class="sxs-lookup"><span data-stu-id="e6d87-205">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="e6d87-206">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="e6d87-206">hashAlgorithm</span></span>|[<span data-ttu-id="e6d87-207">hashAlgorithms</span><span class="sxs-lookup"><span data-stu-id="e6d87-207">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="e6d87-208">SCEP 哈希算法。</span><span class="sxs-lookup"><span data-stu-id="e6d87-208">SCEP Hash Algorithm.</span></span> <span data-ttu-id="e6d87-209">可取值为：`sha1`、`sha2`。</span><span class="sxs-lookup"><span data-stu-id="e6d87-209">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="e6d87-210">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="e6d87-210">extendedKeyUsages</span></span>|<span data-ttu-id="e6d87-211">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)集合</span><span class="sxs-lookup"><span data-stu-id="e6d87-211">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="e6d87-212">扩展的密钥用法 (EKU) 设置。</span><span class="sxs-lookup"><span data-stu-id="e6d87-212">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="e6d87-213">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="e6d87-213">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="e6d87-214">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="e6d87-214">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="e6d87-215">字符串</span><span class="sxs-lookup"><span data-stu-id="e6d87-215">String</span></span>|<span data-ttu-id="e6d87-216">定义 AAD 属性的自定义字符串。</span><span class="sxs-lookup"><span data-stu-id="e6d87-216">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="e6d87-217">响应</span><span class="sxs-lookup"><span data-stu-id="e6d87-217">Response</span></span>
<span data-ttu-id="e6d87-218">如果成功，此方法返回`201 Created`响应代码和响应正文中的[macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e6d87-218">If successful, this method returns a `201 Created` response code and a [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6d87-219">示例</span><span class="sxs-lookup"><span data-stu-id="e6d87-219">Example</span></span>
### <a name="request"></a><span data-ttu-id="e6d87-220">请求</span><span class="sxs-lookup"><span data-stu-id="e6d87-220">Request</span></span>
<span data-ttu-id="e6d87-221">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e6d87-221">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1029

{
  "@odata.type": "#microsoft.graph.macOSScepCertificateProfile",
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
  "hashAlgorithm": "sha2",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```

### <a name="response"></a><span data-ttu-id="e6d87-222">响应</span><span class="sxs-lookup"><span data-stu-id="e6d87-222">Response</span></span>
<span data-ttu-id="e6d87-p121">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e6d87-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1137

{
  "@odata.type": "#microsoft.graph.macOSScepCertificateProfile",
  "id": "78c3929d-929d-78c3-9d92-c3789d92c378",
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
  "hashAlgorithm": "sha2",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```





