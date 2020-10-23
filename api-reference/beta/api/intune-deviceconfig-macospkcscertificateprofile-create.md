---
title: 创建 macOSPkcsCertificateProfile
description: 创建新的 macOSPkcsCertificateProfile 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f3f821b1b201c6927ad3a84bd7e0b4b6631c03bf
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48731853"
---
# <a name="create-macospkcscertificateprofile"></a><span data-ttu-id="f4656-103">创建 macOSPkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="f4656-103">Create macOSPkcsCertificateProfile</span></span>

<span data-ttu-id="f4656-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4656-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f4656-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f4656-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f4656-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f4656-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4656-107">创建新的 [macOSPkcsCertificateProfile](../resources/intune-deviceconfig-macospkcscertificateprofile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f4656-107">Create a new [macOSPkcsCertificateProfile](../resources/intune-deviceconfig-macospkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f4656-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="f4656-108">Prerequisites</span></span>
<span data-ttu-id="f4656-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f4656-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4656-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f4656-111">Permission type</span></span>|<span data-ttu-id="f4656-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f4656-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f4656-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f4656-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f4656-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4656-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f4656-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f4656-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f4656-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f4656-116">Not supported.</span></span>|
|<span data-ttu-id="f4656-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f4656-117">Application</span></span>|<span data-ttu-id="f4656-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4656-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f4656-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f4656-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f4656-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f4656-120">Request headers</span></span>
|<span data-ttu-id="f4656-121">标头</span><span class="sxs-lookup"><span data-stu-id="f4656-121">Header</span></span>|<span data-ttu-id="f4656-122">值</span><span class="sxs-lookup"><span data-stu-id="f4656-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f4656-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f4656-123">Authorization</span></span>|<span data-ttu-id="f4656-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f4656-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f4656-125">接受</span><span class="sxs-lookup"><span data-stu-id="f4656-125">Accept</span></span>|<span data-ttu-id="f4656-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f4656-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4656-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f4656-127">Request body</span></span>
<span data-ttu-id="f4656-128">在请求正文中，提供 macOSPkcsCertificateProfile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f4656-128">In the request body, supply a JSON representation for the macOSPkcsCertificateProfile object.</span></span>

<span data-ttu-id="f4656-129">下表显示创建 macOSPkcsCertificateProfile 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f4656-129">The following table shows the properties that are required when you create the macOSPkcsCertificateProfile.</span></span>

|<span data-ttu-id="f4656-130">属性</span><span class="sxs-lookup"><span data-stu-id="f4656-130">Property</span></span>|<span data-ttu-id="f4656-131">类型</span><span class="sxs-lookup"><span data-stu-id="f4656-131">Type</span></span>|<span data-ttu-id="f4656-132">说明</span><span class="sxs-lookup"><span data-stu-id="f4656-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4656-133">id</span><span class="sxs-lookup"><span data-stu-id="f4656-133">id</span></span>|<span data-ttu-id="f4656-134">String</span><span class="sxs-lookup"><span data-stu-id="f4656-134">String</span></span>|<span data-ttu-id="f4656-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f4656-135">Key of the entity.</span></span> <span data-ttu-id="f4656-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4656-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4656-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f4656-137">lastModifiedDateTime</span></span>|<span data-ttu-id="f4656-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4656-138">DateTimeOffset</span></span>|<span data-ttu-id="f4656-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f4656-139">DateTime the object was last modified.</span></span> <span data-ttu-id="f4656-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4656-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4656-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f4656-141">roleScopeTagIds</span></span>|<span data-ttu-id="f4656-142">String collection</span><span class="sxs-lookup"><span data-stu-id="f4656-142">String collection</span></span>|<span data-ttu-id="f4656-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="f4656-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f4656-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4656-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4656-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f4656-145">supportsScopeTags</span></span>|<span data-ttu-id="f4656-146">布尔</span><span class="sxs-lookup"><span data-stu-id="f4656-146">Boolean</span></span>|<span data-ttu-id="f4656-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="f4656-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f4656-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="f4656-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f4656-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="f4656-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f4656-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="f4656-150">This property is read-only.</span></span> <span data-ttu-id="f4656-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4656-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4656-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f4656-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="f4656-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f4656-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="f4656-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="f4656-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="f4656-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4656-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4656-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f4656-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="f4656-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f4656-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="f4656-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="f4656-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="f4656-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4656-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4656-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f4656-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="f4656-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f4656-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="f4656-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="f4656-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="f4656-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4656-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4656-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f4656-164">createdDateTime</span></span>|<span data-ttu-id="f4656-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4656-165">DateTimeOffset</span></span>|<span data-ttu-id="f4656-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f4656-166">DateTime the object was created.</span></span> <span data-ttu-id="f4656-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4656-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4656-168">说明</span><span class="sxs-lookup"><span data-stu-id="f4656-168">description</span></span>|<span data-ttu-id="f4656-169">String</span><span class="sxs-lookup"><span data-stu-id="f4656-169">String</span></span>|<span data-ttu-id="f4656-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="f4656-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f4656-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4656-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4656-172">displayName</span><span class="sxs-lookup"><span data-stu-id="f4656-172">displayName</span></span>|<span data-ttu-id="f4656-173">String</span><span class="sxs-lookup"><span data-stu-id="f4656-173">String</span></span>|<span data-ttu-id="f4656-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="f4656-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f4656-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4656-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4656-176">version</span><span class="sxs-lookup"><span data-stu-id="f4656-176">version</span></span>|<span data-ttu-id="f4656-177">Int32</span><span class="sxs-lookup"><span data-stu-id="f4656-177">Int32</span></span>|<span data-ttu-id="f4656-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="f4656-178">Version of the device configuration.</span></span> <span data-ttu-id="f4656-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4656-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4656-180">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="f4656-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="f4656-181">Int32</span><span class="sxs-lookup"><span data-stu-id="f4656-181">Int32</span></span>|<span data-ttu-id="f4656-182">证书续订阈值百分比。</span><span class="sxs-lookup"><span data-stu-id="f4656-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="f4656-183">继承自 [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="f4656-183">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="f4656-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="f4656-184">subjectNameFormat</span></span>|[<span data-ttu-id="f4656-185">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="f4656-185">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="f4656-186">证书使用者名称格式。</span><span class="sxs-lookup"><span data-stu-id="f4656-186">Certificate Subject Name Format.</span></span> <span data-ttu-id="f4656-187">继承自 [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="f4656-187">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="f4656-188">可取值为：`commonName`、`commonNameAsEmail`、`custom`、`commonNameIncludingEmail`、`commonNameAsIMEI`、`commonNameAsSerialNumber`。</span><span class="sxs-lookup"><span data-stu-id="f4656-188">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="f4656-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="f4656-189">subjectAlternativeNameType</span></span>|[<span data-ttu-id="f4656-190">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="f4656-190">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="f4656-191">证书使用者备用名称类型。</span><span class="sxs-lookup"><span data-stu-id="f4656-191">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="f4656-192">继承自 [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="f4656-192">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="f4656-193">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService`、`universalResourceIdentifier`。</span><span class="sxs-lookup"><span data-stu-id="f4656-193">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span></span>|
|<span data-ttu-id="f4656-194">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="f4656-194">certificateValidityPeriodValue</span></span>|<span data-ttu-id="f4656-195">Int32</span><span class="sxs-lookup"><span data-stu-id="f4656-195">Int32</span></span>|<span data-ttu-id="f4656-196">证书有效期限的值。</span><span class="sxs-lookup"><span data-stu-id="f4656-196">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="f4656-197">继承自 [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="f4656-197">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="f4656-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="f4656-198">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="f4656-199">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="f4656-199">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="f4656-200">证书有效期的小数位数。</span><span class="sxs-lookup"><span data-stu-id="f4656-200">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="f4656-201">继承自 [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="f4656-201">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="f4656-202">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="f4656-202">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="f4656-203">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="f4656-203">certificationAuthority</span></span>|<span data-ttu-id="f4656-204">String</span><span class="sxs-lookup"><span data-stu-id="f4656-204">String</span></span>|<span data-ttu-id="f4656-205">PKCS 证书颁发机构 FQDN。</span><span class="sxs-lookup"><span data-stu-id="f4656-205">PKCS certification authority FQDN.</span></span>|
|<span data-ttu-id="f4656-206">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="f4656-206">certificationAuthorityName</span></span>|<span data-ttu-id="f4656-207">String</span><span class="sxs-lookup"><span data-stu-id="f4656-207">String</span></span>|<span data-ttu-id="f4656-208">PKCS 证书颁发机构名称。</span><span class="sxs-lookup"><span data-stu-id="f4656-208">PKCS certification authority Name.</span></span>|
|<span data-ttu-id="f4656-209">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="f4656-209">certificateTemplateName</span></span>|<span data-ttu-id="f4656-210">String</span><span class="sxs-lookup"><span data-stu-id="f4656-210">String</span></span>|<span data-ttu-id="f4656-211">PKCS 证书模板名称。</span><span class="sxs-lookup"><span data-stu-id="f4656-211">PKCS certificate template name.</span></span>|
|<span data-ttu-id="f4656-212">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="f4656-212">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="f4656-213">String</span><span class="sxs-lookup"><span data-stu-id="f4656-213">String</span></span>|<span data-ttu-id="f4656-214">定义使用者可选名称的格式字符串。</span><span class="sxs-lookup"><span data-stu-id="f4656-214">Format string that defines the subject alternative name.</span></span>|
|<span data-ttu-id="f4656-215">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="f4656-215">subjectNameFormatString</span></span>|<span data-ttu-id="f4656-216">String</span><span class="sxs-lookup"><span data-stu-id="f4656-216">String</span></span>|<span data-ttu-id="f4656-217">定义主题名称的格式字符串。</span><span class="sxs-lookup"><span data-stu-id="f4656-217">Format string that defines the subject name.</span></span> <span data-ttu-id="f4656-218">示例： CN = {{EmailAddress}}，E = {{EmailAddress}}，OU = 企业用户，O = Contoso Corporation，L = Redmond，ST = WA，C = US</span><span class="sxs-lookup"><span data-stu-id="f4656-218">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="f4656-219">certificateStore</span><span class="sxs-lookup"><span data-stu-id="f4656-219">certificateStore</span></span>|[<span data-ttu-id="f4656-220">certificateStore</span><span class="sxs-lookup"><span data-stu-id="f4656-220">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="f4656-221">目标存储证书。</span><span class="sxs-lookup"><span data-stu-id="f4656-221">Target store certificate.</span></span> <span data-ttu-id="f4656-222">可取值为：`user`、`machine`。</span><span class="sxs-lookup"><span data-stu-id="f4656-222">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="f4656-223">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="f4656-223">customSubjectAlternativeNames</span></span>|<span data-ttu-id="f4656-224">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f4656-224">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="f4656-225">自定义主题备用名称设置。</span><span class="sxs-lookup"><span data-stu-id="f4656-225">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="f4656-226">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="f4656-226">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="f4656-227">allowAllAppsAccess</span><span class="sxs-lookup"><span data-stu-id="f4656-227">allowAllAppsAccess</span></span>|<span data-ttu-id="f4656-228">布尔</span><span class="sxs-lookup"><span data-stu-id="f4656-228">Boolean</span></span>|<span data-ttu-id="f4656-229">AllowAllAppsAccess 设置</span><span class="sxs-lookup"><span data-stu-id="f4656-229">AllowAllAppsAccess setting</span></span>|



## <a name="response"></a><span data-ttu-id="f4656-230">响应</span><span class="sxs-lookup"><span data-stu-id="f4656-230">Response</span></span>
<span data-ttu-id="f4656-231">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [macOSPkcsCertificateProfile](../resources/intune-deviceconfig-macospkcscertificateprofile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f4656-231">If successful, this method returns a `201 Created` response code and a [macOSPkcsCertificateProfile](../resources/intune-deviceconfig-macospkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4656-232">示例</span><span class="sxs-lookup"><span data-stu-id="f4656-232">Example</span></span>

### <a name="request"></a><span data-ttu-id="f4656-233">请求</span><span class="sxs-lookup"><span data-stu-id="f4656-233">Request</span></span>
<span data-ttu-id="f4656-234">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f4656-234">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f4656-235">响应</span><span class="sxs-lookup"><span data-stu-id="f4656-235">Response</span></span>
<span data-ttu-id="f4656-p121">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f4656-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





