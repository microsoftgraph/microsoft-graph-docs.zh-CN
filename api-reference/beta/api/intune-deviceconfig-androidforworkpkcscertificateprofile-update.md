---
title: 更新 androidForWorkPkcsCertificateProfile
description: 更新 androidForWorkPkcsCertificateProfile 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 058cb9ae0ba87aaf88b58f1bf4f3fe61bb458bbc
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30977196"
---
# <a name="update-androidforworkpkcscertificateprofile"></a><span data-ttu-id="33fdd-103">更新 androidForWorkPkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="33fdd-103">Update androidForWorkPkcsCertificateProfile</span></span>

> <span data-ttu-id="33fdd-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="33fdd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="33fdd-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="33fdd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="33fdd-106">更新[androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="33fdd-106">Update the properties of a [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="33fdd-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="33fdd-107">Prerequisites</span></span>
<span data-ttu-id="33fdd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="33fdd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33fdd-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="33fdd-110">Permission type</span></span>|<span data-ttu-id="33fdd-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="33fdd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="33fdd-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="33fdd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="33fdd-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33fdd-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="33fdd-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="33fdd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="33fdd-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="33fdd-115">Not supported.</span></span>|
|<span data-ttu-id="33fdd-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="33fdd-116">Application</span></span>|<span data-ttu-id="33fdd-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="33fdd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="33fdd-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="33fdd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="33fdd-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="33fdd-119">Request headers</span></span>
|<span data-ttu-id="33fdd-120">标头</span><span class="sxs-lookup"><span data-stu-id="33fdd-120">Header</span></span>|<span data-ttu-id="33fdd-121">值</span><span class="sxs-lookup"><span data-stu-id="33fdd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="33fdd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="33fdd-122">Authorization</span></span>|<span data-ttu-id="33fdd-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="33fdd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="33fdd-124">接受</span><span class="sxs-lookup"><span data-stu-id="33fdd-124">Accept</span></span>|<span data-ttu-id="33fdd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="33fdd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="33fdd-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="33fdd-126">Request body</span></span>
<span data-ttu-id="33fdd-127">在请求正文中, 提供[androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="33fdd-127">In the request body, supply a JSON representation for the [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) object.</span></span>

<span data-ttu-id="33fdd-128">下表显示创建[androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="33fdd-128">The following table shows the properties that are required when you create the [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md).</span></span>

|<span data-ttu-id="33fdd-129">属性</span><span class="sxs-lookup"><span data-stu-id="33fdd-129">Property</span></span>|<span data-ttu-id="33fdd-130">类型</span><span class="sxs-lookup"><span data-stu-id="33fdd-130">Type</span></span>|<span data-ttu-id="33fdd-131">说明</span><span class="sxs-lookup"><span data-stu-id="33fdd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33fdd-132">id</span><span class="sxs-lookup"><span data-stu-id="33fdd-132">id</span></span>|<span data-ttu-id="33fdd-133">String</span><span class="sxs-lookup"><span data-stu-id="33fdd-133">String</span></span>|<span data-ttu-id="33fdd-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="33fdd-134">Key of the entity.</span></span> <span data-ttu-id="33fdd-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="33fdd-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33fdd-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="33fdd-136">lastModifiedDateTime</span></span>|<span data-ttu-id="33fdd-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="33fdd-137">DateTimeOffset</span></span>|<span data-ttu-id="33fdd-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="33fdd-138">DateTime the object was last modified.</span></span> <span data-ttu-id="33fdd-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="33fdd-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33fdd-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="33fdd-140">roleScopeTagIds</span></span>|<span data-ttu-id="33fdd-141">String 集合</span><span class="sxs-lookup"><span data-stu-id="33fdd-141">String collection</span></span>|<span data-ttu-id="33fdd-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="33fdd-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="33fdd-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="33fdd-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33fdd-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="33fdd-144">supportsScopeTags</span></span>|<span data-ttu-id="33fdd-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="33fdd-145">Boolean</span></span>|<span data-ttu-id="33fdd-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="33fdd-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="33fdd-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="33fdd-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="33fdd-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="33fdd-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="33fdd-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="33fdd-149">This property is read-only.</span></span> <span data-ttu-id="33fdd-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="33fdd-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33fdd-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="33fdd-151">createdDateTime</span></span>|<span data-ttu-id="33fdd-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="33fdd-152">DateTimeOffset</span></span>|<span data-ttu-id="33fdd-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="33fdd-153">DateTime the object was created.</span></span> <span data-ttu-id="33fdd-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="33fdd-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33fdd-155">description</span><span class="sxs-lookup"><span data-stu-id="33fdd-155">description</span></span>|<span data-ttu-id="33fdd-156">String</span><span class="sxs-lookup"><span data-stu-id="33fdd-156">String</span></span>|<span data-ttu-id="33fdd-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="33fdd-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="33fdd-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="33fdd-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33fdd-159">displayName</span><span class="sxs-lookup"><span data-stu-id="33fdd-159">displayName</span></span>|<span data-ttu-id="33fdd-160">String</span><span class="sxs-lookup"><span data-stu-id="33fdd-160">String</span></span>|<span data-ttu-id="33fdd-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="33fdd-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="33fdd-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="33fdd-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33fdd-163">version</span><span class="sxs-lookup"><span data-stu-id="33fdd-163">version</span></span>|<span data-ttu-id="33fdd-164">Int32</span><span class="sxs-lookup"><span data-stu-id="33fdd-164">Int32</span></span>|<span data-ttu-id="33fdd-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="33fdd-165">Version of the device configuration.</span></span> <span data-ttu-id="33fdd-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="33fdd-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33fdd-167">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="33fdd-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="33fdd-168">Int32</span><span class="sxs-lookup"><span data-stu-id="33fdd-168">Int32</span></span>|<span data-ttu-id="33fdd-169">证书续订阈值百分比。</span><span class="sxs-lookup"><span data-stu-id="33fdd-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="33fdd-170">从[androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)继承的有效值1到99</span><span class="sxs-lookup"><span data-stu-id="33fdd-170">Valid values 1 to 99 Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="33fdd-171">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="33fdd-171">subjectNameFormat</span></span>|[<span data-ttu-id="33fdd-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="33fdd-172">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="33fdd-173">证书使用者名称格式。</span><span class="sxs-lookup"><span data-stu-id="33fdd-173">Certificate Subject Name Format.</span></span> <span data-ttu-id="33fdd-174">继承自[androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="33fdd-174">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="33fdd-175">可取值为：`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId`。</span><span class="sxs-lookup"><span data-stu-id="33fdd-175">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="33fdd-176">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="33fdd-176">certificateValidityPeriodValue</span></span>|<span data-ttu-id="33fdd-177">Int32</span><span class="sxs-lookup"><span data-stu-id="33fdd-177">Int32</span></span>|<span data-ttu-id="33fdd-178">证书有效期限的值。</span><span class="sxs-lookup"><span data-stu-id="33fdd-178">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="33fdd-179">继承自[androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="33fdd-179">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="33fdd-180">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="33fdd-180">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="33fdd-181">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="33fdd-181">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="33fdd-182">证书有效期的小数位数。</span><span class="sxs-lookup"><span data-stu-id="33fdd-182">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="33fdd-183">继承自[androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="33fdd-183">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="33fdd-184">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="33fdd-184">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="33fdd-185">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="33fdd-185">extendedKeyUsages</span></span>|<span data-ttu-id="33fdd-186">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)集合</span><span class="sxs-lookup"><span data-stu-id="33fdd-186">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="33fdd-187">扩展密钥用法 (EKU) 设置。</span><span class="sxs-lookup"><span data-stu-id="33fdd-187">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="33fdd-188">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="33fdd-188">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="33fdd-189">继承自[androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="33fdd-189">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="33fdd-190">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="33fdd-190">certificationAuthority</span></span>|<span data-ttu-id="33fdd-191">String</span><span class="sxs-lookup"><span data-stu-id="33fdd-191">String</span></span>|<span data-ttu-id="33fdd-192">PKCS 证书颁发机构</span><span class="sxs-lookup"><span data-stu-id="33fdd-192">PKCS Certification Authority</span></span>|
|<span data-ttu-id="33fdd-193">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="33fdd-193">certificationAuthorityName</span></span>|<span data-ttu-id="33fdd-194">String</span><span class="sxs-lookup"><span data-stu-id="33fdd-194">String</span></span>|<span data-ttu-id="33fdd-195">PKCS 证书颁发机构名称</span><span class="sxs-lookup"><span data-stu-id="33fdd-195">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="33fdd-196">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="33fdd-196">certificateTemplateName</span></span>|<span data-ttu-id="33fdd-197">String</span><span class="sxs-lookup"><span data-stu-id="33fdd-197">String</span></span>|<span data-ttu-id="33fdd-198">PKCS 证书模板名称</span><span class="sxs-lookup"><span data-stu-id="33fdd-198">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="33fdd-199">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="33fdd-199">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="33fdd-200">String</span><span class="sxs-lookup"><span data-stu-id="33fdd-200">String</span></span>|<span data-ttu-id="33fdd-201">定义 AAD 属性的自定义字符串。</span><span class="sxs-lookup"><span data-stu-id="33fdd-201">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="33fdd-202">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="33fdd-202">subjectAlternativeNameType</span></span>|[<span data-ttu-id="33fdd-203">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="33fdd-203">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="33fdd-204">证书使用者备用名称类型。</span><span class="sxs-lookup"><span data-stu-id="33fdd-204">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="33fdd-205">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute` 或 `domainNameService`。</span><span class="sxs-lookup"><span data-stu-id="33fdd-205">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|



## <a name="response"></a><span data-ttu-id="33fdd-206">响应</span><span class="sxs-lookup"><span data-stu-id="33fdd-206">Response</span></span>
<span data-ttu-id="33fdd-207">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="33fdd-207">If successful, this method returns a `200 OK` response code and an updated [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33fdd-208">示例</span><span class="sxs-lookup"><span data-stu-id="33fdd-208">Example</span></span>

### <a name="request"></a><span data-ttu-id="33fdd-209">请求</span><span class="sxs-lookup"><span data-stu-id="33fdd-209">Request</span></span>
<span data-ttu-id="33fdd-210">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="33fdd-210">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "subjectAlternativeNameType": "emailAddress"
}
```

### <a name="response"></a><span data-ttu-id="33fdd-211">响应</span><span class="sxs-lookup"><span data-stu-id="33fdd-211">Response</span></span>
<span data-ttu-id="33fdd-p116">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="33fdd-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "subjectAlternativeNameType": "emailAddress"
}
```




