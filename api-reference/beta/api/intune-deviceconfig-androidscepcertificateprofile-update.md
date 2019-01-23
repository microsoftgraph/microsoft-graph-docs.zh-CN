---
title: 更新 androidScepCertificateProfile
description: 更新 androidScepCertificateProfile 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b68cd2c1c5a4e55408e0aee6f7797ae08f52a88c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424110"
---
# <a name="update-androidscepcertificateprofile"></a><span data-ttu-id="30fb6-103">更新 androidScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="30fb6-103">Update androidScepCertificateProfile</span></span>

> <span data-ttu-id="30fb6-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="30fb6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="30fb6-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="30fb6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="30fb6-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="30fb6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="30fb6-107">更新[androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="30fb6-107">Update the properties of a [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="30fb6-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="30fb6-108">Prerequisites</span></span>
<span data-ttu-id="30fb6-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="30fb6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="30fb6-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="30fb6-111">Permission type</span></span>|<span data-ttu-id="30fb6-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="30fb6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="30fb6-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="30fb6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="30fb6-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30fb6-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="30fb6-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="30fb6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="30fb6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="30fb6-116">Not supported.</span></span>|
|<span data-ttu-id="30fb6-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="30fb6-117">Application</span></span>|<span data-ttu-id="30fb6-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="30fb6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="30fb6-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="30fb6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="30fb6-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="30fb6-120">Request headers</span></span>
|<span data-ttu-id="30fb6-121">标头</span><span class="sxs-lookup"><span data-stu-id="30fb6-121">Header</span></span>|<span data-ttu-id="30fb6-122">值</span><span class="sxs-lookup"><span data-stu-id="30fb6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="30fb6-123">授权</span><span class="sxs-lookup"><span data-stu-id="30fb6-123">Authorization</span></span>|<span data-ttu-id="30fb6-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="30fb6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="30fb6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="30fb6-125">Accept</span></span>|<span data-ttu-id="30fb6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="30fb6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="30fb6-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="30fb6-127">Request body</span></span>
<span data-ttu-id="30fb6-128">在请求正文中，提供[androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="30fb6-128">In the request body, supply a JSON representation for the [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) object.</span></span>

<span data-ttu-id="30fb6-129">下表显示时创建[androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="30fb6-129">The following table shows the properties that are required when you create the [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md).</span></span>

|<span data-ttu-id="30fb6-130">属性</span><span class="sxs-lookup"><span data-stu-id="30fb6-130">Property</span></span>|<span data-ttu-id="30fb6-131">类型</span><span class="sxs-lookup"><span data-stu-id="30fb6-131">Type</span></span>|<span data-ttu-id="30fb6-132">说明</span><span class="sxs-lookup"><span data-stu-id="30fb6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="30fb6-133">id</span><span class="sxs-lookup"><span data-stu-id="30fb6-133">id</span></span>|<span data-ttu-id="30fb6-134">String</span><span class="sxs-lookup"><span data-stu-id="30fb6-134">String</span></span>|<span data-ttu-id="30fb6-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="30fb6-135">Key of the entity.</span></span> <span data-ttu-id="30fb6-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="30fb6-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="30fb6-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="30fb6-137">lastModifiedDateTime</span></span>|<span data-ttu-id="30fb6-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="30fb6-138">DateTimeOffset</span></span>|<span data-ttu-id="30fb6-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="30fb6-139">DateTime the object was last modified.</span></span> <span data-ttu-id="30fb6-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="30fb6-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="30fb6-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="30fb6-141">roleScopeTagIds</span></span>|<span data-ttu-id="30fb6-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="30fb6-142">String collection</span></span>|<span data-ttu-id="30fb6-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="30fb6-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="30fb6-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="30fb6-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="30fb6-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="30fb6-145">supportsScopeTags</span></span>|<span data-ttu-id="30fb6-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="30fb6-146">Boolean</span></span>|<span data-ttu-id="30fb6-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="30fb6-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="30fb6-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="30fb6-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="30fb6-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="30fb6-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="30fb6-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="30fb6-150">This property is read-only.</span></span> <span data-ttu-id="30fb6-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="30fb6-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="30fb6-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="30fb6-152">createdDateTime</span></span>|<span data-ttu-id="30fb6-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="30fb6-153">DateTimeOffset</span></span>|<span data-ttu-id="30fb6-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="30fb6-154">DateTime the object was created.</span></span> <span data-ttu-id="30fb6-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="30fb6-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="30fb6-156">description</span><span class="sxs-lookup"><span data-stu-id="30fb6-156">description</span></span>|<span data-ttu-id="30fb6-157">String</span><span class="sxs-lookup"><span data-stu-id="30fb6-157">String</span></span>|<span data-ttu-id="30fb6-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="30fb6-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="30fb6-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="30fb6-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="30fb6-160">displayName</span><span class="sxs-lookup"><span data-stu-id="30fb6-160">displayName</span></span>|<span data-ttu-id="30fb6-161">String</span><span class="sxs-lookup"><span data-stu-id="30fb6-161">String</span></span>|<span data-ttu-id="30fb6-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="30fb6-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="30fb6-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="30fb6-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="30fb6-164">version</span><span class="sxs-lookup"><span data-stu-id="30fb6-164">version</span></span>|<span data-ttu-id="30fb6-165">Int32</span><span class="sxs-lookup"><span data-stu-id="30fb6-165">Int32</span></span>|<span data-ttu-id="30fb6-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="30fb6-166">Version of the device configuration.</span></span> <span data-ttu-id="30fb6-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="30fb6-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="30fb6-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="30fb6-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="30fb6-169">Int32</span><span class="sxs-lookup"><span data-stu-id="30fb6-169">Int32</span></span>|<span data-ttu-id="30fb6-170">证书续订阈值百分比。</span><span class="sxs-lookup"><span data-stu-id="30fb6-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="30fb6-171">有效值 1 到 99 继承自[androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="30fb6-171">Valid values 1 to 99 Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="30fb6-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="30fb6-172">subjectNameFormat</span></span>|[<span data-ttu-id="30fb6-173">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="30fb6-173">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="30fb6-174">证书使用者名称格式。</span><span class="sxs-lookup"><span data-stu-id="30fb6-174">Certificate Subject Name Format.</span></span> <span data-ttu-id="30fb6-175">继承自[androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="30fb6-175">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="30fb6-176">可取值为：`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId`。</span><span class="sxs-lookup"><span data-stu-id="30fb6-176">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="30fb6-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="30fb6-177">subjectAlternativeNameType</span></span>|[<span data-ttu-id="30fb6-178">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="30fb6-178">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="30fb6-179">证书使用者替代名称类型。</span><span class="sxs-lookup"><span data-stu-id="30fb6-179">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="30fb6-180">继承自[androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="30fb6-180">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="30fb6-181">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService`。</span><span class="sxs-lookup"><span data-stu-id="30fb6-181">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="30fb6-182">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="30fb6-182">certificateValidityPeriodValue</span></span>|<span data-ttu-id="30fb6-183">Int32</span><span class="sxs-lookup"><span data-stu-id="30fb6-183">Int32</span></span>|<span data-ttu-id="30fb6-184">证书有效期限的值。</span><span class="sxs-lookup"><span data-stu-id="30fb6-184">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="30fb6-185">继承自[androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="30fb6-185">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="30fb6-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="30fb6-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="30fb6-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="30fb6-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="30fb6-188">证书有效期限的小数位数。</span><span class="sxs-lookup"><span data-stu-id="30fb6-188">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="30fb6-189">继承自[androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="30fb6-189">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="30fb6-190">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="30fb6-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="30fb6-191">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="30fb6-191">extendedKeyUsages</span></span>|<span data-ttu-id="30fb6-192">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)集合</span><span class="sxs-lookup"><span data-stu-id="30fb6-192">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="30fb6-193">扩展的密钥用法 (EKU) 设置。</span><span class="sxs-lookup"><span data-stu-id="30fb6-193">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="30fb6-194">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="30fb6-194">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="30fb6-195">继承自[androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="30fb6-195">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="30fb6-196">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="30fb6-196">scepServerUrls</span></span>|<span data-ttu-id="30fb6-197">String 集合</span><span class="sxs-lookup"><span data-stu-id="30fb6-197">String collection</span></span>|<span data-ttu-id="30fb6-198">SCEP 服务器 Url(s)</span><span class="sxs-lookup"><span data-stu-id="30fb6-198">SCEP Server Url(s)</span></span>|
|<span data-ttu-id="30fb6-199">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="30fb6-199">subjectNameFormatString</span></span>|<span data-ttu-id="30fb6-200">String</span><span class="sxs-lookup"><span data-stu-id="30fb6-200">String</span></span>|<span data-ttu-id="30fb6-201">自定义格式使用 SubjectNameFormat = 自定义。</span><span class="sxs-lookup"><span data-stu-id="30fb6-201">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="30fb6-202">示例： CN = {{EmailAddress}} E = {{EmailAddress}}，OU = 企业用户，O = Contoso Corporation L = 雷德蒙德，ST = WA，C = US</span><span class="sxs-lookup"><span data-stu-id="30fb6-202">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="30fb6-203">keyUsage</span><span class="sxs-lookup"><span data-stu-id="30fb6-203">keyUsage</span></span>|[<span data-ttu-id="30fb6-204">keyUsages</span><span class="sxs-lookup"><span data-stu-id="30fb6-204">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="30fb6-205">SCEP 密钥用法。</span><span class="sxs-lookup"><span data-stu-id="30fb6-205">SCEP Key Usage.</span></span> <span data-ttu-id="30fb6-206">可取值为：`keyEncipherment`、`digitalSignature`。</span><span class="sxs-lookup"><span data-stu-id="30fb6-206">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="30fb6-207">keySize</span><span class="sxs-lookup"><span data-stu-id="30fb6-207">keySize</span></span>|[<span data-ttu-id="30fb6-208">keySize</span><span class="sxs-lookup"><span data-stu-id="30fb6-208">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="30fb6-209">SCEP 密钥大小。</span><span class="sxs-lookup"><span data-stu-id="30fb6-209">SCEP Key Size.</span></span> <span data-ttu-id="30fb6-210">可取值为：`size1024`、`size2048`。</span><span class="sxs-lookup"><span data-stu-id="30fb6-210">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="30fb6-211">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="30fb6-211">hashAlgorithm</span></span>|[<span data-ttu-id="30fb6-212">hashAlgorithms</span><span class="sxs-lookup"><span data-stu-id="30fb6-212">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="30fb6-213">SCEP 哈希算法。</span><span class="sxs-lookup"><span data-stu-id="30fb6-213">SCEP Hash Algorithm.</span></span> <span data-ttu-id="30fb6-214">可取值为：`sha1`、`sha2`。</span><span class="sxs-lookup"><span data-stu-id="30fb6-214">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="30fb6-215">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="30fb6-215">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="30fb6-216">String</span><span class="sxs-lookup"><span data-stu-id="30fb6-216">String</span></span>|<span data-ttu-id="30fb6-217">定义 AAD 属性的自定义字符串。</span><span class="sxs-lookup"><span data-stu-id="30fb6-217">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="30fb6-218">响应</span><span class="sxs-lookup"><span data-stu-id="30fb6-218">Response</span></span>
<span data-ttu-id="30fb6-219">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="30fb6-219">If successful, this method returns a `200 OK` response code and an updated [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="30fb6-220">示例</span><span class="sxs-lookup"><span data-stu-id="30fb6-220">Example</span></span>

### <a name="request"></a><span data-ttu-id="30fb6-221">请求</span><span class="sxs-lookup"><span data-stu-id="30fb6-221">Request</span></span>
<span data-ttu-id="30fb6-222">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="30fb6-222">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 974

{
  "@odata.type": "#microsoft.graph.androidScepCertificateProfile",
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
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```

### <a name="response"></a><span data-ttu-id="30fb6-223">响应</span><span class="sxs-lookup"><span data-stu-id="30fb6-223">Response</span></span>
<span data-ttu-id="30fb6-p121">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="30fb6-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1146

{
  "@odata.type": "#microsoft.graph.androidScepCertificateProfile",
  "id": "e9a0dbbd-dbbd-e9a0-bddb-a0e9bddba0e9",
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
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```




