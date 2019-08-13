---
title: 更新 macOSScepCertificateProfile
description: 更新 macOSScepCertificateProfile 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ceefc04c91b8fe424f382eab3b317f42ded00e17
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36315160"
---
# <a name="update-macosscepcertificateprofile"></a><span data-ttu-id="4cddd-103">更新 macOSScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="4cddd-103">Update macOSScepCertificateProfile</span></span>

> <span data-ttu-id="4cddd-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4cddd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4cddd-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4cddd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4cddd-106">更新[macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4cddd-106">Update the properties of a [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4cddd-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="4cddd-107">Prerequisites</span></span>
<span data-ttu-id="4cddd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4cddd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4cddd-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4cddd-110">Permission type</span></span>|<span data-ttu-id="4cddd-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4cddd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4cddd-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4cddd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4cddd-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4cddd-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4cddd-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4cddd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4cddd-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4cddd-115">Not supported.</span></span>|
|<span data-ttu-id="4cddd-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="4cddd-116">Application</span></span>|<span data-ttu-id="4cddd-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4cddd-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4cddd-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4cddd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="4cddd-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4cddd-119">Request headers</span></span>
|<span data-ttu-id="4cddd-120">标头</span><span class="sxs-lookup"><span data-stu-id="4cddd-120">Header</span></span>|<span data-ttu-id="4cddd-121">值</span><span class="sxs-lookup"><span data-stu-id="4cddd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4cddd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4cddd-122">Authorization</span></span>|<span data-ttu-id="4cddd-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4cddd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4cddd-124">接受</span><span class="sxs-lookup"><span data-stu-id="4cddd-124">Accept</span></span>|<span data-ttu-id="4cddd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4cddd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4cddd-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="4cddd-126">Request body</span></span>
<span data-ttu-id="4cddd-127">在请求正文中, 提供[macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4cddd-127">In the request body, supply a JSON representation for the [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) object.</span></span>

<span data-ttu-id="4cddd-128">下表显示创建[macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="4cddd-128">The following table shows the properties that are required when you create the [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md).</span></span>

|<span data-ttu-id="4cddd-129">属性</span><span class="sxs-lookup"><span data-stu-id="4cddd-129">Property</span></span>|<span data-ttu-id="4cddd-130">类型</span><span class="sxs-lookup"><span data-stu-id="4cddd-130">Type</span></span>|<span data-ttu-id="4cddd-131">说明</span><span class="sxs-lookup"><span data-stu-id="4cddd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4cddd-132">id</span><span class="sxs-lookup"><span data-stu-id="4cddd-132">id</span></span>|<span data-ttu-id="4cddd-133">字符串</span><span class="sxs-lookup"><span data-stu-id="4cddd-133">String</span></span>|<span data-ttu-id="4cddd-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="4cddd-134">Key of the entity.</span></span> <span data-ttu-id="4cddd-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4cddd-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4cddd-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4cddd-136">lastModifiedDateTime</span></span>|<span data-ttu-id="4cddd-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4cddd-137">DateTimeOffset</span></span>|<span data-ttu-id="4cddd-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="4cddd-138">DateTime the object was last modified.</span></span> <span data-ttu-id="4cddd-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4cddd-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4cddd-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4cddd-140">roleScopeTagIds</span></span>|<span data-ttu-id="4cddd-141">String collection</span><span class="sxs-lookup"><span data-stu-id="4cddd-141">String collection</span></span>|<span data-ttu-id="4cddd-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="4cddd-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4cddd-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4cddd-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4cddd-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="4cddd-144">supportsScopeTags</span></span>|<span data-ttu-id="4cddd-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="4cddd-145">Boolean</span></span>|<span data-ttu-id="4cddd-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="4cddd-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="4cddd-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="4cddd-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="4cddd-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="4cddd-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="4cddd-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4cddd-149">This property is read-only.</span></span> <span data-ttu-id="4cddd-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4cddd-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4cddd-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4cddd-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="4cddd-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4cddd-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="4cddd-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="4cddd-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="4cddd-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4cddd-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4cddd-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4cddd-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="4cddd-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4cddd-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="4cddd-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="4cddd-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="4cddd-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4cddd-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4cddd-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="4cddd-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="4cddd-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="4cddd-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="4cddd-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="4cddd-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="4cddd-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4cddd-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4cddd-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4cddd-163">createdDateTime</span></span>|<span data-ttu-id="4cddd-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4cddd-164">DateTimeOffset</span></span>|<span data-ttu-id="4cddd-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="4cddd-165">DateTime the object was created.</span></span> <span data-ttu-id="4cddd-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4cddd-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4cddd-167">说明</span><span class="sxs-lookup"><span data-stu-id="4cddd-167">description</span></span>|<span data-ttu-id="4cddd-168">String</span><span class="sxs-lookup"><span data-stu-id="4cddd-168">String</span></span>|<span data-ttu-id="4cddd-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="4cddd-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4cddd-170">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4cddd-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4cddd-171">displayName</span><span class="sxs-lookup"><span data-stu-id="4cddd-171">displayName</span></span>|<span data-ttu-id="4cddd-172">String</span><span class="sxs-lookup"><span data-stu-id="4cddd-172">String</span></span>|<span data-ttu-id="4cddd-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="4cddd-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4cddd-174">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4cddd-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4cddd-175">version</span><span class="sxs-lookup"><span data-stu-id="4cddd-175">version</span></span>|<span data-ttu-id="4cddd-176">Int32</span><span class="sxs-lookup"><span data-stu-id="4cddd-176">Int32</span></span>|<span data-ttu-id="4cddd-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="4cddd-177">Version of the device configuration.</span></span> <span data-ttu-id="4cddd-178">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4cddd-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4cddd-179">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="4cddd-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="4cddd-180">Int32</span><span class="sxs-lookup"><span data-stu-id="4cddd-180">Int32</span></span>|<span data-ttu-id="4cddd-181">证书续订阈值百分比。</span><span class="sxs-lookup"><span data-stu-id="4cddd-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="4cddd-182">继承自[macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="4cddd-182">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="4cddd-183">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="4cddd-183">subjectNameFormat</span></span>|[<span data-ttu-id="4cddd-184">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="4cddd-184">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="4cddd-185">证书使用者名称格式。</span><span class="sxs-lookup"><span data-stu-id="4cddd-185">Certificate Subject Name Format.</span></span> <span data-ttu-id="4cddd-186">继承自[macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="4cddd-186">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="4cddd-187">可取值为：`commonName`、`commonNameAsEmail`、`custom`、`commonNameIncludingEmail`、`commonNameAsIMEI`、`commonNameAsSerialNumber`。</span><span class="sxs-lookup"><span data-stu-id="4cddd-187">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="4cddd-188">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="4cddd-188">subjectAlternativeNameType</span></span>|[<span data-ttu-id="4cddd-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="4cddd-189">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="4cddd-190">证书使用者备用名称类型。</span><span class="sxs-lookup"><span data-stu-id="4cddd-190">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="4cddd-191">继承自[macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="4cddd-191">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="4cddd-192">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService`。</span><span class="sxs-lookup"><span data-stu-id="4cddd-192">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="4cddd-193">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="4cddd-193">certificateValidityPeriodValue</span></span>|<span data-ttu-id="4cddd-194">Int32</span><span class="sxs-lookup"><span data-stu-id="4cddd-194">Int32</span></span>|<span data-ttu-id="4cddd-195">证书有效期限的值。</span><span class="sxs-lookup"><span data-stu-id="4cddd-195">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="4cddd-196">继承自[macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="4cddd-196">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="4cddd-197">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="4cddd-197">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="4cddd-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="4cddd-198">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="4cddd-199">证书有效期的小数位数。</span><span class="sxs-lookup"><span data-stu-id="4cddd-199">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="4cddd-200">继承自[macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="4cddd-200">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="4cddd-201">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="4cddd-201">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="4cddd-202">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="4cddd-202">scepServerUrls</span></span>|<span data-ttu-id="4cddd-203">String collection</span><span class="sxs-lookup"><span data-stu-id="4cddd-203">String collection</span></span>|<span data-ttu-id="4cddd-204">SCEP 服务器 Url。</span><span class="sxs-lookup"><span data-stu-id="4cddd-204">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="4cddd-205">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="4cddd-205">subjectNameFormatString</span></span>|<span data-ttu-id="4cddd-206">String</span><span class="sxs-lookup"><span data-stu-id="4cddd-206">String</span></span>|<span data-ttu-id="4cddd-207">要与 SubjectNameFormat = Custom 一起使用的自定义格式。</span><span class="sxs-lookup"><span data-stu-id="4cddd-207">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="4cddd-208">示例: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = 企业用户, O = Contoso Corporation, L = Redmond, ST = WA, C = US</span><span class="sxs-lookup"><span data-stu-id="4cddd-208">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="4cddd-209">keyUsage</span><span class="sxs-lookup"><span data-stu-id="4cddd-209">keyUsage</span></span>|[<span data-ttu-id="4cddd-210">keyUsages</span><span class="sxs-lookup"><span data-stu-id="4cddd-210">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="4cddd-211">SCEP 密钥用法。</span><span class="sxs-lookup"><span data-stu-id="4cddd-211">SCEP Key Usage.</span></span> <span data-ttu-id="4cddd-212">可取值为：`keyEncipherment`、`digitalSignature`。</span><span class="sxs-lookup"><span data-stu-id="4cddd-212">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="4cddd-213">keySize</span><span class="sxs-lookup"><span data-stu-id="4cddd-213">keySize</span></span>|[<span data-ttu-id="4cddd-214">keySize</span><span class="sxs-lookup"><span data-stu-id="4cddd-214">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="4cddd-215">SCEP 密钥大小。</span><span class="sxs-lookup"><span data-stu-id="4cddd-215">SCEP Key Size.</span></span> <span data-ttu-id="4cddd-216">可取值为：`size1024`、`size2048`。</span><span class="sxs-lookup"><span data-stu-id="4cddd-216">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="4cddd-217">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="4cddd-217">hashAlgorithm</span></span>|[<span data-ttu-id="4cddd-218">hashAlgorithms</span><span class="sxs-lookup"><span data-stu-id="4cddd-218">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="4cddd-219">SCEP 哈希算法。</span><span class="sxs-lookup"><span data-stu-id="4cddd-219">SCEP Hash Algorithm.</span></span> <span data-ttu-id="4cddd-220">可取值为：`sha1`、`sha2`。</span><span class="sxs-lookup"><span data-stu-id="4cddd-220">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="4cddd-221">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="4cddd-221">extendedKeyUsages</span></span>|<span data-ttu-id="4cddd-222">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)集合</span><span class="sxs-lookup"><span data-stu-id="4cddd-222">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="4cddd-223">扩展密钥用法 (EKU) 设置。</span><span class="sxs-lookup"><span data-stu-id="4cddd-223">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="4cddd-224">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="4cddd-224">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="4cddd-225">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="4cddd-225">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="4cddd-226">String</span><span class="sxs-lookup"><span data-stu-id="4cddd-226">String</span></span>|<span data-ttu-id="4cddd-227">定义 AAD 属性的自定义字符串。</span><span class="sxs-lookup"><span data-stu-id="4cddd-227">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="4cddd-228">certificateStore</span><span class="sxs-lookup"><span data-stu-id="4cddd-228">certificateStore</span></span>|[<span data-ttu-id="4cddd-229">certificateStore</span><span class="sxs-lookup"><span data-stu-id="4cddd-229">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="4cddd-230">目标存储证书。</span><span class="sxs-lookup"><span data-stu-id="4cddd-230">Target store certificate.</span></span> <span data-ttu-id="4cddd-231">可取值为：`user`、`machine`。</span><span class="sxs-lookup"><span data-stu-id="4cddd-231">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="4cddd-232">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="4cddd-232">customSubjectAlternativeNames</span></span>|<span data-ttu-id="4cddd-233">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)集合</span><span class="sxs-lookup"><span data-stu-id="4cddd-233">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="4cddd-234">自定义主题备用名称设置。</span><span class="sxs-lookup"><span data-stu-id="4cddd-234">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="4cddd-235">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="4cddd-235">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="4cddd-236">响应</span><span class="sxs-lookup"><span data-stu-id="4cddd-236">Response</span></span>
<span data-ttu-id="4cddd-237">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4cddd-237">If successful, this method returns a `200 OK` response code and an updated [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4cddd-238">示例</span><span class="sxs-lookup"><span data-stu-id="4cddd-238">Example</span></span>

### <a name="request"></a><span data-ttu-id="4cddd-239">请求</span><span class="sxs-lookup"><span data-stu-id="4cddd-239">Request</span></span>
<span data-ttu-id="4cddd-240">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4cddd-240">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="4cddd-241">响应</span><span class="sxs-lookup"><span data-stu-id="4cddd-241">Response</span></span>
<span data-ttu-id="4cddd-p125">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4cddd-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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






