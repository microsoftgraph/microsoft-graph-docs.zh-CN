---
title: 更新 androidWorkProfileScepCertificateProfile
description: 更新 androidWorkProfileScepCertificateProfile 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e0c65ebfe6f2ba4b3b4f55f0a7f0e2e8fc5ec960
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817575"
---
# <a name="update-androidworkprofilescepcertificateprofile"></a><span data-ttu-id="b18b1-103">更新 androidWorkProfileScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="b18b1-103">Update androidWorkProfileScepCertificateProfile</span></span>

> <span data-ttu-id="b18b1-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b18b1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b18b1-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b18b1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b18b1-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b18b1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b18b1-107">更新[androidWorkProfileScepCertificateProfile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b18b1-107">Update the properties of a [androidWorkProfileScepCertificateProfile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b18b1-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b18b1-108">Prerequisites</span></span>
<span data-ttu-id="b18b1-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="b18b1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b18b1-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b18b1-111">Permission type</span></span>|<span data-ttu-id="b18b1-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b18b1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b18b1-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b18b1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b18b1-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b18b1-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b18b1-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b18b1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b18b1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b18b1-116">Not supported.</span></span>|
|<span data-ttu-id="b18b1-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b18b1-117">Application</span></span>|<span data-ttu-id="b18b1-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="b18b1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b18b1-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b18b1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="b18b1-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b18b1-120">Request headers</span></span>
|<span data-ttu-id="b18b1-121">标头</span><span class="sxs-lookup"><span data-stu-id="b18b1-121">Header</span></span>|<span data-ttu-id="b18b1-122">值</span><span class="sxs-lookup"><span data-stu-id="b18b1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b18b1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b18b1-123">Authorization</span></span>|<span data-ttu-id="b18b1-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b18b1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b18b1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b18b1-125">Accept</span></span>|<span data-ttu-id="b18b1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b18b1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b18b1-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b18b1-127">Request body</span></span>
<span data-ttu-id="b18b1-128">在请求正文中，提供[androidWorkProfileScepCertificateProfile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b18b1-128">In the request body, supply a JSON representation for the [androidWorkProfileScepCertificateProfile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md) object.</span></span>

<span data-ttu-id="b18b1-129">下表显示时创建[androidWorkProfileScepCertificateProfile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b18b1-129">The following table shows the properties that are required when you create the [androidWorkProfileScepCertificateProfile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md).</span></span>

|<span data-ttu-id="b18b1-130">属性</span><span class="sxs-lookup"><span data-stu-id="b18b1-130">Property</span></span>|<span data-ttu-id="b18b1-131">类型</span><span class="sxs-lookup"><span data-stu-id="b18b1-131">Type</span></span>|<span data-ttu-id="b18b1-132">说明</span><span class="sxs-lookup"><span data-stu-id="b18b1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b18b1-133">id</span><span class="sxs-lookup"><span data-stu-id="b18b1-133">id</span></span>|<span data-ttu-id="b18b1-134">String</span><span class="sxs-lookup"><span data-stu-id="b18b1-134">String</span></span>|<span data-ttu-id="b18b1-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b18b1-135">Key of the entity.</span></span> <span data-ttu-id="b18b1-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b18b1-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b18b1-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b18b1-137">lastModifiedDateTime</span></span>|<span data-ttu-id="b18b1-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b18b1-138">DateTimeOffset</span></span>|<span data-ttu-id="b18b1-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b18b1-139">DateTime the object was last modified.</span></span> <span data-ttu-id="b18b1-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b18b1-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b18b1-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b18b1-141">roleScopeTagIds</span></span>|<span data-ttu-id="b18b1-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="b18b1-142">String collection</span></span>|<span data-ttu-id="b18b1-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="b18b1-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b18b1-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b18b1-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b18b1-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b18b1-145">supportsScopeTags</span></span>|<span data-ttu-id="b18b1-146">布尔</span><span class="sxs-lookup"><span data-stu-id="b18b1-146">Boolean</span></span>|<span data-ttu-id="b18b1-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="b18b1-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b18b1-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="b18b1-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b18b1-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="b18b1-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b18b1-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="b18b1-150">This property is read-only.</span></span> <span data-ttu-id="b18b1-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b18b1-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b18b1-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b18b1-152">createdDateTime</span></span>|<span data-ttu-id="b18b1-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b18b1-153">DateTimeOffset</span></span>|<span data-ttu-id="b18b1-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b18b1-154">DateTime the object was created.</span></span> <span data-ttu-id="b18b1-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b18b1-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b18b1-156">description</span><span class="sxs-lookup"><span data-stu-id="b18b1-156">description</span></span>|<span data-ttu-id="b18b1-157">String</span><span class="sxs-lookup"><span data-stu-id="b18b1-157">String</span></span>|<span data-ttu-id="b18b1-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="b18b1-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b18b1-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b18b1-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b18b1-160">displayName</span><span class="sxs-lookup"><span data-stu-id="b18b1-160">displayName</span></span>|<span data-ttu-id="b18b1-161">String</span><span class="sxs-lookup"><span data-stu-id="b18b1-161">String</span></span>|<span data-ttu-id="b18b1-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="b18b1-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b18b1-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b18b1-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b18b1-164">version</span><span class="sxs-lookup"><span data-stu-id="b18b1-164">version</span></span>|<span data-ttu-id="b18b1-165">Int32</span><span class="sxs-lookup"><span data-stu-id="b18b1-165">Int32</span></span>|<span data-ttu-id="b18b1-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="b18b1-166">Version of the device configuration.</span></span> <span data-ttu-id="b18b1-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b18b1-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b18b1-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="b18b1-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="b18b1-169">Int32</span><span class="sxs-lookup"><span data-stu-id="b18b1-169">Int32</span></span>|<span data-ttu-id="b18b1-170">证书续订阈值百分比。</span><span class="sxs-lookup"><span data-stu-id="b18b1-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="b18b1-171">有效值 1 到 99 继承自[androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="b18b1-171">Valid values 1 to 99 Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="b18b1-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="b18b1-172">subjectNameFormat</span></span>|[<span data-ttu-id="b18b1-173">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="b18b1-173">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="b18b1-174">证书使用者名称格式。</span><span class="sxs-lookup"><span data-stu-id="b18b1-174">Certificate Subject Name Format.</span></span> <span data-ttu-id="b18b1-175">继承自[androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="b18b1-175">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="b18b1-176">可取值为：`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId`。</span><span class="sxs-lookup"><span data-stu-id="b18b1-176">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="b18b1-177">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="b18b1-177">certificateValidityPeriodValue</span></span>|<span data-ttu-id="b18b1-178">Int32</span><span class="sxs-lookup"><span data-stu-id="b18b1-178">Int32</span></span>|<span data-ttu-id="b18b1-179">证书有效期限的值。</span><span class="sxs-lookup"><span data-stu-id="b18b1-179">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="b18b1-180">继承自[androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="b18b1-180">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="b18b1-181">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="b18b1-181">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="b18b1-182">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="b18b1-182">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="b18b1-183">证书有效期限的小数位数。</span><span class="sxs-lookup"><span data-stu-id="b18b1-183">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="b18b1-184">继承自[androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="b18b1-184">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="b18b1-185">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="b18b1-185">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="b18b1-186">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="b18b1-186">extendedKeyUsages</span></span>|<span data-ttu-id="b18b1-187">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)集合</span><span class="sxs-lookup"><span data-stu-id="b18b1-187">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="b18b1-188">扩展的密钥用法 (EKU) 设置。</span><span class="sxs-lookup"><span data-stu-id="b18b1-188">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="b18b1-189">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="b18b1-189">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="b18b1-190">继承自[androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="b18b1-190">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="b18b1-191">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="b18b1-191">scepServerUrls</span></span>|<span data-ttu-id="b18b1-192">String 集合</span><span class="sxs-lookup"><span data-stu-id="b18b1-192">String collection</span></span>|<span data-ttu-id="b18b1-193">SCEP 服务器 Url(s)</span><span class="sxs-lookup"><span data-stu-id="b18b1-193">SCEP Server Url(s)</span></span>|
|<span data-ttu-id="b18b1-194">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="b18b1-194">subjectNameFormatString</span></span>|<span data-ttu-id="b18b1-195">字符串</span><span class="sxs-lookup"><span data-stu-id="b18b1-195">String</span></span>|<span data-ttu-id="b18b1-196">自定义格式使用 SubjectNameFormat = 自定义。</span><span class="sxs-lookup"><span data-stu-id="b18b1-196">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="b18b1-197">示例： CN = {{EmailAddress}} E = {{EmailAddress}}，OU = 企业用户，O = Contoso Corporation L = 雷德蒙德，ST = WA，C = US</span><span class="sxs-lookup"><span data-stu-id="b18b1-197">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="b18b1-198">keyUsage</span><span class="sxs-lookup"><span data-stu-id="b18b1-198">keyUsage</span></span>|[<span data-ttu-id="b18b1-199">keyUsages</span><span class="sxs-lookup"><span data-stu-id="b18b1-199">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="b18b1-200">SCEP 密钥用法。</span><span class="sxs-lookup"><span data-stu-id="b18b1-200">SCEP Key Usage.</span></span> <span data-ttu-id="b18b1-201">可取值为：`keyEncipherment`、`digitalSignature`。</span><span class="sxs-lookup"><span data-stu-id="b18b1-201">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="b18b1-202">keySize</span><span class="sxs-lookup"><span data-stu-id="b18b1-202">keySize</span></span>|[<span data-ttu-id="b18b1-203">keySize</span><span class="sxs-lookup"><span data-stu-id="b18b1-203">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="b18b1-204">SCEP 密钥大小。</span><span class="sxs-lookup"><span data-stu-id="b18b1-204">SCEP Key Size.</span></span> <span data-ttu-id="b18b1-205">可取值为：`size1024`、`size2048`。</span><span class="sxs-lookup"><span data-stu-id="b18b1-205">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="b18b1-206">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="b18b1-206">hashAlgorithm</span></span>|[<span data-ttu-id="b18b1-207">hashAlgorithms</span><span class="sxs-lookup"><span data-stu-id="b18b1-207">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="b18b1-208">SCEP 哈希算法。</span><span class="sxs-lookup"><span data-stu-id="b18b1-208">SCEP Hash Algorithm.</span></span> <span data-ttu-id="b18b1-209">可取值为：`sha1`、`sha2`。</span><span class="sxs-lookup"><span data-stu-id="b18b1-209">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="b18b1-210">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="b18b1-210">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="b18b1-211">字符串</span><span class="sxs-lookup"><span data-stu-id="b18b1-211">String</span></span>|<span data-ttu-id="b18b1-212">定义 AAD 属性的自定义字符串。</span><span class="sxs-lookup"><span data-stu-id="b18b1-212">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="b18b1-213">certificateStore</span><span class="sxs-lookup"><span data-stu-id="b18b1-213">certificateStore</span></span>|[<span data-ttu-id="b18b1-214">certificateStore</span><span class="sxs-lookup"><span data-stu-id="b18b1-214">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="b18b1-215">目标存储证书。</span><span class="sxs-lookup"><span data-stu-id="b18b1-215">Target store certificate.</span></span> <span data-ttu-id="b18b1-216">可取值为：`user`、`machine`。</span><span class="sxs-lookup"><span data-stu-id="b18b1-216">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="b18b1-217">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="b18b1-217">customSubjectAlternativeNames</span></span>|<span data-ttu-id="b18b1-218">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)集合</span><span class="sxs-lookup"><span data-stu-id="b18b1-218">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="b18b1-219">自定义主题 Alterantive 名称设置。</span><span class="sxs-lookup"><span data-stu-id="b18b1-219">Custom Subject Alterantive Name Settings.</span></span> <span data-ttu-id="b18b1-220">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="b18b1-220">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="b18b1-221">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="b18b1-221">subjectAlternativeNameType</span></span>|[<span data-ttu-id="b18b1-222">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="b18b1-222">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="b18b1-223">证书使用者替代名称类型。</span><span class="sxs-lookup"><span data-stu-id="b18b1-223">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="b18b1-224">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService`。</span><span class="sxs-lookup"><span data-stu-id="b18b1-224">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|



## <a name="response"></a><span data-ttu-id="b18b1-225">响应</span><span class="sxs-lookup"><span data-stu-id="b18b1-225">Response</span></span>
<span data-ttu-id="b18b1-226">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[androidWorkProfileScepCertificateProfile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b18b1-226">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileScepCertificateProfile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b18b1-227">示例</span><span class="sxs-lookup"><span data-stu-id="b18b1-227">Example</span></span>
### <a name="request"></a><span data-ttu-id="b18b1-228">请求</span><span class="sxs-lookup"><span data-stu-id="b18b1-228">Request</span></span>
<span data-ttu-id="b18b1-229">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b18b1-229">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1194

{
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

### <a name="response"></a><span data-ttu-id="b18b1-230">响应</span><span class="sxs-lookup"><span data-stu-id="b18b1-230">Response</span></span>
<span data-ttu-id="b18b1-p123">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b18b1-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





