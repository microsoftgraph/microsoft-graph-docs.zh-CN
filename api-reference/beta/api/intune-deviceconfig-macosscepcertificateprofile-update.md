---
title: 更新 macOSScepCertificateProfile
description: 更新 macOSScepCertificateProfile 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9e654208e006b04c846721fe2cd3446183553902
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27968020"
---
# <a name="update-macosscepcertificateprofile"></a><span data-ttu-id="d288b-103">更新 macOSScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="d288b-103">Update macOSScepCertificateProfile</span></span>

> <span data-ttu-id="d288b-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d288b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d288b-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d288b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d288b-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d288b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d288b-107">更新[macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d288b-107">Update the properties of a [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d288b-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="d288b-108">Prerequisites</span></span>
<span data-ttu-id="d288b-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="d288b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d288b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d288b-111">Permission type</span></span>|<span data-ttu-id="d288b-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d288b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d288b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d288b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d288b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d288b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d288b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d288b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d288b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d288b-116">Not supported.</span></span>|
|<span data-ttu-id="d288b-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d288b-117">Application</span></span>|<span data-ttu-id="d288b-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="d288b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d288b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d288b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="d288b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d288b-120">Request headers</span></span>
|<span data-ttu-id="d288b-121">标头</span><span class="sxs-lookup"><span data-stu-id="d288b-121">Header</span></span>|<span data-ttu-id="d288b-122">值</span><span class="sxs-lookup"><span data-stu-id="d288b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d288b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d288b-123">Authorization</span></span>|<span data-ttu-id="d288b-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d288b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d288b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d288b-125">Accept</span></span>|<span data-ttu-id="d288b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d288b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d288b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d288b-127">Request body</span></span>
<span data-ttu-id="d288b-128">在请求正文中，提供[macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d288b-128">In the request body, supply a JSON representation for the [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) object.</span></span>

<span data-ttu-id="d288b-129">下表显示时创建[macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d288b-129">The following table shows the properties that are required when you create the [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md).</span></span>

|<span data-ttu-id="d288b-130">属性</span><span class="sxs-lookup"><span data-stu-id="d288b-130">Property</span></span>|<span data-ttu-id="d288b-131">类型</span><span class="sxs-lookup"><span data-stu-id="d288b-131">Type</span></span>|<span data-ttu-id="d288b-132">说明</span><span class="sxs-lookup"><span data-stu-id="d288b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d288b-133">id</span><span class="sxs-lookup"><span data-stu-id="d288b-133">id</span></span>|<span data-ttu-id="d288b-134">String</span><span class="sxs-lookup"><span data-stu-id="d288b-134">String</span></span>|<span data-ttu-id="d288b-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d288b-135">Key of the entity.</span></span> <span data-ttu-id="d288b-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d288b-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d288b-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d288b-137">lastModifiedDateTime</span></span>|<span data-ttu-id="d288b-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d288b-138">DateTimeOffset</span></span>|<span data-ttu-id="d288b-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="d288b-139">DateTime the object was last modified.</span></span> <span data-ttu-id="d288b-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d288b-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d288b-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d288b-141">roleScopeTagIds</span></span>|<span data-ttu-id="d288b-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="d288b-142">String collection</span></span>|<span data-ttu-id="d288b-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="d288b-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d288b-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d288b-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d288b-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d288b-145">supportsScopeTags</span></span>|<span data-ttu-id="d288b-146">布尔</span><span class="sxs-lookup"><span data-stu-id="d288b-146">Boolean</span></span>|<span data-ttu-id="d288b-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="d288b-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d288b-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="d288b-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d288b-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="d288b-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d288b-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="d288b-150">This property is read-only.</span></span> <span data-ttu-id="d288b-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d288b-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d288b-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d288b-152">createdDateTime</span></span>|<span data-ttu-id="d288b-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d288b-153">DateTimeOffset</span></span>|<span data-ttu-id="d288b-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="d288b-154">DateTime the object was created.</span></span> <span data-ttu-id="d288b-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d288b-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d288b-156">description</span><span class="sxs-lookup"><span data-stu-id="d288b-156">description</span></span>|<span data-ttu-id="d288b-157">String</span><span class="sxs-lookup"><span data-stu-id="d288b-157">String</span></span>|<span data-ttu-id="d288b-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="d288b-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d288b-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d288b-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d288b-160">displayName</span><span class="sxs-lookup"><span data-stu-id="d288b-160">displayName</span></span>|<span data-ttu-id="d288b-161">String</span><span class="sxs-lookup"><span data-stu-id="d288b-161">String</span></span>|<span data-ttu-id="d288b-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="d288b-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d288b-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d288b-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d288b-164">version</span><span class="sxs-lookup"><span data-stu-id="d288b-164">version</span></span>|<span data-ttu-id="d288b-165">Int32</span><span class="sxs-lookup"><span data-stu-id="d288b-165">Int32</span></span>|<span data-ttu-id="d288b-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="d288b-166">Version of the device configuration.</span></span> <span data-ttu-id="d288b-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d288b-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d288b-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="d288b-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="d288b-169">Int32</span><span class="sxs-lookup"><span data-stu-id="d288b-169">Int32</span></span>|<span data-ttu-id="d288b-170">证书续订阈值百分比。</span><span class="sxs-lookup"><span data-stu-id="d288b-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="d288b-171">继承自[macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="d288b-171">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="d288b-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="d288b-172">subjectNameFormat</span></span>|[<span data-ttu-id="d288b-173">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="d288b-173">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="d288b-174">证书使用者名称格式。</span><span class="sxs-lookup"><span data-stu-id="d288b-174">Certificate Subject Name Format.</span></span> <span data-ttu-id="d288b-175">继承自[macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="d288b-175">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="d288b-176">可取值为：`commonName`、`commonNameAsEmail`、`custom`、`commonNameIncludingEmail`、`commonNameAsIMEI`、`commonNameAsSerialNumber`。</span><span class="sxs-lookup"><span data-stu-id="d288b-176">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="d288b-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="d288b-177">subjectAlternativeNameType</span></span>|[<span data-ttu-id="d288b-178">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="d288b-178">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="d288b-179">证书使用者替代名称类型。</span><span class="sxs-lookup"><span data-stu-id="d288b-179">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="d288b-180">继承自[macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="d288b-180">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="d288b-181">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService`。</span><span class="sxs-lookup"><span data-stu-id="d288b-181">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="d288b-182">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="d288b-182">certificateValidityPeriodValue</span></span>|<span data-ttu-id="d288b-183">Int32</span><span class="sxs-lookup"><span data-stu-id="d288b-183">Int32</span></span>|<span data-ttu-id="d288b-184">证书有效期限的值。</span><span class="sxs-lookup"><span data-stu-id="d288b-184">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="d288b-185">继承自[macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="d288b-185">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="d288b-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="d288b-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="d288b-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="d288b-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="d288b-188">证书有效期限的小数位数。</span><span class="sxs-lookup"><span data-stu-id="d288b-188">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="d288b-189">继承自[macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="d288b-189">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="d288b-190">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="d288b-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="d288b-191">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="d288b-191">scepServerUrls</span></span>|<span data-ttu-id="d288b-192">String 集合</span><span class="sxs-lookup"><span data-stu-id="d288b-192">String collection</span></span>|<span data-ttu-id="d288b-193">SCEP 服务器 Url(s)。</span><span class="sxs-lookup"><span data-stu-id="d288b-193">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="d288b-194">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="d288b-194">subjectNameFormatString</span></span>|<span data-ttu-id="d288b-195">字符串</span><span class="sxs-lookup"><span data-stu-id="d288b-195">String</span></span>|<span data-ttu-id="d288b-196">自定义格式使用 SubjectNameFormat = 自定义。</span><span class="sxs-lookup"><span data-stu-id="d288b-196">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="d288b-197">示例： CN = {{EmailAddress}} E = {{EmailAddress}}，OU = 企业用户，O = Contoso Corporation L = 雷德蒙德，ST = WA，C = US</span><span class="sxs-lookup"><span data-stu-id="d288b-197">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="d288b-198">keyUsage</span><span class="sxs-lookup"><span data-stu-id="d288b-198">keyUsage</span></span>|[<span data-ttu-id="d288b-199">keyUsages</span><span class="sxs-lookup"><span data-stu-id="d288b-199">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="d288b-200">SCEP 密钥用法。</span><span class="sxs-lookup"><span data-stu-id="d288b-200">SCEP Key Usage.</span></span> <span data-ttu-id="d288b-201">可取值为：`keyEncipherment`、`digitalSignature`。</span><span class="sxs-lookup"><span data-stu-id="d288b-201">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="d288b-202">keySize</span><span class="sxs-lookup"><span data-stu-id="d288b-202">keySize</span></span>|[<span data-ttu-id="d288b-203">keySize</span><span class="sxs-lookup"><span data-stu-id="d288b-203">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="d288b-204">SCEP 密钥大小。</span><span class="sxs-lookup"><span data-stu-id="d288b-204">SCEP Key Size.</span></span> <span data-ttu-id="d288b-205">可取值为：`size1024`、`size2048`。</span><span class="sxs-lookup"><span data-stu-id="d288b-205">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="d288b-206">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="d288b-206">hashAlgorithm</span></span>|[<span data-ttu-id="d288b-207">hashAlgorithms</span><span class="sxs-lookup"><span data-stu-id="d288b-207">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="d288b-208">SCEP 哈希算法。</span><span class="sxs-lookup"><span data-stu-id="d288b-208">SCEP Hash Algorithm.</span></span> <span data-ttu-id="d288b-209">可取值为：`sha1`、`sha2`。</span><span class="sxs-lookup"><span data-stu-id="d288b-209">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="d288b-210">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="d288b-210">extendedKeyUsages</span></span>|<span data-ttu-id="d288b-211">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)集合</span><span class="sxs-lookup"><span data-stu-id="d288b-211">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="d288b-212">扩展的密钥用法 (EKU) 设置。</span><span class="sxs-lookup"><span data-stu-id="d288b-212">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="d288b-213">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="d288b-213">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="d288b-214">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="d288b-214">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="d288b-215">字符串</span><span class="sxs-lookup"><span data-stu-id="d288b-215">String</span></span>|<span data-ttu-id="d288b-216">定义 AAD 属性的自定义字符串。</span><span class="sxs-lookup"><span data-stu-id="d288b-216">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="d288b-217">响应</span><span class="sxs-lookup"><span data-stu-id="d288b-217">Response</span></span>
<span data-ttu-id="d288b-218">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d288b-218">If successful, this method returns a `200 OK` response code and an updated [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d288b-219">示例</span><span class="sxs-lookup"><span data-stu-id="d288b-219">Example</span></span>
### <a name="request"></a><span data-ttu-id="d288b-220">请求</span><span class="sxs-lookup"><span data-stu-id="d288b-220">Request</span></span>
<span data-ttu-id="d288b-221">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d288b-221">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 963

{
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

### <a name="response"></a><span data-ttu-id="d288b-222">响应</span><span class="sxs-lookup"><span data-stu-id="d288b-222">Response</span></span>
<span data-ttu-id="d288b-p121">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d288b-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





