---
title: 创建 windows81SCEPCertificateProfile
description: 创建新的 windows81SCEPCertificateProfile 对象。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d28a0930493423885149fc27ad600783c8f2485b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422185"
---
# <a name="create-windows81scepcertificateprofile"></a><span data-ttu-id="66699-103">创建 windows81SCEPCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="66699-103">Create windows81SCEPCertificateProfile</span></span>

> <span data-ttu-id="66699-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="66699-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="66699-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="66699-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="66699-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="66699-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="66699-107">创建新的[windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="66699-107">Create a new [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="66699-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="66699-108">Prerequisites</span></span>
<span data-ttu-id="66699-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="66699-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="66699-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="66699-111">Permission type</span></span>|<span data-ttu-id="66699-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="66699-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="66699-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="66699-113">Delegated (work or school account)</span></span>|<span data-ttu-id="66699-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66699-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="66699-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="66699-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="66699-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="66699-116">Not supported.</span></span>|
|<span data-ttu-id="66699-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="66699-117">Application</span></span>|<span data-ttu-id="66699-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="66699-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="66699-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="66699-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="66699-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="66699-120">Request headers</span></span>
|<span data-ttu-id="66699-121">标头</span><span class="sxs-lookup"><span data-stu-id="66699-121">Header</span></span>|<span data-ttu-id="66699-122">值</span><span class="sxs-lookup"><span data-stu-id="66699-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="66699-123">授权</span><span class="sxs-lookup"><span data-stu-id="66699-123">Authorization</span></span>|<span data-ttu-id="66699-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="66699-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="66699-125">Accept</span><span class="sxs-lookup"><span data-stu-id="66699-125">Accept</span></span>|<span data-ttu-id="66699-126">application/json</span><span class="sxs-lookup"><span data-stu-id="66699-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="66699-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="66699-127">Request body</span></span>
<span data-ttu-id="66699-128">在请求正文中，提供 windows81SCEPCertificateProfile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="66699-128">In the request body, supply a JSON representation for the windows81SCEPCertificateProfile object.</span></span>

<span data-ttu-id="66699-129">下表显示时创建 windows81SCEPCertificateProfile 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="66699-129">The following table shows the properties that are required when you create the windows81SCEPCertificateProfile.</span></span>

|<span data-ttu-id="66699-130">属性</span><span class="sxs-lookup"><span data-stu-id="66699-130">Property</span></span>|<span data-ttu-id="66699-131">类型</span><span class="sxs-lookup"><span data-stu-id="66699-131">Type</span></span>|<span data-ttu-id="66699-132">说明</span><span class="sxs-lookup"><span data-stu-id="66699-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66699-133">id</span><span class="sxs-lookup"><span data-stu-id="66699-133">id</span></span>|<span data-ttu-id="66699-134">String</span><span class="sxs-lookup"><span data-stu-id="66699-134">String</span></span>|<span data-ttu-id="66699-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="66699-135">Key of the entity.</span></span> <span data-ttu-id="66699-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="66699-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="66699-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="66699-137">lastModifiedDateTime</span></span>|<span data-ttu-id="66699-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66699-138">DateTimeOffset</span></span>|<span data-ttu-id="66699-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="66699-139">DateTime the object was last modified.</span></span> <span data-ttu-id="66699-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="66699-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="66699-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="66699-141">roleScopeTagIds</span></span>|<span data-ttu-id="66699-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="66699-142">String collection</span></span>|<span data-ttu-id="66699-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="66699-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="66699-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="66699-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="66699-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="66699-145">supportsScopeTags</span></span>|<span data-ttu-id="66699-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="66699-146">Boolean</span></span>|<span data-ttu-id="66699-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="66699-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="66699-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="66699-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="66699-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="66699-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="66699-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="66699-150">This property is read-only.</span></span> <span data-ttu-id="66699-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="66699-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="66699-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="66699-152">createdDateTime</span></span>|<span data-ttu-id="66699-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66699-153">DateTimeOffset</span></span>|<span data-ttu-id="66699-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="66699-154">DateTime the object was created.</span></span> <span data-ttu-id="66699-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="66699-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="66699-156">description</span><span class="sxs-lookup"><span data-stu-id="66699-156">description</span></span>|<span data-ttu-id="66699-157">String</span><span class="sxs-lookup"><span data-stu-id="66699-157">String</span></span>|<span data-ttu-id="66699-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="66699-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="66699-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="66699-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="66699-160">displayName</span><span class="sxs-lookup"><span data-stu-id="66699-160">displayName</span></span>|<span data-ttu-id="66699-161">String</span><span class="sxs-lookup"><span data-stu-id="66699-161">String</span></span>|<span data-ttu-id="66699-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="66699-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="66699-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="66699-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="66699-164">version</span><span class="sxs-lookup"><span data-stu-id="66699-164">version</span></span>|<span data-ttu-id="66699-165">Int32</span><span class="sxs-lookup"><span data-stu-id="66699-165">Int32</span></span>|<span data-ttu-id="66699-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="66699-166">Version of the device configuration.</span></span> <span data-ttu-id="66699-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="66699-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="66699-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="66699-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="66699-169">Int32</span><span class="sxs-lookup"><span data-stu-id="66699-169">Int32</span></span>|<span data-ttu-id="66699-170">证书续订阈值百分比。</span><span class="sxs-lookup"><span data-stu-id="66699-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="66699-171">有效值 1 到 99 继承自[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="66699-171">Valid values 1 to 99 Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="66699-172">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="66699-172">keyStorageProvider</span></span>|[<span data-ttu-id="66699-173">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="66699-173">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="66699-174">从[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)键存储提供程序 (KSP) 继承。</span><span class="sxs-lookup"><span data-stu-id="66699-174">Key Storage Provider (KSP) Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="66699-175">可取值为：`useTpmKspOtherwiseUseSoftwareKsp`、`useTpmKspOtherwiseFail`、`usePassportForWorkKspOtherwiseFail`、`useSoftwareKsp`。</span><span class="sxs-lookup"><span data-stu-id="66699-175">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="66699-176">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="66699-176">subjectNameFormat</span></span>|[<span data-ttu-id="66699-177">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="66699-177">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="66699-178">证书使用者名称格式继承自[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="66699-178">Certificate Subject Name Format Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="66699-179">可取值为：`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId`。</span><span class="sxs-lookup"><span data-stu-id="66699-179">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="66699-180">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="66699-180">subjectAlternativeNameType</span></span>|[<span data-ttu-id="66699-181">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="66699-181">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="66699-182">证书使用者替代名称类型继承自[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="66699-182">Certificate Subject Alternative Name Type Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="66699-183">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService`。</span><span class="sxs-lookup"><span data-stu-id="66699-183">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="66699-184">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="66699-184">certificateValidityPeriodValue</span></span>|<span data-ttu-id="66699-185">Int32</span><span class="sxs-lookup"><span data-stu-id="66699-185">Int32</span></span>|<span data-ttu-id="66699-186">证书有效性段继承自[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)值</span><span class="sxs-lookup"><span data-stu-id="66699-186">Value for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="66699-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="66699-187">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="66699-188">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="66699-188">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="66699-189">证书有效性段继承自[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)的小数位数。</span><span class="sxs-lookup"><span data-stu-id="66699-189">Scale for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="66699-190">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="66699-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="66699-191">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="66699-191">extendedKeyUsages</span></span>|<span data-ttu-id="66699-192">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)集合</span><span class="sxs-lookup"><span data-stu-id="66699-192">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="66699-193">扩展的密钥用法 (EKU) 设置。</span><span class="sxs-lookup"><span data-stu-id="66699-193">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="66699-194">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="66699-194">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="66699-195">继承自[windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="66699-195">Inherited from [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="66699-196">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="66699-196">customSubjectAlternativeNames</span></span>|<span data-ttu-id="66699-197">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)集合</span><span class="sxs-lookup"><span data-stu-id="66699-197">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="66699-198">自定义主题 Alterantive 名称设置。</span><span class="sxs-lookup"><span data-stu-id="66699-198">Custom Subject Alterantive Name Settings.</span></span> <span data-ttu-id="66699-199">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="66699-199">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="66699-200">继承自[windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="66699-200">Inherited from [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="66699-201">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="66699-201">scepServerUrls</span></span>|<span data-ttu-id="66699-202">String 集合</span><span class="sxs-lookup"><span data-stu-id="66699-202">String collection</span></span>|<span data-ttu-id="66699-203">SCEP 服务器 Url(s)。</span><span class="sxs-lookup"><span data-stu-id="66699-203">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="66699-204">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="66699-204">subjectNameFormatString</span></span>|<span data-ttu-id="66699-205">String</span><span class="sxs-lookup"><span data-stu-id="66699-205">String</span></span>|<span data-ttu-id="66699-206">自定义格式使用 SubjectNameFormat = 自定义。</span><span class="sxs-lookup"><span data-stu-id="66699-206">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="66699-207">示例： CN = {{EmailAddress}} E = {{EmailAddress}}，OU = 企业用户，O = Contoso Corporation L = 雷德蒙德，ST = WA，C = US</span><span class="sxs-lookup"><span data-stu-id="66699-207">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="66699-208">keyUsage</span><span class="sxs-lookup"><span data-stu-id="66699-208">keyUsage</span></span>|[<span data-ttu-id="66699-209">keyUsages</span><span class="sxs-lookup"><span data-stu-id="66699-209">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="66699-210">SCEP 密钥用法。</span><span class="sxs-lookup"><span data-stu-id="66699-210">SCEP Key Usage.</span></span> <span data-ttu-id="66699-211">可取值为：`keyEncipherment`、`digitalSignature`。</span><span class="sxs-lookup"><span data-stu-id="66699-211">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="66699-212">keySize</span><span class="sxs-lookup"><span data-stu-id="66699-212">keySize</span></span>|[<span data-ttu-id="66699-213">keySize</span><span class="sxs-lookup"><span data-stu-id="66699-213">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="66699-214">SCEP 密钥大小。</span><span class="sxs-lookup"><span data-stu-id="66699-214">SCEP Key Size.</span></span> <span data-ttu-id="66699-215">可取值为：`size1024`、`size2048`。</span><span class="sxs-lookup"><span data-stu-id="66699-215">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="66699-216">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="66699-216">hashAlgorithm</span></span>|[<span data-ttu-id="66699-217">hashAlgorithms</span><span class="sxs-lookup"><span data-stu-id="66699-217">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="66699-218">SCEP 哈希算法。</span><span class="sxs-lookup"><span data-stu-id="66699-218">SCEP Hash Algorithm.</span></span> <span data-ttu-id="66699-219">可取值为：`sha1`、`sha2`。</span><span class="sxs-lookup"><span data-stu-id="66699-219">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="66699-220">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="66699-220">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="66699-221">String</span><span class="sxs-lookup"><span data-stu-id="66699-221">String</span></span>|<span data-ttu-id="66699-222">定义 AAD 属性的自定义字符串。</span><span class="sxs-lookup"><span data-stu-id="66699-222">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="66699-223">certificateStore</span><span class="sxs-lookup"><span data-stu-id="66699-223">certificateStore</span></span>|[<span data-ttu-id="66699-224">certificateStore</span><span class="sxs-lookup"><span data-stu-id="66699-224">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="66699-225">目标存储证书。</span><span class="sxs-lookup"><span data-stu-id="66699-225">Target store certificate.</span></span> <span data-ttu-id="66699-226">可取值为：`user`、`machine`。</span><span class="sxs-lookup"><span data-stu-id="66699-226">Possible values are: `user`, `machine`.</span></span>|



## <a name="response"></a><span data-ttu-id="66699-227">响应</span><span class="sxs-lookup"><span data-stu-id="66699-227">Response</span></span>
<span data-ttu-id="66699-228">如果成功，此方法返回`201 Created`响应代码和响应正文中的[windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="66699-228">If successful, this method returns a `201 Created` response code and a [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="66699-229">示例</span><span class="sxs-lookup"><span data-stu-id="66699-229">Example</span></span>

### <a name="request"></a><span data-ttu-id="66699-230">请求</span><span class="sxs-lookup"><span data-stu-id="66699-230">Request</span></span>
<span data-ttu-id="66699-231">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="66699-231">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="66699-232">响应</span><span class="sxs-lookup"><span data-stu-id="66699-232">Response</span></span>
<span data-ttu-id="66699-p123">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="66699-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




