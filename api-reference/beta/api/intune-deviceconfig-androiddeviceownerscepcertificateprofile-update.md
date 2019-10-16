---
title: 更新 androidDeviceOwnerScepCertificateProfile
description: 更新 androidDeviceOwnerScepCertificateProfile 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cbbabde2ba07cb1810acb410ec87a956571e1610
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37534769"
---
# <a name="update-androiddeviceownerscepcertificateprofile"></a><span data-ttu-id="077e3-103">更新 androidDeviceOwnerScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="077e3-103">Update androidDeviceOwnerScepCertificateProfile</span></span>

> <span data-ttu-id="077e3-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="077e3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="077e3-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="077e3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="077e3-106">更新[androidDeviceOwnerScepCertificateProfile](../resources/intune-deviceconfig-androiddeviceownerscepcertificateprofile.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="077e3-106">Update the properties of a [androidDeviceOwnerScepCertificateProfile](../resources/intune-deviceconfig-androiddeviceownerscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="077e3-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="077e3-107">Prerequisites</span></span>
<span data-ttu-id="077e3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="077e3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="077e3-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="077e3-110">Permission type</span></span>|<span data-ttu-id="077e3-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="077e3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="077e3-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="077e3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="077e3-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="077e3-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="077e3-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="077e3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="077e3-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="077e3-115">Not supported.</span></span>|
|<span data-ttu-id="077e3-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="077e3-116">Application</span></span>|<span data-ttu-id="077e3-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="077e3-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="077e3-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="077e3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="077e3-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="077e3-119">Request headers</span></span>
|<span data-ttu-id="077e3-120">标头</span><span class="sxs-lookup"><span data-stu-id="077e3-120">Header</span></span>|<span data-ttu-id="077e3-121">值</span><span class="sxs-lookup"><span data-stu-id="077e3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="077e3-122">授权</span><span class="sxs-lookup"><span data-stu-id="077e3-122">Authorization</span></span>|<span data-ttu-id="077e3-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="077e3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="077e3-124">接受</span><span class="sxs-lookup"><span data-stu-id="077e3-124">Accept</span></span>|<span data-ttu-id="077e3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="077e3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="077e3-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="077e3-126">Request body</span></span>
<span data-ttu-id="077e3-127">在请求正文中，提供[androidDeviceOwnerScepCertificateProfile](../resources/intune-deviceconfig-androiddeviceownerscepcertificateprofile.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="077e3-127">In the request body, supply a JSON representation for the [androidDeviceOwnerScepCertificateProfile](../resources/intune-deviceconfig-androiddeviceownerscepcertificateprofile.md) object.</span></span>

<span data-ttu-id="077e3-128">下表显示创建[androidDeviceOwnerScepCertificateProfile](../resources/intune-deviceconfig-androiddeviceownerscepcertificateprofile.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="077e3-128">The following table shows the properties that are required when you create the [androidDeviceOwnerScepCertificateProfile](../resources/intune-deviceconfig-androiddeviceownerscepcertificateprofile.md).</span></span>

|<span data-ttu-id="077e3-129">属性</span><span class="sxs-lookup"><span data-stu-id="077e3-129">Property</span></span>|<span data-ttu-id="077e3-130">类型</span><span class="sxs-lookup"><span data-stu-id="077e3-130">Type</span></span>|<span data-ttu-id="077e3-131">说明</span><span class="sxs-lookup"><span data-stu-id="077e3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="077e3-132">id</span><span class="sxs-lookup"><span data-stu-id="077e3-132">id</span></span>|<span data-ttu-id="077e3-133">字符串</span><span class="sxs-lookup"><span data-stu-id="077e3-133">String</span></span>|<span data-ttu-id="077e3-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="077e3-134">Key of the entity.</span></span> <span data-ttu-id="077e3-135">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="077e3-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="077e3-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="077e3-136">lastModifiedDateTime</span></span>|<span data-ttu-id="077e3-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="077e3-137">DateTimeOffset</span></span>|<span data-ttu-id="077e3-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="077e3-138">DateTime the object was last modified.</span></span> <span data-ttu-id="077e3-139">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="077e3-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="077e3-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="077e3-140">roleScopeTagIds</span></span>|<span data-ttu-id="077e3-141">String 集合</span><span class="sxs-lookup"><span data-stu-id="077e3-141">String collection</span></span>|<span data-ttu-id="077e3-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="077e3-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="077e3-143">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="077e3-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="077e3-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="077e3-144">supportsScopeTags</span></span>|<span data-ttu-id="077e3-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="077e3-145">Boolean</span></span>|<span data-ttu-id="077e3-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="077e3-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="077e3-147">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="077e3-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="077e3-148">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="077e3-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="077e3-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="077e3-149">This property is read-only.</span></span> <span data-ttu-id="077e3-150">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="077e3-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="077e3-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="077e3-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="077e3-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="077e3-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="077e3-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="077e3-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="077e3-154">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="077e3-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="077e3-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="077e3-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="077e3-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="077e3-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="077e3-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="077e3-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="077e3-158">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="077e3-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="077e3-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="077e3-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="077e3-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="077e3-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="077e3-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="077e3-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="077e3-162">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="077e3-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="077e3-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="077e3-163">createdDateTime</span></span>|<span data-ttu-id="077e3-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="077e3-164">DateTimeOffset</span></span>|<span data-ttu-id="077e3-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="077e3-165">DateTime the object was created.</span></span> <span data-ttu-id="077e3-166">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="077e3-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="077e3-167">说明</span><span class="sxs-lookup"><span data-stu-id="077e3-167">description</span></span>|<span data-ttu-id="077e3-168">String</span><span class="sxs-lookup"><span data-stu-id="077e3-168">String</span></span>|<span data-ttu-id="077e3-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="077e3-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="077e3-170">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="077e3-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="077e3-171">displayName</span><span class="sxs-lookup"><span data-stu-id="077e3-171">displayName</span></span>|<span data-ttu-id="077e3-172">String</span><span class="sxs-lookup"><span data-stu-id="077e3-172">String</span></span>|<span data-ttu-id="077e3-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="077e3-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="077e3-174">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="077e3-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="077e3-175">version</span><span class="sxs-lookup"><span data-stu-id="077e3-175">version</span></span>|<span data-ttu-id="077e3-176">Int32</span><span class="sxs-lookup"><span data-stu-id="077e3-176">Int32</span></span>|<span data-ttu-id="077e3-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="077e3-177">Version of the device configuration.</span></span> <span data-ttu-id="077e3-178">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="077e3-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="077e3-179">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="077e3-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="077e3-180">Int32</span><span class="sxs-lookup"><span data-stu-id="077e3-180">Int32</span></span>|<span data-ttu-id="077e3-181">证书续订阈值百分比。</span><span class="sxs-lookup"><span data-stu-id="077e3-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="077e3-182">从[AndroidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)继承的有效值1到99</span><span class="sxs-lookup"><span data-stu-id="077e3-182">Valid values 1 to 99 Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span></span>|
|<span data-ttu-id="077e3-183">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="077e3-183">subjectNameFormat</span></span>|[<span data-ttu-id="077e3-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="077e3-184">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="077e3-185">证书使用者名称格式。</span><span class="sxs-lookup"><span data-stu-id="077e3-185">Certificate Subject Name Format.</span></span> <span data-ttu-id="077e3-186">继承自[androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="077e3-186">Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span></span> <span data-ttu-id="077e3-187">可取值为：`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId`。</span><span class="sxs-lookup"><span data-stu-id="077e3-187">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="077e3-188">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="077e3-188">certificateValidityPeriodValue</span></span>|<span data-ttu-id="077e3-189">Int32</span><span class="sxs-lookup"><span data-stu-id="077e3-189">Int32</span></span>|<span data-ttu-id="077e3-190">证书有效期限的值。</span><span class="sxs-lookup"><span data-stu-id="077e3-190">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="077e3-191">继承自[androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="077e3-191">Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span></span>|
|<span data-ttu-id="077e3-192">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="077e3-192">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="077e3-193">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="077e3-193">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="077e3-194">证书有效期的小数位数。</span><span class="sxs-lookup"><span data-stu-id="077e3-194">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="077e3-195">继承自[androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="077e3-195">Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span></span> <span data-ttu-id="077e3-196">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="077e3-196">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="077e3-197">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="077e3-197">extendedKeyUsages</span></span>|<span data-ttu-id="077e3-198">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)集合</span><span class="sxs-lookup"><span data-stu-id="077e3-198">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="077e3-199">扩展密钥用法（EKU）设置。</span><span class="sxs-lookup"><span data-stu-id="077e3-199">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="077e3-200">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="077e3-200">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="077e3-201">继承自[androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="077e3-201">Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span></span>|
|<span data-ttu-id="077e3-202">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="077e3-202">subjectAlternativeNameType</span></span>|[<span data-ttu-id="077e3-203">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="077e3-203">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="077e3-204">证书使用者备用名称类型。</span><span class="sxs-lookup"><span data-stu-id="077e3-204">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="077e3-205">继承自[androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="077e3-205">Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span></span> <span data-ttu-id="077e3-206">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService`。</span><span class="sxs-lookup"><span data-stu-id="077e3-206">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="077e3-207">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="077e3-207">scepServerUrls</span></span>|<span data-ttu-id="077e3-208">String 集合</span><span class="sxs-lookup"><span data-stu-id="077e3-208">String collection</span></span>|<span data-ttu-id="077e3-209">SCEP 服务器 Url</span><span class="sxs-lookup"><span data-stu-id="077e3-209">SCEP Server Url(s)</span></span>|
|<span data-ttu-id="077e3-210">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="077e3-210">subjectNameFormatString</span></span>|<span data-ttu-id="077e3-211">字符串</span><span class="sxs-lookup"><span data-stu-id="077e3-211">String</span></span>|<span data-ttu-id="077e3-212">要与 SubjectNameFormat = Custom 一起使用的自定义格式。</span><span class="sxs-lookup"><span data-stu-id="077e3-212">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="077e3-213">示例： CN = {{EmailAddress}}，E = {{EmailAddress}}，OU = 企业用户，O = Contoso Corporation，L = Redmond，ST = WA，C = US</span><span class="sxs-lookup"><span data-stu-id="077e3-213">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="077e3-214">keyUsage</span><span class="sxs-lookup"><span data-stu-id="077e3-214">keyUsage</span></span>|[<span data-ttu-id="077e3-215">keyUsages</span><span class="sxs-lookup"><span data-stu-id="077e3-215">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="077e3-216">SCEP 密钥用法。</span><span class="sxs-lookup"><span data-stu-id="077e3-216">SCEP Key Usage.</span></span> <span data-ttu-id="077e3-217">可取值为：`keyEncipherment`、`digitalSignature`。</span><span class="sxs-lookup"><span data-stu-id="077e3-217">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="077e3-218">keySize</span><span class="sxs-lookup"><span data-stu-id="077e3-218">keySize</span></span>|[<span data-ttu-id="077e3-219">keySize</span><span class="sxs-lookup"><span data-stu-id="077e3-219">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="077e3-220">SCEP 密钥大小。</span><span class="sxs-lookup"><span data-stu-id="077e3-220">SCEP Key Size.</span></span> <span data-ttu-id="077e3-221">可取值为：`size1024`、`size2048`。</span><span class="sxs-lookup"><span data-stu-id="077e3-221">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="077e3-222">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="077e3-222">hashAlgorithm</span></span>|[<span data-ttu-id="077e3-223">hashAlgorithms</span><span class="sxs-lookup"><span data-stu-id="077e3-223">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="077e3-224">SCEP 哈希算法。</span><span class="sxs-lookup"><span data-stu-id="077e3-224">SCEP Hash Algorithm.</span></span> <span data-ttu-id="077e3-225">可取值为：`sha1`、`sha2`。</span><span class="sxs-lookup"><span data-stu-id="077e3-225">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="077e3-226">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="077e3-226">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="077e3-227">字符串</span><span class="sxs-lookup"><span data-stu-id="077e3-227">String</span></span>|<span data-ttu-id="077e3-228">定义 AAD 属性的自定义字符串。</span><span class="sxs-lookup"><span data-stu-id="077e3-228">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="077e3-229">certificateStore</span><span class="sxs-lookup"><span data-stu-id="077e3-229">certificateStore</span></span>|[<span data-ttu-id="077e3-230">certificateStore</span><span class="sxs-lookup"><span data-stu-id="077e3-230">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="077e3-231">目标存储证书。</span><span class="sxs-lookup"><span data-stu-id="077e3-231">Target store certificate.</span></span> <span data-ttu-id="077e3-232">可取值为：`user`、`machine`。</span><span class="sxs-lookup"><span data-stu-id="077e3-232">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="077e3-233">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="077e3-233">customSubjectAlternativeNames</span></span>|<span data-ttu-id="077e3-234">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)集合</span><span class="sxs-lookup"><span data-stu-id="077e3-234">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="077e3-235">自定义主题备用名称设置。</span><span class="sxs-lookup"><span data-stu-id="077e3-235">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="077e3-236">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="077e3-236">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="077e3-237">响应</span><span class="sxs-lookup"><span data-stu-id="077e3-237">Response</span></span>
<span data-ttu-id="077e3-238">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[androidDeviceOwnerScepCertificateProfile](../resources/intune-deviceconfig-androiddeviceownerscepcertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="077e3-238">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerScepCertificateProfile](../resources/intune-deviceconfig-androiddeviceownerscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="077e3-239">示例</span><span class="sxs-lookup"><span data-stu-id="077e3-239">Example</span></span>

### <a name="request"></a><span data-ttu-id="077e3-240">请求</span><span class="sxs-lookup"><span data-stu-id="077e3-240">Request</span></span>
<span data-ttu-id="077e3-241">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="077e3-241">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1982

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerScepCertificateProfile",
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
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
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

### <a name="response"></a><span data-ttu-id="077e3-242">响应</span><span class="sxs-lookup"><span data-stu-id="077e3-242">Response</span></span>
<span data-ttu-id="077e3-p125">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="077e3-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2154

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerScepCertificateProfile",
  "id": "7d8b9c9a-9c9a-7d8b-9a9c-8b7d9a9c8b7d",
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
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
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






