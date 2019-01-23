---
title: 更新 windowsPhone81SCEPCertificateProfile
description: 更新 windowsPhone81SCEPCertificateProfile 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e41cd55846cf5a87bfa8b43aaef31e6a7b1eb245
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404692"
---
# <a name="update-windowsphone81scepcertificateprofile"></a><span data-ttu-id="f8294-103">更新 windowsPhone81SCEPCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="f8294-103">Update windowsPhone81SCEPCertificateProfile</span></span>

> <span data-ttu-id="f8294-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="f8294-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f8294-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f8294-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f8294-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f8294-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f8294-107">更新[windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f8294-107">Update the properties of a [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f8294-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="f8294-108">Prerequisites</span></span>
<span data-ttu-id="f8294-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="f8294-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f8294-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f8294-111">Permission type</span></span>|<span data-ttu-id="f8294-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f8294-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f8294-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f8294-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f8294-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8294-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f8294-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f8294-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f8294-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f8294-116">Not supported.</span></span>|
|<span data-ttu-id="f8294-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f8294-117">Application</span></span>|<span data-ttu-id="f8294-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="f8294-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f8294-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f8294-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="f8294-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f8294-120">Request headers</span></span>
|<span data-ttu-id="f8294-121">标头</span><span class="sxs-lookup"><span data-stu-id="f8294-121">Header</span></span>|<span data-ttu-id="f8294-122">值</span><span class="sxs-lookup"><span data-stu-id="f8294-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f8294-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f8294-123">Authorization</span></span>|<span data-ttu-id="f8294-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f8294-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f8294-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f8294-125">Accept</span></span>|<span data-ttu-id="f8294-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f8294-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8294-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f8294-127">Request body</span></span>
<span data-ttu-id="f8294-128">在请求正文中，提供[windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f8294-128">In the request body, supply a JSON representation for the [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) object.</span></span>

<span data-ttu-id="f8294-129">下表显示时创建[windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f8294-129">The following table shows the properties that are required when you create the [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md).</span></span>

|<span data-ttu-id="f8294-130">属性</span><span class="sxs-lookup"><span data-stu-id="f8294-130">Property</span></span>|<span data-ttu-id="f8294-131">类型</span><span class="sxs-lookup"><span data-stu-id="f8294-131">Type</span></span>|<span data-ttu-id="f8294-132">说明</span><span class="sxs-lookup"><span data-stu-id="f8294-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8294-133">id</span><span class="sxs-lookup"><span data-stu-id="f8294-133">id</span></span>|<span data-ttu-id="f8294-134">String</span><span class="sxs-lookup"><span data-stu-id="f8294-134">String</span></span>|<span data-ttu-id="f8294-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f8294-135">Key of the entity.</span></span> <span data-ttu-id="f8294-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8294-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f8294-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f8294-137">lastModifiedDateTime</span></span>|<span data-ttu-id="f8294-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f8294-138">DateTimeOffset</span></span>|<span data-ttu-id="f8294-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f8294-139">DateTime the object was last modified.</span></span> <span data-ttu-id="f8294-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8294-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f8294-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f8294-141">roleScopeTagIds</span></span>|<span data-ttu-id="f8294-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="f8294-142">String collection</span></span>|<span data-ttu-id="f8294-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="f8294-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f8294-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8294-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f8294-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f8294-145">supportsScopeTags</span></span>|<span data-ttu-id="f8294-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="f8294-146">Boolean</span></span>|<span data-ttu-id="f8294-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="f8294-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f8294-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="f8294-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f8294-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="f8294-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f8294-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="f8294-150">This property is read-only.</span></span> <span data-ttu-id="f8294-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8294-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f8294-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f8294-152">createdDateTime</span></span>|<span data-ttu-id="f8294-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f8294-153">DateTimeOffset</span></span>|<span data-ttu-id="f8294-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f8294-154">DateTime the object was created.</span></span> <span data-ttu-id="f8294-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8294-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f8294-156">description</span><span class="sxs-lookup"><span data-stu-id="f8294-156">description</span></span>|<span data-ttu-id="f8294-157">String</span><span class="sxs-lookup"><span data-stu-id="f8294-157">String</span></span>|<span data-ttu-id="f8294-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="f8294-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f8294-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8294-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f8294-160">displayName</span><span class="sxs-lookup"><span data-stu-id="f8294-160">displayName</span></span>|<span data-ttu-id="f8294-161">String</span><span class="sxs-lookup"><span data-stu-id="f8294-161">String</span></span>|<span data-ttu-id="f8294-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="f8294-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f8294-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8294-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f8294-164">version</span><span class="sxs-lookup"><span data-stu-id="f8294-164">version</span></span>|<span data-ttu-id="f8294-165">Int32</span><span class="sxs-lookup"><span data-stu-id="f8294-165">Int32</span></span>|<span data-ttu-id="f8294-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="f8294-166">Version of the device configuration.</span></span> <span data-ttu-id="f8294-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8294-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f8294-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="f8294-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="f8294-169">Int32</span><span class="sxs-lookup"><span data-stu-id="f8294-169">Int32</span></span>|<span data-ttu-id="f8294-170">证书续订阈值百分比。</span><span class="sxs-lookup"><span data-stu-id="f8294-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="f8294-171">继承自[windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="f8294-171">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="f8294-172">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="f8294-172">keyStorageProvider</span></span>|[<span data-ttu-id="f8294-173">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="f8294-173">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="f8294-174">密钥存储提供程序 (KSP)。</span><span class="sxs-lookup"><span data-stu-id="f8294-174">Key Storage Provider (KSP).</span></span> <span data-ttu-id="f8294-175">继承自[windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="f8294-175">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="f8294-176">可取值为：`useTpmKspOtherwiseUseSoftwareKsp`、`useTpmKspOtherwiseFail`、`usePassportForWorkKspOtherwiseFail`、`useSoftwareKsp`。</span><span class="sxs-lookup"><span data-stu-id="f8294-176">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="f8294-177">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="f8294-177">subjectNameFormat</span></span>|[<span data-ttu-id="f8294-178">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="f8294-178">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="f8294-179">证书使用者名称格式。</span><span class="sxs-lookup"><span data-stu-id="f8294-179">Certificate Subject Name Format.</span></span> <span data-ttu-id="f8294-180">继承自[windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="f8294-180">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="f8294-181">可取值为：`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId`。</span><span class="sxs-lookup"><span data-stu-id="f8294-181">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="f8294-182">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="f8294-182">subjectAlternativeNameType</span></span>|[<span data-ttu-id="f8294-183">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="f8294-183">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="f8294-184">证书使用者替代名称类型。</span><span class="sxs-lookup"><span data-stu-id="f8294-184">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="f8294-185">继承自[windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="f8294-185">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="f8294-186">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService`。</span><span class="sxs-lookup"><span data-stu-id="f8294-186">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="f8294-187">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="f8294-187">certificateValidityPeriodValue</span></span>|<span data-ttu-id="f8294-188">Int32</span><span class="sxs-lookup"><span data-stu-id="f8294-188">Int32</span></span>|<span data-ttu-id="f8294-189">证书 Validtiy 时段的值。</span><span class="sxs-lookup"><span data-stu-id="f8294-189">Value for the Certificate Validtiy Period.</span></span> <span data-ttu-id="f8294-190">继承自[windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="f8294-190">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="f8294-191">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="f8294-191">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="f8294-192">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="f8294-192">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="f8294-193">证书有效期限的小数位数。</span><span class="sxs-lookup"><span data-stu-id="f8294-193">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="f8294-194">继承自[windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="f8294-194">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="f8294-195">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="f8294-195">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="f8294-196">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="f8294-196">extendedKeyUsages</span></span>|<span data-ttu-id="f8294-197">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)集合</span><span class="sxs-lookup"><span data-stu-id="f8294-197">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="f8294-198">扩展的密钥用法 (EKU) 设置。</span><span class="sxs-lookup"><span data-stu-id="f8294-198">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="f8294-199">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="f8294-199">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="f8294-200">继承自[windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="f8294-200">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="f8294-201">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="f8294-201">scepServerUrls</span></span>|<span data-ttu-id="f8294-202">String 集合</span><span class="sxs-lookup"><span data-stu-id="f8294-202">String collection</span></span>|<span data-ttu-id="f8294-203">SCEP 服务器 Url(s)。</span><span class="sxs-lookup"><span data-stu-id="f8294-203">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="f8294-204">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="f8294-204">subjectNameFormatString</span></span>|<span data-ttu-id="f8294-205">String</span><span class="sxs-lookup"><span data-stu-id="f8294-205">String</span></span>|<span data-ttu-id="f8294-206">自定义格式使用 SubjectNameFormat = 自定义。</span><span class="sxs-lookup"><span data-stu-id="f8294-206">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="f8294-207">示例： CN = {{EmailAddress}} E = {{EmailAddress}}，OU = 企业用户，O = Contoso Corporation L = 雷德蒙德，ST = WA，C = US</span><span class="sxs-lookup"><span data-stu-id="f8294-207">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="f8294-208">keyUsage</span><span class="sxs-lookup"><span data-stu-id="f8294-208">keyUsage</span></span>|[<span data-ttu-id="f8294-209">keyUsages</span><span class="sxs-lookup"><span data-stu-id="f8294-209">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="f8294-210">SCEP 密钥用法。</span><span class="sxs-lookup"><span data-stu-id="f8294-210">SCEP Key Usage.</span></span> <span data-ttu-id="f8294-211">可取值为：`keyEncipherment`、`digitalSignature`。</span><span class="sxs-lookup"><span data-stu-id="f8294-211">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="f8294-212">keySize</span><span class="sxs-lookup"><span data-stu-id="f8294-212">keySize</span></span>|[<span data-ttu-id="f8294-213">keySize</span><span class="sxs-lookup"><span data-stu-id="f8294-213">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="f8294-214">SCEP 密钥大小。</span><span class="sxs-lookup"><span data-stu-id="f8294-214">SCEP Key Size.</span></span> <span data-ttu-id="f8294-215">可取值为：`size1024`、`size2048`。</span><span class="sxs-lookup"><span data-stu-id="f8294-215">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="f8294-216">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="f8294-216">hashAlgorithm</span></span>|[<span data-ttu-id="f8294-217">hashAlgorithms</span><span class="sxs-lookup"><span data-stu-id="f8294-217">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="f8294-218">SCEP 哈希算法。</span><span class="sxs-lookup"><span data-stu-id="f8294-218">SCEP Hash Algorithm.</span></span> <span data-ttu-id="f8294-219">可取值为：`sha1`、`sha2`。</span><span class="sxs-lookup"><span data-stu-id="f8294-219">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="f8294-220">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="f8294-220">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="f8294-221">String</span><span class="sxs-lookup"><span data-stu-id="f8294-221">String</span></span>|<span data-ttu-id="f8294-222">定义 AAD 属性的自定义字符串。</span><span class="sxs-lookup"><span data-stu-id="f8294-222">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="f8294-223">响应</span><span class="sxs-lookup"><span data-stu-id="f8294-223">Response</span></span>
<span data-ttu-id="f8294-224">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f8294-224">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8294-225">示例</span><span class="sxs-lookup"><span data-stu-id="f8294-225">Example</span></span>

### <a name="request"></a><span data-ttu-id="f8294-226">请求</span><span class="sxs-lookup"><span data-stu-id="f8294-226">Request</span></span>
<span data-ttu-id="f8294-227">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f8294-227">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="f8294-228">响应</span><span class="sxs-lookup"><span data-stu-id="f8294-228">Response</span></span>
<span data-ttu-id="f8294-p122">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f8294-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




