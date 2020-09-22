---
title: 更新 windows81SCEPCertificateProfile
description: 更新 windows81SCEPCertificateProfile 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 147af4c10c78ce20914415b1e4208c053d0fc8ec
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48014698"
---
# <a name="update-windows81scepcertificateprofile"></a><span data-ttu-id="bc02f-103">更新 windows81SCEPCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="bc02f-103">Update windows81SCEPCertificateProfile</span></span>

<span data-ttu-id="bc02f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bc02f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bc02f-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bc02f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bc02f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bc02f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc02f-107">更新 [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="bc02f-107">Update the properties of a [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bc02f-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="bc02f-108">Prerequisites</span></span>
<span data-ttu-id="bc02f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bc02f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc02f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="bc02f-111">Permission type</span></span>|<span data-ttu-id="bc02f-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="bc02f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bc02f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bc02f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bc02f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc02f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bc02f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bc02f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bc02f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bc02f-116">Not supported.</span></span>|
|<span data-ttu-id="bc02f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="bc02f-117">Application</span></span>|<span data-ttu-id="bc02f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc02f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bc02f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bc02f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="bc02f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="bc02f-120">Request headers</span></span>
|<span data-ttu-id="bc02f-121">标头</span><span class="sxs-lookup"><span data-stu-id="bc02f-121">Header</span></span>|<span data-ttu-id="bc02f-122">值</span><span class="sxs-lookup"><span data-stu-id="bc02f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bc02f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bc02f-123">Authorization</span></span>|<span data-ttu-id="bc02f-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="bc02f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bc02f-125">接受</span><span class="sxs-lookup"><span data-stu-id="bc02f-125">Accept</span></span>|<span data-ttu-id="bc02f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bc02f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bc02f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="bc02f-127">Request body</span></span>
<span data-ttu-id="bc02f-128">在请求正文中，提供 [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bc02f-128">In the request body, supply a JSON representation for the [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) object.</span></span>

<span data-ttu-id="bc02f-129">下表显示创建 [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="bc02f-129">The following table shows the properties that are required when you create the [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md).</span></span>

|<span data-ttu-id="bc02f-130">属性</span><span class="sxs-lookup"><span data-stu-id="bc02f-130">Property</span></span>|<span data-ttu-id="bc02f-131">类型</span><span class="sxs-lookup"><span data-stu-id="bc02f-131">Type</span></span>|<span data-ttu-id="bc02f-132">说明</span><span class="sxs-lookup"><span data-stu-id="bc02f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc02f-133">id</span><span class="sxs-lookup"><span data-stu-id="bc02f-133">id</span></span>|<span data-ttu-id="bc02f-134">String</span><span class="sxs-lookup"><span data-stu-id="bc02f-134">String</span></span>|<span data-ttu-id="bc02f-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="bc02f-135">Key of the entity.</span></span> <span data-ttu-id="bc02f-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bc02f-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bc02f-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bc02f-137">lastModifiedDateTime</span></span>|<span data-ttu-id="bc02f-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc02f-138">DateTimeOffset</span></span>|<span data-ttu-id="bc02f-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="bc02f-139">DateTime the object was last modified.</span></span> <span data-ttu-id="bc02f-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bc02f-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bc02f-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="bc02f-141">roleScopeTagIds</span></span>|<span data-ttu-id="bc02f-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="bc02f-142">String collection</span></span>|<span data-ttu-id="bc02f-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="bc02f-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="bc02f-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bc02f-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bc02f-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="bc02f-145">supportsScopeTags</span></span>|<span data-ttu-id="bc02f-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc02f-146">Boolean</span></span>|<span data-ttu-id="bc02f-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="bc02f-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="bc02f-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="bc02f-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="bc02f-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="bc02f-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="bc02f-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="bc02f-150">This property is read-only.</span></span> <span data-ttu-id="bc02f-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bc02f-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bc02f-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="bc02f-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="bc02f-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="bc02f-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="bc02f-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="bc02f-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="bc02f-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bc02f-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bc02f-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="bc02f-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="bc02f-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="bc02f-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="bc02f-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="bc02f-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="bc02f-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bc02f-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bc02f-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="bc02f-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="bc02f-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="bc02f-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="bc02f-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="bc02f-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="bc02f-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bc02f-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bc02f-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bc02f-164">createdDateTime</span></span>|<span data-ttu-id="bc02f-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc02f-165">DateTimeOffset</span></span>|<span data-ttu-id="bc02f-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="bc02f-166">DateTime the object was created.</span></span> <span data-ttu-id="bc02f-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bc02f-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bc02f-168">description</span><span class="sxs-lookup"><span data-stu-id="bc02f-168">description</span></span>|<span data-ttu-id="bc02f-169">String</span><span class="sxs-lookup"><span data-stu-id="bc02f-169">String</span></span>|<span data-ttu-id="bc02f-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="bc02f-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="bc02f-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bc02f-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bc02f-172">displayName</span><span class="sxs-lookup"><span data-stu-id="bc02f-172">displayName</span></span>|<span data-ttu-id="bc02f-173">String</span><span class="sxs-lookup"><span data-stu-id="bc02f-173">String</span></span>|<span data-ttu-id="bc02f-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="bc02f-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="bc02f-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bc02f-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bc02f-176">version</span><span class="sxs-lookup"><span data-stu-id="bc02f-176">version</span></span>|<span data-ttu-id="bc02f-177">Int32</span><span class="sxs-lookup"><span data-stu-id="bc02f-177">Int32</span></span>|<span data-ttu-id="bc02f-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="bc02f-178">Version of the device configuration.</span></span> <span data-ttu-id="bc02f-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bc02f-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bc02f-180">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="bc02f-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="bc02f-181">Int32</span><span class="sxs-lookup"><span data-stu-id="bc02f-181">Int32</span></span>|<span data-ttu-id="bc02f-182">证书续订阈值百分比。</span><span class="sxs-lookup"><span data-stu-id="bc02f-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="bc02f-183">从[WindowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)继承的有效值1到99</span><span class="sxs-lookup"><span data-stu-id="bc02f-183">Valid values 1 to 99 Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="bc02f-184">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="bc02f-184">keyStorageProvider</span></span>|[<span data-ttu-id="bc02f-185">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="bc02f-185">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="bc02f-186">密钥存储提供程序 (KSP) 继承自 [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="bc02f-186">Key Storage Provider (KSP) Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="bc02f-187">可取值为：`useTpmKspOtherwiseUseSoftwareKsp`、`useTpmKspOtherwiseFail`、`usePassportForWorkKspOtherwiseFail`、`useSoftwareKsp`。</span><span class="sxs-lookup"><span data-stu-id="bc02f-187">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="bc02f-188">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="bc02f-188">subjectNameFormat</span></span>|[<span data-ttu-id="bc02f-189">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="bc02f-189">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="bc02f-190">证书使用者名称格式继承自 [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="bc02f-190">Certificate Subject Name Format Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="bc02f-191">可取值为：`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId`。</span><span class="sxs-lookup"><span data-stu-id="bc02f-191">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="bc02f-192">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="bc02f-192">subjectAlternativeNameType</span></span>|[<span data-ttu-id="bc02f-193">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="bc02f-193">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="bc02f-194">证书使用者备用名称类型继承自 [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="bc02f-194">Certificate Subject Alternative Name Type Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="bc02f-195">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService`。</span><span class="sxs-lookup"><span data-stu-id="bc02f-195">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="bc02f-196">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="bc02f-196">certificateValidityPeriodValue</span></span>|<span data-ttu-id="bc02f-197">Int32</span><span class="sxs-lookup"><span data-stu-id="bc02f-197">Int32</span></span>|<span data-ttu-id="bc02f-198">继承自[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)的证书有效期限的值</span><span class="sxs-lookup"><span data-stu-id="bc02f-198">Value for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="bc02f-199">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="bc02f-199">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="bc02f-200">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="bc02f-200">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="bc02f-201">从 [WindowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)继承的证书有效期限的小数位数。</span><span class="sxs-lookup"><span data-stu-id="bc02f-201">Scale for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="bc02f-202">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="bc02f-202">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="bc02f-203">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="bc02f-203">extendedKeyUsages</span></span>|<span data-ttu-id="bc02f-204">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="bc02f-204">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="bc02f-205"> (EKU) 设置的扩展密钥用法。</span><span class="sxs-lookup"><span data-stu-id="bc02f-205">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="bc02f-206">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="bc02f-206">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="bc02f-207">继承自 [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="bc02f-207">Inherited from [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="bc02f-208">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="bc02f-208">customSubjectAlternativeNames</span></span>|<span data-ttu-id="bc02f-209">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) 集合</span><span class="sxs-lookup"><span data-stu-id="bc02f-209">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="bc02f-210">自定义主题备用名称设置。</span><span class="sxs-lookup"><span data-stu-id="bc02f-210">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="bc02f-211">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="bc02f-211">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="bc02f-212">继承自 [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="bc02f-212">Inherited from [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="bc02f-213">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="bc02f-213">scepServerUrls</span></span>|<span data-ttu-id="bc02f-214">String 集合</span><span class="sxs-lookup"><span data-stu-id="bc02f-214">String collection</span></span>|<span data-ttu-id="bc02f-215">SCEP (s) 的服务器 Url。</span><span class="sxs-lookup"><span data-stu-id="bc02f-215">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="bc02f-216">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="bc02f-216">subjectNameFormatString</span></span>|<span data-ttu-id="bc02f-217">String</span><span class="sxs-lookup"><span data-stu-id="bc02f-217">String</span></span>|<span data-ttu-id="bc02f-218">要与 SubjectNameFormat = Custom 一起使用的自定义格式。</span><span class="sxs-lookup"><span data-stu-id="bc02f-218">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="bc02f-219">示例： CN = {{EmailAddress}}，E = {{EmailAddress}}，OU = 企业用户，O = Contoso Corporation，L = Redmond，ST = WA，C = US</span><span class="sxs-lookup"><span data-stu-id="bc02f-219">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="bc02f-220">keyUsage</span><span class="sxs-lookup"><span data-stu-id="bc02f-220">keyUsage</span></span>|[<span data-ttu-id="bc02f-221">keyUsages</span><span class="sxs-lookup"><span data-stu-id="bc02f-221">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="bc02f-222">SCEP 密钥用法。</span><span class="sxs-lookup"><span data-stu-id="bc02f-222">SCEP Key Usage.</span></span> <span data-ttu-id="bc02f-223">可取值为：`keyEncipherment`、`digitalSignature`。</span><span class="sxs-lookup"><span data-stu-id="bc02f-223">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="bc02f-224">keySize</span><span class="sxs-lookup"><span data-stu-id="bc02f-224">keySize</span></span>|[<span data-ttu-id="bc02f-225">keySize</span><span class="sxs-lookup"><span data-stu-id="bc02f-225">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="bc02f-226">SCEP 密钥大小。</span><span class="sxs-lookup"><span data-stu-id="bc02f-226">SCEP Key Size.</span></span> <span data-ttu-id="bc02f-227">可取值为：`size1024`、`size2048`、`size4096`。</span><span class="sxs-lookup"><span data-stu-id="bc02f-227">Possible values are: `size1024`, `size2048`, `size4096`.</span></span>|
|<span data-ttu-id="bc02f-228">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="bc02f-228">hashAlgorithm</span></span>|[<span data-ttu-id="bc02f-229">hashAlgorithms</span><span class="sxs-lookup"><span data-stu-id="bc02f-229">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="bc02f-230">SCEP 哈希算法。</span><span class="sxs-lookup"><span data-stu-id="bc02f-230">SCEP Hash Algorithm.</span></span> <span data-ttu-id="bc02f-231">可取值为：`sha1`、`sha2`。</span><span class="sxs-lookup"><span data-stu-id="bc02f-231">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="bc02f-232">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="bc02f-232">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="bc02f-233">String</span><span class="sxs-lookup"><span data-stu-id="bc02f-233">String</span></span>|<span data-ttu-id="bc02f-234">定义 AAD 属性的自定义字符串。</span><span class="sxs-lookup"><span data-stu-id="bc02f-234">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="bc02f-235">certificateStore</span><span class="sxs-lookup"><span data-stu-id="bc02f-235">certificateStore</span></span>|[<span data-ttu-id="bc02f-236">certificateStore</span><span class="sxs-lookup"><span data-stu-id="bc02f-236">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="bc02f-237">目标存储证书。</span><span class="sxs-lookup"><span data-stu-id="bc02f-237">Target store certificate.</span></span> <span data-ttu-id="bc02f-238">可取值为：`user`、`machine`。</span><span class="sxs-lookup"><span data-stu-id="bc02f-238">Possible values are: `user`, `machine`.</span></span>|



## <a name="response"></a><span data-ttu-id="bc02f-239">响应</span><span class="sxs-lookup"><span data-stu-id="bc02f-239">Response</span></span>
<span data-ttu-id="bc02f-240">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bc02f-240">If successful, this method returns a `200 OK` response code and an updated [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bc02f-241">示例</span><span class="sxs-lookup"><span data-stu-id="bc02f-241">Example</span></span>

### <a name="request"></a><span data-ttu-id="bc02f-242">请求</span><span class="sxs-lookup"><span data-stu-id="bc02f-242">Request</span></span>
<span data-ttu-id="bc02f-243">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bc02f-243">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="bc02f-244">响应</span><span class="sxs-lookup"><span data-stu-id="bc02f-244">Response</span></span>
<span data-ttu-id="bc02f-p125">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bc02f-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






