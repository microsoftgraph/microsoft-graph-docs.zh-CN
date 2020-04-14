---
title: 更新 windowsPhone81SCEPCertificateProfile
description: 更新 windowsPhone81SCEPCertificateProfile 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 56bafa73e4e877dccc48b16c9106bf581db8e3ad
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43429275"
---
# <a name="update-windowsphone81scepcertificateprofile"></a><span data-ttu-id="2df08-103">更新 windowsPhone81SCEPCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="2df08-103">Update windowsPhone81SCEPCertificateProfile</span></span>

<span data-ttu-id="2df08-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2df08-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2df08-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2df08-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2df08-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2df08-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2df08-107">更新[windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="2df08-107">Update the properties of a [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2df08-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="2df08-108">Prerequisites</span></span>
<span data-ttu-id="2df08-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2df08-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2df08-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="2df08-111">Permission type</span></span>|<span data-ttu-id="2df08-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2df08-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2df08-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2df08-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2df08-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2df08-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2df08-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2df08-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2df08-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2df08-116">Not supported.</span></span>|
|<span data-ttu-id="2df08-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="2df08-117">Application</span></span>|<span data-ttu-id="2df08-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2df08-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2df08-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2df08-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="2df08-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="2df08-120">Request headers</span></span>
|<span data-ttu-id="2df08-121">标头</span><span class="sxs-lookup"><span data-stu-id="2df08-121">Header</span></span>|<span data-ttu-id="2df08-122">值</span><span class="sxs-lookup"><span data-stu-id="2df08-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2df08-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2df08-123">Authorization</span></span>|<span data-ttu-id="2df08-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2df08-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2df08-125">接受</span><span class="sxs-lookup"><span data-stu-id="2df08-125">Accept</span></span>|<span data-ttu-id="2df08-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2df08-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2df08-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2df08-127">Request body</span></span>
<span data-ttu-id="2df08-128">在请求正文中，提供[windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2df08-128">In the request body, supply a JSON representation for the [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) object.</span></span>

<span data-ttu-id="2df08-129">下表显示创建[windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2df08-129">The following table shows the properties that are required when you create the [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md).</span></span>

|<span data-ttu-id="2df08-130">属性</span><span class="sxs-lookup"><span data-stu-id="2df08-130">Property</span></span>|<span data-ttu-id="2df08-131">类型</span><span class="sxs-lookup"><span data-stu-id="2df08-131">Type</span></span>|<span data-ttu-id="2df08-132">说明</span><span class="sxs-lookup"><span data-stu-id="2df08-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2df08-133">id</span><span class="sxs-lookup"><span data-stu-id="2df08-133">id</span></span>|<span data-ttu-id="2df08-134">字符串</span><span class="sxs-lookup"><span data-stu-id="2df08-134">String</span></span>|<span data-ttu-id="2df08-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="2df08-135">Key of the entity.</span></span> <span data-ttu-id="2df08-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2df08-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2df08-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2df08-137">lastModifiedDateTime</span></span>|<span data-ttu-id="2df08-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2df08-138">DateTimeOffset</span></span>|<span data-ttu-id="2df08-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="2df08-139">DateTime the object was last modified.</span></span> <span data-ttu-id="2df08-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2df08-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2df08-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2df08-141">roleScopeTagIds</span></span>|<span data-ttu-id="2df08-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="2df08-142">String collection</span></span>|<span data-ttu-id="2df08-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="2df08-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="2df08-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2df08-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2df08-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="2df08-145">supportsScopeTags</span></span>|<span data-ttu-id="2df08-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="2df08-146">Boolean</span></span>|<span data-ttu-id="2df08-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="2df08-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="2df08-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="2df08-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="2df08-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="2df08-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="2df08-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="2df08-150">This property is read-only.</span></span> <span data-ttu-id="2df08-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2df08-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2df08-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="2df08-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="2df08-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="2df08-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="2df08-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="2df08-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="2df08-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2df08-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2df08-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="2df08-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="2df08-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="2df08-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="2df08-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="2df08-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="2df08-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2df08-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2df08-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="2df08-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="2df08-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="2df08-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="2df08-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="2df08-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="2df08-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2df08-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2df08-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2df08-164">createdDateTime</span></span>|<span data-ttu-id="2df08-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2df08-165">DateTimeOffset</span></span>|<span data-ttu-id="2df08-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="2df08-166">DateTime the object was created.</span></span> <span data-ttu-id="2df08-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2df08-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2df08-168">description</span><span class="sxs-lookup"><span data-stu-id="2df08-168">description</span></span>|<span data-ttu-id="2df08-169">String</span><span class="sxs-lookup"><span data-stu-id="2df08-169">String</span></span>|<span data-ttu-id="2df08-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="2df08-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2df08-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2df08-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2df08-172">displayName</span><span class="sxs-lookup"><span data-stu-id="2df08-172">displayName</span></span>|<span data-ttu-id="2df08-173">String</span><span class="sxs-lookup"><span data-stu-id="2df08-173">String</span></span>|<span data-ttu-id="2df08-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="2df08-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2df08-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2df08-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2df08-176">version</span><span class="sxs-lookup"><span data-stu-id="2df08-176">version</span></span>|<span data-ttu-id="2df08-177">Int32</span><span class="sxs-lookup"><span data-stu-id="2df08-177">Int32</span></span>|<span data-ttu-id="2df08-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="2df08-178">Version of the device configuration.</span></span> <span data-ttu-id="2df08-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2df08-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2df08-180">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="2df08-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="2df08-181">Int32</span><span class="sxs-lookup"><span data-stu-id="2df08-181">Int32</span></span>|<span data-ttu-id="2df08-182">证书续订阈值百分比。</span><span class="sxs-lookup"><span data-stu-id="2df08-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="2df08-183">继承自[windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="2df08-183">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="2df08-184">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="2df08-184">keyStorageProvider</span></span>|[<span data-ttu-id="2df08-185">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="2df08-185">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="2df08-186">密钥存储提供程序（KSP）。</span><span class="sxs-lookup"><span data-stu-id="2df08-186">Key Storage Provider (KSP).</span></span> <span data-ttu-id="2df08-187">继承自[windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="2df08-187">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="2df08-188">可取值为：`useTpmKspOtherwiseUseSoftwareKsp`、`useTpmKspOtherwiseFail`、`usePassportForWorkKspOtherwiseFail`、`useSoftwareKsp`。</span><span class="sxs-lookup"><span data-stu-id="2df08-188">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="2df08-189">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="2df08-189">subjectNameFormat</span></span>|[<span data-ttu-id="2df08-190">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="2df08-190">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="2df08-191">证书使用者名称格式。</span><span class="sxs-lookup"><span data-stu-id="2df08-191">Certificate Subject Name Format.</span></span> <span data-ttu-id="2df08-192">继承自[windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="2df08-192">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="2df08-193">可取值为：`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId`。</span><span class="sxs-lookup"><span data-stu-id="2df08-193">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="2df08-194">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="2df08-194">subjectAlternativeNameType</span></span>|[<span data-ttu-id="2df08-195">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="2df08-195">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="2df08-196">证书使用者备用名称类型。</span><span class="sxs-lookup"><span data-stu-id="2df08-196">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="2df08-197">继承自[windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="2df08-197">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="2df08-198">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService`。</span><span class="sxs-lookup"><span data-stu-id="2df08-198">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="2df08-199">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="2df08-199">certificateValidityPeriodValue</span></span>|<span data-ttu-id="2df08-200">Int32</span><span class="sxs-lookup"><span data-stu-id="2df08-200">Int32</span></span>|<span data-ttu-id="2df08-201">证书 Validtiy 期限的值。</span><span class="sxs-lookup"><span data-stu-id="2df08-201">Value for the Certificate Validtiy Period.</span></span> <span data-ttu-id="2df08-202">继承自[windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="2df08-202">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="2df08-203">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="2df08-203">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="2df08-204">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="2df08-204">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="2df08-205">证书有效期的小数位数。</span><span class="sxs-lookup"><span data-stu-id="2df08-205">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="2df08-206">继承自[windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="2df08-206">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="2df08-207">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="2df08-207">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="2df08-208">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="2df08-208">extendedKeyUsages</span></span>|<span data-ttu-id="2df08-209">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)集合</span><span class="sxs-lookup"><span data-stu-id="2df08-209">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="2df08-210">扩展密钥用法（EKU）设置。</span><span class="sxs-lookup"><span data-stu-id="2df08-210">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="2df08-211">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="2df08-211">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="2df08-212">继承自[windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="2df08-212">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="2df08-213">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="2df08-213">scepServerUrls</span></span>|<span data-ttu-id="2df08-214">String 集合</span><span class="sxs-lookup"><span data-stu-id="2df08-214">String collection</span></span>|<span data-ttu-id="2df08-215">SCEP 服务器 Url。</span><span class="sxs-lookup"><span data-stu-id="2df08-215">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="2df08-216">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="2df08-216">subjectNameFormatString</span></span>|<span data-ttu-id="2df08-217">String</span><span class="sxs-lookup"><span data-stu-id="2df08-217">String</span></span>|<span data-ttu-id="2df08-218">要与 SubjectNameFormat = Custom 一起使用的自定义格式。</span><span class="sxs-lookup"><span data-stu-id="2df08-218">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="2df08-219">示例： CN = {{EmailAddress}}，E = {{EmailAddress}}，OU = 企业用户，O = Contoso Corporation，L = Redmond，ST = WA，C = US</span><span class="sxs-lookup"><span data-stu-id="2df08-219">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="2df08-220">keyUsage</span><span class="sxs-lookup"><span data-stu-id="2df08-220">keyUsage</span></span>|[<span data-ttu-id="2df08-221">keyUsages</span><span class="sxs-lookup"><span data-stu-id="2df08-221">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="2df08-222">SCEP 密钥用法。</span><span class="sxs-lookup"><span data-stu-id="2df08-222">SCEP Key Usage.</span></span> <span data-ttu-id="2df08-223">可取值为：`keyEncipherment`、`digitalSignature`。</span><span class="sxs-lookup"><span data-stu-id="2df08-223">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="2df08-224">keySize</span><span class="sxs-lookup"><span data-stu-id="2df08-224">keySize</span></span>|[<span data-ttu-id="2df08-225">keySize</span><span class="sxs-lookup"><span data-stu-id="2df08-225">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="2df08-226">SCEP 密钥大小。</span><span class="sxs-lookup"><span data-stu-id="2df08-226">SCEP Key Size.</span></span> <span data-ttu-id="2df08-227">可取值为：`size1024`、`size2048`。</span><span class="sxs-lookup"><span data-stu-id="2df08-227">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="2df08-228">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="2df08-228">hashAlgorithm</span></span>|[<span data-ttu-id="2df08-229">hashAlgorithms</span><span class="sxs-lookup"><span data-stu-id="2df08-229">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="2df08-230">SCEP 哈希算法。</span><span class="sxs-lookup"><span data-stu-id="2df08-230">SCEP Hash Algorithm.</span></span> <span data-ttu-id="2df08-231">可取值为：`sha1`、`sha2`。</span><span class="sxs-lookup"><span data-stu-id="2df08-231">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="2df08-232">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="2df08-232">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="2df08-233">String</span><span class="sxs-lookup"><span data-stu-id="2df08-233">String</span></span>|<span data-ttu-id="2df08-234">定义 AAD 属性的自定义字符串。</span><span class="sxs-lookup"><span data-stu-id="2df08-234">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="2df08-235">响应</span><span class="sxs-lookup"><span data-stu-id="2df08-235">Response</span></span>
<span data-ttu-id="2df08-236">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2df08-236">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2df08-237">示例</span><span class="sxs-lookup"><span data-stu-id="2df08-237">Example</span></span>

### <a name="request"></a><span data-ttu-id="2df08-238">请求</span><span class="sxs-lookup"><span data-stu-id="2df08-238">Request</span></span>
<span data-ttu-id="2df08-239">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2df08-239">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2df08-240">响应</span><span class="sxs-lookup"><span data-stu-id="2df08-240">Response</span></span>
<span data-ttu-id="2df08-p124">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2df08-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



