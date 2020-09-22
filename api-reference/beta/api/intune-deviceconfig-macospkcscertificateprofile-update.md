---
title: 更新 macOSPkcsCertificateProfile
description: 更新 macOSPkcsCertificateProfile 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 792b5b0b547bfaaac04bff5ddf299251896b2ae3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48054565"
---
# <a name="update-macospkcscertificateprofile"></a><span data-ttu-id="7868a-103">更新 macOSPkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="7868a-103">Update macOSPkcsCertificateProfile</span></span>

<span data-ttu-id="7868a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7868a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7868a-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7868a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7868a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7868a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7868a-107">更新 [macOSPkcsCertificateProfile](../resources/intune-deviceconfig-macospkcscertificateprofile.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="7868a-107">Update the properties of a [macOSPkcsCertificateProfile](../resources/intune-deviceconfig-macospkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7868a-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="7868a-108">Prerequisites</span></span>
<span data-ttu-id="7868a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7868a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7868a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7868a-111">Permission type</span></span>|<span data-ttu-id="7868a-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7868a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7868a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7868a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7868a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7868a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7868a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7868a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7868a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7868a-116">Not supported.</span></span>|
|<span data-ttu-id="7868a-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="7868a-117">Application</span></span>|<span data-ttu-id="7868a-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7868a-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7868a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7868a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="7868a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="7868a-120">Request headers</span></span>
|<span data-ttu-id="7868a-121">标头</span><span class="sxs-lookup"><span data-stu-id="7868a-121">Header</span></span>|<span data-ttu-id="7868a-122">值</span><span class="sxs-lookup"><span data-stu-id="7868a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7868a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7868a-123">Authorization</span></span>|<span data-ttu-id="7868a-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7868a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7868a-125">接受</span><span class="sxs-lookup"><span data-stu-id="7868a-125">Accept</span></span>|<span data-ttu-id="7868a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7868a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7868a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7868a-127">Request body</span></span>
<span data-ttu-id="7868a-128">在请求正文中，提供 [macOSPkcsCertificateProfile](../resources/intune-deviceconfig-macospkcscertificateprofile.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7868a-128">In the request body, supply a JSON representation for the [macOSPkcsCertificateProfile](../resources/intune-deviceconfig-macospkcscertificateprofile.md) object.</span></span>

<span data-ttu-id="7868a-129">下表显示创建 [macOSPkcsCertificateProfile](../resources/intune-deviceconfig-macospkcscertificateprofile.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="7868a-129">The following table shows the properties that are required when you create the [macOSPkcsCertificateProfile](../resources/intune-deviceconfig-macospkcscertificateprofile.md).</span></span>

|<span data-ttu-id="7868a-130">属性</span><span class="sxs-lookup"><span data-stu-id="7868a-130">Property</span></span>|<span data-ttu-id="7868a-131">类型</span><span class="sxs-lookup"><span data-stu-id="7868a-131">Type</span></span>|<span data-ttu-id="7868a-132">说明</span><span class="sxs-lookup"><span data-stu-id="7868a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7868a-133">id</span><span class="sxs-lookup"><span data-stu-id="7868a-133">id</span></span>|<span data-ttu-id="7868a-134">String</span><span class="sxs-lookup"><span data-stu-id="7868a-134">String</span></span>|<span data-ttu-id="7868a-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="7868a-135">Key of the entity.</span></span> <span data-ttu-id="7868a-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7868a-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7868a-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7868a-137">lastModifiedDateTime</span></span>|<span data-ttu-id="7868a-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7868a-138">DateTimeOffset</span></span>|<span data-ttu-id="7868a-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="7868a-139">DateTime the object was last modified.</span></span> <span data-ttu-id="7868a-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7868a-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7868a-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7868a-141">roleScopeTagIds</span></span>|<span data-ttu-id="7868a-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="7868a-142">String collection</span></span>|<span data-ttu-id="7868a-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="7868a-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="7868a-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7868a-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7868a-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="7868a-145">supportsScopeTags</span></span>|<span data-ttu-id="7868a-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="7868a-146">Boolean</span></span>|<span data-ttu-id="7868a-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="7868a-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="7868a-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="7868a-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="7868a-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="7868a-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="7868a-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="7868a-150">This property is read-only.</span></span> <span data-ttu-id="7868a-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7868a-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7868a-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="7868a-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="7868a-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="7868a-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="7868a-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="7868a-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="7868a-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7868a-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7868a-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="7868a-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="7868a-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="7868a-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="7868a-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="7868a-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="7868a-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7868a-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7868a-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="7868a-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="7868a-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="7868a-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="7868a-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="7868a-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="7868a-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7868a-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7868a-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7868a-164">createdDateTime</span></span>|<span data-ttu-id="7868a-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7868a-165">DateTimeOffset</span></span>|<span data-ttu-id="7868a-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="7868a-166">DateTime the object was created.</span></span> <span data-ttu-id="7868a-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7868a-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7868a-168">说明</span><span class="sxs-lookup"><span data-stu-id="7868a-168">description</span></span>|<span data-ttu-id="7868a-169">String</span><span class="sxs-lookup"><span data-stu-id="7868a-169">String</span></span>|<span data-ttu-id="7868a-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="7868a-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7868a-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7868a-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7868a-172">displayName</span><span class="sxs-lookup"><span data-stu-id="7868a-172">displayName</span></span>|<span data-ttu-id="7868a-173">String</span><span class="sxs-lookup"><span data-stu-id="7868a-173">String</span></span>|<span data-ttu-id="7868a-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="7868a-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7868a-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7868a-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7868a-176">version</span><span class="sxs-lookup"><span data-stu-id="7868a-176">version</span></span>|<span data-ttu-id="7868a-177">Int32</span><span class="sxs-lookup"><span data-stu-id="7868a-177">Int32</span></span>|<span data-ttu-id="7868a-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="7868a-178">Version of the device configuration.</span></span> <span data-ttu-id="7868a-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7868a-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7868a-180">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="7868a-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="7868a-181">Int32</span><span class="sxs-lookup"><span data-stu-id="7868a-181">Int32</span></span>|<span data-ttu-id="7868a-182">证书续订阈值百分比。</span><span class="sxs-lookup"><span data-stu-id="7868a-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="7868a-183">继承自 [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="7868a-183">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="7868a-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="7868a-184">subjectNameFormat</span></span>|[<span data-ttu-id="7868a-185">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="7868a-185">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="7868a-186">证书使用者名称格式。</span><span class="sxs-lookup"><span data-stu-id="7868a-186">Certificate Subject Name Format.</span></span> <span data-ttu-id="7868a-187">继承自 [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="7868a-187">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="7868a-188">可取值为：`commonName`、`commonNameAsEmail`、`custom`、`commonNameIncludingEmail`、`commonNameAsIMEI`、`commonNameAsSerialNumber`。</span><span class="sxs-lookup"><span data-stu-id="7868a-188">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="7868a-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="7868a-189">subjectAlternativeNameType</span></span>|[<span data-ttu-id="7868a-190">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="7868a-190">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="7868a-191">证书使用者备用名称类型。</span><span class="sxs-lookup"><span data-stu-id="7868a-191">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="7868a-192">继承自 [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="7868a-192">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="7868a-193">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService`。</span><span class="sxs-lookup"><span data-stu-id="7868a-193">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="7868a-194">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="7868a-194">certificateValidityPeriodValue</span></span>|<span data-ttu-id="7868a-195">Int32</span><span class="sxs-lookup"><span data-stu-id="7868a-195">Int32</span></span>|<span data-ttu-id="7868a-196">证书有效期限的值。</span><span class="sxs-lookup"><span data-stu-id="7868a-196">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="7868a-197">继承自 [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="7868a-197">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="7868a-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="7868a-198">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="7868a-199">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="7868a-199">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="7868a-200">证书有效期的小数位数。</span><span class="sxs-lookup"><span data-stu-id="7868a-200">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="7868a-201">继承自 [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="7868a-201">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="7868a-202">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="7868a-202">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="7868a-203">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="7868a-203">certificationAuthority</span></span>|<span data-ttu-id="7868a-204">String</span><span class="sxs-lookup"><span data-stu-id="7868a-204">String</span></span>|<span data-ttu-id="7868a-205">PKCS 证书颁发机构 FQDN。</span><span class="sxs-lookup"><span data-stu-id="7868a-205">PKCS certification authority FQDN.</span></span>|
|<span data-ttu-id="7868a-206">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="7868a-206">certificationAuthorityName</span></span>|<span data-ttu-id="7868a-207">String</span><span class="sxs-lookup"><span data-stu-id="7868a-207">String</span></span>|<span data-ttu-id="7868a-208">PKCS 证书颁发机构名称。</span><span class="sxs-lookup"><span data-stu-id="7868a-208">PKCS certification authority Name.</span></span>|
|<span data-ttu-id="7868a-209">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="7868a-209">certificateTemplateName</span></span>|<span data-ttu-id="7868a-210">String</span><span class="sxs-lookup"><span data-stu-id="7868a-210">String</span></span>|<span data-ttu-id="7868a-211">PKCS 证书模板名称。</span><span class="sxs-lookup"><span data-stu-id="7868a-211">PKCS certificate template name.</span></span>|
|<span data-ttu-id="7868a-212">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="7868a-212">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="7868a-213">String</span><span class="sxs-lookup"><span data-stu-id="7868a-213">String</span></span>|<span data-ttu-id="7868a-214">定义使用者可选名称的格式字符串。</span><span class="sxs-lookup"><span data-stu-id="7868a-214">Format string that defines the subject alternative name.</span></span>|
|<span data-ttu-id="7868a-215">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="7868a-215">subjectNameFormatString</span></span>|<span data-ttu-id="7868a-216">String</span><span class="sxs-lookup"><span data-stu-id="7868a-216">String</span></span>|<span data-ttu-id="7868a-217">定义主题名称的格式字符串。</span><span class="sxs-lookup"><span data-stu-id="7868a-217">Format string that defines the subject name.</span></span> <span data-ttu-id="7868a-218">示例： CN = {{EmailAddress}}，E = {{EmailAddress}}，OU = 企业用户，O = Contoso Corporation，L = Redmond，ST = WA，C = US</span><span class="sxs-lookup"><span data-stu-id="7868a-218">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="7868a-219">certificateStore</span><span class="sxs-lookup"><span data-stu-id="7868a-219">certificateStore</span></span>|[<span data-ttu-id="7868a-220">certificateStore</span><span class="sxs-lookup"><span data-stu-id="7868a-220">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="7868a-221">目标存储证书。</span><span class="sxs-lookup"><span data-stu-id="7868a-221">Target store certificate.</span></span> <span data-ttu-id="7868a-222">可取值为：`user`、`machine`。</span><span class="sxs-lookup"><span data-stu-id="7868a-222">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="7868a-223">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="7868a-223">customSubjectAlternativeNames</span></span>|<span data-ttu-id="7868a-224">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7868a-224">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="7868a-225">自定义主题备用名称设置。</span><span class="sxs-lookup"><span data-stu-id="7868a-225">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="7868a-226">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="7868a-226">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="7868a-227">allowAllAppsAccess</span><span class="sxs-lookup"><span data-stu-id="7868a-227">allowAllAppsAccess</span></span>|<span data-ttu-id="7868a-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="7868a-228">Boolean</span></span>|<span data-ttu-id="7868a-229">AllowAllAppsAccess 设置</span><span class="sxs-lookup"><span data-stu-id="7868a-229">AllowAllAppsAccess setting</span></span>|



## <a name="response"></a><span data-ttu-id="7868a-230">响应</span><span class="sxs-lookup"><span data-stu-id="7868a-230">Response</span></span>
<span data-ttu-id="7868a-231">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [macOSPkcsCertificateProfile](../resources/intune-deviceconfig-macospkcscertificateprofile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7868a-231">If successful, this method returns a `200 OK` response code and an updated [macOSPkcsCertificateProfile](../resources/intune-deviceconfig-macospkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7868a-232">示例</span><span class="sxs-lookup"><span data-stu-id="7868a-232">Example</span></span>

### <a name="request"></a><span data-ttu-id="7868a-233">请求</span><span class="sxs-lookup"><span data-stu-id="7868a-233">Request</span></span>
<span data-ttu-id="7868a-234">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7868a-234">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="7868a-235">响应</span><span class="sxs-lookup"><span data-stu-id="7868a-235">Response</span></span>
<span data-ttu-id="7868a-p121">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7868a-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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






