---
title: 创建 androidPkcsCertificateProfile
description: 创建新的 androidPkcsCertificateProfile 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 75c9dcacb8a24dc081158f9a5c5b12e13da3c3d2
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49206977"
---
# <a name="create-androidpkcscertificateprofile"></a><span data-ttu-id="89d07-103">创建 androidPkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="89d07-103">Create androidPkcsCertificateProfile</span></span>

<span data-ttu-id="89d07-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89d07-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="89d07-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="89d07-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="89d07-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="89d07-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="89d07-107">创建新的 [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="89d07-107">Create a new [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="89d07-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="89d07-108">Prerequisites</span></span>
<span data-ttu-id="89d07-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="89d07-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89d07-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="89d07-111">Permission type</span></span>|<span data-ttu-id="89d07-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="89d07-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="89d07-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="89d07-113">Delegated (work or school account)</span></span>|<span data-ttu-id="89d07-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89d07-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="89d07-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="89d07-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="89d07-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="89d07-116">Not supported.</span></span>|
|<span data-ttu-id="89d07-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="89d07-117">Application</span></span>|<span data-ttu-id="89d07-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89d07-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="89d07-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="89d07-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="89d07-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="89d07-120">Request headers</span></span>
|<span data-ttu-id="89d07-121">标头</span><span class="sxs-lookup"><span data-stu-id="89d07-121">Header</span></span>|<span data-ttu-id="89d07-122">值</span><span class="sxs-lookup"><span data-stu-id="89d07-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="89d07-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="89d07-123">Authorization</span></span>|<span data-ttu-id="89d07-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="89d07-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="89d07-125">接受</span><span class="sxs-lookup"><span data-stu-id="89d07-125">Accept</span></span>|<span data-ttu-id="89d07-126">application/json</span><span class="sxs-lookup"><span data-stu-id="89d07-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="89d07-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="89d07-127">Request body</span></span>
<span data-ttu-id="89d07-128">在请求正文中，提供 androidPkcsCertificateProfile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="89d07-128">In the request body, supply a JSON representation for the androidPkcsCertificateProfile object.</span></span>

<span data-ttu-id="89d07-129">下表显示创建 androidPkcsCertificateProfile 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="89d07-129">The following table shows the properties that are required when you create the androidPkcsCertificateProfile.</span></span>

|<span data-ttu-id="89d07-130">属性</span><span class="sxs-lookup"><span data-stu-id="89d07-130">Property</span></span>|<span data-ttu-id="89d07-131">类型</span><span class="sxs-lookup"><span data-stu-id="89d07-131">Type</span></span>|<span data-ttu-id="89d07-132">说明</span><span class="sxs-lookup"><span data-stu-id="89d07-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89d07-133">id</span><span class="sxs-lookup"><span data-stu-id="89d07-133">id</span></span>|<span data-ttu-id="89d07-134">String</span><span class="sxs-lookup"><span data-stu-id="89d07-134">String</span></span>|<span data-ttu-id="89d07-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="89d07-135">Key of the entity.</span></span> <span data-ttu-id="89d07-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="89d07-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89d07-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="89d07-137">lastModifiedDateTime</span></span>|<span data-ttu-id="89d07-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89d07-138">DateTimeOffset</span></span>|<span data-ttu-id="89d07-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="89d07-139">DateTime the object was last modified.</span></span> <span data-ttu-id="89d07-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="89d07-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89d07-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="89d07-141">roleScopeTagIds</span></span>|<span data-ttu-id="89d07-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="89d07-142">String collection</span></span>|<span data-ttu-id="89d07-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="89d07-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="89d07-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="89d07-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89d07-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="89d07-145">supportsScopeTags</span></span>|<span data-ttu-id="89d07-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="89d07-146">Boolean</span></span>|<span data-ttu-id="89d07-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="89d07-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="89d07-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="89d07-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="89d07-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="89d07-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="89d07-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="89d07-150">This property is read-only.</span></span> <span data-ttu-id="89d07-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="89d07-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89d07-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="89d07-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="89d07-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="89d07-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="89d07-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="89d07-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="89d07-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="89d07-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89d07-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="89d07-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="89d07-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="89d07-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="89d07-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="89d07-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="89d07-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="89d07-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89d07-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="89d07-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="89d07-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="89d07-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="89d07-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="89d07-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="89d07-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="89d07-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89d07-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="89d07-164">createdDateTime</span></span>|<span data-ttu-id="89d07-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89d07-165">DateTimeOffset</span></span>|<span data-ttu-id="89d07-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="89d07-166">DateTime the object was created.</span></span> <span data-ttu-id="89d07-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="89d07-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89d07-168">description</span><span class="sxs-lookup"><span data-stu-id="89d07-168">description</span></span>|<span data-ttu-id="89d07-169">String</span><span class="sxs-lookup"><span data-stu-id="89d07-169">String</span></span>|<span data-ttu-id="89d07-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="89d07-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="89d07-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="89d07-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89d07-172">displayName</span><span class="sxs-lookup"><span data-stu-id="89d07-172">displayName</span></span>|<span data-ttu-id="89d07-173">String</span><span class="sxs-lookup"><span data-stu-id="89d07-173">String</span></span>|<span data-ttu-id="89d07-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="89d07-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="89d07-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="89d07-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89d07-176">version</span><span class="sxs-lookup"><span data-stu-id="89d07-176">version</span></span>|<span data-ttu-id="89d07-177">Int32</span><span class="sxs-lookup"><span data-stu-id="89d07-177">Int32</span></span>|<span data-ttu-id="89d07-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="89d07-178">Version of the device configuration.</span></span> <span data-ttu-id="89d07-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="89d07-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89d07-180">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="89d07-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="89d07-181">Int32</span><span class="sxs-lookup"><span data-stu-id="89d07-181">Int32</span></span>|<span data-ttu-id="89d07-182">证书续订阈值百分比。</span><span class="sxs-lookup"><span data-stu-id="89d07-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="89d07-183">从[AndroidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)继承的有效值1到99</span><span class="sxs-lookup"><span data-stu-id="89d07-183">Valid values 1 to 99 Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="89d07-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="89d07-184">subjectNameFormat</span></span>|[<span data-ttu-id="89d07-185">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="89d07-185">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="89d07-186">证书使用者名称格式。</span><span class="sxs-lookup"><span data-stu-id="89d07-186">Certificate Subject Name Format.</span></span> <span data-ttu-id="89d07-187">继承自 [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="89d07-187">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="89d07-188">可取值为：`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId`。</span><span class="sxs-lookup"><span data-stu-id="89d07-188">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="89d07-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="89d07-189">subjectAlternativeNameType</span></span>|[<span data-ttu-id="89d07-190">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="89d07-190">subjectAlternativeNameType</span></span>](../resources/intune-shared-subjectalternativenametype.md)|<span data-ttu-id="89d07-191">证书使用者备用名称类型。</span><span class="sxs-lookup"><span data-stu-id="89d07-191">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="89d07-192">继承自 [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="89d07-192">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="89d07-193">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService`、`universalResourceIdentifier`。</span><span class="sxs-lookup"><span data-stu-id="89d07-193">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span></span>|
|<span data-ttu-id="89d07-194">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="89d07-194">certificateValidityPeriodValue</span></span>|<span data-ttu-id="89d07-195">Int32</span><span class="sxs-lookup"><span data-stu-id="89d07-195">Int32</span></span>|<span data-ttu-id="89d07-196">证书有效期限的值。</span><span class="sxs-lookup"><span data-stu-id="89d07-196">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="89d07-197">继承自 [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="89d07-197">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="89d07-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="89d07-198">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="89d07-199">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="89d07-199">certificateValidityPeriodScale</span></span>](../resources/intune-shared-certificatevalidityperiodscale.md)|<span data-ttu-id="89d07-200">证书有效期的小数位数。</span><span class="sxs-lookup"><span data-stu-id="89d07-200">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="89d07-201">继承自 [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="89d07-201">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="89d07-202">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="89d07-202">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="89d07-203">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="89d07-203">extendedKeyUsages</span></span>|<span data-ttu-id="89d07-204">[extendedKeyUsage](../resources/intune-shared-extendedkeyusage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="89d07-204">[extendedKeyUsage](../resources/intune-shared-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="89d07-205"> (EKU) 设置的扩展密钥用法。</span><span class="sxs-lookup"><span data-stu-id="89d07-205">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="89d07-206">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="89d07-206">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="89d07-207">继承自 [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="89d07-207">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="89d07-208">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="89d07-208">certificationAuthority</span></span>|<span data-ttu-id="89d07-209">String</span><span class="sxs-lookup"><span data-stu-id="89d07-209">String</span></span>|<span data-ttu-id="89d07-210">PKCS 证书颁发机构</span><span class="sxs-lookup"><span data-stu-id="89d07-210">PKCS Certification Authority</span></span>|
|<span data-ttu-id="89d07-211">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="89d07-211">certificationAuthorityName</span></span>|<span data-ttu-id="89d07-212">String</span><span class="sxs-lookup"><span data-stu-id="89d07-212">String</span></span>|<span data-ttu-id="89d07-213">PKCS 证书颁发机构名称</span><span class="sxs-lookup"><span data-stu-id="89d07-213">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="89d07-214">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="89d07-214">certificateTemplateName</span></span>|<span data-ttu-id="89d07-215">String</span><span class="sxs-lookup"><span data-stu-id="89d07-215">String</span></span>|<span data-ttu-id="89d07-216">PKCS 证书模板名称</span><span class="sxs-lookup"><span data-stu-id="89d07-216">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="89d07-217">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="89d07-217">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="89d07-218">String</span><span class="sxs-lookup"><span data-stu-id="89d07-218">String</span></span>|<span data-ttu-id="89d07-219">定义 AAD 属性的自定义字符串。</span><span class="sxs-lookup"><span data-stu-id="89d07-219">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="89d07-220">响应</span><span class="sxs-lookup"><span data-stu-id="89d07-220">Response</span></span>
<span data-ttu-id="89d07-221">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="89d07-221">If successful, this method returns a `201 Created` response code and a [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89d07-222">示例</span><span class="sxs-lookup"><span data-stu-id="89d07-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="89d07-223">请求</span><span class="sxs-lookup"><span data-stu-id="89d07-223">Request</span></span>
<span data-ttu-id="89d07-224">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="89d07-224">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="89d07-225">响应</span><span class="sxs-lookup"><span data-stu-id="89d07-225">Response</span></span>
<span data-ttu-id="89d07-p119">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="89d07-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




