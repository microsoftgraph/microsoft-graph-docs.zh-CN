---
title: 更新 androidDeviceOwnerImportedPFXCertificateProfile
description: 更新 androidDeviceOwnerImportedPFXCertificateProfile 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c7e152720c1de2259d923999c9ae8477c0df4123
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51138555"
---
# <a name="update-androiddeviceownerimportedpfxcertificateprofile"></a><span data-ttu-id="9c8ac-103">更新 androidDeviceOwnerImportedPFXCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="9c8ac-103">Update androidDeviceOwnerImportedPFXCertificateProfile</span></span>

<span data-ttu-id="9c8ac-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c8ac-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9c8ac-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9c8ac-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9c8ac-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9c8ac-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9c8ac-107">更新 [androidDeviceOwnerImportedPFXCertificateProfile 对象](../resources/intune-deviceconfig-androiddeviceownerimportedpfxcertificateprofile.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="9c8ac-107">Update the properties of a [androidDeviceOwnerImportedPFXCertificateProfile](../resources/intune-deviceconfig-androiddeviceownerimportedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9c8ac-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="9c8ac-108">Prerequisites</span></span>
<span data-ttu-id="9c8ac-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9c8ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c8ac-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9c8ac-111">Permission type</span></span>|<span data-ttu-id="9c8ac-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9c8ac-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9c8ac-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9c8ac-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9c8ac-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c8ac-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9c8ac-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9c8ac-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9c8ac-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9c8ac-116">Not supported.</span></span>|
|<span data-ttu-id="9c8ac-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9c8ac-117">Application</span></span>|<span data-ttu-id="9c8ac-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c8ac-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9c8ac-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9c8ac-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="9c8ac-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9c8ac-120">Request headers</span></span>
|<span data-ttu-id="9c8ac-121">标头</span><span class="sxs-lookup"><span data-stu-id="9c8ac-121">Header</span></span>|<span data-ttu-id="9c8ac-122">值</span><span class="sxs-lookup"><span data-stu-id="9c8ac-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9c8ac-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9c8ac-123">Authorization</span></span>|<span data-ttu-id="9c8ac-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9c8ac-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9c8ac-125">接受</span><span class="sxs-lookup"><span data-stu-id="9c8ac-125">Accept</span></span>|<span data-ttu-id="9c8ac-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9c8ac-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9c8ac-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9c8ac-127">Request body</span></span>
<span data-ttu-id="9c8ac-128">在请求正文中，提供 [androidDeviceOwnerImportedPFXCertificateProfile](../resources/intune-deviceconfig-androiddeviceownerimportedpfxcertificateprofile.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9c8ac-128">In the request body, supply a JSON representation for the [androidDeviceOwnerImportedPFXCertificateProfile](../resources/intune-deviceconfig-androiddeviceownerimportedpfxcertificateprofile.md) object.</span></span>

<span data-ttu-id="9c8ac-129">下表显示创建 [androidDeviceOwnerImportedPFXCertificateProfile 时所需的属性](../resources/intune-deviceconfig-androiddeviceownerimportedpfxcertificateprofile.md)。</span><span class="sxs-lookup"><span data-stu-id="9c8ac-129">The following table shows the properties that are required when you create the [androidDeviceOwnerImportedPFXCertificateProfile](../resources/intune-deviceconfig-androiddeviceownerimportedpfxcertificateprofile.md).</span></span>

|<span data-ttu-id="9c8ac-130">属性</span><span class="sxs-lookup"><span data-stu-id="9c8ac-130">Property</span></span>|<span data-ttu-id="9c8ac-131">类型</span><span class="sxs-lookup"><span data-stu-id="9c8ac-131">Type</span></span>|<span data-ttu-id="9c8ac-132">说明</span><span class="sxs-lookup"><span data-stu-id="9c8ac-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c8ac-133">id</span><span class="sxs-lookup"><span data-stu-id="9c8ac-133">id</span></span>|<span data-ttu-id="9c8ac-134">String</span><span class="sxs-lookup"><span data-stu-id="9c8ac-134">String</span></span>|<span data-ttu-id="9c8ac-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="9c8ac-135">Key of the entity.</span></span> <span data-ttu-id="9c8ac-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9c8ac-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9c8ac-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9c8ac-137">lastModifiedDateTime</span></span>|<span data-ttu-id="9c8ac-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9c8ac-138">DateTimeOffset</span></span>|<span data-ttu-id="9c8ac-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="9c8ac-139">DateTime the object was last modified.</span></span> <span data-ttu-id="9c8ac-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9c8ac-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9c8ac-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9c8ac-141">roleScopeTagIds</span></span>|<span data-ttu-id="9c8ac-142">String collection</span><span class="sxs-lookup"><span data-stu-id="9c8ac-142">String collection</span></span>|<span data-ttu-id="9c8ac-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="9c8ac-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9c8ac-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9c8ac-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9c8ac-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="9c8ac-145">supportsScopeTags</span></span>|<span data-ttu-id="9c8ac-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="9c8ac-146">Boolean</span></span>|<span data-ttu-id="9c8ac-147">指示基础设备配置是否支持分配范围标记。</span><span class="sxs-lookup"><span data-stu-id="9c8ac-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="9c8ac-148">当此值为 false 且实体对作用域用户不可见时，不允许分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="9c8ac-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="9c8ac-149">这适用于在 Silverlight 中创建的旧版策略，可通过在 Azure 门户中删除和重新创建策略来解决。</span><span class="sxs-lookup"><span data-stu-id="9c8ac-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="9c8ac-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9c8ac-150">This property is read-only.</span></span> <span data-ttu-id="9c8ac-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9c8ac-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9c8ac-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="9c8ac-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="9c8ac-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="9c8ac-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="9c8ac-154">此策略的操作系统版本适用性。</span><span class="sxs-lookup"><span data-stu-id="9c8ac-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="9c8ac-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9c8ac-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9c8ac-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="9c8ac-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="9c8ac-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="9c8ac-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="9c8ac-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="9c8ac-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="9c8ac-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9c8ac-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9c8ac-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="9c8ac-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="9c8ac-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="9c8ac-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="9c8ac-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="9c8ac-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="9c8ac-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9c8ac-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9c8ac-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9c8ac-164">createdDateTime</span></span>|<span data-ttu-id="9c8ac-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9c8ac-165">DateTimeOffset</span></span>|<span data-ttu-id="9c8ac-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="9c8ac-166">DateTime the object was created.</span></span> <span data-ttu-id="9c8ac-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9c8ac-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9c8ac-168">说明</span><span class="sxs-lookup"><span data-stu-id="9c8ac-168">description</span></span>|<span data-ttu-id="9c8ac-169">String</span><span class="sxs-lookup"><span data-stu-id="9c8ac-169">String</span></span>|<span data-ttu-id="9c8ac-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="9c8ac-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9c8ac-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9c8ac-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9c8ac-172">displayName</span><span class="sxs-lookup"><span data-stu-id="9c8ac-172">displayName</span></span>|<span data-ttu-id="9c8ac-173">String</span><span class="sxs-lookup"><span data-stu-id="9c8ac-173">String</span></span>|<span data-ttu-id="9c8ac-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="9c8ac-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9c8ac-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9c8ac-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9c8ac-176">version</span><span class="sxs-lookup"><span data-stu-id="9c8ac-176">version</span></span>|<span data-ttu-id="9c8ac-177">Int32</span><span class="sxs-lookup"><span data-stu-id="9c8ac-177">Int32</span></span>|<span data-ttu-id="9c8ac-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="9c8ac-178">Version of the device configuration.</span></span> <span data-ttu-id="9c8ac-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9c8ac-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9c8ac-180">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="9c8ac-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="9c8ac-181">Int32</span><span class="sxs-lookup"><span data-stu-id="9c8ac-181">Int32</span></span>|<span data-ttu-id="9c8ac-182">证书续订阈值百分比。</span><span class="sxs-lookup"><span data-stu-id="9c8ac-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="9c8ac-183">有效值 1 到 99 继承自 [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="9c8ac-183">Valid values 1 to 99 Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span></span>|
|<span data-ttu-id="9c8ac-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="9c8ac-184">subjectNameFormat</span></span>|[<span data-ttu-id="9c8ac-185">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="9c8ac-185">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="9c8ac-186">证书主题名称格式。</span><span class="sxs-lookup"><span data-stu-id="9c8ac-186">Certificate Subject Name Format.</span></span> <span data-ttu-id="9c8ac-187">继承自 [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="9c8ac-187">Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span></span> <span data-ttu-id="9c8ac-188">可取值为：`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId`。</span><span class="sxs-lookup"><span data-stu-id="9c8ac-188">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="9c8ac-189">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="9c8ac-189">certificateValidityPeriodValue</span></span>|<span data-ttu-id="9c8ac-190">Int32</span><span class="sxs-lookup"><span data-stu-id="9c8ac-190">Int32</span></span>|<span data-ttu-id="9c8ac-191">证书有效期的值。</span><span class="sxs-lookup"><span data-stu-id="9c8ac-191">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="9c8ac-192">继承自 [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="9c8ac-192">Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span></span>|
|<span data-ttu-id="9c8ac-193">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="9c8ac-193">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="9c8ac-194">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="9c8ac-194">certificateValidityPeriodScale</span></span>](../resources/intune-shared-certificatevalidityperiodscale.md)|<span data-ttu-id="9c8ac-195">证书有效期的缩放。</span><span class="sxs-lookup"><span data-stu-id="9c8ac-195">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="9c8ac-196">继承自 [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="9c8ac-196">Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span></span> <span data-ttu-id="9c8ac-197">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="9c8ac-197">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="9c8ac-198">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="9c8ac-198">extendedKeyUsages</span></span>|<span data-ttu-id="9c8ac-199">[extendedKeyUsage](../resources/intune-shared-extendedkeyusage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9c8ac-199">[extendedKeyUsage](../resources/intune-shared-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="9c8ac-200">EKU (扩展密钥) 设置。</span><span class="sxs-lookup"><span data-stu-id="9c8ac-200">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="9c8ac-201">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="9c8ac-201">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="9c8ac-202">继承自 [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="9c8ac-202">Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span></span>|
|<span data-ttu-id="9c8ac-203">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="9c8ac-203">subjectAlternativeNameType</span></span>|[<span data-ttu-id="9c8ac-204">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="9c8ac-204">subjectAlternativeNameType</span></span>](../resources/intune-shared-subjectalternativenametype.md)|<span data-ttu-id="9c8ac-205">证书主题备用名称类型。</span><span class="sxs-lookup"><span data-stu-id="9c8ac-205">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="9c8ac-206">继承自 [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="9c8ac-206">Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span></span> <span data-ttu-id="9c8ac-207">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService`、`universalResourceIdentifier`。</span><span class="sxs-lookup"><span data-stu-id="9c8ac-207">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span></span>|
|<span data-ttu-id="9c8ac-208">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="9c8ac-208">intendedPurpose</span></span>|[<span data-ttu-id="9c8ac-209">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="9c8ac-209">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="9c8ac-210">证书配置文件的预定用途 - 可以是未分配、SmimeEncryption、SmimeSigning 等。可能的值是 `unassigned` `smimeEncryption` `smimeSigning` ：、、、、。 `vpn` `wifi`</span><span class="sxs-lookup"><span data-stu-id="9c8ac-210">Intended Purpose of the Certificate Profile - which could be Unassigned, SmimeEncryption, SmimeSigning etc. Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="9c8ac-211">响应</span><span class="sxs-lookup"><span data-stu-id="9c8ac-211">Response</span></span>
<span data-ttu-id="9c8ac-212">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [androidDeviceOwnerImportedPFXCertificateProfile](../resources/intune-deviceconfig-androiddeviceownerimportedpfxcertificateprofile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9c8ac-212">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerImportedPFXCertificateProfile](../resources/intune-deviceconfig-androiddeviceownerimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9c8ac-213">示例</span><span class="sxs-lookup"><span data-stu-id="9c8ac-213">Example</span></span>

### <a name="request"></a><span data-ttu-id="9c8ac-214">请求</span><span class="sxs-lookup"><span data-stu-id="9c8ac-214">Request</span></span>
<span data-ttu-id="9c8ac-215">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9c8ac-215">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1503

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerImportedPFXCertificateProfile",
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
  "intendedPurpose": "smimeEncryption"
}
```

### <a name="response"></a><span data-ttu-id="9c8ac-216">响应</span><span class="sxs-lookup"><span data-stu-id="9c8ac-216">Response</span></span>
<span data-ttu-id="9c8ac-p119">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9c8ac-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1675

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerImportedPFXCertificateProfile",
  "id": "8d46d3c7-d3c7-8d46-c7d3-468dc7d3468d",
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
  "intendedPurpose": "smimeEncryption"
}
```




