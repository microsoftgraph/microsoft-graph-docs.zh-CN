---
title: 创建 macOSPkcsCertificateProfile
description: 创建新的 macOSPkcsCertificateProfile 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d62ff86107ceeab4c6f1de284abc0c3178e2d24e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43432499"
---
# <a name="create-macospkcscertificateprofile"></a><span data-ttu-id="34ee8-103">创建 macOSPkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="34ee8-103">Create macOSPkcsCertificateProfile</span></span>

<span data-ttu-id="34ee8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="34ee8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="34ee8-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="34ee8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="34ee8-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="34ee8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34ee8-107">创建新的[macOSPkcsCertificateProfile](../resources/intune-deviceconfig-macospkcscertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="34ee8-107">Create a new [macOSPkcsCertificateProfile](../resources/intune-deviceconfig-macospkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="34ee8-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="34ee8-108">Prerequisites</span></span>
<span data-ttu-id="34ee8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="34ee8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34ee8-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="34ee8-111">Permission type</span></span>|<span data-ttu-id="34ee8-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="34ee8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="34ee8-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="34ee8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="34ee8-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34ee8-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="34ee8-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="34ee8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="34ee8-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="34ee8-116">Not supported.</span></span>|
|<span data-ttu-id="34ee8-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="34ee8-117">Application</span></span>|<span data-ttu-id="34ee8-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34ee8-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="34ee8-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="34ee8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="34ee8-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="34ee8-120">Request headers</span></span>
|<span data-ttu-id="34ee8-121">标头</span><span class="sxs-lookup"><span data-stu-id="34ee8-121">Header</span></span>|<span data-ttu-id="34ee8-122">值</span><span class="sxs-lookup"><span data-stu-id="34ee8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="34ee8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="34ee8-123">Authorization</span></span>|<span data-ttu-id="34ee8-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="34ee8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="34ee8-125">接受</span><span class="sxs-lookup"><span data-stu-id="34ee8-125">Accept</span></span>|<span data-ttu-id="34ee8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="34ee8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="34ee8-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="34ee8-127">Request body</span></span>
<span data-ttu-id="34ee8-128">在请求正文中，提供 macOSPkcsCertificateProfile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="34ee8-128">In the request body, supply a JSON representation for the macOSPkcsCertificateProfile object.</span></span>

<span data-ttu-id="34ee8-129">下表显示创建 macOSPkcsCertificateProfile 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="34ee8-129">The following table shows the properties that are required when you create the macOSPkcsCertificateProfile.</span></span>

|<span data-ttu-id="34ee8-130">属性</span><span class="sxs-lookup"><span data-stu-id="34ee8-130">Property</span></span>|<span data-ttu-id="34ee8-131">类型</span><span class="sxs-lookup"><span data-stu-id="34ee8-131">Type</span></span>|<span data-ttu-id="34ee8-132">说明</span><span class="sxs-lookup"><span data-stu-id="34ee8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34ee8-133">id</span><span class="sxs-lookup"><span data-stu-id="34ee8-133">id</span></span>|<span data-ttu-id="34ee8-134">字符串</span><span class="sxs-lookup"><span data-stu-id="34ee8-134">String</span></span>|<span data-ttu-id="34ee8-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="34ee8-135">Key of the entity.</span></span> <span data-ttu-id="34ee8-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="34ee8-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34ee8-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="34ee8-137">lastModifiedDateTime</span></span>|<span data-ttu-id="34ee8-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34ee8-138">DateTimeOffset</span></span>|<span data-ttu-id="34ee8-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="34ee8-139">DateTime the object was last modified.</span></span> <span data-ttu-id="34ee8-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="34ee8-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34ee8-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="34ee8-141">roleScopeTagIds</span></span>|<span data-ttu-id="34ee8-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="34ee8-142">String collection</span></span>|<span data-ttu-id="34ee8-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="34ee8-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="34ee8-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="34ee8-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34ee8-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="34ee8-145">supportsScopeTags</span></span>|<span data-ttu-id="34ee8-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="34ee8-146">Boolean</span></span>|<span data-ttu-id="34ee8-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="34ee8-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="34ee8-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="34ee8-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="34ee8-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="34ee8-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="34ee8-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="34ee8-150">This property is read-only.</span></span> <span data-ttu-id="34ee8-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="34ee8-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34ee8-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="34ee8-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="34ee8-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="34ee8-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="34ee8-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="34ee8-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="34ee8-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="34ee8-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34ee8-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="34ee8-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="34ee8-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="34ee8-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="34ee8-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="34ee8-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="34ee8-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="34ee8-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34ee8-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="34ee8-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="34ee8-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="34ee8-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="34ee8-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="34ee8-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="34ee8-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="34ee8-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34ee8-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="34ee8-164">createdDateTime</span></span>|<span data-ttu-id="34ee8-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34ee8-165">DateTimeOffset</span></span>|<span data-ttu-id="34ee8-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="34ee8-166">DateTime the object was created.</span></span> <span data-ttu-id="34ee8-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="34ee8-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34ee8-168">description</span><span class="sxs-lookup"><span data-stu-id="34ee8-168">description</span></span>|<span data-ttu-id="34ee8-169">String</span><span class="sxs-lookup"><span data-stu-id="34ee8-169">String</span></span>|<span data-ttu-id="34ee8-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="34ee8-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="34ee8-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="34ee8-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34ee8-172">displayName</span><span class="sxs-lookup"><span data-stu-id="34ee8-172">displayName</span></span>|<span data-ttu-id="34ee8-173">String</span><span class="sxs-lookup"><span data-stu-id="34ee8-173">String</span></span>|<span data-ttu-id="34ee8-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="34ee8-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="34ee8-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="34ee8-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34ee8-176">version</span><span class="sxs-lookup"><span data-stu-id="34ee8-176">version</span></span>|<span data-ttu-id="34ee8-177">Int32</span><span class="sxs-lookup"><span data-stu-id="34ee8-177">Int32</span></span>|<span data-ttu-id="34ee8-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="34ee8-178">Version of the device configuration.</span></span> <span data-ttu-id="34ee8-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="34ee8-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34ee8-180">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="34ee8-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="34ee8-181">Int32</span><span class="sxs-lookup"><span data-stu-id="34ee8-181">Int32</span></span>|<span data-ttu-id="34ee8-182">证书续订阈值百分比。</span><span class="sxs-lookup"><span data-stu-id="34ee8-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="34ee8-183">继承自[macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="34ee8-183">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="34ee8-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="34ee8-184">subjectNameFormat</span></span>|[<span data-ttu-id="34ee8-185">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="34ee8-185">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="34ee8-186">证书使用者名称格式。</span><span class="sxs-lookup"><span data-stu-id="34ee8-186">Certificate Subject Name Format.</span></span> <span data-ttu-id="34ee8-187">继承自[macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="34ee8-187">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="34ee8-188">可取值为：`commonName`、`commonNameAsEmail`、`custom`、`commonNameIncludingEmail`、`commonNameAsIMEI`、`commonNameAsSerialNumber`。</span><span class="sxs-lookup"><span data-stu-id="34ee8-188">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="34ee8-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="34ee8-189">subjectAlternativeNameType</span></span>|[<span data-ttu-id="34ee8-190">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="34ee8-190">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="34ee8-191">证书使用者备用名称类型。</span><span class="sxs-lookup"><span data-stu-id="34ee8-191">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="34ee8-192">继承自[macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="34ee8-192">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="34ee8-193">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService`。</span><span class="sxs-lookup"><span data-stu-id="34ee8-193">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="34ee8-194">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="34ee8-194">certificateValidityPeriodValue</span></span>|<span data-ttu-id="34ee8-195">Int32</span><span class="sxs-lookup"><span data-stu-id="34ee8-195">Int32</span></span>|<span data-ttu-id="34ee8-196">证书有效期限的值。</span><span class="sxs-lookup"><span data-stu-id="34ee8-196">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="34ee8-197">继承自[macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="34ee8-197">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="34ee8-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="34ee8-198">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="34ee8-199">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="34ee8-199">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="34ee8-200">证书有效期的小数位数。</span><span class="sxs-lookup"><span data-stu-id="34ee8-200">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="34ee8-201">继承自[macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="34ee8-201">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="34ee8-202">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="34ee8-202">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="34ee8-203">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="34ee8-203">certificationAuthority</span></span>|<span data-ttu-id="34ee8-204">String</span><span class="sxs-lookup"><span data-stu-id="34ee8-204">String</span></span>|<span data-ttu-id="34ee8-205">PKCS 证书颁发机构 FQDN。</span><span class="sxs-lookup"><span data-stu-id="34ee8-205">PKCS certification authority FQDN.</span></span>|
|<span data-ttu-id="34ee8-206">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="34ee8-206">certificationAuthorityName</span></span>|<span data-ttu-id="34ee8-207">String</span><span class="sxs-lookup"><span data-stu-id="34ee8-207">String</span></span>|<span data-ttu-id="34ee8-208">PKCS 证书颁发机构名称。</span><span class="sxs-lookup"><span data-stu-id="34ee8-208">PKCS certification authority Name.</span></span>|
|<span data-ttu-id="34ee8-209">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="34ee8-209">certificateTemplateName</span></span>|<span data-ttu-id="34ee8-210">String</span><span class="sxs-lookup"><span data-stu-id="34ee8-210">String</span></span>|<span data-ttu-id="34ee8-211">PKCS 证书模板名称。</span><span class="sxs-lookup"><span data-stu-id="34ee8-211">PKCS certificate template name.</span></span>|
|<span data-ttu-id="34ee8-212">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="34ee8-212">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="34ee8-213">String</span><span class="sxs-lookup"><span data-stu-id="34ee8-213">String</span></span>|<span data-ttu-id="34ee8-214">定义使用者可选名称的格式字符串。</span><span class="sxs-lookup"><span data-stu-id="34ee8-214">Format string that defines the subject alternative name.</span></span>|
|<span data-ttu-id="34ee8-215">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="34ee8-215">subjectNameFormatString</span></span>|<span data-ttu-id="34ee8-216">String</span><span class="sxs-lookup"><span data-stu-id="34ee8-216">String</span></span>|<span data-ttu-id="34ee8-217">定义主题名称的格式字符串。</span><span class="sxs-lookup"><span data-stu-id="34ee8-217">Format string that defines the subject name.</span></span> <span data-ttu-id="34ee8-218">示例： CN = {{EmailAddress}}，E = {{EmailAddress}}，OU = 企业用户，O = Contoso Corporation，L = Redmond，ST = WA，C = US</span><span class="sxs-lookup"><span data-stu-id="34ee8-218">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="34ee8-219">certificateStore</span><span class="sxs-lookup"><span data-stu-id="34ee8-219">certificateStore</span></span>|[<span data-ttu-id="34ee8-220">certificateStore</span><span class="sxs-lookup"><span data-stu-id="34ee8-220">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="34ee8-221">目标存储证书。</span><span class="sxs-lookup"><span data-stu-id="34ee8-221">Target store certificate.</span></span> <span data-ttu-id="34ee8-222">可取值为：`user`、`machine`。</span><span class="sxs-lookup"><span data-stu-id="34ee8-222">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="34ee8-223">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="34ee8-223">customSubjectAlternativeNames</span></span>|<span data-ttu-id="34ee8-224">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)集合</span><span class="sxs-lookup"><span data-stu-id="34ee8-224">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="34ee8-225">自定义主题备用名称设置。</span><span class="sxs-lookup"><span data-stu-id="34ee8-225">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="34ee8-226">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="34ee8-226">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="34ee8-227">allowAllAppsAccess</span><span class="sxs-lookup"><span data-stu-id="34ee8-227">allowAllAppsAccess</span></span>|<span data-ttu-id="34ee8-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="34ee8-228">Boolean</span></span>|<span data-ttu-id="34ee8-229">AllowAllAppsAccess 设置</span><span class="sxs-lookup"><span data-stu-id="34ee8-229">AllowAllAppsAccess setting</span></span>|



## <a name="response"></a><span data-ttu-id="34ee8-230">响应</span><span class="sxs-lookup"><span data-stu-id="34ee8-230">Response</span></span>
<span data-ttu-id="34ee8-231">如果成功，此方法在响应`201 Created`正文中返回响应代码和[macOSPkcsCertificateProfile](../resources/intune-deviceconfig-macospkcscertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="34ee8-231">If successful, this method returns a `201 Created` response code and a [macOSPkcsCertificateProfile](../resources/intune-deviceconfig-macospkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34ee8-232">示例</span><span class="sxs-lookup"><span data-stu-id="34ee8-232">Example</span></span>

### <a name="request"></a><span data-ttu-id="34ee8-233">请求</span><span class="sxs-lookup"><span data-stu-id="34ee8-233">Request</span></span>
<span data-ttu-id="34ee8-234">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="34ee8-234">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="34ee8-235">响应</span><span class="sxs-lookup"><span data-stu-id="34ee8-235">Response</span></span>
<span data-ttu-id="34ee8-p121">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="34ee8-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



