---
title: 更新 androidForWorkScepCertificateProfile
description: 更新 androidForWorkScepCertificateProfile 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b34630713b8fe164c12b6bdd32c313517b270773
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49238295"
---
# <a name="update-androidforworkscepcertificateprofile"></a><span data-ttu-id="d2091-103">更新 androidForWorkScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="d2091-103">Update androidForWorkScepCertificateProfile</span></span>

<span data-ttu-id="d2091-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d2091-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d2091-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d2091-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d2091-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d2091-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d2091-107">更新 [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d2091-107">Update the properties of a [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d2091-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="d2091-108">Prerequisites</span></span>
<span data-ttu-id="d2091-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d2091-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2091-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d2091-111">Permission type</span></span>|<span data-ttu-id="d2091-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d2091-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d2091-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d2091-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d2091-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2091-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d2091-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d2091-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d2091-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d2091-116">Not supported.</span></span>|
|<span data-ttu-id="d2091-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d2091-117">Application</span></span>|<span data-ttu-id="d2091-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2091-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d2091-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d2091-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="d2091-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d2091-120">Request headers</span></span>
|<span data-ttu-id="d2091-121">标头</span><span class="sxs-lookup"><span data-stu-id="d2091-121">Header</span></span>|<span data-ttu-id="d2091-122">值</span><span class="sxs-lookup"><span data-stu-id="d2091-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d2091-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d2091-123">Authorization</span></span>|<span data-ttu-id="d2091-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d2091-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d2091-125">接受</span><span class="sxs-lookup"><span data-stu-id="d2091-125">Accept</span></span>|<span data-ttu-id="d2091-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d2091-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2091-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d2091-127">Request body</span></span>
<span data-ttu-id="d2091-128">在请求正文中，提供 [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d2091-128">In the request body, supply a JSON representation for the [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) object.</span></span>

<span data-ttu-id="d2091-129">下表显示创建 [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d2091-129">The following table shows the properties that are required when you create the [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md).</span></span>

|<span data-ttu-id="d2091-130">属性</span><span class="sxs-lookup"><span data-stu-id="d2091-130">Property</span></span>|<span data-ttu-id="d2091-131">类型</span><span class="sxs-lookup"><span data-stu-id="d2091-131">Type</span></span>|<span data-ttu-id="d2091-132">说明</span><span class="sxs-lookup"><span data-stu-id="d2091-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2091-133">id</span><span class="sxs-lookup"><span data-stu-id="d2091-133">id</span></span>|<span data-ttu-id="d2091-134">String</span><span class="sxs-lookup"><span data-stu-id="d2091-134">String</span></span>|<span data-ttu-id="d2091-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d2091-135">Key of the entity.</span></span> <span data-ttu-id="d2091-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d2091-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2091-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d2091-137">lastModifiedDateTime</span></span>|<span data-ttu-id="d2091-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d2091-138">DateTimeOffset</span></span>|<span data-ttu-id="d2091-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="d2091-139">DateTime the object was last modified.</span></span> <span data-ttu-id="d2091-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d2091-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2091-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d2091-141">roleScopeTagIds</span></span>|<span data-ttu-id="d2091-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="d2091-142">String collection</span></span>|<span data-ttu-id="d2091-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="d2091-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d2091-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d2091-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2091-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d2091-145">supportsScopeTags</span></span>|<span data-ttu-id="d2091-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="d2091-146">Boolean</span></span>|<span data-ttu-id="d2091-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="d2091-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d2091-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="d2091-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d2091-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="d2091-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d2091-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="d2091-150">This property is read-only.</span></span> <span data-ttu-id="d2091-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d2091-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2091-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d2091-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="d2091-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d2091-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="d2091-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="d2091-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="d2091-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d2091-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2091-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d2091-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="d2091-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d2091-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="d2091-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="d2091-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="d2091-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d2091-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2091-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="d2091-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="d2091-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="d2091-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="d2091-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="d2091-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="d2091-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d2091-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2091-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d2091-164">createdDateTime</span></span>|<span data-ttu-id="d2091-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d2091-165">DateTimeOffset</span></span>|<span data-ttu-id="d2091-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="d2091-166">DateTime the object was created.</span></span> <span data-ttu-id="d2091-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d2091-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2091-168">description</span><span class="sxs-lookup"><span data-stu-id="d2091-168">description</span></span>|<span data-ttu-id="d2091-169">String</span><span class="sxs-lookup"><span data-stu-id="d2091-169">String</span></span>|<span data-ttu-id="d2091-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="d2091-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d2091-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d2091-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2091-172">displayName</span><span class="sxs-lookup"><span data-stu-id="d2091-172">displayName</span></span>|<span data-ttu-id="d2091-173">String</span><span class="sxs-lookup"><span data-stu-id="d2091-173">String</span></span>|<span data-ttu-id="d2091-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="d2091-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d2091-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d2091-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2091-176">version</span><span class="sxs-lookup"><span data-stu-id="d2091-176">version</span></span>|<span data-ttu-id="d2091-177">Int32</span><span class="sxs-lookup"><span data-stu-id="d2091-177">Int32</span></span>|<span data-ttu-id="d2091-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="d2091-178">Version of the device configuration.</span></span> <span data-ttu-id="d2091-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d2091-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2091-180">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="d2091-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="d2091-181">Int32</span><span class="sxs-lookup"><span data-stu-id="d2091-181">Int32</span></span>|<span data-ttu-id="d2091-182">证书续订阈值百分比。</span><span class="sxs-lookup"><span data-stu-id="d2091-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="d2091-183">从[AndroidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)继承的有效值1到99</span><span class="sxs-lookup"><span data-stu-id="d2091-183">Valid values 1 to 99 Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="d2091-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="d2091-184">subjectNameFormat</span></span>|[<span data-ttu-id="d2091-185">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="d2091-185">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="d2091-186">证书使用者名称格式。</span><span class="sxs-lookup"><span data-stu-id="d2091-186">Certificate Subject Name Format.</span></span> <span data-ttu-id="d2091-187">继承自 [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="d2091-187">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="d2091-188">可取值为：`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId`。</span><span class="sxs-lookup"><span data-stu-id="d2091-188">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="d2091-189">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="d2091-189">certificateValidityPeriodValue</span></span>|<span data-ttu-id="d2091-190">Int32</span><span class="sxs-lookup"><span data-stu-id="d2091-190">Int32</span></span>|<span data-ttu-id="d2091-191">证书有效期限的值。</span><span class="sxs-lookup"><span data-stu-id="d2091-191">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="d2091-192">继承自 [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="d2091-192">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="d2091-193">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="d2091-193">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="d2091-194">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="d2091-194">certificateValidityPeriodScale</span></span>](../resources/intune-shared-certificatevalidityperiodscale.md)|<span data-ttu-id="d2091-195">证书有效期的小数位数。</span><span class="sxs-lookup"><span data-stu-id="d2091-195">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="d2091-196">继承自 [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="d2091-196">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="d2091-197">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="d2091-197">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="d2091-198">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="d2091-198">extendedKeyUsages</span></span>|<span data-ttu-id="d2091-199">[extendedKeyUsage](../resources/intune-shared-extendedkeyusage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d2091-199">[extendedKeyUsage](../resources/intune-shared-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="d2091-200"> (EKU) 设置的扩展密钥用法。</span><span class="sxs-lookup"><span data-stu-id="d2091-200">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="d2091-201">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="d2091-201">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="d2091-202">继承自 [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="d2091-202">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="d2091-203">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="d2091-203">subjectAlternativeNameType</span></span>|[<span data-ttu-id="d2091-204">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="d2091-204">subjectAlternativeNameType</span></span>](../resources/intune-shared-subjectalternativenametype.md)|<span data-ttu-id="d2091-205">证书使用者备用名称类型。</span><span class="sxs-lookup"><span data-stu-id="d2091-205">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="d2091-206">继承自 [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="d2091-206">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="d2091-207">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService`、`universalResourceIdentifier`。</span><span class="sxs-lookup"><span data-stu-id="d2091-207">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span></span>|
|<span data-ttu-id="d2091-208">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="d2091-208">scepServerUrls</span></span>|<span data-ttu-id="d2091-209">String 集合</span><span class="sxs-lookup"><span data-stu-id="d2091-209">String collection</span></span>|<span data-ttu-id="d2091-210">SCEP 服务器 Url (s) </span><span class="sxs-lookup"><span data-stu-id="d2091-210">SCEP Server Url(s)</span></span>|
|<span data-ttu-id="d2091-211">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="d2091-211">subjectNameFormatString</span></span>|<span data-ttu-id="d2091-212">String</span><span class="sxs-lookup"><span data-stu-id="d2091-212">String</span></span>|<span data-ttu-id="d2091-213">要与 SubjectNameFormat = Custom 一起使用的自定义格式。</span><span class="sxs-lookup"><span data-stu-id="d2091-213">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="d2091-214">示例： CN = {{EmailAddress}}，E = {{EmailAddress}}，OU = 企业用户，O = Contoso Corporation，L = Redmond，ST = WA，C = US</span><span class="sxs-lookup"><span data-stu-id="d2091-214">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="d2091-215">keyUsage</span><span class="sxs-lookup"><span data-stu-id="d2091-215">keyUsage</span></span>|[<span data-ttu-id="d2091-216">keyUsages</span><span class="sxs-lookup"><span data-stu-id="d2091-216">keyUsages</span></span>](../resources/intune-shared-keyusages.md)|<span data-ttu-id="d2091-217">SCEP 密钥用法。</span><span class="sxs-lookup"><span data-stu-id="d2091-217">SCEP Key Usage.</span></span> <span data-ttu-id="d2091-218">可取值为：`keyEncipherment`、`digitalSignature`。</span><span class="sxs-lookup"><span data-stu-id="d2091-218">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="d2091-219">keySize</span><span class="sxs-lookup"><span data-stu-id="d2091-219">keySize</span></span>|[<span data-ttu-id="d2091-220">keySize</span><span class="sxs-lookup"><span data-stu-id="d2091-220">keySize</span></span>](../resources/intune-shared-keysize.md)|<span data-ttu-id="d2091-221">SCEP 密钥大小。</span><span class="sxs-lookup"><span data-stu-id="d2091-221">SCEP Key Size.</span></span> <span data-ttu-id="d2091-222">可取值为：`size1024`、`size2048`、`size4096`。</span><span class="sxs-lookup"><span data-stu-id="d2091-222">Possible values are: `size1024`, `size2048`, `size4096`.</span></span>|
|<span data-ttu-id="d2091-223">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="d2091-223">hashAlgorithm</span></span>|[<span data-ttu-id="d2091-224">hashAlgorithms</span><span class="sxs-lookup"><span data-stu-id="d2091-224">hashAlgorithms</span></span>](../resources/intune-shared-hashalgorithms.md)|<span data-ttu-id="d2091-225">SCEP 哈希算法。</span><span class="sxs-lookup"><span data-stu-id="d2091-225">SCEP Hash Algorithm.</span></span> <span data-ttu-id="d2091-226">可取值为：`sha1`、`sha2`。</span><span class="sxs-lookup"><span data-stu-id="d2091-226">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="d2091-227">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="d2091-227">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="d2091-228">String</span><span class="sxs-lookup"><span data-stu-id="d2091-228">String</span></span>|<span data-ttu-id="d2091-229">定义 AAD 属性的自定义字符串。</span><span class="sxs-lookup"><span data-stu-id="d2091-229">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="d2091-230">certificateStore</span><span class="sxs-lookup"><span data-stu-id="d2091-230">certificateStore</span></span>|[<span data-ttu-id="d2091-231">certificateStore</span><span class="sxs-lookup"><span data-stu-id="d2091-231">certificateStore</span></span>](../resources/intune-shared-certificatestore.md)|<span data-ttu-id="d2091-232">目标存储证书。</span><span class="sxs-lookup"><span data-stu-id="d2091-232">Target store certificate.</span></span> <span data-ttu-id="d2091-233">可取值为：`user`、`machine`。</span><span class="sxs-lookup"><span data-stu-id="d2091-233">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="d2091-234">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="d2091-234">customSubjectAlternativeNames</span></span>|<span data-ttu-id="d2091-235">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d2091-235">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="d2091-236">自定义主题备用名称设置。</span><span class="sxs-lookup"><span data-stu-id="d2091-236">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="d2091-237">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="d2091-237">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="d2091-238">响应</span><span class="sxs-lookup"><span data-stu-id="d2091-238">Response</span></span>
<span data-ttu-id="d2091-239">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d2091-239">If successful, this method returns a `200 OK` response code and an updated [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2091-240">示例</span><span class="sxs-lookup"><span data-stu-id="d2091-240">Example</span></span>

### <a name="request"></a><span data-ttu-id="d2091-241">请求</span><span class="sxs-lookup"><span data-stu-id="d2091-241">Request</span></span>
<span data-ttu-id="d2091-242">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d2091-242">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d2091-243">响应</span><span class="sxs-lookup"><span data-stu-id="d2091-243">Response</span></span>
<span data-ttu-id="d2091-p125">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d2091-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




