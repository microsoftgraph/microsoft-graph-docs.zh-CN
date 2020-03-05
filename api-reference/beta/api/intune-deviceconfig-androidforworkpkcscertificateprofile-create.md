---
title: 创建 androidForWorkPkcsCertificateProfile
description: 创建新的 androidForWorkPkcsCertificateProfile 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 56bf602a56d84b0557a9eb81591bb3231c92f1a9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42443809"
---
# <a name="create-androidforworkpkcscertificateprofile"></a><span data-ttu-id="9f6ce-103">创建 androidForWorkPkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="9f6ce-103">Create androidForWorkPkcsCertificateProfile</span></span>

<span data-ttu-id="9f6ce-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="9f6ce-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9f6ce-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9f6ce-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9f6ce-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9f6ce-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9f6ce-107">创建新的[androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9f6ce-107">Create a new [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9f6ce-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="9f6ce-108">Prerequisites</span></span>
<span data-ttu-id="9f6ce-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9f6ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f6ce-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9f6ce-111">Permission type</span></span>|<span data-ttu-id="9f6ce-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9f6ce-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9f6ce-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9f6ce-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9f6ce-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f6ce-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9f6ce-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9f6ce-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f6ce-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9f6ce-116">Not supported.</span></span>|
|<span data-ttu-id="9f6ce-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9f6ce-117">Application</span></span>|<span data-ttu-id="9f6ce-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f6ce-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9f6ce-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9f6ce-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="9f6ce-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9f6ce-120">Request headers</span></span>
|<span data-ttu-id="9f6ce-121">标头</span><span class="sxs-lookup"><span data-stu-id="9f6ce-121">Header</span></span>|<span data-ttu-id="9f6ce-122">值</span><span class="sxs-lookup"><span data-stu-id="9f6ce-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9f6ce-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f6ce-123">Authorization</span></span>|<span data-ttu-id="9f6ce-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9f6ce-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9f6ce-125">接受</span><span class="sxs-lookup"><span data-stu-id="9f6ce-125">Accept</span></span>|<span data-ttu-id="9f6ce-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9f6ce-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f6ce-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9f6ce-127">Request body</span></span>
<span data-ttu-id="9f6ce-128">在请求正文中，提供 androidForWorkPkcsCertificateProfile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9f6ce-128">In the request body, supply a JSON representation for the androidForWorkPkcsCertificateProfile object.</span></span>

<span data-ttu-id="9f6ce-129">下表显示创建 androidForWorkPkcsCertificateProfile 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="9f6ce-129">The following table shows the properties that are required when you create the androidForWorkPkcsCertificateProfile.</span></span>

|<span data-ttu-id="9f6ce-130">属性</span><span class="sxs-lookup"><span data-stu-id="9f6ce-130">Property</span></span>|<span data-ttu-id="9f6ce-131">类型</span><span class="sxs-lookup"><span data-stu-id="9f6ce-131">Type</span></span>|<span data-ttu-id="9f6ce-132">说明</span><span class="sxs-lookup"><span data-stu-id="9f6ce-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f6ce-133">id</span><span class="sxs-lookup"><span data-stu-id="9f6ce-133">id</span></span>|<span data-ttu-id="9f6ce-134">字符串</span><span class="sxs-lookup"><span data-stu-id="9f6ce-134">String</span></span>|<span data-ttu-id="9f6ce-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="9f6ce-135">Key of the entity.</span></span> <span data-ttu-id="9f6ce-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9f6ce-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f6ce-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9f6ce-137">lastModifiedDateTime</span></span>|<span data-ttu-id="9f6ce-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f6ce-138">DateTimeOffset</span></span>|<span data-ttu-id="9f6ce-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="9f6ce-139">DateTime the object was last modified.</span></span> <span data-ttu-id="9f6ce-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9f6ce-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f6ce-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9f6ce-141">roleScopeTagIds</span></span>|<span data-ttu-id="9f6ce-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="9f6ce-142">String collection</span></span>|<span data-ttu-id="9f6ce-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="9f6ce-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9f6ce-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9f6ce-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f6ce-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="9f6ce-145">supportsScopeTags</span></span>|<span data-ttu-id="9f6ce-146">布尔</span><span class="sxs-lookup"><span data-stu-id="9f6ce-146">Boolean</span></span>|<span data-ttu-id="9f6ce-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="9f6ce-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="9f6ce-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="9f6ce-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="9f6ce-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="9f6ce-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="9f6ce-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9f6ce-150">This property is read-only.</span></span> <span data-ttu-id="9f6ce-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9f6ce-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f6ce-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="9f6ce-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="9f6ce-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="9f6ce-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="9f6ce-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="9f6ce-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="9f6ce-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9f6ce-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f6ce-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="9f6ce-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="9f6ce-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="9f6ce-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="9f6ce-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="9f6ce-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="9f6ce-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9f6ce-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f6ce-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="9f6ce-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="9f6ce-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="9f6ce-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="9f6ce-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="9f6ce-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="9f6ce-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9f6ce-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f6ce-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9f6ce-164">createdDateTime</span></span>|<span data-ttu-id="9f6ce-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f6ce-165">DateTimeOffset</span></span>|<span data-ttu-id="9f6ce-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="9f6ce-166">DateTime the object was created.</span></span> <span data-ttu-id="9f6ce-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9f6ce-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f6ce-168">说明</span><span class="sxs-lookup"><span data-stu-id="9f6ce-168">description</span></span>|<span data-ttu-id="9f6ce-169">String</span><span class="sxs-lookup"><span data-stu-id="9f6ce-169">String</span></span>|<span data-ttu-id="9f6ce-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="9f6ce-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9f6ce-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9f6ce-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f6ce-172">displayName</span><span class="sxs-lookup"><span data-stu-id="9f6ce-172">displayName</span></span>|<span data-ttu-id="9f6ce-173">String</span><span class="sxs-lookup"><span data-stu-id="9f6ce-173">String</span></span>|<span data-ttu-id="9f6ce-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="9f6ce-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9f6ce-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9f6ce-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f6ce-176">version</span><span class="sxs-lookup"><span data-stu-id="9f6ce-176">version</span></span>|<span data-ttu-id="9f6ce-177">Int32</span><span class="sxs-lookup"><span data-stu-id="9f6ce-177">Int32</span></span>|<span data-ttu-id="9f6ce-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="9f6ce-178">Version of the device configuration.</span></span> <span data-ttu-id="9f6ce-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9f6ce-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f6ce-180">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="9f6ce-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="9f6ce-181">Int32</span><span class="sxs-lookup"><span data-stu-id="9f6ce-181">Int32</span></span>|<span data-ttu-id="9f6ce-182">证书续订阈值百分比。</span><span class="sxs-lookup"><span data-stu-id="9f6ce-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="9f6ce-183">从[AndroidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)继承的有效值1到99</span><span class="sxs-lookup"><span data-stu-id="9f6ce-183">Valid values 1 to 99 Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="9f6ce-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="9f6ce-184">subjectNameFormat</span></span>|[<span data-ttu-id="9f6ce-185">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="9f6ce-185">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="9f6ce-186">证书使用者名称格式。</span><span class="sxs-lookup"><span data-stu-id="9f6ce-186">Certificate Subject Name Format.</span></span> <span data-ttu-id="9f6ce-187">继承自[androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="9f6ce-187">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="9f6ce-188">可取值为：`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId`。</span><span class="sxs-lookup"><span data-stu-id="9f6ce-188">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="9f6ce-189">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="9f6ce-189">certificateValidityPeriodValue</span></span>|<span data-ttu-id="9f6ce-190">Int32</span><span class="sxs-lookup"><span data-stu-id="9f6ce-190">Int32</span></span>|<span data-ttu-id="9f6ce-191">证书有效期限的值。</span><span class="sxs-lookup"><span data-stu-id="9f6ce-191">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="9f6ce-192">继承自[androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="9f6ce-192">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="9f6ce-193">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="9f6ce-193">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="9f6ce-194">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="9f6ce-194">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="9f6ce-195">证书有效期的小数位数。</span><span class="sxs-lookup"><span data-stu-id="9f6ce-195">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="9f6ce-196">继承自[androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="9f6ce-196">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="9f6ce-197">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="9f6ce-197">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="9f6ce-198">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="9f6ce-198">extendedKeyUsages</span></span>|<span data-ttu-id="9f6ce-199">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)集合</span><span class="sxs-lookup"><span data-stu-id="9f6ce-199">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="9f6ce-200">扩展密钥用法（EKU）设置。</span><span class="sxs-lookup"><span data-stu-id="9f6ce-200">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="9f6ce-201">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="9f6ce-201">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="9f6ce-202">继承自[androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="9f6ce-202">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="9f6ce-203">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="9f6ce-203">subjectAlternativeNameType</span></span>|[<span data-ttu-id="9f6ce-204">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="9f6ce-204">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="9f6ce-205">证书使用者备用名称类型。</span><span class="sxs-lookup"><span data-stu-id="9f6ce-205">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="9f6ce-206">继承自[androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="9f6ce-206">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="9f6ce-207">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService`。</span><span class="sxs-lookup"><span data-stu-id="9f6ce-207">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="9f6ce-208">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="9f6ce-208">certificationAuthority</span></span>|<span data-ttu-id="9f6ce-209">String</span><span class="sxs-lookup"><span data-stu-id="9f6ce-209">String</span></span>|<span data-ttu-id="9f6ce-210">PKCS 证书颁发机构</span><span class="sxs-lookup"><span data-stu-id="9f6ce-210">PKCS Certification Authority</span></span>|
|<span data-ttu-id="9f6ce-211">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="9f6ce-211">certificationAuthorityName</span></span>|<span data-ttu-id="9f6ce-212">String</span><span class="sxs-lookup"><span data-stu-id="9f6ce-212">String</span></span>|<span data-ttu-id="9f6ce-213">PKCS 证书颁发机构名称</span><span class="sxs-lookup"><span data-stu-id="9f6ce-213">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="9f6ce-214">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="9f6ce-214">certificateTemplateName</span></span>|<span data-ttu-id="9f6ce-215">String</span><span class="sxs-lookup"><span data-stu-id="9f6ce-215">String</span></span>|<span data-ttu-id="9f6ce-216">PKCS 证书模板名称</span><span class="sxs-lookup"><span data-stu-id="9f6ce-216">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="9f6ce-217">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="9f6ce-217">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="9f6ce-218">String</span><span class="sxs-lookup"><span data-stu-id="9f6ce-218">String</span></span>|<span data-ttu-id="9f6ce-219">定义 AAD 属性的自定义字符串。</span><span class="sxs-lookup"><span data-stu-id="9f6ce-219">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="9f6ce-220">响应</span><span class="sxs-lookup"><span data-stu-id="9f6ce-220">Response</span></span>
<span data-ttu-id="9f6ce-221">如果成功，此方法在响应`201 Created`正文中返回响应代码和[androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9f6ce-221">If successful, this method returns a `201 Created` response code and a [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f6ce-222">示例</span><span class="sxs-lookup"><span data-stu-id="9f6ce-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="9f6ce-223">请求</span><span class="sxs-lookup"><span data-stu-id="9f6ce-223">Request</span></span>
<span data-ttu-id="9f6ce-224">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9f6ce-224">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9f6ce-225">响应</span><span class="sxs-lookup"><span data-stu-id="9f6ce-225">Response</span></span>
<span data-ttu-id="9f6ce-p119">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9f6ce-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





