---
title: 创建 windows10PkcsCertificateProfile
description: 创建新的 windows10PkcsCertificateProfile 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f4a33bd1b8190a135d26765578ea3f330de8e0e5
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36344999"
---
# <a name="create-windows10pkcscertificateprofile"></a><span data-ttu-id="ab947-103">创建 windows10PkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="ab947-103">Create windows10PkcsCertificateProfile</span></span>

> <span data-ttu-id="ab947-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ab947-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ab947-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ab947-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ab947-106">创建新的[windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ab947-106">Create a new [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ab947-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="ab947-107">Prerequisites</span></span>
<span data-ttu-id="ab947-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ab947-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab947-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ab947-110">Permission type</span></span>|<span data-ttu-id="ab947-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ab947-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ab947-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ab947-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ab947-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab947-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ab947-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ab947-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ab947-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ab947-115">Not supported.</span></span>|
|<span data-ttu-id="ab947-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ab947-116">Application</span></span>|<span data-ttu-id="ab947-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab947-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ab947-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ab947-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ab947-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ab947-119">Request headers</span></span>
|<span data-ttu-id="ab947-120">标头</span><span class="sxs-lookup"><span data-stu-id="ab947-120">Header</span></span>|<span data-ttu-id="ab947-121">值</span><span class="sxs-lookup"><span data-stu-id="ab947-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ab947-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ab947-122">Authorization</span></span>|<span data-ttu-id="ab947-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ab947-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ab947-124">接受</span><span class="sxs-lookup"><span data-stu-id="ab947-124">Accept</span></span>|<span data-ttu-id="ab947-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ab947-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ab947-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ab947-126">Request body</span></span>
<span data-ttu-id="ab947-127">在请求正文中, 提供 windows10PkcsCertificateProfile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ab947-127">In the request body, supply a JSON representation for the windows10PkcsCertificateProfile object.</span></span>

<span data-ttu-id="ab947-128">下表显示创建 windows10PkcsCertificateProfile 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ab947-128">The following table shows the properties that are required when you create the windows10PkcsCertificateProfile.</span></span>

|<span data-ttu-id="ab947-129">属性</span><span class="sxs-lookup"><span data-stu-id="ab947-129">Property</span></span>|<span data-ttu-id="ab947-130">类型</span><span class="sxs-lookup"><span data-stu-id="ab947-130">Type</span></span>|<span data-ttu-id="ab947-131">说明</span><span class="sxs-lookup"><span data-stu-id="ab947-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab947-132">id</span><span class="sxs-lookup"><span data-stu-id="ab947-132">id</span></span>|<span data-ttu-id="ab947-133">字符串</span><span class="sxs-lookup"><span data-stu-id="ab947-133">String</span></span>|<span data-ttu-id="ab947-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="ab947-134">Key of the entity.</span></span> <span data-ttu-id="ab947-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ab947-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab947-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ab947-136">lastModifiedDateTime</span></span>|<span data-ttu-id="ab947-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ab947-137">DateTimeOffset</span></span>|<span data-ttu-id="ab947-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="ab947-138">DateTime the object was last modified.</span></span> <span data-ttu-id="ab947-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ab947-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab947-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ab947-140">roleScopeTagIds</span></span>|<span data-ttu-id="ab947-141">String collection</span><span class="sxs-lookup"><span data-stu-id="ab947-141">String collection</span></span>|<span data-ttu-id="ab947-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="ab947-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ab947-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ab947-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab947-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ab947-144">supportsScopeTags</span></span>|<span data-ttu-id="ab947-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="ab947-145">Boolean</span></span>|<span data-ttu-id="ab947-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="ab947-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ab947-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="ab947-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ab947-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="ab947-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ab947-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="ab947-149">This property is read-only.</span></span> <span data-ttu-id="ab947-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ab947-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab947-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ab947-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="ab947-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ab947-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="ab947-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="ab947-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="ab947-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ab947-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab947-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ab947-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="ab947-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ab947-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="ab947-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="ab947-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="ab947-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ab947-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab947-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ab947-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="ab947-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ab947-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="ab947-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="ab947-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="ab947-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ab947-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab947-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ab947-163">createdDateTime</span></span>|<span data-ttu-id="ab947-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ab947-164">DateTimeOffset</span></span>|<span data-ttu-id="ab947-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="ab947-165">DateTime the object was created.</span></span> <span data-ttu-id="ab947-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ab947-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab947-167">说明</span><span class="sxs-lookup"><span data-stu-id="ab947-167">description</span></span>|<span data-ttu-id="ab947-168">String</span><span class="sxs-lookup"><span data-stu-id="ab947-168">String</span></span>|<span data-ttu-id="ab947-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="ab947-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ab947-170">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ab947-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab947-171">displayName</span><span class="sxs-lookup"><span data-stu-id="ab947-171">displayName</span></span>|<span data-ttu-id="ab947-172">String</span><span class="sxs-lookup"><span data-stu-id="ab947-172">String</span></span>|<span data-ttu-id="ab947-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="ab947-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ab947-174">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ab947-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab947-175">version</span><span class="sxs-lookup"><span data-stu-id="ab947-175">version</span></span>|<span data-ttu-id="ab947-176">Int32</span><span class="sxs-lookup"><span data-stu-id="ab947-176">Int32</span></span>|<span data-ttu-id="ab947-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="ab947-177">Version of the device configuration.</span></span> <span data-ttu-id="ab947-178">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ab947-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab947-179">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="ab947-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="ab947-180">Int32</span><span class="sxs-lookup"><span data-stu-id="ab947-180">Int32</span></span>|<span data-ttu-id="ab947-181">证书续订阈值百分比。</span><span class="sxs-lookup"><span data-stu-id="ab947-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="ab947-182">从[WindowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)继承的有效值1到99</span><span class="sxs-lookup"><span data-stu-id="ab947-182">Valid values 1 to 99 Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="ab947-183">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="ab947-183">keyStorageProvider</span></span>|[<span data-ttu-id="ab947-184">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="ab947-184">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="ab947-185">从[WindowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)继承的密钥存储提供程序 (KSP)。</span><span class="sxs-lookup"><span data-stu-id="ab947-185">Key Storage Provider (KSP) Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="ab947-186">可取值为：`useTpmKspOtherwiseUseSoftwareKsp`、`useTpmKspOtherwiseFail`、`usePassportForWorkKspOtherwiseFail`、`useSoftwareKsp`。</span><span class="sxs-lookup"><span data-stu-id="ab947-186">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="ab947-187">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="ab947-187">subjectNameFormat</span></span>|[<span data-ttu-id="ab947-188">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="ab947-188">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="ab947-189">证书使用者名称格式继承自[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="ab947-189">Certificate Subject Name Format Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="ab947-190">可取值为：`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId`。</span><span class="sxs-lookup"><span data-stu-id="ab947-190">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="ab947-191">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="ab947-191">subjectAlternativeNameType</span></span>|[<span data-ttu-id="ab947-192">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="ab947-192">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="ab947-193">证书使用者备用名称类型继承自[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="ab947-193">Certificate Subject Alternative Name Type Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="ab947-194">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService`。</span><span class="sxs-lookup"><span data-stu-id="ab947-194">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="ab947-195">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="ab947-195">certificateValidityPeriodValue</span></span>|<span data-ttu-id="ab947-196">Int32</span><span class="sxs-lookup"><span data-stu-id="ab947-196">Int32</span></span>|<span data-ttu-id="ab947-197">继承自[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)的证书有效期限的值</span><span class="sxs-lookup"><span data-stu-id="ab947-197">Value for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="ab947-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="ab947-198">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="ab947-199">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="ab947-199">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="ab947-200">从[WindowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)继承的证书有效期限的小数位数。</span><span class="sxs-lookup"><span data-stu-id="ab947-200">Scale for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="ab947-201">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="ab947-201">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="ab947-202">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="ab947-202">certificationAuthority</span></span>|<span data-ttu-id="ab947-203">String</span><span class="sxs-lookup"><span data-stu-id="ab947-203">String</span></span>|<span data-ttu-id="ab947-204">PKCS 证书颁发机构</span><span class="sxs-lookup"><span data-stu-id="ab947-204">PKCS Certification Authority</span></span>|
|<span data-ttu-id="ab947-205">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="ab947-205">certificationAuthorityName</span></span>|<span data-ttu-id="ab947-206">String</span><span class="sxs-lookup"><span data-stu-id="ab947-206">String</span></span>|<span data-ttu-id="ab947-207">PKCS 证书颁发机构名称</span><span class="sxs-lookup"><span data-stu-id="ab947-207">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="ab947-208">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="ab947-208">certificateTemplateName</span></span>|<span data-ttu-id="ab947-209">String</span><span class="sxs-lookup"><span data-stu-id="ab947-209">String</span></span>|<span data-ttu-id="ab947-210">PKCS 证书模板名称</span><span class="sxs-lookup"><span data-stu-id="ab947-210">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="ab947-211">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="ab947-211">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="ab947-212">String</span><span class="sxs-lookup"><span data-stu-id="ab947-212">String</span></span>|<span data-ttu-id="ab947-213">定义 AAD 属性的自定义字符串。</span><span class="sxs-lookup"><span data-stu-id="ab947-213">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="ab947-214">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="ab947-214">extendedKeyUsages</span></span>|<span data-ttu-id="ab947-215">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)集合</span><span class="sxs-lookup"><span data-stu-id="ab947-215">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="ab947-216">扩展密钥用法 (EKU) 设置。</span><span class="sxs-lookup"><span data-stu-id="ab947-216">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="ab947-217">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="ab947-217">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="ab947-218">响应</span><span class="sxs-lookup"><span data-stu-id="ab947-218">Response</span></span>
<span data-ttu-id="ab947-219">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ab947-219">If successful, this method returns a `201 Created` response code and a [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab947-220">示例</span><span class="sxs-lookup"><span data-stu-id="ab947-220">Example</span></span>

### <a name="request"></a><span data-ttu-id="ab947-221">请求</span><span class="sxs-lookup"><span data-stu-id="ab947-221">Request</span></span>
<span data-ttu-id="ab947-222">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ab947-222">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1784

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
  ]
}
```

### <a name="response"></a><span data-ttu-id="ab947-223">响应</span><span class="sxs-lookup"><span data-stu-id="ab947-223">Response</span></span>
<span data-ttu-id="ab947-p119">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ab947-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1956

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
  ]
}
```






