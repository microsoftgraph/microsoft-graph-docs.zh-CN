---
title: 创建 windows81SCEPCertificateProfile
description: 创建新的 windows81SCEPCertificateProfile 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5a2def1fe83215e20b4fb2e0363237fe5af1f085
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30983272"
---
# <a name="create-windows81scepcertificateprofile"></a><span data-ttu-id="95f89-103">创建 windows81SCEPCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="95f89-103">Create windows81SCEPCertificateProfile</span></span>

> <span data-ttu-id="95f89-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="95f89-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="95f89-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="95f89-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95f89-106">创建新的[windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="95f89-106">Create a new [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="95f89-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="95f89-107">Prerequisites</span></span>
<span data-ttu-id="95f89-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="95f89-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95f89-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="95f89-110">Permission type</span></span>|<span data-ttu-id="95f89-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="95f89-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="95f89-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="95f89-112">Delegated (work or school account)</span></span>|<span data-ttu-id="95f89-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95f89-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="95f89-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="95f89-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="95f89-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="95f89-115">Not supported.</span></span>|
|<span data-ttu-id="95f89-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="95f89-116">Application</span></span>|<span data-ttu-id="95f89-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="95f89-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="95f89-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="95f89-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="95f89-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="95f89-119">Request headers</span></span>
|<span data-ttu-id="95f89-120">标头</span><span class="sxs-lookup"><span data-stu-id="95f89-120">Header</span></span>|<span data-ttu-id="95f89-121">值</span><span class="sxs-lookup"><span data-stu-id="95f89-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="95f89-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="95f89-122">Authorization</span></span>|<span data-ttu-id="95f89-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="95f89-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="95f89-124">接受</span><span class="sxs-lookup"><span data-stu-id="95f89-124">Accept</span></span>|<span data-ttu-id="95f89-125">application/json</span><span class="sxs-lookup"><span data-stu-id="95f89-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="95f89-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="95f89-126">Request body</span></span>
<span data-ttu-id="95f89-127">在请求正文中, 提供 windows81SCEPCertificateProfile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="95f89-127">In the request body, supply a JSON representation for the windows81SCEPCertificateProfile object.</span></span>

<span data-ttu-id="95f89-128">下表显示创建 windows81SCEPCertificateProfile 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="95f89-128">The following table shows the properties that are required when you create the windows81SCEPCertificateProfile.</span></span>

|<span data-ttu-id="95f89-129">属性</span><span class="sxs-lookup"><span data-stu-id="95f89-129">Property</span></span>|<span data-ttu-id="95f89-130">类型</span><span class="sxs-lookup"><span data-stu-id="95f89-130">Type</span></span>|<span data-ttu-id="95f89-131">说明</span><span class="sxs-lookup"><span data-stu-id="95f89-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95f89-132">id</span><span class="sxs-lookup"><span data-stu-id="95f89-132">id</span></span>|<span data-ttu-id="95f89-133">String</span><span class="sxs-lookup"><span data-stu-id="95f89-133">String</span></span>|<span data-ttu-id="95f89-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="95f89-134">Key of the entity.</span></span> <span data-ttu-id="95f89-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95f89-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95f89-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="95f89-136">lastModifiedDateTime</span></span>|<span data-ttu-id="95f89-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95f89-137">DateTimeOffset</span></span>|<span data-ttu-id="95f89-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="95f89-138">DateTime the object was last modified.</span></span> <span data-ttu-id="95f89-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95f89-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95f89-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="95f89-140">roleScopeTagIds</span></span>|<span data-ttu-id="95f89-141">String 集合</span><span class="sxs-lookup"><span data-stu-id="95f89-141">String collection</span></span>|<span data-ttu-id="95f89-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="95f89-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="95f89-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95f89-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95f89-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="95f89-144">supportsScopeTags</span></span>|<span data-ttu-id="95f89-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="95f89-145">Boolean</span></span>|<span data-ttu-id="95f89-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="95f89-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="95f89-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="95f89-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="95f89-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="95f89-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="95f89-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="95f89-149">This property is read-only.</span></span> <span data-ttu-id="95f89-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95f89-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95f89-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="95f89-151">createdDateTime</span></span>|<span data-ttu-id="95f89-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95f89-152">DateTimeOffset</span></span>|<span data-ttu-id="95f89-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="95f89-153">DateTime the object was created.</span></span> <span data-ttu-id="95f89-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95f89-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95f89-155">description</span><span class="sxs-lookup"><span data-stu-id="95f89-155">description</span></span>|<span data-ttu-id="95f89-156">String</span><span class="sxs-lookup"><span data-stu-id="95f89-156">String</span></span>|<span data-ttu-id="95f89-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="95f89-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="95f89-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95f89-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95f89-159">displayName</span><span class="sxs-lookup"><span data-stu-id="95f89-159">displayName</span></span>|<span data-ttu-id="95f89-160">String</span><span class="sxs-lookup"><span data-stu-id="95f89-160">String</span></span>|<span data-ttu-id="95f89-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="95f89-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="95f89-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95f89-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95f89-163">version</span><span class="sxs-lookup"><span data-stu-id="95f89-163">version</span></span>|<span data-ttu-id="95f89-164">Int32</span><span class="sxs-lookup"><span data-stu-id="95f89-164">Int32</span></span>|<span data-ttu-id="95f89-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="95f89-165">Version of the device configuration.</span></span> <span data-ttu-id="95f89-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95f89-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95f89-167">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="95f89-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="95f89-168">Int32</span><span class="sxs-lookup"><span data-stu-id="95f89-168">Int32</span></span>|<span data-ttu-id="95f89-169">证书续订阈值百分比。</span><span class="sxs-lookup"><span data-stu-id="95f89-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="95f89-170">从[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)继承的有效值1到99</span><span class="sxs-lookup"><span data-stu-id="95f89-170">Valid values 1 to 99 Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="95f89-171">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="95f89-171">keyStorageProvider</span></span>|[<span data-ttu-id="95f89-172">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="95f89-172">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="95f89-173">从[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)继承的密钥存储提供程序 (KSP)。</span><span class="sxs-lookup"><span data-stu-id="95f89-173">Key Storage Provider (KSP) Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="95f89-174">可取值为：`useTpmKspOtherwiseUseSoftwareKsp`、`useTpmKspOtherwiseFail`、`usePassportForWorkKspOtherwiseFail`、`useSoftwareKsp`。</span><span class="sxs-lookup"><span data-stu-id="95f89-174">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="95f89-175">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="95f89-175">subjectNameFormat</span></span>|[<span data-ttu-id="95f89-176">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="95f89-176">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="95f89-177">证书使用者名称格式继承自[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="95f89-177">Certificate Subject Name Format Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="95f89-178">可取值为：`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId`。</span><span class="sxs-lookup"><span data-stu-id="95f89-178">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="95f89-179">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="95f89-179">subjectAlternativeNameType</span></span>|[<span data-ttu-id="95f89-180">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="95f89-180">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="95f89-181">证书使用者备用名称类型继承自[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="95f89-181">Certificate Subject Alternative Name Type Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="95f89-182">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute` 或 `domainNameService`。</span><span class="sxs-lookup"><span data-stu-id="95f89-182">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="95f89-183">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="95f89-183">certificateValidityPeriodValue</span></span>|<span data-ttu-id="95f89-184">Int32</span><span class="sxs-lookup"><span data-stu-id="95f89-184">Int32</span></span>|<span data-ttu-id="95f89-185">继承自[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)的证书有效期限的值</span><span class="sxs-lookup"><span data-stu-id="95f89-185">Value for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="95f89-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="95f89-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="95f89-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="95f89-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="95f89-188">从[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)继承的证书有效期限的小数位数。</span><span class="sxs-lookup"><span data-stu-id="95f89-188">Scale for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="95f89-189">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="95f89-189">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="95f89-190">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="95f89-190">extendedKeyUsages</span></span>|<span data-ttu-id="95f89-191">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)集合</span><span class="sxs-lookup"><span data-stu-id="95f89-191">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="95f89-192">扩展密钥用法 (EKU) 设置。</span><span class="sxs-lookup"><span data-stu-id="95f89-192">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="95f89-193">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="95f89-193">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="95f89-194">继承自[windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="95f89-194">Inherited from [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="95f89-195">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="95f89-195">customSubjectAlternativeNames</span></span>|<span data-ttu-id="95f89-196">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)集合</span><span class="sxs-lookup"><span data-stu-id="95f89-196">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="95f89-197">自定义主题 Alterantive 名称设置。</span><span class="sxs-lookup"><span data-stu-id="95f89-197">Custom Subject Alterantive Name Settings.</span></span> <span data-ttu-id="95f89-198">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="95f89-198">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="95f89-199">继承自[windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="95f89-199">Inherited from [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="95f89-200">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="95f89-200">scepServerUrls</span></span>|<span data-ttu-id="95f89-201">String 集合</span><span class="sxs-lookup"><span data-stu-id="95f89-201">String collection</span></span>|<span data-ttu-id="95f89-202">SCEP 服务器 Url。</span><span class="sxs-lookup"><span data-stu-id="95f89-202">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="95f89-203">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="95f89-203">subjectNameFormatString</span></span>|<span data-ttu-id="95f89-204">String</span><span class="sxs-lookup"><span data-stu-id="95f89-204">String</span></span>|<span data-ttu-id="95f89-205">要与 SubjectNameFormat = custom 一起使用的自定义格式。</span><span class="sxs-lookup"><span data-stu-id="95f89-205">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="95f89-206">示例: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = 企业用户, O = Contoso Corporation, L = Redmond, ST = WA, C = US</span><span class="sxs-lookup"><span data-stu-id="95f89-206">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="95f89-207">keyUsage</span><span class="sxs-lookup"><span data-stu-id="95f89-207">keyUsage</span></span>|[<span data-ttu-id="95f89-208">keyUsages</span><span class="sxs-lookup"><span data-stu-id="95f89-208">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="95f89-209">SCEP 密钥用法。</span><span class="sxs-lookup"><span data-stu-id="95f89-209">SCEP Key Usage.</span></span> <span data-ttu-id="95f89-210">可取值为：`keyEncipherment`、`digitalSignature`。</span><span class="sxs-lookup"><span data-stu-id="95f89-210">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="95f89-211">keySize</span><span class="sxs-lookup"><span data-stu-id="95f89-211">keySize</span></span>|[<span data-ttu-id="95f89-212">keySize</span><span class="sxs-lookup"><span data-stu-id="95f89-212">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="95f89-213">SCEP 密钥大小。</span><span class="sxs-lookup"><span data-stu-id="95f89-213">SCEP Key Size.</span></span> <span data-ttu-id="95f89-214">可取值为：`size1024`、`size2048`。</span><span class="sxs-lookup"><span data-stu-id="95f89-214">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="95f89-215">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="95f89-215">hashAlgorithm</span></span>|[<span data-ttu-id="95f89-216">hashAlgorithms</span><span class="sxs-lookup"><span data-stu-id="95f89-216">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="95f89-217">SCEP 哈希算法。</span><span class="sxs-lookup"><span data-stu-id="95f89-217">SCEP Hash Algorithm.</span></span> <span data-ttu-id="95f89-218">可取值为：`sha1`、`sha2`。</span><span class="sxs-lookup"><span data-stu-id="95f89-218">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="95f89-219">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="95f89-219">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="95f89-220">String</span><span class="sxs-lookup"><span data-stu-id="95f89-220">String</span></span>|<span data-ttu-id="95f89-221">定义 AAD 属性的自定义字符串。</span><span class="sxs-lookup"><span data-stu-id="95f89-221">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="95f89-222">certificateStore</span><span class="sxs-lookup"><span data-stu-id="95f89-222">certificateStore</span></span>|[<span data-ttu-id="95f89-223">certificateStore</span><span class="sxs-lookup"><span data-stu-id="95f89-223">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="95f89-224">目标存储证书。</span><span class="sxs-lookup"><span data-stu-id="95f89-224">Target store certificate.</span></span> <span data-ttu-id="95f89-225">可取值为：`user`、`machine`。</span><span class="sxs-lookup"><span data-stu-id="95f89-225">Possible values are: `user`, `machine`.</span></span>|



## <a name="response"></a><span data-ttu-id="95f89-226">响应</span><span class="sxs-lookup"><span data-stu-id="95f89-226">Response</span></span>
<span data-ttu-id="95f89-227">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="95f89-227">If successful, this method returns a `201 Created` response code and a [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95f89-228">示例</span><span class="sxs-lookup"><span data-stu-id="95f89-228">Example</span></span>

### <a name="request"></a><span data-ttu-id="95f89-229">请求</span><span class="sxs-lookup"><span data-stu-id="95f89-229">Request</span></span>
<span data-ttu-id="95f89-230">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="95f89-230">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="95f89-231">响应</span><span class="sxs-lookup"><span data-stu-id="95f89-231">Response</span></span>
<span data-ttu-id="95f89-p122">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="95f89-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




