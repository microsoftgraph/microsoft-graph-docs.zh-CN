---
title: 创建 androidDeviceOwnerImportedPFXCertificateProfile
description: 创建新的 androidDeviceOwnerImportedPFXCertificateProfile 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 29de44f7d88b01c9b0453dd5b318b98dc9546c59
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49240829"
---
# <a name="create-androiddeviceownerimportedpfxcertificateprofile"></a><span data-ttu-id="0f58d-103">创建 androidDeviceOwnerImportedPFXCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="0f58d-103">Create androidDeviceOwnerImportedPFXCertificateProfile</span></span>

<span data-ttu-id="0f58d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f58d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0f58d-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0f58d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0f58d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0f58d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f58d-107">创建新的 [androidDeviceOwnerImportedPFXCertificateProfile](../resources/intune-deviceconfig-androiddeviceownerimportedpfxcertificateprofile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0f58d-107">Create a new [androidDeviceOwnerImportedPFXCertificateProfile](../resources/intune-deviceconfig-androiddeviceownerimportedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0f58d-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="0f58d-108">Prerequisites</span></span>
<span data-ttu-id="0f58d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0f58d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0f58d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="0f58d-111">Permission type</span></span>|<span data-ttu-id="0f58d-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0f58d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0f58d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0f58d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0f58d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f58d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0f58d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0f58d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0f58d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0f58d-116">Not supported.</span></span>|
|<span data-ttu-id="0f58d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="0f58d-117">Application</span></span>|<span data-ttu-id="0f58d-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f58d-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0f58d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0f58d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="0f58d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="0f58d-120">Request headers</span></span>
|<span data-ttu-id="0f58d-121">标头</span><span class="sxs-lookup"><span data-stu-id="0f58d-121">Header</span></span>|<span data-ttu-id="0f58d-122">值</span><span class="sxs-lookup"><span data-stu-id="0f58d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0f58d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0f58d-123">Authorization</span></span>|<span data-ttu-id="0f58d-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0f58d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0f58d-125">接受</span><span class="sxs-lookup"><span data-stu-id="0f58d-125">Accept</span></span>|<span data-ttu-id="0f58d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0f58d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0f58d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0f58d-127">Request body</span></span>
<span data-ttu-id="0f58d-128">在请求正文中，提供 androidDeviceOwnerImportedPFXCertificateProfile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0f58d-128">In the request body, supply a JSON representation for the androidDeviceOwnerImportedPFXCertificateProfile object.</span></span>

<span data-ttu-id="0f58d-129">下表显示创建 androidDeviceOwnerImportedPFXCertificateProfile 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="0f58d-129">The following table shows the properties that are required when you create the androidDeviceOwnerImportedPFXCertificateProfile.</span></span>

|<span data-ttu-id="0f58d-130">属性</span><span class="sxs-lookup"><span data-stu-id="0f58d-130">Property</span></span>|<span data-ttu-id="0f58d-131">类型</span><span class="sxs-lookup"><span data-stu-id="0f58d-131">Type</span></span>|<span data-ttu-id="0f58d-132">说明</span><span class="sxs-lookup"><span data-stu-id="0f58d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f58d-133">id</span><span class="sxs-lookup"><span data-stu-id="0f58d-133">id</span></span>|<span data-ttu-id="0f58d-134">String</span><span class="sxs-lookup"><span data-stu-id="0f58d-134">String</span></span>|<span data-ttu-id="0f58d-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="0f58d-135">Key of the entity.</span></span> <span data-ttu-id="0f58d-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0f58d-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0f58d-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0f58d-137">lastModifiedDateTime</span></span>|<span data-ttu-id="0f58d-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f58d-138">DateTimeOffset</span></span>|<span data-ttu-id="0f58d-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="0f58d-139">DateTime the object was last modified.</span></span> <span data-ttu-id="0f58d-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0f58d-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0f58d-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0f58d-141">roleScopeTagIds</span></span>|<span data-ttu-id="0f58d-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="0f58d-142">String collection</span></span>|<span data-ttu-id="0f58d-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="0f58d-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0f58d-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0f58d-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0f58d-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="0f58d-145">supportsScopeTags</span></span>|<span data-ttu-id="0f58d-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="0f58d-146">Boolean</span></span>|<span data-ttu-id="0f58d-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="0f58d-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="0f58d-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="0f58d-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="0f58d-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="0f58d-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="0f58d-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="0f58d-150">This property is read-only.</span></span> <span data-ttu-id="0f58d-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0f58d-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0f58d-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="0f58d-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="0f58d-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="0f58d-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="0f58d-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="0f58d-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="0f58d-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0f58d-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0f58d-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="0f58d-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="0f58d-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="0f58d-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="0f58d-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="0f58d-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="0f58d-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0f58d-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0f58d-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="0f58d-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="0f58d-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="0f58d-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="0f58d-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="0f58d-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="0f58d-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0f58d-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0f58d-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0f58d-164">createdDateTime</span></span>|<span data-ttu-id="0f58d-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f58d-165">DateTimeOffset</span></span>|<span data-ttu-id="0f58d-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="0f58d-166">DateTime the object was created.</span></span> <span data-ttu-id="0f58d-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0f58d-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0f58d-168">description</span><span class="sxs-lookup"><span data-stu-id="0f58d-168">description</span></span>|<span data-ttu-id="0f58d-169">String</span><span class="sxs-lookup"><span data-stu-id="0f58d-169">String</span></span>|<span data-ttu-id="0f58d-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="0f58d-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0f58d-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0f58d-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0f58d-172">displayName</span><span class="sxs-lookup"><span data-stu-id="0f58d-172">displayName</span></span>|<span data-ttu-id="0f58d-173">String</span><span class="sxs-lookup"><span data-stu-id="0f58d-173">String</span></span>|<span data-ttu-id="0f58d-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="0f58d-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0f58d-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0f58d-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0f58d-176">version</span><span class="sxs-lookup"><span data-stu-id="0f58d-176">version</span></span>|<span data-ttu-id="0f58d-177">Int32</span><span class="sxs-lookup"><span data-stu-id="0f58d-177">Int32</span></span>|<span data-ttu-id="0f58d-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="0f58d-178">Version of the device configuration.</span></span> <span data-ttu-id="0f58d-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0f58d-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0f58d-180">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="0f58d-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="0f58d-181">Int32</span><span class="sxs-lookup"><span data-stu-id="0f58d-181">Int32</span></span>|<span data-ttu-id="0f58d-182">证书续订阈值百分比。</span><span class="sxs-lookup"><span data-stu-id="0f58d-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="0f58d-183">从[AndroidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)继承的有效值1到99</span><span class="sxs-lookup"><span data-stu-id="0f58d-183">Valid values 1 to 99 Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span></span>|
|<span data-ttu-id="0f58d-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="0f58d-184">subjectNameFormat</span></span>|[<span data-ttu-id="0f58d-185">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="0f58d-185">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="0f58d-186">证书使用者名称格式。</span><span class="sxs-lookup"><span data-stu-id="0f58d-186">Certificate Subject Name Format.</span></span> <span data-ttu-id="0f58d-187">继承自 [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="0f58d-187">Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span></span> <span data-ttu-id="0f58d-188">可取值为：`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId`。</span><span class="sxs-lookup"><span data-stu-id="0f58d-188">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="0f58d-189">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="0f58d-189">certificateValidityPeriodValue</span></span>|<span data-ttu-id="0f58d-190">Int32</span><span class="sxs-lookup"><span data-stu-id="0f58d-190">Int32</span></span>|<span data-ttu-id="0f58d-191">证书有效期限的值。</span><span class="sxs-lookup"><span data-stu-id="0f58d-191">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="0f58d-192">继承自 [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="0f58d-192">Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span></span>|
|<span data-ttu-id="0f58d-193">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="0f58d-193">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="0f58d-194">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="0f58d-194">certificateValidityPeriodScale</span></span>](../resources/intune-shared-certificatevalidityperiodscale.md)|<span data-ttu-id="0f58d-195">证书有效期的小数位数。</span><span class="sxs-lookup"><span data-stu-id="0f58d-195">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="0f58d-196">继承自 [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="0f58d-196">Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span></span> <span data-ttu-id="0f58d-197">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="0f58d-197">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="0f58d-198">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="0f58d-198">extendedKeyUsages</span></span>|<span data-ttu-id="0f58d-199">[extendedKeyUsage](../resources/intune-shared-extendedkeyusage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0f58d-199">[extendedKeyUsage](../resources/intune-shared-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="0f58d-200"> (EKU) 设置的扩展密钥用法。</span><span class="sxs-lookup"><span data-stu-id="0f58d-200">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="0f58d-201">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="0f58d-201">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="0f58d-202">继承自 [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="0f58d-202">Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span></span>|
|<span data-ttu-id="0f58d-203">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="0f58d-203">subjectAlternativeNameType</span></span>|[<span data-ttu-id="0f58d-204">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="0f58d-204">subjectAlternativeNameType</span></span>](../resources/intune-shared-subjectalternativenametype.md)|<span data-ttu-id="0f58d-205">证书使用者备用名称类型。</span><span class="sxs-lookup"><span data-stu-id="0f58d-205">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="0f58d-206">继承自 [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="0f58d-206">Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span></span> <span data-ttu-id="0f58d-207">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService`、`universalResourceIdentifier`。</span><span class="sxs-lookup"><span data-stu-id="0f58d-207">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span></span>|
|<span data-ttu-id="0f58d-208">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="0f58d-208">intendedPurpose</span></span>|[<span data-ttu-id="0f58d-209">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="0f58d-209">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="0f58d-210">证书配置文件的预期用途-可以为未分配、SmimeEncryption、SmimeSigning 等。可能的值为： `unassigned` 、 `smimeEncryption` 、、 `smimeSigning` `vpn` 、 `wifi` 。</span><span class="sxs-lookup"><span data-stu-id="0f58d-210">Intended Purpose of the Certificate Profile - which could be Unassigned, SmimeEncryption, SmimeSigning etc. Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="0f58d-211">响应</span><span class="sxs-lookup"><span data-stu-id="0f58d-211">Response</span></span>
<span data-ttu-id="0f58d-212">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [androidDeviceOwnerImportedPFXCertificateProfile](../resources/intune-deviceconfig-androiddeviceownerimportedpfxcertificateprofile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0f58d-212">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerImportedPFXCertificateProfile](../resources/intune-deviceconfig-androiddeviceownerimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f58d-213">示例</span><span class="sxs-lookup"><span data-stu-id="0f58d-213">Example</span></span>

### <a name="request"></a><span data-ttu-id="0f58d-214">请求</span><span class="sxs-lookup"><span data-stu-id="0f58d-214">Request</span></span>
<span data-ttu-id="0f58d-215">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0f58d-215">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="0f58d-216">响应</span><span class="sxs-lookup"><span data-stu-id="0f58d-216">Response</span></span>
<span data-ttu-id="0f58d-p119">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0f58d-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




