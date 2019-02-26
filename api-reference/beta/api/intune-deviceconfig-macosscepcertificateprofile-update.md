---
title: 更新 macOSScepCertificateProfile
description: 更新 macOSScepCertificateProfile 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 29b34723f32476dcc8d52a02998f242ea8539da4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30160933"
---
# <a name="update-macosscepcertificateprofile"></a><span data-ttu-id="0b287-103">更新 macOSScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="0b287-103">Update macOSScepCertificateProfile</span></span>

> <span data-ttu-id="0b287-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0b287-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0b287-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0b287-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0b287-106">更新[macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0b287-106">Update the properties of a [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0b287-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="0b287-107">Prerequisites</span></span>
<span data-ttu-id="0b287-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="0b287-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0b287-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="0b287-110">Permission type</span></span>|<span data-ttu-id="0b287-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0b287-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0b287-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0b287-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0b287-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b287-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0b287-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0b287-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0b287-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0b287-115">Not supported.</span></span>|
|<span data-ttu-id="0b287-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="0b287-116">Application</span></span>|<span data-ttu-id="0b287-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="0b287-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0b287-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0b287-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="0b287-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="0b287-119">Request headers</span></span>
|<span data-ttu-id="0b287-120">标头</span><span class="sxs-lookup"><span data-stu-id="0b287-120">Header</span></span>|<span data-ttu-id="0b287-121">值</span><span class="sxs-lookup"><span data-stu-id="0b287-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0b287-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0b287-122">Authorization</span></span>|<span data-ttu-id="0b287-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0b287-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0b287-124">Accept</span><span class="sxs-lookup"><span data-stu-id="0b287-124">Accept</span></span>|<span data-ttu-id="0b287-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0b287-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b287-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="0b287-126">Request body</span></span>
<span data-ttu-id="0b287-127">在请求正文中, 提供[macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0b287-127">In the request body, supply a JSON representation for the [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) object.</span></span>

<span data-ttu-id="0b287-128">下表显示创建[macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="0b287-128">The following table shows the properties that are required when you create the [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md).</span></span>

|<span data-ttu-id="0b287-129">属性</span><span class="sxs-lookup"><span data-stu-id="0b287-129">Property</span></span>|<span data-ttu-id="0b287-130">类型</span><span class="sxs-lookup"><span data-stu-id="0b287-130">Type</span></span>|<span data-ttu-id="0b287-131">说明</span><span class="sxs-lookup"><span data-stu-id="0b287-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b287-132">id</span><span class="sxs-lookup"><span data-stu-id="0b287-132">id</span></span>|<span data-ttu-id="0b287-133">String</span><span class="sxs-lookup"><span data-stu-id="0b287-133">String</span></span>|<span data-ttu-id="0b287-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="0b287-134">Key of the entity.</span></span> <span data-ttu-id="0b287-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0b287-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0b287-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0b287-136">lastModifiedDateTime</span></span>|<span data-ttu-id="0b287-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0b287-137">DateTimeOffset</span></span>|<span data-ttu-id="0b287-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="0b287-138">DateTime the object was last modified.</span></span> <span data-ttu-id="0b287-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0b287-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0b287-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0b287-140">roleScopeTagIds</span></span>|<span data-ttu-id="0b287-141">String collection</span><span class="sxs-lookup"><span data-stu-id="0b287-141">String collection</span></span>|<span data-ttu-id="0b287-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="0b287-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0b287-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0b287-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0b287-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="0b287-144">supportsScopeTags</span></span>|<span data-ttu-id="0b287-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="0b287-145">Boolean</span></span>|<span data-ttu-id="0b287-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="0b287-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="0b287-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="0b287-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="0b287-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="0b287-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="0b287-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="0b287-149">This property is read-only.</span></span> <span data-ttu-id="0b287-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0b287-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0b287-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0b287-151">createdDateTime</span></span>|<span data-ttu-id="0b287-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0b287-152">DateTimeOffset</span></span>|<span data-ttu-id="0b287-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="0b287-153">DateTime the object was created.</span></span> <span data-ttu-id="0b287-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0b287-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0b287-155">description</span><span class="sxs-lookup"><span data-stu-id="0b287-155">description</span></span>|<span data-ttu-id="0b287-156">String</span><span class="sxs-lookup"><span data-stu-id="0b287-156">String</span></span>|<span data-ttu-id="0b287-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="0b287-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0b287-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0b287-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0b287-159">displayName</span><span class="sxs-lookup"><span data-stu-id="0b287-159">displayName</span></span>|<span data-ttu-id="0b287-160">String</span><span class="sxs-lookup"><span data-stu-id="0b287-160">String</span></span>|<span data-ttu-id="0b287-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="0b287-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0b287-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0b287-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0b287-163">version</span><span class="sxs-lookup"><span data-stu-id="0b287-163">version</span></span>|<span data-ttu-id="0b287-164">Int32</span><span class="sxs-lookup"><span data-stu-id="0b287-164">Int32</span></span>|<span data-ttu-id="0b287-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="0b287-165">Version of the device configuration.</span></span> <span data-ttu-id="0b287-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0b287-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0b287-167">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="0b287-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="0b287-168">Int32</span><span class="sxs-lookup"><span data-stu-id="0b287-168">Int32</span></span>|<span data-ttu-id="0b287-169">证书续订阈值百分比。</span><span class="sxs-lookup"><span data-stu-id="0b287-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="0b287-170">继承自[macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="0b287-170">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="0b287-171">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="0b287-171">subjectNameFormat</span></span>|[<span data-ttu-id="0b287-172">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="0b287-172">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="0b287-173">证书使用者名称格式。</span><span class="sxs-lookup"><span data-stu-id="0b287-173">Certificate Subject Name Format.</span></span> <span data-ttu-id="0b287-174">继承自[macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="0b287-174">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="0b287-175">可取值为：`commonName`、`commonNameAsEmail`、`custom`、`commonNameIncludingEmail`、`commonNameAsIMEI`、`commonNameAsSerialNumber`。</span><span class="sxs-lookup"><span data-stu-id="0b287-175">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="0b287-176">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="0b287-176">subjectAlternativeNameType</span></span>|[<span data-ttu-id="0b287-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="0b287-177">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="0b287-178">证书使用者备用名称类型。</span><span class="sxs-lookup"><span data-stu-id="0b287-178">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="0b287-179">继承自[macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="0b287-179">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="0b287-180">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService`。</span><span class="sxs-lookup"><span data-stu-id="0b287-180">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="0b287-181">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="0b287-181">certificateValidityPeriodValue</span></span>|<span data-ttu-id="0b287-182">Int32</span><span class="sxs-lookup"><span data-stu-id="0b287-182">Int32</span></span>|<span data-ttu-id="0b287-183">证书有效期限的值。</span><span class="sxs-lookup"><span data-stu-id="0b287-183">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="0b287-184">继承自[macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="0b287-184">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="0b287-185">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="0b287-185">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="0b287-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="0b287-186">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="0b287-187">证书有效期的小数位数。</span><span class="sxs-lookup"><span data-stu-id="0b287-187">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="0b287-188">继承自[macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="0b287-188">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="0b287-189">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="0b287-189">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="0b287-190">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="0b287-190">scepServerUrls</span></span>|<span data-ttu-id="0b287-191">String collection</span><span class="sxs-lookup"><span data-stu-id="0b287-191">String collection</span></span>|<span data-ttu-id="0b287-192">SCEP 服务器 Url。</span><span class="sxs-lookup"><span data-stu-id="0b287-192">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="0b287-193">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="0b287-193">subjectNameFormatString</span></span>|<span data-ttu-id="0b287-194">String</span><span class="sxs-lookup"><span data-stu-id="0b287-194">String</span></span>|<span data-ttu-id="0b287-195">要与 SubjectNameFormat = custom 一起使用的自定义格式。</span><span class="sxs-lookup"><span data-stu-id="0b287-195">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="0b287-196">示例: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = 企业用户, O = Contoso Corporation, L = Redmond, ST = WA, C = US</span><span class="sxs-lookup"><span data-stu-id="0b287-196">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="0b287-197">keyUsage</span><span class="sxs-lookup"><span data-stu-id="0b287-197">keyUsage</span></span>|[<span data-ttu-id="0b287-198">keyUsages</span><span class="sxs-lookup"><span data-stu-id="0b287-198">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="0b287-199">SCEP 密钥用法。</span><span class="sxs-lookup"><span data-stu-id="0b287-199">SCEP Key Usage.</span></span> <span data-ttu-id="0b287-200">可取值为：`keyEncipherment`、`digitalSignature`。</span><span class="sxs-lookup"><span data-stu-id="0b287-200">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="0b287-201">keySize</span><span class="sxs-lookup"><span data-stu-id="0b287-201">keySize</span></span>|[<span data-ttu-id="0b287-202">keySize</span><span class="sxs-lookup"><span data-stu-id="0b287-202">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="0b287-203">SCEP 密钥大小。</span><span class="sxs-lookup"><span data-stu-id="0b287-203">SCEP Key Size.</span></span> <span data-ttu-id="0b287-204">可取值为：`size1024`、`size2048`。</span><span class="sxs-lookup"><span data-stu-id="0b287-204">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="0b287-205">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="0b287-205">hashAlgorithm</span></span>|[<span data-ttu-id="0b287-206">hashAlgorithms</span><span class="sxs-lookup"><span data-stu-id="0b287-206">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="0b287-207">SCEP 哈希算法。</span><span class="sxs-lookup"><span data-stu-id="0b287-207">SCEP Hash Algorithm.</span></span> <span data-ttu-id="0b287-208">可取值为：`sha1`、`sha2`。</span><span class="sxs-lookup"><span data-stu-id="0b287-208">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="0b287-209">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="0b287-209">extendedKeyUsages</span></span>|<span data-ttu-id="0b287-210">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)集合</span><span class="sxs-lookup"><span data-stu-id="0b287-210">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="0b287-211">扩展密钥用法 (EKU) 设置。</span><span class="sxs-lookup"><span data-stu-id="0b287-211">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="0b287-212">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="0b287-212">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="0b287-213">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="0b287-213">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="0b287-214">String</span><span class="sxs-lookup"><span data-stu-id="0b287-214">String</span></span>|<span data-ttu-id="0b287-215">定义 AAD 属性的自定义字符串。</span><span class="sxs-lookup"><span data-stu-id="0b287-215">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="0b287-216">certificateStore</span><span class="sxs-lookup"><span data-stu-id="0b287-216">certificateStore</span></span>|[<span data-ttu-id="0b287-217">certificateStore</span><span class="sxs-lookup"><span data-stu-id="0b287-217">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="0b287-218">目标存储证书。</span><span class="sxs-lookup"><span data-stu-id="0b287-218">Target store certificate.</span></span> <span data-ttu-id="0b287-219">可取值为：`user`、`machine`。</span><span class="sxs-lookup"><span data-stu-id="0b287-219">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="0b287-220">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="0b287-220">customSubjectAlternativeNames</span></span>|<span data-ttu-id="0b287-221">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)集合</span><span class="sxs-lookup"><span data-stu-id="0b287-221">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="0b287-222">自定义主题备用名称设置。</span><span class="sxs-lookup"><span data-stu-id="0b287-222">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="0b287-223">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="0b287-223">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="0b287-224">响应</span><span class="sxs-lookup"><span data-stu-id="0b287-224">Response</span></span>
<span data-ttu-id="0b287-225">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0b287-225">If successful, this method returns a `200 OK` response code and an updated [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b287-226">示例</span><span class="sxs-lookup"><span data-stu-id="0b287-226">Example</span></span>

### <a name="request"></a><span data-ttu-id="0b287-227">请求</span><span class="sxs-lookup"><span data-stu-id="0b287-227">Request</span></span>
<span data-ttu-id="0b287-228">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0b287-228">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1189

{
  "@odata.type": "#microsoft.graph.macOSScepCertificateProfile",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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

### <a name="response"></a><span data-ttu-id="0b287-229">响应</span><span class="sxs-lookup"><span data-stu-id="0b287-229">Response</span></span>
<span data-ttu-id="0b287-p122">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0b287-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1361

{
  "@odata.type": "#microsoft.graph.macOSScepCertificateProfile",
  "id": "78c3929d-929d-78c3-9d92-c3789d92c378",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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




