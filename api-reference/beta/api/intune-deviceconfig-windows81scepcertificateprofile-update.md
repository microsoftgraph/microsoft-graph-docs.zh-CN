---
title: 更新 windows81SCEPCertificateProfile
description: 更新 windows81SCEPCertificateProfile 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9f3acc143eaeb30e1e794df3b4c739a8a8bd9e7f
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48723558"
---
# <a name="update-windows81scepcertificateprofile"></a><span data-ttu-id="eae49-103">更新 windows81SCEPCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="eae49-103">Update windows81SCEPCertificateProfile</span></span>

<span data-ttu-id="eae49-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eae49-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="eae49-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="eae49-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eae49-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="eae49-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eae49-107">更新 [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="eae49-107">Update the properties of a [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eae49-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="eae49-108">Prerequisites</span></span>
<span data-ttu-id="eae49-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="eae49-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eae49-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="eae49-111">Permission type</span></span>|<span data-ttu-id="eae49-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="eae49-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eae49-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="eae49-113">Delegated (work or school account)</span></span>|<span data-ttu-id="eae49-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eae49-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="eae49-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="eae49-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eae49-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="eae49-116">Not supported.</span></span>|
|<span data-ttu-id="eae49-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="eae49-117">Application</span></span>|<span data-ttu-id="eae49-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eae49-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="eae49-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="eae49-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="eae49-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="eae49-120">Request headers</span></span>
|<span data-ttu-id="eae49-121">标头</span><span class="sxs-lookup"><span data-stu-id="eae49-121">Header</span></span>|<span data-ttu-id="eae49-122">值</span><span class="sxs-lookup"><span data-stu-id="eae49-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eae49-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="eae49-123">Authorization</span></span>|<span data-ttu-id="eae49-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="eae49-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eae49-125">接受</span><span class="sxs-lookup"><span data-stu-id="eae49-125">Accept</span></span>|<span data-ttu-id="eae49-126">application/json</span><span class="sxs-lookup"><span data-stu-id="eae49-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eae49-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="eae49-127">Request body</span></span>
<span data-ttu-id="eae49-128">在请求正文中，提供 [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="eae49-128">In the request body, supply a JSON representation for the [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) object.</span></span>

<span data-ttu-id="eae49-129">下表显示创建 [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="eae49-129">The following table shows the properties that are required when you create the [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md).</span></span>

|<span data-ttu-id="eae49-130">属性</span><span class="sxs-lookup"><span data-stu-id="eae49-130">Property</span></span>|<span data-ttu-id="eae49-131">类型</span><span class="sxs-lookup"><span data-stu-id="eae49-131">Type</span></span>|<span data-ttu-id="eae49-132">说明</span><span class="sxs-lookup"><span data-stu-id="eae49-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eae49-133">id</span><span class="sxs-lookup"><span data-stu-id="eae49-133">id</span></span>|<span data-ttu-id="eae49-134">String</span><span class="sxs-lookup"><span data-stu-id="eae49-134">String</span></span>|<span data-ttu-id="eae49-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="eae49-135">Key of the entity.</span></span> <span data-ttu-id="eae49-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="eae49-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eae49-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="eae49-137">lastModifiedDateTime</span></span>|<span data-ttu-id="eae49-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eae49-138">DateTimeOffset</span></span>|<span data-ttu-id="eae49-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="eae49-139">DateTime the object was last modified.</span></span> <span data-ttu-id="eae49-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="eae49-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eae49-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="eae49-141">roleScopeTagIds</span></span>|<span data-ttu-id="eae49-142">String collection</span><span class="sxs-lookup"><span data-stu-id="eae49-142">String collection</span></span>|<span data-ttu-id="eae49-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="eae49-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="eae49-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="eae49-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eae49-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="eae49-145">supportsScopeTags</span></span>|<span data-ttu-id="eae49-146">布尔</span><span class="sxs-lookup"><span data-stu-id="eae49-146">Boolean</span></span>|<span data-ttu-id="eae49-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="eae49-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="eae49-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="eae49-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="eae49-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="eae49-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="eae49-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="eae49-150">This property is read-only.</span></span> <span data-ttu-id="eae49-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="eae49-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eae49-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="eae49-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="eae49-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="eae49-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="eae49-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="eae49-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="eae49-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="eae49-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eae49-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="eae49-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="eae49-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="eae49-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="eae49-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="eae49-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="eae49-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="eae49-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eae49-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="eae49-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="eae49-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="eae49-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="eae49-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="eae49-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="eae49-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="eae49-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eae49-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="eae49-164">createdDateTime</span></span>|<span data-ttu-id="eae49-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eae49-165">DateTimeOffset</span></span>|<span data-ttu-id="eae49-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="eae49-166">DateTime the object was created.</span></span> <span data-ttu-id="eae49-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="eae49-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eae49-168">说明</span><span class="sxs-lookup"><span data-stu-id="eae49-168">description</span></span>|<span data-ttu-id="eae49-169">String</span><span class="sxs-lookup"><span data-stu-id="eae49-169">String</span></span>|<span data-ttu-id="eae49-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="eae49-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="eae49-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="eae49-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eae49-172">displayName</span><span class="sxs-lookup"><span data-stu-id="eae49-172">displayName</span></span>|<span data-ttu-id="eae49-173">String</span><span class="sxs-lookup"><span data-stu-id="eae49-173">String</span></span>|<span data-ttu-id="eae49-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="eae49-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="eae49-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="eae49-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eae49-176">version</span><span class="sxs-lookup"><span data-stu-id="eae49-176">version</span></span>|<span data-ttu-id="eae49-177">Int32</span><span class="sxs-lookup"><span data-stu-id="eae49-177">Int32</span></span>|<span data-ttu-id="eae49-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="eae49-178">Version of the device configuration.</span></span> <span data-ttu-id="eae49-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="eae49-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eae49-180">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="eae49-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="eae49-181">Int32</span><span class="sxs-lookup"><span data-stu-id="eae49-181">Int32</span></span>|<span data-ttu-id="eae49-182">证书续订阈值百分比。</span><span class="sxs-lookup"><span data-stu-id="eae49-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="eae49-183">从[WindowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)继承的有效值1到99</span><span class="sxs-lookup"><span data-stu-id="eae49-183">Valid values 1 to 99 Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="eae49-184">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="eae49-184">keyStorageProvider</span></span>|[<span data-ttu-id="eae49-185">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="eae49-185">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="eae49-186">密钥存储提供程序 (KSP) 继承自 [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="eae49-186">Key Storage Provider (KSP) Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="eae49-187">可取值为：`useTpmKspOtherwiseUseSoftwareKsp`、`useTpmKspOtherwiseFail`、`usePassportForWorkKspOtherwiseFail`、`useSoftwareKsp`。</span><span class="sxs-lookup"><span data-stu-id="eae49-187">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="eae49-188">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="eae49-188">subjectNameFormat</span></span>|[<span data-ttu-id="eae49-189">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="eae49-189">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="eae49-190">证书使用者名称格式继承自 [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="eae49-190">Certificate Subject Name Format Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="eae49-191">可取值为：`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId`。</span><span class="sxs-lookup"><span data-stu-id="eae49-191">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="eae49-192">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="eae49-192">subjectAlternativeNameType</span></span>|[<span data-ttu-id="eae49-193">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="eae49-193">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="eae49-194">证书使用者备用名称类型继承自 [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="eae49-194">Certificate Subject Alternative Name Type Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="eae49-195">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService`、`universalResourceIdentifier`。</span><span class="sxs-lookup"><span data-stu-id="eae49-195">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span></span>|
|<span data-ttu-id="eae49-196">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="eae49-196">certificateValidityPeriodValue</span></span>|<span data-ttu-id="eae49-197">Int32</span><span class="sxs-lookup"><span data-stu-id="eae49-197">Int32</span></span>|<span data-ttu-id="eae49-198">继承自[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)的证书有效期限的值</span><span class="sxs-lookup"><span data-stu-id="eae49-198">Value for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="eae49-199">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="eae49-199">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="eae49-200">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="eae49-200">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="eae49-201">从 [WindowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)继承的证书有效期限的小数位数。</span><span class="sxs-lookup"><span data-stu-id="eae49-201">Scale for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="eae49-202">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="eae49-202">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="eae49-203">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="eae49-203">extendedKeyUsages</span></span>|<span data-ttu-id="eae49-204">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="eae49-204">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="eae49-205"> (EKU) 设置的扩展密钥用法。</span><span class="sxs-lookup"><span data-stu-id="eae49-205">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="eae49-206">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="eae49-206">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="eae49-207">继承自 [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="eae49-207">Inherited from [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="eae49-208">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="eae49-208">customSubjectAlternativeNames</span></span>|<span data-ttu-id="eae49-209">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) 集合</span><span class="sxs-lookup"><span data-stu-id="eae49-209">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="eae49-210">自定义主题备用名称设置。</span><span class="sxs-lookup"><span data-stu-id="eae49-210">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="eae49-211">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="eae49-211">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="eae49-212">继承自 [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="eae49-212">Inherited from [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="eae49-213">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="eae49-213">scepServerUrls</span></span>|<span data-ttu-id="eae49-214">String collection</span><span class="sxs-lookup"><span data-stu-id="eae49-214">String collection</span></span>|<span data-ttu-id="eae49-215">SCEP (s) 的服务器 Url。</span><span class="sxs-lookup"><span data-stu-id="eae49-215">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="eae49-216">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="eae49-216">subjectNameFormatString</span></span>|<span data-ttu-id="eae49-217">String</span><span class="sxs-lookup"><span data-stu-id="eae49-217">String</span></span>|<span data-ttu-id="eae49-218">要与 SubjectNameFormat = Custom 一起使用的自定义格式。</span><span class="sxs-lookup"><span data-stu-id="eae49-218">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="eae49-219">示例： CN = {{EmailAddress}}，E = {{EmailAddress}}，OU = 企业用户，O = Contoso Corporation，L = Redmond，ST = WA，C = US</span><span class="sxs-lookup"><span data-stu-id="eae49-219">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="eae49-220">keyUsage</span><span class="sxs-lookup"><span data-stu-id="eae49-220">keyUsage</span></span>|[<span data-ttu-id="eae49-221">keyUsages</span><span class="sxs-lookup"><span data-stu-id="eae49-221">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="eae49-222">SCEP 密钥用法。</span><span class="sxs-lookup"><span data-stu-id="eae49-222">SCEP Key Usage.</span></span> <span data-ttu-id="eae49-223">可取值为：`keyEncipherment`、`digitalSignature`。</span><span class="sxs-lookup"><span data-stu-id="eae49-223">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="eae49-224">keySize</span><span class="sxs-lookup"><span data-stu-id="eae49-224">keySize</span></span>|[<span data-ttu-id="eae49-225">keySize</span><span class="sxs-lookup"><span data-stu-id="eae49-225">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="eae49-226">SCEP 密钥大小。</span><span class="sxs-lookup"><span data-stu-id="eae49-226">SCEP Key Size.</span></span> <span data-ttu-id="eae49-227">可取值为：`size1024`、`size2048`、`size4096`。</span><span class="sxs-lookup"><span data-stu-id="eae49-227">Possible values are: `size1024`, `size2048`, `size4096`.</span></span>|
|<span data-ttu-id="eae49-228">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="eae49-228">hashAlgorithm</span></span>|[<span data-ttu-id="eae49-229">hashAlgorithms</span><span class="sxs-lookup"><span data-stu-id="eae49-229">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="eae49-230">SCEP 哈希算法。</span><span class="sxs-lookup"><span data-stu-id="eae49-230">SCEP Hash Algorithm.</span></span> <span data-ttu-id="eae49-231">可取值为：`sha1`、`sha2`。</span><span class="sxs-lookup"><span data-stu-id="eae49-231">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="eae49-232">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="eae49-232">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="eae49-233">String</span><span class="sxs-lookup"><span data-stu-id="eae49-233">String</span></span>|<span data-ttu-id="eae49-234">定义 AAD 属性的自定义字符串。</span><span class="sxs-lookup"><span data-stu-id="eae49-234">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="eae49-235">certificateStore</span><span class="sxs-lookup"><span data-stu-id="eae49-235">certificateStore</span></span>|[<span data-ttu-id="eae49-236">certificateStore</span><span class="sxs-lookup"><span data-stu-id="eae49-236">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="eae49-237">目标存储证书。</span><span class="sxs-lookup"><span data-stu-id="eae49-237">Target store certificate.</span></span> <span data-ttu-id="eae49-238">可取值为：`user`、`machine`。</span><span class="sxs-lookup"><span data-stu-id="eae49-238">Possible values are: `user`, `machine`.</span></span>|



## <a name="response"></a><span data-ttu-id="eae49-239">响应</span><span class="sxs-lookup"><span data-stu-id="eae49-239">Response</span></span>
<span data-ttu-id="eae49-240">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="eae49-240">If successful, this method returns a `200 OK` response code and an updated [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eae49-241">示例</span><span class="sxs-lookup"><span data-stu-id="eae49-241">Example</span></span>

### <a name="request"></a><span data-ttu-id="eae49-242">请求</span><span class="sxs-lookup"><span data-stu-id="eae49-242">Request</span></span>
<span data-ttu-id="eae49-243">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="eae49-243">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="eae49-244">响应</span><span class="sxs-lookup"><span data-stu-id="eae49-244">Response</span></span>
<span data-ttu-id="eae49-p125">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="eae49-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





