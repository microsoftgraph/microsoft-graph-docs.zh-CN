---
title: 更新 androidScepCertificateProfile
description: 更新 androidScepCertificateProfile 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b2b585d6034f6df4837338adac19b3e1b157da0e
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49265876"
---
# <a name="update-androidscepcertificateprofile"></a><span data-ttu-id="71302-103">更新 androidScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="71302-103">Update androidScepCertificateProfile</span></span>

<span data-ttu-id="71302-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71302-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="71302-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="71302-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="71302-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="71302-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="71302-107">更新 [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="71302-107">Update the properties of a [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="71302-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="71302-108">Prerequisites</span></span>
<span data-ttu-id="71302-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="71302-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71302-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="71302-111">Permission type</span></span>|<span data-ttu-id="71302-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="71302-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="71302-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="71302-113">Delegated (work or school account)</span></span>|<span data-ttu-id="71302-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71302-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="71302-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="71302-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="71302-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="71302-116">Not supported.</span></span>|
|<span data-ttu-id="71302-117">Application</span><span class="sxs-lookup"><span data-stu-id="71302-117">Application</span></span>|<span data-ttu-id="71302-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71302-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="71302-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="71302-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="71302-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="71302-120">Request headers</span></span>
|<span data-ttu-id="71302-121">标头</span><span class="sxs-lookup"><span data-stu-id="71302-121">Header</span></span>|<span data-ttu-id="71302-122">值</span><span class="sxs-lookup"><span data-stu-id="71302-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="71302-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="71302-123">Authorization</span></span>|<span data-ttu-id="71302-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="71302-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="71302-125">接受</span><span class="sxs-lookup"><span data-stu-id="71302-125">Accept</span></span>|<span data-ttu-id="71302-126">application/json</span><span class="sxs-lookup"><span data-stu-id="71302-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="71302-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="71302-127">Request body</span></span>
<span data-ttu-id="71302-128">在请求正文中，提供 [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="71302-128">In the request body, supply a JSON representation for the [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) object.</span></span>

<span data-ttu-id="71302-129">下表显示创建 [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="71302-129">The following table shows the properties that are required when you create the [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md).</span></span>

|<span data-ttu-id="71302-130">属性</span><span class="sxs-lookup"><span data-stu-id="71302-130">Property</span></span>|<span data-ttu-id="71302-131">类型</span><span class="sxs-lookup"><span data-stu-id="71302-131">Type</span></span>|<span data-ttu-id="71302-132">说明</span><span class="sxs-lookup"><span data-stu-id="71302-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71302-133">id</span><span class="sxs-lookup"><span data-stu-id="71302-133">id</span></span>|<span data-ttu-id="71302-134">字符串</span><span class="sxs-lookup"><span data-stu-id="71302-134">String</span></span>|<span data-ttu-id="71302-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="71302-135">Key of the entity.</span></span> <span data-ttu-id="71302-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="71302-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71302-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="71302-137">lastModifiedDateTime</span></span>|<span data-ttu-id="71302-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71302-138">DateTimeOffset</span></span>|<span data-ttu-id="71302-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="71302-139">DateTime the object was last modified.</span></span> <span data-ttu-id="71302-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="71302-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71302-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="71302-141">roleScopeTagIds</span></span>|<span data-ttu-id="71302-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="71302-142">String collection</span></span>|<span data-ttu-id="71302-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="71302-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="71302-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="71302-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71302-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="71302-145">supportsScopeTags</span></span>|<span data-ttu-id="71302-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="71302-146">Boolean</span></span>|<span data-ttu-id="71302-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="71302-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="71302-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="71302-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="71302-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="71302-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="71302-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="71302-150">This property is read-only.</span></span> <span data-ttu-id="71302-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="71302-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71302-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="71302-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="71302-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="71302-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="71302-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="71302-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="71302-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="71302-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71302-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="71302-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="71302-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="71302-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="71302-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="71302-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="71302-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="71302-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71302-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="71302-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="71302-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="71302-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="71302-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="71302-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="71302-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="71302-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71302-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="71302-164">createdDateTime</span></span>|<span data-ttu-id="71302-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71302-165">DateTimeOffset</span></span>|<span data-ttu-id="71302-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="71302-166">DateTime the object was created.</span></span> <span data-ttu-id="71302-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="71302-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71302-168">description</span><span class="sxs-lookup"><span data-stu-id="71302-168">description</span></span>|<span data-ttu-id="71302-169">字符串</span><span class="sxs-lookup"><span data-stu-id="71302-169">String</span></span>|<span data-ttu-id="71302-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="71302-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="71302-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="71302-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71302-172">displayName</span><span class="sxs-lookup"><span data-stu-id="71302-172">displayName</span></span>|<span data-ttu-id="71302-173">字符串</span><span class="sxs-lookup"><span data-stu-id="71302-173">String</span></span>|<span data-ttu-id="71302-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="71302-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="71302-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="71302-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71302-176">version</span><span class="sxs-lookup"><span data-stu-id="71302-176">version</span></span>|<span data-ttu-id="71302-177">Int32</span><span class="sxs-lookup"><span data-stu-id="71302-177">Int32</span></span>|<span data-ttu-id="71302-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="71302-178">Version of the device configuration.</span></span> <span data-ttu-id="71302-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="71302-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71302-180">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="71302-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="71302-181">Int32</span><span class="sxs-lookup"><span data-stu-id="71302-181">Int32</span></span>|<span data-ttu-id="71302-182">证书续订阈值百分比。</span><span class="sxs-lookup"><span data-stu-id="71302-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="71302-183">从[AndroidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)继承的有效值1到99</span><span class="sxs-lookup"><span data-stu-id="71302-183">Valid values 1 to 99 Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="71302-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="71302-184">subjectNameFormat</span></span>|[<span data-ttu-id="71302-185">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="71302-185">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="71302-186">证书使用者名称格式。</span><span class="sxs-lookup"><span data-stu-id="71302-186">Certificate Subject Name Format.</span></span> <span data-ttu-id="71302-187">继承自 [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="71302-187">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="71302-188">可取值为：`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId`。</span><span class="sxs-lookup"><span data-stu-id="71302-188">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="71302-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="71302-189">subjectAlternativeNameType</span></span>|[<span data-ttu-id="71302-190">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="71302-190">subjectAlternativeNameType</span></span>](../resources/intune-shared-subjectalternativenametype.md)|<span data-ttu-id="71302-191">证书使用者备用名称类型。</span><span class="sxs-lookup"><span data-stu-id="71302-191">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="71302-192">继承自 [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="71302-192">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="71302-193">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService`、`universalResourceIdentifier`。</span><span class="sxs-lookup"><span data-stu-id="71302-193">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span></span>|
|<span data-ttu-id="71302-194">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="71302-194">certificateValidityPeriodValue</span></span>|<span data-ttu-id="71302-195">Int32</span><span class="sxs-lookup"><span data-stu-id="71302-195">Int32</span></span>|<span data-ttu-id="71302-196">证书有效期限的值。</span><span class="sxs-lookup"><span data-stu-id="71302-196">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="71302-197">继承自 [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="71302-197">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="71302-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="71302-198">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="71302-199">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="71302-199">certificateValidityPeriodScale</span></span>](../resources/intune-shared-certificatevalidityperiodscale.md)|<span data-ttu-id="71302-200">证书有效期的小数位数。</span><span class="sxs-lookup"><span data-stu-id="71302-200">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="71302-201">继承自 [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="71302-201">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="71302-202">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="71302-202">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="71302-203">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="71302-203">extendedKeyUsages</span></span>|<span data-ttu-id="71302-204">[extendedKeyUsage](../resources/intune-shared-extendedkeyusage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="71302-204">[extendedKeyUsage](../resources/intune-shared-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="71302-205"> (EKU) 设置的扩展密钥用法。</span><span class="sxs-lookup"><span data-stu-id="71302-205">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="71302-206">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="71302-206">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="71302-207">继承自 [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="71302-207">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="71302-208">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="71302-208">scepServerUrls</span></span>|<span data-ttu-id="71302-209">String 集合</span><span class="sxs-lookup"><span data-stu-id="71302-209">String collection</span></span>|<span data-ttu-id="71302-210">SCEP 服务器 Url (s) </span><span class="sxs-lookup"><span data-stu-id="71302-210">SCEP Server Url(s)</span></span>|
|<span data-ttu-id="71302-211">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="71302-211">subjectNameFormatString</span></span>|<span data-ttu-id="71302-212">字符串</span><span class="sxs-lookup"><span data-stu-id="71302-212">String</span></span>|<span data-ttu-id="71302-213">要与 SubjectNameFormat = Custom 一起使用的自定义格式。</span><span class="sxs-lookup"><span data-stu-id="71302-213">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="71302-214">示例： CN = {{EmailAddress}}，E = {{EmailAddress}}，OU = 企业用户，O = Contoso Corporation，L = Redmond，ST = WA，C = US</span><span class="sxs-lookup"><span data-stu-id="71302-214">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="71302-215">keyUsage</span><span class="sxs-lookup"><span data-stu-id="71302-215">keyUsage</span></span>|[<span data-ttu-id="71302-216">keyUsages</span><span class="sxs-lookup"><span data-stu-id="71302-216">keyUsages</span></span>](../resources/intune-shared-keyusages.md)|<span data-ttu-id="71302-217">SCEP 密钥用法。</span><span class="sxs-lookup"><span data-stu-id="71302-217">SCEP Key Usage.</span></span> <span data-ttu-id="71302-218">可取值为：`keyEncipherment`、`digitalSignature`。</span><span class="sxs-lookup"><span data-stu-id="71302-218">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="71302-219">keySize</span><span class="sxs-lookup"><span data-stu-id="71302-219">keySize</span></span>|[<span data-ttu-id="71302-220">keySize</span><span class="sxs-lookup"><span data-stu-id="71302-220">keySize</span></span>](../resources/intune-shared-keysize.md)|<span data-ttu-id="71302-221">SCEP 密钥大小。</span><span class="sxs-lookup"><span data-stu-id="71302-221">SCEP Key Size.</span></span> <span data-ttu-id="71302-222">可取值为：`size1024`、`size2048`、`size4096`。</span><span class="sxs-lookup"><span data-stu-id="71302-222">Possible values are: `size1024`, `size2048`, `size4096`.</span></span>|
|<span data-ttu-id="71302-223">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="71302-223">hashAlgorithm</span></span>|[<span data-ttu-id="71302-224">hashAlgorithms</span><span class="sxs-lookup"><span data-stu-id="71302-224">hashAlgorithms</span></span>](../resources/intune-shared-hashalgorithms.md)|<span data-ttu-id="71302-225">SCEP 哈希算法。</span><span class="sxs-lookup"><span data-stu-id="71302-225">SCEP Hash Algorithm.</span></span> <span data-ttu-id="71302-226">可取值为：`sha1`、`sha2`。</span><span class="sxs-lookup"><span data-stu-id="71302-226">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="71302-227">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="71302-227">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="71302-228">字符串</span><span class="sxs-lookup"><span data-stu-id="71302-228">String</span></span>|<span data-ttu-id="71302-229">定义 AAD 属性的自定义字符串。</span><span class="sxs-lookup"><span data-stu-id="71302-229">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="71302-230">响应</span><span class="sxs-lookup"><span data-stu-id="71302-230">Response</span></span>
<span data-ttu-id="71302-231">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="71302-231">If successful, this method returns a `200 OK` response code and an updated [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71302-232">示例</span><span class="sxs-lookup"><span data-stu-id="71302-232">Example</span></span>

### <a name="request"></a><span data-ttu-id="71302-233">请求</span><span class="sxs-lookup"><span data-stu-id="71302-233">Request</span></span>
<span data-ttu-id="71302-234">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="71302-234">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="71302-235">响应</span><span class="sxs-lookup"><span data-stu-id="71302-235">Response</span></span>
<span data-ttu-id="71302-p123">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="71302-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




