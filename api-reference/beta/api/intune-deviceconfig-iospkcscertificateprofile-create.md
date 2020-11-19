---
title: 创建 iosPkcsCertificateProfile
description: 创建新的 iosPkcsCertificateProfile 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3a55acb790e4d5b13d2ffb23724d0a955421e7be
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49220453"
---
# <a name="create-iospkcscertificateprofile"></a><span data-ttu-id="150cf-103">创建 iosPkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="150cf-103">Create iosPkcsCertificateProfile</span></span>

<span data-ttu-id="150cf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="150cf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="150cf-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="150cf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="150cf-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="150cf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="150cf-107">创建新的 [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="150cf-107">Create a new [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="150cf-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="150cf-108">Prerequisites</span></span>
<span data-ttu-id="150cf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="150cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="150cf-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="150cf-111">Permission type</span></span>|<span data-ttu-id="150cf-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="150cf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="150cf-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="150cf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="150cf-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="150cf-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="150cf-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="150cf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="150cf-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="150cf-116">Not supported.</span></span>|
|<span data-ttu-id="150cf-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="150cf-117">Application</span></span>|<span data-ttu-id="150cf-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="150cf-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="150cf-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="150cf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="150cf-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="150cf-120">Request headers</span></span>
|<span data-ttu-id="150cf-121">标头</span><span class="sxs-lookup"><span data-stu-id="150cf-121">Header</span></span>|<span data-ttu-id="150cf-122">值</span><span class="sxs-lookup"><span data-stu-id="150cf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="150cf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="150cf-123">Authorization</span></span>|<span data-ttu-id="150cf-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="150cf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="150cf-125">接受</span><span class="sxs-lookup"><span data-stu-id="150cf-125">Accept</span></span>|<span data-ttu-id="150cf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="150cf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="150cf-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="150cf-127">Request body</span></span>
<span data-ttu-id="150cf-128">在请求正文中，提供 iosPkcsCertificateProfile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="150cf-128">In the request body, supply a JSON representation for the iosPkcsCertificateProfile object.</span></span>

<span data-ttu-id="150cf-129">下表显示创建 iosPkcsCertificateProfile 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="150cf-129">The following table shows the properties that are required when you create the iosPkcsCertificateProfile.</span></span>

|<span data-ttu-id="150cf-130">属性</span><span class="sxs-lookup"><span data-stu-id="150cf-130">Property</span></span>|<span data-ttu-id="150cf-131">类型</span><span class="sxs-lookup"><span data-stu-id="150cf-131">Type</span></span>|<span data-ttu-id="150cf-132">说明</span><span class="sxs-lookup"><span data-stu-id="150cf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="150cf-133">id</span><span class="sxs-lookup"><span data-stu-id="150cf-133">id</span></span>|<span data-ttu-id="150cf-134">String</span><span class="sxs-lookup"><span data-stu-id="150cf-134">String</span></span>|<span data-ttu-id="150cf-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="150cf-135">Key of the entity.</span></span> <span data-ttu-id="150cf-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="150cf-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="150cf-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="150cf-137">lastModifiedDateTime</span></span>|<span data-ttu-id="150cf-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="150cf-138">DateTimeOffset</span></span>|<span data-ttu-id="150cf-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="150cf-139">DateTime the object was last modified.</span></span> <span data-ttu-id="150cf-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="150cf-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="150cf-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="150cf-141">roleScopeTagIds</span></span>|<span data-ttu-id="150cf-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="150cf-142">String collection</span></span>|<span data-ttu-id="150cf-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="150cf-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="150cf-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="150cf-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="150cf-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="150cf-145">supportsScopeTags</span></span>|<span data-ttu-id="150cf-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="150cf-146">Boolean</span></span>|<span data-ttu-id="150cf-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="150cf-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="150cf-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="150cf-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="150cf-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="150cf-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="150cf-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="150cf-150">This property is read-only.</span></span> <span data-ttu-id="150cf-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="150cf-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="150cf-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="150cf-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="150cf-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="150cf-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="150cf-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="150cf-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="150cf-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="150cf-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="150cf-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="150cf-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="150cf-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="150cf-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="150cf-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="150cf-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="150cf-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="150cf-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="150cf-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="150cf-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="150cf-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="150cf-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="150cf-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="150cf-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="150cf-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="150cf-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="150cf-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="150cf-164">createdDateTime</span></span>|<span data-ttu-id="150cf-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="150cf-165">DateTimeOffset</span></span>|<span data-ttu-id="150cf-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="150cf-166">DateTime the object was created.</span></span> <span data-ttu-id="150cf-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="150cf-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="150cf-168">description</span><span class="sxs-lookup"><span data-stu-id="150cf-168">description</span></span>|<span data-ttu-id="150cf-169">String</span><span class="sxs-lookup"><span data-stu-id="150cf-169">String</span></span>|<span data-ttu-id="150cf-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="150cf-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="150cf-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="150cf-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="150cf-172">displayName</span><span class="sxs-lookup"><span data-stu-id="150cf-172">displayName</span></span>|<span data-ttu-id="150cf-173">String</span><span class="sxs-lookup"><span data-stu-id="150cf-173">String</span></span>|<span data-ttu-id="150cf-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="150cf-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="150cf-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="150cf-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="150cf-176">version</span><span class="sxs-lookup"><span data-stu-id="150cf-176">version</span></span>|<span data-ttu-id="150cf-177">Int32</span><span class="sxs-lookup"><span data-stu-id="150cf-177">Int32</span></span>|<span data-ttu-id="150cf-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="150cf-178">Version of the device configuration.</span></span> <span data-ttu-id="150cf-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="150cf-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="150cf-180">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="150cf-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="150cf-181">Int32</span><span class="sxs-lookup"><span data-stu-id="150cf-181">Int32</span></span>|<span data-ttu-id="150cf-182">证书续订阈值百分比。</span><span class="sxs-lookup"><span data-stu-id="150cf-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="150cf-183">从[IosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)继承的有效值1到99</span><span class="sxs-lookup"><span data-stu-id="150cf-183">Valid values 1 to 99 Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="150cf-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="150cf-184">subjectNameFormat</span></span>|[<span data-ttu-id="150cf-185">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="150cf-185">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="150cf-186">证书使用者名称格式。</span><span class="sxs-lookup"><span data-stu-id="150cf-186">Certificate Subject Name Format.</span></span> <span data-ttu-id="150cf-187">继承自 [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="150cf-187">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="150cf-188">可取值为：`commonName`、`commonNameAsEmail`、`custom`、`commonNameIncludingEmail`、`commonNameAsIMEI`、`commonNameAsSerialNumber`。</span><span class="sxs-lookup"><span data-stu-id="150cf-188">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="150cf-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="150cf-189">subjectAlternativeNameType</span></span>|[<span data-ttu-id="150cf-190">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="150cf-190">subjectAlternativeNameType</span></span>](../resources/intune-shared-subjectalternativenametype.md)|<span data-ttu-id="150cf-191">证书使用者备用名称类型。</span><span class="sxs-lookup"><span data-stu-id="150cf-191">Certificate Subject Alternative Name type.</span></span> <span data-ttu-id="150cf-192">继承自 [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="150cf-192">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="150cf-193">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService`、`universalResourceIdentifier`。</span><span class="sxs-lookup"><span data-stu-id="150cf-193">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span></span>|
|<span data-ttu-id="150cf-194">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="150cf-194">certificateValidityPeriodValue</span></span>|<span data-ttu-id="150cf-195">Int32</span><span class="sxs-lookup"><span data-stu-id="150cf-195">Int32</span></span>|<span data-ttu-id="150cf-196">证书有效期限的值。</span><span class="sxs-lookup"><span data-stu-id="150cf-196">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="150cf-197">继承自 [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="150cf-197">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="150cf-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="150cf-198">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="150cf-199">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="150cf-199">certificateValidityPeriodScale</span></span>](../resources/intune-shared-certificatevalidityperiodscale.md)|<span data-ttu-id="150cf-200">证书有效期的小数位数。</span><span class="sxs-lookup"><span data-stu-id="150cf-200">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="150cf-201">继承自 [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="150cf-201">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="150cf-202">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="150cf-202">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="150cf-203">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="150cf-203">certificationAuthority</span></span>|<span data-ttu-id="150cf-204">String</span><span class="sxs-lookup"><span data-stu-id="150cf-204">String</span></span>|<span data-ttu-id="150cf-205">PKCS 证书颁发机构。</span><span class="sxs-lookup"><span data-stu-id="150cf-205">PKCS Certification Authority.</span></span>|
|<span data-ttu-id="150cf-206">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="150cf-206">certificationAuthorityName</span></span>|<span data-ttu-id="150cf-207">String</span><span class="sxs-lookup"><span data-stu-id="150cf-207">String</span></span>|<span data-ttu-id="150cf-208">PKCS 证书颁发机构名称。</span><span class="sxs-lookup"><span data-stu-id="150cf-208">PKCS Certification Authority Name.</span></span>|
|<span data-ttu-id="150cf-209">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="150cf-209">certificateTemplateName</span></span>|<span data-ttu-id="150cf-210">String</span><span class="sxs-lookup"><span data-stu-id="150cf-210">String</span></span>|<span data-ttu-id="150cf-211">PKCS 证书模板名称。</span><span class="sxs-lookup"><span data-stu-id="150cf-211">PKCS Certificate Template Name.</span></span>|
|<span data-ttu-id="150cf-212">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="150cf-212">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="150cf-213">String</span><span class="sxs-lookup"><span data-stu-id="150cf-213">String</span></span>|<span data-ttu-id="150cf-214">定义 AAD 属性的自定义字符串。</span><span class="sxs-lookup"><span data-stu-id="150cf-214">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="150cf-215">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="150cf-215">subjectNameFormatString</span></span>|<span data-ttu-id="150cf-216">String</span><span class="sxs-lookup"><span data-stu-id="150cf-216">String</span></span>|<span data-ttu-id="150cf-217">要与 SubjectNameFormat = Custom 一起使用的自定义格式。</span><span class="sxs-lookup"><span data-stu-id="150cf-217">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="150cf-218">示例： CN = {{EmailAddress}}，E = {{EmailAddress}}，OU = 企业用户，O = Contoso Corporation，L = Redmond，ST = WA，C = US</span><span class="sxs-lookup"><span data-stu-id="150cf-218">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="150cf-219">certificateStore</span><span class="sxs-lookup"><span data-stu-id="150cf-219">certificateStore</span></span>|[<span data-ttu-id="150cf-220">certificateStore</span><span class="sxs-lookup"><span data-stu-id="150cf-220">certificateStore</span></span>](../resources/intune-shared-certificatestore.md)|<span data-ttu-id="150cf-221">目标存储证书。</span><span class="sxs-lookup"><span data-stu-id="150cf-221">Target store certificate.</span></span> <span data-ttu-id="150cf-222">可取值为：`user`、`machine`。</span><span class="sxs-lookup"><span data-stu-id="150cf-222">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="150cf-223">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="150cf-223">customSubjectAlternativeNames</span></span>|<span data-ttu-id="150cf-224">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) 集合</span><span class="sxs-lookup"><span data-stu-id="150cf-224">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="150cf-225">自定义主题备用名称设置。</span><span class="sxs-lookup"><span data-stu-id="150cf-225">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="150cf-226">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="150cf-226">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="150cf-227">响应</span><span class="sxs-lookup"><span data-stu-id="150cf-227">Response</span></span>
<span data-ttu-id="150cf-228">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="150cf-228">If successful, this method returns a `201 Created` response code and a [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="150cf-229">示例</span><span class="sxs-lookup"><span data-stu-id="150cf-229">Example</span></span>

### <a name="request"></a><span data-ttu-id="150cf-230">请求</span><span class="sxs-lookup"><span data-stu-id="150cf-230">Request</span></span>
<span data-ttu-id="150cf-231">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="150cf-231">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1824

{
  "@odata.type": "#microsoft.graph.iosPkcsCertificateProfile",
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
  ]
}
```

### <a name="response"></a><span data-ttu-id="150cf-232">响应</span><span class="sxs-lookup"><span data-stu-id="150cf-232">Response</span></span>
<span data-ttu-id="150cf-p121">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="150cf-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1996

{
  "@odata.type": "#microsoft.graph.iosPkcsCertificateProfile",
  "id": "ed0264dd-64dd-ed02-dd64-02eddd6402ed",
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
  ]
}
```




