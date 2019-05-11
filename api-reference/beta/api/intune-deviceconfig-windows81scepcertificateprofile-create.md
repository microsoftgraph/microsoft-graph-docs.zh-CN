---
title: 创建 windows81SCEPCertificateProfile
description: 创建新的 windows81SCEPCertificateProfile 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 74498b693f98a47211d3c7222e58e5473258ac84
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33918232"
---
# <a name="create-windows81scepcertificateprofile"></a><span data-ttu-id="51dea-103">创建 windows81SCEPCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="51dea-103">Create windows81SCEPCertificateProfile</span></span>

> <span data-ttu-id="51dea-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="51dea-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="51dea-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="51dea-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51dea-106">创建新的[windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="51dea-106">Create a new [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="51dea-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="51dea-107">Prerequisites</span></span>
<span data-ttu-id="51dea-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="51dea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51dea-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="51dea-110">Permission type</span></span>|<span data-ttu-id="51dea-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="51dea-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51dea-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="51dea-112">Delegated (work or school account)</span></span>|<span data-ttu-id="51dea-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51dea-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="51dea-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="51dea-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51dea-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="51dea-115">Not supported.</span></span>|
|<span data-ttu-id="51dea-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="51dea-116">Application</span></span>|<span data-ttu-id="51dea-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="51dea-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="51dea-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="51dea-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="51dea-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="51dea-119">Request headers</span></span>
|<span data-ttu-id="51dea-120">标头</span><span class="sxs-lookup"><span data-stu-id="51dea-120">Header</span></span>|<span data-ttu-id="51dea-121">值</span><span class="sxs-lookup"><span data-stu-id="51dea-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="51dea-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="51dea-122">Authorization</span></span>|<span data-ttu-id="51dea-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="51dea-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="51dea-124">接受</span><span class="sxs-lookup"><span data-stu-id="51dea-124">Accept</span></span>|<span data-ttu-id="51dea-125">application/json</span><span class="sxs-lookup"><span data-stu-id="51dea-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="51dea-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="51dea-126">Request body</span></span>
<span data-ttu-id="51dea-127">在请求正文中, 提供 windows81SCEPCertificateProfile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="51dea-127">In the request body, supply a JSON representation for the windows81SCEPCertificateProfile object.</span></span>

<span data-ttu-id="51dea-128">下表显示创建 windows81SCEPCertificateProfile 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="51dea-128">The following table shows the properties that are required when you create the windows81SCEPCertificateProfile.</span></span>

|<span data-ttu-id="51dea-129">属性</span><span class="sxs-lookup"><span data-stu-id="51dea-129">Property</span></span>|<span data-ttu-id="51dea-130">类型</span><span class="sxs-lookup"><span data-stu-id="51dea-130">Type</span></span>|<span data-ttu-id="51dea-131">说明</span><span class="sxs-lookup"><span data-stu-id="51dea-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51dea-132">id</span><span class="sxs-lookup"><span data-stu-id="51dea-132">id</span></span>|<span data-ttu-id="51dea-133">字符串</span><span class="sxs-lookup"><span data-stu-id="51dea-133">String</span></span>|<span data-ttu-id="51dea-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="51dea-134">Key of the entity.</span></span> <span data-ttu-id="51dea-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="51dea-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51dea-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="51dea-136">lastModifiedDateTime</span></span>|<span data-ttu-id="51dea-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51dea-137">DateTimeOffset</span></span>|<span data-ttu-id="51dea-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="51dea-138">DateTime the object was last modified.</span></span> <span data-ttu-id="51dea-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="51dea-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51dea-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="51dea-140">roleScopeTagIds</span></span>|<span data-ttu-id="51dea-141">String collection</span><span class="sxs-lookup"><span data-stu-id="51dea-141">String collection</span></span>|<span data-ttu-id="51dea-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="51dea-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="51dea-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="51dea-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51dea-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="51dea-144">supportsScopeTags</span></span>|<span data-ttu-id="51dea-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="51dea-145">Boolean</span></span>|<span data-ttu-id="51dea-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="51dea-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="51dea-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="51dea-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="51dea-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="51dea-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="51dea-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="51dea-149">This property is read-only.</span></span> <span data-ttu-id="51dea-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="51dea-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51dea-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="51dea-151">createdDateTime</span></span>|<span data-ttu-id="51dea-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51dea-152">DateTimeOffset</span></span>|<span data-ttu-id="51dea-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="51dea-153">DateTime the object was created.</span></span> <span data-ttu-id="51dea-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="51dea-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51dea-155">说明</span><span class="sxs-lookup"><span data-stu-id="51dea-155">description</span></span>|<span data-ttu-id="51dea-156">String</span><span class="sxs-lookup"><span data-stu-id="51dea-156">String</span></span>|<span data-ttu-id="51dea-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="51dea-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="51dea-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="51dea-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51dea-159">displayName</span><span class="sxs-lookup"><span data-stu-id="51dea-159">displayName</span></span>|<span data-ttu-id="51dea-160">String</span><span class="sxs-lookup"><span data-stu-id="51dea-160">String</span></span>|<span data-ttu-id="51dea-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="51dea-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="51dea-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="51dea-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51dea-163">version</span><span class="sxs-lookup"><span data-stu-id="51dea-163">version</span></span>|<span data-ttu-id="51dea-164">Int32</span><span class="sxs-lookup"><span data-stu-id="51dea-164">Int32</span></span>|<span data-ttu-id="51dea-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="51dea-165">Version of the device configuration.</span></span> <span data-ttu-id="51dea-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="51dea-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51dea-167">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="51dea-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="51dea-168">Int32</span><span class="sxs-lookup"><span data-stu-id="51dea-168">Int32</span></span>|<span data-ttu-id="51dea-169">证书续订阈值百分比。</span><span class="sxs-lookup"><span data-stu-id="51dea-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="51dea-170">从[WindowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)继承的有效值1到99</span><span class="sxs-lookup"><span data-stu-id="51dea-170">Valid values 1 to 99 Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="51dea-171">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="51dea-171">keyStorageProvider</span></span>|[<span data-ttu-id="51dea-172">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="51dea-172">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="51dea-173">从[WindowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)继承的密钥存储提供程序 (KSP)。</span><span class="sxs-lookup"><span data-stu-id="51dea-173">Key Storage Provider (KSP) Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="51dea-174">可取值为：`useTpmKspOtherwiseUseSoftwareKsp`、`useTpmKspOtherwiseFail`、`usePassportForWorkKspOtherwiseFail`、`useSoftwareKsp`。</span><span class="sxs-lookup"><span data-stu-id="51dea-174">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="51dea-175">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="51dea-175">subjectNameFormat</span></span>|[<span data-ttu-id="51dea-176">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="51dea-176">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="51dea-177">证书使用者名称格式继承自[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="51dea-177">Certificate Subject Name Format Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="51dea-178">可取值为：`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId`。</span><span class="sxs-lookup"><span data-stu-id="51dea-178">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="51dea-179">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="51dea-179">subjectAlternativeNameType</span></span>|[<span data-ttu-id="51dea-180">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="51dea-180">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="51dea-181">证书使用者备用名称类型继承自[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="51dea-181">Certificate Subject Alternative Name Type Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="51dea-182">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService`。</span><span class="sxs-lookup"><span data-stu-id="51dea-182">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="51dea-183">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="51dea-183">certificateValidityPeriodValue</span></span>|<span data-ttu-id="51dea-184">Int32</span><span class="sxs-lookup"><span data-stu-id="51dea-184">Int32</span></span>|<span data-ttu-id="51dea-185">继承自[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)的证书有效期限的值</span><span class="sxs-lookup"><span data-stu-id="51dea-185">Value for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="51dea-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="51dea-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="51dea-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="51dea-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="51dea-188">从[WindowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)继承的证书有效期限的小数位数。</span><span class="sxs-lookup"><span data-stu-id="51dea-188">Scale for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="51dea-189">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="51dea-189">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="51dea-190">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="51dea-190">extendedKeyUsages</span></span>|<span data-ttu-id="51dea-191">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)集合</span><span class="sxs-lookup"><span data-stu-id="51dea-191">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="51dea-192">扩展密钥用法 (EKU) 设置。</span><span class="sxs-lookup"><span data-stu-id="51dea-192">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="51dea-193">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="51dea-193">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="51dea-194">继承自[windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="51dea-194">Inherited from [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="51dea-195">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="51dea-195">customSubjectAlternativeNames</span></span>|<span data-ttu-id="51dea-196">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)集合</span><span class="sxs-lookup"><span data-stu-id="51dea-196">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="51dea-197">自定义主题备用名称设置。</span><span class="sxs-lookup"><span data-stu-id="51dea-197">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="51dea-198">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="51dea-198">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="51dea-199">继承自[windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="51dea-199">Inherited from [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="51dea-200">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="51dea-200">scepServerUrls</span></span>|<span data-ttu-id="51dea-201">String collection</span><span class="sxs-lookup"><span data-stu-id="51dea-201">String collection</span></span>|<span data-ttu-id="51dea-202">SCEP 服务器 Url。</span><span class="sxs-lookup"><span data-stu-id="51dea-202">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="51dea-203">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="51dea-203">subjectNameFormatString</span></span>|<span data-ttu-id="51dea-204">String</span><span class="sxs-lookup"><span data-stu-id="51dea-204">String</span></span>|<span data-ttu-id="51dea-205">要与 SubjectNameFormat = Custom 一起使用的自定义格式。</span><span class="sxs-lookup"><span data-stu-id="51dea-205">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="51dea-206">示例: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = 企业用户, O = Contoso Corporation, L = Redmond, ST = WA, C = US</span><span class="sxs-lookup"><span data-stu-id="51dea-206">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="51dea-207">keyUsage</span><span class="sxs-lookup"><span data-stu-id="51dea-207">keyUsage</span></span>|[<span data-ttu-id="51dea-208">keyUsages</span><span class="sxs-lookup"><span data-stu-id="51dea-208">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="51dea-209">SCEP 密钥用法。</span><span class="sxs-lookup"><span data-stu-id="51dea-209">SCEP Key Usage.</span></span> <span data-ttu-id="51dea-210">可取值为：`keyEncipherment`、`digitalSignature`。</span><span class="sxs-lookup"><span data-stu-id="51dea-210">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="51dea-211">keySize</span><span class="sxs-lookup"><span data-stu-id="51dea-211">keySize</span></span>|[<span data-ttu-id="51dea-212">keySize</span><span class="sxs-lookup"><span data-stu-id="51dea-212">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="51dea-213">SCEP 密钥大小。</span><span class="sxs-lookup"><span data-stu-id="51dea-213">SCEP Key Size.</span></span> <span data-ttu-id="51dea-214">可取值为：`size1024`、`size2048`。</span><span class="sxs-lookup"><span data-stu-id="51dea-214">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="51dea-215">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="51dea-215">hashAlgorithm</span></span>|[<span data-ttu-id="51dea-216">hashAlgorithms</span><span class="sxs-lookup"><span data-stu-id="51dea-216">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="51dea-217">SCEP 哈希算法。</span><span class="sxs-lookup"><span data-stu-id="51dea-217">SCEP Hash Algorithm.</span></span> <span data-ttu-id="51dea-218">可取值为：`sha1`、`sha2`。</span><span class="sxs-lookup"><span data-stu-id="51dea-218">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="51dea-219">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="51dea-219">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="51dea-220">String</span><span class="sxs-lookup"><span data-stu-id="51dea-220">String</span></span>|<span data-ttu-id="51dea-221">定义 AAD 属性的自定义字符串。</span><span class="sxs-lookup"><span data-stu-id="51dea-221">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="51dea-222">certificateStore</span><span class="sxs-lookup"><span data-stu-id="51dea-222">certificateStore</span></span>|[<span data-ttu-id="51dea-223">certificateStore</span><span class="sxs-lookup"><span data-stu-id="51dea-223">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="51dea-224">目标存储证书。</span><span class="sxs-lookup"><span data-stu-id="51dea-224">Target store certificate.</span></span> <span data-ttu-id="51dea-225">可取值为：`user`、`machine`。</span><span class="sxs-lookup"><span data-stu-id="51dea-225">Possible values are: `user`, `machine`.</span></span>|



## <a name="response"></a><span data-ttu-id="51dea-226">响应</span><span class="sxs-lookup"><span data-stu-id="51dea-226">Response</span></span>
<span data-ttu-id="51dea-227">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="51dea-227">If successful, this method returns a `201 Created` response code and a [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51dea-228">示例</span><span class="sxs-lookup"><span data-stu-id="51dea-228">Example</span></span>

### <a name="request"></a><span data-ttu-id="51dea-229">请求</span><span class="sxs-lookup"><span data-stu-id="51dea-229">Request</span></span>
<span data-ttu-id="51dea-230">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="51dea-230">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1251

{
  "@odata.type": "#microsoft.graph.windows81SCEPCertificateProfile",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "renewalThresholdPercentage": 10,
  "keyStorageProvider": "useTpmKspOtherwiseFail",
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
  "customSubjectAlternativeNames": [
    {
      "@odata.type": "microsoft.graph.customSubjectAlternativeName",
      "sanType": "emailAddress",
      "name": "Name value"
    }
  ],
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "certificateStore": "machine"
}
```

### <a name="response"></a><span data-ttu-id="51dea-231">响应</span><span class="sxs-lookup"><span data-stu-id="51dea-231">Response</span></span>
<span data-ttu-id="51dea-p122">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="51dea-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1423

{
  "@odata.type": "#microsoft.graph.windows81SCEPCertificateProfile",
  "id": "2daf8af2-8af2-2daf-f28a-af2df28aaf2d",
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
  "keyStorageProvider": "useTpmKspOtherwiseFail",
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
  "customSubjectAlternativeNames": [
    {
      "@odata.type": "microsoft.graph.customSubjectAlternativeName",
      "sanType": "emailAddress",
      "name": "Name value"
    }
  ],
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "certificateStore": "machine"
}
```




