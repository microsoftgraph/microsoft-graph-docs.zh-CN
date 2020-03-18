---
title: 创建 androidWorkProfilePkcsCertificateProfile
description: 创建新的 androidWorkProfilePkcsCertificateProfile 对象。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 167b0a69d0be0ed18cf4a420b2f043f4b7207267
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42758360"
---
# <a name="create-androidworkprofilepkcscertificateprofile"></a><span data-ttu-id="2c094-103">创建 androidWorkProfilePkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="2c094-103">Create androidWorkProfilePkcsCertificateProfile</span></span>

> <span data-ttu-id="2c094-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2c094-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2c094-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2c094-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2c094-106">创建新的[androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2c094-106">Create a new [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2c094-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="2c094-107">Prerequisites</span></span>
<span data-ttu-id="2c094-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2c094-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2c094-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="2c094-110">Permission type</span></span>|<span data-ttu-id="2c094-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2c094-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2c094-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2c094-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2c094-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c094-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2c094-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2c094-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2c094-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="2c094-115">Not supported.</span></span>|
|<span data-ttu-id="2c094-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="2c094-116">Application</span></span>|<span data-ttu-id="2c094-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c094-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2c094-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2c094-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="2c094-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="2c094-119">Request headers</span></span>
|<span data-ttu-id="2c094-120">标头</span><span class="sxs-lookup"><span data-stu-id="2c094-120">Header</span></span>|<span data-ttu-id="2c094-121">值</span><span class="sxs-lookup"><span data-stu-id="2c094-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2c094-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2c094-122">Authorization</span></span>|<span data-ttu-id="2c094-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2c094-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2c094-124">接受</span><span class="sxs-lookup"><span data-stu-id="2c094-124">Accept</span></span>|<span data-ttu-id="2c094-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2c094-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2c094-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="2c094-126">Request body</span></span>
<span data-ttu-id="2c094-127">在请求正文中，提供 androidWorkProfilePkcsCertificateProfile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2c094-127">In the request body, supply a JSON representation for the androidWorkProfilePkcsCertificateProfile object.</span></span>

<span data-ttu-id="2c094-128">下表显示创建 androidWorkProfilePkcsCertificateProfile 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2c094-128">The following table shows the properties that are required when you create the androidWorkProfilePkcsCertificateProfile.</span></span>

|<span data-ttu-id="2c094-129">属性</span><span class="sxs-lookup"><span data-stu-id="2c094-129">Property</span></span>|<span data-ttu-id="2c094-130">类型</span><span class="sxs-lookup"><span data-stu-id="2c094-130">Type</span></span>|<span data-ttu-id="2c094-131">说明</span><span class="sxs-lookup"><span data-stu-id="2c094-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c094-132">id</span><span class="sxs-lookup"><span data-stu-id="2c094-132">id</span></span>|<span data-ttu-id="2c094-133">字符串</span><span class="sxs-lookup"><span data-stu-id="2c094-133">String</span></span>|<span data-ttu-id="2c094-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="2c094-134">Key of the entity.</span></span> <span data-ttu-id="2c094-135">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2c094-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2c094-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2c094-136">lastModifiedDateTime</span></span>|<span data-ttu-id="2c094-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2c094-137">DateTimeOffset</span></span>|<span data-ttu-id="2c094-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="2c094-138">DateTime the object was last modified.</span></span> <span data-ttu-id="2c094-139">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2c094-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2c094-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2c094-140">roleScopeTagIds</span></span>|<span data-ttu-id="2c094-141">String collection</span><span class="sxs-lookup"><span data-stu-id="2c094-141">String collection</span></span>|<span data-ttu-id="2c094-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="2c094-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="2c094-143">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2c094-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2c094-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="2c094-144">supportsScopeTags</span></span>|<span data-ttu-id="2c094-145">布尔值</span><span class="sxs-lookup"><span data-stu-id="2c094-145">Boolean</span></span>|<span data-ttu-id="2c094-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="2c094-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="2c094-147">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="2c094-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="2c094-148">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="2c094-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="2c094-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="2c094-149">This property is read-only.</span></span> <span data-ttu-id="2c094-150">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2c094-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2c094-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="2c094-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="2c094-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="2c094-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="2c094-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="2c094-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="2c094-154">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2c094-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2c094-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="2c094-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="2c094-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="2c094-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="2c094-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="2c094-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="2c094-158">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2c094-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2c094-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="2c094-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="2c094-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="2c094-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="2c094-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="2c094-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="2c094-162">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2c094-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2c094-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2c094-163">createdDateTime</span></span>|<span data-ttu-id="2c094-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2c094-164">DateTimeOffset</span></span>|<span data-ttu-id="2c094-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="2c094-165">DateTime the object was created.</span></span> <span data-ttu-id="2c094-166">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2c094-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2c094-167">说明</span><span class="sxs-lookup"><span data-stu-id="2c094-167">description</span></span>|<span data-ttu-id="2c094-168">String</span><span class="sxs-lookup"><span data-stu-id="2c094-168">String</span></span>|<span data-ttu-id="2c094-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="2c094-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2c094-170">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2c094-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2c094-171">displayName</span><span class="sxs-lookup"><span data-stu-id="2c094-171">displayName</span></span>|<span data-ttu-id="2c094-172">String</span><span class="sxs-lookup"><span data-stu-id="2c094-172">String</span></span>|<span data-ttu-id="2c094-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="2c094-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2c094-174">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2c094-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2c094-175">version</span><span class="sxs-lookup"><span data-stu-id="2c094-175">version</span></span>|<span data-ttu-id="2c094-176">Int32</span><span class="sxs-lookup"><span data-stu-id="2c094-176">Int32</span></span>|<span data-ttu-id="2c094-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="2c094-177">Version of the device configuration.</span></span> <span data-ttu-id="2c094-178">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2c094-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2c094-179">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="2c094-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="2c094-180">Int32</span><span class="sxs-lookup"><span data-stu-id="2c094-180">Int32</span></span>|<span data-ttu-id="2c094-181">证书续订阈值百分比。</span><span class="sxs-lookup"><span data-stu-id="2c094-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="2c094-182">从[AndroidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)继承的有效值1到99</span><span class="sxs-lookup"><span data-stu-id="2c094-182">Valid values 1 to 99 Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="2c094-183">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="2c094-183">subjectNameFormat</span></span>|[<span data-ttu-id="2c094-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="2c094-184">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="2c094-185">证书使用者名称格式。</span><span class="sxs-lookup"><span data-stu-id="2c094-185">Certificate Subject Name Format.</span></span> <span data-ttu-id="2c094-186">继承自[androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="2c094-186">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="2c094-187">可取值为：`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId`。</span><span class="sxs-lookup"><span data-stu-id="2c094-187">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="2c094-188">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="2c094-188">certificateValidityPeriodValue</span></span>|<span data-ttu-id="2c094-189">Int32</span><span class="sxs-lookup"><span data-stu-id="2c094-189">Int32</span></span>|<span data-ttu-id="2c094-190">证书有效期限的值。</span><span class="sxs-lookup"><span data-stu-id="2c094-190">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="2c094-191">继承自[androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="2c094-191">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="2c094-192">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="2c094-192">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="2c094-193">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="2c094-193">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="2c094-194">证书有效期的小数位数。</span><span class="sxs-lookup"><span data-stu-id="2c094-194">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="2c094-195">继承自[androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="2c094-195">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="2c094-196">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="2c094-196">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="2c094-197">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="2c094-197">extendedKeyUsages</span></span>|<span data-ttu-id="2c094-198">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)集合</span><span class="sxs-lookup"><span data-stu-id="2c094-198">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="2c094-199">扩展密钥用法（EKU）设置。</span><span class="sxs-lookup"><span data-stu-id="2c094-199">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="2c094-200">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="2c094-200">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="2c094-201">继承自[androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="2c094-201">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="2c094-202">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="2c094-202">subjectAlternativeNameType</span></span>|[<span data-ttu-id="2c094-203">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="2c094-203">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="2c094-204">证书使用者备用名称类型。</span><span class="sxs-lookup"><span data-stu-id="2c094-204">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="2c094-205">继承自[androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="2c094-205">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="2c094-206">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService`。</span><span class="sxs-lookup"><span data-stu-id="2c094-206">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="2c094-207">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="2c094-207">certificationAuthority</span></span>|<span data-ttu-id="2c094-208">String</span><span class="sxs-lookup"><span data-stu-id="2c094-208">String</span></span>|<span data-ttu-id="2c094-209">PKCS 证书颁发机构</span><span class="sxs-lookup"><span data-stu-id="2c094-209">PKCS Certification Authority</span></span>|
|<span data-ttu-id="2c094-210">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="2c094-210">certificationAuthorityName</span></span>|<span data-ttu-id="2c094-211">String</span><span class="sxs-lookup"><span data-stu-id="2c094-211">String</span></span>|<span data-ttu-id="2c094-212">PKCS 证书颁发机构名称</span><span class="sxs-lookup"><span data-stu-id="2c094-212">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="2c094-213">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="2c094-213">certificateTemplateName</span></span>|<span data-ttu-id="2c094-214">String</span><span class="sxs-lookup"><span data-stu-id="2c094-214">String</span></span>|<span data-ttu-id="2c094-215">PKCS 证书模板名称</span><span class="sxs-lookup"><span data-stu-id="2c094-215">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="2c094-216">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="2c094-216">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="2c094-217">String</span><span class="sxs-lookup"><span data-stu-id="2c094-217">String</span></span>|<span data-ttu-id="2c094-218">定义 AAD 属性的自定义字符串。</span><span class="sxs-lookup"><span data-stu-id="2c094-218">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="2c094-219">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="2c094-219">subjectNameFormatString</span></span>|<span data-ttu-id="2c094-220">String</span><span class="sxs-lookup"><span data-stu-id="2c094-220">String</span></span>|<span data-ttu-id="2c094-221">要与 SubjectNameFormat = Custom 一起使用的自定义格式。</span><span class="sxs-lookup"><span data-stu-id="2c094-221">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="2c094-222">示例： CN = {{EmailAddress}}，E = {{EmailAddress}}，OU = 企业用户，O = Contoso Corporation，L = Redmond，ST = WA，C = US</span><span class="sxs-lookup"><span data-stu-id="2c094-222">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="2c094-223">certificateStore</span><span class="sxs-lookup"><span data-stu-id="2c094-223">certificateStore</span></span>|[<span data-ttu-id="2c094-224">certificateStore</span><span class="sxs-lookup"><span data-stu-id="2c094-224">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="2c094-225">目标存储证书。</span><span class="sxs-lookup"><span data-stu-id="2c094-225">Target store certificate.</span></span> <span data-ttu-id="2c094-226">可取值为：`user`、`machine`。</span><span class="sxs-lookup"><span data-stu-id="2c094-226">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="2c094-227">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="2c094-227">customSubjectAlternativeNames</span></span>|<span data-ttu-id="2c094-228">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)集合</span><span class="sxs-lookup"><span data-stu-id="2c094-228">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="2c094-229">自定义主题备用名称设置。</span><span class="sxs-lookup"><span data-stu-id="2c094-229">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="2c094-230">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="2c094-230">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="2c094-231">响应</span><span class="sxs-lookup"><span data-stu-id="2c094-231">Response</span></span>
<span data-ttu-id="2c094-232">如果成功，此方法在响应`201 Created`正文中返回响应代码和[androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2c094-232">If successful, this method returns a `201 Created` response code and a [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2c094-233">示例</span><span class="sxs-lookup"><span data-stu-id="2c094-233">Example</span></span>

### <a name="request"></a><span data-ttu-id="2c094-234">请求</span><span class="sxs-lookup"><span data-stu-id="2c094-234">Request</span></span>
<span data-ttu-id="2c094-235">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2c094-235">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2032

{
  "@odata.type": "#microsoft.graph.androidWorkProfilePkcsCertificateProfile",
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
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "subjectAlternativeNameType": "emailAddress",
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "subjectNameFormatString": "Subject Name Format String value",
  "certificateStore": "machine",
  "customSubjectAlternativeNames": [
    {
      "@odata.type": "microsoft.graph.customSubjectAlternativeName",
      "sanType": "emailAddress",
      "name": "Name value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="2c094-236">响应</span><span class="sxs-lookup"><span data-stu-id="2c094-236">Response</span></span>
<span data-ttu-id="2c094-p122">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2c094-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2204

{
  "@odata.type": "#microsoft.graph.androidWorkProfilePkcsCertificateProfile",
  "id": "a7d4a505-a505-a7d4-05a5-d4a705a5d4a7",
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
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "subjectAlternativeNameType": "emailAddress",
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "subjectNameFormatString": "Subject Name Format String value",
  "certificateStore": "machine",
  "customSubjectAlternativeNames": [
    {
      "@odata.type": "microsoft.graph.customSubjectAlternativeName",
      "sanType": "emailAddress",
      "name": "Name value"
    }
  ]
}
```




