---
title: 更新 androidForWorkScepCertificateProfile
description: 更新 androidForWorkScepCertificateProfile 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a9d2565698430634ead4479faa780b39278a3df9
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37176413"
---
# <a name="update-androidforworkscepcertificateprofile"></a><span data-ttu-id="ce6e8-103">更新 androidForWorkScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="ce6e8-103">Update androidForWorkScepCertificateProfile</span></span>

> <span data-ttu-id="ce6e8-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ce6e8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ce6e8-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ce6e8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ce6e8-106">更新[androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ce6e8-106">Update the properties of a [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ce6e8-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="ce6e8-107">Prerequisites</span></span>
<span data-ttu-id="ce6e8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ce6e8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce6e8-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ce6e8-110">Permission type</span></span>|<span data-ttu-id="ce6e8-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ce6e8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ce6e8-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ce6e8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ce6e8-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce6e8-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ce6e8-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ce6e8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ce6e8-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ce6e8-115">Not supported.</span></span>|
|<span data-ttu-id="ce6e8-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ce6e8-116">Application</span></span>|<span data-ttu-id="ce6e8-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce6e8-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ce6e8-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ce6e8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ce6e8-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ce6e8-119">Request headers</span></span>
|<span data-ttu-id="ce6e8-120">标头</span><span class="sxs-lookup"><span data-stu-id="ce6e8-120">Header</span></span>|<span data-ttu-id="ce6e8-121">值</span><span class="sxs-lookup"><span data-stu-id="ce6e8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ce6e8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ce6e8-122">Authorization</span></span>|<span data-ttu-id="ce6e8-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ce6e8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ce6e8-124">接受</span><span class="sxs-lookup"><span data-stu-id="ce6e8-124">Accept</span></span>|<span data-ttu-id="ce6e8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ce6e8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ce6e8-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ce6e8-126">Request body</span></span>
<span data-ttu-id="ce6e8-127">在请求正文中，提供[androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ce6e8-127">In the request body, supply a JSON representation for the [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) object.</span></span>

<span data-ttu-id="ce6e8-128">下表显示创建[androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ce6e8-128">The following table shows the properties that are required when you create the [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md).</span></span>

|<span data-ttu-id="ce6e8-129">属性</span><span class="sxs-lookup"><span data-stu-id="ce6e8-129">Property</span></span>|<span data-ttu-id="ce6e8-130">类型</span><span class="sxs-lookup"><span data-stu-id="ce6e8-130">Type</span></span>|<span data-ttu-id="ce6e8-131">说明</span><span class="sxs-lookup"><span data-stu-id="ce6e8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce6e8-132">id</span><span class="sxs-lookup"><span data-stu-id="ce6e8-132">id</span></span>|<span data-ttu-id="ce6e8-133">字符串</span><span class="sxs-lookup"><span data-stu-id="ce6e8-133">String</span></span>|<span data-ttu-id="ce6e8-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="ce6e8-134">Key of the entity.</span></span> <span data-ttu-id="ce6e8-135">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce6e8-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce6e8-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ce6e8-136">lastModifiedDateTime</span></span>|<span data-ttu-id="ce6e8-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce6e8-137">DateTimeOffset</span></span>|<span data-ttu-id="ce6e8-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="ce6e8-138">DateTime the object was last modified.</span></span> <span data-ttu-id="ce6e8-139">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce6e8-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce6e8-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ce6e8-140">roleScopeTagIds</span></span>|<span data-ttu-id="ce6e8-141">String collection</span><span class="sxs-lookup"><span data-stu-id="ce6e8-141">String collection</span></span>|<span data-ttu-id="ce6e8-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="ce6e8-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ce6e8-143">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce6e8-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce6e8-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ce6e8-144">supportsScopeTags</span></span>|<span data-ttu-id="ce6e8-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce6e8-145">Boolean</span></span>|<span data-ttu-id="ce6e8-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="ce6e8-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ce6e8-147">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="ce6e8-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ce6e8-148">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="ce6e8-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ce6e8-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="ce6e8-149">This property is read-only.</span></span> <span data-ttu-id="ce6e8-150">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce6e8-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce6e8-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ce6e8-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="ce6e8-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ce6e8-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="ce6e8-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="ce6e8-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="ce6e8-154">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce6e8-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce6e8-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ce6e8-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="ce6e8-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ce6e8-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="ce6e8-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="ce6e8-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="ce6e8-158">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce6e8-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce6e8-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ce6e8-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="ce6e8-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ce6e8-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="ce6e8-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="ce6e8-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="ce6e8-162">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce6e8-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce6e8-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ce6e8-163">createdDateTime</span></span>|<span data-ttu-id="ce6e8-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce6e8-164">DateTimeOffset</span></span>|<span data-ttu-id="ce6e8-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="ce6e8-165">DateTime the object was created.</span></span> <span data-ttu-id="ce6e8-166">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce6e8-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce6e8-167">说明</span><span class="sxs-lookup"><span data-stu-id="ce6e8-167">description</span></span>|<span data-ttu-id="ce6e8-168">String</span><span class="sxs-lookup"><span data-stu-id="ce6e8-168">String</span></span>|<span data-ttu-id="ce6e8-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="ce6e8-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ce6e8-170">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce6e8-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce6e8-171">displayName</span><span class="sxs-lookup"><span data-stu-id="ce6e8-171">displayName</span></span>|<span data-ttu-id="ce6e8-172">String</span><span class="sxs-lookup"><span data-stu-id="ce6e8-172">String</span></span>|<span data-ttu-id="ce6e8-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="ce6e8-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ce6e8-174">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce6e8-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce6e8-175">version</span><span class="sxs-lookup"><span data-stu-id="ce6e8-175">version</span></span>|<span data-ttu-id="ce6e8-176">Int32</span><span class="sxs-lookup"><span data-stu-id="ce6e8-176">Int32</span></span>|<span data-ttu-id="ce6e8-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="ce6e8-177">Version of the device configuration.</span></span> <span data-ttu-id="ce6e8-178">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce6e8-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce6e8-179">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="ce6e8-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="ce6e8-180">Int32</span><span class="sxs-lookup"><span data-stu-id="ce6e8-180">Int32</span></span>|<span data-ttu-id="ce6e8-181">证书续订阈值百分比。</span><span class="sxs-lookup"><span data-stu-id="ce6e8-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="ce6e8-182">从[AndroidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)继承的有效值1到99</span><span class="sxs-lookup"><span data-stu-id="ce6e8-182">Valid values 1 to 99 Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="ce6e8-183">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="ce6e8-183">subjectNameFormat</span></span>|[<span data-ttu-id="ce6e8-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="ce6e8-184">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="ce6e8-185">证书使用者名称格式。</span><span class="sxs-lookup"><span data-stu-id="ce6e8-185">Certificate Subject Name Format.</span></span> <span data-ttu-id="ce6e8-186">继承自[androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="ce6e8-186">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="ce6e8-187">可取值为：`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId`。</span><span class="sxs-lookup"><span data-stu-id="ce6e8-187">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="ce6e8-188">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="ce6e8-188">certificateValidityPeriodValue</span></span>|<span data-ttu-id="ce6e8-189">Int32</span><span class="sxs-lookup"><span data-stu-id="ce6e8-189">Int32</span></span>|<span data-ttu-id="ce6e8-190">证书有效期限的值。</span><span class="sxs-lookup"><span data-stu-id="ce6e8-190">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="ce6e8-191">继承自[androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="ce6e8-191">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="ce6e8-192">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="ce6e8-192">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="ce6e8-193">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="ce6e8-193">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="ce6e8-194">证书有效期的小数位数。</span><span class="sxs-lookup"><span data-stu-id="ce6e8-194">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="ce6e8-195">继承自[androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="ce6e8-195">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="ce6e8-196">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="ce6e8-196">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="ce6e8-197">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="ce6e8-197">extendedKeyUsages</span></span>|<span data-ttu-id="ce6e8-198">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)集合</span><span class="sxs-lookup"><span data-stu-id="ce6e8-198">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="ce6e8-199">扩展密钥用法（EKU）设置。</span><span class="sxs-lookup"><span data-stu-id="ce6e8-199">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="ce6e8-200">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="ce6e8-200">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="ce6e8-201">继承自[androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="ce6e8-201">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="ce6e8-202">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="ce6e8-202">subjectAlternativeNameType</span></span>|[<span data-ttu-id="ce6e8-203">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="ce6e8-203">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="ce6e8-204">证书使用者备用名称类型。</span><span class="sxs-lookup"><span data-stu-id="ce6e8-204">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="ce6e8-205">继承自[androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="ce6e8-205">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="ce6e8-206">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService`。</span><span class="sxs-lookup"><span data-stu-id="ce6e8-206">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="ce6e8-207">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="ce6e8-207">scepServerUrls</span></span>|<span data-ttu-id="ce6e8-208">String collection</span><span class="sxs-lookup"><span data-stu-id="ce6e8-208">String collection</span></span>|<span data-ttu-id="ce6e8-209">SCEP 服务器 Url</span><span class="sxs-lookup"><span data-stu-id="ce6e8-209">SCEP Server Url(s)</span></span>|
|<span data-ttu-id="ce6e8-210">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="ce6e8-210">subjectNameFormatString</span></span>|<span data-ttu-id="ce6e8-211">String</span><span class="sxs-lookup"><span data-stu-id="ce6e8-211">String</span></span>|<span data-ttu-id="ce6e8-212">要与 SubjectNameFormat = Custom 一起使用的自定义格式。</span><span class="sxs-lookup"><span data-stu-id="ce6e8-212">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="ce6e8-213">示例： CN = {{EmailAddress}}，E = {{EmailAddress}}，OU = 企业用户，O = Contoso Corporation，L = Redmond，ST = WA，C = US</span><span class="sxs-lookup"><span data-stu-id="ce6e8-213">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="ce6e8-214">keyUsage</span><span class="sxs-lookup"><span data-stu-id="ce6e8-214">keyUsage</span></span>|[<span data-ttu-id="ce6e8-215">keyUsages</span><span class="sxs-lookup"><span data-stu-id="ce6e8-215">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="ce6e8-216">SCEP 密钥用法。</span><span class="sxs-lookup"><span data-stu-id="ce6e8-216">SCEP Key Usage.</span></span> <span data-ttu-id="ce6e8-217">可取值为：`keyEncipherment`、`digitalSignature`。</span><span class="sxs-lookup"><span data-stu-id="ce6e8-217">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="ce6e8-218">keySize</span><span class="sxs-lookup"><span data-stu-id="ce6e8-218">keySize</span></span>|[<span data-ttu-id="ce6e8-219">keySize</span><span class="sxs-lookup"><span data-stu-id="ce6e8-219">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="ce6e8-220">SCEP 密钥大小。</span><span class="sxs-lookup"><span data-stu-id="ce6e8-220">SCEP Key Size.</span></span> <span data-ttu-id="ce6e8-221">可取值为：`size1024`、`size2048`。</span><span class="sxs-lookup"><span data-stu-id="ce6e8-221">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="ce6e8-222">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="ce6e8-222">hashAlgorithm</span></span>|[<span data-ttu-id="ce6e8-223">hashAlgorithms</span><span class="sxs-lookup"><span data-stu-id="ce6e8-223">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="ce6e8-224">SCEP 哈希算法。</span><span class="sxs-lookup"><span data-stu-id="ce6e8-224">SCEP Hash Algorithm.</span></span> <span data-ttu-id="ce6e8-225">可取值为：`sha1`、`sha2`。</span><span class="sxs-lookup"><span data-stu-id="ce6e8-225">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="ce6e8-226">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="ce6e8-226">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="ce6e8-227">String</span><span class="sxs-lookup"><span data-stu-id="ce6e8-227">String</span></span>|<span data-ttu-id="ce6e8-228">定义 AAD 属性的自定义字符串。</span><span class="sxs-lookup"><span data-stu-id="ce6e8-228">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="ce6e8-229">certificateStore</span><span class="sxs-lookup"><span data-stu-id="ce6e8-229">certificateStore</span></span>|[<span data-ttu-id="ce6e8-230">certificateStore</span><span class="sxs-lookup"><span data-stu-id="ce6e8-230">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="ce6e8-231">目标存储证书。</span><span class="sxs-lookup"><span data-stu-id="ce6e8-231">Target store certificate.</span></span> <span data-ttu-id="ce6e8-232">可取值为：`user`、`machine`。</span><span class="sxs-lookup"><span data-stu-id="ce6e8-232">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="ce6e8-233">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="ce6e8-233">customSubjectAlternativeNames</span></span>|<span data-ttu-id="ce6e8-234">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)集合</span><span class="sxs-lookup"><span data-stu-id="ce6e8-234">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="ce6e8-235">自定义主题备用名称设置。</span><span class="sxs-lookup"><span data-stu-id="ce6e8-235">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="ce6e8-236">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="ce6e8-236">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="ce6e8-237">响应</span><span class="sxs-lookup"><span data-stu-id="ce6e8-237">Response</span></span>
<span data-ttu-id="ce6e8-238">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ce6e8-238">If successful, this method returns a `200 OK` response code and an updated [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce6e8-239">示例</span><span class="sxs-lookup"><span data-stu-id="ce6e8-239">Example</span></span>

### <a name="request"></a><span data-ttu-id="ce6e8-240">请求</span><span class="sxs-lookup"><span data-stu-id="ce6e8-240">Request</span></span>
<span data-ttu-id="ce6e8-241">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ce6e8-241">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1978

{
  "@odata.type": "#microsoft.graph.androidForWorkScepCertificateProfile",
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

### <a name="response"></a><span data-ttu-id="ce6e8-242">响应</span><span class="sxs-lookup"><span data-stu-id="ce6e8-242">Response</span></span>
<span data-ttu-id="ce6e8-p125">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ce6e8-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2150

{
  "@odata.type": "#microsoft.graph.androidForWorkScepCertificateProfile",
  "id": "09e532af-32af-09e5-af32-e509af32e509",
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




