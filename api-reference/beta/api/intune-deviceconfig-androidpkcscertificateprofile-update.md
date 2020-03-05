---
title: 更新 androidPkcsCertificateProfile
description: 更新 androidPkcsCertificateProfile 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 86eb081001a56fe97ee226131d5993cc3e046e97
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42449654"
---
# <a name="update-androidpkcscertificateprofile"></a><span data-ttu-id="64acc-103">更新 androidPkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="64acc-103">Update androidPkcsCertificateProfile</span></span>

<span data-ttu-id="64acc-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="64acc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="64acc-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="64acc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="64acc-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="64acc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64acc-107">更新[androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="64acc-107">Update the properties of a [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="64acc-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="64acc-108">Prerequisites</span></span>
<span data-ttu-id="64acc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="64acc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64acc-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="64acc-111">Permission type</span></span>|<span data-ttu-id="64acc-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="64acc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="64acc-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="64acc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="64acc-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64acc-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="64acc-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="64acc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="64acc-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="64acc-116">Not supported.</span></span>|
|<span data-ttu-id="64acc-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="64acc-117">Application</span></span>|<span data-ttu-id="64acc-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64acc-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="64acc-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="64acc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="64acc-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="64acc-120">Request headers</span></span>
|<span data-ttu-id="64acc-121">标头</span><span class="sxs-lookup"><span data-stu-id="64acc-121">Header</span></span>|<span data-ttu-id="64acc-122">值</span><span class="sxs-lookup"><span data-stu-id="64acc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="64acc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="64acc-123">Authorization</span></span>|<span data-ttu-id="64acc-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="64acc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="64acc-125">接受</span><span class="sxs-lookup"><span data-stu-id="64acc-125">Accept</span></span>|<span data-ttu-id="64acc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="64acc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="64acc-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="64acc-127">Request body</span></span>
<span data-ttu-id="64acc-128">在请求正文中，提供[androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="64acc-128">In the request body, supply a JSON representation for the [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) object.</span></span>

<span data-ttu-id="64acc-129">下表显示创建[androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="64acc-129">The following table shows the properties that are required when you create the [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md).</span></span>

|<span data-ttu-id="64acc-130">属性</span><span class="sxs-lookup"><span data-stu-id="64acc-130">Property</span></span>|<span data-ttu-id="64acc-131">类型</span><span class="sxs-lookup"><span data-stu-id="64acc-131">Type</span></span>|<span data-ttu-id="64acc-132">说明</span><span class="sxs-lookup"><span data-stu-id="64acc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64acc-133">id</span><span class="sxs-lookup"><span data-stu-id="64acc-133">id</span></span>|<span data-ttu-id="64acc-134">字符串</span><span class="sxs-lookup"><span data-stu-id="64acc-134">String</span></span>|<span data-ttu-id="64acc-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="64acc-135">Key of the entity.</span></span> <span data-ttu-id="64acc-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64acc-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64acc-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="64acc-137">lastModifiedDateTime</span></span>|<span data-ttu-id="64acc-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64acc-138">DateTimeOffset</span></span>|<span data-ttu-id="64acc-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="64acc-139">DateTime the object was last modified.</span></span> <span data-ttu-id="64acc-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64acc-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64acc-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="64acc-141">roleScopeTagIds</span></span>|<span data-ttu-id="64acc-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="64acc-142">String collection</span></span>|<span data-ttu-id="64acc-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="64acc-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="64acc-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64acc-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64acc-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="64acc-145">supportsScopeTags</span></span>|<span data-ttu-id="64acc-146">布尔</span><span class="sxs-lookup"><span data-stu-id="64acc-146">Boolean</span></span>|<span data-ttu-id="64acc-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="64acc-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="64acc-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="64acc-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="64acc-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="64acc-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="64acc-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="64acc-150">This property is read-only.</span></span> <span data-ttu-id="64acc-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64acc-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64acc-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="64acc-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="64acc-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="64acc-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="64acc-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="64acc-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="64acc-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64acc-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64acc-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="64acc-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="64acc-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="64acc-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="64acc-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="64acc-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="64acc-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64acc-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64acc-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="64acc-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="64acc-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="64acc-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="64acc-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="64acc-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="64acc-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64acc-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64acc-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="64acc-164">createdDateTime</span></span>|<span data-ttu-id="64acc-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64acc-165">DateTimeOffset</span></span>|<span data-ttu-id="64acc-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="64acc-166">DateTime the object was created.</span></span> <span data-ttu-id="64acc-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64acc-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64acc-168">说明</span><span class="sxs-lookup"><span data-stu-id="64acc-168">description</span></span>|<span data-ttu-id="64acc-169">String</span><span class="sxs-lookup"><span data-stu-id="64acc-169">String</span></span>|<span data-ttu-id="64acc-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="64acc-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="64acc-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64acc-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64acc-172">displayName</span><span class="sxs-lookup"><span data-stu-id="64acc-172">displayName</span></span>|<span data-ttu-id="64acc-173">String</span><span class="sxs-lookup"><span data-stu-id="64acc-173">String</span></span>|<span data-ttu-id="64acc-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="64acc-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="64acc-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64acc-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64acc-176">version</span><span class="sxs-lookup"><span data-stu-id="64acc-176">version</span></span>|<span data-ttu-id="64acc-177">Int32</span><span class="sxs-lookup"><span data-stu-id="64acc-177">Int32</span></span>|<span data-ttu-id="64acc-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="64acc-178">Version of the device configuration.</span></span> <span data-ttu-id="64acc-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64acc-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64acc-180">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="64acc-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="64acc-181">Int32</span><span class="sxs-lookup"><span data-stu-id="64acc-181">Int32</span></span>|<span data-ttu-id="64acc-182">证书续订阈值百分比。</span><span class="sxs-lookup"><span data-stu-id="64acc-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="64acc-183">从[AndroidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)继承的有效值1到99</span><span class="sxs-lookup"><span data-stu-id="64acc-183">Valid values 1 to 99 Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="64acc-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="64acc-184">subjectNameFormat</span></span>|[<span data-ttu-id="64acc-185">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="64acc-185">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="64acc-186">证书使用者名称格式。</span><span class="sxs-lookup"><span data-stu-id="64acc-186">Certificate Subject Name Format.</span></span> <span data-ttu-id="64acc-187">继承自[androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="64acc-187">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="64acc-188">可取值为：`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId`。</span><span class="sxs-lookup"><span data-stu-id="64acc-188">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="64acc-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="64acc-189">subjectAlternativeNameType</span></span>|[<span data-ttu-id="64acc-190">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="64acc-190">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="64acc-191">证书使用者备用名称类型。</span><span class="sxs-lookup"><span data-stu-id="64acc-191">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="64acc-192">继承自[androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="64acc-192">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="64acc-193">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService`。</span><span class="sxs-lookup"><span data-stu-id="64acc-193">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="64acc-194">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="64acc-194">certificateValidityPeriodValue</span></span>|<span data-ttu-id="64acc-195">Int32</span><span class="sxs-lookup"><span data-stu-id="64acc-195">Int32</span></span>|<span data-ttu-id="64acc-196">证书有效期限的值。</span><span class="sxs-lookup"><span data-stu-id="64acc-196">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="64acc-197">继承自[androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="64acc-197">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="64acc-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="64acc-198">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="64acc-199">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="64acc-199">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="64acc-200">证书有效期的小数位数。</span><span class="sxs-lookup"><span data-stu-id="64acc-200">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="64acc-201">继承自[androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="64acc-201">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="64acc-202">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="64acc-202">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="64acc-203">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="64acc-203">extendedKeyUsages</span></span>|<span data-ttu-id="64acc-204">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)集合</span><span class="sxs-lookup"><span data-stu-id="64acc-204">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="64acc-205">扩展密钥用法（EKU）设置。</span><span class="sxs-lookup"><span data-stu-id="64acc-205">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="64acc-206">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="64acc-206">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="64acc-207">继承自[androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="64acc-207">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="64acc-208">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="64acc-208">certificationAuthority</span></span>|<span data-ttu-id="64acc-209">String</span><span class="sxs-lookup"><span data-stu-id="64acc-209">String</span></span>|<span data-ttu-id="64acc-210">PKCS 证书颁发机构</span><span class="sxs-lookup"><span data-stu-id="64acc-210">PKCS Certification Authority</span></span>|
|<span data-ttu-id="64acc-211">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="64acc-211">certificationAuthorityName</span></span>|<span data-ttu-id="64acc-212">String</span><span class="sxs-lookup"><span data-stu-id="64acc-212">String</span></span>|<span data-ttu-id="64acc-213">PKCS 证书颁发机构名称</span><span class="sxs-lookup"><span data-stu-id="64acc-213">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="64acc-214">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="64acc-214">certificateTemplateName</span></span>|<span data-ttu-id="64acc-215">String</span><span class="sxs-lookup"><span data-stu-id="64acc-215">String</span></span>|<span data-ttu-id="64acc-216">PKCS 证书模板名称</span><span class="sxs-lookup"><span data-stu-id="64acc-216">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="64acc-217">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="64acc-217">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="64acc-218">String</span><span class="sxs-lookup"><span data-stu-id="64acc-218">String</span></span>|<span data-ttu-id="64acc-219">定义 AAD 属性的自定义字符串。</span><span class="sxs-lookup"><span data-stu-id="64acc-219">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="64acc-220">响应</span><span class="sxs-lookup"><span data-stu-id="64acc-220">Response</span></span>
<span data-ttu-id="64acc-221">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="64acc-221">If successful, this method returns a `200 OK` response code and an updated [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64acc-222">示例</span><span class="sxs-lookup"><span data-stu-id="64acc-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="64acc-223">请求</span><span class="sxs-lookup"><span data-stu-id="64acc-223">Request</span></span>
<span data-ttu-id="64acc-224">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="64acc-224">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="64acc-225">响应</span><span class="sxs-lookup"><span data-stu-id="64acc-225">Response</span></span>
<span data-ttu-id="64acc-p119">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="64acc-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





