---
title: 创建 macOSPkcsCertificateProfile
description: 创建新的 macOSPkcsCertificateProfile 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c44b595ec20027fa26efcdac2b458781e5c189bf
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37533558"
---
# <a name="create-macospkcscertificateprofile"></a><span data-ttu-id="538fa-103">创建 macOSPkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="538fa-103">Create macOSPkcsCertificateProfile</span></span>

> <span data-ttu-id="538fa-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="538fa-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="538fa-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="538fa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="538fa-106">创建新的[macOSPkcsCertificateProfile](../resources/intune-deviceconfig-macospkcscertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="538fa-106">Create a new [macOSPkcsCertificateProfile](../resources/intune-deviceconfig-macospkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="538fa-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="538fa-107">Prerequisites</span></span>
<span data-ttu-id="538fa-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="538fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="538fa-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="538fa-110">Permission type</span></span>|<span data-ttu-id="538fa-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="538fa-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="538fa-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="538fa-112">Delegated (work or school account)</span></span>|<span data-ttu-id="538fa-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="538fa-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="538fa-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="538fa-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="538fa-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="538fa-115">Not supported.</span></span>|
|<span data-ttu-id="538fa-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="538fa-116">Application</span></span>|<span data-ttu-id="538fa-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="538fa-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="538fa-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="538fa-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="538fa-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="538fa-119">Request headers</span></span>
|<span data-ttu-id="538fa-120">标头</span><span class="sxs-lookup"><span data-stu-id="538fa-120">Header</span></span>|<span data-ttu-id="538fa-121">值</span><span class="sxs-lookup"><span data-stu-id="538fa-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="538fa-122">授权</span><span class="sxs-lookup"><span data-stu-id="538fa-122">Authorization</span></span>|<span data-ttu-id="538fa-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="538fa-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="538fa-124">接受</span><span class="sxs-lookup"><span data-stu-id="538fa-124">Accept</span></span>|<span data-ttu-id="538fa-125">application/json</span><span class="sxs-lookup"><span data-stu-id="538fa-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="538fa-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="538fa-126">Request body</span></span>
<span data-ttu-id="538fa-127">在请求正文中，提供 macOSPkcsCertificateProfile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="538fa-127">In the request body, supply a JSON representation for the macOSPkcsCertificateProfile object.</span></span>

<span data-ttu-id="538fa-128">下表显示创建 macOSPkcsCertificateProfile 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="538fa-128">The following table shows the properties that are required when you create the macOSPkcsCertificateProfile.</span></span>

|<span data-ttu-id="538fa-129">属性</span><span class="sxs-lookup"><span data-stu-id="538fa-129">Property</span></span>|<span data-ttu-id="538fa-130">类型</span><span class="sxs-lookup"><span data-stu-id="538fa-130">Type</span></span>|<span data-ttu-id="538fa-131">说明</span><span class="sxs-lookup"><span data-stu-id="538fa-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="538fa-132">id</span><span class="sxs-lookup"><span data-stu-id="538fa-132">id</span></span>|<span data-ttu-id="538fa-133">字符串</span><span class="sxs-lookup"><span data-stu-id="538fa-133">String</span></span>|<span data-ttu-id="538fa-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="538fa-134">Key of the entity.</span></span> <span data-ttu-id="538fa-135">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="538fa-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="538fa-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="538fa-136">lastModifiedDateTime</span></span>|<span data-ttu-id="538fa-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="538fa-137">DateTimeOffset</span></span>|<span data-ttu-id="538fa-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="538fa-138">DateTime the object was last modified.</span></span> <span data-ttu-id="538fa-139">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="538fa-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="538fa-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="538fa-140">roleScopeTagIds</span></span>|<span data-ttu-id="538fa-141">String 集合</span><span class="sxs-lookup"><span data-stu-id="538fa-141">String collection</span></span>|<span data-ttu-id="538fa-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="538fa-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="538fa-143">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="538fa-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="538fa-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="538fa-144">supportsScopeTags</span></span>|<span data-ttu-id="538fa-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="538fa-145">Boolean</span></span>|<span data-ttu-id="538fa-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="538fa-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="538fa-147">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="538fa-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="538fa-148">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="538fa-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="538fa-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="538fa-149">This property is read-only.</span></span> <span data-ttu-id="538fa-150">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="538fa-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="538fa-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="538fa-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="538fa-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="538fa-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="538fa-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="538fa-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="538fa-154">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="538fa-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="538fa-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="538fa-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="538fa-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="538fa-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="538fa-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="538fa-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="538fa-158">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="538fa-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="538fa-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="538fa-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="538fa-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="538fa-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="538fa-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="538fa-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="538fa-162">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="538fa-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="538fa-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="538fa-163">createdDateTime</span></span>|<span data-ttu-id="538fa-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="538fa-164">DateTimeOffset</span></span>|<span data-ttu-id="538fa-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="538fa-165">DateTime the object was created.</span></span> <span data-ttu-id="538fa-166">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="538fa-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="538fa-167">说明</span><span class="sxs-lookup"><span data-stu-id="538fa-167">description</span></span>|<span data-ttu-id="538fa-168">String</span><span class="sxs-lookup"><span data-stu-id="538fa-168">String</span></span>|<span data-ttu-id="538fa-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="538fa-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="538fa-170">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="538fa-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="538fa-171">displayName</span><span class="sxs-lookup"><span data-stu-id="538fa-171">displayName</span></span>|<span data-ttu-id="538fa-172">String</span><span class="sxs-lookup"><span data-stu-id="538fa-172">String</span></span>|<span data-ttu-id="538fa-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="538fa-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="538fa-174">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="538fa-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="538fa-175">version</span><span class="sxs-lookup"><span data-stu-id="538fa-175">version</span></span>|<span data-ttu-id="538fa-176">Int32</span><span class="sxs-lookup"><span data-stu-id="538fa-176">Int32</span></span>|<span data-ttu-id="538fa-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="538fa-177">Version of the device configuration.</span></span> <span data-ttu-id="538fa-178">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="538fa-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="538fa-179">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="538fa-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="538fa-180">Int32</span><span class="sxs-lookup"><span data-stu-id="538fa-180">Int32</span></span>|<span data-ttu-id="538fa-181">证书续订阈值百分比。</span><span class="sxs-lookup"><span data-stu-id="538fa-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="538fa-182">继承自[macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="538fa-182">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="538fa-183">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="538fa-183">subjectNameFormat</span></span>|[<span data-ttu-id="538fa-184">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="538fa-184">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="538fa-185">证书使用者名称格式。</span><span class="sxs-lookup"><span data-stu-id="538fa-185">Certificate Subject Name Format.</span></span> <span data-ttu-id="538fa-186">继承自[macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="538fa-186">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="538fa-187">可取值为：`commonName`、`commonNameAsEmail`、`custom`、`commonNameIncludingEmail`、`commonNameAsIMEI`、`commonNameAsSerialNumber`。</span><span class="sxs-lookup"><span data-stu-id="538fa-187">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="538fa-188">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="538fa-188">subjectAlternativeNameType</span></span>|[<span data-ttu-id="538fa-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="538fa-189">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="538fa-190">证书使用者备用名称类型。</span><span class="sxs-lookup"><span data-stu-id="538fa-190">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="538fa-191">继承自[macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="538fa-191">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="538fa-192">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService`。</span><span class="sxs-lookup"><span data-stu-id="538fa-192">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="538fa-193">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="538fa-193">certificateValidityPeriodValue</span></span>|<span data-ttu-id="538fa-194">Int32</span><span class="sxs-lookup"><span data-stu-id="538fa-194">Int32</span></span>|<span data-ttu-id="538fa-195">证书有效期限的值。</span><span class="sxs-lookup"><span data-stu-id="538fa-195">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="538fa-196">继承自[macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="538fa-196">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="538fa-197">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="538fa-197">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="538fa-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="538fa-198">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="538fa-199">证书有效期的小数位数。</span><span class="sxs-lookup"><span data-stu-id="538fa-199">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="538fa-200">继承自[macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="538fa-200">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="538fa-201">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="538fa-201">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="538fa-202">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="538fa-202">certificationAuthority</span></span>|<span data-ttu-id="538fa-203">字符串</span><span class="sxs-lookup"><span data-stu-id="538fa-203">String</span></span>|<span data-ttu-id="538fa-204">PKCS 证书颁发机构 FQDN。</span><span class="sxs-lookup"><span data-stu-id="538fa-204">PKCS certification authority FQDN.</span></span>|
|<span data-ttu-id="538fa-205">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="538fa-205">certificationAuthorityName</span></span>|<span data-ttu-id="538fa-206">字符串</span><span class="sxs-lookup"><span data-stu-id="538fa-206">String</span></span>|<span data-ttu-id="538fa-207">PKCS 证书颁发机构名称。</span><span class="sxs-lookup"><span data-stu-id="538fa-207">PKCS certification authority Name.</span></span>|
|<span data-ttu-id="538fa-208">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="538fa-208">certificateTemplateName</span></span>|<span data-ttu-id="538fa-209">字符串</span><span class="sxs-lookup"><span data-stu-id="538fa-209">String</span></span>|<span data-ttu-id="538fa-210">PKCS 证书模板名称。</span><span class="sxs-lookup"><span data-stu-id="538fa-210">PKCS certificate template name.</span></span>|
|<span data-ttu-id="538fa-211">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="538fa-211">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="538fa-212">字符串</span><span class="sxs-lookup"><span data-stu-id="538fa-212">String</span></span>|<span data-ttu-id="538fa-213">定义使用者可选名称的格式字符串。</span><span class="sxs-lookup"><span data-stu-id="538fa-213">Format string that defines the subject alternative name.</span></span>|
|<span data-ttu-id="538fa-214">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="538fa-214">subjectNameFormatString</span></span>|<span data-ttu-id="538fa-215">字符串</span><span class="sxs-lookup"><span data-stu-id="538fa-215">String</span></span>|<span data-ttu-id="538fa-216">定义主题名称的格式字符串。</span><span class="sxs-lookup"><span data-stu-id="538fa-216">Format string that defines the subject name.</span></span> <span data-ttu-id="538fa-217">示例： CN = {{EmailAddress}}，E = {{EmailAddress}}，OU = 企业用户，O = Contoso Corporation，L = Redmond，ST = WA，C = US</span><span class="sxs-lookup"><span data-stu-id="538fa-217">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="538fa-218">certificateStore</span><span class="sxs-lookup"><span data-stu-id="538fa-218">certificateStore</span></span>|[<span data-ttu-id="538fa-219">certificateStore</span><span class="sxs-lookup"><span data-stu-id="538fa-219">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="538fa-220">目标存储证书。</span><span class="sxs-lookup"><span data-stu-id="538fa-220">Target store certificate.</span></span> <span data-ttu-id="538fa-221">可取值为：`user`、`machine`。</span><span class="sxs-lookup"><span data-stu-id="538fa-221">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="538fa-222">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="538fa-222">customSubjectAlternativeNames</span></span>|<span data-ttu-id="538fa-223">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)集合</span><span class="sxs-lookup"><span data-stu-id="538fa-223">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="538fa-224">自定义主题备用名称设置。</span><span class="sxs-lookup"><span data-stu-id="538fa-224">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="538fa-225">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="538fa-225">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="538fa-226">allowAllAppsAccess</span><span class="sxs-lookup"><span data-stu-id="538fa-226">allowAllAppsAccess</span></span>|<span data-ttu-id="538fa-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="538fa-227">Boolean</span></span>|<span data-ttu-id="538fa-228">AllowAllAppsAccess 设置</span><span class="sxs-lookup"><span data-stu-id="538fa-228">AllowAllAppsAccess setting</span></span>|



## <a name="response"></a><span data-ttu-id="538fa-229">响应</span><span class="sxs-lookup"><span data-stu-id="538fa-229">Response</span></span>
<span data-ttu-id="538fa-230">如果成功，此方法在响应`201 Created`正文中返回响应代码和[macOSPkcsCertificateProfile](../resources/intune-deviceconfig-macospkcscertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="538fa-230">If successful, this method returns a `201 Created` response code and a [macOSPkcsCertificateProfile](../resources/intune-deviceconfig-macospkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="538fa-231">示例</span><span class="sxs-lookup"><span data-stu-id="538fa-231">Example</span></span>

### <a name="request"></a><span data-ttu-id="538fa-232">请求</span><span class="sxs-lookup"><span data-stu-id="538fa-232">Request</span></span>
<span data-ttu-id="538fa-233">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="538fa-233">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1857

{
  "@odata.type": "#microsoft.graph.macOSPkcsCertificateProfile",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
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
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "subjectNameFormatString": "Subject Name Format String value",
  "certificateStore": "machine",
  "customSubjectAlternativeNames": [
    {
      "@odata.type": "microsoft.graph.customSubjectAlternativeName",
      "sanType": "emailAddress",
      "name": "Name value"
    }
  ],
  "allowAllAppsAccess": true
}
```

### <a name="response"></a><span data-ttu-id="538fa-234">响应</span><span class="sxs-lookup"><span data-stu-id="538fa-234">Response</span></span>
<span data-ttu-id="538fa-p121">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="538fa-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2029

{
  "@odata.type": "#microsoft.graph.macOSPkcsCertificateProfile",
  "id": "4b489237-9237-4b48-3792-484b3792484b",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
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
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "subjectNameFormatString": "Subject Name Format String value",
  "certificateStore": "machine",
  "customSubjectAlternativeNames": [
    {
      "@odata.type": "microsoft.graph.customSubjectAlternativeName",
      "sanType": "emailAddress",
      "name": "Name value"
    }
  ],
  "allowAllAppsAccess": true
}
```






