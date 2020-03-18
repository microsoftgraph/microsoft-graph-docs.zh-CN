---
title: 更新 iosScepCertificateProfile
description: 更新 iosScepCertificateProfile 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: aa2a2db3a79a23f4030dd4e668b882f0e343e09e
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42749513"
---
# <a name="update-iosscepcertificateprofile"></a><span data-ttu-id="4695a-103">更新 iosScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="4695a-103">Update iosScepCertificateProfile</span></span>

> <span data-ttu-id="4695a-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4695a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4695a-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4695a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4695a-106">更新[iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4695a-106">Update the properties of a [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4695a-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="4695a-107">Prerequisites</span></span>
<span data-ttu-id="4695a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4695a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4695a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4695a-110">Permission type</span></span>|<span data-ttu-id="4695a-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4695a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4695a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4695a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4695a-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4695a-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4695a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4695a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4695a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4695a-115">Not supported.</span></span>|
|<span data-ttu-id="4695a-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="4695a-116">Application</span></span>|<span data-ttu-id="4695a-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4695a-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4695a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4695a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="4695a-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4695a-119">Request headers</span></span>
|<span data-ttu-id="4695a-120">标头</span><span class="sxs-lookup"><span data-stu-id="4695a-120">Header</span></span>|<span data-ttu-id="4695a-121">值</span><span class="sxs-lookup"><span data-stu-id="4695a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4695a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4695a-122">Authorization</span></span>|<span data-ttu-id="4695a-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4695a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4695a-124">接受</span><span class="sxs-lookup"><span data-stu-id="4695a-124">Accept</span></span>|<span data-ttu-id="4695a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4695a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4695a-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="4695a-126">Request body</span></span>
<span data-ttu-id="4695a-127">在请求正文中，提供[iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4695a-127">In the request body, supply a JSON representation for the [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) object.</span></span>

<span data-ttu-id="4695a-128">下表显示创建[iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="4695a-128">The following table shows the properties that are required when you create the [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md).</span></span>

|<span data-ttu-id="4695a-129">属性</span><span class="sxs-lookup"><span data-stu-id="4695a-129">Property</span></span>|<span data-ttu-id="4695a-130">类型</span><span class="sxs-lookup"><span data-stu-id="4695a-130">Type</span></span>|<span data-ttu-id="4695a-131">说明</span><span class="sxs-lookup"><span data-stu-id="4695a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4695a-132">id</span><span class="sxs-lookup"><span data-stu-id="4695a-132">id</span></span>|<span data-ttu-id="4695a-133">字符串</span><span class="sxs-lookup"><span data-stu-id="4695a-133">String</span></span>|<span data-ttu-id="4695a-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="4695a-134">Key of the entity.</span></span> <span data-ttu-id="4695a-135">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4695a-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4695a-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4695a-136">lastModifiedDateTime</span></span>|<span data-ttu-id="4695a-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4695a-137">DateTimeOffset</span></span>|<span data-ttu-id="4695a-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="4695a-138">DateTime the object was last modified.</span></span> <span data-ttu-id="4695a-139">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4695a-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4695a-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4695a-140">roleScopeTagIds</span></span>|<span data-ttu-id="4695a-141">String collection</span><span class="sxs-lookup"><span data-stu-id="4695a-141">String collection</span></span>|<span data-ttu-id="4695a-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="4695a-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4695a-143">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4695a-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4695a-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="4695a-144">supportsScopeTags</span></span>|<span data-ttu-id="4695a-145">布尔值</span><span class="sxs-lookup"><span data-stu-id="4695a-145">Boolean</span></span>|<span data-ttu-id="4695a-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="4695a-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="4695a-147">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="4695a-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="4695a-148">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="4695a-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="4695a-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4695a-149">This property is read-only.</span></span> <span data-ttu-id="4695a-150">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4695a-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4695a-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4695a-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="4695a-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4695a-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="4695a-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="4695a-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="4695a-154">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4695a-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4695a-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4695a-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="4695a-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4695a-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="4695a-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="4695a-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="4695a-158">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4695a-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4695a-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="4695a-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="4695a-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="4695a-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="4695a-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="4695a-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="4695a-162">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4695a-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4695a-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4695a-163">createdDateTime</span></span>|<span data-ttu-id="4695a-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4695a-164">DateTimeOffset</span></span>|<span data-ttu-id="4695a-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="4695a-165">DateTime the object was created.</span></span> <span data-ttu-id="4695a-166">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4695a-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4695a-167">说明</span><span class="sxs-lookup"><span data-stu-id="4695a-167">description</span></span>|<span data-ttu-id="4695a-168">String</span><span class="sxs-lookup"><span data-stu-id="4695a-168">String</span></span>|<span data-ttu-id="4695a-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="4695a-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4695a-170">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4695a-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4695a-171">displayName</span><span class="sxs-lookup"><span data-stu-id="4695a-171">displayName</span></span>|<span data-ttu-id="4695a-172">String</span><span class="sxs-lookup"><span data-stu-id="4695a-172">String</span></span>|<span data-ttu-id="4695a-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="4695a-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4695a-174">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4695a-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4695a-175">version</span><span class="sxs-lookup"><span data-stu-id="4695a-175">version</span></span>|<span data-ttu-id="4695a-176">Int32</span><span class="sxs-lookup"><span data-stu-id="4695a-176">Int32</span></span>|<span data-ttu-id="4695a-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="4695a-177">Version of the device configuration.</span></span> <span data-ttu-id="4695a-178">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4695a-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4695a-179">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="4695a-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="4695a-180">Int32</span><span class="sxs-lookup"><span data-stu-id="4695a-180">Int32</span></span>|<span data-ttu-id="4695a-181">证书续订阈值百分比。</span><span class="sxs-lookup"><span data-stu-id="4695a-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="4695a-182">从[IosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)继承的有效值1到99</span><span class="sxs-lookup"><span data-stu-id="4695a-182">Valid values 1 to 99 Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="4695a-183">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="4695a-183">subjectNameFormat</span></span>|[<span data-ttu-id="4695a-184">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="4695a-184">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="4695a-185">证书使用者名称格式。</span><span class="sxs-lookup"><span data-stu-id="4695a-185">Certificate Subject Name Format.</span></span> <span data-ttu-id="4695a-186">继承自[iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="4695a-186">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="4695a-187">可取值为：`commonName`、`commonNameAsEmail`、`custom`、`commonNameIncludingEmail`、`commonNameAsIMEI`、`commonNameAsSerialNumber`。</span><span class="sxs-lookup"><span data-stu-id="4695a-187">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="4695a-188">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="4695a-188">subjectAlternativeNameType</span></span>|[<span data-ttu-id="4695a-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="4695a-189">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="4695a-190">证书使用者备用名称类型。</span><span class="sxs-lookup"><span data-stu-id="4695a-190">Certificate Subject Alternative Name type.</span></span> <span data-ttu-id="4695a-191">继承自[iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="4695a-191">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="4695a-192">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService`。</span><span class="sxs-lookup"><span data-stu-id="4695a-192">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="4695a-193">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="4695a-193">certificateValidityPeriodValue</span></span>|<span data-ttu-id="4695a-194">Int32</span><span class="sxs-lookup"><span data-stu-id="4695a-194">Int32</span></span>|<span data-ttu-id="4695a-195">证书有效期限的值。</span><span class="sxs-lookup"><span data-stu-id="4695a-195">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="4695a-196">继承自[iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="4695a-196">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="4695a-197">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="4695a-197">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="4695a-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="4695a-198">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="4695a-199">证书有效期的小数位数。</span><span class="sxs-lookup"><span data-stu-id="4695a-199">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="4695a-200">继承自[iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="4695a-200">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="4695a-201">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="4695a-201">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="4695a-202">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="4695a-202">scepServerUrls</span></span>|<span data-ttu-id="4695a-203">String collection</span><span class="sxs-lookup"><span data-stu-id="4695a-203">String collection</span></span>|<span data-ttu-id="4695a-204">SCEP 服务器 Url。</span><span class="sxs-lookup"><span data-stu-id="4695a-204">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="4695a-205">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="4695a-205">subjectNameFormatString</span></span>|<span data-ttu-id="4695a-206">String</span><span class="sxs-lookup"><span data-stu-id="4695a-206">String</span></span>|<span data-ttu-id="4695a-207">要与 SubjectNameFormat = Custom 一起使用的自定义格式。</span><span class="sxs-lookup"><span data-stu-id="4695a-207">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="4695a-208">示例： CN = {{EmailAddress}}，E = {{EmailAddress}}，OU = 企业用户，O = Contoso Corporation，L = Redmond，ST = WA，C = US</span><span class="sxs-lookup"><span data-stu-id="4695a-208">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="4695a-209">keyUsage</span><span class="sxs-lookup"><span data-stu-id="4695a-209">keyUsage</span></span>|[<span data-ttu-id="4695a-210">keyUsages</span><span class="sxs-lookup"><span data-stu-id="4695a-210">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="4695a-211">SCEP 密钥用法。</span><span class="sxs-lookup"><span data-stu-id="4695a-211">SCEP Key Usage.</span></span> <span data-ttu-id="4695a-212">可取值为：`keyEncipherment`、`digitalSignature`。</span><span class="sxs-lookup"><span data-stu-id="4695a-212">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="4695a-213">keySize</span><span class="sxs-lookup"><span data-stu-id="4695a-213">keySize</span></span>|[<span data-ttu-id="4695a-214">keySize</span><span class="sxs-lookup"><span data-stu-id="4695a-214">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="4695a-215">SCEP 密钥大小。</span><span class="sxs-lookup"><span data-stu-id="4695a-215">SCEP Key Size.</span></span> <span data-ttu-id="4695a-216">可取值为：`size1024`、`size2048`。</span><span class="sxs-lookup"><span data-stu-id="4695a-216">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="4695a-217">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="4695a-217">extendedKeyUsages</span></span>|<span data-ttu-id="4695a-218">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)集合</span><span class="sxs-lookup"><span data-stu-id="4695a-218">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="4695a-219">扩展密钥用法（EKU）设置。</span><span class="sxs-lookup"><span data-stu-id="4695a-219">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="4695a-220">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="4695a-220">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="4695a-221">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="4695a-221">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="4695a-222">String</span><span class="sxs-lookup"><span data-stu-id="4695a-222">String</span></span>|<span data-ttu-id="4695a-223">定义 AAD 属性的自定义字符串。</span><span class="sxs-lookup"><span data-stu-id="4695a-223">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="4695a-224">certificateStore</span><span class="sxs-lookup"><span data-stu-id="4695a-224">certificateStore</span></span>|[<span data-ttu-id="4695a-225">certificateStore</span><span class="sxs-lookup"><span data-stu-id="4695a-225">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="4695a-226">目标存储证书。</span><span class="sxs-lookup"><span data-stu-id="4695a-226">Target store certificate.</span></span> <span data-ttu-id="4695a-227">可取值为：`user`、`machine`。</span><span class="sxs-lookup"><span data-stu-id="4695a-227">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="4695a-228">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="4695a-228">customSubjectAlternativeNames</span></span>|<span data-ttu-id="4695a-229">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)集合</span><span class="sxs-lookup"><span data-stu-id="4695a-229">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="4695a-230">自定义主题备用名称设置。</span><span class="sxs-lookup"><span data-stu-id="4695a-230">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="4695a-231">OnPremisesUserPrincipalName 变量支持以及此处记录的其他变量： https://go.microsoft.com/fwlink/?LinkId=2027630。</span><span class="sxs-lookup"><span data-stu-id="4695a-231">The OnPremisesUserPrincipalName variable is support as well as others documented here: https://go.microsoft.com/fwlink/?LinkId=2027630.</span></span> <span data-ttu-id="4695a-232">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="4695a-232">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="4695a-233">响应</span><span class="sxs-lookup"><span data-stu-id="4695a-233">Response</span></span>
<span data-ttu-id="4695a-234">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4695a-234">If successful, this method returns a `200 OK` response code and an updated [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4695a-235">示例</span><span class="sxs-lookup"><span data-stu-id="4695a-235">Example</span></span>

### <a name="request"></a><span data-ttu-id="4695a-236">请求</span><span class="sxs-lookup"><span data-stu-id="4695a-236">Request</span></span>
<span data-ttu-id="4695a-237">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4695a-237">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1932

{
  "@odata.type": "#microsoft.graph.iosScepCertificateProfile",
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

### <a name="response"></a><span data-ttu-id="4695a-238">响应</span><span class="sxs-lookup"><span data-stu-id="4695a-238">Response</span></span>
<span data-ttu-id="4695a-p124">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4695a-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2104

{
  "@odata.type": "#microsoft.graph.iosScepCertificateProfile",
  "id": "0deb8dbf-8dbf-0deb-bf8d-eb0dbf8deb0d",
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




