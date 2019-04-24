---
title: 创建 androidWorkProfilePkcsCertificateProfile
description: 创建新的 androidWorkProfilePkcsCertificateProfile 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: db76928fc56900bea778ff85f6d3bc32a9f83595
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32474295"
---
# <a name="create-androidworkprofilepkcscertificateprofile"></a><span data-ttu-id="c9c85-103">创建 androidWorkProfilePkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="c9c85-103">Create androidWorkProfilePkcsCertificateProfile</span></span>

> <span data-ttu-id="c9c85-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c9c85-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c9c85-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c9c85-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c9c85-106">创建新的[androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c9c85-106">Create a new [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c9c85-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="c9c85-107">Prerequisites</span></span>
<span data-ttu-id="c9c85-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c9c85-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9c85-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c9c85-110">Permission type</span></span>|<span data-ttu-id="c9c85-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c9c85-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c9c85-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c9c85-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c9c85-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9c85-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c9c85-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c9c85-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c9c85-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c9c85-115">Not supported.</span></span>|
|<span data-ttu-id="c9c85-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c9c85-116">Application</span></span>|<span data-ttu-id="c9c85-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="c9c85-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c9c85-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c9c85-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c9c85-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c9c85-119">Request headers</span></span>
|<span data-ttu-id="c9c85-120">标头</span><span class="sxs-lookup"><span data-stu-id="c9c85-120">Header</span></span>|<span data-ttu-id="c9c85-121">值</span><span class="sxs-lookup"><span data-stu-id="c9c85-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c9c85-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c9c85-122">Authorization</span></span>|<span data-ttu-id="c9c85-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c9c85-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c9c85-124">接受</span><span class="sxs-lookup"><span data-stu-id="c9c85-124">Accept</span></span>|<span data-ttu-id="c9c85-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c9c85-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c9c85-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c9c85-126">Request body</span></span>
<span data-ttu-id="c9c85-127">在请求正文中, 提供 androidWorkProfilePkcsCertificateProfile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c9c85-127">In the request body, supply a JSON representation for the androidWorkProfilePkcsCertificateProfile object.</span></span>

<span data-ttu-id="c9c85-128">下表显示创建 androidWorkProfilePkcsCertificateProfile 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c9c85-128">The following table shows the properties that are required when you create the androidWorkProfilePkcsCertificateProfile.</span></span>

|<span data-ttu-id="c9c85-129">属性</span><span class="sxs-lookup"><span data-stu-id="c9c85-129">Property</span></span>|<span data-ttu-id="c9c85-130">类型</span><span class="sxs-lookup"><span data-stu-id="c9c85-130">Type</span></span>|<span data-ttu-id="c9c85-131">说明</span><span class="sxs-lookup"><span data-stu-id="c9c85-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9c85-132">id</span><span class="sxs-lookup"><span data-stu-id="c9c85-132">id</span></span>|<span data-ttu-id="c9c85-133">String</span><span class="sxs-lookup"><span data-stu-id="c9c85-133">String</span></span>|<span data-ttu-id="c9c85-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c9c85-134">Key of the entity.</span></span> <span data-ttu-id="c9c85-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c9c85-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9c85-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c9c85-136">lastModifiedDateTime</span></span>|<span data-ttu-id="c9c85-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9c85-137">DateTimeOffset</span></span>|<span data-ttu-id="c9c85-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c9c85-138">DateTime the object was last modified.</span></span> <span data-ttu-id="c9c85-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c9c85-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9c85-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c9c85-140">roleScopeTagIds</span></span>|<span data-ttu-id="c9c85-141">String collection</span><span class="sxs-lookup"><span data-stu-id="c9c85-141">String collection</span></span>|<span data-ttu-id="c9c85-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="c9c85-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c9c85-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c9c85-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9c85-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c9c85-144">supportsScopeTags</span></span>|<span data-ttu-id="c9c85-145">布尔</span><span class="sxs-lookup"><span data-stu-id="c9c85-145">Boolean</span></span>|<span data-ttu-id="c9c85-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="c9c85-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c9c85-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="c9c85-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c9c85-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="c9c85-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c9c85-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c9c85-149">This property is read-only.</span></span> <span data-ttu-id="c9c85-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c9c85-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9c85-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c9c85-151">createdDateTime</span></span>|<span data-ttu-id="c9c85-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9c85-152">DateTimeOffset</span></span>|<span data-ttu-id="c9c85-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c9c85-153">DateTime the object was created.</span></span> <span data-ttu-id="c9c85-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c9c85-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9c85-155">description</span><span class="sxs-lookup"><span data-stu-id="c9c85-155">description</span></span>|<span data-ttu-id="c9c85-156">字符串</span><span class="sxs-lookup"><span data-stu-id="c9c85-156">String</span></span>|<span data-ttu-id="c9c85-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="c9c85-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c9c85-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c9c85-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9c85-159">displayName</span><span class="sxs-lookup"><span data-stu-id="c9c85-159">displayName</span></span>|<span data-ttu-id="c9c85-160">String</span><span class="sxs-lookup"><span data-stu-id="c9c85-160">String</span></span>|<span data-ttu-id="c9c85-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="c9c85-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c9c85-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c9c85-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9c85-163">version</span><span class="sxs-lookup"><span data-stu-id="c9c85-163">version</span></span>|<span data-ttu-id="c9c85-164">Int32</span><span class="sxs-lookup"><span data-stu-id="c9c85-164">Int32</span></span>|<span data-ttu-id="c9c85-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="c9c85-165">Version of the device configuration.</span></span> <span data-ttu-id="c9c85-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c9c85-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9c85-167">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="c9c85-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="c9c85-168">Int32</span><span class="sxs-lookup"><span data-stu-id="c9c85-168">Int32</span></span>|<span data-ttu-id="c9c85-169">证书续订阈值百分比。</span><span class="sxs-lookup"><span data-stu-id="c9c85-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="c9c85-170">从[androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)继承的有效值1到99</span><span class="sxs-lookup"><span data-stu-id="c9c85-170">Valid values 1 to 99 Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="c9c85-171">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="c9c85-171">subjectNameFormat</span></span>|[<span data-ttu-id="c9c85-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="c9c85-172">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="c9c85-173">证书使用者名称格式。</span><span class="sxs-lookup"><span data-stu-id="c9c85-173">Certificate Subject Name Format.</span></span> <span data-ttu-id="c9c85-174">继承自[androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="c9c85-174">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="c9c85-175">可取值为：`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId`。</span><span class="sxs-lookup"><span data-stu-id="c9c85-175">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="c9c85-176">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="c9c85-176">certificateValidityPeriodValue</span></span>|<span data-ttu-id="c9c85-177">Int32</span><span class="sxs-lookup"><span data-stu-id="c9c85-177">Int32</span></span>|<span data-ttu-id="c9c85-178">证书有效期限的值。</span><span class="sxs-lookup"><span data-stu-id="c9c85-178">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="c9c85-179">继承自[androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="c9c85-179">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="c9c85-180">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="c9c85-180">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="c9c85-181">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="c9c85-181">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="c9c85-182">证书有效期的小数位数。</span><span class="sxs-lookup"><span data-stu-id="c9c85-182">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="c9c85-183">继承自[androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="c9c85-183">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="c9c85-184">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="c9c85-184">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="c9c85-185">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="c9c85-185">extendedKeyUsages</span></span>|<span data-ttu-id="c9c85-186">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)集合</span><span class="sxs-lookup"><span data-stu-id="c9c85-186">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="c9c85-187">扩展密钥用法 (EKU) 设置。</span><span class="sxs-lookup"><span data-stu-id="c9c85-187">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="c9c85-188">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="c9c85-188">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="c9c85-189">继承自[androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="c9c85-189">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="c9c85-190">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="c9c85-190">subjectAlternativeNameType</span></span>|[<span data-ttu-id="c9c85-191">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="c9c85-191">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="c9c85-192">证书使用者备用名称类型。</span><span class="sxs-lookup"><span data-stu-id="c9c85-192">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="c9c85-193">继承自[androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="c9c85-193">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="c9c85-194">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute` 或 `domainNameService`。</span><span class="sxs-lookup"><span data-stu-id="c9c85-194">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="c9c85-195">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="c9c85-195">certificationAuthority</span></span>|<span data-ttu-id="c9c85-196">字符串</span><span class="sxs-lookup"><span data-stu-id="c9c85-196">String</span></span>|<span data-ttu-id="c9c85-197">PKCS 证书颁发机构</span><span class="sxs-lookup"><span data-stu-id="c9c85-197">PKCS Certification Authority</span></span>|
|<span data-ttu-id="c9c85-198">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="c9c85-198">certificationAuthorityName</span></span>|<span data-ttu-id="c9c85-199">字符串</span><span class="sxs-lookup"><span data-stu-id="c9c85-199">String</span></span>|<span data-ttu-id="c9c85-200">PKCS 证书颁发机构名称</span><span class="sxs-lookup"><span data-stu-id="c9c85-200">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="c9c85-201">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="c9c85-201">certificateTemplateName</span></span>|<span data-ttu-id="c9c85-202">字符串</span><span class="sxs-lookup"><span data-stu-id="c9c85-202">String</span></span>|<span data-ttu-id="c9c85-203">PKCS 证书模板名称</span><span class="sxs-lookup"><span data-stu-id="c9c85-203">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="c9c85-204">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="c9c85-204">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="c9c85-205">字符串</span><span class="sxs-lookup"><span data-stu-id="c9c85-205">String</span></span>|<span data-ttu-id="c9c85-206">定义 AAD 属性的自定义字符串。</span><span class="sxs-lookup"><span data-stu-id="c9c85-206">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="c9c85-207">响应</span><span class="sxs-lookup"><span data-stu-id="c9c85-207">Response</span></span>
<span data-ttu-id="c9c85-208">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c9c85-208">If successful, this method returns a `201 Created` response code and a [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9c85-209">示例</span><span class="sxs-lookup"><span data-stu-id="c9c85-209">Example</span></span>

### <a name="request"></a><span data-ttu-id="c9c85-210">请求</span><span class="sxs-lookup"><span data-stu-id="c9c85-210">Request</span></span>
<span data-ttu-id="c9c85-211">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c9c85-211">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 969

{
  "@odata.type": "#microsoft.graph.androidWorkProfilePkcsCertificateProfile",
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
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```

### <a name="response"></a><span data-ttu-id="c9c85-212">响应</span><span class="sxs-lookup"><span data-stu-id="c9c85-212">Response</span></span>
<span data-ttu-id="c9c85-p116">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c9c85-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1141

{
  "@odata.type": "#microsoft.graph.androidWorkProfilePkcsCertificateProfile",
  "id": "a7d4a505-a505-a7d4-05a5-d4a705a5d4a7",
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
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```





