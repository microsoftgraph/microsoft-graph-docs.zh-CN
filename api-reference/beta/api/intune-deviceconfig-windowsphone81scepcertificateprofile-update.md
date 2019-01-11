---
title: 更新 windowsPhone81SCEPCertificateProfile
description: 更新 windowsPhone81SCEPCertificateProfile 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ffa02d096b5a493cc64acb53764fb992afcd20ed
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27806767"
---
# <a name="update-windowsphone81scepcertificateprofile"></a><span data-ttu-id="f37fe-103">更新 windowsPhone81SCEPCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="f37fe-103">Update windowsPhone81SCEPCertificateProfile</span></span>

> <span data-ttu-id="f37fe-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f37fe-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f37fe-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f37fe-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f37fe-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f37fe-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f37fe-107">更新[windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f37fe-107">Update the properties of a [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f37fe-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="f37fe-108">Prerequisites</span></span>
<span data-ttu-id="f37fe-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="f37fe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f37fe-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f37fe-111">Permission type</span></span>|<span data-ttu-id="f37fe-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f37fe-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f37fe-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f37fe-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f37fe-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f37fe-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f37fe-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f37fe-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f37fe-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f37fe-116">Not supported.</span></span>|
|<span data-ttu-id="f37fe-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f37fe-117">Application</span></span>|<span data-ttu-id="f37fe-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="f37fe-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f37fe-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f37fe-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="f37fe-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f37fe-120">Request headers</span></span>
|<span data-ttu-id="f37fe-121">标头</span><span class="sxs-lookup"><span data-stu-id="f37fe-121">Header</span></span>|<span data-ttu-id="f37fe-122">值</span><span class="sxs-lookup"><span data-stu-id="f37fe-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f37fe-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f37fe-123">Authorization</span></span>|<span data-ttu-id="f37fe-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f37fe-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f37fe-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f37fe-125">Accept</span></span>|<span data-ttu-id="f37fe-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f37fe-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f37fe-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f37fe-127">Request body</span></span>
<span data-ttu-id="f37fe-128">在请求正文中，提供[windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f37fe-128">In the request body, supply a JSON representation for the [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) object.</span></span>

<span data-ttu-id="f37fe-129">下表显示时创建[windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f37fe-129">The following table shows the properties that are required when you create the [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md).</span></span>

|<span data-ttu-id="f37fe-130">属性</span><span class="sxs-lookup"><span data-stu-id="f37fe-130">Property</span></span>|<span data-ttu-id="f37fe-131">类型</span><span class="sxs-lookup"><span data-stu-id="f37fe-131">Type</span></span>|<span data-ttu-id="f37fe-132">说明</span><span class="sxs-lookup"><span data-stu-id="f37fe-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f37fe-133">id</span><span class="sxs-lookup"><span data-stu-id="f37fe-133">id</span></span>|<span data-ttu-id="f37fe-134">String</span><span class="sxs-lookup"><span data-stu-id="f37fe-134">String</span></span>|<span data-ttu-id="f37fe-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f37fe-135">Key of the entity.</span></span> <span data-ttu-id="f37fe-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f37fe-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f37fe-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f37fe-137">lastModifiedDateTime</span></span>|<span data-ttu-id="f37fe-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f37fe-138">DateTimeOffset</span></span>|<span data-ttu-id="f37fe-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f37fe-139">DateTime the object was last modified.</span></span> <span data-ttu-id="f37fe-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f37fe-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f37fe-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f37fe-141">roleScopeTagIds</span></span>|<span data-ttu-id="f37fe-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="f37fe-142">String collection</span></span>|<span data-ttu-id="f37fe-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="f37fe-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f37fe-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f37fe-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f37fe-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f37fe-145">supportsScopeTags</span></span>|<span data-ttu-id="f37fe-146">布尔</span><span class="sxs-lookup"><span data-stu-id="f37fe-146">Boolean</span></span>|<span data-ttu-id="f37fe-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="f37fe-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f37fe-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="f37fe-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f37fe-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="f37fe-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f37fe-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="f37fe-150">This property is read-only.</span></span> <span data-ttu-id="f37fe-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f37fe-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f37fe-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f37fe-152">createdDateTime</span></span>|<span data-ttu-id="f37fe-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f37fe-153">DateTimeOffset</span></span>|<span data-ttu-id="f37fe-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f37fe-154">DateTime the object was created.</span></span> <span data-ttu-id="f37fe-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f37fe-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f37fe-156">description</span><span class="sxs-lookup"><span data-stu-id="f37fe-156">description</span></span>|<span data-ttu-id="f37fe-157">String</span><span class="sxs-lookup"><span data-stu-id="f37fe-157">String</span></span>|<span data-ttu-id="f37fe-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="f37fe-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f37fe-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f37fe-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f37fe-160">displayName</span><span class="sxs-lookup"><span data-stu-id="f37fe-160">displayName</span></span>|<span data-ttu-id="f37fe-161">String</span><span class="sxs-lookup"><span data-stu-id="f37fe-161">String</span></span>|<span data-ttu-id="f37fe-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="f37fe-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f37fe-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f37fe-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f37fe-164">version</span><span class="sxs-lookup"><span data-stu-id="f37fe-164">version</span></span>|<span data-ttu-id="f37fe-165">Int32</span><span class="sxs-lookup"><span data-stu-id="f37fe-165">Int32</span></span>|<span data-ttu-id="f37fe-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="f37fe-166">Version of the device configuration.</span></span> <span data-ttu-id="f37fe-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f37fe-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f37fe-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="f37fe-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="f37fe-169">Int32</span><span class="sxs-lookup"><span data-stu-id="f37fe-169">Int32</span></span>|<span data-ttu-id="f37fe-170">证书续订阈值百分比。</span><span class="sxs-lookup"><span data-stu-id="f37fe-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="f37fe-171">继承自[windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="f37fe-171">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="f37fe-172">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="f37fe-172">keyStorageProvider</span></span>|[<span data-ttu-id="f37fe-173">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="f37fe-173">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="f37fe-174">密钥存储提供程序 (KSP)。</span><span class="sxs-lookup"><span data-stu-id="f37fe-174">Key Storage Provider (KSP).</span></span> <span data-ttu-id="f37fe-175">继承自[windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="f37fe-175">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="f37fe-176">可取值为：`useTpmKspOtherwiseUseSoftwareKsp`、`useTpmKspOtherwiseFail`、`usePassportForWorkKspOtherwiseFail`、`useSoftwareKsp`。</span><span class="sxs-lookup"><span data-stu-id="f37fe-176">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="f37fe-177">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="f37fe-177">subjectNameFormat</span></span>|[<span data-ttu-id="f37fe-178">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="f37fe-178">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="f37fe-179">证书使用者名称格式。</span><span class="sxs-lookup"><span data-stu-id="f37fe-179">Certificate Subject Name Format.</span></span> <span data-ttu-id="f37fe-180">继承自[windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="f37fe-180">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="f37fe-181">可取值为：`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId`。</span><span class="sxs-lookup"><span data-stu-id="f37fe-181">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="f37fe-182">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="f37fe-182">subjectAlternativeNameType</span></span>|[<span data-ttu-id="f37fe-183">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="f37fe-183">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="f37fe-184">证书使用者替代名称类型。</span><span class="sxs-lookup"><span data-stu-id="f37fe-184">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="f37fe-185">继承自[windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="f37fe-185">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="f37fe-186">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService`。</span><span class="sxs-lookup"><span data-stu-id="f37fe-186">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="f37fe-187">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="f37fe-187">certificateValidityPeriodValue</span></span>|<span data-ttu-id="f37fe-188">Int32</span><span class="sxs-lookup"><span data-stu-id="f37fe-188">Int32</span></span>|<span data-ttu-id="f37fe-189">证书 Validtiy 时段的值。</span><span class="sxs-lookup"><span data-stu-id="f37fe-189">Value for the Certificate Validtiy Period.</span></span> <span data-ttu-id="f37fe-190">继承自[windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="f37fe-190">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="f37fe-191">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="f37fe-191">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="f37fe-192">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="f37fe-192">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="f37fe-193">证书有效期限的小数位数。</span><span class="sxs-lookup"><span data-stu-id="f37fe-193">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="f37fe-194">继承自[windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="f37fe-194">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="f37fe-195">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="f37fe-195">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="f37fe-196">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="f37fe-196">extendedKeyUsages</span></span>|<span data-ttu-id="f37fe-197">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)集合</span><span class="sxs-lookup"><span data-stu-id="f37fe-197">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="f37fe-198">扩展的密钥用法 (EKU) 设置。</span><span class="sxs-lookup"><span data-stu-id="f37fe-198">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="f37fe-199">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="f37fe-199">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="f37fe-200">继承自[windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="f37fe-200">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="f37fe-201">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="f37fe-201">scepServerUrls</span></span>|<span data-ttu-id="f37fe-202">String 集合</span><span class="sxs-lookup"><span data-stu-id="f37fe-202">String collection</span></span>|<span data-ttu-id="f37fe-203">SCEP 服务器 Url(s)。</span><span class="sxs-lookup"><span data-stu-id="f37fe-203">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="f37fe-204">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="f37fe-204">subjectNameFormatString</span></span>|<span data-ttu-id="f37fe-205">字符串</span><span class="sxs-lookup"><span data-stu-id="f37fe-205">String</span></span>|<span data-ttu-id="f37fe-206">自定义格式使用 SubjectNameFormat = 自定义。</span><span class="sxs-lookup"><span data-stu-id="f37fe-206">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="f37fe-207">示例： CN = {{EmailAddress}} E = {{EmailAddress}}，OU = 企业用户，O = Contoso Corporation L = 雷德蒙德，ST = WA，C = US</span><span class="sxs-lookup"><span data-stu-id="f37fe-207">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="f37fe-208">keyUsage</span><span class="sxs-lookup"><span data-stu-id="f37fe-208">keyUsage</span></span>|[<span data-ttu-id="f37fe-209">keyUsages</span><span class="sxs-lookup"><span data-stu-id="f37fe-209">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="f37fe-210">SCEP 密钥用法。</span><span class="sxs-lookup"><span data-stu-id="f37fe-210">SCEP Key Usage.</span></span> <span data-ttu-id="f37fe-211">可取值为：`keyEncipherment`、`digitalSignature`。</span><span class="sxs-lookup"><span data-stu-id="f37fe-211">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="f37fe-212">keySize</span><span class="sxs-lookup"><span data-stu-id="f37fe-212">keySize</span></span>|[<span data-ttu-id="f37fe-213">keySize</span><span class="sxs-lookup"><span data-stu-id="f37fe-213">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="f37fe-214">SCEP 密钥大小。</span><span class="sxs-lookup"><span data-stu-id="f37fe-214">SCEP Key Size.</span></span> <span data-ttu-id="f37fe-215">可取值为：`size1024`、`size2048`。</span><span class="sxs-lookup"><span data-stu-id="f37fe-215">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="f37fe-216">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="f37fe-216">hashAlgorithm</span></span>|[<span data-ttu-id="f37fe-217">hashAlgorithms</span><span class="sxs-lookup"><span data-stu-id="f37fe-217">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="f37fe-218">SCEP 哈希算法。</span><span class="sxs-lookup"><span data-stu-id="f37fe-218">SCEP Hash Algorithm.</span></span> <span data-ttu-id="f37fe-219">可取值为：`sha1`、`sha2`。</span><span class="sxs-lookup"><span data-stu-id="f37fe-219">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="f37fe-220">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="f37fe-220">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="f37fe-221">字符串</span><span class="sxs-lookup"><span data-stu-id="f37fe-221">String</span></span>|<span data-ttu-id="f37fe-222">定义 AAD 属性的自定义字符串。</span><span class="sxs-lookup"><span data-stu-id="f37fe-222">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="f37fe-223">响应</span><span class="sxs-lookup"><span data-stu-id="f37fe-223">Response</span></span>
<span data-ttu-id="f37fe-224">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f37fe-224">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f37fe-225">示例</span><span class="sxs-lookup"><span data-stu-id="f37fe-225">Example</span></span>
### <a name="request"></a><span data-ttu-id="f37fe-226">请求</span><span class="sxs-lookup"><span data-stu-id="f37fe-226">Request</span></span>
<span data-ttu-id="f37fe-227">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f37fe-227">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1021

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
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```

### <a name="response"></a><span data-ttu-id="f37fe-228">响应</span><span class="sxs-lookup"><span data-stu-id="f37fe-228">Response</span></span>
<span data-ttu-id="f37fe-p122">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f37fe-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1204

{
  "@odata.type": "#microsoft.graph.windowsPhone81SCEPCertificateProfile",
  "id": "f070e30e-e30e-f070-0ee3-70f00ee370f0",
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
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```





