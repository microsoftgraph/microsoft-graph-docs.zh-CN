---
title: 更新 androidImportedPFXCertificateProfile
description: 更新 androidImportedPFXCertificateProfile 对象的属性。
author: tfitzmac
ms.openlocfilehash: f8f4f78dbefaa3ed2b9e945d2d5eece5046a5bba
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27352533"
---
# <a name="update-androidimportedpfxcertificateprofile"></a><span data-ttu-id="d56bb-103">更新 androidImportedPFXCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="d56bb-103">Update androidImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="d56bb-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d56bb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d56bb-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d56bb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d56bb-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d56bb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d56bb-107">更新[androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d56bb-107">Update the properties of a [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d56bb-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="d56bb-108">Prerequisites</span></span>
<span data-ttu-id="d56bb-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="d56bb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d56bb-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d56bb-111">Permission type</span></span>|<span data-ttu-id="d56bb-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d56bb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d56bb-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d56bb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d56bb-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d56bb-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d56bb-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d56bb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d56bb-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d56bb-116">Not supported.</span></span>|
|<span data-ttu-id="d56bb-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d56bb-117">Application</span></span>|<span data-ttu-id="d56bb-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="d56bb-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d56bb-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d56bb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="d56bb-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d56bb-120">Request headers</span></span>
|<span data-ttu-id="d56bb-121">标头</span><span class="sxs-lookup"><span data-stu-id="d56bb-121">Header</span></span>|<span data-ttu-id="d56bb-122">值</span><span class="sxs-lookup"><span data-stu-id="d56bb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d56bb-123">授权</span><span class="sxs-lookup"><span data-stu-id="d56bb-123">Authorization</span></span>|<span data-ttu-id="d56bb-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d56bb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d56bb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d56bb-125">Accept</span></span>|<span data-ttu-id="d56bb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d56bb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d56bb-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d56bb-127">Request body</span></span>
<span data-ttu-id="d56bb-128">在请求正文中，提供[androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d56bb-128">In the request body, supply a JSON representation for the [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) object.</span></span>

<span data-ttu-id="d56bb-129">下表显示时创建[androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d56bb-129">The following table shows the properties that are required when you create the [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md).</span></span>

|<span data-ttu-id="d56bb-130">属性</span><span class="sxs-lookup"><span data-stu-id="d56bb-130">Property</span></span>|<span data-ttu-id="d56bb-131">类型</span><span class="sxs-lookup"><span data-stu-id="d56bb-131">Type</span></span>|<span data-ttu-id="d56bb-132">说明</span><span class="sxs-lookup"><span data-stu-id="d56bb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d56bb-133">id</span><span class="sxs-lookup"><span data-stu-id="d56bb-133">id</span></span>|<span data-ttu-id="d56bb-134">String</span><span class="sxs-lookup"><span data-stu-id="d56bb-134">String</span></span>|<span data-ttu-id="d56bb-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d56bb-135">Key of the entity.</span></span> <span data-ttu-id="d56bb-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d56bb-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d56bb-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d56bb-137">lastModifiedDateTime</span></span>|<span data-ttu-id="d56bb-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d56bb-138">DateTimeOffset</span></span>|<span data-ttu-id="d56bb-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="d56bb-139">DateTime the object was last modified.</span></span> <span data-ttu-id="d56bb-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d56bb-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d56bb-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d56bb-141">roleScopeTagIds</span></span>|<span data-ttu-id="d56bb-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="d56bb-142">String collection</span></span>|<span data-ttu-id="d56bb-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="d56bb-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d56bb-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d56bb-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d56bb-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d56bb-145">supportsScopeTags</span></span>|<span data-ttu-id="d56bb-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="d56bb-146">Boolean</span></span>|<span data-ttu-id="d56bb-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="d56bb-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d56bb-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="d56bb-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d56bb-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="d56bb-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d56bb-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="d56bb-150">This property is read-only.</span></span> <span data-ttu-id="d56bb-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d56bb-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d56bb-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d56bb-152">createdDateTime</span></span>|<span data-ttu-id="d56bb-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d56bb-153">DateTimeOffset</span></span>|<span data-ttu-id="d56bb-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="d56bb-154">DateTime the object was created.</span></span> <span data-ttu-id="d56bb-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d56bb-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d56bb-156">description</span><span class="sxs-lookup"><span data-stu-id="d56bb-156">description</span></span>|<span data-ttu-id="d56bb-157">String</span><span class="sxs-lookup"><span data-stu-id="d56bb-157">String</span></span>|<span data-ttu-id="d56bb-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="d56bb-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d56bb-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d56bb-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d56bb-160">displayName</span><span class="sxs-lookup"><span data-stu-id="d56bb-160">displayName</span></span>|<span data-ttu-id="d56bb-161">String</span><span class="sxs-lookup"><span data-stu-id="d56bb-161">String</span></span>|<span data-ttu-id="d56bb-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="d56bb-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d56bb-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d56bb-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d56bb-164">version</span><span class="sxs-lookup"><span data-stu-id="d56bb-164">version</span></span>|<span data-ttu-id="d56bb-165">Int32</span><span class="sxs-lookup"><span data-stu-id="d56bb-165">Int32</span></span>|<span data-ttu-id="d56bb-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="d56bb-166">Version of the device configuration.</span></span> <span data-ttu-id="d56bb-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d56bb-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d56bb-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="d56bb-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="d56bb-169">Int32</span><span class="sxs-lookup"><span data-stu-id="d56bb-169">Int32</span></span>|<span data-ttu-id="d56bb-170">证书续订阈值百分比。</span><span class="sxs-lookup"><span data-stu-id="d56bb-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="d56bb-171">有效值 1 到 99 继承自[androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="d56bb-171">Valid values 1 to 99 Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="d56bb-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="d56bb-172">subjectNameFormat</span></span>|[<span data-ttu-id="d56bb-173">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="d56bb-173">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="d56bb-174">证书使用者名称格式。</span><span class="sxs-lookup"><span data-stu-id="d56bb-174">Certificate Subject Name Format.</span></span> <span data-ttu-id="d56bb-175">继承自[androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="d56bb-175">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="d56bb-176">可取值为：`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId`。</span><span class="sxs-lookup"><span data-stu-id="d56bb-176">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="d56bb-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="d56bb-177">subjectAlternativeNameType</span></span>|[<span data-ttu-id="d56bb-178">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="d56bb-178">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="d56bb-179">证书使用者替代名称类型。</span><span class="sxs-lookup"><span data-stu-id="d56bb-179">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="d56bb-180">继承自[androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="d56bb-180">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="d56bb-181">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService`。</span><span class="sxs-lookup"><span data-stu-id="d56bb-181">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="d56bb-182">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="d56bb-182">certificateValidityPeriodValue</span></span>|<span data-ttu-id="d56bb-183">Int32</span><span class="sxs-lookup"><span data-stu-id="d56bb-183">Int32</span></span>|<span data-ttu-id="d56bb-184">证书有效期限的值。</span><span class="sxs-lookup"><span data-stu-id="d56bb-184">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="d56bb-185">继承自[androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="d56bb-185">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="d56bb-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="d56bb-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="d56bb-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="d56bb-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="d56bb-188">证书有效期限的小数位数。</span><span class="sxs-lookup"><span data-stu-id="d56bb-188">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="d56bb-189">继承自[androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="d56bb-189">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="d56bb-190">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="d56bb-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="d56bb-191">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="d56bb-191">extendedKeyUsages</span></span>|<span data-ttu-id="d56bb-192">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)集合</span><span class="sxs-lookup"><span data-stu-id="d56bb-192">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="d56bb-193">扩展的密钥用法 (EKU) 设置。</span><span class="sxs-lookup"><span data-stu-id="d56bb-193">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="d56bb-194">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="d56bb-194">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="d56bb-195">继承自[androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="d56bb-195">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="d56bb-196">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="d56bb-196">intendedPurpose</span></span>|[<span data-ttu-id="d56bb-197">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="d56bb-197">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="d56bb-198">尚未编档。</span><span class="sxs-lookup"><span data-stu-id="d56bb-198">Not yet documented.</span></span> <span data-ttu-id="d56bb-199">可取值为：`unassigned`、`smimeEncryption`、`smimeSigning`、`vpn`、`wifi`。</span><span class="sxs-lookup"><span data-stu-id="d56bb-199">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="d56bb-200">响应</span><span class="sxs-lookup"><span data-stu-id="d56bb-200">Response</span></span>
<span data-ttu-id="d56bb-201">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d56bb-201">If successful, this method returns a `200 OK` response code and an updated [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d56bb-202">示例</span><span class="sxs-lookup"><span data-stu-id="d56bb-202">Example</span></span>
### <a name="request"></a><span data-ttu-id="d56bb-203">请求</span><span class="sxs-lookup"><span data-stu-id="d56bb-203">Request</span></span>
<span data-ttu-id="d56bb-204">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d56bb-204">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 708

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
  "intendedPurpose": "smimeEncryption"
}
```

### <a name="response"></a><span data-ttu-id="d56bb-205">响应</span><span class="sxs-lookup"><span data-stu-id="d56bb-205">Response</span></span>
<span data-ttu-id="d56bb-p118">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d56bb-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 891

{
  "@odata.type": "#microsoft.graph.androidImportedPFXCertificateProfile",
  "id": "1cd3b0a6-b0a6-1cd3-a6b0-d31ca6b0d31c",
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
  "intendedPurpose": "smimeEncryption"
}
```





