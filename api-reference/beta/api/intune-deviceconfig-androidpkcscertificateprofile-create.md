---
title: 创建 androidPkcsCertificateProfile
description: 创建新的 androidPkcsCertificateProfile 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2f4b6d34520bcfd80895c880afdb5db3c923ea16
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51137866"
---
# <a name="create-androidpkcscertificateprofile"></a><span data-ttu-id="f243c-103">创建 androidPkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="f243c-103">Create androidPkcsCertificateProfile</span></span>

<span data-ttu-id="f243c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f243c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f243c-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f243c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f243c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f243c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f243c-107">创建新的 [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f243c-107">Create a new [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f243c-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="f243c-108">Prerequisites</span></span>
<span data-ttu-id="f243c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f243c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f243c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f243c-111">Permission type</span></span>|<span data-ttu-id="f243c-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f243c-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f243c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f243c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f243c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f243c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f243c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f243c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f243c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f243c-116">Not supported.</span></span>|
|<span data-ttu-id="f243c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f243c-117">Application</span></span>|<span data-ttu-id="f243c-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f243c-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f243c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f243c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f243c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f243c-120">Request headers</span></span>
|<span data-ttu-id="f243c-121">标头</span><span class="sxs-lookup"><span data-stu-id="f243c-121">Header</span></span>|<span data-ttu-id="f243c-122">值</span><span class="sxs-lookup"><span data-stu-id="f243c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f243c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f243c-123">Authorization</span></span>|<span data-ttu-id="f243c-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f243c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f243c-125">接受</span><span class="sxs-lookup"><span data-stu-id="f243c-125">Accept</span></span>|<span data-ttu-id="f243c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f243c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f243c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f243c-127">Request body</span></span>
<span data-ttu-id="f243c-128">在请求正文中，提供 androidPkcsCertificateProfile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f243c-128">In the request body, supply a JSON representation for the androidPkcsCertificateProfile object.</span></span>

<span data-ttu-id="f243c-129">下表显示创建 androidPkcsCertificateProfile 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f243c-129">The following table shows the properties that are required when you create the androidPkcsCertificateProfile.</span></span>

|<span data-ttu-id="f243c-130">属性</span><span class="sxs-lookup"><span data-stu-id="f243c-130">Property</span></span>|<span data-ttu-id="f243c-131">类型</span><span class="sxs-lookup"><span data-stu-id="f243c-131">Type</span></span>|<span data-ttu-id="f243c-132">说明</span><span class="sxs-lookup"><span data-stu-id="f243c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f243c-133">id</span><span class="sxs-lookup"><span data-stu-id="f243c-133">id</span></span>|<span data-ttu-id="f243c-134">String</span><span class="sxs-lookup"><span data-stu-id="f243c-134">String</span></span>|<span data-ttu-id="f243c-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f243c-135">Key of the entity.</span></span> <span data-ttu-id="f243c-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f243c-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f243c-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f243c-137">lastModifiedDateTime</span></span>|<span data-ttu-id="f243c-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f243c-138">DateTimeOffset</span></span>|<span data-ttu-id="f243c-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f243c-139">DateTime the object was last modified.</span></span> <span data-ttu-id="f243c-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f243c-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f243c-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f243c-141">roleScopeTagIds</span></span>|<span data-ttu-id="f243c-142">String collection</span><span class="sxs-lookup"><span data-stu-id="f243c-142">String collection</span></span>|<span data-ttu-id="f243c-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="f243c-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f243c-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f243c-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f243c-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f243c-145">supportsScopeTags</span></span>|<span data-ttu-id="f243c-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="f243c-146">Boolean</span></span>|<span data-ttu-id="f243c-147">指示基础设备配置是否支持分配范围标记。</span><span class="sxs-lookup"><span data-stu-id="f243c-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f243c-148">当此值为 false 且实体对作用域用户不可见时，不允许分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="f243c-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f243c-149">这适用于在 Silverlight 中创建的旧版策略，可通过在 Azure 门户中删除和重新创建策略来解决。</span><span class="sxs-lookup"><span data-stu-id="f243c-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f243c-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="f243c-150">This property is read-only.</span></span> <span data-ttu-id="f243c-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f243c-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f243c-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f243c-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="f243c-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f243c-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="f243c-154">此策略的操作系统版本适用性。</span><span class="sxs-lookup"><span data-stu-id="f243c-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="f243c-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f243c-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f243c-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f243c-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="f243c-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f243c-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="f243c-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="f243c-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="f243c-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f243c-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f243c-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f243c-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="f243c-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f243c-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="f243c-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="f243c-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="f243c-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f243c-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f243c-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f243c-164">createdDateTime</span></span>|<span data-ttu-id="f243c-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f243c-165">DateTimeOffset</span></span>|<span data-ttu-id="f243c-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f243c-166">DateTime the object was created.</span></span> <span data-ttu-id="f243c-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f243c-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f243c-168">说明</span><span class="sxs-lookup"><span data-stu-id="f243c-168">description</span></span>|<span data-ttu-id="f243c-169">String</span><span class="sxs-lookup"><span data-stu-id="f243c-169">String</span></span>|<span data-ttu-id="f243c-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="f243c-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f243c-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f243c-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f243c-172">displayName</span><span class="sxs-lookup"><span data-stu-id="f243c-172">displayName</span></span>|<span data-ttu-id="f243c-173">String</span><span class="sxs-lookup"><span data-stu-id="f243c-173">String</span></span>|<span data-ttu-id="f243c-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="f243c-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f243c-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f243c-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f243c-176">version</span><span class="sxs-lookup"><span data-stu-id="f243c-176">version</span></span>|<span data-ttu-id="f243c-177">Int32</span><span class="sxs-lookup"><span data-stu-id="f243c-177">Int32</span></span>|<span data-ttu-id="f243c-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="f243c-178">Version of the device configuration.</span></span> <span data-ttu-id="f243c-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f243c-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f243c-180">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="f243c-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="f243c-181">Int32</span><span class="sxs-lookup"><span data-stu-id="f243c-181">Int32</span></span>|<span data-ttu-id="f243c-182">证书续订阈值百分比。</span><span class="sxs-lookup"><span data-stu-id="f243c-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="f243c-183">有效值 1 到 99 继承自 [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="f243c-183">Valid values 1 to 99 Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="f243c-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="f243c-184">subjectNameFormat</span></span>|[<span data-ttu-id="f243c-185">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="f243c-185">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="f243c-186">证书主题名称格式。</span><span class="sxs-lookup"><span data-stu-id="f243c-186">Certificate Subject Name Format.</span></span> <span data-ttu-id="f243c-187">继承自 [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="f243c-187">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="f243c-188">可取值为：`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId`。</span><span class="sxs-lookup"><span data-stu-id="f243c-188">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="f243c-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="f243c-189">subjectAlternativeNameType</span></span>|[<span data-ttu-id="f243c-190">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="f243c-190">subjectAlternativeNameType</span></span>](../resources/intune-shared-subjectalternativenametype.md)|<span data-ttu-id="f243c-191">证书主题备用名称类型。</span><span class="sxs-lookup"><span data-stu-id="f243c-191">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="f243c-192">继承自 [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="f243c-192">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="f243c-193">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService`、`universalResourceIdentifier`。</span><span class="sxs-lookup"><span data-stu-id="f243c-193">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span></span>|
|<span data-ttu-id="f243c-194">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="f243c-194">certificateValidityPeriodValue</span></span>|<span data-ttu-id="f243c-195">Int32</span><span class="sxs-lookup"><span data-stu-id="f243c-195">Int32</span></span>|<span data-ttu-id="f243c-196">证书有效期的值。</span><span class="sxs-lookup"><span data-stu-id="f243c-196">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="f243c-197">继承自 [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="f243c-197">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="f243c-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="f243c-198">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="f243c-199">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="f243c-199">certificateValidityPeriodScale</span></span>](../resources/intune-shared-certificatevalidityperiodscale.md)|<span data-ttu-id="f243c-200">证书有效期的缩放。</span><span class="sxs-lookup"><span data-stu-id="f243c-200">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="f243c-201">继承自 [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="f243c-201">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="f243c-202">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="f243c-202">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="f243c-203">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="f243c-203">extendedKeyUsages</span></span>|<span data-ttu-id="f243c-204">[extendedKeyUsage](../resources/intune-shared-extendedkeyusage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f243c-204">[extendedKeyUsage](../resources/intune-shared-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="f243c-205">EKU (扩展密钥) 设置。</span><span class="sxs-lookup"><span data-stu-id="f243c-205">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="f243c-206">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="f243c-206">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="f243c-207">继承自 [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="f243c-207">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="f243c-208">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="f243c-208">certificationAuthority</span></span>|<span data-ttu-id="f243c-209">String</span><span class="sxs-lookup"><span data-stu-id="f243c-209">String</span></span>|<span data-ttu-id="f243c-210">PKCS 证书颁发机构</span><span class="sxs-lookup"><span data-stu-id="f243c-210">PKCS Certification Authority</span></span>|
|<span data-ttu-id="f243c-211">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="f243c-211">certificationAuthorityName</span></span>|<span data-ttu-id="f243c-212">String</span><span class="sxs-lookup"><span data-stu-id="f243c-212">String</span></span>|<span data-ttu-id="f243c-213">PKCS 证书颁发机构名称</span><span class="sxs-lookup"><span data-stu-id="f243c-213">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="f243c-214">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="f243c-214">certificateTemplateName</span></span>|<span data-ttu-id="f243c-215">String</span><span class="sxs-lookup"><span data-stu-id="f243c-215">String</span></span>|<span data-ttu-id="f243c-216">PKCS 证书模板名称</span><span class="sxs-lookup"><span data-stu-id="f243c-216">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="f243c-217">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="f243c-217">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="f243c-218">String</span><span class="sxs-lookup"><span data-stu-id="f243c-218">String</span></span>|<span data-ttu-id="f243c-219">定义 AAD 属性的自定义字符串。</span><span class="sxs-lookup"><span data-stu-id="f243c-219">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="f243c-220">响应</span><span class="sxs-lookup"><span data-stu-id="f243c-220">Response</span></span>
<span data-ttu-id="f243c-221">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f243c-221">If successful, this method returns a `201 Created` response code and a [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f243c-222">示例</span><span class="sxs-lookup"><span data-stu-id="f243c-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="f243c-223">请求</span><span class="sxs-lookup"><span data-stu-id="f243c-223">Request</span></span>
<span data-ttu-id="f243c-224">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f243c-224">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1731

{
  "@odata.type": "#microsoft.graph.androidPkcsCertificateProfile",
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
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```

### <a name="response"></a><span data-ttu-id="f243c-225">响应</span><span class="sxs-lookup"><span data-stu-id="f243c-225">Response</span></span>
<span data-ttu-id="f243c-p119">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f243c-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1903

{
  "@odata.type": "#microsoft.graph.androidPkcsCertificateProfile",
  "id": "bb55705b-705b-bb55-5b70-55bb5b7055bb",
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
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```




