---
title: 更新 androidWorkProfileScepCertificateProfile
description: 更新 androidWorkProfileScepCertificateProfile 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5aa49fc03d9ce526d989f07139ede5ed458b172e
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33928314"
---
# <a name="update-androidworkprofilescepcertificateprofile"></a><span data-ttu-id="14472-103">更新 androidWorkProfileScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="14472-103">Update androidWorkProfileScepCertificateProfile</span></span>

> <span data-ttu-id="14472-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="14472-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="14472-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="14472-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="14472-106">更新[androidWorkProfileScepCertificateProfile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="14472-106">Update the properties of a [androidWorkProfileScepCertificateProfile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="14472-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="14472-107">Prerequisites</span></span>
<span data-ttu-id="14472-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="14472-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14472-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="14472-110">Permission type</span></span>|<span data-ttu-id="14472-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="14472-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="14472-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="14472-112">Delegated (work or school account)</span></span>|<span data-ttu-id="14472-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14472-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="14472-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="14472-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="14472-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="14472-115">Not supported.</span></span>|
|<span data-ttu-id="14472-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="14472-116">Application</span></span>|<span data-ttu-id="14472-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="14472-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="14472-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="14472-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="14472-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="14472-119">Request headers</span></span>
|<span data-ttu-id="14472-120">标头</span><span class="sxs-lookup"><span data-stu-id="14472-120">Header</span></span>|<span data-ttu-id="14472-121">值</span><span class="sxs-lookup"><span data-stu-id="14472-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="14472-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="14472-122">Authorization</span></span>|<span data-ttu-id="14472-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="14472-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="14472-124">接受</span><span class="sxs-lookup"><span data-stu-id="14472-124">Accept</span></span>|<span data-ttu-id="14472-125">application/json</span><span class="sxs-lookup"><span data-stu-id="14472-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="14472-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="14472-126">Request body</span></span>
<span data-ttu-id="14472-127">在请求正文中, 提供[androidWorkProfileScepCertificateProfile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="14472-127">In the request body, supply a JSON representation for the [androidWorkProfileScepCertificateProfile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md) object.</span></span>

<span data-ttu-id="14472-128">下表显示创建[androidWorkProfileScepCertificateProfile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="14472-128">The following table shows the properties that are required when you create the [androidWorkProfileScepCertificateProfile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md).</span></span>

|<span data-ttu-id="14472-129">属性</span><span class="sxs-lookup"><span data-stu-id="14472-129">Property</span></span>|<span data-ttu-id="14472-130">类型</span><span class="sxs-lookup"><span data-stu-id="14472-130">Type</span></span>|<span data-ttu-id="14472-131">说明</span><span class="sxs-lookup"><span data-stu-id="14472-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14472-132">id</span><span class="sxs-lookup"><span data-stu-id="14472-132">id</span></span>|<span data-ttu-id="14472-133">字符串</span><span class="sxs-lookup"><span data-stu-id="14472-133">String</span></span>|<span data-ttu-id="14472-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="14472-134">Key of the entity.</span></span> <span data-ttu-id="14472-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="14472-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="14472-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="14472-136">lastModifiedDateTime</span></span>|<span data-ttu-id="14472-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="14472-137">DateTimeOffset</span></span>|<span data-ttu-id="14472-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="14472-138">DateTime the object was last modified.</span></span> <span data-ttu-id="14472-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="14472-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="14472-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="14472-140">roleScopeTagIds</span></span>|<span data-ttu-id="14472-141">String collection</span><span class="sxs-lookup"><span data-stu-id="14472-141">String collection</span></span>|<span data-ttu-id="14472-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="14472-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="14472-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="14472-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="14472-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="14472-144">supportsScopeTags</span></span>|<span data-ttu-id="14472-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="14472-145">Boolean</span></span>|<span data-ttu-id="14472-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="14472-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="14472-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="14472-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="14472-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="14472-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="14472-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="14472-149">This property is read-only.</span></span> <span data-ttu-id="14472-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="14472-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="14472-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="14472-151">createdDateTime</span></span>|<span data-ttu-id="14472-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="14472-152">DateTimeOffset</span></span>|<span data-ttu-id="14472-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="14472-153">DateTime the object was created.</span></span> <span data-ttu-id="14472-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="14472-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="14472-155">说明</span><span class="sxs-lookup"><span data-stu-id="14472-155">description</span></span>|<span data-ttu-id="14472-156">String</span><span class="sxs-lookup"><span data-stu-id="14472-156">String</span></span>|<span data-ttu-id="14472-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="14472-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="14472-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="14472-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="14472-159">displayName</span><span class="sxs-lookup"><span data-stu-id="14472-159">displayName</span></span>|<span data-ttu-id="14472-160">String</span><span class="sxs-lookup"><span data-stu-id="14472-160">String</span></span>|<span data-ttu-id="14472-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="14472-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="14472-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="14472-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="14472-163">version</span><span class="sxs-lookup"><span data-stu-id="14472-163">version</span></span>|<span data-ttu-id="14472-164">Int32</span><span class="sxs-lookup"><span data-stu-id="14472-164">Int32</span></span>|<span data-ttu-id="14472-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="14472-165">Version of the device configuration.</span></span> <span data-ttu-id="14472-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="14472-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="14472-167">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="14472-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="14472-168">Int32</span><span class="sxs-lookup"><span data-stu-id="14472-168">Int32</span></span>|<span data-ttu-id="14472-169">证书续订阈值百分比。</span><span class="sxs-lookup"><span data-stu-id="14472-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="14472-170">从[AndroidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)继承的有效值1到99</span><span class="sxs-lookup"><span data-stu-id="14472-170">Valid values 1 to 99 Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="14472-171">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="14472-171">subjectNameFormat</span></span>|[<span data-ttu-id="14472-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="14472-172">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="14472-173">证书使用者名称格式。</span><span class="sxs-lookup"><span data-stu-id="14472-173">Certificate Subject Name Format.</span></span> <span data-ttu-id="14472-174">继承自[androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="14472-174">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="14472-175">可取值为：`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId`。</span><span class="sxs-lookup"><span data-stu-id="14472-175">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="14472-176">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="14472-176">certificateValidityPeriodValue</span></span>|<span data-ttu-id="14472-177">Int32</span><span class="sxs-lookup"><span data-stu-id="14472-177">Int32</span></span>|<span data-ttu-id="14472-178">证书有效期限的值。</span><span class="sxs-lookup"><span data-stu-id="14472-178">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="14472-179">继承自[androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="14472-179">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="14472-180">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="14472-180">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="14472-181">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="14472-181">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="14472-182">证书有效期的小数位数。</span><span class="sxs-lookup"><span data-stu-id="14472-182">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="14472-183">继承自[androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="14472-183">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="14472-184">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="14472-184">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="14472-185">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="14472-185">extendedKeyUsages</span></span>|<span data-ttu-id="14472-186">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)集合</span><span class="sxs-lookup"><span data-stu-id="14472-186">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="14472-187">扩展密钥用法 (EKU) 设置。</span><span class="sxs-lookup"><span data-stu-id="14472-187">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="14472-188">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="14472-188">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="14472-189">继承自[androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="14472-189">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="14472-190">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="14472-190">subjectAlternativeNameType</span></span>|[<span data-ttu-id="14472-191">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="14472-191">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="14472-192">证书使用者备用名称类型。</span><span class="sxs-lookup"><span data-stu-id="14472-192">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="14472-193">继承自[androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="14472-193">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="14472-194">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService`。</span><span class="sxs-lookup"><span data-stu-id="14472-194">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="14472-195">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="14472-195">scepServerUrls</span></span>|<span data-ttu-id="14472-196">String collection</span><span class="sxs-lookup"><span data-stu-id="14472-196">String collection</span></span>|<span data-ttu-id="14472-197">SCEP 服务器 Url</span><span class="sxs-lookup"><span data-stu-id="14472-197">SCEP Server Url(s)</span></span>|
|<span data-ttu-id="14472-198">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="14472-198">subjectNameFormatString</span></span>|<span data-ttu-id="14472-199">String</span><span class="sxs-lookup"><span data-stu-id="14472-199">String</span></span>|<span data-ttu-id="14472-200">要与 SubjectNameFormat = Custom 一起使用的自定义格式。</span><span class="sxs-lookup"><span data-stu-id="14472-200">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="14472-201">示例: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = 企业用户, O = Contoso Corporation, L = Redmond, ST = WA, C = US</span><span class="sxs-lookup"><span data-stu-id="14472-201">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="14472-202">keyUsage</span><span class="sxs-lookup"><span data-stu-id="14472-202">keyUsage</span></span>|[<span data-ttu-id="14472-203">keyUsages</span><span class="sxs-lookup"><span data-stu-id="14472-203">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="14472-204">SCEP 密钥用法。</span><span class="sxs-lookup"><span data-stu-id="14472-204">SCEP Key Usage.</span></span> <span data-ttu-id="14472-205">可取值为：`keyEncipherment`、`digitalSignature`。</span><span class="sxs-lookup"><span data-stu-id="14472-205">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="14472-206">keySize</span><span class="sxs-lookup"><span data-stu-id="14472-206">keySize</span></span>|[<span data-ttu-id="14472-207">keySize</span><span class="sxs-lookup"><span data-stu-id="14472-207">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="14472-208">SCEP 密钥大小。</span><span class="sxs-lookup"><span data-stu-id="14472-208">SCEP Key Size.</span></span> <span data-ttu-id="14472-209">可取值为：`size1024`、`size2048`。</span><span class="sxs-lookup"><span data-stu-id="14472-209">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="14472-210">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="14472-210">hashAlgorithm</span></span>|[<span data-ttu-id="14472-211">hashAlgorithms</span><span class="sxs-lookup"><span data-stu-id="14472-211">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="14472-212">SCEP 哈希算法。</span><span class="sxs-lookup"><span data-stu-id="14472-212">SCEP Hash Algorithm.</span></span> <span data-ttu-id="14472-213">可取值为：`sha1`、`sha2`。</span><span class="sxs-lookup"><span data-stu-id="14472-213">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="14472-214">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="14472-214">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="14472-215">String</span><span class="sxs-lookup"><span data-stu-id="14472-215">String</span></span>|<span data-ttu-id="14472-216">定义 AAD 属性的自定义字符串。</span><span class="sxs-lookup"><span data-stu-id="14472-216">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="14472-217">certificateStore</span><span class="sxs-lookup"><span data-stu-id="14472-217">certificateStore</span></span>|[<span data-ttu-id="14472-218">certificateStore</span><span class="sxs-lookup"><span data-stu-id="14472-218">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="14472-219">目标存储证书。</span><span class="sxs-lookup"><span data-stu-id="14472-219">Target store certificate.</span></span> <span data-ttu-id="14472-220">可取值为：`user`、`machine`。</span><span class="sxs-lookup"><span data-stu-id="14472-220">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="14472-221">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="14472-221">customSubjectAlternativeNames</span></span>|<span data-ttu-id="14472-222">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)集合</span><span class="sxs-lookup"><span data-stu-id="14472-222">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="14472-223">自定义主题备用名称设置。</span><span class="sxs-lookup"><span data-stu-id="14472-223">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="14472-224">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="14472-224">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="14472-225">响应</span><span class="sxs-lookup"><span data-stu-id="14472-225">Response</span></span>
<span data-ttu-id="14472-226">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[androidWorkProfileScepCertificateProfile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="14472-226">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileScepCertificateProfile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="14472-227">示例</span><span class="sxs-lookup"><span data-stu-id="14472-227">Example</span></span>

### <a name="request"></a><span data-ttu-id="14472-228">请求</span><span class="sxs-lookup"><span data-stu-id="14472-228">Request</span></span>
<span data-ttu-id="14472-229">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="14472-229">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1209

{
  "@odata.type": "#microsoft.graph.androidWorkProfileScepCertificateProfile",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "renewalThresholdPercentage": 10,
  "subjectNameFormat": "commonNameIncludingEmail",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "subjectAlternativeNameType": "emailAddress",
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
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

### <a name="response"></a><span data-ttu-id="14472-230">响应</span><span class="sxs-lookup"><span data-stu-id="14472-230">Response</span></span>
<span data-ttu-id="14472-p122">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="14472-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1381

{
  "@odata.type": "#microsoft.graph.androidWorkProfileScepCertificateProfile",
  "id": "6f494abf-4abf-6f49-bf4a-496fbf4a496f",
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
  "subjectNameFormat": "commonNameIncludingEmail",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "subjectAlternativeNameType": "emailAddress",
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
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




