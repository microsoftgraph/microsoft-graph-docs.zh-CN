---
title: 更新 androidForWorkPkcsCertificateProfile
description: 更新 androidForWorkPkcsCertificateProfile 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e8b6a5bd206b1ec152bfe1050fc79774dbfcede9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48066208"
---
# <a name="update-androidforworkpkcscertificateprofile"></a><span data-ttu-id="44028-103">更新 androidForWorkPkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="44028-103">Update androidForWorkPkcsCertificateProfile</span></span>

<span data-ttu-id="44028-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="44028-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="44028-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="44028-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="44028-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="44028-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="44028-107">更新 [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="44028-107">Update the properties of a [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="44028-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="44028-108">Prerequisites</span></span>
<span data-ttu-id="44028-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="44028-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44028-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="44028-111">Permission type</span></span>|<span data-ttu-id="44028-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="44028-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="44028-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="44028-113">Delegated (work or school account)</span></span>|<span data-ttu-id="44028-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44028-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="44028-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="44028-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="44028-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="44028-116">Not supported.</span></span>|
|<span data-ttu-id="44028-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="44028-117">Application</span></span>|<span data-ttu-id="44028-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44028-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="44028-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="44028-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="44028-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="44028-120">Request headers</span></span>
|<span data-ttu-id="44028-121">标头</span><span class="sxs-lookup"><span data-stu-id="44028-121">Header</span></span>|<span data-ttu-id="44028-122">值</span><span class="sxs-lookup"><span data-stu-id="44028-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="44028-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="44028-123">Authorization</span></span>|<span data-ttu-id="44028-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="44028-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="44028-125">接受</span><span class="sxs-lookup"><span data-stu-id="44028-125">Accept</span></span>|<span data-ttu-id="44028-126">application/json</span><span class="sxs-lookup"><span data-stu-id="44028-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="44028-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="44028-127">Request body</span></span>
<span data-ttu-id="44028-128">在请求正文中，提供 [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="44028-128">In the request body, supply a JSON representation for the [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) object.</span></span>

<span data-ttu-id="44028-129">下表显示创建 [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="44028-129">The following table shows the properties that are required when you create the [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md).</span></span>

|<span data-ttu-id="44028-130">属性</span><span class="sxs-lookup"><span data-stu-id="44028-130">Property</span></span>|<span data-ttu-id="44028-131">类型</span><span class="sxs-lookup"><span data-stu-id="44028-131">Type</span></span>|<span data-ttu-id="44028-132">说明</span><span class="sxs-lookup"><span data-stu-id="44028-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44028-133">id</span><span class="sxs-lookup"><span data-stu-id="44028-133">id</span></span>|<span data-ttu-id="44028-134">String</span><span class="sxs-lookup"><span data-stu-id="44028-134">String</span></span>|<span data-ttu-id="44028-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="44028-135">Key of the entity.</span></span> <span data-ttu-id="44028-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="44028-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44028-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="44028-137">lastModifiedDateTime</span></span>|<span data-ttu-id="44028-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44028-138">DateTimeOffset</span></span>|<span data-ttu-id="44028-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="44028-139">DateTime the object was last modified.</span></span> <span data-ttu-id="44028-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="44028-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44028-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="44028-141">roleScopeTagIds</span></span>|<span data-ttu-id="44028-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="44028-142">String collection</span></span>|<span data-ttu-id="44028-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="44028-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="44028-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="44028-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44028-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="44028-145">supportsScopeTags</span></span>|<span data-ttu-id="44028-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="44028-146">Boolean</span></span>|<span data-ttu-id="44028-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="44028-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="44028-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="44028-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="44028-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="44028-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="44028-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="44028-150">This property is read-only.</span></span> <span data-ttu-id="44028-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="44028-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44028-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="44028-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="44028-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="44028-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="44028-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="44028-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="44028-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="44028-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44028-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="44028-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="44028-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="44028-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="44028-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="44028-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="44028-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="44028-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44028-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="44028-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="44028-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="44028-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="44028-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="44028-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="44028-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="44028-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44028-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="44028-164">createdDateTime</span></span>|<span data-ttu-id="44028-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44028-165">DateTimeOffset</span></span>|<span data-ttu-id="44028-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="44028-166">DateTime the object was created.</span></span> <span data-ttu-id="44028-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="44028-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44028-168">说明</span><span class="sxs-lookup"><span data-stu-id="44028-168">description</span></span>|<span data-ttu-id="44028-169">String</span><span class="sxs-lookup"><span data-stu-id="44028-169">String</span></span>|<span data-ttu-id="44028-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="44028-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="44028-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="44028-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44028-172">displayName</span><span class="sxs-lookup"><span data-stu-id="44028-172">displayName</span></span>|<span data-ttu-id="44028-173">String</span><span class="sxs-lookup"><span data-stu-id="44028-173">String</span></span>|<span data-ttu-id="44028-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="44028-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="44028-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="44028-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44028-176">version</span><span class="sxs-lookup"><span data-stu-id="44028-176">version</span></span>|<span data-ttu-id="44028-177">Int32</span><span class="sxs-lookup"><span data-stu-id="44028-177">Int32</span></span>|<span data-ttu-id="44028-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="44028-178">Version of the device configuration.</span></span> <span data-ttu-id="44028-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="44028-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44028-180">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="44028-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="44028-181">Int32</span><span class="sxs-lookup"><span data-stu-id="44028-181">Int32</span></span>|<span data-ttu-id="44028-182">证书续订阈值百分比。</span><span class="sxs-lookup"><span data-stu-id="44028-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="44028-183">从[AndroidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)继承的有效值1到99</span><span class="sxs-lookup"><span data-stu-id="44028-183">Valid values 1 to 99 Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="44028-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="44028-184">subjectNameFormat</span></span>|[<span data-ttu-id="44028-185">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="44028-185">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="44028-186">证书使用者名称格式。</span><span class="sxs-lookup"><span data-stu-id="44028-186">Certificate Subject Name Format.</span></span> <span data-ttu-id="44028-187">继承自 [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="44028-187">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="44028-188">可取值为：`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId`。</span><span class="sxs-lookup"><span data-stu-id="44028-188">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="44028-189">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="44028-189">certificateValidityPeriodValue</span></span>|<span data-ttu-id="44028-190">Int32</span><span class="sxs-lookup"><span data-stu-id="44028-190">Int32</span></span>|<span data-ttu-id="44028-191">证书有效期限的值。</span><span class="sxs-lookup"><span data-stu-id="44028-191">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="44028-192">继承自 [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="44028-192">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="44028-193">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="44028-193">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="44028-194">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="44028-194">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="44028-195">证书有效期的小数位数。</span><span class="sxs-lookup"><span data-stu-id="44028-195">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="44028-196">继承自 [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="44028-196">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="44028-197">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="44028-197">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="44028-198">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="44028-198">extendedKeyUsages</span></span>|<span data-ttu-id="44028-199">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="44028-199">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="44028-200"> (EKU) 设置的扩展密钥用法。</span><span class="sxs-lookup"><span data-stu-id="44028-200">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="44028-201">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="44028-201">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="44028-202">继承自 [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="44028-202">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="44028-203">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="44028-203">subjectAlternativeNameType</span></span>|[<span data-ttu-id="44028-204">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="44028-204">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="44028-205">证书使用者备用名称类型。</span><span class="sxs-lookup"><span data-stu-id="44028-205">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="44028-206">继承自 [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="44028-206">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="44028-207">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService`。</span><span class="sxs-lookup"><span data-stu-id="44028-207">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="44028-208">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="44028-208">certificationAuthority</span></span>|<span data-ttu-id="44028-209">String</span><span class="sxs-lookup"><span data-stu-id="44028-209">String</span></span>|<span data-ttu-id="44028-210">PKCS 证书颁发机构</span><span class="sxs-lookup"><span data-stu-id="44028-210">PKCS Certification Authority</span></span>|
|<span data-ttu-id="44028-211">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="44028-211">certificationAuthorityName</span></span>|<span data-ttu-id="44028-212">String</span><span class="sxs-lookup"><span data-stu-id="44028-212">String</span></span>|<span data-ttu-id="44028-213">PKCS 证书颁发机构名称</span><span class="sxs-lookup"><span data-stu-id="44028-213">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="44028-214">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="44028-214">certificateTemplateName</span></span>|<span data-ttu-id="44028-215">String</span><span class="sxs-lookup"><span data-stu-id="44028-215">String</span></span>|<span data-ttu-id="44028-216">PKCS 证书模板名称</span><span class="sxs-lookup"><span data-stu-id="44028-216">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="44028-217">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="44028-217">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="44028-218">String</span><span class="sxs-lookup"><span data-stu-id="44028-218">String</span></span>|<span data-ttu-id="44028-219">定义 AAD 属性的自定义字符串。</span><span class="sxs-lookup"><span data-stu-id="44028-219">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="44028-220">响应</span><span class="sxs-lookup"><span data-stu-id="44028-220">Response</span></span>
<span data-ttu-id="44028-221">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="44028-221">If successful, this method returns a `200 OK` response code and an updated [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44028-222">示例</span><span class="sxs-lookup"><span data-stu-id="44028-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="44028-223">请求</span><span class="sxs-lookup"><span data-stu-id="44028-223">Request</span></span>
<span data-ttu-id="44028-224">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="44028-224">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1738

{
  "@odata.type": "#microsoft.graph.androidForWorkPkcsCertificateProfile",
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
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```

### <a name="response"></a><span data-ttu-id="44028-225">响应</span><span class="sxs-lookup"><span data-stu-id="44028-225">Response</span></span>
<span data-ttu-id="44028-p119">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="44028-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1910

{
  "@odata.type": "#microsoft.graph.androidForWorkPkcsCertificateProfile",
  "id": "0a2d7691-7691-0a2d-9176-2d0a91762d0a",
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
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```






