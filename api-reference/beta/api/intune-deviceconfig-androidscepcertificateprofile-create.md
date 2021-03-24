---
title: 创建 androidScepCertificateProfile
description: 创建新的 androidScepCertificateProfile 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 659467321509abe7662ba6c61a7f89f2ae9fa00e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51137817"
---
# <a name="create-androidscepcertificateprofile"></a><span data-ttu-id="36843-103">创建 androidScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="36843-103">Create androidScepCertificateProfile</span></span>

<span data-ttu-id="36843-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="36843-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="36843-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="36843-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="36843-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="36843-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="36843-107">创建新的 [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="36843-107">Create a new [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="36843-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="36843-108">Prerequisites</span></span>
<span data-ttu-id="36843-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="36843-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36843-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="36843-111">Permission type</span></span>|<span data-ttu-id="36843-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="36843-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="36843-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="36843-113">Delegated (work or school account)</span></span>|<span data-ttu-id="36843-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36843-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="36843-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="36843-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="36843-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="36843-116">Not supported.</span></span>|
|<span data-ttu-id="36843-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="36843-117">Application</span></span>|<span data-ttu-id="36843-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36843-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="36843-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="36843-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="36843-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="36843-120">Request headers</span></span>
|<span data-ttu-id="36843-121">标头</span><span class="sxs-lookup"><span data-stu-id="36843-121">Header</span></span>|<span data-ttu-id="36843-122">值</span><span class="sxs-lookup"><span data-stu-id="36843-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="36843-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="36843-123">Authorization</span></span>|<span data-ttu-id="36843-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="36843-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="36843-125">接受</span><span class="sxs-lookup"><span data-stu-id="36843-125">Accept</span></span>|<span data-ttu-id="36843-126">application/json</span><span class="sxs-lookup"><span data-stu-id="36843-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="36843-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="36843-127">Request body</span></span>
<span data-ttu-id="36843-128">在请求正文中，提供 androidScepCertificateProfile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="36843-128">In the request body, supply a JSON representation for the androidScepCertificateProfile object.</span></span>

<span data-ttu-id="36843-129">下表显示创建 androidScepCertificateProfile 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="36843-129">The following table shows the properties that are required when you create the androidScepCertificateProfile.</span></span>

|<span data-ttu-id="36843-130">属性</span><span class="sxs-lookup"><span data-stu-id="36843-130">Property</span></span>|<span data-ttu-id="36843-131">类型</span><span class="sxs-lookup"><span data-stu-id="36843-131">Type</span></span>|<span data-ttu-id="36843-132">说明</span><span class="sxs-lookup"><span data-stu-id="36843-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="36843-133">id</span><span class="sxs-lookup"><span data-stu-id="36843-133">id</span></span>|<span data-ttu-id="36843-134">String</span><span class="sxs-lookup"><span data-stu-id="36843-134">String</span></span>|<span data-ttu-id="36843-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="36843-135">Key of the entity.</span></span> <span data-ttu-id="36843-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="36843-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36843-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="36843-137">lastModifiedDateTime</span></span>|<span data-ttu-id="36843-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="36843-138">DateTimeOffset</span></span>|<span data-ttu-id="36843-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="36843-139">DateTime the object was last modified.</span></span> <span data-ttu-id="36843-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="36843-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36843-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="36843-141">roleScopeTagIds</span></span>|<span data-ttu-id="36843-142">String collection</span><span class="sxs-lookup"><span data-stu-id="36843-142">String collection</span></span>|<span data-ttu-id="36843-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="36843-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="36843-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="36843-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36843-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="36843-145">supportsScopeTags</span></span>|<span data-ttu-id="36843-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="36843-146">Boolean</span></span>|<span data-ttu-id="36843-147">指示基础设备配置是否支持分配范围标记。</span><span class="sxs-lookup"><span data-stu-id="36843-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="36843-148">当此值为 false 且实体对作用域用户不可见时，不允许分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="36843-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="36843-149">这适用于在 Silverlight 中创建的旧版策略，可通过在 Azure 门户中删除和重新创建策略来解决。</span><span class="sxs-lookup"><span data-stu-id="36843-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="36843-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="36843-150">This property is read-only.</span></span> <span data-ttu-id="36843-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="36843-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36843-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="36843-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="36843-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="36843-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="36843-154">此策略的操作系统版本适用性。</span><span class="sxs-lookup"><span data-stu-id="36843-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="36843-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="36843-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36843-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="36843-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="36843-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="36843-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="36843-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="36843-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="36843-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="36843-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36843-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="36843-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="36843-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="36843-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="36843-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="36843-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="36843-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="36843-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36843-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="36843-164">createdDateTime</span></span>|<span data-ttu-id="36843-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="36843-165">DateTimeOffset</span></span>|<span data-ttu-id="36843-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="36843-166">DateTime the object was created.</span></span> <span data-ttu-id="36843-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="36843-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36843-168">说明</span><span class="sxs-lookup"><span data-stu-id="36843-168">description</span></span>|<span data-ttu-id="36843-169">String</span><span class="sxs-lookup"><span data-stu-id="36843-169">String</span></span>|<span data-ttu-id="36843-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="36843-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="36843-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="36843-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36843-172">displayName</span><span class="sxs-lookup"><span data-stu-id="36843-172">displayName</span></span>|<span data-ttu-id="36843-173">String</span><span class="sxs-lookup"><span data-stu-id="36843-173">String</span></span>|<span data-ttu-id="36843-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="36843-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="36843-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="36843-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36843-176">version</span><span class="sxs-lookup"><span data-stu-id="36843-176">version</span></span>|<span data-ttu-id="36843-177">Int32</span><span class="sxs-lookup"><span data-stu-id="36843-177">Int32</span></span>|<span data-ttu-id="36843-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="36843-178">Version of the device configuration.</span></span> <span data-ttu-id="36843-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="36843-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36843-180">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="36843-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="36843-181">Int32</span><span class="sxs-lookup"><span data-stu-id="36843-181">Int32</span></span>|<span data-ttu-id="36843-182">证书续订阈值百分比。</span><span class="sxs-lookup"><span data-stu-id="36843-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="36843-183">有效值 1 到 99 继承自 [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="36843-183">Valid values 1 to 99 Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="36843-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="36843-184">subjectNameFormat</span></span>|[<span data-ttu-id="36843-185">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="36843-185">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="36843-186">证书主题名称格式。</span><span class="sxs-lookup"><span data-stu-id="36843-186">Certificate Subject Name Format.</span></span> <span data-ttu-id="36843-187">继承自 [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="36843-187">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="36843-188">可取值为：`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId`。</span><span class="sxs-lookup"><span data-stu-id="36843-188">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="36843-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="36843-189">subjectAlternativeNameType</span></span>|[<span data-ttu-id="36843-190">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="36843-190">subjectAlternativeNameType</span></span>](../resources/intune-shared-subjectalternativenametype.md)|<span data-ttu-id="36843-191">证书主题备用名称类型。</span><span class="sxs-lookup"><span data-stu-id="36843-191">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="36843-192">继承自 [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="36843-192">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="36843-193">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService`、`universalResourceIdentifier`。</span><span class="sxs-lookup"><span data-stu-id="36843-193">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span></span>|
|<span data-ttu-id="36843-194">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="36843-194">certificateValidityPeriodValue</span></span>|<span data-ttu-id="36843-195">Int32</span><span class="sxs-lookup"><span data-stu-id="36843-195">Int32</span></span>|<span data-ttu-id="36843-196">证书有效期的值。</span><span class="sxs-lookup"><span data-stu-id="36843-196">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="36843-197">继承自 [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="36843-197">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="36843-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="36843-198">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="36843-199">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="36843-199">certificateValidityPeriodScale</span></span>](../resources/intune-shared-certificatevalidityperiodscale.md)|<span data-ttu-id="36843-200">证书有效期的缩放。</span><span class="sxs-lookup"><span data-stu-id="36843-200">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="36843-201">继承自 [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="36843-201">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="36843-202">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="36843-202">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="36843-203">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="36843-203">extendedKeyUsages</span></span>|<span data-ttu-id="36843-204">[extendedKeyUsage](../resources/intune-shared-extendedkeyusage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="36843-204">[extendedKeyUsage](../resources/intune-shared-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="36843-205">EKU (扩展密钥) 设置。</span><span class="sxs-lookup"><span data-stu-id="36843-205">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="36843-206">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="36843-206">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="36843-207">继承自 [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="36843-207">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="36843-208">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="36843-208">scepServerUrls</span></span>|<span data-ttu-id="36843-209">String collection</span><span class="sxs-lookup"><span data-stu-id="36843-209">String collection</span></span>|<span data-ttu-id="36843-210">SCEP 服务器 URL () </span><span class="sxs-lookup"><span data-stu-id="36843-210">SCEP Server Url(s)</span></span>|
|<span data-ttu-id="36843-211">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="36843-211">subjectNameFormatString</span></span>|<span data-ttu-id="36843-212">String</span><span class="sxs-lookup"><span data-stu-id="36843-212">String</span></span>|<span data-ttu-id="36843-213">要与 SubjectNameFormat 一同使用的自定义格式 = Custom。</span><span class="sxs-lookup"><span data-stu-id="36843-213">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="36843-214">示例：CN={{EmailAddress}}，E={{EmailAddress}，OU=Enterprise Users，O=Contoso Corporation，L=Redmond，ST=WA，C=US</span><span class="sxs-lookup"><span data-stu-id="36843-214">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="36843-215">keyUsage</span><span class="sxs-lookup"><span data-stu-id="36843-215">keyUsage</span></span>|[<span data-ttu-id="36843-216">keyUsages</span><span class="sxs-lookup"><span data-stu-id="36843-216">keyUsages</span></span>](../resources/intune-shared-keyusages.md)|<span data-ttu-id="36843-217">SCEP 密钥用法。</span><span class="sxs-lookup"><span data-stu-id="36843-217">SCEP Key Usage.</span></span> <span data-ttu-id="36843-218">可取值为：`keyEncipherment`、`digitalSignature`。</span><span class="sxs-lookup"><span data-stu-id="36843-218">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="36843-219">keySize</span><span class="sxs-lookup"><span data-stu-id="36843-219">keySize</span></span>|[<span data-ttu-id="36843-220">keySize</span><span class="sxs-lookup"><span data-stu-id="36843-220">keySize</span></span>](../resources/intune-shared-keysize.md)|<span data-ttu-id="36843-221">SCEP 密钥大小。</span><span class="sxs-lookup"><span data-stu-id="36843-221">SCEP Key Size.</span></span> <span data-ttu-id="36843-222">可取值为：`size1024`、`size2048`、`size4096`。</span><span class="sxs-lookup"><span data-stu-id="36843-222">Possible values are: `size1024`, `size2048`, `size4096`.</span></span>|
|<span data-ttu-id="36843-223">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="36843-223">hashAlgorithm</span></span>|[<span data-ttu-id="36843-224">hashAlgorithms</span><span class="sxs-lookup"><span data-stu-id="36843-224">hashAlgorithms</span></span>](../resources/intune-shared-hashalgorithms.md)|<span data-ttu-id="36843-225">SCEP 哈希算法。</span><span class="sxs-lookup"><span data-stu-id="36843-225">SCEP Hash Algorithm.</span></span> <span data-ttu-id="36843-226">可取值为：`sha1`、`sha2`。</span><span class="sxs-lookup"><span data-stu-id="36843-226">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="36843-227">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="36843-227">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="36843-228">String</span><span class="sxs-lookup"><span data-stu-id="36843-228">String</span></span>|<span data-ttu-id="36843-229">定义 AAD 属性的自定义字符串。</span><span class="sxs-lookup"><span data-stu-id="36843-229">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="36843-230">响应</span><span class="sxs-lookup"><span data-stu-id="36843-230">Response</span></span>
<span data-ttu-id="36843-231">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="36843-231">If successful, this method returns a `201 Created` response code and a [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36843-232">示例</span><span class="sxs-lookup"><span data-stu-id="36843-232">Example</span></span>

### <a name="request"></a><span data-ttu-id="36843-233">请求</span><span class="sxs-lookup"><span data-stu-id="36843-233">Request</span></span>
<span data-ttu-id="36843-234">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="36843-234">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1747

{
  "@odata.type": "#microsoft.graph.androidScepCertificateProfile",
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

### <a name="response"></a><span data-ttu-id="36843-235">响应</span><span class="sxs-lookup"><span data-stu-id="36843-235">Response</span></span>
<span data-ttu-id="36843-p123">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="36843-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1919

{
  "@odata.type": "#microsoft.graph.androidScepCertificateProfile",
  "id": "e9a0dbbd-dbbd-e9a0-bddb-a0e9bddba0e9",
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




