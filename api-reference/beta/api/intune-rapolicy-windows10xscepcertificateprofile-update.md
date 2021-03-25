---
title: 更新 windows10XSCEPCertificateProfile
description: 更新 windows10XSCEPCertificateProfile 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 721b41e592d5885596efc185cfc1d2c5df2bcb2c
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51151919"
---
# <a name="update-windows10xscepcertificateprofile"></a><span data-ttu-id="063e2-103">更新 windows10XSCEPCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="063e2-103">Update windows10XSCEPCertificateProfile</span></span>

<span data-ttu-id="063e2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="063e2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="063e2-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="063e2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="063e2-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="063e2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="063e2-107">更新 [windows10XSCEPCertificateProfile 对象](../resources/intune-rapolicy-windows10xscepcertificateprofile.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="063e2-107">Update the properties of a [windows10XSCEPCertificateProfile](../resources/intune-rapolicy-windows10xscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="063e2-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="063e2-108">Prerequisites</span></span>
<span data-ttu-id="063e2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="063e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="063e2-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="063e2-111">Permission type</span></span>|<span data-ttu-id="063e2-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="063e2-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="063e2-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="063e2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="063e2-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="063e2-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="063e2-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="063e2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="063e2-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="063e2-116">Not supported.</span></span>|
|<span data-ttu-id="063e2-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="063e2-117">Application</span></span>|<span data-ttu-id="063e2-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="063e2-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="063e2-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="063e2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/resourceAccessProfiles/{deviceManagementResourceAccessProfileBaseId}
```

## <a name="request-headers"></a><span data-ttu-id="063e2-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="063e2-120">Request headers</span></span>
|<span data-ttu-id="063e2-121">标头</span><span class="sxs-lookup"><span data-stu-id="063e2-121">Header</span></span>|<span data-ttu-id="063e2-122">值</span><span class="sxs-lookup"><span data-stu-id="063e2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="063e2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="063e2-123">Authorization</span></span>|<span data-ttu-id="063e2-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="063e2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="063e2-125">接受</span><span class="sxs-lookup"><span data-stu-id="063e2-125">Accept</span></span>|<span data-ttu-id="063e2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="063e2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="063e2-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="063e2-127">Request body</span></span>
<span data-ttu-id="063e2-128">在请求正文中，提供 [windows10XSCEPCertificateProfile](../resources/intune-rapolicy-windows10xscepcertificateprofile.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="063e2-128">In the request body, supply a JSON representation for the [windows10XSCEPCertificateProfile](../resources/intune-rapolicy-windows10xscepcertificateprofile.md) object.</span></span>

<span data-ttu-id="063e2-129">下表显示创建 [windows10XSCEPCertificateProfile 时所需的属性](../resources/intune-rapolicy-windows10xscepcertificateprofile.md)。</span><span class="sxs-lookup"><span data-stu-id="063e2-129">The following table shows the properties that are required when you create the [windows10XSCEPCertificateProfile](../resources/intune-rapolicy-windows10xscepcertificateprofile.md).</span></span>

|<span data-ttu-id="063e2-130">属性</span><span class="sxs-lookup"><span data-stu-id="063e2-130">Property</span></span>|<span data-ttu-id="063e2-131">类型</span><span class="sxs-lookup"><span data-stu-id="063e2-131">Type</span></span>|<span data-ttu-id="063e2-132">说明</span><span class="sxs-lookup"><span data-stu-id="063e2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="063e2-133">id</span><span class="sxs-lookup"><span data-stu-id="063e2-133">id</span></span>|<span data-ttu-id="063e2-134">String</span><span class="sxs-lookup"><span data-stu-id="063e2-134">String</span></span>|<span data-ttu-id="063e2-135">配置文件标识符 继承自 [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="063e2-135">Profile identifier Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="063e2-136">version</span><span class="sxs-lookup"><span data-stu-id="063e2-136">version</span></span>|<span data-ttu-id="063e2-137">Int32</span><span class="sxs-lookup"><span data-stu-id="063e2-137">Int32</span></span>|<span data-ttu-id="063e2-138">配置文件的版本 继承自 [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="063e2-138">Version of the profile Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="063e2-139">displayName</span><span class="sxs-lookup"><span data-stu-id="063e2-139">displayName</span></span>|<span data-ttu-id="063e2-140">String</span><span class="sxs-lookup"><span data-stu-id="063e2-140">String</span></span>|<span data-ttu-id="063e2-141">配置文件显示名称继承自 [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="063e2-141">Profile display name Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="063e2-142">说明</span><span class="sxs-lookup"><span data-stu-id="063e2-142">description</span></span>|<span data-ttu-id="063e2-143">String</span><span class="sxs-lookup"><span data-stu-id="063e2-143">String</span></span>|<span data-ttu-id="063e2-144">配置文件说明 继承自 [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="063e2-144">Profile description Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="063e2-145">creationDateTime</span><span class="sxs-lookup"><span data-stu-id="063e2-145">creationDateTime</span></span>|<span data-ttu-id="063e2-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="063e2-146">DateTimeOffset</span></span>|<span data-ttu-id="063e2-147">DateTime 配置文件已创建 继承自 [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="063e2-147">DateTime profile was created Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="063e2-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="063e2-148">lastModifiedDateTime</span></span>|<span data-ttu-id="063e2-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="063e2-149">DateTimeOffset</span></span>|<span data-ttu-id="063e2-150">DateTime 配置文件上次修改时间 继承自 [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="063e2-150">DateTime profile was last modified Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="063e2-151">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="063e2-151">roleScopeTagIds</span></span>|<span data-ttu-id="063e2-152">String collection</span><span class="sxs-lookup"><span data-stu-id="063e2-152">String collection</span></span>|<span data-ttu-id="063e2-153">范围标记 继承自 [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="063e2-153">Scope Tags Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="063e2-154">certificateStore</span><span class="sxs-lookup"><span data-stu-id="063e2-154">certificateStore</span></span>|[<span data-ttu-id="063e2-155">certificateStore</span><span class="sxs-lookup"><span data-stu-id="063e2-155">certificateStore</span></span>](../resources/intune-shared-certificatestore.md)|<span data-ttu-id="063e2-156">目标存储证书。</span><span class="sxs-lookup"><span data-stu-id="063e2-156">Target store certificate.</span></span> <span data-ttu-id="063e2-157">可取值为：`user`、`machine`。</span><span class="sxs-lookup"><span data-stu-id="063e2-157">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="063e2-158">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="063e2-158">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="063e2-159">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="063e2-159">certificateValidityPeriodScale</span></span>](../resources/intune-shared-certificatevalidityperiodscale.md)|<span data-ttu-id="063e2-160">证书有效期的缩放。</span><span class="sxs-lookup"><span data-stu-id="063e2-160">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="063e2-161">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="063e2-161">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="063e2-162">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="063e2-162">certificateValidityPeriodValue</span></span>|<span data-ttu-id="063e2-163">Int32</span><span class="sxs-lookup"><span data-stu-id="063e2-163">Int32</span></span>|<span data-ttu-id="063e2-164">证书有效期的值</span><span class="sxs-lookup"><span data-stu-id="063e2-164">Value for the Certificate Validity Period</span></span>|
|<span data-ttu-id="063e2-165">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="063e2-165">extendedKeyUsages</span></span>|<span data-ttu-id="063e2-166">[extendedKeyUsage](../resources/intune-shared-extendedkeyusage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="063e2-166">[extendedKeyUsage](../resources/intune-shared-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="063e2-167">EKU (扩展密钥) 设置。</span><span class="sxs-lookup"><span data-stu-id="063e2-167">Extended Key Usage (EKU) settings.</span></span>|
|<span data-ttu-id="063e2-168">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="063e2-168">hashAlgorithm</span></span>|<span data-ttu-id="063e2-169">[hashAlgorithms](../resources/intune-shared-hashalgorithms.md) 集合</span><span class="sxs-lookup"><span data-stu-id="063e2-169">[hashAlgorithms](../resources/intune-shared-hashalgorithms.md) collection</span></span>|<span data-ttu-id="063e2-170">SCEP 哈希算法。</span><span class="sxs-lookup"><span data-stu-id="063e2-170">SCEP Hash Algorithm.</span></span> <span data-ttu-id="063e2-171">可取值为：`sha1`、`sha2`。</span><span class="sxs-lookup"><span data-stu-id="063e2-171">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="063e2-172">keySize</span><span class="sxs-lookup"><span data-stu-id="063e2-172">keySize</span></span>|[<span data-ttu-id="063e2-173">keySize</span><span class="sxs-lookup"><span data-stu-id="063e2-173">keySize</span></span>](../resources/intune-shared-keysize.md)|<span data-ttu-id="063e2-174">SCEP 密钥大小。</span><span class="sxs-lookup"><span data-stu-id="063e2-174">SCEP Key Size.</span></span> <span data-ttu-id="063e2-175">可取值为：`size1024`、`size2048`、`size4096`。</span><span class="sxs-lookup"><span data-stu-id="063e2-175">Possible values are: `size1024`, `size2048`, `size4096`.</span></span>|
|<span data-ttu-id="063e2-176">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="063e2-176">keyStorageProvider</span></span>|[<span data-ttu-id="063e2-177">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="063e2-177">keyStorageProviderOption</span></span>](../resources/intune-shared-keystorageprovideroption.md)|<span data-ttu-id="063e2-178">密钥存储提供程序 (KSP) 。</span><span class="sxs-lookup"><span data-stu-id="063e2-178">Key Storage Provider (KSP).</span></span> <span data-ttu-id="063e2-179">可取值为：`useTpmKspOtherwiseUseSoftwareKsp`、`useTpmKspOtherwiseFail`、`usePassportForWorkKspOtherwiseFail`、`useSoftwareKsp`。</span><span class="sxs-lookup"><span data-stu-id="063e2-179">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="063e2-180">keyUsage</span><span class="sxs-lookup"><span data-stu-id="063e2-180">keyUsage</span></span>|[<span data-ttu-id="063e2-181">keyUsages</span><span class="sxs-lookup"><span data-stu-id="063e2-181">keyUsages</span></span>](../resources/intune-shared-keyusages.md)|<span data-ttu-id="063e2-182">SCEP 密钥用法。</span><span class="sxs-lookup"><span data-stu-id="063e2-182">SCEP Key Usage.</span></span> <span data-ttu-id="063e2-183">可取值为：`keyEncipherment`、`digitalSignature`。</span><span class="sxs-lookup"><span data-stu-id="063e2-183">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="063e2-184">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="063e2-184">renewalThresholdPercentage</span></span>|<span data-ttu-id="063e2-185">Int32</span><span class="sxs-lookup"><span data-stu-id="063e2-185">Int32</span></span>|<span data-ttu-id="063e2-186">证书续订阈值百分比</span><span class="sxs-lookup"><span data-stu-id="063e2-186">Certificate renewal threshold percentage</span></span>|
|<span data-ttu-id="063e2-187">rootCertificateId</span><span class="sxs-lookup"><span data-stu-id="063e2-187">rootCertificateId</span></span>|<span data-ttu-id="063e2-188">Guid</span><span class="sxs-lookup"><span data-stu-id="063e2-188">Guid</span></span>|<span data-ttu-id="063e2-189">受信任的根证书 ID</span><span class="sxs-lookup"><span data-stu-id="063e2-189">Trusted Root Certificate ID</span></span>|
|<span data-ttu-id="063e2-190">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="063e2-190">scepServerUrls</span></span>|<span data-ttu-id="063e2-191">String collection</span><span class="sxs-lookup"><span data-stu-id="063e2-191">String collection</span></span>|<span data-ttu-id="063e2-192">SCEP 服务器 URL () 。</span><span class="sxs-lookup"><span data-stu-id="063e2-192">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="063e2-193">subjectAlternativeNameFormats</span><span class="sxs-lookup"><span data-stu-id="063e2-193">subjectAlternativeNameFormats</span></span>|<span data-ttu-id="063e2-194">[windows10XCustomSubjectAlternativeName](../resources/intune-rapolicy-windows10xcustomsubjectalternativename.md) 集合</span><span class="sxs-lookup"><span data-stu-id="063e2-194">[windows10XCustomSubjectAlternativeName](../resources/intune-rapolicy-windows10xcustomsubjectalternativename.md) collection</span></span>|<span data-ttu-id="063e2-195">自定义 AAD 属性。</span><span class="sxs-lookup"><span data-stu-id="063e2-195">Custom AAD Attributes.</span></span>|
|<span data-ttu-id="063e2-196">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="063e2-196">subjectNameFormatString</span></span>|<span data-ttu-id="063e2-197">String</span><span class="sxs-lookup"><span data-stu-id="063e2-197">String</span></span>|<span data-ttu-id="063e2-198">要与 SubjectNameFormat 一同使用的自定义格式 = Custom。</span><span class="sxs-lookup"><span data-stu-id="063e2-198">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="063e2-199">示例：CN={{EmailAddress}}，E={{EmailAddress}，OU=Enterprise Users，O=Contoso Corporation，L=Redmond，ST=WA，C=US</span><span class="sxs-lookup"><span data-stu-id="063e2-199">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|



## <a name="response"></a><span data-ttu-id="063e2-200">响应</span><span class="sxs-lookup"><span data-stu-id="063e2-200">Response</span></span>
<span data-ttu-id="063e2-201">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [windows10XSCEPCertificateProfile](../resources/intune-rapolicy-windows10xscepcertificateprofile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="063e2-201">If successful, this method returns a `200 OK` response code and an updated [windows10XSCEPCertificateProfile](../resources/intune-rapolicy-windows10xscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="063e2-202">示例</span><span class="sxs-lookup"><span data-stu-id="063e2-202">Example</span></span>

### <a name="request"></a><span data-ttu-id="063e2-203">请求</span><span class="sxs-lookup"><span data-stu-id="063e2-203">Request</span></span>
<span data-ttu-id="063e2-204">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="063e2-204">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/resourceAccessProfiles/{deviceManagementResourceAccessProfileBaseId}
Content-type: application/json
Content-length: 1178

{
  "@odata.type": "#microsoft.graph.windows10XSCEPCertificateProfile",
  "version": 7,
  "displayName": "Display Name value",
  "description": "Description value",
  "creationDateTime": "2017-01-01T00:00:43.1365422-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "certificateStore": "machine",
  "certificateValidityPeriodScale": "months",
  "certificateValidityPeriodValue": 14,
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "hashAlgorithm": [
    "sha2"
  ],
  "keySize": "size2048",
  "keyStorageProvider": "useTpmKspOtherwiseFail",
  "keyUsage": "digitalSignature",
  "renewalThresholdPercentage": 10,
  "rootCertificateId": "ed919bbc-9bbc-ed91-bc9b-91edbc9b91ed",
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectAlternativeNameFormats": [
    {
      "@odata.type": "microsoft.graph.windows10XCustomSubjectAlternativeName",
      "sanType": "emailAddress",
      "name": "Name value"
    }
  ],
  "subjectNameFormatString": "Subject Name Format String value"
}
```

### <a name="response"></a><span data-ttu-id="063e2-205">响应</span><span class="sxs-lookup"><span data-stu-id="063e2-205">Response</span></span>
<span data-ttu-id="063e2-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="063e2-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1291

{
  "@odata.type": "#microsoft.graph.windows10XSCEPCertificateProfile",
  "id": "d174d58e-d58e-d174-8ed5-74d18ed574d1",
  "version": 7,
  "displayName": "Display Name value",
  "description": "Description value",
  "creationDateTime": "2017-01-01T00:00:43.1365422-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "certificateStore": "machine",
  "certificateValidityPeriodScale": "months",
  "certificateValidityPeriodValue": 14,
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "hashAlgorithm": [
    "sha2"
  ],
  "keySize": "size2048",
  "keyStorageProvider": "useTpmKspOtherwiseFail",
  "keyUsage": "digitalSignature",
  "renewalThresholdPercentage": 10,
  "rootCertificateId": "ed919bbc-9bbc-ed91-bc9b-91edbc9b91ed",
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectAlternativeNameFormats": [
    {
      "@odata.type": "microsoft.graph.windows10XCustomSubjectAlternativeName",
      "sanType": "emailAddress",
      "name": "Name value"
    }
  ],
  "subjectNameFormatString": "Subject Name Format String value"
}
```




