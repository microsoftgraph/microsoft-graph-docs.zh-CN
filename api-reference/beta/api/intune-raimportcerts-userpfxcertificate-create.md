---
title: 创建 userPFXCertificate
description: 创建新的 userPFXCertificate 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 06cc1ad70417e771a6ab0a20b45be3c9c735bfad
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37537308"
---
# <a name="create-userpfxcertificate"></a><span data-ttu-id="3355e-103">创建 userPFXCertificate</span><span class="sxs-lookup"><span data-stu-id="3355e-103">Create userPFXCertificate</span></span>

> <span data-ttu-id="3355e-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3355e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3355e-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3355e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3355e-106">创建新的[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="3355e-106">Create a new [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3355e-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="3355e-107">Prerequisites</span></span>
<span data-ttu-id="3355e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3355e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3355e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="3355e-110">Permission type</span></span>|<span data-ttu-id="3355e-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3355e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3355e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3355e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3355e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3355e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3355e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3355e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3355e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3355e-115">Not supported.</span></span>|
|<span data-ttu-id="3355e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="3355e-116">Application</span></span>|<span data-ttu-id="3355e-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3355e-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3355e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3355e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userPfxCertificates
```

## <a name="request-headers"></a><span data-ttu-id="3355e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="3355e-119">Request headers</span></span>
|<span data-ttu-id="3355e-120">标头</span><span class="sxs-lookup"><span data-stu-id="3355e-120">Header</span></span>|<span data-ttu-id="3355e-121">值</span><span class="sxs-lookup"><span data-stu-id="3355e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3355e-122">授权</span><span class="sxs-lookup"><span data-stu-id="3355e-122">Authorization</span></span>|<span data-ttu-id="3355e-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3355e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3355e-124">接受</span><span class="sxs-lookup"><span data-stu-id="3355e-124">Accept</span></span>|<span data-ttu-id="3355e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3355e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3355e-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="3355e-126">Request body</span></span>
<span data-ttu-id="3355e-127">在请求正文中，提供 userPFXCertificate 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3355e-127">In the request body, supply a JSON representation for the userPFXCertificate object.</span></span>

<span data-ttu-id="3355e-128">下表显示创建 userPFXCertificate 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3355e-128">The following table shows the properties that are required when you create the userPFXCertificate.</span></span>

|<span data-ttu-id="3355e-129">属性</span><span class="sxs-lookup"><span data-stu-id="3355e-129">Property</span></span>|<span data-ttu-id="3355e-130">类型</span><span class="sxs-lookup"><span data-stu-id="3355e-130">Type</span></span>|<span data-ttu-id="3355e-131">说明</span><span class="sxs-lookup"><span data-stu-id="3355e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3355e-132">id</span><span class="sxs-lookup"><span data-stu-id="3355e-132">id</span></span>|<span data-ttu-id="3355e-133">String</span><span class="sxs-lookup"><span data-stu-id="3355e-133">String</span></span>|<span data-ttu-id="3355e-134">PFX 证书的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="3355e-134">Unique identifier for the PFX certificate.</span></span>|
|<span data-ttu-id="3355e-135">为</span><span class="sxs-lookup"><span data-stu-id="3355e-135">thumbprint</span></span>|<span data-ttu-id="3355e-136">字符串</span><span class="sxs-lookup"><span data-stu-id="3355e-136">String</span></span>|<span data-ttu-id="3355e-137">SHA-1 PFX 证书的指纹。</span><span class="sxs-lookup"><span data-stu-id="3355e-137">SHA-1 thumbprint of the PFX certificate.</span></span>|
|<span data-ttu-id="3355e-138">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="3355e-138">intendedPurpose</span></span>|[<span data-ttu-id="3355e-139">userPfxIntendedPurpose</span><span class="sxs-lookup"><span data-stu-id="3355e-139">userPfxIntendedPurpose</span></span>](../resources/intune-raimportcerts-userpfxintendedpurpose.md)|<span data-ttu-id="3355e-140">证书的预期目的是从部署的角度来看。</span><span class="sxs-lookup"><span data-stu-id="3355e-140">Certificate's intended purpose from the point-of-view of deployment.</span></span> <span data-ttu-id="3355e-141">可取值为：`unassigned`、`smimeEncryption`、`smimeSigning`、`vpn`、`wifi`。</span><span class="sxs-lookup"><span data-stu-id="3355e-141">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|
|<span data-ttu-id="3355e-142">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="3355e-142">userPrincipalName</span></span>|<span data-ttu-id="3355e-143">字符串</span><span class="sxs-lookup"><span data-stu-id="3355e-143">String</span></span>|<span data-ttu-id="3355e-144">PFX 证书的用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="3355e-144">User Principal Name of the PFX certificate.</span></span>|
|<span data-ttu-id="3355e-145">startDateTime</span><span class="sxs-lookup"><span data-stu-id="3355e-145">startDateTime</span></span>|<span data-ttu-id="3355e-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3355e-146">DateTimeOffset</span></span>|<span data-ttu-id="3355e-147">证书的有效期开始日期/时间。</span><span class="sxs-lookup"><span data-stu-id="3355e-147">Certificate's validity start date/time.</span></span>|
|<span data-ttu-id="3355e-148">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="3355e-148">expirationDateTime</span></span>|<span data-ttu-id="3355e-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3355e-149">DateTimeOffset</span></span>|<span data-ttu-id="3355e-150">证书的有效期到期日期/时间。</span><span class="sxs-lookup"><span data-stu-id="3355e-150">Certificate's validity expiration date/time.</span></span>|
|<span data-ttu-id="3355e-151">providerName</span><span class="sxs-lookup"><span data-stu-id="3355e-151">providerName</span></span>|<span data-ttu-id="3355e-152">字符串</span><span class="sxs-lookup"><span data-stu-id="3355e-152">String</span></span>|<span data-ttu-id="3355e-153">用于加密此 blob 的加密提供程序。</span><span class="sxs-lookup"><span data-stu-id="3355e-153">Crypto provider used to encrypt this blob.</span></span>|
|<span data-ttu-id="3355e-154">名</span><span class="sxs-lookup"><span data-stu-id="3355e-154">keyName</span></span>|<span data-ttu-id="3355e-155">字符串</span><span class="sxs-lookup"><span data-stu-id="3355e-155">String</span></span>|<span data-ttu-id="3355e-156">用于对 blob 进行加密的密钥（在提供程序中）的名称。</span><span class="sxs-lookup"><span data-stu-id="3355e-156">Name of the key (within the provider) used to encrypt the blob.</span></span>|
|<span data-ttu-id="3355e-157">paddingScheme</span><span class="sxs-lookup"><span data-stu-id="3355e-157">paddingScheme</span></span>|[<span data-ttu-id="3355e-158">userPfxPaddingScheme</span><span class="sxs-lookup"><span data-stu-id="3355e-158">userPfxPaddingScheme</span></span>](../resources/intune-raimportcerts-userpfxpaddingscheme.md)|<span data-ttu-id="3355e-159">加密/解密过程中提供程序使用的填充方案。</span><span class="sxs-lookup"><span data-stu-id="3355e-159">Padding scheme used by the provider during encryption/decryption.</span></span> <span data-ttu-id="3355e-160">可取值为：`none`、`pkcs1`、`oaepSha1`、`oaepSha256`、`oaepSha384`、`oaepSha512`。</span><span class="sxs-lookup"><span data-stu-id="3355e-160">Possible values are: `none`, `pkcs1`, `oaepSha1`, `oaepSha256`, `oaepSha384`, `oaepSha512`.</span></span>|
|<span data-ttu-id="3355e-161">encryptedPfxBlob</span><span class="sxs-lookup"><span data-stu-id="3355e-161">encryptedPfxBlob</span></span>|<span data-ttu-id="3355e-162">Binary</span><span class="sxs-lookup"><span data-stu-id="3355e-162">Binary</span></span>|<span data-ttu-id="3355e-163">加密的 PFX blob。</span><span class="sxs-lookup"><span data-stu-id="3355e-163">Encrypted PFX blob.</span></span>|
|<span data-ttu-id="3355e-164">encryptedPfxPassword</span><span class="sxs-lookup"><span data-stu-id="3355e-164">encryptedPfxPassword</span></span>|<span data-ttu-id="3355e-165">字符串</span><span class="sxs-lookup"><span data-stu-id="3355e-165">String</span></span>|<span data-ttu-id="3355e-166">加密的 PFX 密码。</span><span class="sxs-lookup"><span data-stu-id="3355e-166">Encrypted PFX password.</span></span>|
|<span data-ttu-id="3355e-167">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3355e-167">createdDateTime</span></span>|<span data-ttu-id="3355e-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3355e-168">DateTimeOffset</span></span>|<span data-ttu-id="3355e-169">导入此 PFX 证书的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="3355e-169">Date/time when this PFX certificate was imported.</span></span>|
|<span data-ttu-id="3355e-170">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3355e-170">lastModifiedDateTime</span></span>|<span data-ttu-id="3355e-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3355e-171">DateTimeOffset</span></span>|<span data-ttu-id="3355e-172">上次修改此 PFX 证书的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="3355e-172">Date/time when this PFX certificate was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="3355e-173">响应</span><span class="sxs-lookup"><span data-stu-id="3355e-173">Response</span></span>
<span data-ttu-id="3355e-174">如果成功，此方法在响应`201 Created`正文中返回响应代码和[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="3355e-174">If successful, this method returns a `201 Created` response code and a [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3355e-175">示例</span><span class="sxs-lookup"><span data-stu-id="3355e-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="3355e-176">请求</span><span class="sxs-lookup"><span data-stu-id="3355e-176">Request</span></span>
<span data-ttu-id="3355e-177">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3355e-177">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userPfxCertificates
Content-type: application/json
Content-length: 523

{
  "@odata.type": "#microsoft.graph.userPFXCertificate",
  "thumbprint": "Thumbprint value",
  "intendedPurpose": "smimeEncryption",
  "userPrincipalName": "User Principal Name value",
  "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "providerName": "Provider Name value",
  "keyName": "Key Name value",
  "paddingScheme": "pkcs1",
  "encryptedPfxBlob": "ZW5jcnlwdGVkUGZ4QmxvYg==",
  "encryptedPfxPassword": "Encrypted Pfx Password value"
}
```

### <a name="response"></a><span data-ttu-id="3355e-178">响应</span><span class="sxs-lookup"><span data-stu-id="3355e-178">Response</span></span>
<span data-ttu-id="3355e-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3355e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 695

{
  "@odata.type": "#microsoft.graph.userPFXCertificate",
  "id": "045c159b-159b-045c-9b15-5c049b155c04",
  "thumbprint": "Thumbprint value",
  "intendedPurpose": "smimeEncryption",
  "userPrincipalName": "User Principal Name value",
  "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "providerName": "Provider Name value",
  "keyName": "Key Name value",
  "paddingScheme": "pkcs1",
  "encryptedPfxBlob": "ZW5jcnlwdGVkUGZ4QmxvYg==",
  "encryptedPfxPassword": "Encrypted Pfx Password value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```






