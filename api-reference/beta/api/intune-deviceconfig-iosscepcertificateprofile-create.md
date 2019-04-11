---
title: 创建 iosScepCertificateProfile
description: 创建新的 iosScepCertificateProfile 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 272089b0280e92cca47bdb191f72c02d84031939
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31778234"
---
# <a name="create-iosscepcertificateprofile"></a><span data-ttu-id="c5957-103">创建 iosScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="c5957-103">Create iosScepCertificateProfile</span></span>

> <span data-ttu-id="c5957-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c5957-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c5957-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c5957-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5957-106">创建新的[iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c5957-106">Create a new [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c5957-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="c5957-107">Prerequisites</span></span>
<span data-ttu-id="c5957-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c5957-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5957-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c5957-110">Permission type</span></span>|<span data-ttu-id="c5957-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c5957-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c5957-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c5957-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c5957-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5957-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c5957-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c5957-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c5957-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c5957-115">Not supported.</span></span>|
|<span data-ttu-id="c5957-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c5957-116">Application</span></span>|<span data-ttu-id="c5957-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="c5957-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c5957-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c5957-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c5957-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c5957-119">Request headers</span></span>
|<span data-ttu-id="c5957-120">标头</span><span class="sxs-lookup"><span data-stu-id="c5957-120">Header</span></span>|<span data-ttu-id="c5957-121">值</span><span class="sxs-lookup"><span data-stu-id="c5957-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c5957-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c5957-122">Authorization</span></span>|<span data-ttu-id="c5957-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c5957-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c5957-124">接受</span><span class="sxs-lookup"><span data-stu-id="c5957-124">Accept</span></span>|<span data-ttu-id="c5957-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c5957-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5957-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c5957-126">Request body</span></span>
<span data-ttu-id="c5957-127">在请求正文中, 提供 iosScepCertificateProfile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c5957-127">In the request body, supply a JSON representation for the iosScepCertificateProfile object.</span></span>

<span data-ttu-id="c5957-128">下表显示创建 iosScepCertificateProfile 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c5957-128">The following table shows the properties that are required when you create the iosScepCertificateProfile.</span></span>

|<span data-ttu-id="c5957-129">属性</span><span class="sxs-lookup"><span data-stu-id="c5957-129">Property</span></span>|<span data-ttu-id="c5957-130">类型</span><span class="sxs-lookup"><span data-stu-id="c5957-130">Type</span></span>|<span data-ttu-id="c5957-131">说明</span><span class="sxs-lookup"><span data-stu-id="c5957-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5957-132">id</span><span class="sxs-lookup"><span data-stu-id="c5957-132">id</span></span>|<span data-ttu-id="c5957-133">String</span><span class="sxs-lookup"><span data-stu-id="c5957-133">String</span></span>|<span data-ttu-id="c5957-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c5957-134">Key of the entity.</span></span> <span data-ttu-id="c5957-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c5957-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5957-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c5957-136">lastModifiedDateTime</span></span>|<span data-ttu-id="c5957-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5957-137">DateTimeOffset</span></span>|<span data-ttu-id="c5957-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c5957-138">DateTime the object was last modified.</span></span> <span data-ttu-id="c5957-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c5957-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5957-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c5957-140">roleScopeTagIds</span></span>|<span data-ttu-id="c5957-141">String 集合</span><span class="sxs-lookup"><span data-stu-id="c5957-141">String collection</span></span>|<span data-ttu-id="c5957-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="c5957-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c5957-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c5957-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5957-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c5957-144">supportsScopeTags</span></span>|<span data-ttu-id="c5957-145">布尔值</span><span class="sxs-lookup"><span data-stu-id="c5957-145">Boolean</span></span>|<span data-ttu-id="c5957-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="c5957-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c5957-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="c5957-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c5957-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="c5957-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c5957-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c5957-149">This property is read-only.</span></span> <span data-ttu-id="c5957-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c5957-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5957-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c5957-151">createdDateTime</span></span>|<span data-ttu-id="c5957-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5957-152">DateTimeOffset</span></span>|<span data-ttu-id="c5957-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c5957-153">DateTime the object was created.</span></span> <span data-ttu-id="c5957-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c5957-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5957-155">description</span><span class="sxs-lookup"><span data-stu-id="c5957-155">description</span></span>|<span data-ttu-id="c5957-156">String</span><span class="sxs-lookup"><span data-stu-id="c5957-156">String</span></span>|<span data-ttu-id="c5957-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="c5957-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c5957-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c5957-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5957-159">displayName</span><span class="sxs-lookup"><span data-stu-id="c5957-159">displayName</span></span>|<span data-ttu-id="c5957-160">String</span><span class="sxs-lookup"><span data-stu-id="c5957-160">String</span></span>|<span data-ttu-id="c5957-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="c5957-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c5957-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c5957-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5957-163">version</span><span class="sxs-lookup"><span data-stu-id="c5957-163">version</span></span>|<span data-ttu-id="c5957-164">Int32</span><span class="sxs-lookup"><span data-stu-id="c5957-164">Int32</span></span>|<span data-ttu-id="c5957-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="c5957-165">Version of the device configuration.</span></span> <span data-ttu-id="c5957-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c5957-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5957-167">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="c5957-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="c5957-168">Int32</span><span class="sxs-lookup"><span data-stu-id="c5957-168">Int32</span></span>|<span data-ttu-id="c5957-169">证书续订阈值百分比。</span><span class="sxs-lookup"><span data-stu-id="c5957-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="c5957-170">从[iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)继承的有效值1到99</span><span class="sxs-lookup"><span data-stu-id="c5957-170">Valid values 1 to 99 Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="c5957-171">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="c5957-171">subjectNameFormat</span></span>|[<span data-ttu-id="c5957-172">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="c5957-172">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="c5957-173">证书使用者名称格式。</span><span class="sxs-lookup"><span data-stu-id="c5957-173">Certificate Subject Name Format.</span></span> <span data-ttu-id="c5957-174">继承自[iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="c5957-174">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="c5957-175">可取值为：`commonName`、`commonNameAsEmail`、`custom`、`commonNameIncludingEmail`、`commonNameAsIMEI`、`commonNameAsSerialNumber`。</span><span class="sxs-lookup"><span data-stu-id="c5957-175">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="c5957-176">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="c5957-176">subjectAlternativeNameType</span></span>|[<span data-ttu-id="c5957-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="c5957-177">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="c5957-178">证书使用者备用名称类型。</span><span class="sxs-lookup"><span data-stu-id="c5957-178">Certificate Subject Alternative Name type.</span></span> <span data-ttu-id="c5957-179">继承自[iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="c5957-179">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="c5957-180">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute` 或 `domainNameService`。</span><span class="sxs-lookup"><span data-stu-id="c5957-180">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="c5957-181">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="c5957-181">certificateValidityPeriodValue</span></span>|<span data-ttu-id="c5957-182">Int32</span><span class="sxs-lookup"><span data-stu-id="c5957-182">Int32</span></span>|<span data-ttu-id="c5957-183">证书有效期限的值。</span><span class="sxs-lookup"><span data-stu-id="c5957-183">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="c5957-184">继承自[iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="c5957-184">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="c5957-185">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="c5957-185">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="c5957-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="c5957-186">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="c5957-187">证书有效期的小数位数。</span><span class="sxs-lookup"><span data-stu-id="c5957-187">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="c5957-188">继承自[iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="c5957-188">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="c5957-189">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="c5957-189">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="c5957-190">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="c5957-190">scepServerUrls</span></span>|<span data-ttu-id="c5957-191">String 集合</span><span class="sxs-lookup"><span data-stu-id="c5957-191">String collection</span></span>|<span data-ttu-id="c5957-192">SCEP 服务器 Url。</span><span class="sxs-lookup"><span data-stu-id="c5957-192">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="c5957-193">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="c5957-193">subjectNameFormatString</span></span>|<span data-ttu-id="c5957-194">String</span><span class="sxs-lookup"><span data-stu-id="c5957-194">String</span></span>|<span data-ttu-id="c5957-195">要与 SubjectNameFormat = custom 一起使用的自定义格式。</span><span class="sxs-lookup"><span data-stu-id="c5957-195">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="c5957-196">示例: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = 企业用户, O = Contoso Corporation, L = Redmond, ST = WA, C = US</span><span class="sxs-lookup"><span data-stu-id="c5957-196">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="c5957-197">keyUsage</span><span class="sxs-lookup"><span data-stu-id="c5957-197">keyUsage</span></span>|[<span data-ttu-id="c5957-198">keyUsages</span><span class="sxs-lookup"><span data-stu-id="c5957-198">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="c5957-199">SCEP 密钥用法。</span><span class="sxs-lookup"><span data-stu-id="c5957-199">SCEP Key Usage.</span></span> <span data-ttu-id="c5957-200">可取值为：`keyEncipherment`、`digitalSignature`。</span><span class="sxs-lookup"><span data-stu-id="c5957-200">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="c5957-201">keySize</span><span class="sxs-lookup"><span data-stu-id="c5957-201">keySize</span></span>|[<span data-ttu-id="c5957-202">keySize</span><span class="sxs-lookup"><span data-stu-id="c5957-202">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="c5957-203">SCEP 密钥大小。</span><span class="sxs-lookup"><span data-stu-id="c5957-203">SCEP Key Size.</span></span> <span data-ttu-id="c5957-204">可取值为：`size1024`、`size2048`。</span><span class="sxs-lookup"><span data-stu-id="c5957-204">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="c5957-205">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="c5957-205">extendedKeyUsages</span></span>|<span data-ttu-id="c5957-206">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)集合</span><span class="sxs-lookup"><span data-stu-id="c5957-206">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="c5957-207">扩展密钥用法 (EKU) 设置。</span><span class="sxs-lookup"><span data-stu-id="c5957-207">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="c5957-208">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="c5957-208">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="c5957-209">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="c5957-209">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="c5957-210">String</span><span class="sxs-lookup"><span data-stu-id="c5957-210">String</span></span>|<span data-ttu-id="c5957-211">定义 AAD 属性的自定义字符串。</span><span class="sxs-lookup"><span data-stu-id="c5957-211">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="c5957-212">certificateStore</span><span class="sxs-lookup"><span data-stu-id="c5957-212">certificateStore</span></span>|[<span data-ttu-id="c5957-213">certificateStore</span><span class="sxs-lookup"><span data-stu-id="c5957-213">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="c5957-214">目标存储证书。</span><span class="sxs-lookup"><span data-stu-id="c5957-214">Target store certificate.</span></span> <span data-ttu-id="c5957-215">可取值为：`user`、`machine`。</span><span class="sxs-lookup"><span data-stu-id="c5957-215">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="c5957-216">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="c5957-216">customSubjectAlternativeNames</span></span>|<span data-ttu-id="c5957-217">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)集合</span><span class="sxs-lookup"><span data-stu-id="c5957-217">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="c5957-218">自定义主题备用名称设置。</span><span class="sxs-lookup"><span data-stu-id="c5957-218">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="c5957-219">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="c5957-219">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="c5957-220">响应</span><span class="sxs-lookup"><span data-stu-id="c5957-220">Response</span></span>
<span data-ttu-id="c5957-221">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c5957-221">If successful, this method returns a `201 Created` response code and a [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5957-222">示例</span><span class="sxs-lookup"><span data-stu-id="c5957-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="c5957-223">请求</span><span class="sxs-lookup"><span data-stu-id="c5957-223">Request</span></span>
<span data-ttu-id="c5957-224">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c5957-224">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1159

{
  "@odata.type": "#microsoft.graph.iosScepCertificateProfile",
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

### <a name="response"></a><span data-ttu-id="c5957-225">响应</span><span class="sxs-lookup"><span data-stu-id="c5957-225">Response</span></span>
<span data-ttu-id="c5957-p121">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c5957-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





