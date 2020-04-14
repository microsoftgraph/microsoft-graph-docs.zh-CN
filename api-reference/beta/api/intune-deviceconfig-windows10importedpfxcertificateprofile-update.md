---
title: 更新 windows10ImportedPFXCertificateProfile
description: 更新 windows10ImportedPFXCertificateProfile 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 48d6e5bda20a56221745667211cf36b495ad64e9
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43430725"
---
# <a name="update-windows10importedpfxcertificateprofile"></a><span data-ttu-id="9ee56-103">更新 windows10ImportedPFXCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="9ee56-103">Update windows10ImportedPFXCertificateProfile</span></span>

<span data-ttu-id="9ee56-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9ee56-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9ee56-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9ee56-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9ee56-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9ee56-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ee56-107">更新[windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9ee56-107">Update the properties of a [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9ee56-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="9ee56-108">Prerequisites</span></span>
<span data-ttu-id="9ee56-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9ee56-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ee56-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9ee56-111">Permission type</span></span>|<span data-ttu-id="9ee56-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9ee56-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9ee56-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9ee56-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9ee56-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ee56-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9ee56-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9ee56-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9ee56-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9ee56-116">Not supported.</span></span>|
|<span data-ttu-id="9ee56-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9ee56-117">Application</span></span>|<span data-ttu-id="9ee56-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ee56-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9ee56-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9ee56-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="9ee56-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9ee56-120">Request headers</span></span>
|<span data-ttu-id="9ee56-121">标头</span><span class="sxs-lookup"><span data-stu-id="9ee56-121">Header</span></span>|<span data-ttu-id="9ee56-122">值</span><span class="sxs-lookup"><span data-stu-id="9ee56-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9ee56-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9ee56-123">Authorization</span></span>|<span data-ttu-id="9ee56-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9ee56-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9ee56-125">接受</span><span class="sxs-lookup"><span data-stu-id="9ee56-125">Accept</span></span>|<span data-ttu-id="9ee56-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9ee56-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9ee56-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9ee56-127">Request body</span></span>
<span data-ttu-id="9ee56-128">在请求正文中，提供[windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9ee56-128">In the request body, supply a JSON representation for the [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md) object.</span></span>

<span data-ttu-id="9ee56-129">下表显示创建[windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="9ee56-129">The following table shows the properties that are required when you create the [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md).</span></span>

|<span data-ttu-id="9ee56-130">属性</span><span class="sxs-lookup"><span data-stu-id="9ee56-130">Property</span></span>|<span data-ttu-id="9ee56-131">类型</span><span class="sxs-lookup"><span data-stu-id="9ee56-131">Type</span></span>|<span data-ttu-id="9ee56-132">说明</span><span class="sxs-lookup"><span data-stu-id="9ee56-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ee56-133">id</span><span class="sxs-lookup"><span data-stu-id="9ee56-133">id</span></span>|<span data-ttu-id="9ee56-134">字符串</span><span class="sxs-lookup"><span data-stu-id="9ee56-134">String</span></span>|<span data-ttu-id="9ee56-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="9ee56-135">Key of the entity.</span></span> <span data-ttu-id="9ee56-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9ee56-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ee56-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9ee56-137">lastModifiedDateTime</span></span>|<span data-ttu-id="9ee56-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ee56-138">DateTimeOffset</span></span>|<span data-ttu-id="9ee56-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="9ee56-139">DateTime the object was last modified.</span></span> <span data-ttu-id="9ee56-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9ee56-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ee56-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9ee56-141">roleScopeTagIds</span></span>|<span data-ttu-id="9ee56-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="9ee56-142">String collection</span></span>|<span data-ttu-id="9ee56-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="9ee56-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9ee56-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9ee56-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ee56-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="9ee56-145">supportsScopeTags</span></span>|<span data-ttu-id="9ee56-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ee56-146">Boolean</span></span>|<span data-ttu-id="9ee56-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="9ee56-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="9ee56-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="9ee56-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="9ee56-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="9ee56-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="9ee56-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9ee56-150">This property is read-only.</span></span> <span data-ttu-id="9ee56-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9ee56-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ee56-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="9ee56-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="9ee56-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="9ee56-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="9ee56-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="9ee56-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="9ee56-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9ee56-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ee56-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="9ee56-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="9ee56-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="9ee56-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="9ee56-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="9ee56-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="9ee56-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9ee56-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ee56-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="9ee56-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="9ee56-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="9ee56-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="9ee56-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="9ee56-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="9ee56-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9ee56-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ee56-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9ee56-164">createdDateTime</span></span>|<span data-ttu-id="9ee56-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ee56-165">DateTimeOffset</span></span>|<span data-ttu-id="9ee56-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="9ee56-166">DateTime the object was created.</span></span> <span data-ttu-id="9ee56-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9ee56-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ee56-168">description</span><span class="sxs-lookup"><span data-stu-id="9ee56-168">description</span></span>|<span data-ttu-id="9ee56-169">String</span><span class="sxs-lookup"><span data-stu-id="9ee56-169">String</span></span>|<span data-ttu-id="9ee56-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="9ee56-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9ee56-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9ee56-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ee56-172">displayName</span><span class="sxs-lookup"><span data-stu-id="9ee56-172">displayName</span></span>|<span data-ttu-id="9ee56-173">String</span><span class="sxs-lookup"><span data-stu-id="9ee56-173">String</span></span>|<span data-ttu-id="9ee56-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="9ee56-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9ee56-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9ee56-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ee56-176">version</span><span class="sxs-lookup"><span data-stu-id="9ee56-176">version</span></span>|<span data-ttu-id="9ee56-177">Int32</span><span class="sxs-lookup"><span data-stu-id="9ee56-177">Int32</span></span>|<span data-ttu-id="9ee56-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="9ee56-178">Version of the device configuration.</span></span> <span data-ttu-id="9ee56-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9ee56-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ee56-180">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="9ee56-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="9ee56-181">Int32</span><span class="sxs-lookup"><span data-stu-id="9ee56-181">Int32</span></span>|<span data-ttu-id="9ee56-182">证书续订阈值百分比。</span><span class="sxs-lookup"><span data-stu-id="9ee56-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="9ee56-183">从[WindowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)继承的有效值1到99</span><span class="sxs-lookup"><span data-stu-id="9ee56-183">Valid values 1 to 99 Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="9ee56-184">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="9ee56-184">keyStorageProvider</span></span>|[<span data-ttu-id="9ee56-185">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="9ee56-185">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="9ee56-186">从[WindowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)继承的密钥存储提供程序（KSP）。</span><span class="sxs-lookup"><span data-stu-id="9ee56-186">Key Storage Provider (KSP) Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="9ee56-187">可取值为：`useTpmKspOtherwiseUseSoftwareKsp`、`useTpmKspOtherwiseFail`、`usePassportForWorkKspOtherwiseFail`、`useSoftwareKsp`。</span><span class="sxs-lookup"><span data-stu-id="9ee56-187">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="9ee56-188">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="9ee56-188">subjectNameFormat</span></span>|[<span data-ttu-id="9ee56-189">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="9ee56-189">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="9ee56-190">证书使用者名称格式继承自[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="9ee56-190">Certificate Subject Name Format Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="9ee56-191">可取值为：`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId`。</span><span class="sxs-lookup"><span data-stu-id="9ee56-191">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="9ee56-192">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="9ee56-192">subjectAlternativeNameType</span></span>|[<span data-ttu-id="9ee56-193">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="9ee56-193">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="9ee56-194">证书使用者备用名称类型继承自[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="9ee56-194">Certificate Subject Alternative Name Type Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="9ee56-195">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService`。</span><span class="sxs-lookup"><span data-stu-id="9ee56-195">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="9ee56-196">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="9ee56-196">certificateValidityPeriodValue</span></span>|<span data-ttu-id="9ee56-197">Int32</span><span class="sxs-lookup"><span data-stu-id="9ee56-197">Int32</span></span>|<span data-ttu-id="9ee56-198">继承自[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)的证书有效期限的值</span><span class="sxs-lookup"><span data-stu-id="9ee56-198">Value for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="9ee56-199">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="9ee56-199">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="9ee56-200">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="9ee56-200">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="9ee56-201">从[WindowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)继承的证书有效期限的小数位数。</span><span class="sxs-lookup"><span data-stu-id="9ee56-201">Scale for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="9ee56-202">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="9ee56-202">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="9ee56-203">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="9ee56-203">intendedPurpose</span></span>|[<span data-ttu-id="9ee56-204">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="9ee56-204">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="9ee56-205">证书配置文件的预期用途-可以为未分配、SmimeEncryption、SmimeSigning 等。可能的值为`unassigned`： `smimeEncryption`、 `smimeSigning`、 `vpn`、 `wifi`、。</span><span class="sxs-lookup"><span data-stu-id="9ee56-205">Intended Purpose of the Certificate Profile - which could be Unassigned, SmimeEncryption, SmimeSigning etc. Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="9ee56-206">响应</span><span class="sxs-lookup"><span data-stu-id="9ee56-206">Response</span></span>
<span data-ttu-id="9ee56-207">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9ee56-207">If successful, this method returns a `200 OK` response code and an updated [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ee56-208">示例</span><span class="sxs-lookup"><span data-stu-id="9ee56-208">Example</span></span>

### <a name="request"></a><span data-ttu-id="9ee56-209">请求</span><span class="sxs-lookup"><span data-stu-id="9ee56-209">Request</span></span>
<span data-ttu-id="9ee56-210">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9ee56-210">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1359

{
  "@odata.type": "#microsoft.graph.windows10ImportedPFXCertificateProfile",
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
  "intendedPurpose": "smimeEncryption"
}
```

### <a name="response"></a><span data-ttu-id="9ee56-211">响应</span><span class="sxs-lookup"><span data-stu-id="9ee56-211">Response</span></span>
<span data-ttu-id="9ee56-p118">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9ee56-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1531

{
  "@odata.type": "#microsoft.graph.windows10ImportedPFXCertificateProfile",
  "id": "b582514b-514b-b582-4b51-82b54b5182b5",
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
  "intendedPurpose": "smimeEncryption"
}
```



