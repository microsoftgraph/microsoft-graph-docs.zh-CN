---
title: 更新 windowsPhone81SCEPCertificateProfile
description: 更新 windowsPhone81SCEPCertificateProfile 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0f4be62b347f7a834c8f2000815ebc4c5defe0fa
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51147131"
---
# <a name="update-windowsphone81scepcertificateprofile"></a><span data-ttu-id="06764-103">更新 windowsPhone81SCEPCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="06764-103">Update windowsPhone81SCEPCertificateProfile</span></span>

<span data-ttu-id="06764-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="06764-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="06764-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="06764-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="06764-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="06764-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06764-107">更新 [windowsPhone81SCEPCertificateProfile 对象](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="06764-107">Update the properties of a [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="06764-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="06764-108">Prerequisites</span></span>
<span data-ttu-id="06764-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="06764-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06764-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="06764-111">Permission type</span></span>|<span data-ttu-id="06764-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="06764-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="06764-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="06764-113">Delegated (work or school account)</span></span>|<span data-ttu-id="06764-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06764-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="06764-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="06764-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="06764-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="06764-116">Not supported.</span></span>|
|<span data-ttu-id="06764-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="06764-117">Application</span></span>|<span data-ttu-id="06764-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06764-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="06764-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="06764-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="06764-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="06764-120">Request headers</span></span>
|<span data-ttu-id="06764-121">标头</span><span class="sxs-lookup"><span data-stu-id="06764-121">Header</span></span>|<span data-ttu-id="06764-122">值</span><span class="sxs-lookup"><span data-stu-id="06764-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="06764-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="06764-123">Authorization</span></span>|<span data-ttu-id="06764-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="06764-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="06764-125">接受</span><span class="sxs-lookup"><span data-stu-id="06764-125">Accept</span></span>|<span data-ttu-id="06764-126">application/json</span><span class="sxs-lookup"><span data-stu-id="06764-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="06764-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="06764-127">Request body</span></span>
<span data-ttu-id="06764-128">在请求正文中，提供 [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="06764-128">In the request body, supply a JSON representation for the [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) object.</span></span>

<span data-ttu-id="06764-129">下表显示创建 [windowsPhone81SCEPCertificateProfile 时所需的属性](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md)。</span><span class="sxs-lookup"><span data-stu-id="06764-129">The following table shows the properties that are required when you create the [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md).</span></span>

|<span data-ttu-id="06764-130">属性</span><span class="sxs-lookup"><span data-stu-id="06764-130">Property</span></span>|<span data-ttu-id="06764-131">类型</span><span class="sxs-lookup"><span data-stu-id="06764-131">Type</span></span>|<span data-ttu-id="06764-132">说明</span><span class="sxs-lookup"><span data-stu-id="06764-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06764-133">id</span><span class="sxs-lookup"><span data-stu-id="06764-133">id</span></span>|<span data-ttu-id="06764-134">String</span><span class="sxs-lookup"><span data-stu-id="06764-134">String</span></span>|<span data-ttu-id="06764-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="06764-135">Key of the entity.</span></span> <span data-ttu-id="06764-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06764-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06764-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="06764-137">lastModifiedDateTime</span></span>|<span data-ttu-id="06764-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06764-138">DateTimeOffset</span></span>|<span data-ttu-id="06764-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="06764-139">DateTime the object was last modified.</span></span> <span data-ttu-id="06764-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06764-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06764-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="06764-141">roleScopeTagIds</span></span>|<span data-ttu-id="06764-142">String collection</span><span class="sxs-lookup"><span data-stu-id="06764-142">String collection</span></span>|<span data-ttu-id="06764-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="06764-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="06764-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06764-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06764-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="06764-145">supportsScopeTags</span></span>|<span data-ttu-id="06764-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="06764-146">Boolean</span></span>|<span data-ttu-id="06764-147">指示基础设备配置是否支持分配范围标记。</span><span class="sxs-lookup"><span data-stu-id="06764-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="06764-148">当此值为 false 且实体对作用域用户不可见时，不允许分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="06764-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="06764-149">这适用于在 Silverlight 中创建的旧版策略，可通过在 Azure 门户中删除和重新创建策略来解决。</span><span class="sxs-lookup"><span data-stu-id="06764-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="06764-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="06764-150">This property is read-only.</span></span> <span data-ttu-id="06764-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06764-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06764-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="06764-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="06764-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="06764-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="06764-154">此策略的操作系统版本适用性。</span><span class="sxs-lookup"><span data-stu-id="06764-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="06764-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06764-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06764-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="06764-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="06764-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="06764-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="06764-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="06764-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="06764-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06764-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06764-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="06764-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="06764-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="06764-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="06764-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="06764-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="06764-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06764-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06764-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="06764-164">createdDateTime</span></span>|<span data-ttu-id="06764-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06764-165">DateTimeOffset</span></span>|<span data-ttu-id="06764-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="06764-166">DateTime the object was created.</span></span> <span data-ttu-id="06764-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06764-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06764-168">说明</span><span class="sxs-lookup"><span data-stu-id="06764-168">description</span></span>|<span data-ttu-id="06764-169">String</span><span class="sxs-lookup"><span data-stu-id="06764-169">String</span></span>|<span data-ttu-id="06764-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="06764-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="06764-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06764-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06764-172">displayName</span><span class="sxs-lookup"><span data-stu-id="06764-172">displayName</span></span>|<span data-ttu-id="06764-173">String</span><span class="sxs-lookup"><span data-stu-id="06764-173">String</span></span>|<span data-ttu-id="06764-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="06764-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="06764-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06764-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06764-176">version</span><span class="sxs-lookup"><span data-stu-id="06764-176">version</span></span>|<span data-ttu-id="06764-177">Int32</span><span class="sxs-lookup"><span data-stu-id="06764-177">Int32</span></span>|<span data-ttu-id="06764-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="06764-178">Version of the device configuration.</span></span> <span data-ttu-id="06764-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06764-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06764-180">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="06764-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="06764-181">Int32</span><span class="sxs-lookup"><span data-stu-id="06764-181">Int32</span></span>|<span data-ttu-id="06764-182">证书续订阈值百分比。</span><span class="sxs-lookup"><span data-stu-id="06764-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="06764-183">继承自 [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="06764-183">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="06764-184">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="06764-184">keyStorageProvider</span></span>|[<span data-ttu-id="06764-185">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="06764-185">keyStorageProviderOption</span></span>](../resources/intune-shared-keystorageprovideroption.md)|<span data-ttu-id="06764-186">密钥存储提供程序 (KSP) 。</span><span class="sxs-lookup"><span data-stu-id="06764-186">Key Storage Provider (KSP).</span></span> <span data-ttu-id="06764-187">继承自 [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="06764-187">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="06764-188">可取值为：`useTpmKspOtherwiseUseSoftwareKsp`、`useTpmKspOtherwiseFail`、`usePassportForWorkKspOtherwiseFail`、`useSoftwareKsp`。</span><span class="sxs-lookup"><span data-stu-id="06764-188">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="06764-189">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="06764-189">subjectNameFormat</span></span>|[<span data-ttu-id="06764-190">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="06764-190">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="06764-191">证书主题名称格式。</span><span class="sxs-lookup"><span data-stu-id="06764-191">Certificate Subject Name Format.</span></span> <span data-ttu-id="06764-192">继承自 [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="06764-192">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="06764-193">可取值为：`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId`。</span><span class="sxs-lookup"><span data-stu-id="06764-193">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="06764-194">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="06764-194">subjectAlternativeNameType</span></span>|[<span data-ttu-id="06764-195">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="06764-195">subjectAlternativeNameType</span></span>](../resources/intune-shared-subjectalternativenametype.md)|<span data-ttu-id="06764-196">证书主题备用名称类型。</span><span class="sxs-lookup"><span data-stu-id="06764-196">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="06764-197">继承自 [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="06764-197">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="06764-198">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService`、`universalResourceIdentifier`。</span><span class="sxs-lookup"><span data-stu-id="06764-198">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span></span>|
|<span data-ttu-id="06764-199">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="06764-199">certificateValidityPeriodValue</span></span>|<span data-ttu-id="06764-200">Int32</span><span class="sxs-lookup"><span data-stu-id="06764-200">Int32</span></span>|<span data-ttu-id="06764-201">证书有效期的值。</span><span class="sxs-lookup"><span data-stu-id="06764-201">Value for the Certificate Validtiy Period.</span></span> <span data-ttu-id="06764-202">继承自 [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="06764-202">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="06764-203">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="06764-203">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="06764-204">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="06764-204">certificateValidityPeriodScale</span></span>](../resources/intune-shared-certificatevalidityperiodscale.md)|<span data-ttu-id="06764-205">证书有效期的缩放。</span><span class="sxs-lookup"><span data-stu-id="06764-205">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="06764-206">继承自 [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="06764-206">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="06764-207">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="06764-207">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="06764-208">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="06764-208">extendedKeyUsages</span></span>|<span data-ttu-id="06764-209">[extendedKeyUsage](../resources/intune-shared-extendedkeyusage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="06764-209">[extendedKeyUsage](../resources/intune-shared-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="06764-210">EKU (扩展密钥) 设置。</span><span class="sxs-lookup"><span data-stu-id="06764-210">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="06764-211">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="06764-211">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="06764-212">继承自 [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="06764-212">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="06764-213">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="06764-213">scepServerUrls</span></span>|<span data-ttu-id="06764-214">String collection</span><span class="sxs-lookup"><span data-stu-id="06764-214">String collection</span></span>|<span data-ttu-id="06764-215">SCEP 服务器 URL () 。</span><span class="sxs-lookup"><span data-stu-id="06764-215">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="06764-216">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="06764-216">subjectNameFormatString</span></span>|<span data-ttu-id="06764-217">String</span><span class="sxs-lookup"><span data-stu-id="06764-217">String</span></span>|<span data-ttu-id="06764-218">要与 SubjectNameFormat 一同使用的自定义格式 = Custom。</span><span class="sxs-lookup"><span data-stu-id="06764-218">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="06764-219">示例：CN={{EmailAddress}}，E={{EmailAddress}，OU=Enterprise Users，O=Contoso Corporation，L=Redmond，ST=WA，C=US</span><span class="sxs-lookup"><span data-stu-id="06764-219">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="06764-220">keyUsage</span><span class="sxs-lookup"><span data-stu-id="06764-220">keyUsage</span></span>|[<span data-ttu-id="06764-221">keyUsages</span><span class="sxs-lookup"><span data-stu-id="06764-221">keyUsages</span></span>](../resources/intune-shared-keyusages.md)|<span data-ttu-id="06764-222">SCEP 密钥用法。</span><span class="sxs-lookup"><span data-stu-id="06764-222">SCEP Key Usage.</span></span> <span data-ttu-id="06764-223">可取值为：`keyEncipherment`、`digitalSignature`。</span><span class="sxs-lookup"><span data-stu-id="06764-223">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="06764-224">keySize</span><span class="sxs-lookup"><span data-stu-id="06764-224">keySize</span></span>|[<span data-ttu-id="06764-225">keySize</span><span class="sxs-lookup"><span data-stu-id="06764-225">keySize</span></span>](../resources/intune-shared-keysize.md)|<span data-ttu-id="06764-226">SCEP 密钥大小。</span><span class="sxs-lookup"><span data-stu-id="06764-226">SCEP Key Size.</span></span> <span data-ttu-id="06764-227">可取值为：`size1024`、`size2048`、`size4096`。</span><span class="sxs-lookup"><span data-stu-id="06764-227">Possible values are: `size1024`, `size2048`, `size4096`.</span></span>|
|<span data-ttu-id="06764-228">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="06764-228">hashAlgorithm</span></span>|[<span data-ttu-id="06764-229">hashAlgorithms</span><span class="sxs-lookup"><span data-stu-id="06764-229">hashAlgorithms</span></span>](../resources/intune-shared-hashalgorithms.md)|<span data-ttu-id="06764-230">SCEP 哈希算法。</span><span class="sxs-lookup"><span data-stu-id="06764-230">SCEP Hash Algorithm.</span></span> <span data-ttu-id="06764-231">可取值为：`sha1`、`sha2`。</span><span class="sxs-lookup"><span data-stu-id="06764-231">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="06764-232">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="06764-232">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="06764-233">String</span><span class="sxs-lookup"><span data-stu-id="06764-233">String</span></span>|<span data-ttu-id="06764-234">定义 AAD 属性的自定义字符串。</span><span class="sxs-lookup"><span data-stu-id="06764-234">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="06764-235">响应</span><span class="sxs-lookup"><span data-stu-id="06764-235">Response</span></span>
<span data-ttu-id="06764-236">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="06764-236">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06764-237">示例</span><span class="sxs-lookup"><span data-stu-id="06764-237">Example</span></span>

### <a name="request"></a><span data-ttu-id="06764-238">请求</span><span class="sxs-lookup"><span data-stu-id="06764-238">Request</span></span>
<span data-ttu-id="06764-239">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="06764-239">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1805

{
  "@odata.type": "#microsoft.graph.windowsPhone81SCEPCertificateProfile",
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

### <a name="response"></a><span data-ttu-id="06764-240">响应</span><span class="sxs-lookup"><span data-stu-id="06764-240">Response</span></span>
<span data-ttu-id="06764-p124">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="06764-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1977

{
  "@odata.type": "#microsoft.graph.windowsPhone81SCEPCertificateProfile",
  "id": "f070e30e-e30e-f070-0ee3-70f00ee370f0",
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




