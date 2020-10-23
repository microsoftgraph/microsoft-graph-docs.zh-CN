---
title: 创建 windows10PkcsCertificateProfile
description: 创建新的 windows10PkcsCertificateProfile 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7bb76ccc722c59ff1929712dcad4c91bcd0eab42
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48734642"
---
# <a name="create-windows10pkcscertificateprofile"></a><span data-ttu-id="74657-103">创建 windows10PkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="74657-103">Create windows10PkcsCertificateProfile</span></span>

<span data-ttu-id="74657-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="74657-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="74657-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="74657-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="74657-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="74657-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="74657-107">创建新的 [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="74657-107">Create a new [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="74657-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="74657-108">Prerequisites</span></span>
<span data-ttu-id="74657-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="74657-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74657-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="74657-111">Permission type</span></span>|<span data-ttu-id="74657-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="74657-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="74657-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="74657-113">Delegated (work or school account)</span></span>|<span data-ttu-id="74657-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74657-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="74657-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="74657-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="74657-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="74657-116">Not supported.</span></span>|
|<span data-ttu-id="74657-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="74657-117">Application</span></span>|<span data-ttu-id="74657-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74657-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="74657-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="74657-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="74657-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="74657-120">Request headers</span></span>
|<span data-ttu-id="74657-121">标头</span><span class="sxs-lookup"><span data-stu-id="74657-121">Header</span></span>|<span data-ttu-id="74657-122">值</span><span class="sxs-lookup"><span data-stu-id="74657-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="74657-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="74657-123">Authorization</span></span>|<span data-ttu-id="74657-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="74657-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="74657-125">接受</span><span class="sxs-lookup"><span data-stu-id="74657-125">Accept</span></span>|<span data-ttu-id="74657-126">application/json</span><span class="sxs-lookup"><span data-stu-id="74657-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="74657-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="74657-127">Request body</span></span>
<span data-ttu-id="74657-128">在请求正文中，提供 windows10PkcsCertificateProfile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="74657-128">In the request body, supply a JSON representation for the windows10PkcsCertificateProfile object.</span></span>

<span data-ttu-id="74657-129">下表显示创建 windows10PkcsCertificateProfile 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="74657-129">The following table shows the properties that are required when you create the windows10PkcsCertificateProfile.</span></span>

|<span data-ttu-id="74657-130">属性</span><span class="sxs-lookup"><span data-stu-id="74657-130">Property</span></span>|<span data-ttu-id="74657-131">类型</span><span class="sxs-lookup"><span data-stu-id="74657-131">Type</span></span>|<span data-ttu-id="74657-132">说明</span><span class="sxs-lookup"><span data-stu-id="74657-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74657-133">id</span><span class="sxs-lookup"><span data-stu-id="74657-133">id</span></span>|<span data-ttu-id="74657-134">String</span><span class="sxs-lookup"><span data-stu-id="74657-134">String</span></span>|<span data-ttu-id="74657-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="74657-135">Key of the entity.</span></span> <span data-ttu-id="74657-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="74657-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="74657-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="74657-137">lastModifiedDateTime</span></span>|<span data-ttu-id="74657-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="74657-138">DateTimeOffset</span></span>|<span data-ttu-id="74657-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="74657-139">DateTime the object was last modified.</span></span> <span data-ttu-id="74657-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="74657-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="74657-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="74657-141">roleScopeTagIds</span></span>|<span data-ttu-id="74657-142">String collection</span><span class="sxs-lookup"><span data-stu-id="74657-142">String collection</span></span>|<span data-ttu-id="74657-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="74657-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="74657-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="74657-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="74657-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="74657-145">supportsScopeTags</span></span>|<span data-ttu-id="74657-146">布尔</span><span class="sxs-lookup"><span data-stu-id="74657-146">Boolean</span></span>|<span data-ttu-id="74657-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="74657-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="74657-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="74657-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="74657-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="74657-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="74657-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="74657-150">This property is read-only.</span></span> <span data-ttu-id="74657-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="74657-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="74657-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="74657-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="74657-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="74657-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="74657-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="74657-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="74657-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="74657-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="74657-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="74657-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="74657-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="74657-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="74657-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="74657-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="74657-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="74657-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="74657-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="74657-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="74657-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="74657-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="74657-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="74657-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="74657-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="74657-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="74657-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="74657-164">createdDateTime</span></span>|<span data-ttu-id="74657-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="74657-165">DateTimeOffset</span></span>|<span data-ttu-id="74657-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="74657-166">DateTime the object was created.</span></span> <span data-ttu-id="74657-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="74657-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="74657-168">说明</span><span class="sxs-lookup"><span data-stu-id="74657-168">description</span></span>|<span data-ttu-id="74657-169">String</span><span class="sxs-lookup"><span data-stu-id="74657-169">String</span></span>|<span data-ttu-id="74657-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="74657-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="74657-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="74657-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="74657-172">displayName</span><span class="sxs-lookup"><span data-stu-id="74657-172">displayName</span></span>|<span data-ttu-id="74657-173">String</span><span class="sxs-lookup"><span data-stu-id="74657-173">String</span></span>|<span data-ttu-id="74657-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="74657-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="74657-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="74657-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="74657-176">version</span><span class="sxs-lookup"><span data-stu-id="74657-176">version</span></span>|<span data-ttu-id="74657-177">Int32</span><span class="sxs-lookup"><span data-stu-id="74657-177">Int32</span></span>|<span data-ttu-id="74657-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="74657-178">Version of the device configuration.</span></span> <span data-ttu-id="74657-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="74657-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="74657-180">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="74657-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="74657-181">Int32</span><span class="sxs-lookup"><span data-stu-id="74657-181">Int32</span></span>|<span data-ttu-id="74657-182">证书续订阈值百分比。</span><span class="sxs-lookup"><span data-stu-id="74657-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="74657-183">从[WindowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)继承的有效值1到99</span><span class="sxs-lookup"><span data-stu-id="74657-183">Valid values 1 to 99 Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="74657-184">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="74657-184">keyStorageProvider</span></span>|[<span data-ttu-id="74657-185">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="74657-185">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="74657-186">密钥存储提供程序 (KSP) 继承自 [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="74657-186">Key Storage Provider (KSP) Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="74657-187">可取值为：`useTpmKspOtherwiseUseSoftwareKsp`、`useTpmKspOtherwiseFail`、`usePassportForWorkKspOtherwiseFail`、`useSoftwareKsp`。</span><span class="sxs-lookup"><span data-stu-id="74657-187">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="74657-188">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="74657-188">subjectNameFormat</span></span>|[<span data-ttu-id="74657-189">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="74657-189">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="74657-190">证书使用者名称格式继承自 [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="74657-190">Certificate Subject Name Format Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="74657-191">可取值为：`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId`。</span><span class="sxs-lookup"><span data-stu-id="74657-191">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="74657-192">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="74657-192">subjectAlternativeNameType</span></span>|[<span data-ttu-id="74657-193">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="74657-193">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="74657-194">证书使用者备用名称类型继承自 [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="74657-194">Certificate Subject Alternative Name Type Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="74657-195">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService`、`universalResourceIdentifier`。</span><span class="sxs-lookup"><span data-stu-id="74657-195">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span></span>|
|<span data-ttu-id="74657-196">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="74657-196">certificateValidityPeriodValue</span></span>|<span data-ttu-id="74657-197">Int32</span><span class="sxs-lookup"><span data-stu-id="74657-197">Int32</span></span>|<span data-ttu-id="74657-198">继承自[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)的证书有效期限的值</span><span class="sxs-lookup"><span data-stu-id="74657-198">Value for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="74657-199">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="74657-199">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="74657-200">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="74657-200">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="74657-201">从 [WindowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)继承的证书有效期限的小数位数。</span><span class="sxs-lookup"><span data-stu-id="74657-201">Scale for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="74657-202">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="74657-202">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="74657-203">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="74657-203">certificationAuthority</span></span>|<span data-ttu-id="74657-204">String</span><span class="sxs-lookup"><span data-stu-id="74657-204">String</span></span>|<span data-ttu-id="74657-205">PKCS 证书颁发机构</span><span class="sxs-lookup"><span data-stu-id="74657-205">PKCS Certification Authority</span></span>|
|<span data-ttu-id="74657-206">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="74657-206">certificationAuthorityName</span></span>|<span data-ttu-id="74657-207">String</span><span class="sxs-lookup"><span data-stu-id="74657-207">String</span></span>|<span data-ttu-id="74657-208">PKCS 证书颁发机构名称</span><span class="sxs-lookup"><span data-stu-id="74657-208">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="74657-209">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="74657-209">certificateTemplateName</span></span>|<span data-ttu-id="74657-210">String</span><span class="sxs-lookup"><span data-stu-id="74657-210">String</span></span>|<span data-ttu-id="74657-211">PKCS 证书模板名称</span><span class="sxs-lookup"><span data-stu-id="74657-211">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="74657-212">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="74657-212">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="74657-213">String</span><span class="sxs-lookup"><span data-stu-id="74657-213">String</span></span>|<span data-ttu-id="74657-214">定义 AAD 属性的自定义字符串。</span><span class="sxs-lookup"><span data-stu-id="74657-214">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="74657-215">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="74657-215">extendedKeyUsages</span></span>|<span data-ttu-id="74657-216">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="74657-216">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="74657-217"> (EKU) 设置的扩展密钥用法。</span><span class="sxs-lookup"><span data-stu-id="74657-217">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="74657-218">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="74657-218">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="74657-219">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="74657-219">subjectNameFormatString</span></span>|<span data-ttu-id="74657-220">String</span><span class="sxs-lookup"><span data-stu-id="74657-220">String</span></span>|<span data-ttu-id="74657-221">要与 SubjectNameFormat = Custom 一起使用的自定义格式。</span><span class="sxs-lookup"><span data-stu-id="74657-221">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="74657-222">示例： CN = {{EmailAddress}}，E = {{EmailAddress}}，OU = 企业用户，O = Contoso Corporation，L = Redmond，ST = WA，C = US</span><span class="sxs-lookup"><span data-stu-id="74657-222">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="74657-223">certificateStore</span><span class="sxs-lookup"><span data-stu-id="74657-223">certificateStore</span></span>|[<span data-ttu-id="74657-224">certificateStore</span><span class="sxs-lookup"><span data-stu-id="74657-224">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="74657-225">目标存储证书。</span><span class="sxs-lookup"><span data-stu-id="74657-225">Target store certificate.</span></span> <span data-ttu-id="74657-226">可取值为：`user`、`machine`。</span><span class="sxs-lookup"><span data-stu-id="74657-226">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="74657-227">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="74657-227">customSubjectAlternativeNames</span></span>|<span data-ttu-id="74657-228">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) 集合</span><span class="sxs-lookup"><span data-stu-id="74657-228">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="74657-229">自定义主题备用名称设置。</span><span class="sxs-lookup"><span data-stu-id="74657-229">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="74657-230">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="74657-230">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="74657-231">响应</span><span class="sxs-lookup"><span data-stu-id="74657-231">Response</span></span>
<span data-ttu-id="74657-232">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="74657-232">If successful, this method returns a `201 Created` response code and a [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="74657-233">示例</span><span class="sxs-lookup"><span data-stu-id="74657-233">Example</span></span>

### <a name="request"></a><span data-ttu-id="74657-234">请求</span><span class="sxs-lookup"><span data-stu-id="74657-234">Request</span></span>
<span data-ttu-id="74657-235">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="74657-235">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2074

{
  "@odata.type": "#microsoft.graph.windows10PkcsCertificateProfile",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "renewalThresholdPercentage": 10,
  "keyStorageProvider": "useTpmKspOtherwiseFail",
  "subjectNameFormat": "commonNameIncludingEmail",
  "subjectAlternativeNameType": "emailAddress",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "subjectNameFormatString": "Subject Name Format String value",
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

### <a name="response"></a><span data-ttu-id="74657-236">响应</span><span class="sxs-lookup"><span data-stu-id="74657-236">Response</span></span>
<span data-ttu-id="74657-p122">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="74657-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2246

{
  "@odata.type": "#microsoft.graph.windows10PkcsCertificateProfile",
  "id": "414c69c0-69c0-414c-c069-4c41c0694c41",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
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
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "subjectNameFormatString": "Subject Name Format String value",
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





