---
title: 更新 windows10ImportedPFXCertificateProfile
description: 更新 windows10ImportedPFXCertificateProfile 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2bd45a3030447acc6358cf7812b578a9468a713b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27925068"
---
# <a name="update-windows10importedpfxcertificateprofile"></a><span data-ttu-id="d74fe-103">更新 windows10ImportedPFXCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="d74fe-103">Update windows10ImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="d74fe-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d74fe-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d74fe-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d74fe-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d74fe-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d74fe-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d74fe-107">更新[windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d74fe-107">Update the properties of a [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d74fe-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="d74fe-108">Prerequisites</span></span>
<span data-ttu-id="d74fe-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="d74fe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d74fe-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d74fe-111">Permission type</span></span>|<span data-ttu-id="d74fe-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d74fe-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d74fe-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d74fe-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d74fe-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d74fe-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d74fe-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d74fe-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d74fe-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d74fe-116">Not supported.</span></span>|
|<span data-ttu-id="d74fe-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d74fe-117">Application</span></span>|<span data-ttu-id="d74fe-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="d74fe-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d74fe-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d74fe-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="d74fe-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d74fe-120">Request headers</span></span>
|<span data-ttu-id="d74fe-121">标头</span><span class="sxs-lookup"><span data-stu-id="d74fe-121">Header</span></span>|<span data-ttu-id="d74fe-122">值</span><span class="sxs-lookup"><span data-stu-id="d74fe-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d74fe-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d74fe-123">Authorization</span></span>|<span data-ttu-id="d74fe-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d74fe-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d74fe-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d74fe-125">Accept</span></span>|<span data-ttu-id="d74fe-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d74fe-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d74fe-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d74fe-127">Request body</span></span>
<span data-ttu-id="d74fe-128">在请求正文中，提供[windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d74fe-128">In the request body, supply a JSON representation for the [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md) object.</span></span>

<span data-ttu-id="d74fe-129">下表显示时创建[windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d74fe-129">The following table shows the properties that are required when you create the [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md).</span></span>

|<span data-ttu-id="d74fe-130">属性</span><span class="sxs-lookup"><span data-stu-id="d74fe-130">Property</span></span>|<span data-ttu-id="d74fe-131">类型</span><span class="sxs-lookup"><span data-stu-id="d74fe-131">Type</span></span>|<span data-ttu-id="d74fe-132">说明</span><span class="sxs-lookup"><span data-stu-id="d74fe-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d74fe-133">id</span><span class="sxs-lookup"><span data-stu-id="d74fe-133">id</span></span>|<span data-ttu-id="d74fe-134">String</span><span class="sxs-lookup"><span data-stu-id="d74fe-134">String</span></span>|<span data-ttu-id="d74fe-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d74fe-135">Key of the entity.</span></span> <span data-ttu-id="d74fe-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d74fe-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d74fe-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d74fe-137">lastModifiedDateTime</span></span>|<span data-ttu-id="d74fe-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d74fe-138">DateTimeOffset</span></span>|<span data-ttu-id="d74fe-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="d74fe-139">DateTime the object was last modified.</span></span> <span data-ttu-id="d74fe-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d74fe-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d74fe-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d74fe-141">roleScopeTagIds</span></span>|<span data-ttu-id="d74fe-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="d74fe-142">String collection</span></span>|<span data-ttu-id="d74fe-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="d74fe-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d74fe-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d74fe-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d74fe-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d74fe-145">supportsScopeTags</span></span>|<span data-ttu-id="d74fe-146">布尔</span><span class="sxs-lookup"><span data-stu-id="d74fe-146">Boolean</span></span>|<span data-ttu-id="d74fe-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="d74fe-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d74fe-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="d74fe-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d74fe-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="d74fe-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d74fe-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="d74fe-150">This property is read-only.</span></span> <span data-ttu-id="d74fe-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d74fe-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d74fe-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d74fe-152">createdDateTime</span></span>|<span data-ttu-id="d74fe-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d74fe-153">DateTimeOffset</span></span>|<span data-ttu-id="d74fe-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="d74fe-154">DateTime the object was created.</span></span> <span data-ttu-id="d74fe-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d74fe-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d74fe-156">description</span><span class="sxs-lookup"><span data-stu-id="d74fe-156">description</span></span>|<span data-ttu-id="d74fe-157">String</span><span class="sxs-lookup"><span data-stu-id="d74fe-157">String</span></span>|<span data-ttu-id="d74fe-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="d74fe-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d74fe-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d74fe-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d74fe-160">displayName</span><span class="sxs-lookup"><span data-stu-id="d74fe-160">displayName</span></span>|<span data-ttu-id="d74fe-161">String</span><span class="sxs-lookup"><span data-stu-id="d74fe-161">String</span></span>|<span data-ttu-id="d74fe-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="d74fe-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d74fe-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d74fe-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d74fe-164">version</span><span class="sxs-lookup"><span data-stu-id="d74fe-164">version</span></span>|<span data-ttu-id="d74fe-165">Int32</span><span class="sxs-lookup"><span data-stu-id="d74fe-165">Int32</span></span>|<span data-ttu-id="d74fe-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="d74fe-166">Version of the device configuration.</span></span> <span data-ttu-id="d74fe-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d74fe-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d74fe-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="d74fe-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="d74fe-169">Int32</span><span class="sxs-lookup"><span data-stu-id="d74fe-169">Int32</span></span>|<span data-ttu-id="d74fe-170">证书续订阈值百分比。</span><span class="sxs-lookup"><span data-stu-id="d74fe-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="d74fe-171">有效值 1 到 99 继承自[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="d74fe-171">Valid values 1 to 99 Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="d74fe-172">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="d74fe-172">keyStorageProvider</span></span>|[<span data-ttu-id="d74fe-173">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="d74fe-173">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="d74fe-174">从[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)键存储提供程序 (KSP) 继承。</span><span class="sxs-lookup"><span data-stu-id="d74fe-174">Key Storage Provider (KSP) Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="d74fe-175">可取值为：`useTpmKspOtherwiseUseSoftwareKsp`、`useTpmKspOtherwiseFail`、`usePassportForWorkKspOtherwiseFail`、`useSoftwareKsp`。</span><span class="sxs-lookup"><span data-stu-id="d74fe-175">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="d74fe-176">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="d74fe-176">subjectNameFormat</span></span>|[<span data-ttu-id="d74fe-177">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="d74fe-177">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="d74fe-178">证书使用者名称格式继承自[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="d74fe-178">Certificate Subject Name Format Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="d74fe-179">可取值为：`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId`。</span><span class="sxs-lookup"><span data-stu-id="d74fe-179">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="d74fe-180">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="d74fe-180">subjectAlternativeNameType</span></span>|[<span data-ttu-id="d74fe-181">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="d74fe-181">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="d74fe-182">证书使用者替代名称类型继承自[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="d74fe-182">Certificate Subject Alternative Name Type Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="d74fe-183">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService`。</span><span class="sxs-lookup"><span data-stu-id="d74fe-183">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="d74fe-184">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="d74fe-184">certificateValidityPeriodValue</span></span>|<span data-ttu-id="d74fe-185">Int32</span><span class="sxs-lookup"><span data-stu-id="d74fe-185">Int32</span></span>|<span data-ttu-id="d74fe-186">证书有效性段继承自[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)值</span><span class="sxs-lookup"><span data-stu-id="d74fe-186">Value for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="d74fe-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="d74fe-187">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="d74fe-188">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="d74fe-188">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="d74fe-189">证书有效性段继承自[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)的小数位数。</span><span class="sxs-lookup"><span data-stu-id="d74fe-189">Scale for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="d74fe-190">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="d74fe-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="d74fe-191">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="d74fe-191">intendedPurpose</span></span>|[<span data-ttu-id="d74fe-192">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="d74fe-192">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="d74fe-193">尚未编档。</span><span class="sxs-lookup"><span data-stu-id="d74fe-193">Not yet documented.</span></span> <span data-ttu-id="d74fe-194">可取值为：`unassigned`、`smimeEncryption`、`smimeSigning`、`vpn`、`wifi`。</span><span class="sxs-lookup"><span data-stu-id="d74fe-194">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="d74fe-195">响应</span><span class="sxs-lookup"><span data-stu-id="d74fe-195">Response</span></span>
<span data-ttu-id="d74fe-196">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d74fe-196">If successful, this method returns a `200 OK` response code and an updated [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d74fe-197">示例</span><span class="sxs-lookup"><span data-stu-id="d74fe-197">Example</span></span>
### <a name="request"></a><span data-ttu-id="d74fe-198">请求</span><span class="sxs-lookup"><span data-stu-id="d74fe-198">Request</span></span>
<span data-ttu-id="d74fe-199">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d74fe-199">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 573

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
  "intendedPurpose": "smimeEncryption"
}
```

### <a name="response"></a><span data-ttu-id="d74fe-200">响应</span><span class="sxs-lookup"><span data-stu-id="d74fe-200">Response</span></span>
<span data-ttu-id="d74fe-p117">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d74fe-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 758

{
  "@odata.type": "#microsoft.graph.windows10ImportedPFXCertificateProfile",
  "id": "b582514b-514b-b582-4b51-82b54b5182b5",
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
  "intendedPurpose": "smimeEncryption"
}
```





