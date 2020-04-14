---
title: 更新 macOSScepCertificateProfile
description: 更新 macOSScepCertificateProfile 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f3979c0674d87de4052b0bfadaa33cf5a42dd2e9
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43432364"
---
# <a name="update-macosscepcertificateprofile"></a><span data-ttu-id="b255d-103">更新 macOSScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="b255d-103">Update macOSScepCertificateProfile</span></span>

<span data-ttu-id="b255d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b255d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b255d-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b255d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b255d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b255d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b255d-107">更新[macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b255d-107">Update the properties of a [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b255d-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b255d-108">Prerequisites</span></span>
<span data-ttu-id="b255d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b255d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b255d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b255d-111">Permission type</span></span>|<span data-ttu-id="b255d-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b255d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b255d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b255d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b255d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b255d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b255d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b255d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b255d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b255d-116">Not supported.</span></span>|
|<span data-ttu-id="b255d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b255d-117">Application</span></span>|<span data-ttu-id="b255d-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b255d-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b255d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b255d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="b255d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b255d-120">Request headers</span></span>
|<span data-ttu-id="b255d-121">标头</span><span class="sxs-lookup"><span data-stu-id="b255d-121">Header</span></span>|<span data-ttu-id="b255d-122">值</span><span class="sxs-lookup"><span data-stu-id="b255d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b255d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b255d-123">Authorization</span></span>|<span data-ttu-id="b255d-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b255d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b255d-125">接受</span><span class="sxs-lookup"><span data-stu-id="b255d-125">Accept</span></span>|<span data-ttu-id="b255d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b255d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b255d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b255d-127">Request body</span></span>
<span data-ttu-id="b255d-128">在请求正文中，提供[macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b255d-128">In the request body, supply a JSON representation for the [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) object.</span></span>

<span data-ttu-id="b255d-129">下表显示创建[macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b255d-129">The following table shows the properties that are required when you create the [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md).</span></span>

|<span data-ttu-id="b255d-130">属性</span><span class="sxs-lookup"><span data-stu-id="b255d-130">Property</span></span>|<span data-ttu-id="b255d-131">类型</span><span class="sxs-lookup"><span data-stu-id="b255d-131">Type</span></span>|<span data-ttu-id="b255d-132">说明</span><span class="sxs-lookup"><span data-stu-id="b255d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b255d-133">id</span><span class="sxs-lookup"><span data-stu-id="b255d-133">id</span></span>|<span data-ttu-id="b255d-134">字符串</span><span class="sxs-lookup"><span data-stu-id="b255d-134">String</span></span>|<span data-ttu-id="b255d-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b255d-135">Key of the entity.</span></span> <span data-ttu-id="b255d-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b255d-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b255d-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b255d-137">lastModifiedDateTime</span></span>|<span data-ttu-id="b255d-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b255d-138">DateTimeOffset</span></span>|<span data-ttu-id="b255d-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b255d-139">DateTime the object was last modified.</span></span> <span data-ttu-id="b255d-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b255d-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b255d-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b255d-141">roleScopeTagIds</span></span>|<span data-ttu-id="b255d-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="b255d-142">String collection</span></span>|<span data-ttu-id="b255d-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="b255d-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b255d-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b255d-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b255d-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b255d-145">supportsScopeTags</span></span>|<span data-ttu-id="b255d-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="b255d-146">Boolean</span></span>|<span data-ttu-id="b255d-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="b255d-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b255d-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="b255d-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b255d-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="b255d-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b255d-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="b255d-150">This property is read-only.</span></span> <span data-ttu-id="b255d-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b255d-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b255d-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b255d-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="b255d-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b255d-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="b255d-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="b255d-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="b255d-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b255d-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b255d-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b255d-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="b255d-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b255d-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="b255d-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="b255d-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="b255d-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b255d-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b255d-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b255d-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="b255d-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b255d-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="b255d-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="b255d-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="b255d-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b255d-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b255d-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b255d-164">createdDateTime</span></span>|<span data-ttu-id="b255d-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b255d-165">DateTimeOffset</span></span>|<span data-ttu-id="b255d-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b255d-166">DateTime the object was created.</span></span> <span data-ttu-id="b255d-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b255d-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b255d-168">description</span><span class="sxs-lookup"><span data-stu-id="b255d-168">description</span></span>|<span data-ttu-id="b255d-169">String</span><span class="sxs-lookup"><span data-stu-id="b255d-169">String</span></span>|<span data-ttu-id="b255d-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="b255d-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b255d-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b255d-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b255d-172">displayName</span><span class="sxs-lookup"><span data-stu-id="b255d-172">displayName</span></span>|<span data-ttu-id="b255d-173">String</span><span class="sxs-lookup"><span data-stu-id="b255d-173">String</span></span>|<span data-ttu-id="b255d-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="b255d-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b255d-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b255d-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b255d-176">version</span><span class="sxs-lookup"><span data-stu-id="b255d-176">version</span></span>|<span data-ttu-id="b255d-177">Int32</span><span class="sxs-lookup"><span data-stu-id="b255d-177">Int32</span></span>|<span data-ttu-id="b255d-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="b255d-178">Version of the device configuration.</span></span> <span data-ttu-id="b255d-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b255d-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b255d-180">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="b255d-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="b255d-181">Int32</span><span class="sxs-lookup"><span data-stu-id="b255d-181">Int32</span></span>|<span data-ttu-id="b255d-182">证书续订阈值百分比。</span><span class="sxs-lookup"><span data-stu-id="b255d-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="b255d-183">继承自[macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="b255d-183">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="b255d-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="b255d-184">subjectNameFormat</span></span>|[<span data-ttu-id="b255d-185">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="b255d-185">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="b255d-186">证书使用者名称格式。</span><span class="sxs-lookup"><span data-stu-id="b255d-186">Certificate Subject Name Format.</span></span> <span data-ttu-id="b255d-187">继承自[macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="b255d-187">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="b255d-188">可取值为：`commonName`、`commonNameAsEmail`、`custom`、`commonNameIncludingEmail`、`commonNameAsIMEI`、`commonNameAsSerialNumber`。</span><span class="sxs-lookup"><span data-stu-id="b255d-188">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="b255d-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="b255d-189">subjectAlternativeNameType</span></span>|[<span data-ttu-id="b255d-190">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="b255d-190">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="b255d-191">证书使用者备用名称类型。</span><span class="sxs-lookup"><span data-stu-id="b255d-191">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="b255d-192">继承自[macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="b255d-192">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="b255d-193">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService`。</span><span class="sxs-lookup"><span data-stu-id="b255d-193">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="b255d-194">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="b255d-194">certificateValidityPeriodValue</span></span>|<span data-ttu-id="b255d-195">Int32</span><span class="sxs-lookup"><span data-stu-id="b255d-195">Int32</span></span>|<span data-ttu-id="b255d-196">证书有效期限的值。</span><span class="sxs-lookup"><span data-stu-id="b255d-196">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="b255d-197">继承自[macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="b255d-197">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="b255d-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="b255d-198">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="b255d-199">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="b255d-199">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="b255d-200">证书有效期的小数位数。</span><span class="sxs-lookup"><span data-stu-id="b255d-200">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="b255d-201">继承自[macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="b255d-201">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="b255d-202">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="b255d-202">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="b255d-203">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="b255d-203">scepServerUrls</span></span>|<span data-ttu-id="b255d-204">String 集合</span><span class="sxs-lookup"><span data-stu-id="b255d-204">String collection</span></span>|<span data-ttu-id="b255d-205">SCEP 服务器 Url。</span><span class="sxs-lookup"><span data-stu-id="b255d-205">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="b255d-206">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="b255d-206">subjectNameFormatString</span></span>|<span data-ttu-id="b255d-207">String</span><span class="sxs-lookup"><span data-stu-id="b255d-207">String</span></span>|<span data-ttu-id="b255d-208">要与 SubjectNameFormat = Custom 一起使用的自定义格式。</span><span class="sxs-lookup"><span data-stu-id="b255d-208">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="b255d-209">示例： CN = {{EmailAddress}}，E = {{EmailAddress}}，OU = 企业用户，O = Contoso Corporation，L = Redmond，ST = WA，C = US</span><span class="sxs-lookup"><span data-stu-id="b255d-209">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="b255d-210">keyUsage</span><span class="sxs-lookup"><span data-stu-id="b255d-210">keyUsage</span></span>|[<span data-ttu-id="b255d-211">keyUsages</span><span class="sxs-lookup"><span data-stu-id="b255d-211">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="b255d-212">SCEP 密钥用法。</span><span class="sxs-lookup"><span data-stu-id="b255d-212">SCEP Key Usage.</span></span> <span data-ttu-id="b255d-213">可取值为：`keyEncipherment`、`digitalSignature`。</span><span class="sxs-lookup"><span data-stu-id="b255d-213">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="b255d-214">keySize</span><span class="sxs-lookup"><span data-stu-id="b255d-214">keySize</span></span>|[<span data-ttu-id="b255d-215">keySize</span><span class="sxs-lookup"><span data-stu-id="b255d-215">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="b255d-216">SCEP 密钥大小。</span><span class="sxs-lookup"><span data-stu-id="b255d-216">SCEP Key Size.</span></span> <span data-ttu-id="b255d-217">可取值为：`size1024`、`size2048`。</span><span class="sxs-lookup"><span data-stu-id="b255d-217">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="b255d-218">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="b255d-218">hashAlgorithm</span></span>|[<span data-ttu-id="b255d-219">hashAlgorithms</span><span class="sxs-lookup"><span data-stu-id="b255d-219">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="b255d-220">SCEP 哈希算法。</span><span class="sxs-lookup"><span data-stu-id="b255d-220">SCEP Hash Algorithm.</span></span> <span data-ttu-id="b255d-221">可取值为：`sha1`、`sha2`。</span><span class="sxs-lookup"><span data-stu-id="b255d-221">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="b255d-222">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="b255d-222">extendedKeyUsages</span></span>|<span data-ttu-id="b255d-223">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)集合</span><span class="sxs-lookup"><span data-stu-id="b255d-223">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="b255d-224">扩展密钥用法（EKU）设置。</span><span class="sxs-lookup"><span data-stu-id="b255d-224">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="b255d-225">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="b255d-225">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="b255d-226">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="b255d-226">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="b255d-227">String</span><span class="sxs-lookup"><span data-stu-id="b255d-227">String</span></span>|<span data-ttu-id="b255d-228">定义 AAD 属性的自定义字符串。</span><span class="sxs-lookup"><span data-stu-id="b255d-228">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="b255d-229">certificateStore</span><span class="sxs-lookup"><span data-stu-id="b255d-229">certificateStore</span></span>|[<span data-ttu-id="b255d-230">certificateStore</span><span class="sxs-lookup"><span data-stu-id="b255d-230">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="b255d-231">目标存储证书。</span><span class="sxs-lookup"><span data-stu-id="b255d-231">Target store certificate.</span></span> <span data-ttu-id="b255d-232">可取值为：`user`、`machine`。</span><span class="sxs-lookup"><span data-stu-id="b255d-232">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="b255d-233">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="b255d-233">customSubjectAlternativeNames</span></span>|<span data-ttu-id="b255d-234">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)集合</span><span class="sxs-lookup"><span data-stu-id="b255d-234">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="b255d-235">自定义主题备用名称设置。</span><span class="sxs-lookup"><span data-stu-id="b255d-235">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="b255d-236">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="b255d-236">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="b255d-237">响应</span><span class="sxs-lookup"><span data-stu-id="b255d-237">Response</span></span>
<span data-ttu-id="b255d-238">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b255d-238">If successful, this method returns a `200 OK` response code and an updated [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b255d-239">示例</span><span class="sxs-lookup"><span data-stu-id="b255d-239">Example</span></span>

### <a name="request"></a><span data-ttu-id="b255d-240">请求</span><span class="sxs-lookup"><span data-stu-id="b255d-240">Request</span></span>
<span data-ttu-id="b255d-241">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b255d-241">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b255d-242">响应</span><span class="sxs-lookup"><span data-stu-id="b255d-242">Response</span></span>
<span data-ttu-id="b255d-p125">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b255d-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



