---
title: 创建 windowsPhone81ImportedPFXCertificateProfile
description: 创建新的 windowsPhone81ImportedPFXCertificateProfile 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1126114b04d6c10acd0f01f1d07efbe695e08ad7
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30144931"
---
# <a name="create-windowsphone81importedpfxcertificateprofile"></a><span data-ttu-id="d9b60-103">创建 windowsPhone81ImportedPFXCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="d9b60-103">Create windowsPhone81ImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="d9b60-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d9b60-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d9b60-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d9b60-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d9b60-106">创建新的[windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d9b60-106">Create a new [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d9b60-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="d9b60-107">Prerequisites</span></span>
<span data-ttu-id="d9b60-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="d9b60-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d9b60-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d9b60-110">Permission type</span></span>|<span data-ttu-id="d9b60-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d9b60-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d9b60-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d9b60-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d9b60-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9b60-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d9b60-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d9b60-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d9b60-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d9b60-115">Not supported.</span></span>|
|<span data-ttu-id="d9b60-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d9b60-116">Application</span></span>|<span data-ttu-id="d9b60-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="d9b60-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d9b60-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d9b60-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d9b60-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="d9b60-119">Request headers</span></span>
|<span data-ttu-id="d9b60-120">标头</span><span class="sxs-lookup"><span data-stu-id="d9b60-120">Header</span></span>|<span data-ttu-id="d9b60-121">值</span><span class="sxs-lookup"><span data-stu-id="d9b60-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d9b60-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d9b60-122">Authorization</span></span>|<span data-ttu-id="d9b60-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d9b60-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d9b60-124">Accept</span><span class="sxs-lookup"><span data-stu-id="d9b60-124">Accept</span></span>|<span data-ttu-id="d9b60-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d9b60-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d9b60-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d9b60-126">Request body</span></span>
<span data-ttu-id="d9b60-127">在请求正文中, 提供 windowsPhone81ImportedPFXCertificateProfile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d9b60-127">In the request body, supply a JSON representation for the windowsPhone81ImportedPFXCertificateProfile object.</span></span>

<span data-ttu-id="d9b60-128">下表显示创建 windowsPhone81ImportedPFXCertificateProfile 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d9b60-128">The following table shows the properties that are required when you create the windowsPhone81ImportedPFXCertificateProfile.</span></span>

|<span data-ttu-id="d9b60-129">属性</span><span class="sxs-lookup"><span data-stu-id="d9b60-129">Property</span></span>|<span data-ttu-id="d9b60-130">类型</span><span class="sxs-lookup"><span data-stu-id="d9b60-130">Type</span></span>|<span data-ttu-id="d9b60-131">说明</span><span class="sxs-lookup"><span data-stu-id="d9b60-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9b60-132">id</span><span class="sxs-lookup"><span data-stu-id="d9b60-132">id</span></span>|<span data-ttu-id="d9b60-133">String</span><span class="sxs-lookup"><span data-stu-id="d9b60-133">String</span></span>|<span data-ttu-id="d9b60-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d9b60-134">Key of the entity.</span></span> <span data-ttu-id="d9b60-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d9b60-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d9b60-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d9b60-136">lastModifiedDateTime</span></span>|<span data-ttu-id="d9b60-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d9b60-137">DateTimeOffset</span></span>|<span data-ttu-id="d9b60-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="d9b60-138">DateTime the object was last modified.</span></span> <span data-ttu-id="d9b60-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d9b60-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d9b60-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d9b60-140">roleScopeTagIds</span></span>|<span data-ttu-id="d9b60-141">String collection</span><span class="sxs-lookup"><span data-stu-id="d9b60-141">String collection</span></span>|<span data-ttu-id="d9b60-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="d9b60-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d9b60-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d9b60-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d9b60-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d9b60-144">supportsScopeTags</span></span>|<span data-ttu-id="d9b60-145">布尔</span><span class="sxs-lookup"><span data-stu-id="d9b60-145">Boolean</span></span>|<span data-ttu-id="d9b60-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="d9b60-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d9b60-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="d9b60-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d9b60-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="d9b60-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d9b60-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="d9b60-149">This property is read-only.</span></span> <span data-ttu-id="d9b60-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d9b60-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d9b60-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d9b60-151">createdDateTime</span></span>|<span data-ttu-id="d9b60-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d9b60-152">DateTimeOffset</span></span>|<span data-ttu-id="d9b60-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="d9b60-153">DateTime the object was created.</span></span> <span data-ttu-id="d9b60-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d9b60-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d9b60-155">description</span><span class="sxs-lookup"><span data-stu-id="d9b60-155">description</span></span>|<span data-ttu-id="d9b60-156">String</span><span class="sxs-lookup"><span data-stu-id="d9b60-156">String</span></span>|<span data-ttu-id="d9b60-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="d9b60-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d9b60-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d9b60-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d9b60-159">displayName</span><span class="sxs-lookup"><span data-stu-id="d9b60-159">displayName</span></span>|<span data-ttu-id="d9b60-160">String</span><span class="sxs-lookup"><span data-stu-id="d9b60-160">String</span></span>|<span data-ttu-id="d9b60-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="d9b60-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d9b60-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d9b60-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d9b60-163">version</span><span class="sxs-lookup"><span data-stu-id="d9b60-163">version</span></span>|<span data-ttu-id="d9b60-164">Int32</span><span class="sxs-lookup"><span data-stu-id="d9b60-164">Int32</span></span>|<span data-ttu-id="d9b60-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="d9b60-165">Version of the device configuration.</span></span> <span data-ttu-id="d9b60-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d9b60-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d9b60-167">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="d9b60-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="d9b60-168">Int32</span><span class="sxs-lookup"><span data-stu-id="d9b60-168">Int32</span></span>|<span data-ttu-id="d9b60-169">证书续订阈值百分比。</span><span class="sxs-lookup"><span data-stu-id="d9b60-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="d9b60-170">从[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)继承的有效值1到99</span><span class="sxs-lookup"><span data-stu-id="d9b60-170">Valid values 1 to 99 Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="d9b60-171">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="d9b60-171">keyStorageProvider</span></span>|[<span data-ttu-id="d9b60-172">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="d9b60-172">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="d9b60-173">从[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)继承的密钥存储提供程序 (KSP)。</span><span class="sxs-lookup"><span data-stu-id="d9b60-173">Key Storage Provider (KSP) Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="d9b60-174">可取值为：`useTpmKspOtherwiseUseSoftwareKsp`、`useTpmKspOtherwiseFail`、`usePassportForWorkKspOtherwiseFail`、`useSoftwareKsp`。</span><span class="sxs-lookup"><span data-stu-id="d9b60-174">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="d9b60-175">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="d9b60-175">subjectNameFormat</span></span>|[<span data-ttu-id="d9b60-176">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="d9b60-176">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="d9b60-177">证书使用者名称格式继承自[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="d9b60-177">Certificate Subject Name Format Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="d9b60-178">可取值为：`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId`。</span><span class="sxs-lookup"><span data-stu-id="d9b60-178">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="d9b60-179">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="d9b60-179">subjectAlternativeNameType</span></span>|[<span data-ttu-id="d9b60-180">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="d9b60-180">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="d9b60-181">证书使用者备用名称类型继承自[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="d9b60-181">Certificate Subject Alternative Name Type Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="d9b60-182">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService`。</span><span class="sxs-lookup"><span data-stu-id="d9b60-182">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="d9b60-183">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="d9b60-183">certificateValidityPeriodValue</span></span>|<span data-ttu-id="d9b60-184">Int32</span><span class="sxs-lookup"><span data-stu-id="d9b60-184">Int32</span></span>|<span data-ttu-id="d9b60-185">继承自[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)的证书有效期限的值</span><span class="sxs-lookup"><span data-stu-id="d9b60-185">Value for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="d9b60-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="d9b60-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="d9b60-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="d9b60-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="d9b60-188">从[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)继承的证书有效期限的小数位数。</span><span class="sxs-lookup"><span data-stu-id="d9b60-188">Scale for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="d9b60-189">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="d9b60-189">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="d9b60-190">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="d9b60-190">intendedPurpose</span></span>|[<span data-ttu-id="d9b60-191">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="d9b60-191">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="d9b60-192">尚未记录。</span><span class="sxs-lookup"><span data-stu-id="d9b60-192">Not yet documented.</span></span> <span data-ttu-id="d9b60-193">可取值为：`unassigned`、`smimeEncryption`、`smimeSigning`、`vpn`、`wifi`。</span><span class="sxs-lookup"><span data-stu-id="d9b60-193">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="d9b60-194">响应</span><span class="sxs-lookup"><span data-stu-id="d9b60-194">Response</span></span>
<span data-ttu-id="d9b60-195">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d9b60-195">If successful, this method returns a `201 Created` response code and a [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d9b60-196">示例</span><span class="sxs-lookup"><span data-stu-id="d9b60-196">Example</span></span>

### <a name="request"></a><span data-ttu-id="d9b60-197">请求</span><span class="sxs-lookup"><span data-stu-id="d9b60-197">Request</span></span>
<span data-ttu-id="d9b60-198">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d9b60-198">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="d9b60-199">响应</span><span class="sxs-lookup"><span data-stu-id="d9b60-199">Response</span></span>
<span data-ttu-id="d9b60-p116">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d9b60-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




