---
title: 更新 androidWorkProfilePkcsCertificateProfile
description: 更新 androidWorkProfilePkcsCertificateProfile 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 842dc5776622a5a01d933443c9f4d594f743c18f
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51151793"
---
# <a name="update-androidworkprofilepkcscertificateprofile"></a><span data-ttu-id="c4daa-103">更新 androidWorkProfilePkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="c4daa-103">Update androidWorkProfilePkcsCertificateProfile</span></span>

<span data-ttu-id="c4daa-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c4daa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c4daa-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c4daa-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c4daa-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c4daa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c4daa-107">更新 [androidWorkProfilePkcsCertificateProfile 对象](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="c4daa-107">Update the properties of a [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c4daa-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="c4daa-108">Prerequisites</span></span>
<span data-ttu-id="c4daa-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c4daa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4daa-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c4daa-111">Permission type</span></span>|<span data-ttu-id="c4daa-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c4daa-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c4daa-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c4daa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c4daa-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4daa-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c4daa-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c4daa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c4daa-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c4daa-116">Not supported.</span></span>|
|<span data-ttu-id="c4daa-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c4daa-117">Application</span></span>|<span data-ttu-id="c4daa-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4daa-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c4daa-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c4daa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="c4daa-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c4daa-120">Request headers</span></span>
|<span data-ttu-id="c4daa-121">标头</span><span class="sxs-lookup"><span data-stu-id="c4daa-121">Header</span></span>|<span data-ttu-id="c4daa-122">值</span><span class="sxs-lookup"><span data-stu-id="c4daa-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c4daa-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c4daa-123">Authorization</span></span>|<span data-ttu-id="c4daa-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c4daa-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c4daa-125">接受</span><span class="sxs-lookup"><span data-stu-id="c4daa-125">Accept</span></span>|<span data-ttu-id="c4daa-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c4daa-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4daa-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c4daa-127">Request body</span></span>
<span data-ttu-id="c4daa-128">在请求正文中，提供 [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c4daa-128">In the request body, supply a JSON representation for the [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) object.</span></span>

<span data-ttu-id="c4daa-129">下表显示创建 [androidWorkProfilePkcsCertificateProfile 时所需的属性](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md)。</span><span class="sxs-lookup"><span data-stu-id="c4daa-129">The following table shows the properties that are required when you create the [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md).</span></span>

|<span data-ttu-id="c4daa-130">属性</span><span class="sxs-lookup"><span data-stu-id="c4daa-130">Property</span></span>|<span data-ttu-id="c4daa-131">类型</span><span class="sxs-lookup"><span data-stu-id="c4daa-131">Type</span></span>|<span data-ttu-id="c4daa-132">说明</span><span class="sxs-lookup"><span data-stu-id="c4daa-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c4daa-133">id</span><span class="sxs-lookup"><span data-stu-id="c4daa-133">id</span></span>|<span data-ttu-id="c4daa-134">String</span><span class="sxs-lookup"><span data-stu-id="c4daa-134">String</span></span>|<span data-ttu-id="c4daa-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c4daa-135">Key of the entity.</span></span> <span data-ttu-id="c4daa-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c4daa-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4daa-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c4daa-137">lastModifiedDateTime</span></span>|<span data-ttu-id="c4daa-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c4daa-138">DateTimeOffset</span></span>|<span data-ttu-id="c4daa-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c4daa-139">DateTime the object was last modified.</span></span> <span data-ttu-id="c4daa-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c4daa-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4daa-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c4daa-141">roleScopeTagIds</span></span>|<span data-ttu-id="c4daa-142">String collection</span><span class="sxs-lookup"><span data-stu-id="c4daa-142">String collection</span></span>|<span data-ttu-id="c4daa-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="c4daa-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c4daa-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c4daa-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4daa-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c4daa-145">supportsScopeTags</span></span>|<span data-ttu-id="c4daa-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="c4daa-146">Boolean</span></span>|<span data-ttu-id="c4daa-147">指示基础设备配置是否支持分配范围标记。</span><span class="sxs-lookup"><span data-stu-id="c4daa-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c4daa-148">当此值为 false 且实体对作用域用户不可见时，不允许分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="c4daa-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c4daa-149">这适用于在 Silverlight 中创建的旧版策略，可通过在 Azure 门户中删除和重新创建策略来解决。</span><span class="sxs-lookup"><span data-stu-id="c4daa-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c4daa-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c4daa-150">This property is read-only.</span></span> <span data-ttu-id="c4daa-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c4daa-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4daa-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c4daa-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="c4daa-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c4daa-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="c4daa-154">此策略的操作系统版本适用性。</span><span class="sxs-lookup"><span data-stu-id="c4daa-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="c4daa-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c4daa-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4daa-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c4daa-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="c4daa-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c4daa-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="c4daa-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="c4daa-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="c4daa-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c4daa-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4daa-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c4daa-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="c4daa-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c4daa-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="c4daa-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="c4daa-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="c4daa-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c4daa-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4daa-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c4daa-164">createdDateTime</span></span>|<span data-ttu-id="c4daa-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c4daa-165">DateTimeOffset</span></span>|<span data-ttu-id="c4daa-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c4daa-166">DateTime the object was created.</span></span> <span data-ttu-id="c4daa-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c4daa-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4daa-168">说明</span><span class="sxs-lookup"><span data-stu-id="c4daa-168">description</span></span>|<span data-ttu-id="c4daa-169">String</span><span class="sxs-lookup"><span data-stu-id="c4daa-169">String</span></span>|<span data-ttu-id="c4daa-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="c4daa-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c4daa-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c4daa-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4daa-172">displayName</span><span class="sxs-lookup"><span data-stu-id="c4daa-172">displayName</span></span>|<span data-ttu-id="c4daa-173">String</span><span class="sxs-lookup"><span data-stu-id="c4daa-173">String</span></span>|<span data-ttu-id="c4daa-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="c4daa-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c4daa-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c4daa-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4daa-176">version</span><span class="sxs-lookup"><span data-stu-id="c4daa-176">version</span></span>|<span data-ttu-id="c4daa-177">Int32</span><span class="sxs-lookup"><span data-stu-id="c4daa-177">Int32</span></span>|<span data-ttu-id="c4daa-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="c4daa-178">Version of the device configuration.</span></span> <span data-ttu-id="c4daa-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c4daa-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4daa-180">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="c4daa-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="c4daa-181">Int32</span><span class="sxs-lookup"><span data-stu-id="c4daa-181">Int32</span></span>|<span data-ttu-id="c4daa-182">证书续订阈值百分比。</span><span class="sxs-lookup"><span data-stu-id="c4daa-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="c4daa-183">有效值 1 到 99 继承自 [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="c4daa-183">Valid values 1 to 99 Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="c4daa-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="c4daa-184">subjectNameFormat</span></span>|[<span data-ttu-id="c4daa-185">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="c4daa-185">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="c4daa-186">证书主题名称格式。</span><span class="sxs-lookup"><span data-stu-id="c4daa-186">Certificate Subject Name Format.</span></span> <span data-ttu-id="c4daa-187">继承自 [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="c4daa-187">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="c4daa-188">可取值为：`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId`。</span><span class="sxs-lookup"><span data-stu-id="c4daa-188">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="c4daa-189">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="c4daa-189">certificateValidityPeriodValue</span></span>|<span data-ttu-id="c4daa-190">Int32</span><span class="sxs-lookup"><span data-stu-id="c4daa-190">Int32</span></span>|<span data-ttu-id="c4daa-191">证书有效期的值。</span><span class="sxs-lookup"><span data-stu-id="c4daa-191">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="c4daa-192">继承自 [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="c4daa-192">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="c4daa-193">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="c4daa-193">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="c4daa-194">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="c4daa-194">certificateValidityPeriodScale</span></span>](../resources/intune-shared-certificatevalidityperiodscale.md)|<span data-ttu-id="c4daa-195">证书有效期的缩放。</span><span class="sxs-lookup"><span data-stu-id="c4daa-195">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="c4daa-196">继承自 [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="c4daa-196">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="c4daa-197">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="c4daa-197">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="c4daa-198">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="c4daa-198">extendedKeyUsages</span></span>|<span data-ttu-id="c4daa-199">[extendedKeyUsage](../resources/intune-shared-extendedkeyusage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c4daa-199">[extendedKeyUsage](../resources/intune-shared-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="c4daa-200">EKU (扩展密钥) 设置。</span><span class="sxs-lookup"><span data-stu-id="c4daa-200">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="c4daa-201">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="c4daa-201">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="c4daa-202">继承自 [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="c4daa-202">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="c4daa-203">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="c4daa-203">subjectAlternativeNameType</span></span>|[<span data-ttu-id="c4daa-204">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="c4daa-204">subjectAlternativeNameType</span></span>](../resources/intune-shared-subjectalternativenametype.md)|<span data-ttu-id="c4daa-205">证书主题备用名称类型。</span><span class="sxs-lookup"><span data-stu-id="c4daa-205">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="c4daa-206">继承自 [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="c4daa-206">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="c4daa-207">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService`、`universalResourceIdentifier`。</span><span class="sxs-lookup"><span data-stu-id="c4daa-207">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span></span>|
|<span data-ttu-id="c4daa-208">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="c4daa-208">certificationAuthority</span></span>|<span data-ttu-id="c4daa-209">String</span><span class="sxs-lookup"><span data-stu-id="c4daa-209">String</span></span>|<span data-ttu-id="c4daa-210">PKCS 证书颁发机构</span><span class="sxs-lookup"><span data-stu-id="c4daa-210">PKCS Certification Authority</span></span>|
|<span data-ttu-id="c4daa-211">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="c4daa-211">certificationAuthorityName</span></span>|<span data-ttu-id="c4daa-212">String</span><span class="sxs-lookup"><span data-stu-id="c4daa-212">String</span></span>|<span data-ttu-id="c4daa-213">PKCS 证书颁发机构名称</span><span class="sxs-lookup"><span data-stu-id="c4daa-213">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="c4daa-214">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="c4daa-214">certificateTemplateName</span></span>|<span data-ttu-id="c4daa-215">String</span><span class="sxs-lookup"><span data-stu-id="c4daa-215">String</span></span>|<span data-ttu-id="c4daa-216">PKCS 证书模板名称</span><span class="sxs-lookup"><span data-stu-id="c4daa-216">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="c4daa-217">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="c4daa-217">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="c4daa-218">String</span><span class="sxs-lookup"><span data-stu-id="c4daa-218">String</span></span>|<span data-ttu-id="c4daa-219">定义 AAD 属性的自定义字符串。</span><span class="sxs-lookup"><span data-stu-id="c4daa-219">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="c4daa-220">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="c4daa-220">subjectNameFormatString</span></span>|<span data-ttu-id="c4daa-221">String</span><span class="sxs-lookup"><span data-stu-id="c4daa-221">String</span></span>|<span data-ttu-id="c4daa-222">要与 SubjectNameFormat 一同使用的自定义格式 = Custom。</span><span class="sxs-lookup"><span data-stu-id="c4daa-222">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="c4daa-223">示例：CN={{EmailAddress}}，E={{EmailAddress}，OU=Enterprise Users，O=Contoso Corporation，L=Redmond，ST=WA，C=US</span><span class="sxs-lookup"><span data-stu-id="c4daa-223">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="c4daa-224">certificateStore</span><span class="sxs-lookup"><span data-stu-id="c4daa-224">certificateStore</span></span>|[<span data-ttu-id="c4daa-225">certificateStore</span><span class="sxs-lookup"><span data-stu-id="c4daa-225">certificateStore</span></span>](../resources/intune-shared-certificatestore.md)|<span data-ttu-id="c4daa-226">目标存储证书。</span><span class="sxs-lookup"><span data-stu-id="c4daa-226">Target store certificate.</span></span> <span data-ttu-id="c4daa-227">可取值为：`user`、`machine`。</span><span class="sxs-lookup"><span data-stu-id="c4daa-227">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="c4daa-228">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="c4daa-228">customSubjectAlternativeNames</span></span>|<span data-ttu-id="c4daa-229">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c4daa-229">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="c4daa-230">自定义主题备用名称设置。</span><span class="sxs-lookup"><span data-stu-id="c4daa-230">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="c4daa-231">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="c4daa-231">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="c4daa-232">响应</span><span class="sxs-lookup"><span data-stu-id="c4daa-232">Response</span></span>
<span data-ttu-id="c4daa-233">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c4daa-233">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4daa-234">示例</span><span class="sxs-lookup"><span data-stu-id="c4daa-234">Example</span></span>

### <a name="request"></a><span data-ttu-id="c4daa-235">请求</span><span class="sxs-lookup"><span data-stu-id="c4daa-235">Request</span></span>
<span data-ttu-id="c4daa-236">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c4daa-236">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="c4daa-237">响应</span><span class="sxs-lookup"><span data-stu-id="c4daa-237">Response</span></span>
<span data-ttu-id="c4daa-p122">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c4daa-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




