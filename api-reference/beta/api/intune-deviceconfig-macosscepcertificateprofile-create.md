---
title: 创建 macOSScepCertificateProfile
description: 创建新的 macOSScepCertificateProfile 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9c42c15d5b6dc6c5b7dc3edc0cb472298a91576d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35947115"
---
# <a name="create-macosscepcertificateprofile"></a><span data-ttu-id="ddcfb-103">创建 macOSScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="ddcfb-103">Create macOSScepCertificateProfile</span></span>

> <span data-ttu-id="ddcfb-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ddcfb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ddcfb-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ddcfb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ddcfb-106">创建新的[macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ddcfb-106">Create a new [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ddcfb-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="ddcfb-107">Prerequisites</span></span>
<span data-ttu-id="ddcfb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ddcfb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ddcfb-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ddcfb-110">Permission type</span></span>|<span data-ttu-id="ddcfb-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ddcfb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ddcfb-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ddcfb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ddcfb-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ddcfb-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ddcfb-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ddcfb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ddcfb-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ddcfb-115">Not supported.</span></span>|
|<span data-ttu-id="ddcfb-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ddcfb-116">Application</span></span>|<span data-ttu-id="ddcfb-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="ddcfb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ddcfb-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ddcfb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ddcfb-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ddcfb-119">Request headers</span></span>
|<span data-ttu-id="ddcfb-120">标头</span><span class="sxs-lookup"><span data-stu-id="ddcfb-120">Header</span></span>|<span data-ttu-id="ddcfb-121">值</span><span class="sxs-lookup"><span data-stu-id="ddcfb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ddcfb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ddcfb-122">Authorization</span></span>|<span data-ttu-id="ddcfb-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ddcfb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ddcfb-124">接受</span><span class="sxs-lookup"><span data-stu-id="ddcfb-124">Accept</span></span>|<span data-ttu-id="ddcfb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ddcfb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ddcfb-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ddcfb-126">Request body</span></span>
<span data-ttu-id="ddcfb-127">在请求正文中, 提供 macOSScepCertificateProfile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ddcfb-127">In the request body, supply a JSON representation for the macOSScepCertificateProfile object.</span></span>

<span data-ttu-id="ddcfb-128">下表显示创建 macOSScepCertificateProfile 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ddcfb-128">The following table shows the properties that are required when you create the macOSScepCertificateProfile.</span></span>

|<span data-ttu-id="ddcfb-129">属性</span><span class="sxs-lookup"><span data-stu-id="ddcfb-129">Property</span></span>|<span data-ttu-id="ddcfb-130">类型</span><span class="sxs-lookup"><span data-stu-id="ddcfb-130">Type</span></span>|<span data-ttu-id="ddcfb-131">说明</span><span class="sxs-lookup"><span data-stu-id="ddcfb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ddcfb-132">id</span><span class="sxs-lookup"><span data-stu-id="ddcfb-132">id</span></span>|<span data-ttu-id="ddcfb-133">字符串</span><span class="sxs-lookup"><span data-stu-id="ddcfb-133">String</span></span>|<span data-ttu-id="ddcfb-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="ddcfb-134">Key of the entity.</span></span> <span data-ttu-id="ddcfb-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ddcfb-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ddcfb-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ddcfb-136">lastModifiedDateTime</span></span>|<span data-ttu-id="ddcfb-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ddcfb-137">DateTimeOffset</span></span>|<span data-ttu-id="ddcfb-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="ddcfb-138">DateTime the object was last modified.</span></span> <span data-ttu-id="ddcfb-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ddcfb-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ddcfb-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ddcfb-140">roleScopeTagIds</span></span>|<span data-ttu-id="ddcfb-141">String collection</span><span class="sxs-lookup"><span data-stu-id="ddcfb-141">String collection</span></span>|<span data-ttu-id="ddcfb-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="ddcfb-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ddcfb-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ddcfb-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ddcfb-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ddcfb-144">supportsScopeTags</span></span>|<span data-ttu-id="ddcfb-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddcfb-145">Boolean</span></span>|<span data-ttu-id="ddcfb-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="ddcfb-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ddcfb-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="ddcfb-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ddcfb-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="ddcfb-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ddcfb-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="ddcfb-149">This property is read-only.</span></span> <span data-ttu-id="ddcfb-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ddcfb-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ddcfb-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ddcfb-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="ddcfb-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ddcfb-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="ddcfb-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="ddcfb-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="ddcfb-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ddcfb-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ddcfb-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ddcfb-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="ddcfb-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ddcfb-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="ddcfb-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="ddcfb-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="ddcfb-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ddcfb-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ddcfb-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ddcfb-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="ddcfb-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ddcfb-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="ddcfb-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="ddcfb-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="ddcfb-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ddcfb-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ddcfb-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ddcfb-163">createdDateTime</span></span>|<span data-ttu-id="ddcfb-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ddcfb-164">DateTimeOffset</span></span>|<span data-ttu-id="ddcfb-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="ddcfb-165">DateTime the object was created.</span></span> <span data-ttu-id="ddcfb-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ddcfb-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ddcfb-167">说明</span><span class="sxs-lookup"><span data-stu-id="ddcfb-167">description</span></span>|<span data-ttu-id="ddcfb-168">String</span><span class="sxs-lookup"><span data-stu-id="ddcfb-168">String</span></span>|<span data-ttu-id="ddcfb-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="ddcfb-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ddcfb-170">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ddcfb-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ddcfb-171">displayName</span><span class="sxs-lookup"><span data-stu-id="ddcfb-171">displayName</span></span>|<span data-ttu-id="ddcfb-172">String</span><span class="sxs-lookup"><span data-stu-id="ddcfb-172">String</span></span>|<span data-ttu-id="ddcfb-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="ddcfb-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ddcfb-174">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ddcfb-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ddcfb-175">version</span><span class="sxs-lookup"><span data-stu-id="ddcfb-175">version</span></span>|<span data-ttu-id="ddcfb-176">Int32</span><span class="sxs-lookup"><span data-stu-id="ddcfb-176">Int32</span></span>|<span data-ttu-id="ddcfb-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="ddcfb-177">Version of the device configuration.</span></span> <span data-ttu-id="ddcfb-178">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ddcfb-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ddcfb-179">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="ddcfb-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="ddcfb-180">Int32</span><span class="sxs-lookup"><span data-stu-id="ddcfb-180">Int32</span></span>|<span data-ttu-id="ddcfb-181">证书续订阈值百分比。</span><span class="sxs-lookup"><span data-stu-id="ddcfb-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="ddcfb-182">继承自[macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="ddcfb-182">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="ddcfb-183">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="ddcfb-183">subjectNameFormat</span></span>|[<span data-ttu-id="ddcfb-184">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="ddcfb-184">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="ddcfb-185">证书使用者名称格式。</span><span class="sxs-lookup"><span data-stu-id="ddcfb-185">Certificate Subject Name Format.</span></span> <span data-ttu-id="ddcfb-186">继承自[macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="ddcfb-186">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="ddcfb-187">可取值为：`commonName`、`commonNameAsEmail`、`custom`、`commonNameIncludingEmail`、`commonNameAsIMEI`、`commonNameAsSerialNumber`。</span><span class="sxs-lookup"><span data-stu-id="ddcfb-187">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="ddcfb-188">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="ddcfb-188">subjectAlternativeNameType</span></span>|[<span data-ttu-id="ddcfb-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="ddcfb-189">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="ddcfb-190">证书使用者备用名称类型。</span><span class="sxs-lookup"><span data-stu-id="ddcfb-190">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="ddcfb-191">继承自[macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="ddcfb-191">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="ddcfb-192">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService`。</span><span class="sxs-lookup"><span data-stu-id="ddcfb-192">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="ddcfb-193">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="ddcfb-193">certificateValidityPeriodValue</span></span>|<span data-ttu-id="ddcfb-194">Int32</span><span class="sxs-lookup"><span data-stu-id="ddcfb-194">Int32</span></span>|<span data-ttu-id="ddcfb-195">证书有效期限的值。</span><span class="sxs-lookup"><span data-stu-id="ddcfb-195">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="ddcfb-196">继承自[macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="ddcfb-196">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="ddcfb-197">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="ddcfb-197">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="ddcfb-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="ddcfb-198">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="ddcfb-199">证书有效期的小数位数。</span><span class="sxs-lookup"><span data-stu-id="ddcfb-199">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="ddcfb-200">继承自[macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="ddcfb-200">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="ddcfb-201">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="ddcfb-201">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="ddcfb-202">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="ddcfb-202">scepServerUrls</span></span>|<span data-ttu-id="ddcfb-203">String collection</span><span class="sxs-lookup"><span data-stu-id="ddcfb-203">String collection</span></span>|<span data-ttu-id="ddcfb-204">SCEP 服务器 Url。</span><span class="sxs-lookup"><span data-stu-id="ddcfb-204">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="ddcfb-205">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="ddcfb-205">subjectNameFormatString</span></span>|<span data-ttu-id="ddcfb-206">String</span><span class="sxs-lookup"><span data-stu-id="ddcfb-206">String</span></span>|<span data-ttu-id="ddcfb-207">要与 SubjectNameFormat = Custom 一起使用的自定义格式。</span><span class="sxs-lookup"><span data-stu-id="ddcfb-207">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="ddcfb-208">示例: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = 企业用户, O = Contoso Corporation, L = Redmond, ST = WA, C = US</span><span class="sxs-lookup"><span data-stu-id="ddcfb-208">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="ddcfb-209">keyUsage</span><span class="sxs-lookup"><span data-stu-id="ddcfb-209">keyUsage</span></span>|[<span data-ttu-id="ddcfb-210">keyUsages</span><span class="sxs-lookup"><span data-stu-id="ddcfb-210">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="ddcfb-211">SCEP 密钥用法。</span><span class="sxs-lookup"><span data-stu-id="ddcfb-211">SCEP Key Usage.</span></span> <span data-ttu-id="ddcfb-212">可取值为：`keyEncipherment`、`digitalSignature`。</span><span class="sxs-lookup"><span data-stu-id="ddcfb-212">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="ddcfb-213">keySize</span><span class="sxs-lookup"><span data-stu-id="ddcfb-213">keySize</span></span>|[<span data-ttu-id="ddcfb-214">keySize</span><span class="sxs-lookup"><span data-stu-id="ddcfb-214">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="ddcfb-215">SCEP 密钥大小。</span><span class="sxs-lookup"><span data-stu-id="ddcfb-215">SCEP Key Size.</span></span> <span data-ttu-id="ddcfb-216">可取值为：`size1024`、`size2048`。</span><span class="sxs-lookup"><span data-stu-id="ddcfb-216">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="ddcfb-217">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="ddcfb-217">hashAlgorithm</span></span>|[<span data-ttu-id="ddcfb-218">hashAlgorithms</span><span class="sxs-lookup"><span data-stu-id="ddcfb-218">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="ddcfb-219">SCEP 哈希算法。</span><span class="sxs-lookup"><span data-stu-id="ddcfb-219">SCEP Hash Algorithm.</span></span> <span data-ttu-id="ddcfb-220">可取值为：`sha1`、`sha2`。</span><span class="sxs-lookup"><span data-stu-id="ddcfb-220">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="ddcfb-221">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="ddcfb-221">extendedKeyUsages</span></span>|<span data-ttu-id="ddcfb-222">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)集合</span><span class="sxs-lookup"><span data-stu-id="ddcfb-222">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="ddcfb-223">扩展密钥用法 (EKU) 设置。</span><span class="sxs-lookup"><span data-stu-id="ddcfb-223">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="ddcfb-224">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="ddcfb-224">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="ddcfb-225">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="ddcfb-225">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="ddcfb-226">String</span><span class="sxs-lookup"><span data-stu-id="ddcfb-226">String</span></span>|<span data-ttu-id="ddcfb-227">定义 AAD 属性的自定义字符串。</span><span class="sxs-lookup"><span data-stu-id="ddcfb-227">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="ddcfb-228">certificateStore</span><span class="sxs-lookup"><span data-stu-id="ddcfb-228">certificateStore</span></span>|[<span data-ttu-id="ddcfb-229">certificateStore</span><span class="sxs-lookup"><span data-stu-id="ddcfb-229">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="ddcfb-230">目标存储证书。</span><span class="sxs-lookup"><span data-stu-id="ddcfb-230">Target store certificate.</span></span> <span data-ttu-id="ddcfb-231">可取值为：`user`、`machine`。</span><span class="sxs-lookup"><span data-stu-id="ddcfb-231">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="ddcfb-232">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="ddcfb-232">customSubjectAlternativeNames</span></span>|<span data-ttu-id="ddcfb-233">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)集合</span><span class="sxs-lookup"><span data-stu-id="ddcfb-233">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="ddcfb-234">自定义主题备用名称设置。</span><span class="sxs-lookup"><span data-stu-id="ddcfb-234">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="ddcfb-235">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="ddcfb-235">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="ddcfb-236">响应</span><span class="sxs-lookup"><span data-stu-id="ddcfb-236">Response</span></span>
<span data-ttu-id="ddcfb-237">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ddcfb-237">If successful, this method returns a `201 Created` response code and a [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ddcfb-238">示例</span><span class="sxs-lookup"><span data-stu-id="ddcfb-238">Example</span></span>

### <a name="request"></a><span data-ttu-id="ddcfb-239">请求</span><span class="sxs-lookup"><span data-stu-id="ddcfb-239">Request</span></span>
<span data-ttu-id="ddcfb-240">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ddcfb-240">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ddcfb-241">响应</span><span class="sxs-lookup"><span data-stu-id="ddcfb-241">Response</span></span>
<span data-ttu-id="ddcfb-p125">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ddcfb-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





