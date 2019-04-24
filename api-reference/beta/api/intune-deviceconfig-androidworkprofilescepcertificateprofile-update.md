---
title: 更新 androidWorkProfileScepCertificateProfile
description: 更新 androidWorkProfileScepCertificateProfile 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: caf0b434a2ffb17dbe66fd48a59a4c5c715ef141
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32472986"
---
# <a name="update-androidworkprofilescepcertificateprofile"></a><span data-ttu-id="57f48-103">更新 androidWorkProfileScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="57f48-103">Update androidWorkProfileScepCertificateProfile</span></span>

> <span data-ttu-id="57f48-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="57f48-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="57f48-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="57f48-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="57f48-106">更新[androidWorkProfileScepCertificateProfile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="57f48-106">Update the properties of a [androidWorkProfileScepCertificateProfile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="57f48-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="57f48-107">Prerequisites</span></span>
<span data-ttu-id="57f48-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="57f48-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="57f48-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="57f48-110">Permission type</span></span>|<span data-ttu-id="57f48-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="57f48-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="57f48-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="57f48-112">Delegated (work or school account)</span></span>|<span data-ttu-id="57f48-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57f48-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="57f48-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="57f48-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="57f48-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="57f48-115">Not supported.</span></span>|
|<span data-ttu-id="57f48-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="57f48-116">Application</span></span>|<span data-ttu-id="57f48-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="57f48-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="57f48-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="57f48-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="57f48-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="57f48-119">Request headers</span></span>
|<span data-ttu-id="57f48-120">标头</span><span class="sxs-lookup"><span data-stu-id="57f48-120">Header</span></span>|<span data-ttu-id="57f48-121">值</span><span class="sxs-lookup"><span data-stu-id="57f48-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="57f48-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="57f48-122">Authorization</span></span>|<span data-ttu-id="57f48-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="57f48-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="57f48-124">接受</span><span class="sxs-lookup"><span data-stu-id="57f48-124">Accept</span></span>|<span data-ttu-id="57f48-125">application/json</span><span class="sxs-lookup"><span data-stu-id="57f48-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="57f48-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="57f48-126">Request body</span></span>
<span data-ttu-id="57f48-127">在请求正文中, 提供[androidWorkProfileScepCertificateProfile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="57f48-127">In the request body, supply a JSON representation for the [androidWorkProfileScepCertificateProfile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md) object.</span></span>

<span data-ttu-id="57f48-128">下表显示创建[androidWorkProfileScepCertificateProfile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="57f48-128">The following table shows the properties that are required when you create the [androidWorkProfileScepCertificateProfile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md).</span></span>

|<span data-ttu-id="57f48-129">属性</span><span class="sxs-lookup"><span data-stu-id="57f48-129">Property</span></span>|<span data-ttu-id="57f48-130">类型</span><span class="sxs-lookup"><span data-stu-id="57f48-130">Type</span></span>|<span data-ttu-id="57f48-131">说明</span><span class="sxs-lookup"><span data-stu-id="57f48-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57f48-132">id</span><span class="sxs-lookup"><span data-stu-id="57f48-132">id</span></span>|<span data-ttu-id="57f48-133">String</span><span class="sxs-lookup"><span data-stu-id="57f48-133">String</span></span>|<span data-ttu-id="57f48-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="57f48-134">Key of the entity.</span></span> <span data-ttu-id="57f48-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="57f48-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="57f48-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="57f48-136">lastModifiedDateTime</span></span>|<span data-ttu-id="57f48-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="57f48-137">DateTimeOffset</span></span>|<span data-ttu-id="57f48-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="57f48-138">DateTime the object was last modified.</span></span> <span data-ttu-id="57f48-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="57f48-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="57f48-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="57f48-140">roleScopeTagIds</span></span>|<span data-ttu-id="57f48-141">String collection</span><span class="sxs-lookup"><span data-stu-id="57f48-141">String collection</span></span>|<span data-ttu-id="57f48-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="57f48-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="57f48-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="57f48-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="57f48-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="57f48-144">supportsScopeTags</span></span>|<span data-ttu-id="57f48-145">布尔</span><span class="sxs-lookup"><span data-stu-id="57f48-145">Boolean</span></span>|<span data-ttu-id="57f48-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="57f48-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="57f48-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="57f48-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="57f48-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="57f48-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="57f48-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="57f48-149">This property is read-only.</span></span> <span data-ttu-id="57f48-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="57f48-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="57f48-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="57f48-151">createdDateTime</span></span>|<span data-ttu-id="57f48-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="57f48-152">DateTimeOffset</span></span>|<span data-ttu-id="57f48-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="57f48-153">DateTime the object was created.</span></span> <span data-ttu-id="57f48-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="57f48-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="57f48-155">description</span><span class="sxs-lookup"><span data-stu-id="57f48-155">description</span></span>|<span data-ttu-id="57f48-156">字符串</span><span class="sxs-lookup"><span data-stu-id="57f48-156">String</span></span>|<span data-ttu-id="57f48-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="57f48-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="57f48-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="57f48-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="57f48-159">displayName</span><span class="sxs-lookup"><span data-stu-id="57f48-159">displayName</span></span>|<span data-ttu-id="57f48-160">String</span><span class="sxs-lookup"><span data-stu-id="57f48-160">String</span></span>|<span data-ttu-id="57f48-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="57f48-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="57f48-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="57f48-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="57f48-163">version</span><span class="sxs-lookup"><span data-stu-id="57f48-163">version</span></span>|<span data-ttu-id="57f48-164">Int32</span><span class="sxs-lookup"><span data-stu-id="57f48-164">Int32</span></span>|<span data-ttu-id="57f48-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="57f48-165">Version of the device configuration.</span></span> <span data-ttu-id="57f48-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="57f48-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="57f48-167">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="57f48-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="57f48-168">Int32</span><span class="sxs-lookup"><span data-stu-id="57f48-168">Int32</span></span>|<span data-ttu-id="57f48-169">证书续订阈值百分比。</span><span class="sxs-lookup"><span data-stu-id="57f48-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="57f48-170">从[androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)继承的有效值1到99</span><span class="sxs-lookup"><span data-stu-id="57f48-170">Valid values 1 to 99 Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="57f48-171">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="57f48-171">subjectNameFormat</span></span>|[<span data-ttu-id="57f48-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="57f48-172">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="57f48-173">证书使用者名称格式。</span><span class="sxs-lookup"><span data-stu-id="57f48-173">Certificate Subject Name Format.</span></span> <span data-ttu-id="57f48-174">继承自[androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="57f48-174">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="57f48-175">可取值为：`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId`。</span><span class="sxs-lookup"><span data-stu-id="57f48-175">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="57f48-176">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="57f48-176">certificateValidityPeriodValue</span></span>|<span data-ttu-id="57f48-177">Int32</span><span class="sxs-lookup"><span data-stu-id="57f48-177">Int32</span></span>|<span data-ttu-id="57f48-178">证书有效期限的值。</span><span class="sxs-lookup"><span data-stu-id="57f48-178">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="57f48-179">继承自[androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="57f48-179">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="57f48-180">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="57f48-180">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="57f48-181">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="57f48-181">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="57f48-182">证书有效期的小数位数。</span><span class="sxs-lookup"><span data-stu-id="57f48-182">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="57f48-183">继承自[androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="57f48-183">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="57f48-184">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="57f48-184">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="57f48-185">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="57f48-185">extendedKeyUsages</span></span>|<span data-ttu-id="57f48-186">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)集合</span><span class="sxs-lookup"><span data-stu-id="57f48-186">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="57f48-187">扩展密钥用法 (EKU) 设置。</span><span class="sxs-lookup"><span data-stu-id="57f48-187">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="57f48-188">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="57f48-188">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="57f48-189">继承自[androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="57f48-189">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="57f48-190">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="57f48-190">subjectAlternativeNameType</span></span>|[<span data-ttu-id="57f48-191">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="57f48-191">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="57f48-192">证书使用者备用名称类型。</span><span class="sxs-lookup"><span data-stu-id="57f48-192">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="57f48-193">继承自[androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="57f48-193">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="57f48-194">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute` 或 `domainNameService`。</span><span class="sxs-lookup"><span data-stu-id="57f48-194">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="57f48-195">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="57f48-195">scepServerUrls</span></span>|<span data-ttu-id="57f48-196">String collection</span><span class="sxs-lookup"><span data-stu-id="57f48-196">String collection</span></span>|<span data-ttu-id="57f48-197">SCEP 服务器 Url</span><span class="sxs-lookup"><span data-stu-id="57f48-197">SCEP Server Url(s)</span></span>|
|<span data-ttu-id="57f48-198">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="57f48-198">subjectNameFormatString</span></span>|<span data-ttu-id="57f48-199">字符串</span><span class="sxs-lookup"><span data-stu-id="57f48-199">String</span></span>|<span data-ttu-id="57f48-200">要与 SubjectNameFormat = custom 一起使用的自定义格式。</span><span class="sxs-lookup"><span data-stu-id="57f48-200">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="57f48-201">示例: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = 企业用户, O = Contoso Corporation, L = Redmond, ST = WA, C = US</span><span class="sxs-lookup"><span data-stu-id="57f48-201">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="57f48-202">keyUsage</span><span class="sxs-lookup"><span data-stu-id="57f48-202">keyUsage</span></span>|[<span data-ttu-id="57f48-203">keyUsages</span><span class="sxs-lookup"><span data-stu-id="57f48-203">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="57f48-204">SCEP 密钥用法。</span><span class="sxs-lookup"><span data-stu-id="57f48-204">SCEP Key Usage.</span></span> <span data-ttu-id="57f48-205">可取值为：`keyEncipherment`、`digitalSignature`。</span><span class="sxs-lookup"><span data-stu-id="57f48-205">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="57f48-206">keySize</span><span class="sxs-lookup"><span data-stu-id="57f48-206">keySize</span></span>|[<span data-ttu-id="57f48-207">keySize</span><span class="sxs-lookup"><span data-stu-id="57f48-207">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="57f48-208">SCEP 密钥大小。</span><span class="sxs-lookup"><span data-stu-id="57f48-208">SCEP Key Size.</span></span> <span data-ttu-id="57f48-209">可取值为：`size1024`、`size2048`。</span><span class="sxs-lookup"><span data-stu-id="57f48-209">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="57f48-210">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="57f48-210">hashAlgorithm</span></span>|[<span data-ttu-id="57f48-211">hashAlgorithms</span><span class="sxs-lookup"><span data-stu-id="57f48-211">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="57f48-212">SCEP 哈希算法。</span><span class="sxs-lookup"><span data-stu-id="57f48-212">SCEP Hash Algorithm.</span></span> <span data-ttu-id="57f48-213">可取值为：`sha1`、`sha2`。</span><span class="sxs-lookup"><span data-stu-id="57f48-213">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="57f48-214">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="57f48-214">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="57f48-215">字符串</span><span class="sxs-lookup"><span data-stu-id="57f48-215">String</span></span>|<span data-ttu-id="57f48-216">定义 AAD 属性的自定义字符串。</span><span class="sxs-lookup"><span data-stu-id="57f48-216">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="57f48-217">certificateStore</span><span class="sxs-lookup"><span data-stu-id="57f48-217">certificateStore</span></span>|[<span data-ttu-id="57f48-218">certificateStore</span><span class="sxs-lookup"><span data-stu-id="57f48-218">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="57f48-219">目标存储证书。</span><span class="sxs-lookup"><span data-stu-id="57f48-219">Target store certificate.</span></span> <span data-ttu-id="57f48-220">可取值为：`user`、`machine`。</span><span class="sxs-lookup"><span data-stu-id="57f48-220">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="57f48-221">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="57f48-221">customSubjectAlternativeNames</span></span>|<span data-ttu-id="57f48-222">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)集合</span><span class="sxs-lookup"><span data-stu-id="57f48-222">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="57f48-223">自定义主题备用名称设置。</span><span class="sxs-lookup"><span data-stu-id="57f48-223">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="57f48-224">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="57f48-224">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="57f48-225">响应</span><span class="sxs-lookup"><span data-stu-id="57f48-225">Response</span></span>
<span data-ttu-id="57f48-226">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[androidWorkProfileScepCertificateProfile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="57f48-226">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileScepCertificateProfile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="57f48-227">示例</span><span class="sxs-lookup"><span data-stu-id="57f48-227">Example</span></span>

### <a name="request"></a><span data-ttu-id="57f48-228">请求</span><span class="sxs-lookup"><span data-stu-id="57f48-228">Request</span></span>
<span data-ttu-id="57f48-229">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="57f48-229">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="57f48-230">响应</span><span class="sxs-lookup"><span data-stu-id="57f48-230">Response</span></span>
<span data-ttu-id="57f48-p122">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="57f48-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





