---
title: 更新 iosScepCertificateProfile
description: 更新 iosScepCertificateProfile 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c7ac67a81dab6faca9724c9cf7eec17d4920414d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396495"
---
# <a name="update-iosscepcertificateprofile"></a><span data-ttu-id="855be-103">更新 iosScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="855be-103">Update iosScepCertificateProfile</span></span>

> <span data-ttu-id="855be-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="855be-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="855be-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="855be-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="855be-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="855be-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="855be-107">更新[iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="855be-107">Update the properties of a [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="855be-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="855be-108">Prerequisites</span></span>
<span data-ttu-id="855be-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="855be-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="855be-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="855be-111">Permission type</span></span>|<span data-ttu-id="855be-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="855be-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="855be-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="855be-113">Delegated (work or school account)</span></span>|<span data-ttu-id="855be-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="855be-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="855be-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="855be-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="855be-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="855be-116">Not supported.</span></span>|
|<span data-ttu-id="855be-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="855be-117">Application</span></span>|<span data-ttu-id="855be-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="855be-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="855be-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="855be-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="855be-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="855be-120">Request headers</span></span>
|<span data-ttu-id="855be-121">标头</span><span class="sxs-lookup"><span data-stu-id="855be-121">Header</span></span>|<span data-ttu-id="855be-122">值</span><span class="sxs-lookup"><span data-stu-id="855be-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="855be-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="855be-123">Authorization</span></span>|<span data-ttu-id="855be-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="855be-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="855be-125">Accept</span><span class="sxs-lookup"><span data-stu-id="855be-125">Accept</span></span>|<span data-ttu-id="855be-126">application/json</span><span class="sxs-lookup"><span data-stu-id="855be-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="855be-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="855be-127">Request body</span></span>
<span data-ttu-id="855be-128">在请求正文中，提供[iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="855be-128">In the request body, supply a JSON representation for the [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) object.</span></span>

<span data-ttu-id="855be-129">下表显示时创建[iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="855be-129">The following table shows the properties that are required when you create the [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md).</span></span>

|<span data-ttu-id="855be-130">属性</span><span class="sxs-lookup"><span data-stu-id="855be-130">Property</span></span>|<span data-ttu-id="855be-131">类型</span><span class="sxs-lookup"><span data-stu-id="855be-131">Type</span></span>|<span data-ttu-id="855be-132">说明</span><span class="sxs-lookup"><span data-stu-id="855be-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="855be-133">id</span><span class="sxs-lookup"><span data-stu-id="855be-133">id</span></span>|<span data-ttu-id="855be-134">String</span><span class="sxs-lookup"><span data-stu-id="855be-134">String</span></span>|<span data-ttu-id="855be-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="855be-135">Key of the entity.</span></span> <span data-ttu-id="855be-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="855be-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="855be-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="855be-137">lastModifiedDateTime</span></span>|<span data-ttu-id="855be-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="855be-138">DateTimeOffset</span></span>|<span data-ttu-id="855be-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="855be-139">DateTime the object was last modified.</span></span> <span data-ttu-id="855be-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="855be-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="855be-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="855be-141">roleScopeTagIds</span></span>|<span data-ttu-id="855be-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="855be-142">String collection</span></span>|<span data-ttu-id="855be-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="855be-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="855be-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="855be-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="855be-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="855be-145">supportsScopeTags</span></span>|<span data-ttu-id="855be-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="855be-146">Boolean</span></span>|<span data-ttu-id="855be-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="855be-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="855be-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="855be-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="855be-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="855be-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="855be-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="855be-150">This property is read-only.</span></span> <span data-ttu-id="855be-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="855be-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="855be-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="855be-152">createdDateTime</span></span>|<span data-ttu-id="855be-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="855be-153">DateTimeOffset</span></span>|<span data-ttu-id="855be-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="855be-154">DateTime the object was created.</span></span> <span data-ttu-id="855be-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="855be-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="855be-156">description</span><span class="sxs-lookup"><span data-stu-id="855be-156">description</span></span>|<span data-ttu-id="855be-157">String</span><span class="sxs-lookup"><span data-stu-id="855be-157">String</span></span>|<span data-ttu-id="855be-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="855be-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="855be-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="855be-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="855be-160">displayName</span><span class="sxs-lookup"><span data-stu-id="855be-160">displayName</span></span>|<span data-ttu-id="855be-161">String</span><span class="sxs-lookup"><span data-stu-id="855be-161">String</span></span>|<span data-ttu-id="855be-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="855be-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="855be-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="855be-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="855be-164">version</span><span class="sxs-lookup"><span data-stu-id="855be-164">version</span></span>|<span data-ttu-id="855be-165">Int32</span><span class="sxs-lookup"><span data-stu-id="855be-165">Int32</span></span>|<span data-ttu-id="855be-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="855be-166">Version of the device configuration.</span></span> <span data-ttu-id="855be-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="855be-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="855be-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="855be-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="855be-169">Int32</span><span class="sxs-lookup"><span data-stu-id="855be-169">Int32</span></span>|<span data-ttu-id="855be-170">证书续订阈值百分比。</span><span class="sxs-lookup"><span data-stu-id="855be-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="855be-171">有效值 1 到 99 继承自[iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="855be-171">Valid values 1 to 99 Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="855be-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="855be-172">subjectNameFormat</span></span>|[<span data-ttu-id="855be-173">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="855be-173">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="855be-174">证书使用者名称格式。</span><span class="sxs-lookup"><span data-stu-id="855be-174">Certificate Subject Name Format.</span></span> <span data-ttu-id="855be-175">继承自[iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="855be-175">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="855be-176">可取值为：`commonName`、`commonNameAsEmail`、`custom`、`commonNameIncludingEmail`、`commonNameAsIMEI`、`commonNameAsSerialNumber`。</span><span class="sxs-lookup"><span data-stu-id="855be-176">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="855be-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="855be-177">subjectAlternativeNameType</span></span>|[<span data-ttu-id="855be-178">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="855be-178">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="855be-179">证书使用者替代名称类型。</span><span class="sxs-lookup"><span data-stu-id="855be-179">Certificate Subject Alternative Name type.</span></span> <span data-ttu-id="855be-180">继承自[iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="855be-180">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="855be-181">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService`。</span><span class="sxs-lookup"><span data-stu-id="855be-181">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="855be-182">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="855be-182">certificateValidityPeriodValue</span></span>|<span data-ttu-id="855be-183">Int32</span><span class="sxs-lookup"><span data-stu-id="855be-183">Int32</span></span>|<span data-ttu-id="855be-184">证书有效期限的值。</span><span class="sxs-lookup"><span data-stu-id="855be-184">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="855be-185">继承自[iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="855be-185">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="855be-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="855be-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="855be-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="855be-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="855be-188">证书有效期限的小数位数。</span><span class="sxs-lookup"><span data-stu-id="855be-188">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="855be-189">继承自[iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="855be-189">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="855be-190">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="855be-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="855be-191">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="855be-191">scepServerUrls</span></span>|<span data-ttu-id="855be-192">String 集合</span><span class="sxs-lookup"><span data-stu-id="855be-192">String collection</span></span>|<span data-ttu-id="855be-193">SCEP 服务器 Url(s)。</span><span class="sxs-lookup"><span data-stu-id="855be-193">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="855be-194">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="855be-194">subjectNameFormatString</span></span>|<span data-ttu-id="855be-195">String</span><span class="sxs-lookup"><span data-stu-id="855be-195">String</span></span>|<span data-ttu-id="855be-196">自定义格式使用 SubjectNameFormat = 自定义。</span><span class="sxs-lookup"><span data-stu-id="855be-196">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="855be-197">示例： CN = {{EmailAddress}} E = {{EmailAddress}}，OU = 企业用户，O = Contoso Corporation L = 雷德蒙德，ST = WA，C = US</span><span class="sxs-lookup"><span data-stu-id="855be-197">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="855be-198">keyUsage</span><span class="sxs-lookup"><span data-stu-id="855be-198">keyUsage</span></span>|[<span data-ttu-id="855be-199">keyUsages</span><span class="sxs-lookup"><span data-stu-id="855be-199">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="855be-200">SCEP 密钥用法。</span><span class="sxs-lookup"><span data-stu-id="855be-200">SCEP Key Usage.</span></span> <span data-ttu-id="855be-201">可取值为：`keyEncipherment`、`digitalSignature`。</span><span class="sxs-lookup"><span data-stu-id="855be-201">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="855be-202">keySize</span><span class="sxs-lookup"><span data-stu-id="855be-202">keySize</span></span>|[<span data-ttu-id="855be-203">keySize</span><span class="sxs-lookup"><span data-stu-id="855be-203">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="855be-204">SCEP 密钥大小。</span><span class="sxs-lookup"><span data-stu-id="855be-204">SCEP Key Size.</span></span> <span data-ttu-id="855be-205">可取值为：`size1024`、`size2048`。</span><span class="sxs-lookup"><span data-stu-id="855be-205">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="855be-206">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="855be-206">extendedKeyUsages</span></span>|<span data-ttu-id="855be-207">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)集合</span><span class="sxs-lookup"><span data-stu-id="855be-207">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="855be-208">扩展的密钥用法 (EKU) 设置。</span><span class="sxs-lookup"><span data-stu-id="855be-208">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="855be-209">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="855be-209">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="855be-210">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="855be-210">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="855be-211">String</span><span class="sxs-lookup"><span data-stu-id="855be-211">String</span></span>|<span data-ttu-id="855be-212">定义 AAD 属性的自定义字符串。</span><span class="sxs-lookup"><span data-stu-id="855be-212">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="855be-213">certificateStore</span><span class="sxs-lookup"><span data-stu-id="855be-213">certificateStore</span></span>|[<span data-ttu-id="855be-214">certificateStore</span><span class="sxs-lookup"><span data-stu-id="855be-214">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="855be-215">目标存储证书。</span><span class="sxs-lookup"><span data-stu-id="855be-215">Target store certificate.</span></span> <span data-ttu-id="855be-216">可取值为：`user`、`machine`。</span><span class="sxs-lookup"><span data-stu-id="855be-216">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="855be-217">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="855be-217">customSubjectAlternativeNames</span></span>|<span data-ttu-id="855be-218">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)集合</span><span class="sxs-lookup"><span data-stu-id="855be-218">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="855be-219">自定义主题 Alterantive 名称设置。</span><span class="sxs-lookup"><span data-stu-id="855be-219">Custom Subject Alterantive Name Settings.</span></span> <span data-ttu-id="855be-220">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="855be-220">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="855be-221">响应</span><span class="sxs-lookup"><span data-stu-id="855be-221">Response</span></span>
<span data-ttu-id="855be-222">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="855be-222">If successful, this method returns a `200 OK` response code and an updated [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="855be-223">示例</span><span class="sxs-lookup"><span data-stu-id="855be-223">Example</span></span>

### <a name="request"></a><span data-ttu-id="855be-224">请求</span><span class="sxs-lookup"><span data-stu-id="855be-224">Request</span></span>
<span data-ttu-id="855be-225">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="855be-225">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1159

{
  "@odata.type": "#microsoft.graph.iosScepCertificateProfile",
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

### <a name="response"></a><span data-ttu-id="855be-226">响应</span><span class="sxs-lookup"><span data-stu-id="855be-226">Response</span></span>
<span data-ttu-id="855be-p122">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="855be-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1331

{
  "@odata.type": "#microsoft.graph.iosScepCertificateProfile",
  "id": "0deb8dbf-8dbf-0deb-bf8d-eb0dbf8deb0d",
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




