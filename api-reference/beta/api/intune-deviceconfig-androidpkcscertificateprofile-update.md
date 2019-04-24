---
title: 更新 androidPkcsCertificateProfile
description: 更新 androidPkcsCertificateProfile 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4142893ca96f953a8269fa54be07a9b35f5a9ff8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32475947"
---
# <a name="update-androidpkcscertificateprofile"></a><span data-ttu-id="9b836-103">更新 androidPkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="9b836-103">Update androidPkcsCertificateProfile</span></span>

> <span data-ttu-id="9b836-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9b836-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9b836-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9b836-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9b836-106">更新[androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9b836-106">Update the properties of a [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9b836-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="9b836-107">Prerequisites</span></span>
<span data-ttu-id="9b836-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9b836-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b836-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="9b836-110">Permission type</span></span>|<span data-ttu-id="9b836-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9b836-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9b836-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9b836-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9b836-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b836-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9b836-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9b836-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9b836-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9b836-115">Not supported.</span></span>|
|<span data-ttu-id="9b836-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="9b836-116">Application</span></span>|<span data-ttu-id="9b836-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="9b836-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9b836-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9b836-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="9b836-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="9b836-119">Request headers</span></span>
|<span data-ttu-id="9b836-120">标头</span><span class="sxs-lookup"><span data-stu-id="9b836-120">Header</span></span>|<span data-ttu-id="9b836-121">值</span><span class="sxs-lookup"><span data-stu-id="9b836-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9b836-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9b836-122">Authorization</span></span>|<span data-ttu-id="9b836-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9b836-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9b836-124">接受</span><span class="sxs-lookup"><span data-stu-id="9b836-124">Accept</span></span>|<span data-ttu-id="9b836-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9b836-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9b836-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="9b836-126">Request body</span></span>
<span data-ttu-id="9b836-127">在请求正文中, 提供[androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9b836-127">In the request body, supply a JSON representation for the [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) object.</span></span>

<span data-ttu-id="9b836-128">下表显示创建[androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="9b836-128">The following table shows the properties that are required when you create the [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md).</span></span>

|<span data-ttu-id="9b836-129">属性</span><span class="sxs-lookup"><span data-stu-id="9b836-129">Property</span></span>|<span data-ttu-id="9b836-130">类型</span><span class="sxs-lookup"><span data-stu-id="9b836-130">Type</span></span>|<span data-ttu-id="9b836-131">说明</span><span class="sxs-lookup"><span data-stu-id="9b836-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b836-132">id</span><span class="sxs-lookup"><span data-stu-id="9b836-132">id</span></span>|<span data-ttu-id="9b836-133">String</span><span class="sxs-lookup"><span data-stu-id="9b836-133">String</span></span>|<span data-ttu-id="9b836-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="9b836-134">Key of the entity.</span></span> <span data-ttu-id="9b836-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9b836-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9b836-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9b836-136">lastModifiedDateTime</span></span>|<span data-ttu-id="9b836-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9b836-137">DateTimeOffset</span></span>|<span data-ttu-id="9b836-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="9b836-138">DateTime the object was last modified.</span></span> <span data-ttu-id="9b836-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9b836-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9b836-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9b836-140">roleScopeTagIds</span></span>|<span data-ttu-id="9b836-141">String collection</span><span class="sxs-lookup"><span data-stu-id="9b836-141">String collection</span></span>|<span data-ttu-id="9b836-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="9b836-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9b836-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9b836-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9b836-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="9b836-144">supportsScopeTags</span></span>|<span data-ttu-id="9b836-145">布尔</span><span class="sxs-lookup"><span data-stu-id="9b836-145">Boolean</span></span>|<span data-ttu-id="9b836-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="9b836-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="9b836-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="9b836-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="9b836-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="9b836-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="9b836-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9b836-149">This property is read-only.</span></span> <span data-ttu-id="9b836-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9b836-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9b836-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9b836-151">createdDateTime</span></span>|<span data-ttu-id="9b836-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9b836-152">DateTimeOffset</span></span>|<span data-ttu-id="9b836-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="9b836-153">DateTime the object was created.</span></span> <span data-ttu-id="9b836-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9b836-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9b836-155">description</span><span class="sxs-lookup"><span data-stu-id="9b836-155">description</span></span>|<span data-ttu-id="9b836-156">字符串</span><span class="sxs-lookup"><span data-stu-id="9b836-156">String</span></span>|<span data-ttu-id="9b836-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="9b836-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9b836-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9b836-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9b836-159">displayName</span><span class="sxs-lookup"><span data-stu-id="9b836-159">displayName</span></span>|<span data-ttu-id="9b836-160">String</span><span class="sxs-lookup"><span data-stu-id="9b836-160">String</span></span>|<span data-ttu-id="9b836-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="9b836-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9b836-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9b836-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9b836-163">version</span><span class="sxs-lookup"><span data-stu-id="9b836-163">version</span></span>|<span data-ttu-id="9b836-164">Int32</span><span class="sxs-lookup"><span data-stu-id="9b836-164">Int32</span></span>|<span data-ttu-id="9b836-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="9b836-165">Version of the device configuration.</span></span> <span data-ttu-id="9b836-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9b836-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9b836-167">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="9b836-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="9b836-168">Int32</span><span class="sxs-lookup"><span data-stu-id="9b836-168">Int32</span></span>|<span data-ttu-id="9b836-169">证书续订阈值百分比。</span><span class="sxs-lookup"><span data-stu-id="9b836-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="9b836-170">从[androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)继承的有效值1到99</span><span class="sxs-lookup"><span data-stu-id="9b836-170">Valid values 1 to 99 Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="9b836-171">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="9b836-171">subjectNameFormat</span></span>|[<span data-ttu-id="9b836-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="9b836-172">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="9b836-173">证书使用者名称格式。</span><span class="sxs-lookup"><span data-stu-id="9b836-173">Certificate Subject Name Format.</span></span> <span data-ttu-id="9b836-174">继承自[androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="9b836-174">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="9b836-175">可取值为：`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId`。</span><span class="sxs-lookup"><span data-stu-id="9b836-175">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="9b836-176">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="9b836-176">subjectAlternativeNameType</span></span>|[<span data-ttu-id="9b836-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="9b836-177">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="9b836-178">证书使用者备用名称类型。</span><span class="sxs-lookup"><span data-stu-id="9b836-178">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="9b836-179">继承自[androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="9b836-179">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="9b836-180">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute` 或 `domainNameService`。</span><span class="sxs-lookup"><span data-stu-id="9b836-180">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="9b836-181">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="9b836-181">certificateValidityPeriodValue</span></span>|<span data-ttu-id="9b836-182">Int32</span><span class="sxs-lookup"><span data-stu-id="9b836-182">Int32</span></span>|<span data-ttu-id="9b836-183">证书有效期限的值。</span><span class="sxs-lookup"><span data-stu-id="9b836-183">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="9b836-184">继承自[androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="9b836-184">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="9b836-185">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="9b836-185">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="9b836-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="9b836-186">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="9b836-187">证书有效期的小数位数。</span><span class="sxs-lookup"><span data-stu-id="9b836-187">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="9b836-188">继承自[androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="9b836-188">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="9b836-189">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="9b836-189">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="9b836-190">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="9b836-190">extendedKeyUsages</span></span>|<span data-ttu-id="9b836-191">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)集合</span><span class="sxs-lookup"><span data-stu-id="9b836-191">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="9b836-192">扩展密钥用法 (EKU) 设置。</span><span class="sxs-lookup"><span data-stu-id="9b836-192">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="9b836-193">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="9b836-193">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="9b836-194">继承自[androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="9b836-194">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="9b836-195">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="9b836-195">certificationAuthority</span></span>|<span data-ttu-id="9b836-196">字符串</span><span class="sxs-lookup"><span data-stu-id="9b836-196">String</span></span>|<span data-ttu-id="9b836-197">PKCS 证书颁发机构</span><span class="sxs-lookup"><span data-stu-id="9b836-197">PKCS Certification Authority</span></span>|
|<span data-ttu-id="9b836-198">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="9b836-198">certificationAuthorityName</span></span>|<span data-ttu-id="9b836-199">字符串</span><span class="sxs-lookup"><span data-stu-id="9b836-199">String</span></span>|<span data-ttu-id="9b836-200">PKCS 证书颁发机构名称</span><span class="sxs-lookup"><span data-stu-id="9b836-200">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="9b836-201">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="9b836-201">certificateTemplateName</span></span>|<span data-ttu-id="9b836-202">字符串</span><span class="sxs-lookup"><span data-stu-id="9b836-202">String</span></span>|<span data-ttu-id="9b836-203">PKCS 证书模板名称</span><span class="sxs-lookup"><span data-stu-id="9b836-203">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="9b836-204">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="9b836-204">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="9b836-205">字符串</span><span class="sxs-lookup"><span data-stu-id="9b836-205">String</span></span>|<span data-ttu-id="9b836-206">定义 AAD 属性的自定义字符串。</span><span class="sxs-lookup"><span data-stu-id="9b836-206">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="9b836-207">响应</span><span class="sxs-lookup"><span data-stu-id="9b836-207">Response</span></span>
<span data-ttu-id="9b836-208">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9b836-208">If successful, this method returns a `200 OK` response code and an updated [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9b836-209">示例</span><span class="sxs-lookup"><span data-stu-id="9b836-209">Example</span></span>

### <a name="request"></a><span data-ttu-id="9b836-210">请求</span><span class="sxs-lookup"><span data-stu-id="9b836-210">Request</span></span>
<span data-ttu-id="9b836-211">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9b836-211">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 958

{
  "@odata.type": "#microsoft.graph.androidPkcsCertificateProfile",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "renewalThresholdPercentage": 10,
  "subjectNameFormat": "commonNameIncludingEmail",
  "subjectAlternativeNameType": "emailAddress",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```

### <a name="response"></a><span data-ttu-id="9b836-212">响应</span><span class="sxs-lookup"><span data-stu-id="9b836-212">Response</span></span>
<span data-ttu-id="9b836-p116">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9b836-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1130

{
  "@odata.type": "#microsoft.graph.androidPkcsCertificateProfile",
  "id": "bb55705b-705b-bb55-5b70-55bb5b7055bb",
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
  "subjectAlternativeNameType": "emailAddress",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```





