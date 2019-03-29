---
title: 创建 windowsPhone81SCEPCertificateProfile
description: 创建新的 windowsPhone81SCEPCertificateProfile 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 69222d314245f9d25eedcc712bb05441ae7d9a72
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30971526"
---
# <a name="create-windowsphone81scepcertificateprofile"></a><span data-ttu-id="a9b12-103">创建 windowsPhone81SCEPCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="a9b12-103">Create windowsPhone81SCEPCertificateProfile</span></span>

> <span data-ttu-id="a9b12-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a9b12-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a9b12-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a9b12-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a9b12-106">创建新的[windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a9b12-106">Create a new [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a9b12-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="a9b12-107">Prerequisites</span></span>
<span data-ttu-id="a9b12-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a9b12-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9b12-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a9b12-110">Permission type</span></span>|<span data-ttu-id="a9b12-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a9b12-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a9b12-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a9b12-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a9b12-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9b12-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a9b12-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a9b12-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a9b12-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a9b12-115">Not supported.</span></span>|
|<span data-ttu-id="a9b12-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a9b12-116">Application</span></span>|<span data-ttu-id="a9b12-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="a9b12-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a9b12-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a9b12-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a9b12-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a9b12-119">Request headers</span></span>
|<span data-ttu-id="a9b12-120">标头</span><span class="sxs-lookup"><span data-stu-id="a9b12-120">Header</span></span>|<span data-ttu-id="a9b12-121">值</span><span class="sxs-lookup"><span data-stu-id="a9b12-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a9b12-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a9b12-122">Authorization</span></span>|<span data-ttu-id="a9b12-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a9b12-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a9b12-124">接受</span><span class="sxs-lookup"><span data-stu-id="a9b12-124">Accept</span></span>|<span data-ttu-id="a9b12-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a9b12-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a9b12-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a9b12-126">Request body</span></span>
<span data-ttu-id="a9b12-127">在请求正文中, 提供 windowsPhone81SCEPCertificateProfile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a9b12-127">In the request body, supply a JSON representation for the windowsPhone81SCEPCertificateProfile object.</span></span>

<span data-ttu-id="a9b12-128">下表显示创建 windowsPhone81SCEPCertificateProfile 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a9b12-128">The following table shows the properties that are required when you create the windowsPhone81SCEPCertificateProfile.</span></span>

|<span data-ttu-id="a9b12-129">属性</span><span class="sxs-lookup"><span data-stu-id="a9b12-129">Property</span></span>|<span data-ttu-id="a9b12-130">类型</span><span class="sxs-lookup"><span data-stu-id="a9b12-130">Type</span></span>|<span data-ttu-id="a9b12-131">说明</span><span class="sxs-lookup"><span data-stu-id="a9b12-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9b12-132">id</span><span class="sxs-lookup"><span data-stu-id="a9b12-132">id</span></span>|<span data-ttu-id="a9b12-133">String</span><span class="sxs-lookup"><span data-stu-id="a9b12-133">String</span></span>|<span data-ttu-id="a9b12-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a9b12-134">Key of the entity.</span></span> <span data-ttu-id="a9b12-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a9b12-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a9b12-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a9b12-136">lastModifiedDateTime</span></span>|<span data-ttu-id="a9b12-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9b12-137">DateTimeOffset</span></span>|<span data-ttu-id="a9b12-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="a9b12-138">DateTime the object was last modified.</span></span> <span data-ttu-id="a9b12-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a9b12-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a9b12-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a9b12-140">roleScopeTagIds</span></span>|<span data-ttu-id="a9b12-141">String 集合</span><span class="sxs-lookup"><span data-stu-id="a9b12-141">String collection</span></span>|<span data-ttu-id="a9b12-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="a9b12-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a9b12-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a9b12-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a9b12-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a9b12-144">supportsScopeTags</span></span>|<span data-ttu-id="a9b12-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="a9b12-145">Boolean</span></span>|<span data-ttu-id="a9b12-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="a9b12-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a9b12-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="a9b12-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a9b12-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="a9b12-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a9b12-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="a9b12-149">This property is read-only.</span></span> <span data-ttu-id="a9b12-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a9b12-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a9b12-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a9b12-151">createdDateTime</span></span>|<span data-ttu-id="a9b12-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9b12-152">DateTimeOffset</span></span>|<span data-ttu-id="a9b12-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="a9b12-153">DateTime the object was created.</span></span> <span data-ttu-id="a9b12-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a9b12-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a9b12-155">description</span><span class="sxs-lookup"><span data-stu-id="a9b12-155">description</span></span>|<span data-ttu-id="a9b12-156">String</span><span class="sxs-lookup"><span data-stu-id="a9b12-156">String</span></span>|<span data-ttu-id="a9b12-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="a9b12-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a9b12-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a9b12-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a9b12-159">displayName</span><span class="sxs-lookup"><span data-stu-id="a9b12-159">displayName</span></span>|<span data-ttu-id="a9b12-160">String</span><span class="sxs-lookup"><span data-stu-id="a9b12-160">String</span></span>|<span data-ttu-id="a9b12-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="a9b12-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a9b12-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a9b12-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a9b12-163">version</span><span class="sxs-lookup"><span data-stu-id="a9b12-163">version</span></span>|<span data-ttu-id="a9b12-164">Int32</span><span class="sxs-lookup"><span data-stu-id="a9b12-164">Int32</span></span>|<span data-ttu-id="a9b12-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="a9b12-165">Version of the device configuration.</span></span> <span data-ttu-id="a9b12-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a9b12-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a9b12-167">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="a9b12-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="a9b12-168">Int32</span><span class="sxs-lookup"><span data-stu-id="a9b12-168">Int32</span></span>|<span data-ttu-id="a9b12-169">证书续订阈值百分比。</span><span class="sxs-lookup"><span data-stu-id="a9b12-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="a9b12-170">继承自[windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="a9b12-170">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="a9b12-171">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="a9b12-171">keyStorageProvider</span></span>|[<span data-ttu-id="a9b12-172">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="a9b12-172">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="a9b12-173">密钥存储提供程序 (KSP)。</span><span class="sxs-lookup"><span data-stu-id="a9b12-173">Key Storage Provider (KSP).</span></span> <span data-ttu-id="a9b12-174">继承自[windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="a9b12-174">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="a9b12-175">可取值为：`useTpmKspOtherwiseUseSoftwareKsp`、`useTpmKspOtherwiseFail`、`usePassportForWorkKspOtherwiseFail`、`useSoftwareKsp`。</span><span class="sxs-lookup"><span data-stu-id="a9b12-175">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="a9b12-176">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="a9b12-176">subjectNameFormat</span></span>|[<span data-ttu-id="a9b12-177">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="a9b12-177">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="a9b12-178">证书使用者名称格式。</span><span class="sxs-lookup"><span data-stu-id="a9b12-178">Certificate Subject Name Format.</span></span> <span data-ttu-id="a9b12-179">继承自[windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="a9b12-179">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="a9b12-180">可取值为：`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId`。</span><span class="sxs-lookup"><span data-stu-id="a9b12-180">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="a9b12-181">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="a9b12-181">subjectAlternativeNameType</span></span>|[<span data-ttu-id="a9b12-182">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="a9b12-182">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="a9b12-183">证书使用者备用名称类型。</span><span class="sxs-lookup"><span data-stu-id="a9b12-183">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="a9b12-184">继承自[windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="a9b12-184">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="a9b12-185">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute` 或 `domainNameService`。</span><span class="sxs-lookup"><span data-stu-id="a9b12-185">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="a9b12-186">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="a9b12-186">certificateValidityPeriodValue</span></span>|<span data-ttu-id="a9b12-187">Int32</span><span class="sxs-lookup"><span data-stu-id="a9b12-187">Int32</span></span>|<span data-ttu-id="a9b12-188">证书 Validtiy 期限的值。</span><span class="sxs-lookup"><span data-stu-id="a9b12-188">Value for the Certificate Validtiy Period.</span></span> <span data-ttu-id="a9b12-189">继承自[windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="a9b12-189">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="a9b12-190">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="a9b12-190">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="a9b12-191">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="a9b12-191">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="a9b12-192">证书有效期的小数位数。</span><span class="sxs-lookup"><span data-stu-id="a9b12-192">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="a9b12-193">继承自[windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="a9b12-193">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="a9b12-194">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="a9b12-194">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="a9b12-195">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="a9b12-195">extendedKeyUsages</span></span>|<span data-ttu-id="a9b12-196">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)集合</span><span class="sxs-lookup"><span data-stu-id="a9b12-196">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="a9b12-197">扩展密钥用法 (EKU) 设置。</span><span class="sxs-lookup"><span data-stu-id="a9b12-197">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="a9b12-198">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="a9b12-198">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="a9b12-199">继承自[windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="a9b12-199">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="a9b12-200">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="a9b12-200">scepServerUrls</span></span>|<span data-ttu-id="a9b12-201">String 集合</span><span class="sxs-lookup"><span data-stu-id="a9b12-201">String collection</span></span>|<span data-ttu-id="a9b12-202">SCEP 服务器 Url。</span><span class="sxs-lookup"><span data-stu-id="a9b12-202">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="a9b12-203">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="a9b12-203">subjectNameFormatString</span></span>|<span data-ttu-id="a9b12-204">String</span><span class="sxs-lookup"><span data-stu-id="a9b12-204">String</span></span>|<span data-ttu-id="a9b12-205">要与 SubjectNameFormat = custom 一起使用的自定义格式。</span><span class="sxs-lookup"><span data-stu-id="a9b12-205">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="a9b12-206">示例: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = 企业用户, O = Contoso Corporation, L = Redmond, ST = WA, C = US</span><span class="sxs-lookup"><span data-stu-id="a9b12-206">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="a9b12-207">keyUsage</span><span class="sxs-lookup"><span data-stu-id="a9b12-207">keyUsage</span></span>|[<span data-ttu-id="a9b12-208">keyUsages</span><span class="sxs-lookup"><span data-stu-id="a9b12-208">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="a9b12-209">SCEP 密钥用法。</span><span class="sxs-lookup"><span data-stu-id="a9b12-209">SCEP Key Usage.</span></span> <span data-ttu-id="a9b12-210">可取值为：`keyEncipherment`、`digitalSignature`。</span><span class="sxs-lookup"><span data-stu-id="a9b12-210">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="a9b12-211">keySize</span><span class="sxs-lookup"><span data-stu-id="a9b12-211">keySize</span></span>|[<span data-ttu-id="a9b12-212">keySize</span><span class="sxs-lookup"><span data-stu-id="a9b12-212">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="a9b12-213">SCEP 密钥大小。</span><span class="sxs-lookup"><span data-stu-id="a9b12-213">SCEP Key Size.</span></span> <span data-ttu-id="a9b12-214">可取值为：`size1024`、`size2048`。</span><span class="sxs-lookup"><span data-stu-id="a9b12-214">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="a9b12-215">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="a9b12-215">hashAlgorithm</span></span>|[<span data-ttu-id="a9b12-216">hashAlgorithms</span><span class="sxs-lookup"><span data-stu-id="a9b12-216">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="a9b12-217">SCEP 哈希算法。</span><span class="sxs-lookup"><span data-stu-id="a9b12-217">SCEP Hash Algorithm.</span></span> <span data-ttu-id="a9b12-218">可取值为：`sha1`、`sha2`。</span><span class="sxs-lookup"><span data-stu-id="a9b12-218">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="a9b12-219">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="a9b12-219">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="a9b12-220">String</span><span class="sxs-lookup"><span data-stu-id="a9b12-220">String</span></span>|<span data-ttu-id="a9b12-221">定义 AAD 属性的自定义字符串。</span><span class="sxs-lookup"><span data-stu-id="a9b12-221">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="a9b12-222">响应</span><span class="sxs-lookup"><span data-stu-id="a9b12-222">Response</span></span>
<span data-ttu-id="a9b12-223">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a9b12-223">If successful, this method returns a `201 Created` response code and a [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9b12-224">示例</span><span class="sxs-lookup"><span data-stu-id="a9b12-224">Example</span></span>

### <a name="request"></a><span data-ttu-id="a9b12-225">请求</span><span class="sxs-lookup"><span data-stu-id="a9b12-225">Request</span></span>
<span data-ttu-id="a9b12-226">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a9b12-226">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1032

{
  "@odata.type": "#microsoft.graph.windowsPhone81SCEPCertificateProfile",
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

### <a name="response"></a><span data-ttu-id="a9b12-227">响应</span><span class="sxs-lookup"><span data-stu-id="a9b12-227">Response</span></span>
<span data-ttu-id="a9b12-p121">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a9b12-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




