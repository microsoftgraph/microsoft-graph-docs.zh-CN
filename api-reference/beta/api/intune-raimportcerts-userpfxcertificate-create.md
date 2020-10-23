---
title: 创建 userPFXCertificate
description: 创建新的 userPFXCertificate 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2af465d96a576867f8b712679d61012bfcd8888a
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48731160"
---
# <a name="create-userpfxcertificate"></a><span data-ttu-id="55803-103">创建 userPFXCertificate</span><span class="sxs-lookup"><span data-stu-id="55803-103">Create userPFXCertificate</span></span>

<span data-ttu-id="55803-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55803-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="55803-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="55803-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="55803-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="55803-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55803-107">创建新的 [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="55803-107">Create a new [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="55803-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="55803-108">Prerequisites</span></span>
<span data-ttu-id="55803-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="55803-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55803-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="55803-111">Permission type</span></span>|<span data-ttu-id="55803-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="55803-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="55803-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="55803-113">Delegated (work or school account)</span></span>|<span data-ttu-id="55803-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55803-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="55803-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="55803-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="55803-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="55803-116">Not supported.</span></span>|
|<span data-ttu-id="55803-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="55803-117">Application</span></span>|<span data-ttu-id="55803-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55803-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="55803-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="55803-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userPfxCertificates
```

## <a name="request-headers"></a><span data-ttu-id="55803-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="55803-120">Request headers</span></span>
|<span data-ttu-id="55803-121">标头</span><span class="sxs-lookup"><span data-stu-id="55803-121">Header</span></span>|<span data-ttu-id="55803-122">值</span><span class="sxs-lookup"><span data-stu-id="55803-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="55803-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="55803-123">Authorization</span></span>|<span data-ttu-id="55803-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="55803-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="55803-125">接受</span><span class="sxs-lookup"><span data-stu-id="55803-125">Accept</span></span>|<span data-ttu-id="55803-126">application/json</span><span class="sxs-lookup"><span data-stu-id="55803-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="55803-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="55803-127">Request body</span></span>
<span data-ttu-id="55803-128">在请求正文中，提供 userPFXCertificate 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="55803-128">In the request body, supply a JSON representation for the userPFXCertificate object.</span></span>

<span data-ttu-id="55803-129">下表显示创建 userPFXCertificate 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="55803-129">The following table shows the properties that are required when you create the userPFXCertificate.</span></span>

|<span data-ttu-id="55803-130">属性</span><span class="sxs-lookup"><span data-stu-id="55803-130">Property</span></span>|<span data-ttu-id="55803-131">类型</span><span class="sxs-lookup"><span data-stu-id="55803-131">Type</span></span>|<span data-ttu-id="55803-132">说明</span><span class="sxs-lookup"><span data-stu-id="55803-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55803-133">id</span><span class="sxs-lookup"><span data-stu-id="55803-133">id</span></span>|<span data-ttu-id="55803-134">String</span><span class="sxs-lookup"><span data-stu-id="55803-134">String</span></span>|<span data-ttu-id="55803-135">PFX 证书的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="55803-135">Unique identifier for the PFX certificate.</span></span>|
|<span data-ttu-id="55803-136">为</span><span class="sxs-lookup"><span data-stu-id="55803-136">thumbprint</span></span>|<span data-ttu-id="55803-137">String</span><span class="sxs-lookup"><span data-stu-id="55803-137">String</span></span>|<span data-ttu-id="55803-138">SHA-1 PFX 证书的指纹。</span><span class="sxs-lookup"><span data-stu-id="55803-138">SHA-1 thumbprint of the PFX certificate.</span></span>|
|<span data-ttu-id="55803-139">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="55803-139">intendedPurpose</span></span>|[<span data-ttu-id="55803-140">userPfxIntendedPurpose</span><span class="sxs-lookup"><span data-stu-id="55803-140">userPfxIntendedPurpose</span></span>](../resources/intune-raimportcerts-userpfxintendedpurpose.md)|<span data-ttu-id="55803-141">证书的预期目的是从部署的角度来看。</span><span class="sxs-lookup"><span data-stu-id="55803-141">Certificate's intended purpose from the point-of-view of deployment.</span></span> <span data-ttu-id="55803-142">可取值为：`unassigned`、`smimeEncryption`、`smimeSigning`、`vpn`、`wifi`。</span><span class="sxs-lookup"><span data-stu-id="55803-142">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|
|<span data-ttu-id="55803-143">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="55803-143">userPrincipalName</span></span>|<span data-ttu-id="55803-144">String</span><span class="sxs-lookup"><span data-stu-id="55803-144">String</span></span>|<span data-ttu-id="55803-145">PFX 证书的用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="55803-145">User Principal Name of the PFX certificate.</span></span>|
|<span data-ttu-id="55803-146">startDateTime</span><span class="sxs-lookup"><span data-stu-id="55803-146">startDateTime</span></span>|<span data-ttu-id="55803-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="55803-147">DateTimeOffset</span></span>|<span data-ttu-id="55803-148">证书的有效期开始日期/时间。</span><span class="sxs-lookup"><span data-stu-id="55803-148">Certificate's validity start date/time.</span></span>|
|<span data-ttu-id="55803-149">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="55803-149">expirationDateTime</span></span>|<span data-ttu-id="55803-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="55803-150">DateTimeOffset</span></span>|<span data-ttu-id="55803-151">证书的有效期到期日期/时间。</span><span class="sxs-lookup"><span data-stu-id="55803-151">Certificate's validity expiration date/time.</span></span>|
|<span data-ttu-id="55803-152">providerName</span><span class="sxs-lookup"><span data-stu-id="55803-152">providerName</span></span>|<span data-ttu-id="55803-153">String</span><span class="sxs-lookup"><span data-stu-id="55803-153">String</span></span>|<span data-ttu-id="55803-154">用于加密此 blob 的加密提供程序。</span><span class="sxs-lookup"><span data-stu-id="55803-154">Crypto provider used to encrypt this blob.</span></span>|
|<span data-ttu-id="55803-155">名</span><span class="sxs-lookup"><span data-stu-id="55803-155">keyName</span></span>|<span data-ttu-id="55803-156">String</span><span class="sxs-lookup"><span data-stu-id="55803-156">String</span></span>|<span data-ttu-id="55803-157">提供程序) 用于对 blob 进行加密的密钥 (的名称。</span><span class="sxs-lookup"><span data-stu-id="55803-157">Name of the key (within the provider) used to encrypt the blob.</span></span>|
|<span data-ttu-id="55803-158">paddingScheme</span><span class="sxs-lookup"><span data-stu-id="55803-158">paddingScheme</span></span>|[<span data-ttu-id="55803-159">userPfxPaddingScheme</span><span class="sxs-lookup"><span data-stu-id="55803-159">userPfxPaddingScheme</span></span>](../resources/intune-raimportcerts-userpfxpaddingscheme.md)|<span data-ttu-id="55803-160">加密/解密过程中提供程序使用的填充方案。</span><span class="sxs-lookup"><span data-stu-id="55803-160">Padding scheme used by the provider during encryption/decryption.</span></span> <span data-ttu-id="55803-161">可取值为：`none`、`pkcs1`、`oaepSha1`、`oaepSha256`、`oaepSha384`、`oaepSha512`。</span><span class="sxs-lookup"><span data-stu-id="55803-161">Possible values are: `none`, `pkcs1`, `oaepSha1`, `oaepSha256`, `oaepSha384`, `oaepSha512`.</span></span>|
|<span data-ttu-id="55803-162">encryptedPfxBlob</span><span class="sxs-lookup"><span data-stu-id="55803-162">encryptedPfxBlob</span></span>|<span data-ttu-id="55803-163">Binary</span><span class="sxs-lookup"><span data-stu-id="55803-163">Binary</span></span>|<span data-ttu-id="55803-164">加密的 PFX blob。</span><span class="sxs-lookup"><span data-stu-id="55803-164">Encrypted PFX blob.</span></span>|
|<span data-ttu-id="55803-165">encryptedPfxPassword</span><span class="sxs-lookup"><span data-stu-id="55803-165">encryptedPfxPassword</span></span>|<span data-ttu-id="55803-166">String</span><span class="sxs-lookup"><span data-stu-id="55803-166">String</span></span>|<span data-ttu-id="55803-167">加密的 PFX 密码。</span><span class="sxs-lookup"><span data-stu-id="55803-167">Encrypted PFX password.</span></span>|
|<span data-ttu-id="55803-168">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="55803-168">createdDateTime</span></span>|<span data-ttu-id="55803-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="55803-169">DateTimeOffset</span></span>|<span data-ttu-id="55803-170">导入此 PFX 证书的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="55803-170">Date/time when this PFX certificate was imported.</span></span>|
|<span data-ttu-id="55803-171">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="55803-171">lastModifiedDateTime</span></span>|<span data-ttu-id="55803-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="55803-172">DateTimeOffset</span></span>|<span data-ttu-id="55803-173">上次修改此 PFX 证书的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="55803-173">Date/time when this PFX certificate was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="55803-174">响应</span><span class="sxs-lookup"><span data-stu-id="55803-174">Response</span></span>
<span data-ttu-id="55803-175">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="55803-175">If successful, this method returns a `201 Created` response code and a [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="55803-176">示例</span><span class="sxs-lookup"><span data-stu-id="55803-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="55803-177">请求</span><span class="sxs-lookup"><span data-stu-id="55803-177">Request</span></span>
<span data-ttu-id="55803-178">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="55803-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="55803-179">响应</span><span class="sxs-lookup"><span data-stu-id="55803-179">Response</span></span>
<span data-ttu-id="55803-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="55803-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





