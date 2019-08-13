---
title: 创建 androidPkcsCertificateProfile
description: 创建新的 androidPkcsCertificateProfile 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 64595201a7008ab1c5d09dc1614be6759a396596
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36341064"
---
# <a name="create-androidpkcscertificateprofile"></a><span data-ttu-id="2f404-103">创建 androidPkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="2f404-103">Create androidPkcsCertificateProfile</span></span>

> <span data-ttu-id="2f404-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2f404-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2f404-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2f404-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f404-106">创建新的[androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2f404-106">Create a new [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2f404-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="2f404-107">Prerequisites</span></span>
<span data-ttu-id="2f404-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2f404-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f404-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="2f404-110">Permission type</span></span>|<span data-ttu-id="2f404-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2f404-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f404-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2f404-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2f404-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f404-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2f404-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2f404-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f404-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="2f404-115">Not supported.</span></span>|
|<span data-ttu-id="2f404-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="2f404-116">Application</span></span>|<span data-ttu-id="2f404-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f404-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f404-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2f404-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="2f404-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="2f404-119">Request headers</span></span>
|<span data-ttu-id="2f404-120">标头</span><span class="sxs-lookup"><span data-stu-id="2f404-120">Header</span></span>|<span data-ttu-id="2f404-121">值</span><span class="sxs-lookup"><span data-stu-id="2f404-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f404-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2f404-122">Authorization</span></span>|<span data-ttu-id="2f404-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2f404-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f404-124">接受</span><span class="sxs-lookup"><span data-stu-id="2f404-124">Accept</span></span>|<span data-ttu-id="2f404-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2f404-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f404-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="2f404-126">Request body</span></span>
<span data-ttu-id="2f404-127">在请求正文中, 提供 androidPkcsCertificateProfile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2f404-127">In the request body, supply a JSON representation for the androidPkcsCertificateProfile object.</span></span>

<span data-ttu-id="2f404-128">下表显示创建 androidPkcsCertificateProfile 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2f404-128">The following table shows the properties that are required when you create the androidPkcsCertificateProfile.</span></span>

|<span data-ttu-id="2f404-129">属性</span><span class="sxs-lookup"><span data-stu-id="2f404-129">Property</span></span>|<span data-ttu-id="2f404-130">类型</span><span class="sxs-lookup"><span data-stu-id="2f404-130">Type</span></span>|<span data-ttu-id="2f404-131">说明</span><span class="sxs-lookup"><span data-stu-id="2f404-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f404-132">id</span><span class="sxs-lookup"><span data-stu-id="2f404-132">id</span></span>|<span data-ttu-id="2f404-133">字符串</span><span class="sxs-lookup"><span data-stu-id="2f404-133">String</span></span>|<span data-ttu-id="2f404-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="2f404-134">Key of the entity.</span></span> <span data-ttu-id="2f404-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f404-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f404-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2f404-136">lastModifiedDateTime</span></span>|<span data-ttu-id="2f404-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f404-137">DateTimeOffset</span></span>|<span data-ttu-id="2f404-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="2f404-138">DateTime the object was last modified.</span></span> <span data-ttu-id="2f404-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f404-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f404-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2f404-140">roleScopeTagIds</span></span>|<span data-ttu-id="2f404-141">String collection</span><span class="sxs-lookup"><span data-stu-id="2f404-141">String collection</span></span>|<span data-ttu-id="2f404-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="2f404-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="2f404-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f404-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f404-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="2f404-144">supportsScopeTags</span></span>|<span data-ttu-id="2f404-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f404-145">Boolean</span></span>|<span data-ttu-id="2f404-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="2f404-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="2f404-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="2f404-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="2f404-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="2f404-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="2f404-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="2f404-149">This property is read-only.</span></span> <span data-ttu-id="2f404-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f404-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f404-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="2f404-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="2f404-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="2f404-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="2f404-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="2f404-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="2f404-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f404-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f404-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="2f404-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="2f404-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="2f404-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="2f404-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="2f404-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="2f404-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f404-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f404-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="2f404-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="2f404-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="2f404-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="2f404-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="2f404-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="2f404-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f404-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f404-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2f404-163">createdDateTime</span></span>|<span data-ttu-id="2f404-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f404-164">DateTimeOffset</span></span>|<span data-ttu-id="2f404-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="2f404-165">DateTime the object was created.</span></span> <span data-ttu-id="2f404-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f404-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f404-167">说明</span><span class="sxs-lookup"><span data-stu-id="2f404-167">description</span></span>|<span data-ttu-id="2f404-168">String</span><span class="sxs-lookup"><span data-stu-id="2f404-168">String</span></span>|<span data-ttu-id="2f404-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="2f404-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2f404-170">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f404-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f404-171">displayName</span><span class="sxs-lookup"><span data-stu-id="2f404-171">displayName</span></span>|<span data-ttu-id="2f404-172">String</span><span class="sxs-lookup"><span data-stu-id="2f404-172">String</span></span>|<span data-ttu-id="2f404-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="2f404-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2f404-174">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f404-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f404-175">version</span><span class="sxs-lookup"><span data-stu-id="2f404-175">version</span></span>|<span data-ttu-id="2f404-176">Int32</span><span class="sxs-lookup"><span data-stu-id="2f404-176">Int32</span></span>|<span data-ttu-id="2f404-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="2f404-177">Version of the device configuration.</span></span> <span data-ttu-id="2f404-178">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f404-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f404-179">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="2f404-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="2f404-180">Int32</span><span class="sxs-lookup"><span data-stu-id="2f404-180">Int32</span></span>|<span data-ttu-id="2f404-181">证书续订阈值百分比。</span><span class="sxs-lookup"><span data-stu-id="2f404-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="2f404-182">从[AndroidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)继承的有效值1到99</span><span class="sxs-lookup"><span data-stu-id="2f404-182">Valid values 1 to 99 Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="2f404-183">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="2f404-183">subjectNameFormat</span></span>|[<span data-ttu-id="2f404-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="2f404-184">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="2f404-185">证书使用者名称格式。</span><span class="sxs-lookup"><span data-stu-id="2f404-185">Certificate Subject Name Format.</span></span> <span data-ttu-id="2f404-186">继承自[androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="2f404-186">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="2f404-187">可取值为：`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId`。</span><span class="sxs-lookup"><span data-stu-id="2f404-187">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="2f404-188">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="2f404-188">subjectAlternativeNameType</span></span>|[<span data-ttu-id="2f404-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="2f404-189">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="2f404-190">证书使用者备用名称类型。</span><span class="sxs-lookup"><span data-stu-id="2f404-190">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="2f404-191">继承自[androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="2f404-191">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="2f404-192">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService`。</span><span class="sxs-lookup"><span data-stu-id="2f404-192">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="2f404-193">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="2f404-193">certificateValidityPeriodValue</span></span>|<span data-ttu-id="2f404-194">Int32</span><span class="sxs-lookup"><span data-stu-id="2f404-194">Int32</span></span>|<span data-ttu-id="2f404-195">证书有效期限的值。</span><span class="sxs-lookup"><span data-stu-id="2f404-195">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="2f404-196">继承自[androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="2f404-196">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="2f404-197">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="2f404-197">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="2f404-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="2f404-198">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="2f404-199">证书有效期的小数位数。</span><span class="sxs-lookup"><span data-stu-id="2f404-199">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="2f404-200">继承自[androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="2f404-200">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="2f404-201">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="2f404-201">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="2f404-202">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="2f404-202">extendedKeyUsages</span></span>|<span data-ttu-id="2f404-203">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)集合</span><span class="sxs-lookup"><span data-stu-id="2f404-203">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="2f404-204">扩展密钥用法 (EKU) 设置。</span><span class="sxs-lookup"><span data-stu-id="2f404-204">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="2f404-205">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="2f404-205">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="2f404-206">继承自[androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="2f404-206">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="2f404-207">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="2f404-207">certificationAuthority</span></span>|<span data-ttu-id="2f404-208">String</span><span class="sxs-lookup"><span data-stu-id="2f404-208">String</span></span>|<span data-ttu-id="2f404-209">PKCS 证书颁发机构</span><span class="sxs-lookup"><span data-stu-id="2f404-209">PKCS Certification Authority</span></span>|
|<span data-ttu-id="2f404-210">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="2f404-210">certificationAuthorityName</span></span>|<span data-ttu-id="2f404-211">String</span><span class="sxs-lookup"><span data-stu-id="2f404-211">String</span></span>|<span data-ttu-id="2f404-212">PKCS 证书颁发机构名称</span><span class="sxs-lookup"><span data-stu-id="2f404-212">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="2f404-213">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="2f404-213">certificateTemplateName</span></span>|<span data-ttu-id="2f404-214">String</span><span class="sxs-lookup"><span data-stu-id="2f404-214">String</span></span>|<span data-ttu-id="2f404-215">PKCS 证书模板名称</span><span class="sxs-lookup"><span data-stu-id="2f404-215">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="2f404-216">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="2f404-216">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="2f404-217">String</span><span class="sxs-lookup"><span data-stu-id="2f404-217">String</span></span>|<span data-ttu-id="2f404-218">定义 AAD 属性的自定义字符串。</span><span class="sxs-lookup"><span data-stu-id="2f404-218">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="2f404-219">响应</span><span class="sxs-lookup"><span data-stu-id="2f404-219">Response</span></span>
<span data-ttu-id="2f404-220">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2f404-220">If successful, this method returns a `201 Created` response code and a [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f404-221">示例</span><span class="sxs-lookup"><span data-stu-id="2f404-221">Example</span></span>

### <a name="request"></a><span data-ttu-id="2f404-222">请求</span><span class="sxs-lookup"><span data-stu-id="2f404-222">Request</span></span>
<span data-ttu-id="2f404-223">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2f404-223">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2f404-224">响应</span><span class="sxs-lookup"><span data-stu-id="2f404-224">Response</span></span>
<span data-ttu-id="2f404-p119">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2f404-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






