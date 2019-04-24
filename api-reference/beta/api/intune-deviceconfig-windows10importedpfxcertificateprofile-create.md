---
title: 创建 windows10ImportedPFXCertificateProfile
description: 创建新的 windows10ImportedPFXCertificateProfile 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0ae2fa6642c8e4278be33995892c4946df48ead5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32516796"
---
# <a name="create-windows10importedpfxcertificateprofile"></a><span data-ttu-id="f418d-103">创建 windows10ImportedPFXCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="f418d-103">Create windows10ImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="f418d-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f418d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f418d-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f418d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f418d-106">创建新的[windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f418d-106">Create a new [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f418d-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="f418d-107">Prerequisites</span></span>
<span data-ttu-id="f418d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f418d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f418d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f418d-110">Permission type</span></span>|<span data-ttu-id="f418d-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f418d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f418d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f418d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f418d-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f418d-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f418d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f418d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f418d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f418d-115">Not supported.</span></span>|
|<span data-ttu-id="f418d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f418d-116">Application</span></span>|<span data-ttu-id="f418d-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="f418d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f418d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f418d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f418d-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f418d-119">Request headers</span></span>
|<span data-ttu-id="f418d-120">标头</span><span class="sxs-lookup"><span data-stu-id="f418d-120">Header</span></span>|<span data-ttu-id="f418d-121">值</span><span class="sxs-lookup"><span data-stu-id="f418d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f418d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f418d-122">Authorization</span></span>|<span data-ttu-id="f418d-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f418d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f418d-124">接受</span><span class="sxs-lookup"><span data-stu-id="f418d-124">Accept</span></span>|<span data-ttu-id="f418d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f418d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f418d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f418d-126">Request body</span></span>
<span data-ttu-id="f418d-127">在请求正文中, 提供 windows10ImportedPFXCertificateProfile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f418d-127">In the request body, supply a JSON representation for the windows10ImportedPFXCertificateProfile object.</span></span>

<span data-ttu-id="f418d-128">下表显示创建 windows10ImportedPFXCertificateProfile 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f418d-128">The following table shows the properties that are required when you create the windows10ImportedPFXCertificateProfile.</span></span>

|<span data-ttu-id="f418d-129">属性</span><span class="sxs-lookup"><span data-stu-id="f418d-129">Property</span></span>|<span data-ttu-id="f418d-130">类型</span><span class="sxs-lookup"><span data-stu-id="f418d-130">Type</span></span>|<span data-ttu-id="f418d-131">说明</span><span class="sxs-lookup"><span data-stu-id="f418d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f418d-132">id</span><span class="sxs-lookup"><span data-stu-id="f418d-132">id</span></span>|<span data-ttu-id="f418d-133">String</span><span class="sxs-lookup"><span data-stu-id="f418d-133">String</span></span>|<span data-ttu-id="f418d-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f418d-134">Key of the entity.</span></span> <span data-ttu-id="f418d-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f418d-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f418d-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f418d-136">lastModifiedDateTime</span></span>|<span data-ttu-id="f418d-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f418d-137">DateTimeOffset</span></span>|<span data-ttu-id="f418d-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f418d-138">DateTime the object was last modified.</span></span> <span data-ttu-id="f418d-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f418d-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f418d-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f418d-140">roleScopeTagIds</span></span>|<span data-ttu-id="f418d-141">String collection</span><span class="sxs-lookup"><span data-stu-id="f418d-141">String collection</span></span>|<span data-ttu-id="f418d-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="f418d-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f418d-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f418d-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f418d-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f418d-144">supportsScopeTags</span></span>|<span data-ttu-id="f418d-145">布尔</span><span class="sxs-lookup"><span data-stu-id="f418d-145">Boolean</span></span>|<span data-ttu-id="f418d-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="f418d-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f418d-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="f418d-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f418d-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="f418d-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f418d-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="f418d-149">This property is read-only.</span></span> <span data-ttu-id="f418d-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f418d-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f418d-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f418d-151">createdDateTime</span></span>|<span data-ttu-id="f418d-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f418d-152">DateTimeOffset</span></span>|<span data-ttu-id="f418d-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f418d-153">DateTime the object was created.</span></span> <span data-ttu-id="f418d-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f418d-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f418d-155">description</span><span class="sxs-lookup"><span data-stu-id="f418d-155">description</span></span>|<span data-ttu-id="f418d-156">字符串</span><span class="sxs-lookup"><span data-stu-id="f418d-156">String</span></span>|<span data-ttu-id="f418d-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="f418d-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f418d-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f418d-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f418d-159">displayName</span><span class="sxs-lookup"><span data-stu-id="f418d-159">displayName</span></span>|<span data-ttu-id="f418d-160">String</span><span class="sxs-lookup"><span data-stu-id="f418d-160">String</span></span>|<span data-ttu-id="f418d-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="f418d-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f418d-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f418d-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f418d-163">version</span><span class="sxs-lookup"><span data-stu-id="f418d-163">version</span></span>|<span data-ttu-id="f418d-164">Int32</span><span class="sxs-lookup"><span data-stu-id="f418d-164">Int32</span></span>|<span data-ttu-id="f418d-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="f418d-165">Version of the device configuration.</span></span> <span data-ttu-id="f418d-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f418d-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f418d-167">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="f418d-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="f418d-168">Int32</span><span class="sxs-lookup"><span data-stu-id="f418d-168">Int32</span></span>|<span data-ttu-id="f418d-169">证书续订阈值百分比。</span><span class="sxs-lookup"><span data-stu-id="f418d-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="f418d-170">从[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)继承的有效值1到99</span><span class="sxs-lookup"><span data-stu-id="f418d-170">Valid values 1 to 99 Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="f418d-171">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="f418d-171">keyStorageProvider</span></span>|[<span data-ttu-id="f418d-172">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="f418d-172">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="f418d-173">从[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)继承的密钥存储提供程序 (KSP)。</span><span class="sxs-lookup"><span data-stu-id="f418d-173">Key Storage Provider (KSP) Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="f418d-174">可取值为：`useTpmKspOtherwiseUseSoftwareKsp`、`useTpmKspOtherwiseFail`、`usePassportForWorkKspOtherwiseFail`、`useSoftwareKsp`。</span><span class="sxs-lookup"><span data-stu-id="f418d-174">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="f418d-175">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="f418d-175">subjectNameFormat</span></span>|[<span data-ttu-id="f418d-176">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="f418d-176">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="f418d-177">证书使用者名称格式继承自[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="f418d-177">Certificate Subject Name Format Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="f418d-178">可取值为：`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId`。</span><span class="sxs-lookup"><span data-stu-id="f418d-178">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="f418d-179">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="f418d-179">subjectAlternativeNameType</span></span>|[<span data-ttu-id="f418d-180">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="f418d-180">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="f418d-181">证书使用者备用名称类型继承自[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="f418d-181">Certificate Subject Alternative Name Type Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="f418d-182">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute` 或 `domainNameService`。</span><span class="sxs-lookup"><span data-stu-id="f418d-182">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="f418d-183">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="f418d-183">certificateValidityPeriodValue</span></span>|<span data-ttu-id="f418d-184">Int32</span><span class="sxs-lookup"><span data-stu-id="f418d-184">Int32</span></span>|<span data-ttu-id="f418d-185">继承自[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)的证书有效期限的值</span><span class="sxs-lookup"><span data-stu-id="f418d-185">Value for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="f418d-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="f418d-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="f418d-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="f418d-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="f418d-188">从[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)继承的证书有效期限的小数位数。</span><span class="sxs-lookup"><span data-stu-id="f418d-188">Scale for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="f418d-189">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="f418d-189">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="f418d-190">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="f418d-190">intendedPurpose</span></span>|[<span data-ttu-id="f418d-191">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="f418d-191">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="f418d-192">尚未记录。</span><span class="sxs-lookup"><span data-stu-id="f418d-192">Not yet documented.</span></span> <span data-ttu-id="f418d-193">可取值为：`unassigned`、`smimeEncryption`、`smimeSigning`、`vpn` 或 `wifi`。</span><span class="sxs-lookup"><span data-stu-id="f418d-193">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="f418d-194">响应</span><span class="sxs-lookup"><span data-stu-id="f418d-194">Response</span></span>
<span data-ttu-id="f418d-195">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f418d-195">If successful, this method returns a `201 Created` response code and a [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f418d-196">示例</span><span class="sxs-lookup"><span data-stu-id="f418d-196">Example</span></span>

### <a name="request"></a><span data-ttu-id="f418d-197">请求</span><span class="sxs-lookup"><span data-stu-id="f418d-197">Request</span></span>
<span data-ttu-id="f418d-198">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f418d-198">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 586

{
  "@odata.type": "#microsoft.graph.windows10ImportedPFXCertificateProfile",
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

### <a name="response"></a><span data-ttu-id="f418d-199">响应</span><span class="sxs-lookup"><span data-stu-id="f418d-199">Response</span></span>
<span data-ttu-id="f418d-p116">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f418d-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 758

{
  "@odata.type": "#microsoft.graph.windows10ImportedPFXCertificateProfile",
  "id": "b582514b-514b-b582-4b51-82b54b5182b5",
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





