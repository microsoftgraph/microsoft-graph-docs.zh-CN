---
title: 更新 windowsPhone81ImportedPFXCertificateProfile
description: 更新 windowsPhone81ImportedPFXCertificateProfile 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4f087edba9825dd9d18d6ba965282d4c1d99b15d
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33917707"
---
# <a name="update-windowsphone81importedpfxcertificateprofile"></a><span data-ttu-id="623e7-103">更新 windowsPhone81ImportedPFXCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="623e7-103">Update windowsPhone81ImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="623e7-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="623e7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="623e7-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="623e7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="623e7-106">更新[windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="623e7-106">Update the properties of a [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="623e7-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="623e7-107">Prerequisites</span></span>
<span data-ttu-id="623e7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="623e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="623e7-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="623e7-110">Permission type</span></span>|<span data-ttu-id="623e7-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="623e7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="623e7-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="623e7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="623e7-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="623e7-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="623e7-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="623e7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="623e7-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="623e7-115">Not supported.</span></span>|
|<span data-ttu-id="623e7-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="623e7-116">Application</span></span>|<span data-ttu-id="623e7-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="623e7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="623e7-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="623e7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="623e7-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="623e7-119">Request headers</span></span>
|<span data-ttu-id="623e7-120">标头</span><span class="sxs-lookup"><span data-stu-id="623e7-120">Header</span></span>|<span data-ttu-id="623e7-121">值</span><span class="sxs-lookup"><span data-stu-id="623e7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="623e7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="623e7-122">Authorization</span></span>|<span data-ttu-id="623e7-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="623e7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="623e7-124">接受</span><span class="sxs-lookup"><span data-stu-id="623e7-124">Accept</span></span>|<span data-ttu-id="623e7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="623e7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="623e7-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="623e7-126">Request body</span></span>
<span data-ttu-id="623e7-127">在请求正文中, 提供[windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="623e7-127">In the request body, supply a JSON representation for the [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) object.</span></span>

<span data-ttu-id="623e7-128">下表显示创建[windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="623e7-128">The following table shows the properties that are required when you create the [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md).</span></span>

|<span data-ttu-id="623e7-129">属性</span><span class="sxs-lookup"><span data-stu-id="623e7-129">Property</span></span>|<span data-ttu-id="623e7-130">类型</span><span class="sxs-lookup"><span data-stu-id="623e7-130">Type</span></span>|<span data-ttu-id="623e7-131">说明</span><span class="sxs-lookup"><span data-stu-id="623e7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="623e7-132">id</span><span class="sxs-lookup"><span data-stu-id="623e7-132">id</span></span>|<span data-ttu-id="623e7-133">字符串</span><span class="sxs-lookup"><span data-stu-id="623e7-133">String</span></span>|<span data-ttu-id="623e7-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="623e7-134">Key of the entity.</span></span> <span data-ttu-id="623e7-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="623e7-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="623e7-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="623e7-136">lastModifiedDateTime</span></span>|<span data-ttu-id="623e7-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="623e7-137">DateTimeOffset</span></span>|<span data-ttu-id="623e7-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="623e7-138">DateTime the object was last modified.</span></span> <span data-ttu-id="623e7-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="623e7-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="623e7-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="623e7-140">roleScopeTagIds</span></span>|<span data-ttu-id="623e7-141">String collection</span><span class="sxs-lookup"><span data-stu-id="623e7-141">String collection</span></span>|<span data-ttu-id="623e7-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="623e7-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="623e7-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="623e7-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="623e7-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="623e7-144">supportsScopeTags</span></span>|<span data-ttu-id="623e7-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="623e7-145">Boolean</span></span>|<span data-ttu-id="623e7-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="623e7-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="623e7-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="623e7-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="623e7-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="623e7-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="623e7-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="623e7-149">This property is read-only.</span></span> <span data-ttu-id="623e7-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="623e7-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="623e7-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="623e7-151">createdDateTime</span></span>|<span data-ttu-id="623e7-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="623e7-152">DateTimeOffset</span></span>|<span data-ttu-id="623e7-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="623e7-153">DateTime the object was created.</span></span> <span data-ttu-id="623e7-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="623e7-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="623e7-155">说明</span><span class="sxs-lookup"><span data-stu-id="623e7-155">description</span></span>|<span data-ttu-id="623e7-156">String</span><span class="sxs-lookup"><span data-stu-id="623e7-156">String</span></span>|<span data-ttu-id="623e7-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="623e7-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="623e7-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="623e7-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="623e7-159">displayName</span><span class="sxs-lookup"><span data-stu-id="623e7-159">displayName</span></span>|<span data-ttu-id="623e7-160">String</span><span class="sxs-lookup"><span data-stu-id="623e7-160">String</span></span>|<span data-ttu-id="623e7-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="623e7-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="623e7-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="623e7-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="623e7-163">version</span><span class="sxs-lookup"><span data-stu-id="623e7-163">version</span></span>|<span data-ttu-id="623e7-164">Int32</span><span class="sxs-lookup"><span data-stu-id="623e7-164">Int32</span></span>|<span data-ttu-id="623e7-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="623e7-165">Version of the device configuration.</span></span> <span data-ttu-id="623e7-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="623e7-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="623e7-167">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="623e7-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="623e7-168">Int32</span><span class="sxs-lookup"><span data-stu-id="623e7-168">Int32</span></span>|<span data-ttu-id="623e7-169">证书续订阈值百分比。</span><span class="sxs-lookup"><span data-stu-id="623e7-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="623e7-170">从[WindowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)继承的有效值1到99</span><span class="sxs-lookup"><span data-stu-id="623e7-170">Valid values 1 to 99 Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="623e7-171">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="623e7-171">keyStorageProvider</span></span>|[<span data-ttu-id="623e7-172">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="623e7-172">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="623e7-173">从[WindowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)继承的密钥存储提供程序 (KSP)。</span><span class="sxs-lookup"><span data-stu-id="623e7-173">Key Storage Provider (KSP) Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="623e7-174">可取值为：`useTpmKspOtherwiseUseSoftwareKsp`、`useTpmKspOtherwiseFail`、`usePassportForWorkKspOtherwiseFail`、`useSoftwareKsp`。</span><span class="sxs-lookup"><span data-stu-id="623e7-174">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="623e7-175">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="623e7-175">subjectNameFormat</span></span>|[<span data-ttu-id="623e7-176">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="623e7-176">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="623e7-177">证书使用者名称格式继承自[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="623e7-177">Certificate Subject Name Format Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="623e7-178">可取值为：`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId`。</span><span class="sxs-lookup"><span data-stu-id="623e7-178">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="623e7-179">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="623e7-179">subjectAlternativeNameType</span></span>|[<span data-ttu-id="623e7-180">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="623e7-180">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="623e7-181">证书使用者备用名称类型继承自[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="623e7-181">Certificate Subject Alternative Name Type Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="623e7-182">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService`。</span><span class="sxs-lookup"><span data-stu-id="623e7-182">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="623e7-183">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="623e7-183">certificateValidityPeriodValue</span></span>|<span data-ttu-id="623e7-184">Int32</span><span class="sxs-lookup"><span data-stu-id="623e7-184">Int32</span></span>|<span data-ttu-id="623e7-185">继承自[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)的证书有效期限的值</span><span class="sxs-lookup"><span data-stu-id="623e7-185">Value for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="623e7-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="623e7-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="623e7-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="623e7-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="623e7-188">从[WindowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)继承的证书有效期限的小数位数。</span><span class="sxs-lookup"><span data-stu-id="623e7-188">Scale for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="623e7-189">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="623e7-189">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="623e7-190">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="623e7-190">intendedPurpose</span></span>|[<span data-ttu-id="623e7-191">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="623e7-191">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="623e7-192">尚未记录。</span><span class="sxs-lookup"><span data-stu-id="623e7-192">Not yet documented.</span></span> <span data-ttu-id="623e7-193">可取值为：`unassigned`、`smimeEncryption`、`smimeSigning`、`vpn`、`wifi`。</span><span class="sxs-lookup"><span data-stu-id="623e7-193">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="623e7-194">响应</span><span class="sxs-lookup"><span data-stu-id="623e7-194">Response</span></span>
<span data-ttu-id="623e7-195">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="623e7-195">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="623e7-196">示例</span><span class="sxs-lookup"><span data-stu-id="623e7-196">Example</span></span>

### <a name="request"></a><span data-ttu-id="623e7-197">请求</span><span class="sxs-lookup"><span data-stu-id="623e7-197">Request</span></span>
<span data-ttu-id="623e7-198">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="623e7-198">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 591

{
  "@odata.type": "#microsoft.graph.windowsPhone81ImportedPFXCertificateProfile",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "renewalThresholdPercentage": 10,
  "keyStorageProvider": "useTpmKspOtherwiseFail",
  "subjectNameFormat": "commonNameIncludingEmail",
  "subjectAlternativeNameType": "emailAddress",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "intendedPurpose": "smimeEncryption"
}
```

### <a name="response"></a><span data-ttu-id="623e7-199">响应</span><span class="sxs-lookup"><span data-stu-id="623e7-199">Response</span></span>
<span data-ttu-id="623e7-p116">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="623e7-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 763

{
  "@odata.type": "#microsoft.graph.windowsPhone81ImportedPFXCertificateProfile",
  "id": "08c7f847-f847-08c7-47f8-c70847f8c708",
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
  "keyStorageProvider": "useTpmKspOtherwiseFail",
  "subjectNameFormat": "commonNameIncludingEmail",
  "subjectAlternativeNameType": "emailAddress",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "intendedPurpose": "smimeEncryption"
}
```




