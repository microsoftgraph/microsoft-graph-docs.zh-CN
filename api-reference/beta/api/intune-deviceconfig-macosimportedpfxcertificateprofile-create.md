---
title: 创建 macOSImportedPFXCertificateProfile
description: 创建新的 macOSImportedPFXCertificateProfile 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c2bb939245e60f9941d28e5a92432cf67744e324
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37184113"
---
# <a name="create-macosimportedpfxcertificateprofile"></a><span data-ttu-id="6967a-103">创建 macOSImportedPFXCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="6967a-103">Create macOSImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="6967a-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6967a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6967a-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6967a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6967a-106">创建新的[macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6967a-106">Create a new [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6967a-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="6967a-107">Prerequisites</span></span>
<span data-ttu-id="6967a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6967a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6967a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="6967a-110">Permission type</span></span>|<span data-ttu-id="6967a-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6967a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6967a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6967a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6967a-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6967a-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6967a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6967a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6967a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6967a-115">Not supported.</span></span>|
|<span data-ttu-id="6967a-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="6967a-116">Application</span></span>|<span data-ttu-id="6967a-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6967a-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6967a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6967a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="6967a-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="6967a-119">Request headers</span></span>
|<span data-ttu-id="6967a-120">标头</span><span class="sxs-lookup"><span data-stu-id="6967a-120">Header</span></span>|<span data-ttu-id="6967a-121">值</span><span class="sxs-lookup"><span data-stu-id="6967a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6967a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6967a-122">Authorization</span></span>|<span data-ttu-id="6967a-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6967a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6967a-124">接受</span><span class="sxs-lookup"><span data-stu-id="6967a-124">Accept</span></span>|<span data-ttu-id="6967a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6967a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6967a-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="6967a-126">Request body</span></span>
<span data-ttu-id="6967a-127">在请求正文中，提供 macOSImportedPFXCertificateProfile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6967a-127">In the request body, supply a JSON representation for the macOSImportedPFXCertificateProfile object.</span></span>

<span data-ttu-id="6967a-128">下表显示创建 macOSImportedPFXCertificateProfile 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6967a-128">The following table shows the properties that are required when you create the macOSImportedPFXCertificateProfile.</span></span>

|<span data-ttu-id="6967a-129">属性</span><span class="sxs-lookup"><span data-stu-id="6967a-129">Property</span></span>|<span data-ttu-id="6967a-130">类型</span><span class="sxs-lookup"><span data-stu-id="6967a-130">Type</span></span>|<span data-ttu-id="6967a-131">说明</span><span class="sxs-lookup"><span data-stu-id="6967a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6967a-132">id</span><span class="sxs-lookup"><span data-stu-id="6967a-132">id</span></span>|<span data-ttu-id="6967a-133">字符串</span><span class="sxs-lookup"><span data-stu-id="6967a-133">String</span></span>|<span data-ttu-id="6967a-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="6967a-134">Key of the entity.</span></span> <span data-ttu-id="6967a-135">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6967a-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6967a-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6967a-136">lastModifiedDateTime</span></span>|<span data-ttu-id="6967a-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6967a-137">DateTimeOffset</span></span>|<span data-ttu-id="6967a-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="6967a-138">DateTime the object was last modified.</span></span> <span data-ttu-id="6967a-139">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6967a-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6967a-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6967a-140">roleScopeTagIds</span></span>|<span data-ttu-id="6967a-141">String collection</span><span class="sxs-lookup"><span data-stu-id="6967a-141">String collection</span></span>|<span data-ttu-id="6967a-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="6967a-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6967a-143">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6967a-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6967a-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="6967a-144">supportsScopeTags</span></span>|<span data-ttu-id="6967a-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="6967a-145">Boolean</span></span>|<span data-ttu-id="6967a-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="6967a-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6967a-147">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="6967a-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6967a-148">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="6967a-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6967a-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6967a-149">This property is read-only.</span></span> <span data-ttu-id="6967a-150">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6967a-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6967a-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="6967a-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="6967a-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="6967a-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="6967a-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="6967a-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="6967a-154">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6967a-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6967a-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="6967a-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="6967a-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="6967a-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="6967a-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="6967a-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="6967a-158">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6967a-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6967a-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="6967a-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="6967a-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="6967a-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="6967a-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="6967a-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="6967a-162">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6967a-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6967a-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6967a-163">createdDateTime</span></span>|<span data-ttu-id="6967a-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6967a-164">DateTimeOffset</span></span>|<span data-ttu-id="6967a-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="6967a-165">DateTime the object was created.</span></span> <span data-ttu-id="6967a-166">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6967a-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6967a-167">说明</span><span class="sxs-lookup"><span data-stu-id="6967a-167">description</span></span>|<span data-ttu-id="6967a-168">String</span><span class="sxs-lookup"><span data-stu-id="6967a-168">String</span></span>|<span data-ttu-id="6967a-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="6967a-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6967a-170">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6967a-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6967a-171">displayName</span><span class="sxs-lookup"><span data-stu-id="6967a-171">displayName</span></span>|<span data-ttu-id="6967a-172">String</span><span class="sxs-lookup"><span data-stu-id="6967a-172">String</span></span>|<span data-ttu-id="6967a-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="6967a-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6967a-174">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6967a-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6967a-175">version</span><span class="sxs-lookup"><span data-stu-id="6967a-175">version</span></span>|<span data-ttu-id="6967a-176">Int32</span><span class="sxs-lookup"><span data-stu-id="6967a-176">Int32</span></span>|<span data-ttu-id="6967a-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="6967a-177">Version of the device configuration.</span></span> <span data-ttu-id="6967a-178">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6967a-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6967a-179">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="6967a-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="6967a-180">Int32</span><span class="sxs-lookup"><span data-stu-id="6967a-180">Int32</span></span>|<span data-ttu-id="6967a-181">证书续订阈值百分比。</span><span class="sxs-lookup"><span data-stu-id="6967a-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="6967a-182">继承自[macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="6967a-182">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="6967a-183">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="6967a-183">subjectNameFormat</span></span>|[<span data-ttu-id="6967a-184">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="6967a-184">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="6967a-185">证书使用者名称格式。</span><span class="sxs-lookup"><span data-stu-id="6967a-185">Certificate Subject Name Format.</span></span> <span data-ttu-id="6967a-186">继承自[macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="6967a-186">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="6967a-187">可取值为：`commonName`、`commonNameAsEmail`、`custom`、`commonNameIncludingEmail`、`commonNameAsIMEI`、`commonNameAsSerialNumber`。</span><span class="sxs-lookup"><span data-stu-id="6967a-187">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="6967a-188">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="6967a-188">subjectAlternativeNameType</span></span>|[<span data-ttu-id="6967a-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="6967a-189">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="6967a-190">证书使用者备用名称类型。</span><span class="sxs-lookup"><span data-stu-id="6967a-190">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="6967a-191">继承自[macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="6967a-191">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="6967a-192">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService`。</span><span class="sxs-lookup"><span data-stu-id="6967a-192">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="6967a-193">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="6967a-193">certificateValidityPeriodValue</span></span>|<span data-ttu-id="6967a-194">Int32</span><span class="sxs-lookup"><span data-stu-id="6967a-194">Int32</span></span>|<span data-ttu-id="6967a-195">证书有效期限的值。</span><span class="sxs-lookup"><span data-stu-id="6967a-195">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="6967a-196">继承自[macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="6967a-196">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="6967a-197">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="6967a-197">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="6967a-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="6967a-198">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="6967a-199">证书有效期的小数位数。</span><span class="sxs-lookup"><span data-stu-id="6967a-199">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="6967a-200">继承自[macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="6967a-200">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="6967a-201">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="6967a-201">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="6967a-202">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="6967a-202">intendedPurpose</span></span>|[<span data-ttu-id="6967a-203">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="6967a-203">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="6967a-204">尚未记录。</span><span class="sxs-lookup"><span data-stu-id="6967a-204">Not yet documented.</span></span> <span data-ttu-id="6967a-205">可取值为：`unassigned`、`smimeEncryption`、`smimeSigning`、`vpn`、`wifi`。</span><span class="sxs-lookup"><span data-stu-id="6967a-205">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="6967a-206">响应</span><span class="sxs-lookup"><span data-stu-id="6967a-206">Response</span></span>
<span data-ttu-id="6967a-207">如果成功，此方法在响应`201 Created`正文中返回响应代码和[macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6967a-207">If successful, this method returns a `201 Created` response code and a [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6967a-208">示例</span><span class="sxs-lookup"><span data-stu-id="6967a-208">Example</span></span>

### <a name="request"></a><span data-ttu-id="6967a-209">请求</span><span class="sxs-lookup"><span data-stu-id="6967a-209">Request</span></span>
<span data-ttu-id="6967a-210">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6967a-210">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="6967a-211">响应</span><span class="sxs-lookup"><span data-stu-id="6967a-211">Response</span></span>
<span data-ttu-id="6967a-p119">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6967a-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




