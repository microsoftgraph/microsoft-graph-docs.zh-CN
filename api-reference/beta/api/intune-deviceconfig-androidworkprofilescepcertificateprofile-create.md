---
title: 创建 androidWorkProfileScepCertificateProfile
description: 创建新的 androidWorkProfileScepCertificateProfile 对象。
ms.openlocfilehash: 780418250a7d8e00cc7923dda66d4f8d8682dddc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048135"
---
# <a name="create-androidworkprofilescepcertificateprofile"></a><span data-ttu-id="676aa-103">创建 androidWorkProfileScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="676aa-103">Create androidWorkProfileScepCertificateProfile</span></span>

> <span data-ttu-id="676aa-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="676aa-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="676aa-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="676aa-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="676aa-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="676aa-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="676aa-107">创建新的[androidWorkProfileScepCertificateProfile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="676aa-107">Create a new [androidWorkProfileScepCertificateProfile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="676aa-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="676aa-108">Prerequisites</span></span>
<span data-ttu-id="676aa-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="676aa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="676aa-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="676aa-111">Permission type</span></span>|<span data-ttu-id="676aa-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="676aa-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="676aa-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="676aa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="676aa-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="676aa-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="676aa-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="676aa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="676aa-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="676aa-116">Not supported.</span></span>|
|<span data-ttu-id="676aa-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="676aa-117">Application</span></span>|<span data-ttu-id="676aa-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="676aa-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="676aa-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="676aa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="676aa-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="676aa-120">Request headers</span></span>
|<span data-ttu-id="676aa-121">标头</span><span class="sxs-lookup"><span data-stu-id="676aa-121">Header</span></span>|<span data-ttu-id="676aa-122">值</span><span class="sxs-lookup"><span data-stu-id="676aa-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="676aa-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="676aa-123">Authorization</span></span>|<span data-ttu-id="676aa-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="676aa-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="676aa-125">Accept</span><span class="sxs-lookup"><span data-stu-id="676aa-125">Accept</span></span>|<span data-ttu-id="676aa-126">application/json</span><span class="sxs-lookup"><span data-stu-id="676aa-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="676aa-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="676aa-127">Request body</span></span>
<span data-ttu-id="676aa-128">在请求正文中，提供 androidWorkProfileScepCertificateProfile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="676aa-128">In the request body, supply a JSON representation for the androidWorkProfileScepCertificateProfile object.</span></span>

<span data-ttu-id="676aa-129">下表显示时创建 androidWorkProfileScepCertificateProfile 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="676aa-129">The following table shows the properties that are required when you create the androidWorkProfileScepCertificateProfile.</span></span>

|<span data-ttu-id="676aa-130">属性</span><span class="sxs-lookup"><span data-stu-id="676aa-130">Property</span></span>|<span data-ttu-id="676aa-131">类型</span><span class="sxs-lookup"><span data-stu-id="676aa-131">Type</span></span>|<span data-ttu-id="676aa-132">说明</span><span class="sxs-lookup"><span data-stu-id="676aa-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="676aa-133">id</span><span class="sxs-lookup"><span data-stu-id="676aa-133">id</span></span>|<span data-ttu-id="676aa-134">String</span><span class="sxs-lookup"><span data-stu-id="676aa-134">String</span></span>|<span data-ttu-id="676aa-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="676aa-135">Key of the entity.</span></span> <span data-ttu-id="676aa-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="676aa-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="676aa-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="676aa-137">lastModifiedDateTime</span></span>|<span data-ttu-id="676aa-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="676aa-138">DateTimeOffset</span></span>|<span data-ttu-id="676aa-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="676aa-139">DateTime the object was last modified.</span></span> <span data-ttu-id="676aa-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="676aa-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="676aa-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="676aa-141">roleScopeTagIds</span></span>|<span data-ttu-id="676aa-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="676aa-142">String collection</span></span>|<span data-ttu-id="676aa-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="676aa-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="676aa-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="676aa-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="676aa-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="676aa-145">supportsScopeTags</span></span>|<span data-ttu-id="676aa-146">布尔</span><span class="sxs-lookup"><span data-stu-id="676aa-146">Boolean</span></span>|<span data-ttu-id="676aa-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="676aa-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="676aa-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="676aa-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="676aa-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="676aa-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="676aa-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="676aa-150">This property is read-only.</span></span> <span data-ttu-id="676aa-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="676aa-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="676aa-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="676aa-152">createdDateTime</span></span>|<span data-ttu-id="676aa-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="676aa-153">DateTimeOffset</span></span>|<span data-ttu-id="676aa-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="676aa-154">DateTime the object was created.</span></span> <span data-ttu-id="676aa-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="676aa-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="676aa-156">description</span><span class="sxs-lookup"><span data-stu-id="676aa-156">description</span></span>|<span data-ttu-id="676aa-157">String</span><span class="sxs-lookup"><span data-stu-id="676aa-157">String</span></span>|<span data-ttu-id="676aa-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="676aa-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="676aa-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="676aa-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="676aa-160">displayName</span><span class="sxs-lookup"><span data-stu-id="676aa-160">displayName</span></span>|<span data-ttu-id="676aa-161">String</span><span class="sxs-lookup"><span data-stu-id="676aa-161">String</span></span>|<span data-ttu-id="676aa-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="676aa-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="676aa-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="676aa-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="676aa-164">version</span><span class="sxs-lookup"><span data-stu-id="676aa-164">version</span></span>|<span data-ttu-id="676aa-165">Int32</span><span class="sxs-lookup"><span data-stu-id="676aa-165">Int32</span></span>|<span data-ttu-id="676aa-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="676aa-166">Version of the device configuration.</span></span> <span data-ttu-id="676aa-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="676aa-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="676aa-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="676aa-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="676aa-169">Int32</span><span class="sxs-lookup"><span data-stu-id="676aa-169">Int32</span></span>|<span data-ttu-id="676aa-170">证书续订阈值百分比。</span><span class="sxs-lookup"><span data-stu-id="676aa-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="676aa-171">有效值 1 到 99 继承自[androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="676aa-171">Valid values 1 to 99 Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="676aa-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="676aa-172">subjectNameFormat</span></span>|[<span data-ttu-id="676aa-173">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="676aa-173">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="676aa-174">证书使用者名称格式。</span><span class="sxs-lookup"><span data-stu-id="676aa-174">Certificate Subject Name Format.</span></span> <span data-ttu-id="676aa-175">继承自[androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="676aa-175">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="676aa-176">可取值为：`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId`。</span><span class="sxs-lookup"><span data-stu-id="676aa-176">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="676aa-177">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="676aa-177">certificateValidityPeriodValue</span></span>|<span data-ttu-id="676aa-178">Int32</span><span class="sxs-lookup"><span data-stu-id="676aa-178">Int32</span></span>|<span data-ttu-id="676aa-179">证书有效期限的值。</span><span class="sxs-lookup"><span data-stu-id="676aa-179">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="676aa-180">继承自[androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="676aa-180">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="676aa-181">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="676aa-181">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="676aa-182">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="676aa-182">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="676aa-183">证书有效期限的小数位数。</span><span class="sxs-lookup"><span data-stu-id="676aa-183">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="676aa-184">继承自[androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="676aa-184">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="676aa-185">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="676aa-185">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="676aa-186">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="676aa-186">extendedKeyUsages</span></span>|<span data-ttu-id="676aa-187">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)集合</span><span class="sxs-lookup"><span data-stu-id="676aa-187">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="676aa-188">扩展的密钥用法 (EKU) 设置。</span><span class="sxs-lookup"><span data-stu-id="676aa-188">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="676aa-189">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="676aa-189">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="676aa-190">继承自[androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="676aa-190">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="676aa-191">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="676aa-191">scepServerUrls</span></span>|<span data-ttu-id="676aa-192">String 集合</span><span class="sxs-lookup"><span data-stu-id="676aa-192">String collection</span></span>|<span data-ttu-id="676aa-193">SCEP 服务器 Url(s)</span><span class="sxs-lookup"><span data-stu-id="676aa-193">SCEP Server Url(s)</span></span>|
|<span data-ttu-id="676aa-194">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="676aa-194">subjectNameFormatString</span></span>|<span data-ttu-id="676aa-195">字符串</span><span class="sxs-lookup"><span data-stu-id="676aa-195">String</span></span>|<span data-ttu-id="676aa-196">自定义格式使用 SubjectNameFormat = 自定义。</span><span class="sxs-lookup"><span data-stu-id="676aa-196">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="676aa-197">示例： CN = {{EmailAddress}} E = {{EmailAddress}}，OU = 企业用户，O = Contoso Corporation L = 雷德蒙德，ST = WA，C = US</span><span class="sxs-lookup"><span data-stu-id="676aa-197">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="676aa-198">keyUsage</span><span class="sxs-lookup"><span data-stu-id="676aa-198">keyUsage</span></span>|[<span data-ttu-id="676aa-199">keyUsages</span><span class="sxs-lookup"><span data-stu-id="676aa-199">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="676aa-200">SCEP 密钥用法。</span><span class="sxs-lookup"><span data-stu-id="676aa-200">SCEP Key Usage.</span></span> <span data-ttu-id="676aa-201">可取值为：`keyEncipherment`、`digitalSignature`。</span><span class="sxs-lookup"><span data-stu-id="676aa-201">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="676aa-202">keySize</span><span class="sxs-lookup"><span data-stu-id="676aa-202">keySize</span></span>|[<span data-ttu-id="676aa-203">keySize</span><span class="sxs-lookup"><span data-stu-id="676aa-203">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="676aa-204">SCEP 密钥大小。</span><span class="sxs-lookup"><span data-stu-id="676aa-204">SCEP Key Size.</span></span> <span data-ttu-id="676aa-205">可取值为：`size1024`、`size2048`。</span><span class="sxs-lookup"><span data-stu-id="676aa-205">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="676aa-206">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="676aa-206">hashAlgorithm</span></span>|[<span data-ttu-id="676aa-207">hashAlgorithms</span><span class="sxs-lookup"><span data-stu-id="676aa-207">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="676aa-208">SCEP 哈希算法。</span><span class="sxs-lookup"><span data-stu-id="676aa-208">SCEP Hash Algorithm.</span></span> <span data-ttu-id="676aa-209">可取值为：`sha1`、`sha2`。</span><span class="sxs-lookup"><span data-stu-id="676aa-209">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="676aa-210">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="676aa-210">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="676aa-211">字符串</span><span class="sxs-lookup"><span data-stu-id="676aa-211">String</span></span>|<span data-ttu-id="676aa-212">定义 AAD 属性的自定义字符串。</span><span class="sxs-lookup"><span data-stu-id="676aa-212">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="676aa-213">certificateStore</span><span class="sxs-lookup"><span data-stu-id="676aa-213">certificateStore</span></span>|[<span data-ttu-id="676aa-214">certificateStore</span><span class="sxs-lookup"><span data-stu-id="676aa-214">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="676aa-215">目标存储证书。</span><span class="sxs-lookup"><span data-stu-id="676aa-215">Target store certificate.</span></span> <span data-ttu-id="676aa-216">可取值为：`user`、`machine`。</span><span class="sxs-lookup"><span data-stu-id="676aa-216">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="676aa-217">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="676aa-217">customSubjectAlternativeNames</span></span>|<span data-ttu-id="676aa-218">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)集合</span><span class="sxs-lookup"><span data-stu-id="676aa-218">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="676aa-219">自定义主题 Alterantive 名称设置。</span><span class="sxs-lookup"><span data-stu-id="676aa-219">Custom Subject Alterantive Name Settings.</span></span> <span data-ttu-id="676aa-220">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="676aa-220">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="676aa-221">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="676aa-221">subjectAlternativeNameType</span></span>|[<span data-ttu-id="676aa-222">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="676aa-222">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="676aa-223">证书使用者替代名称类型。</span><span class="sxs-lookup"><span data-stu-id="676aa-223">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="676aa-224">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService`。</span><span class="sxs-lookup"><span data-stu-id="676aa-224">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|



## <a name="response"></a><span data-ttu-id="676aa-225">响应</span><span class="sxs-lookup"><span data-stu-id="676aa-225">Response</span></span>
<span data-ttu-id="676aa-226">如果成功，此方法返回`201 Created`响应代码和响应正文中的[androidWorkProfileScepCertificateProfile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="676aa-226">If successful, this method returns a `201 Created` response code and a [androidWorkProfileScepCertificateProfile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="676aa-227">示例</span><span class="sxs-lookup"><span data-stu-id="676aa-227">Example</span></span>
### <a name="request"></a><span data-ttu-id="676aa-228">请求</span><span class="sxs-lookup"><span data-stu-id="676aa-228">Request</span></span>
<span data-ttu-id="676aa-229">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="676aa-229">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1273

{
  "@odata.type": "#microsoft.graph.androidWorkProfileScepCertificateProfile",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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
  ],
  "subjectAlternativeNameType": "emailAddress"
}
```

### <a name="response"></a><span data-ttu-id="676aa-230">响应</span><span class="sxs-lookup"><span data-stu-id="676aa-230">Response</span></span>
<span data-ttu-id="676aa-p123">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="676aa-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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
  ],
  "subjectAlternativeNameType": "emailAddress"
}
```





