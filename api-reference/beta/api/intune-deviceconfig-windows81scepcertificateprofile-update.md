---
title: 更新 windows81SCEPCertificateProfile
description: 更新 windows81SCEPCertificateProfile 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 1f39c9571db6834abfcaa221eda2269c02a3ee4a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27809392"
---
# <a name="update-windows81scepcertificateprofile"></a><span data-ttu-id="d1cb6-103">更新 windows81SCEPCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="d1cb6-103">Update windows81SCEPCertificateProfile</span></span>

> <span data-ttu-id="d1cb6-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d1cb6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d1cb6-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d1cb6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d1cb6-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d1cb6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d1cb6-107">更新[windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d1cb6-107">Update the properties of a [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d1cb6-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="d1cb6-108">Prerequisites</span></span>
<span data-ttu-id="d1cb6-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="d1cb6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1cb6-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d1cb6-111">Permission type</span></span>|<span data-ttu-id="d1cb6-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d1cb6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d1cb6-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d1cb6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d1cb6-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1cb6-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d1cb6-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d1cb6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d1cb6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d1cb6-116">Not supported.</span></span>|
|<span data-ttu-id="d1cb6-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d1cb6-117">Application</span></span>|<span data-ttu-id="d1cb6-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="d1cb6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d1cb6-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d1cb6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="d1cb6-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d1cb6-120">Request headers</span></span>
|<span data-ttu-id="d1cb6-121">标头</span><span class="sxs-lookup"><span data-stu-id="d1cb6-121">Header</span></span>|<span data-ttu-id="d1cb6-122">值</span><span class="sxs-lookup"><span data-stu-id="d1cb6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d1cb6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d1cb6-123">Authorization</span></span>|<span data-ttu-id="d1cb6-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d1cb6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d1cb6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d1cb6-125">Accept</span></span>|<span data-ttu-id="d1cb6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d1cb6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d1cb6-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d1cb6-127">Request body</span></span>
<span data-ttu-id="d1cb6-128">在请求正文中，提供[windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d1cb6-128">In the request body, supply a JSON representation for the [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) object.</span></span>

<span data-ttu-id="d1cb6-129">下表显示时创建[windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d1cb6-129">The following table shows the properties that are required when you create the [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md).</span></span>

|<span data-ttu-id="d1cb6-130">属性</span><span class="sxs-lookup"><span data-stu-id="d1cb6-130">Property</span></span>|<span data-ttu-id="d1cb6-131">类型</span><span class="sxs-lookup"><span data-stu-id="d1cb6-131">Type</span></span>|<span data-ttu-id="d1cb6-132">说明</span><span class="sxs-lookup"><span data-stu-id="d1cb6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1cb6-133">id</span><span class="sxs-lookup"><span data-stu-id="d1cb6-133">id</span></span>|<span data-ttu-id="d1cb6-134">String</span><span class="sxs-lookup"><span data-stu-id="d1cb6-134">String</span></span>|<span data-ttu-id="d1cb6-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d1cb6-135">Key of the entity.</span></span> <span data-ttu-id="d1cb6-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1cb6-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d1cb6-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d1cb6-137">lastModifiedDateTime</span></span>|<span data-ttu-id="d1cb6-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d1cb6-138">DateTimeOffset</span></span>|<span data-ttu-id="d1cb6-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="d1cb6-139">DateTime the object was last modified.</span></span> <span data-ttu-id="d1cb6-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1cb6-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d1cb6-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d1cb6-141">roleScopeTagIds</span></span>|<span data-ttu-id="d1cb6-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="d1cb6-142">String collection</span></span>|<span data-ttu-id="d1cb6-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="d1cb6-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d1cb6-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1cb6-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d1cb6-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d1cb6-145">supportsScopeTags</span></span>|<span data-ttu-id="d1cb6-146">布尔</span><span class="sxs-lookup"><span data-stu-id="d1cb6-146">Boolean</span></span>|<span data-ttu-id="d1cb6-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="d1cb6-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d1cb6-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="d1cb6-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d1cb6-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="d1cb6-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d1cb6-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="d1cb6-150">This property is read-only.</span></span> <span data-ttu-id="d1cb6-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1cb6-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d1cb6-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d1cb6-152">createdDateTime</span></span>|<span data-ttu-id="d1cb6-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d1cb6-153">DateTimeOffset</span></span>|<span data-ttu-id="d1cb6-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="d1cb6-154">DateTime the object was created.</span></span> <span data-ttu-id="d1cb6-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1cb6-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d1cb6-156">description</span><span class="sxs-lookup"><span data-stu-id="d1cb6-156">description</span></span>|<span data-ttu-id="d1cb6-157">String</span><span class="sxs-lookup"><span data-stu-id="d1cb6-157">String</span></span>|<span data-ttu-id="d1cb6-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="d1cb6-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d1cb6-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1cb6-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d1cb6-160">displayName</span><span class="sxs-lookup"><span data-stu-id="d1cb6-160">displayName</span></span>|<span data-ttu-id="d1cb6-161">String</span><span class="sxs-lookup"><span data-stu-id="d1cb6-161">String</span></span>|<span data-ttu-id="d1cb6-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="d1cb6-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d1cb6-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1cb6-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d1cb6-164">version</span><span class="sxs-lookup"><span data-stu-id="d1cb6-164">version</span></span>|<span data-ttu-id="d1cb6-165">Int32</span><span class="sxs-lookup"><span data-stu-id="d1cb6-165">Int32</span></span>|<span data-ttu-id="d1cb6-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="d1cb6-166">Version of the device configuration.</span></span> <span data-ttu-id="d1cb6-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1cb6-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d1cb6-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="d1cb6-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="d1cb6-169">Int32</span><span class="sxs-lookup"><span data-stu-id="d1cb6-169">Int32</span></span>|<span data-ttu-id="d1cb6-170">证书续订阈值百分比。</span><span class="sxs-lookup"><span data-stu-id="d1cb6-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="d1cb6-171">有效值 1 到 99 继承自[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="d1cb6-171">Valid values 1 to 99 Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="d1cb6-172">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="d1cb6-172">keyStorageProvider</span></span>|[<span data-ttu-id="d1cb6-173">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="d1cb6-173">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="d1cb6-174">从[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)键存储提供程序 (KSP) 继承。</span><span class="sxs-lookup"><span data-stu-id="d1cb6-174">Key Storage Provider (KSP) Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="d1cb6-175">可取值为：`useTpmKspOtherwiseUseSoftwareKsp`、`useTpmKspOtherwiseFail`、`usePassportForWorkKspOtherwiseFail`、`useSoftwareKsp`。</span><span class="sxs-lookup"><span data-stu-id="d1cb6-175">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="d1cb6-176">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="d1cb6-176">subjectNameFormat</span></span>|[<span data-ttu-id="d1cb6-177">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="d1cb6-177">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="d1cb6-178">证书使用者名称格式继承自[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="d1cb6-178">Certificate Subject Name Format Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="d1cb6-179">可取值为：`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId`。</span><span class="sxs-lookup"><span data-stu-id="d1cb6-179">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="d1cb6-180">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="d1cb6-180">subjectAlternativeNameType</span></span>|[<span data-ttu-id="d1cb6-181">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="d1cb6-181">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="d1cb6-182">证书使用者替代名称类型继承自[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="d1cb6-182">Certificate Subject Alternative Name Type Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="d1cb6-183">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService`。</span><span class="sxs-lookup"><span data-stu-id="d1cb6-183">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="d1cb6-184">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="d1cb6-184">certificateValidityPeriodValue</span></span>|<span data-ttu-id="d1cb6-185">Int32</span><span class="sxs-lookup"><span data-stu-id="d1cb6-185">Int32</span></span>|<span data-ttu-id="d1cb6-186">证书有效性段继承自[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)值</span><span class="sxs-lookup"><span data-stu-id="d1cb6-186">Value for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="d1cb6-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="d1cb6-187">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="d1cb6-188">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="d1cb6-188">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="d1cb6-189">证书有效性段继承自[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)的小数位数。</span><span class="sxs-lookup"><span data-stu-id="d1cb6-189">Scale for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="d1cb6-190">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="d1cb6-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="d1cb6-191">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="d1cb6-191">extendedKeyUsages</span></span>|<span data-ttu-id="d1cb6-192">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)集合</span><span class="sxs-lookup"><span data-stu-id="d1cb6-192">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="d1cb6-193">扩展的密钥用法 (EKU) 设置。</span><span class="sxs-lookup"><span data-stu-id="d1cb6-193">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="d1cb6-194">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="d1cb6-194">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="d1cb6-195">继承自[windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="d1cb6-195">Inherited from [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="d1cb6-196">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="d1cb6-196">customSubjectAlternativeNames</span></span>|<span data-ttu-id="d1cb6-197">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)集合</span><span class="sxs-lookup"><span data-stu-id="d1cb6-197">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="d1cb6-198">自定义主题 Alterantive 名称设置。</span><span class="sxs-lookup"><span data-stu-id="d1cb6-198">Custom Subject Alterantive Name Settings.</span></span> <span data-ttu-id="d1cb6-199">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="d1cb6-199">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="d1cb6-200">继承自[windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="d1cb6-200">Inherited from [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="d1cb6-201">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="d1cb6-201">scepServerUrls</span></span>|<span data-ttu-id="d1cb6-202">String 集合</span><span class="sxs-lookup"><span data-stu-id="d1cb6-202">String collection</span></span>|<span data-ttu-id="d1cb6-203">SCEP 服务器 Url(s)。</span><span class="sxs-lookup"><span data-stu-id="d1cb6-203">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="d1cb6-204">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="d1cb6-204">subjectNameFormatString</span></span>|<span data-ttu-id="d1cb6-205">字符串</span><span class="sxs-lookup"><span data-stu-id="d1cb6-205">String</span></span>|<span data-ttu-id="d1cb6-206">自定义格式使用 SubjectNameFormat = 自定义。</span><span class="sxs-lookup"><span data-stu-id="d1cb6-206">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="d1cb6-207">示例： CN = {{EmailAddress}} E = {{EmailAddress}}，OU = 企业用户，O = Contoso Corporation L = 雷德蒙德，ST = WA，C = US</span><span class="sxs-lookup"><span data-stu-id="d1cb6-207">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="d1cb6-208">keyUsage</span><span class="sxs-lookup"><span data-stu-id="d1cb6-208">keyUsage</span></span>|[<span data-ttu-id="d1cb6-209">keyUsages</span><span class="sxs-lookup"><span data-stu-id="d1cb6-209">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="d1cb6-210">SCEP 密钥用法。</span><span class="sxs-lookup"><span data-stu-id="d1cb6-210">SCEP Key Usage.</span></span> <span data-ttu-id="d1cb6-211">可取值为：`keyEncipherment`、`digitalSignature`。</span><span class="sxs-lookup"><span data-stu-id="d1cb6-211">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="d1cb6-212">keySize</span><span class="sxs-lookup"><span data-stu-id="d1cb6-212">keySize</span></span>|[<span data-ttu-id="d1cb6-213">keySize</span><span class="sxs-lookup"><span data-stu-id="d1cb6-213">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="d1cb6-214">SCEP 密钥大小。</span><span class="sxs-lookup"><span data-stu-id="d1cb6-214">SCEP Key Size.</span></span> <span data-ttu-id="d1cb6-215">可取值为：`size1024`、`size2048`。</span><span class="sxs-lookup"><span data-stu-id="d1cb6-215">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="d1cb6-216">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="d1cb6-216">hashAlgorithm</span></span>|[<span data-ttu-id="d1cb6-217">hashAlgorithms</span><span class="sxs-lookup"><span data-stu-id="d1cb6-217">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="d1cb6-218">SCEP 哈希算法。</span><span class="sxs-lookup"><span data-stu-id="d1cb6-218">SCEP Hash Algorithm.</span></span> <span data-ttu-id="d1cb6-219">可取值为：`sha1`、`sha2`。</span><span class="sxs-lookup"><span data-stu-id="d1cb6-219">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="d1cb6-220">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="d1cb6-220">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="d1cb6-221">字符串</span><span class="sxs-lookup"><span data-stu-id="d1cb6-221">String</span></span>|<span data-ttu-id="d1cb6-222">定义 AAD 属性的自定义字符串。</span><span class="sxs-lookup"><span data-stu-id="d1cb6-222">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="d1cb6-223">certificateStore</span><span class="sxs-lookup"><span data-stu-id="d1cb6-223">certificateStore</span></span>|[<span data-ttu-id="d1cb6-224">certificateStore</span><span class="sxs-lookup"><span data-stu-id="d1cb6-224">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="d1cb6-225">目标存储证书。</span><span class="sxs-lookup"><span data-stu-id="d1cb6-225">Target store certificate.</span></span> <span data-ttu-id="d1cb6-226">可取值为：`user`、`machine`。</span><span class="sxs-lookup"><span data-stu-id="d1cb6-226">Possible values are: `user`, `machine`.</span></span>|



## <a name="response"></a><span data-ttu-id="d1cb6-227">响应</span><span class="sxs-lookup"><span data-stu-id="d1cb6-227">Response</span></span>
<span data-ttu-id="d1cb6-228">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d1cb6-228">If successful, this method returns a `200 OK` response code and an updated [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1cb6-229">示例</span><span class="sxs-lookup"><span data-stu-id="d1cb6-229">Example</span></span>
### <a name="request"></a><span data-ttu-id="d1cb6-230">请求</span><span class="sxs-lookup"><span data-stu-id="d1cb6-230">Request</span></span>
<span data-ttu-id="d1cb6-231">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d1cb6-231">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1245

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "renewalThresholdPercentage": 10,
  "keyStorageProvider": "useTpmKspOtherwiseFail",
  "subjectNameFormat": "commonNameIncludingEmail",
  "subjectAlternativeNameType": "emailAddress",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "customSubjectAlternativeNames": [
    {
      "@odata.type": "microsoft.graph.customSubjectAlternativeName",
      "sanType": "emailAddress",
      "name": "Name value"
    }
  ],
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "certificateStore": "machine"
}
```

### <a name="response"></a><span data-ttu-id="d1cb6-232">响应</span><span class="sxs-lookup"><span data-stu-id="d1cb6-232">Response</span></span>
<span data-ttu-id="d1cb6-p123">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d1cb6-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1423

{
  "@odata.type": "#microsoft.graph.windows81SCEPCertificateProfile",
  "id": "2daf8af2-8af2-2daf-f28a-af2df28aaf2d",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "renewalThresholdPercentage": 10,
  "keyStorageProvider": "useTpmKspOtherwiseFail",
  "subjectNameFormat": "commonNameIncludingEmail",
  "subjectAlternativeNameType": "emailAddress",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "customSubjectAlternativeNames": [
    {
      "@odata.type": "microsoft.graph.customSubjectAlternativeName",
      "sanType": "emailAddress",
      "name": "Name value"
    }
  ],
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "certificateStore": "machine"
}
```





