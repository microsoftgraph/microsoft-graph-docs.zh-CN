---
title: 创建 macOSScepCertificateProfile
description: 创建新的 macOSScepCertificateProfile 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0efe8def5afda0fce5515f53e05f206154436b89
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51132665"
---
# <a name="create-macosscepcertificateprofile"></a><span data-ttu-id="bdde7-103">创建 macOSScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="bdde7-103">Create macOSScepCertificateProfile</span></span>

<span data-ttu-id="bdde7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bdde7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bdde7-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bdde7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bdde7-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bdde7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bdde7-107">创建新的 [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bdde7-107">Create a new [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bdde7-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="bdde7-108">Prerequisites</span></span>
<span data-ttu-id="bdde7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bdde7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bdde7-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="bdde7-111">Permission type</span></span>|<span data-ttu-id="bdde7-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bdde7-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bdde7-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bdde7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bdde7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bdde7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bdde7-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bdde7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bdde7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bdde7-116">Not supported.</span></span>|
|<span data-ttu-id="bdde7-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="bdde7-117">Application</span></span>|<span data-ttu-id="bdde7-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bdde7-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bdde7-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bdde7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="bdde7-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="bdde7-120">Request headers</span></span>
|<span data-ttu-id="bdde7-121">标头</span><span class="sxs-lookup"><span data-stu-id="bdde7-121">Header</span></span>|<span data-ttu-id="bdde7-122">值</span><span class="sxs-lookup"><span data-stu-id="bdde7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bdde7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bdde7-123">Authorization</span></span>|<span data-ttu-id="bdde7-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="bdde7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bdde7-125">接受</span><span class="sxs-lookup"><span data-stu-id="bdde7-125">Accept</span></span>|<span data-ttu-id="bdde7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bdde7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bdde7-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="bdde7-127">Request body</span></span>
<span data-ttu-id="bdde7-128">在请求正文中，提供 macOSScepCertificateProfile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bdde7-128">In the request body, supply a JSON representation for the macOSScepCertificateProfile object.</span></span>

<span data-ttu-id="bdde7-129">下表显示创建 macOSScepCertificateProfile 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="bdde7-129">The following table shows the properties that are required when you create the macOSScepCertificateProfile.</span></span>

|<span data-ttu-id="bdde7-130">属性</span><span class="sxs-lookup"><span data-stu-id="bdde7-130">Property</span></span>|<span data-ttu-id="bdde7-131">类型</span><span class="sxs-lookup"><span data-stu-id="bdde7-131">Type</span></span>|<span data-ttu-id="bdde7-132">说明</span><span class="sxs-lookup"><span data-stu-id="bdde7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bdde7-133">id</span><span class="sxs-lookup"><span data-stu-id="bdde7-133">id</span></span>|<span data-ttu-id="bdde7-134">String</span><span class="sxs-lookup"><span data-stu-id="bdde7-134">String</span></span>|<span data-ttu-id="bdde7-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="bdde7-135">Key of the entity.</span></span> <span data-ttu-id="bdde7-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bdde7-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bdde7-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bdde7-137">lastModifiedDateTime</span></span>|<span data-ttu-id="bdde7-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bdde7-138">DateTimeOffset</span></span>|<span data-ttu-id="bdde7-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="bdde7-139">DateTime the object was last modified.</span></span> <span data-ttu-id="bdde7-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bdde7-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bdde7-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="bdde7-141">roleScopeTagIds</span></span>|<span data-ttu-id="bdde7-142">String collection</span><span class="sxs-lookup"><span data-stu-id="bdde7-142">String collection</span></span>|<span data-ttu-id="bdde7-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="bdde7-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="bdde7-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bdde7-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bdde7-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="bdde7-145">supportsScopeTags</span></span>|<span data-ttu-id="bdde7-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="bdde7-146">Boolean</span></span>|<span data-ttu-id="bdde7-147">指示基础设备配置是否支持分配范围标记。</span><span class="sxs-lookup"><span data-stu-id="bdde7-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="bdde7-148">当此值为 false 且实体对作用域用户不可见时，不允许分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="bdde7-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="bdde7-149">这适用于在 Silverlight 中创建的旧版策略，可通过在 Azure 门户中删除和重新创建策略来解决。</span><span class="sxs-lookup"><span data-stu-id="bdde7-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="bdde7-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="bdde7-150">This property is read-only.</span></span> <span data-ttu-id="bdde7-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bdde7-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bdde7-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="bdde7-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="bdde7-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="bdde7-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="bdde7-154">此策略的操作系统版本适用性。</span><span class="sxs-lookup"><span data-stu-id="bdde7-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="bdde7-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bdde7-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bdde7-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="bdde7-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="bdde7-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="bdde7-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="bdde7-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="bdde7-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="bdde7-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bdde7-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bdde7-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="bdde7-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="bdde7-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="bdde7-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="bdde7-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="bdde7-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="bdde7-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bdde7-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bdde7-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bdde7-164">createdDateTime</span></span>|<span data-ttu-id="bdde7-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bdde7-165">DateTimeOffset</span></span>|<span data-ttu-id="bdde7-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="bdde7-166">DateTime the object was created.</span></span> <span data-ttu-id="bdde7-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bdde7-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bdde7-168">说明</span><span class="sxs-lookup"><span data-stu-id="bdde7-168">description</span></span>|<span data-ttu-id="bdde7-169">String</span><span class="sxs-lookup"><span data-stu-id="bdde7-169">String</span></span>|<span data-ttu-id="bdde7-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="bdde7-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="bdde7-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bdde7-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bdde7-172">displayName</span><span class="sxs-lookup"><span data-stu-id="bdde7-172">displayName</span></span>|<span data-ttu-id="bdde7-173">String</span><span class="sxs-lookup"><span data-stu-id="bdde7-173">String</span></span>|<span data-ttu-id="bdde7-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="bdde7-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="bdde7-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bdde7-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bdde7-176">version</span><span class="sxs-lookup"><span data-stu-id="bdde7-176">version</span></span>|<span data-ttu-id="bdde7-177">Int32</span><span class="sxs-lookup"><span data-stu-id="bdde7-177">Int32</span></span>|<span data-ttu-id="bdde7-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="bdde7-178">Version of the device configuration.</span></span> <span data-ttu-id="bdde7-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bdde7-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bdde7-180">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="bdde7-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="bdde7-181">Int32</span><span class="sxs-lookup"><span data-stu-id="bdde7-181">Int32</span></span>|<span data-ttu-id="bdde7-182">证书续订阈值百分比。</span><span class="sxs-lookup"><span data-stu-id="bdde7-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="bdde7-183">继承自 [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="bdde7-183">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="bdde7-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="bdde7-184">subjectNameFormat</span></span>|[<span data-ttu-id="bdde7-185">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="bdde7-185">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="bdde7-186">证书主题名称格式。</span><span class="sxs-lookup"><span data-stu-id="bdde7-186">Certificate Subject Name Format.</span></span> <span data-ttu-id="bdde7-187">继承自 [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="bdde7-187">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="bdde7-188">可取值为：`commonName`、`commonNameAsEmail`、`custom`、`commonNameIncludingEmail`、`commonNameAsIMEI`、`commonNameAsSerialNumber`。</span><span class="sxs-lookup"><span data-stu-id="bdde7-188">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="bdde7-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="bdde7-189">subjectAlternativeNameType</span></span>|[<span data-ttu-id="bdde7-190">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="bdde7-190">subjectAlternativeNameType</span></span>](../resources/intune-shared-subjectalternativenametype.md)|<span data-ttu-id="bdde7-191">证书主题备用名称类型。</span><span class="sxs-lookup"><span data-stu-id="bdde7-191">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="bdde7-192">继承自 [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="bdde7-192">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="bdde7-193">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService`、`universalResourceIdentifier`。</span><span class="sxs-lookup"><span data-stu-id="bdde7-193">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span></span>|
|<span data-ttu-id="bdde7-194">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="bdde7-194">certificateValidityPeriodValue</span></span>|<span data-ttu-id="bdde7-195">Int32</span><span class="sxs-lookup"><span data-stu-id="bdde7-195">Int32</span></span>|<span data-ttu-id="bdde7-196">证书有效期的值。</span><span class="sxs-lookup"><span data-stu-id="bdde7-196">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="bdde7-197">继承自 [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="bdde7-197">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="bdde7-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="bdde7-198">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="bdde7-199">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="bdde7-199">certificateValidityPeriodScale</span></span>](../resources/intune-shared-certificatevalidityperiodscale.md)|<span data-ttu-id="bdde7-200">证书有效期的缩放。</span><span class="sxs-lookup"><span data-stu-id="bdde7-200">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="bdde7-201">继承自 [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="bdde7-201">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="bdde7-202">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="bdde7-202">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="bdde7-203">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="bdde7-203">scepServerUrls</span></span>|<span data-ttu-id="bdde7-204">String collection</span><span class="sxs-lookup"><span data-stu-id="bdde7-204">String collection</span></span>|<span data-ttu-id="bdde7-205">SCEP 服务器 URL () 。</span><span class="sxs-lookup"><span data-stu-id="bdde7-205">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="bdde7-206">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="bdde7-206">subjectNameFormatString</span></span>|<span data-ttu-id="bdde7-207">String</span><span class="sxs-lookup"><span data-stu-id="bdde7-207">String</span></span>|<span data-ttu-id="bdde7-208">要与 SubjectNameFormat 一同使用的自定义格式 = Custom。</span><span class="sxs-lookup"><span data-stu-id="bdde7-208">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="bdde7-209">示例：CN={{EmailAddress}}，E={{EmailAddress}，OU=Enterprise Users，O=Contoso Corporation，L=Redmond，ST=WA，C=US</span><span class="sxs-lookup"><span data-stu-id="bdde7-209">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="bdde7-210">keyUsage</span><span class="sxs-lookup"><span data-stu-id="bdde7-210">keyUsage</span></span>|[<span data-ttu-id="bdde7-211">keyUsages</span><span class="sxs-lookup"><span data-stu-id="bdde7-211">keyUsages</span></span>](../resources/intune-shared-keyusages.md)|<span data-ttu-id="bdde7-212">SCEP 密钥用法。</span><span class="sxs-lookup"><span data-stu-id="bdde7-212">SCEP Key Usage.</span></span> <span data-ttu-id="bdde7-213">可取值为：`keyEncipherment`、`digitalSignature`。</span><span class="sxs-lookup"><span data-stu-id="bdde7-213">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="bdde7-214">keySize</span><span class="sxs-lookup"><span data-stu-id="bdde7-214">keySize</span></span>|[<span data-ttu-id="bdde7-215">keySize</span><span class="sxs-lookup"><span data-stu-id="bdde7-215">keySize</span></span>](../resources/intune-shared-keysize.md)|<span data-ttu-id="bdde7-216">SCEP 密钥大小。</span><span class="sxs-lookup"><span data-stu-id="bdde7-216">SCEP Key Size.</span></span> <span data-ttu-id="bdde7-217">可取值为：`size1024`、`size2048`、`size4096`。</span><span class="sxs-lookup"><span data-stu-id="bdde7-217">Possible values are: `size1024`, `size2048`, `size4096`.</span></span>|
|<span data-ttu-id="bdde7-218">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="bdde7-218">hashAlgorithm</span></span>|[<span data-ttu-id="bdde7-219">hashAlgorithms</span><span class="sxs-lookup"><span data-stu-id="bdde7-219">hashAlgorithms</span></span>](../resources/intune-shared-hashalgorithms.md)|<span data-ttu-id="bdde7-220">SCEP 哈希算法。</span><span class="sxs-lookup"><span data-stu-id="bdde7-220">SCEP Hash Algorithm.</span></span> <span data-ttu-id="bdde7-221">可取值为：`sha1`、`sha2`。</span><span class="sxs-lookup"><span data-stu-id="bdde7-221">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="bdde7-222">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="bdde7-222">extendedKeyUsages</span></span>|<span data-ttu-id="bdde7-223">[extendedKeyUsage](../resources/intune-shared-extendedkeyusage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="bdde7-223">[extendedKeyUsage](../resources/intune-shared-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="bdde7-224">EKU (扩展密钥) 设置。</span><span class="sxs-lookup"><span data-stu-id="bdde7-224">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="bdde7-225">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="bdde7-225">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="bdde7-226">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="bdde7-226">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="bdde7-227">String</span><span class="sxs-lookup"><span data-stu-id="bdde7-227">String</span></span>|<span data-ttu-id="bdde7-228">定义 AAD 属性的自定义字符串。</span><span class="sxs-lookup"><span data-stu-id="bdde7-228">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="bdde7-229">certificateStore</span><span class="sxs-lookup"><span data-stu-id="bdde7-229">certificateStore</span></span>|[<span data-ttu-id="bdde7-230">certificateStore</span><span class="sxs-lookup"><span data-stu-id="bdde7-230">certificateStore</span></span>](../resources/intune-shared-certificatestore.md)|<span data-ttu-id="bdde7-231">目标存储证书。</span><span class="sxs-lookup"><span data-stu-id="bdde7-231">Target store certificate.</span></span> <span data-ttu-id="bdde7-232">可取值为：`user`、`machine`。</span><span class="sxs-lookup"><span data-stu-id="bdde7-232">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="bdde7-233">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="bdde7-233">customSubjectAlternativeNames</span></span>|<span data-ttu-id="bdde7-234">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) 集合</span><span class="sxs-lookup"><span data-stu-id="bdde7-234">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="bdde7-235">自定义主题备用名称设置。</span><span class="sxs-lookup"><span data-stu-id="bdde7-235">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="bdde7-236">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="bdde7-236">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="bdde7-237">响应</span><span class="sxs-lookup"><span data-stu-id="bdde7-237">Response</span></span>
<span data-ttu-id="bdde7-238">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bdde7-238">If successful, this method returns a `201 Created` response code and a [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bdde7-239">示例</span><span class="sxs-lookup"><span data-stu-id="bdde7-239">Example</span></span>

### <a name="request"></a><span data-ttu-id="bdde7-240">请求</span><span class="sxs-lookup"><span data-stu-id="bdde7-240">Request</span></span>
<span data-ttu-id="bdde7-241">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bdde7-241">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1962

{
  "@odata.type": "#microsoft.graph.macOSScepCertificateProfile",
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

### <a name="response"></a><span data-ttu-id="bdde7-242">响应</span><span class="sxs-lookup"><span data-stu-id="bdde7-242">Response</span></span>
<span data-ttu-id="bdde7-p125">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bdde7-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2134

{
  "@odata.type": "#microsoft.graph.macOSScepCertificateProfile",
  "id": "78c3929d-929d-78c3-9d92-c3789d92c378",
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




