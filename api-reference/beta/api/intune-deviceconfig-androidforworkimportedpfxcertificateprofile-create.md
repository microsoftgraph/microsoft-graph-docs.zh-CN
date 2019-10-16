---
title: 创建 androidForWorkImportedPFXCertificateProfile
description: 创建新的 androidForWorkImportedPFXCertificateProfile 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f1617e0db273e108d233b066812da2fd07af5809
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37534594"
---
# <a name="create-androidforworkimportedpfxcertificateprofile"></a><span data-ttu-id="70f69-103">创建 androidForWorkImportedPFXCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="70f69-103">Create androidForWorkImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="70f69-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="70f69-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="70f69-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="70f69-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="70f69-106">创建新的[androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="70f69-106">Create a new [androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="70f69-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="70f69-107">Prerequisites</span></span>
<span data-ttu-id="70f69-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="70f69-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70f69-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="70f69-110">Permission type</span></span>|<span data-ttu-id="70f69-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="70f69-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="70f69-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="70f69-112">Delegated (work or school account)</span></span>|<span data-ttu-id="70f69-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70f69-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="70f69-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="70f69-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="70f69-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="70f69-115">Not supported.</span></span>|
|<span data-ttu-id="70f69-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="70f69-116">Application</span></span>|<span data-ttu-id="70f69-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70f69-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="70f69-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="70f69-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="70f69-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="70f69-119">Request headers</span></span>
|<span data-ttu-id="70f69-120">标头</span><span class="sxs-lookup"><span data-stu-id="70f69-120">Header</span></span>|<span data-ttu-id="70f69-121">值</span><span class="sxs-lookup"><span data-stu-id="70f69-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="70f69-122">授权</span><span class="sxs-lookup"><span data-stu-id="70f69-122">Authorization</span></span>|<span data-ttu-id="70f69-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="70f69-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="70f69-124">接受</span><span class="sxs-lookup"><span data-stu-id="70f69-124">Accept</span></span>|<span data-ttu-id="70f69-125">application/json</span><span class="sxs-lookup"><span data-stu-id="70f69-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="70f69-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="70f69-126">Request body</span></span>
<span data-ttu-id="70f69-127">在请求正文中，提供 androidForWorkImportedPFXCertificateProfile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="70f69-127">In the request body, supply a JSON representation for the androidForWorkImportedPFXCertificateProfile object.</span></span>

<span data-ttu-id="70f69-128">下表显示创建 androidForWorkImportedPFXCertificateProfile 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="70f69-128">The following table shows the properties that are required when you create the androidForWorkImportedPFXCertificateProfile.</span></span>

|<span data-ttu-id="70f69-129">属性</span><span class="sxs-lookup"><span data-stu-id="70f69-129">Property</span></span>|<span data-ttu-id="70f69-130">类型</span><span class="sxs-lookup"><span data-stu-id="70f69-130">Type</span></span>|<span data-ttu-id="70f69-131">说明</span><span class="sxs-lookup"><span data-stu-id="70f69-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70f69-132">id</span><span class="sxs-lookup"><span data-stu-id="70f69-132">id</span></span>|<span data-ttu-id="70f69-133">字符串</span><span class="sxs-lookup"><span data-stu-id="70f69-133">String</span></span>|<span data-ttu-id="70f69-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="70f69-134">Key of the entity.</span></span> <span data-ttu-id="70f69-135">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="70f69-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="70f69-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="70f69-136">lastModifiedDateTime</span></span>|<span data-ttu-id="70f69-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="70f69-137">DateTimeOffset</span></span>|<span data-ttu-id="70f69-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="70f69-138">DateTime the object was last modified.</span></span> <span data-ttu-id="70f69-139">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="70f69-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="70f69-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="70f69-140">roleScopeTagIds</span></span>|<span data-ttu-id="70f69-141">String 集合</span><span class="sxs-lookup"><span data-stu-id="70f69-141">String collection</span></span>|<span data-ttu-id="70f69-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="70f69-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="70f69-143">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="70f69-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="70f69-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="70f69-144">supportsScopeTags</span></span>|<span data-ttu-id="70f69-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="70f69-145">Boolean</span></span>|<span data-ttu-id="70f69-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="70f69-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="70f69-147">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="70f69-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="70f69-148">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="70f69-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="70f69-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="70f69-149">This property is read-only.</span></span> <span data-ttu-id="70f69-150">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="70f69-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="70f69-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="70f69-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="70f69-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="70f69-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="70f69-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="70f69-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="70f69-154">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="70f69-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="70f69-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="70f69-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="70f69-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="70f69-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="70f69-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="70f69-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="70f69-158">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="70f69-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="70f69-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="70f69-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="70f69-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="70f69-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="70f69-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="70f69-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="70f69-162">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="70f69-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="70f69-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="70f69-163">createdDateTime</span></span>|<span data-ttu-id="70f69-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="70f69-164">DateTimeOffset</span></span>|<span data-ttu-id="70f69-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="70f69-165">DateTime the object was created.</span></span> <span data-ttu-id="70f69-166">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="70f69-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="70f69-167">说明</span><span class="sxs-lookup"><span data-stu-id="70f69-167">description</span></span>|<span data-ttu-id="70f69-168">String</span><span class="sxs-lookup"><span data-stu-id="70f69-168">String</span></span>|<span data-ttu-id="70f69-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="70f69-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="70f69-170">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="70f69-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="70f69-171">displayName</span><span class="sxs-lookup"><span data-stu-id="70f69-171">displayName</span></span>|<span data-ttu-id="70f69-172">String</span><span class="sxs-lookup"><span data-stu-id="70f69-172">String</span></span>|<span data-ttu-id="70f69-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="70f69-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="70f69-174">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="70f69-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="70f69-175">version</span><span class="sxs-lookup"><span data-stu-id="70f69-175">version</span></span>|<span data-ttu-id="70f69-176">Int32</span><span class="sxs-lookup"><span data-stu-id="70f69-176">Int32</span></span>|<span data-ttu-id="70f69-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="70f69-177">Version of the device configuration.</span></span> <span data-ttu-id="70f69-178">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="70f69-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="70f69-179">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="70f69-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="70f69-180">Int32</span><span class="sxs-lookup"><span data-stu-id="70f69-180">Int32</span></span>|<span data-ttu-id="70f69-181">证书续订阈值百分比。</span><span class="sxs-lookup"><span data-stu-id="70f69-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="70f69-182">从[AndroidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)继承的有效值1到99</span><span class="sxs-lookup"><span data-stu-id="70f69-182">Valid values 1 to 99 Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="70f69-183">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="70f69-183">subjectNameFormat</span></span>|[<span data-ttu-id="70f69-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="70f69-184">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="70f69-185">证书使用者名称格式。</span><span class="sxs-lookup"><span data-stu-id="70f69-185">Certificate Subject Name Format.</span></span> <span data-ttu-id="70f69-186">继承自[androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="70f69-186">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="70f69-187">可取值为：`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId`。</span><span class="sxs-lookup"><span data-stu-id="70f69-187">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="70f69-188">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="70f69-188">subjectAlternativeNameType</span></span>|[<span data-ttu-id="70f69-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="70f69-189">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="70f69-190">证书使用者备用名称类型。</span><span class="sxs-lookup"><span data-stu-id="70f69-190">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="70f69-191">继承自[androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="70f69-191">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="70f69-192">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService`。</span><span class="sxs-lookup"><span data-stu-id="70f69-192">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="70f69-193">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="70f69-193">certificateValidityPeriodValue</span></span>|<span data-ttu-id="70f69-194">Int32</span><span class="sxs-lookup"><span data-stu-id="70f69-194">Int32</span></span>|<span data-ttu-id="70f69-195">证书有效期限的值。</span><span class="sxs-lookup"><span data-stu-id="70f69-195">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="70f69-196">继承自[androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="70f69-196">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="70f69-197">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="70f69-197">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="70f69-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="70f69-198">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="70f69-199">证书有效期的小数位数。</span><span class="sxs-lookup"><span data-stu-id="70f69-199">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="70f69-200">继承自[androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="70f69-200">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="70f69-201">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="70f69-201">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="70f69-202">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="70f69-202">extendedKeyUsages</span></span>|<span data-ttu-id="70f69-203">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)集合</span><span class="sxs-lookup"><span data-stu-id="70f69-203">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="70f69-204">扩展密钥用法（EKU）设置。</span><span class="sxs-lookup"><span data-stu-id="70f69-204">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="70f69-205">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="70f69-205">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="70f69-206">继承自[androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="70f69-206">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="70f69-207">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="70f69-207">intendedPurpose</span></span>|[<span data-ttu-id="70f69-208">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="70f69-208">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="70f69-209">尚未记录。</span><span class="sxs-lookup"><span data-stu-id="70f69-209">Not yet documented.</span></span> <span data-ttu-id="70f69-210">可取值为：`unassigned`、`smimeEncryption`、`smimeSigning`、`vpn`、`wifi`。</span><span class="sxs-lookup"><span data-stu-id="70f69-210">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="70f69-211">响应</span><span class="sxs-lookup"><span data-stu-id="70f69-211">Response</span></span>
<span data-ttu-id="70f69-212">如果成功，此方法在响应`201 Created`正文中返回响应代码和[androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="70f69-212">If successful, this method returns a `201 Created` response code and a [androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="70f69-213">示例</span><span class="sxs-lookup"><span data-stu-id="70f69-213">Example</span></span>

### <a name="request"></a><span data-ttu-id="70f69-214">请求</span><span class="sxs-lookup"><span data-stu-id="70f69-214">Request</span></span>
<span data-ttu-id="70f69-215">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="70f69-215">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1499

{
  "@odata.type": "#microsoft.graph.androidForWorkImportedPFXCertificateProfile",
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
  "intendedPurpose": "smimeEncryption"
}
```

### <a name="response"></a><span data-ttu-id="70f69-216">响应</span><span class="sxs-lookup"><span data-stu-id="70f69-216">Response</span></span>
<span data-ttu-id="70f69-p120">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="70f69-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1671

{
  "@odata.type": "#microsoft.graph.androidForWorkImportedPFXCertificateProfile",
  "id": "a0bfd7bc-d7bc-a0bf-bcd7-bfa0bcd7bfa0",
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
  "intendedPurpose": "smimeEncryption"
}
```






