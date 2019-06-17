---
title: 更新 windows81SCEPCertificateProfile
description: 更新 windows81SCEPCertificateProfile 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cc436e360de4964692d355a0c7517c3e459b7053
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34977749"
---
# <a name="update-windows81scepcertificateprofile"></a><span data-ttu-id="ef4fb-103">更新 windows81SCEPCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="ef4fb-103">Update windows81SCEPCertificateProfile</span></span>

> <span data-ttu-id="ef4fb-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ef4fb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ef4fb-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ef4fb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ef4fb-106">更新[windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ef4fb-106">Update the properties of a [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ef4fb-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="ef4fb-107">Prerequisites</span></span>
<span data-ttu-id="ef4fb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ef4fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef4fb-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ef4fb-110">Permission type</span></span>|<span data-ttu-id="ef4fb-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ef4fb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ef4fb-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ef4fb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ef4fb-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef4fb-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ef4fb-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ef4fb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ef4fb-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ef4fb-115">Not supported.</span></span>|
|<span data-ttu-id="ef4fb-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ef4fb-116">Application</span></span>|<span data-ttu-id="ef4fb-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="ef4fb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ef4fb-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ef4fb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ef4fb-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ef4fb-119">Request headers</span></span>
|<span data-ttu-id="ef4fb-120">标头</span><span class="sxs-lookup"><span data-stu-id="ef4fb-120">Header</span></span>|<span data-ttu-id="ef4fb-121">值</span><span class="sxs-lookup"><span data-stu-id="ef4fb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ef4fb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ef4fb-122">Authorization</span></span>|<span data-ttu-id="ef4fb-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ef4fb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ef4fb-124">接受</span><span class="sxs-lookup"><span data-stu-id="ef4fb-124">Accept</span></span>|<span data-ttu-id="ef4fb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ef4fb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef4fb-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ef4fb-126">Request body</span></span>
<span data-ttu-id="ef4fb-127">在请求正文中, 提供[windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ef4fb-127">In the request body, supply a JSON representation for the [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) object.</span></span>

<span data-ttu-id="ef4fb-128">下表显示创建[windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ef4fb-128">The following table shows the properties that are required when you create the [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md).</span></span>

|<span data-ttu-id="ef4fb-129">属性</span><span class="sxs-lookup"><span data-stu-id="ef4fb-129">Property</span></span>|<span data-ttu-id="ef4fb-130">类型</span><span class="sxs-lookup"><span data-stu-id="ef4fb-130">Type</span></span>|<span data-ttu-id="ef4fb-131">说明</span><span class="sxs-lookup"><span data-stu-id="ef4fb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef4fb-132">id</span><span class="sxs-lookup"><span data-stu-id="ef4fb-132">id</span></span>|<span data-ttu-id="ef4fb-133">字符串</span><span class="sxs-lookup"><span data-stu-id="ef4fb-133">String</span></span>|<span data-ttu-id="ef4fb-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="ef4fb-134">Key of the entity.</span></span> <span data-ttu-id="ef4fb-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef4fb-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef4fb-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ef4fb-136">lastModifiedDateTime</span></span>|<span data-ttu-id="ef4fb-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef4fb-137">DateTimeOffset</span></span>|<span data-ttu-id="ef4fb-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="ef4fb-138">DateTime the object was last modified.</span></span> <span data-ttu-id="ef4fb-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef4fb-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef4fb-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ef4fb-140">roleScopeTagIds</span></span>|<span data-ttu-id="ef4fb-141">String collection</span><span class="sxs-lookup"><span data-stu-id="ef4fb-141">String collection</span></span>|<span data-ttu-id="ef4fb-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="ef4fb-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ef4fb-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef4fb-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef4fb-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ef4fb-144">supportsScopeTags</span></span>|<span data-ttu-id="ef4fb-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="ef4fb-145">Boolean</span></span>|<span data-ttu-id="ef4fb-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="ef4fb-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ef4fb-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="ef4fb-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ef4fb-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="ef4fb-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ef4fb-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="ef4fb-149">This property is read-only.</span></span> <span data-ttu-id="ef4fb-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef4fb-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef4fb-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ef4fb-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="ef4fb-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ef4fb-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="ef4fb-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="ef4fb-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="ef4fb-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef4fb-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef4fb-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ef4fb-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="ef4fb-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ef4fb-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="ef4fb-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="ef4fb-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="ef4fb-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef4fb-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef4fb-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ef4fb-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="ef4fb-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ef4fb-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="ef4fb-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="ef4fb-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="ef4fb-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef4fb-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef4fb-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ef4fb-163">createdDateTime</span></span>|<span data-ttu-id="ef4fb-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef4fb-164">DateTimeOffset</span></span>|<span data-ttu-id="ef4fb-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="ef4fb-165">DateTime the object was created.</span></span> <span data-ttu-id="ef4fb-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef4fb-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef4fb-167">说明</span><span class="sxs-lookup"><span data-stu-id="ef4fb-167">description</span></span>|<span data-ttu-id="ef4fb-168">String</span><span class="sxs-lookup"><span data-stu-id="ef4fb-168">String</span></span>|<span data-ttu-id="ef4fb-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="ef4fb-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ef4fb-170">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef4fb-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef4fb-171">displayName</span><span class="sxs-lookup"><span data-stu-id="ef4fb-171">displayName</span></span>|<span data-ttu-id="ef4fb-172">String</span><span class="sxs-lookup"><span data-stu-id="ef4fb-172">String</span></span>|<span data-ttu-id="ef4fb-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="ef4fb-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ef4fb-174">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef4fb-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef4fb-175">version</span><span class="sxs-lookup"><span data-stu-id="ef4fb-175">version</span></span>|<span data-ttu-id="ef4fb-176">Int32</span><span class="sxs-lookup"><span data-stu-id="ef4fb-176">Int32</span></span>|<span data-ttu-id="ef4fb-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="ef4fb-177">Version of the device configuration.</span></span> <span data-ttu-id="ef4fb-178">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef4fb-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef4fb-179">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="ef4fb-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="ef4fb-180">Int32</span><span class="sxs-lookup"><span data-stu-id="ef4fb-180">Int32</span></span>|<span data-ttu-id="ef4fb-181">证书续订阈值百分比。</span><span class="sxs-lookup"><span data-stu-id="ef4fb-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="ef4fb-182">从[WindowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)继承的有效值1到99</span><span class="sxs-lookup"><span data-stu-id="ef4fb-182">Valid values 1 to 99 Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="ef4fb-183">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="ef4fb-183">keyStorageProvider</span></span>|[<span data-ttu-id="ef4fb-184">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="ef4fb-184">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="ef4fb-185">从[WindowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)继承的密钥存储提供程序 (KSP)。</span><span class="sxs-lookup"><span data-stu-id="ef4fb-185">Key Storage Provider (KSP) Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="ef4fb-186">可取值为：`useTpmKspOtherwiseUseSoftwareKsp`、`useTpmKspOtherwiseFail`、`usePassportForWorkKspOtherwiseFail`、`useSoftwareKsp`。</span><span class="sxs-lookup"><span data-stu-id="ef4fb-186">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="ef4fb-187">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="ef4fb-187">subjectNameFormat</span></span>|[<span data-ttu-id="ef4fb-188">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="ef4fb-188">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="ef4fb-189">证书使用者名称格式继承自[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="ef4fb-189">Certificate Subject Name Format Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="ef4fb-190">可取值为：`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId`。</span><span class="sxs-lookup"><span data-stu-id="ef4fb-190">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="ef4fb-191">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="ef4fb-191">subjectAlternativeNameType</span></span>|[<span data-ttu-id="ef4fb-192">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="ef4fb-192">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="ef4fb-193">证书使用者备用名称类型继承自[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="ef4fb-193">Certificate Subject Alternative Name Type Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="ef4fb-194">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService`。</span><span class="sxs-lookup"><span data-stu-id="ef4fb-194">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="ef4fb-195">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="ef4fb-195">certificateValidityPeriodValue</span></span>|<span data-ttu-id="ef4fb-196">Int32</span><span class="sxs-lookup"><span data-stu-id="ef4fb-196">Int32</span></span>|<span data-ttu-id="ef4fb-197">继承自[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)的证书有效期限的值</span><span class="sxs-lookup"><span data-stu-id="ef4fb-197">Value for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="ef4fb-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="ef4fb-198">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="ef4fb-199">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="ef4fb-199">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="ef4fb-200">从[WindowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)继承的证书有效期限的小数位数。</span><span class="sxs-lookup"><span data-stu-id="ef4fb-200">Scale for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="ef4fb-201">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="ef4fb-201">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="ef4fb-202">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="ef4fb-202">extendedKeyUsages</span></span>|<span data-ttu-id="ef4fb-203">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)集合</span><span class="sxs-lookup"><span data-stu-id="ef4fb-203">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="ef4fb-204">扩展密钥用法 (EKU) 设置。</span><span class="sxs-lookup"><span data-stu-id="ef4fb-204">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="ef4fb-205">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="ef4fb-205">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="ef4fb-206">继承自[windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="ef4fb-206">Inherited from [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="ef4fb-207">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="ef4fb-207">customSubjectAlternativeNames</span></span>|<span data-ttu-id="ef4fb-208">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)集合</span><span class="sxs-lookup"><span data-stu-id="ef4fb-208">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="ef4fb-209">自定义主题备用名称设置。</span><span class="sxs-lookup"><span data-stu-id="ef4fb-209">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="ef4fb-210">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="ef4fb-210">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="ef4fb-211">继承自[windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="ef4fb-211">Inherited from [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="ef4fb-212">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="ef4fb-212">scepServerUrls</span></span>|<span data-ttu-id="ef4fb-213">String collection</span><span class="sxs-lookup"><span data-stu-id="ef4fb-213">String collection</span></span>|<span data-ttu-id="ef4fb-214">SCEP 服务器 Url。</span><span class="sxs-lookup"><span data-stu-id="ef4fb-214">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="ef4fb-215">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="ef4fb-215">subjectNameFormatString</span></span>|<span data-ttu-id="ef4fb-216">String</span><span class="sxs-lookup"><span data-stu-id="ef4fb-216">String</span></span>|<span data-ttu-id="ef4fb-217">要与 SubjectNameFormat = Custom 一起使用的自定义格式。</span><span class="sxs-lookup"><span data-stu-id="ef4fb-217">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="ef4fb-218">示例: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = 企业用户, O = Contoso Corporation, L = Redmond, ST = WA, C = US</span><span class="sxs-lookup"><span data-stu-id="ef4fb-218">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="ef4fb-219">keyUsage</span><span class="sxs-lookup"><span data-stu-id="ef4fb-219">keyUsage</span></span>|[<span data-ttu-id="ef4fb-220">keyUsages</span><span class="sxs-lookup"><span data-stu-id="ef4fb-220">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="ef4fb-221">SCEP 密钥用法。</span><span class="sxs-lookup"><span data-stu-id="ef4fb-221">SCEP Key Usage.</span></span> <span data-ttu-id="ef4fb-222">可取值为：`keyEncipherment`、`digitalSignature`。</span><span class="sxs-lookup"><span data-stu-id="ef4fb-222">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="ef4fb-223">keySize</span><span class="sxs-lookup"><span data-stu-id="ef4fb-223">keySize</span></span>|[<span data-ttu-id="ef4fb-224">keySize</span><span class="sxs-lookup"><span data-stu-id="ef4fb-224">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="ef4fb-225">SCEP 密钥大小。</span><span class="sxs-lookup"><span data-stu-id="ef4fb-225">SCEP Key Size.</span></span> <span data-ttu-id="ef4fb-226">可取值为：`size1024`、`size2048`。</span><span class="sxs-lookup"><span data-stu-id="ef4fb-226">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="ef4fb-227">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="ef4fb-227">hashAlgorithm</span></span>|[<span data-ttu-id="ef4fb-228">hashAlgorithms</span><span class="sxs-lookup"><span data-stu-id="ef4fb-228">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="ef4fb-229">SCEP 哈希算法。</span><span class="sxs-lookup"><span data-stu-id="ef4fb-229">SCEP Hash Algorithm.</span></span> <span data-ttu-id="ef4fb-230">可取值为：`sha1`、`sha2`。</span><span class="sxs-lookup"><span data-stu-id="ef4fb-230">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="ef4fb-231">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="ef4fb-231">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="ef4fb-232">String</span><span class="sxs-lookup"><span data-stu-id="ef4fb-232">String</span></span>|<span data-ttu-id="ef4fb-233">定义 AAD 属性的自定义字符串。</span><span class="sxs-lookup"><span data-stu-id="ef4fb-233">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="ef4fb-234">certificateStore</span><span class="sxs-lookup"><span data-stu-id="ef4fb-234">certificateStore</span></span>|[<span data-ttu-id="ef4fb-235">certificateStore</span><span class="sxs-lookup"><span data-stu-id="ef4fb-235">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="ef4fb-236">目标存储证书。</span><span class="sxs-lookup"><span data-stu-id="ef4fb-236">Target store certificate.</span></span> <span data-ttu-id="ef4fb-237">可取值为：`user`、`machine`。</span><span class="sxs-lookup"><span data-stu-id="ef4fb-237">Possible values are: `user`, `machine`.</span></span>|



## <a name="response"></a><span data-ttu-id="ef4fb-238">响应</span><span class="sxs-lookup"><span data-stu-id="ef4fb-238">Response</span></span>
<span data-ttu-id="ef4fb-239">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ef4fb-239">If successful, this method returns a `200 OK` response code and an updated [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ef4fb-240">示例</span><span class="sxs-lookup"><span data-stu-id="ef4fb-240">Example</span></span>

### <a name="request"></a><span data-ttu-id="ef4fb-241">请求</span><span class="sxs-lookup"><span data-stu-id="ef4fb-241">Request</span></span>
<span data-ttu-id="ef4fb-242">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ef4fb-242">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2024

{
  "@odata.type": "#microsoft.graph.windows81SCEPCertificateProfile",
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
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "customSubjectAlternativeNames": [
    {
      "@odata.type": "microsoft.graph.customSubjectAlternativeName",
      "sanType": "emailAddress",
      "name": "Name value"
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
  "certificateStore": "machine"
}
```

### <a name="response"></a><span data-ttu-id="ef4fb-243">响应</span><span class="sxs-lookup"><span data-stu-id="ef4fb-243">Response</span></span>
<span data-ttu-id="ef4fb-p125">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ef4fb-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2196

{
  "@odata.type": "#microsoft.graph.windows81SCEPCertificateProfile",
  "id": "2daf8af2-8af2-2daf-f28a-af2df28aaf2d",
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
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "customSubjectAlternativeNames": [
    {
      "@odata.type": "microsoft.graph.customSubjectAlternativeName",
      "sanType": "emailAddress",
      "name": "Name value"
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
  "certificateStore": "machine"
}
```





