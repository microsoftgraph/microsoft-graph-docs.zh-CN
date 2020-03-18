---
title: 更新 macOSImportedPFXCertificateProfile
description: 更新 macOSImportedPFXCertificateProfile 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 440e18ca9258ae9a2467e18d405b930259c34118
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42745371"
---
# <a name="update-macosimportedpfxcertificateprofile"></a><span data-ttu-id="2dfc4-103">更新 macOSImportedPFXCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="2dfc4-103">Update macOSImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="2dfc4-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2dfc4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2dfc4-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2dfc4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2dfc4-106">更新[macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="2dfc4-106">Update the properties of a [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2dfc4-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="2dfc4-107">Prerequisites</span></span>
<span data-ttu-id="2dfc4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2dfc4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2dfc4-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="2dfc4-110">Permission type</span></span>|<span data-ttu-id="2dfc4-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2dfc4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2dfc4-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2dfc4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2dfc4-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2dfc4-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2dfc4-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2dfc4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2dfc4-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="2dfc4-115">Not supported.</span></span>|
|<span data-ttu-id="2dfc4-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="2dfc4-116">Application</span></span>|<span data-ttu-id="2dfc4-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2dfc4-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2dfc4-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2dfc4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="2dfc4-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="2dfc4-119">Request headers</span></span>
|<span data-ttu-id="2dfc4-120">标头</span><span class="sxs-lookup"><span data-stu-id="2dfc4-120">Header</span></span>|<span data-ttu-id="2dfc4-121">值</span><span class="sxs-lookup"><span data-stu-id="2dfc4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2dfc4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2dfc4-122">Authorization</span></span>|<span data-ttu-id="2dfc4-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2dfc4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2dfc4-124">接受</span><span class="sxs-lookup"><span data-stu-id="2dfc4-124">Accept</span></span>|<span data-ttu-id="2dfc4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2dfc4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2dfc4-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="2dfc4-126">Request body</span></span>
<span data-ttu-id="2dfc4-127">在请求正文中，提供[macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2dfc4-127">In the request body, supply a JSON representation for the [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) object.</span></span>

<span data-ttu-id="2dfc4-128">下表显示创建[macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2dfc4-128">The following table shows the properties that are required when you create the [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md).</span></span>

|<span data-ttu-id="2dfc4-129">属性</span><span class="sxs-lookup"><span data-stu-id="2dfc4-129">Property</span></span>|<span data-ttu-id="2dfc4-130">类型</span><span class="sxs-lookup"><span data-stu-id="2dfc4-130">Type</span></span>|<span data-ttu-id="2dfc4-131">说明</span><span class="sxs-lookup"><span data-stu-id="2dfc4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2dfc4-132">id</span><span class="sxs-lookup"><span data-stu-id="2dfc4-132">id</span></span>|<span data-ttu-id="2dfc4-133">字符串</span><span class="sxs-lookup"><span data-stu-id="2dfc4-133">String</span></span>|<span data-ttu-id="2dfc4-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="2dfc4-134">Key of the entity.</span></span> <span data-ttu-id="2dfc4-135">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2dfc4-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2dfc4-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2dfc4-136">lastModifiedDateTime</span></span>|<span data-ttu-id="2dfc4-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2dfc4-137">DateTimeOffset</span></span>|<span data-ttu-id="2dfc4-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="2dfc4-138">DateTime the object was last modified.</span></span> <span data-ttu-id="2dfc4-139">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2dfc4-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2dfc4-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2dfc4-140">roleScopeTagIds</span></span>|<span data-ttu-id="2dfc4-141">String collection</span><span class="sxs-lookup"><span data-stu-id="2dfc4-141">String collection</span></span>|<span data-ttu-id="2dfc4-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="2dfc4-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="2dfc4-143">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2dfc4-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2dfc4-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="2dfc4-144">supportsScopeTags</span></span>|<span data-ttu-id="2dfc4-145">布尔值</span><span class="sxs-lookup"><span data-stu-id="2dfc4-145">Boolean</span></span>|<span data-ttu-id="2dfc4-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="2dfc4-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="2dfc4-147">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="2dfc4-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="2dfc4-148">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="2dfc4-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="2dfc4-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="2dfc4-149">This property is read-only.</span></span> <span data-ttu-id="2dfc4-150">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2dfc4-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2dfc4-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="2dfc4-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="2dfc4-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="2dfc4-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="2dfc4-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="2dfc4-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="2dfc4-154">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2dfc4-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2dfc4-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="2dfc4-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="2dfc4-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="2dfc4-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="2dfc4-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="2dfc4-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="2dfc4-158">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2dfc4-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2dfc4-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="2dfc4-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="2dfc4-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="2dfc4-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="2dfc4-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="2dfc4-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="2dfc4-162">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2dfc4-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2dfc4-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2dfc4-163">createdDateTime</span></span>|<span data-ttu-id="2dfc4-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2dfc4-164">DateTimeOffset</span></span>|<span data-ttu-id="2dfc4-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="2dfc4-165">DateTime the object was created.</span></span> <span data-ttu-id="2dfc4-166">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2dfc4-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2dfc4-167">说明</span><span class="sxs-lookup"><span data-stu-id="2dfc4-167">description</span></span>|<span data-ttu-id="2dfc4-168">String</span><span class="sxs-lookup"><span data-stu-id="2dfc4-168">String</span></span>|<span data-ttu-id="2dfc4-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="2dfc4-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2dfc4-170">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2dfc4-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2dfc4-171">displayName</span><span class="sxs-lookup"><span data-stu-id="2dfc4-171">displayName</span></span>|<span data-ttu-id="2dfc4-172">String</span><span class="sxs-lookup"><span data-stu-id="2dfc4-172">String</span></span>|<span data-ttu-id="2dfc4-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="2dfc4-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2dfc4-174">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2dfc4-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2dfc4-175">version</span><span class="sxs-lookup"><span data-stu-id="2dfc4-175">version</span></span>|<span data-ttu-id="2dfc4-176">Int32</span><span class="sxs-lookup"><span data-stu-id="2dfc4-176">Int32</span></span>|<span data-ttu-id="2dfc4-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="2dfc4-177">Version of the device configuration.</span></span> <span data-ttu-id="2dfc4-178">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2dfc4-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2dfc4-179">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="2dfc4-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="2dfc4-180">Int32</span><span class="sxs-lookup"><span data-stu-id="2dfc4-180">Int32</span></span>|<span data-ttu-id="2dfc4-181">证书续订阈值百分比。</span><span class="sxs-lookup"><span data-stu-id="2dfc4-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="2dfc4-182">继承自[macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="2dfc4-182">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="2dfc4-183">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="2dfc4-183">subjectNameFormat</span></span>|[<span data-ttu-id="2dfc4-184">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="2dfc4-184">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="2dfc4-185">证书使用者名称格式。</span><span class="sxs-lookup"><span data-stu-id="2dfc4-185">Certificate Subject Name Format.</span></span> <span data-ttu-id="2dfc4-186">继承自[macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="2dfc4-186">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="2dfc4-187">可取值为：`commonName`、`commonNameAsEmail`、`custom`、`commonNameIncludingEmail`、`commonNameAsIMEI`、`commonNameAsSerialNumber`。</span><span class="sxs-lookup"><span data-stu-id="2dfc4-187">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="2dfc4-188">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="2dfc4-188">subjectAlternativeNameType</span></span>|[<span data-ttu-id="2dfc4-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="2dfc4-189">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="2dfc4-190">证书使用者备用名称类型。</span><span class="sxs-lookup"><span data-stu-id="2dfc4-190">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="2dfc4-191">继承自[macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="2dfc4-191">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="2dfc4-192">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService`。</span><span class="sxs-lookup"><span data-stu-id="2dfc4-192">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="2dfc4-193">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="2dfc4-193">certificateValidityPeriodValue</span></span>|<span data-ttu-id="2dfc4-194">Int32</span><span class="sxs-lookup"><span data-stu-id="2dfc4-194">Int32</span></span>|<span data-ttu-id="2dfc4-195">证书有效期限的值。</span><span class="sxs-lookup"><span data-stu-id="2dfc4-195">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="2dfc4-196">继承自[macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="2dfc4-196">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="2dfc4-197">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="2dfc4-197">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="2dfc4-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="2dfc4-198">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="2dfc4-199">证书有效期的小数位数。</span><span class="sxs-lookup"><span data-stu-id="2dfc4-199">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="2dfc4-200">继承自[macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="2dfc4-200">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="2dfc4-201">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="2dfc4-201">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="2dfc4-202">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="2dfc4-202">intendedPurpose</span></span>|[<span data-ttu-id="2dfc4-203">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="2dfc4-203">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="2dfc4-204">证书配置文件的预期用途-可以为未分配、SmimeEncryption、SmimeSigning 等。可能的值为`unassigned`： `smimeEncryption`、 `smimeSigning`、 `vpn`、 `wifi`、。</span><span class="sxs-lookup"><span data-stu-id="2dfc4-204">Intended Purpose of the Certificate Profile - which could be Unassigned, SmimeEncryption, SmimeSigning etc. Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="2dfc4-205">响应</span><span class="sxs-lookup"><span data-stu-id="2dfc4-205">Response</span></span>
<span data-ttu-id="2dfc4-206">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2dfc4-206">If successful, this method returns a `200 OK` response code and an updated [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2dfc4-207">示例</span><span class="sxs-lookup"><span data-stu-id="2dfc4-207">Example</span></span>

### <a name="request"></a><span data-ttu-id="2dfc4-208">请求</span><span class="sxs-lookup"><span data-stu-id="2dfc4-208">Request</span></span>
<span data-ttu-id="2dfc4-209">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2dfc4-209">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1297

{
  "@odata.type": "#microsoft.graph.macOSImportedPFXCertificateProfile",
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
  "subjectNameFormat": "commonNameAsEmail",
  "subjectAlternativeNameType": "emailAddress",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "intendedPurpose": "smimeEncryption"
}
```

### <a name="response"></a><span data-ttu-id="2dfc4-210">响应</span><span class="sxs-lookup"><span data-stu-id="2dfc4-210">Response</span></span>
<span data-ttu-id="2dfc4-p118">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2dfc4-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1469

{
  "@odata.type": "#microsoft.graph.macOSImportedPFXCertificateProfile",
  "id": "4175bd8c-bd8c-4175-8cbd-75418cbd7541",
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
  "subjectNameFormat": "commonNameAsEmail",
  "subjectAlternativeNameType": "emailAddress",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "intendedPurpose": "smimeEncryption"
}
```




