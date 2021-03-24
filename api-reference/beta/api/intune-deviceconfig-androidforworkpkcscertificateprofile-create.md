---
title: 创建 androidForWorkPkcsCertificateProfile
description: 创建新的 androidForWorkPkcsCertificateProfile 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f95f36d6eed71e7b38bdff3e443e71ed3533f607
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51142595"
---
# <a name="create-androidforworkpkcscertificateprofile"></a><span data-ttu-id="de93f-103">创建 androidForWorkPkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="de93f-103">Create androidForWorkPkcsCertificateProfile</span></span>

<span data-ttu-id="de93f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="de93f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="de93f-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="de93f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="de93f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="de93f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="de93f-107">创建新的 [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="de93f-107">Create a new [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="de93f-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="de93f-108">Prerequisites</span></span>
<span data-ttu-id="de93f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="de93f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de93f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="de93f-111">Permission type</span></span>|<span data-ttu-id="de93f-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="de93f-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="de93f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="de93f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="de93f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de93f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="de93f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="de93f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="de93f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="de93f-116">Not supported.</span></span>|
|<span data-ttu-id="de93f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="de93f-117">Application</span></span>|<span data-ttu-id="de93f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de93f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="de93f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="de93f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="de93f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="de93f-120">Request headers</span></span>
|<span data-ttu-id="de93f-121">标头</span><span class="sxs-lookup"><span data-stu-id="de93f-121">Header</span></span>|<span data-ttu-id="de93f-122">值</span><span class="sxs-lookup"><span data-stu-id="de93f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="de93f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="de93f-123">Authorization</span></span>|<span data-ttu-id="de93f-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="de93f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="de93f-125">接受</span><span class="sxs-lookup"><span data-stu-id="de93f-125">Accept</span></span>|<span data-ttu-id="de93f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="de93f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="de93f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="de93f-127">Request body</span></span>
<span data-ttu-id="de93f-128">在请求正文中，提供 androidForWorkPkcsCertificateProfile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="de93f-128">In the request body, supply a JSON representation for the androidForWorkPkcsCertificateProfile object.</span></span>

<span data-ttu-id="de93f-129">下表显示创建 androidForWorkPkcsCertificateProfile 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="de93f-129">The following table shows the properties that are required when you create the androidForWorkPkcsCertificateProfile.</span></span>

|<span data-ttu-id="de93f-130">属性</span><span class="sxs-lookup"><span data-stu-id="de93f-130">Property</span></span>|<span data-ttu-id="de93f-131">类型</span><span class="sxs-lookup"><span data-stu-id="de93f-131">Type</span></span>|<span data-ttu-id="de93f-132">说明</span><span class="sxs-lookup"><span data-stu-id="de93f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de93f-133">id</span><span class="sxs-lookup"><span data-stu-id="de93f-133">id</span></span>|<span data-ttu-id="de93f-134">String</span><span class="sxs-lookup"><span data-stu-id="de93f-134">String</span></span>|<span data-ttu-id="de93f-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="de93f-135">Key of the entity.</span></span> <span data-ttu-id="de93f-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="de93f-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="de93f-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="de93f-137">lastModifiedDateTime</span></span>|<span data-ttu-id="de93f-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de93f-138">DateTimeOffset</span></span>|<span data-ttu-id="de93f-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="de93f-139">DateTime the object was last modified.</span></span> <span data-ttu-id="de93f-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="de93f-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="de93f-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="de93f-141">roleScopeTagIds</span></span>|<span data-ttu-id="de93f-142">String collection</span><span class="sxs-lookup"><span data-stu-id="de93f-142">String collection</span></span>|<span data-ttu-id="de93f-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="de93f-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="de93f-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="de93f-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="de93f-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="de93f-145">supportsScopeTags</span></span>|<span data-ttu-id="de93f-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="de93f-146">Boolean</span></span>|<span data-ttu-id="de93f-147">指示基础设备配置是否支持分配范围标记。</span><span class="sxs-lookup"><span data-stu-id="de93f-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="de93f-148">当此值为 false 且实体对作用域用户不可见时，不允许分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="de93f-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="de93f-149">这适用于在 Silverlight 中创建的旧版策略，可通过在 Azure 门户中删除和重新创建策略来解决。</span><span class="sxs-lookup"><span data-stu-id="de93f-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="de93f-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="de93f-150">This property is read-only.</span></span> <span data-ttu-id="de93f-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="de93f-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="de93f-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="de93f-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="de93f-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="de93f-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="de93f-154">此策略的操作系统版本适用性。</span><span class="sxs-lookup"><span data-stu-id="de93f-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="de93f-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="de93f-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="de93f-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="de93f-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="de93f-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="de93f-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="de93f-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="de93f-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="de93f-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="de93f-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="de93f-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="de93f-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="de93f-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="de93f-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="de93f-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="de93f-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="de93f-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="de93f-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="de93f-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="de93f-164">createdDateTime</span></span>|<span data-ttu-id="de93f-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de93f-165">DateTimeOffset</span></span>|<span data-ttu-id="de93f-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="de93f-166">DateTime the object was created.</span></span> <span data-ttu-id="de93f-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="de93f-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="de93f-168">说明</span><span class="sxs-lookup"><span data-stu-id="de93f-168">description</span></span>|<span data-ttu-id="de93f-169">String</span><span class="sxs-lookup"><span data-stu-id="de93f-169">String</span></span>|<span data-ttu-id="de93f-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="de93f-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="de93f-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="de93f-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="de93f-172">displayName</span><span class="sxs-lookup"><span data-stu-id="de93f-172">displayName</span></span>|<span data-ttu-id="de93f-173">String</span><span class="sxs-lookup"><span data-stu-id="de93f-173">String</span></span>|<span data-ttu-id="de93f-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="de93f-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="de93f-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="de93f-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="de93f-176">version</span><span class="sxs-lookup"><span data-stu-id="de93f-176">version</span></span>|<span data-ttu-id="de93f-177">Int32</span><span class="sxs-lookup"><span data-stu-id="de93f-177">Int32</span></span>|<span data-ttu-id="de93f-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="de93f-178">Version of the device configuration.</span></span> <span data-ttu-id="de93f-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="de93f-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="de93f-180">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="de93f-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="de93f-181">Int32</span><span class="sxs-lookup"><span data-stu-id="de93f-181">Int32</span></span>|<span data-ttu-id="de93f-182">证书续订阈值百分比。</span><span class="sxs-lookup"><span data-stu-id="de93f-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="de93f-183">有效值 1 到 99 继承自 [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="de93f-183">Valid values 1 to 99 Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="de93f-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="de93f-184">subjectNameFormat</span></span>|[<span data-ttu-id="de93f-185">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="de93f-185">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="de93f-186">证书主题名称格式。</span><span class="sxs-lookup"><span data-stu-id="de93f-186">Certificate Subject Name Format.</span></span> <span data-ttu-id="de93f-187">继承自 [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="de93f-187">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="de93f-188">可取值为：`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId`。</span><span class="sxs-lookup"><span data-stu-id="de93f-188">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="de93f-189">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="de93f-189">certificateValidityPeriodValue</span></span>|<span data-ttu-id="de93f-190">Int32</span><span class="sxs-lookup"><span data-stu-id="de93f-190">Int32</span></span>|<span data-ttu-id="de93f-191">证书有效期的值。</span><span class="sxs-lookup"><span data-stu-id="de93f-191">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="de93f-192">继承自 [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="de93f-192">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="de93f-193">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="de93f-193">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="de93f-194">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="de93f-194">certificateValidityPeriodScale</span></span>](../resources/intune-shared-certificatevalidityperiodscale.md)|<span data-ttu-id="de93f-195">证书有效期的缩放。</span><span class="sxs-lookup"><span data-stu-id="de93f-195">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="de93f-196">继承自 [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="de93f-196">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="de93f-197">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="de93f-197">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="de93f-198">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="de93f-198">extendedKeyUsages</span></span>|<span data-ttu-id="de93f-199">[extendedKeyUsage](../resources/intune-shared-extendedkeyusage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="de93f-199">[extendedKeyUsage](../resources/intune-shared-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="de93f-200">EKU (扩展密钥) 设置。</span><span class="sxs-lookup"><span data-stu-id="de93f-200">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="de93f-201">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="de93f-201">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="de93f-202">继承自 [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="de93f-202">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="de93f-203">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="de93f-203">subjectAlternativeNameType</span></span>|[<span data-ttu-id="de93f-204">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="de93f-204">subjectAlternativeNameType</span></span>](../resources/intune-shared-subjectalternativenametype.md)|<span data-ttu-id="de93f-205">证书主题备用名称类型。</span><span class="sxs-lookup"><span data-stu-id="de93f-205">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="de93f-206">继承自 [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="de93f-206">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="de93f-207">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService`、`universalResourceIdentifier`。</span><span class="sxs-lookup"><span data-stu-id="de93f-207">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span></span>|
|<span data-ttu-id="de93f-208">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="de93f-208">certificationAuthority</span></span>|<span data-ttu-id="de93f-209">String</span><span class="sxs-lookup"><span data-stu-id="de93f-209">String</span></span>|<span data-ttu-id="de93f-210">PKCS 证书颁发机构</span><span class="sxs-lookup"><span data-stu-id="de93f-210">PKCS Certification Authority</span></span>|
|<span data-ttu-id="de93f-211">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="de93f-211">certificationAuthorityName</span></span>|<span data-ttu-id="de93f-212">String</span><span class="sxs-lookup"><span data-stu-id="de93f-212">String</span></span>|<span data-ttu-id="de93f-213">PKCS 证书颁发机构名称</span><span class="sxs-lookup"><span data-stu-id="de93f-213">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="de93f-214">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="de93f-214">certificateTemplateName</span></span>|<span data-ttu-id="de93f-215">String</span><span class="sxs-lookup"><span data-stu-id="de93f-215">String</span></span>|<span data-ttu-id="de93f-216">PKCS 证书模板名称</span><span class="sxs-lookup"><span data-stu-id="de93f-216">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="de93f-217">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="de93f-217">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="de93f-218">String</span><span class="sxs-lookup"><span data-stu-id="de93f-218">String</span></span>|<span data-ttu-id="de93f-219">定义 AAD 属性的自定义字符串。</span><span class="sxs-lookup"><span data-stu-id="de93f-219">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="de93f-220">响应</span><span class="sxs-lookup"><span data-stu-id="de93f-220">Response</span></span>
<span data-ttu-id="de93f-221">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="de93f-221">If successful, this method returns a `201 Created` response code and a [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de93f-222">示例</span><span class="sxs-lookup"><span data-stu-id="de93f-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="de93f-223">请求</span><span class="sxs-lookup"><span data-stu-id="de93f-223">Request</span></span>
<span data-ttu-id="de93f-224">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="de93f-224">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="de93f-225">响应</span><span class="sxs-lookup"><span data-stu-id="de93f-225">Response</span></span>
<span data-ttu-id="de93f-p119">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="de93f-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




