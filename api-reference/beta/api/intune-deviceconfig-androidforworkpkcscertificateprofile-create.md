---
title: 创建 androidForWorkPkcsCertificateProfile
description: 创建新的 androidForWorkPkcsCertificateProfile 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: acab0a328ad14d9fe17d5e568047edacaded0462
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32478376"
---
# <a name="create-androidforworkpkcscertificateprofile"></a><span data-ttu-id="0b5b6-103">创建 androidForWorkPkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="0b5b6-103">Create androidForWorkPkcsCertificateProfile</span></span>

> <span data-ttu-id="0b5b6-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0b5b6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0b5b6-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0b5b6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0b5b6-106">创建新的[androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0b5b6-106">Create a new [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0b5b6-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="0b5b6-107">Prerequisites</span></span>
<span data-ttu-id="0b5b6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0b5b6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b5b6-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="0b5b6-110">Permission type</span></span>|<span data-ttu-id="0b5b6-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0b5b6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0b5b6-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0b5b6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0b5b6-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b5b6-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0b5b6-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0b5b6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0b5b6-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0b5b6-115">Not supported.</span></span>|
|<span data-ttu-id="0b5b6-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="0b5b6-116">Application</span></span>|<span data-ttu-id="0b5b6-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="0b5b6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0b5b6-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0b5b6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="0b5b6-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="0b5b6-119">Request headers</span></span>
|<span data-ttu-id="0b5b6-120">标头</span><span class="sxs-lookup"><span data-stu-id="0b5b6-120">Header</span></span>|<span data-ttu-id="0b5b6-121">值</span><span class="sxs-lookup"><span data-stu-id="0b5b6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0b5b6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0b5b6-122">Authorization</span></span>|<span data-ttu-id="0b5b6-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0b5b6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0b5b6-124">接受</span><span class="sxs-lookup"><span data-stu-id="0b5b6-124">Accept</span></span>|<span data-ttu-id="0b5b6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0b5b6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b5b6-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="0b5b6-126">Request body</span></span>
<span data-ttu-id="0b5b6-127">在请求正文中, 提供 androidForWorkPkcsCertificateProfile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0b5b6-127">In the request body, supply a JSON representation for the androidForWorkPkcsCertificateProfile object.</span></span>

<span data-ttu-id="0b5b6-128">下表显示创建 androidForWorkPkcsCertificateProfile 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="0b5b6-128">The following table shows the properties that are required when you create the androidForWorkPkcsCertificateProfile.</span></span>

|<span data-ttu-id="0b5b6-129">属性</span><span class="sxs-lookup"><span data-stu-id="0b5b6-129">Property</span></span>|<span data-ttu-id="0b5b6-130">类型</span><span class="sxs-lookup"><span data-stu-id="0b5b6-130">Type</span></span>|<span data-ttu-id="0b5b6-131">说明</span><span class="sxs-lookup"><span data-stu-id="0b5b6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b5b6-132">id</span><span class="sxs-lookup"><span data-stu-id="0b5b6-132">id</span></span>|<span data-ttu-id="0b5b6-133">String</span><span class="sxs-lookup"><span data-stu-id="0b5b6-133">String</span></span>|<span data-ttu-id="0b5b6-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="0b5b6-134">Key of the entity.</span></span> <span data-ttu-id="0b5b6-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0b5b6-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0b5b6-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0b5b6-136">lastModifiedDateTime</span></span>|<span data-ttu-id="0b5b6-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0b5b6-137">DateTimeOffset</span></span>|<span data-ttu-id="0b5b6-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="0b5b6-138">DateTime the object was last modified.</span></span> <span data-ttu-id="0b5b6-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0b5b6-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0b5b6-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0b5b6-140">roleScopeTagIds</span></span>|<span data-ttu-id="0b5b6-141">String collection</span><span class="sxs-lookup"><span data-stu-id="0b5b6-141">String collection</span></span>|<span data-ttu-id="0b5b6-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="0b5b6-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0b5b6-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0b5b6-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0b5b6-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="0b5b6-144">supportsScopeTags</span></span>|<span data-ttu-id="0b5b6-145">布尔</span><span class="sxs-lookup"><span data-stu-id="0b5b6-145">Boolean</span></span>|<span data-ttu-id="0b5b6-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="0b5b6-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="0b5b6-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="0b5b6-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="0b5b6-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="0b5b6-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="0b5b6-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="0b5b6-149">This property is read-only.</span></span> <span data-ttu-id="0b5b6-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0b5b6-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0b5b6-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0b5b6-151">createdDateTime</span></span>|<span data-ttu-id="0b5b6-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0b5b6-152">DateTimeOffset</span></span>|<span data-ttu-id="0b5b6-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="0b5b6-153">DateTime the object was created.</span></span> <span data-ttu-id="0b5b6-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0b5b6-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0b5b6-155">description</span><span class="sxs-lookup"><span data-stu-id="0b5b6-155">description</span></span>|<span data-ttu-id="0b5b6-156">字符串</span><span class="sxs-lookup"><span data-stu-id="0b5b6-156">String</span></span>|<span data-ttu-id="0b5b6-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="0b5b6-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0b5b6-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0b5b6-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0b5b6-159">displayName</span><span class="sxs-lookup"><span data-stu-id="0b5b6-159">displayName</span></span>|<span data-ttu-id="0b5b6-160">String</span><span class="sxs-lookup"><span data-stu-id="0b5b6-160">String</span></span>|<span data-ttu-id="0b5b6-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="0b5b6-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0b5b6-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0b5b6-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0b5b6-163">version</span><span class="sxs-lookup"><span data-stu-id="0b5b6-163">version</span></span>|<span data-ttu-id="0b5b6-164">Int32</span><span class="sxs-lookup"><span data-stu-id="0b5b6-164">Int32</span></span>|<span data-ttu-id="0b5b6-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="0b5b6-165">Version of the device configuration.</span></span> <span data-ttu-id="0b5b6-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0b5b6-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0b5b6-167">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="0b5b6-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="0b5b6-168">Int32</span><span class="sxs-lookup"><span data-stu-id="0b5b6-168">Int32</span></span>|<span data-ttu-id="0b5b6-169">证书续订阈值百分比。</span><span class="sxs-lookup"><span data-stu-id="0b5b6-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="0b5b6-170">从[androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)继承的有效值1到99</span><span class="sxs-lookup"><span data-stu-id="0b5b6-170">Valid values 1 to 99 Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="0b5b6-171">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="0b5b6-171">subjectNameFormat</span></span>|[<span data-ttu-id="0b5b6-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="0b5b6-172">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="0b5b6-173">证书使用者名称格式。</span><span class="sxs-lookup"><span data-stu-id="0b5b6-173">Certificate Subject Name Format.</span></span> <span data-ttu-id="0b5b6-174">继承自[androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="0b5b6-174">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="0b5b6-175">可取值为：`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId`。</span><span class="sxs-lookup"><span data-stu-id="0b5b6-175">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="0b5b6-176">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="0b5b6-176">certificateValidityPeriodValue</span></span>|<span data-ttu-id="0b5b6-177">Int32</span><span class="sxs-lookup"><span data-stu-id="0b5b6-177">Int32</span></span>|<span data-ttu-id="0b5b6-178">证书有效期限的值。</span><span class="sxs-lookup"><span data-stu-id="0b5b6-178">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="0b5b6-179">继承自[androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="0b5b6-179">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="0b5b6-180">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="0b5b6-180">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="0b5b6-181">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="0b5b6-181">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="0b5b6-182">证书有效期的小数位数。</span><span class="sxs-lookup"><span data-stu-id="0b5b6-182">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="0b5b6-183">继承自[androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="0b5b6-183">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="0b5b6-184">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="0b5b6-184">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="0b5b6-185">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="0b5b6-185">extendedKeyUsages</span></span>|<span data-ttu-id="0b5b6-186">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)集合</span><span class="sxs-lookup"><span data-stu-id="0b5b6-186">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="0b5b6-187">扩展密钥用法 (EKU) 设置。</span><span class="sxs-lookup"><span data-stu-id="0b5b6-187">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="0b5b6-188">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="0b5b6-188">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="0b5b6-189">继承自[androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="0b5b6-189">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="0b5b6-190">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="0b5b6-190">subjectAlternativeNameType</span></span>|[<span data-ttu-id="0b5b6-191">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="0b5b6-191">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="0b5b6-192">证书使用者备用名称类型。</span><span class="sxs-lookup"><span data-stu-id="0b5b6-192">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="0b5b6-193">继承自[androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="0b5b6-193">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="0b5b6-194">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute` 或 `domainNameService`。</span><span class="sxs-lookup"><span data-stu-id="0b5b6-194">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="0b5b6-195">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="0b5b6-195">certificationAuthority</span></span>|<span data-ttu-id="0b5b6-196">字符串</span><span class="sxs-lookup"><span data-stu-id="0b5b6-196">String</span></span>|<span data-ttu-id="0b5b6-197">PKCS 证书颁发机构</span><span class="sxs-lookup"><span data-stu-id="0b5b6-197">PKCS Certification Authority</span></span>|
|<span data-ttu-id="0b5b6-198">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="0b5b6-198">certificationAuthorityName</span></span>|<span data-ttu-id="0b5b6-199">字符串</span><span class="sxs-lookup"><span data-stu-id="0b5b6-199">String</span></span>|<span data-ttu-id="0b5b6-200">PKCS 证书颁发机构名称</span><span class="sxs-lookup"><span data-stu-id="0b5b6-200">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="0b5b6-201">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="0b5b6-201">certificateTemplateName</span></span>|<span data-ttu-id="0b5b6-202">字符串</span><span class="sxs-lookup"><span data-stu-id="0b5b6-202">String</span></span>|<span data-ttu-id="0b5b6-203">PKCS 证书模板名称</span><span class="sxs-lookup"><span data-stu-id="0b5b6-203">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="0b5b6-204">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="0b5b6-204">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="0b5b6-205">字符串</span><span class="sxs-lookup"><span data-stu-id="0b5b6-205">String</span></span>|<span data-ttu-id="0b5b6-206">定义 AAD 属性的自定义字符串。</span><span class="sxs-lookup"><span data-stu-id="0b5b6-206">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="0b5b6-207">响应</span><span class="sxs-lookup"><span data-stu-id="0b5b6-207">Response</span></span>
<span data-ttu-id="0b5b6-208">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0b5b6-208">If successful, this method returns a `201 Created` response code and a [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b5b6-209">示例</span><span class="sxs-lookup"><span data-stu-id="0b5b6-209">Example</span></span>

### <a name="request"></a><span data-ttu-id="0b5b6-210">请求</span><span class="sxs-lookup"><span data-stu-id="0b5b6-210">Request</span></span>
<span data-ttu-id="0b5b6-211">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0b5b6-211">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 965

{
  "@odata.type": "#microsoft.graph.androidForWorkPkcsCertificateProfile",
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

### <a name="response"></a><span data-ttu-id="0b5b6-212">响应</span><span class="sxs-lookup"><span data-stu-id="0b5b6-212">Response</span></span>
<span data-ttu-id="0b5b6-p116">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0b5b6-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1137

{
  "@odata.type": "#microsoft.graph.androidForWorkPkcsCertificateProfile",
  "id": "0a2d7691-7691-0a2d-9176-2d0a91762d0a",
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





