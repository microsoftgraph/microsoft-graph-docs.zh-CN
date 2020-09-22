---
title: 创建 userPFXCertificate
description: 创建新的 userPFXCertificate 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c86303f417ac40c19a0e2f86702d27f36d5a1720
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48088053"
---
# <a name="create-userpfxcertificate"></a><span data-ttu-id="bc1fc-103">创建 userPFXCertificate</span><span class="sxs-lookup"><span data-stu-id="bc1fc-103">Create userPFXCertificate</span></span>

<span data-ttu-id="bc1fc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bc1fc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bc1fc-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bc1fc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bc1fc-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bc1fc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc1fc-107">创建新的 [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bc1fc-107">Create a new [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bc1fc-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="bc1fc-108">Prerequisites</span></span>
<span data-ttu-id="bc1fc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bc1fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc1fc-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="bc1fc-111">Permission type</span></span>|<span data-ttu-id="bc1fc-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="bc1fc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bc1fc-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bc1fc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bc1fc-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc1fc-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bc1fc-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bc1fc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bc1fc-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bc1fc-116">Not supported.</span></span>|
|<span data-ttu-id="bc1fc-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="bc1fc-117">Application</span></span>|<span data-ttu-id="bc1fc-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc1fc-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bc1fc-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bc1fc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userPfxCertificates
```

## <a name="request-headers"></a><span data-ttu-id="bc1fc-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="bc1fc-120">Request headers</span></span>
|<span data-ttu-id="bc1fc-121">标头</span><span class="sxs-lookup"><span data-stu-id="bc1fc-121">Header</span></span>|<span data-ttu-id="bc1fc-122">值</span><span class="sxs-lookup"><span data-stu-id="bc1fc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bc1fc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bc1fc-123">Authorization</span></span>|<span data-ttu-id="bc1fc-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="bc1fc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bc1fc-125">接受</span><span class="sxs-lookup"><span data-stu-id="bc1fc-125">Accept</span></span>|<span data-ttu-id="bc1fc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bc1fc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bc1fc-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="bc1fc-127">Request body</span></span>
<span data-ttu-id="bc1fc-128">在请求正文中，提供 userPFXCertificate 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bc1fc-128">In the request body, supply a JSON representation for the userPFXCertificate object.</span></span>

<span data-ttu-id="bc1fc-129">下表显示创建 userPFXCertificate 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="bc1fc-129">The following table shows the properties that are required when you create the userPFXCertificate.</span></span>

|<span data-ttu-id="bc1fc-130">属性</span><span class="sxs-lookup"><span data-stu-id="bc1fc-130">Property</span></span>|<span data-ttu-id="bc1fc-131">类型</span><span class="sxs-lookup"><span data-stu-id="bc1fc-131">Type</span></span>|<span data-ttu-id="bc1fc-132">说明</span><span class="sxs-lookup"><span data-stu-id="bc1fc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc1fc-133">id</span><span class="sxs-lookup"><span data-stu-id="bc1fc-133">id</span></span>|<span data-ttu-id="bc1fc-134">字符串</span><span class="sxs-lookup"><span data-stu-id="bc1fc-134">String</span></span>|<span data-ttu-id="bc1fc-135">PFX 证书的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="bc1fc-135">Unique identifier for the PFX certificate.</span></span>|
|<span data-ttu-id="bc1fc-136">为</span><span class="sxs-lookup"><span data-stu-id="bc1fc-136">thumbprint</span></span>|<span data-ttu-id="bc1fc-137">字符串</span><span class="sxs-lookup"><span data-stu-id="bc1fc-137">String</span></span>|<span data-ttu-id="bc1fc-138">SHA-1 PFX 证书的指纹。</span><span class="sxs-lookup"><span data-stu-id="bc1fc-138">SHA-1 thumbprint of the PFX certificate.</span></span>|
|<span data-ttu-id="bc1fc-139">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="bc1fc-139">intendedPurpose</span></span>|[<span data-ttu-id="bc1fc-140">userPfxIntendedPurpose</span><span class="sxs-lookup"><span data-stu-id="bc1fc-140">userPfxIntendedPurpose</span></span>](../resources/intune-raimportcerts-userpfxintendedpurpose.md)|<span data-ttu-id="bc1fc-141">证书的预期目的是从部署的角度来看。</span><span class="sxs-lookup"><span data-stu-id="bc1fc-141">Certificate's intended purpose from the point-of-view of deployment.</span></span> <span data-ttu-id="bc1fc-142">可取值为：`unassigned`、`smimeEncryption`、`smimeSigning`、`vpn`、`wifi`。</span><span class="sxs-lookup"><span data-stu-id="bc1fc-142">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|
|<span data-ttu-id="bc1fc-143">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="bc1fc-143">userPrincipalName</span></span>|<span data-ttu-id="bc1fc-144">字符串</span><span class="sxs-lookup"><span data-stu-id="bc1fc-144">String</span></span>|<span data-ttu-id="bc1fc-145">PFX 证书的用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="bc1fc-145">User Principal Name of the PFX certificate.</span></span>|
|<span data-ttu-id="bc1fc-146">startDateTime</span><span class="sxs-lookup"><span data-stu-id="bc1fc-146">startDateTime</span></span>|<span data-ttu-id="bc1fc-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc1fc-147">DateTimeOffset</span></span>|<span data-ttu-id="bc1fc-148">证书的有效期开始日期/时间。</span><span class="sxs-lookup"><span data-stu-id="bc1fc-148">Certificate's validity start date/time.</span></span>|
|<span data-ttu-id="bc1fc-149">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="bc1fc-149">expirationDateTime</span></span>|<span data-ttu-id="bc1fc-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc1fc-150">DateTimeOffset</span></span>|<span data-ttu-id="bc1fc-151">证书的有效期到期日期/时间。</span><span class="sxs-lookup"><span data-stu-id="bc1fc-151">Certificate's validity expiration date/time.</span></span>|
|<span data-ttu-id="bc1fc-152">providerName</span><span class="sxs-lookup"><span data-stu-id="bc1fc-152">providerName</span></span>|<span data-ttu-id="bc1fc-153">字符串</span><span class="sxs-lookup"><span data-stu-id="bc1fc-153">String</span></span>|<span data-ttu-id="bc1fc-154">用于加密此 blob 的加密提供程序。</span><span class="sxs-lookup"><span data-stu-id="bc1fc-154">Crypto provider used to encrypt this blob.</span></span>|
|<span data-ttu-id="bc1fc-155">名</span><span class="sxs-lookup"><span data-stu-id="bc1fc-155">keyName</span></span>|<span data-ttu-id="bc1fc-156">字符串</span><span class="sxs-lookup"><span data-stu-id="bc1fc-156">String</span></span>|<span data-ttu-id="bc1fc-157">提供程序) 用于对 blob 进行加密的密钥 (的名称。</span><span class="sxs-lookup"><span data-stu-id="bc1fc-157">Name of the key (within the provider) used to encrypt the blob.</span></span>|
|<span data-ttu-id="bc1fc-158">paddingScheme</span><span class="sxs-lookup"><span data-stu-id="bc1fc-158">paddingScheme</span></span>|[<span data-ttu-id="bc1fc-159">userPfxPaddingScheme</span><span class="sxs-lookup"><span data-stu-id="bc1fc-159">userPfxPaddingScheme</span></span>](../resources/intune-raimportcerts-userpfxpaddingscheme.md)|<span data-ttu-id="bc1fc-160">加密/解密过程中提供程序使用的填充方案。</span><span class="sxs-lookup"><span data-stu-id="bc1fc-160">Padding scheme used by the provider during encryption/decryption.</span></span> <span data-ttu-id="bc1fc-161">可取值为：`none`、`pkcs1`、`oaepSha1`、`oaepSha256`、`oaepSha384`、`oaepSha512`。</span><span class="sxs-lookup"><span data-stu-id="bc1fc-161">Possible values are: `none`, `pkcs1`, `oaepSha1`, `oaepSha256`, `oaepSha384`, `oaepSha512`.</span></span>|
|<span data-ttu-id="bc1fc-162">encryptedPfxBlob</span><span class="sxs-lookup"><span data-stu-id="bc1fc-162">encryptedPfxBlob</span></span>|<span data-ttu-id="bc1fc-163">Binary</span><span class="sxs-lookup"><span data-stu-id="bc1fc-163">Binary</span></span>|<span data-ttu-id="bc1fc-164">加密的 PFX blob。</span><span class="sxs-lookup"><span data-stu-id="bc1fc-164">Encrypted PFX blob.</span></span>|
|<span data-ttu-id="bc1fc-165">encryptedPfxPassword</span><span class="sxs-lookup"><span data-stu-id="bc1fc-165">encryptedPfxPassword</span></span>|<span data-ttu-id="bc1fc-166">字符串</span><span class="sxs-lookup"><span data-stu-id="bc1fc-166">String</span></span>|<span data-ttu-id="bc1fc-167">加密的 PFX 密码。</span><span class="sxs-lookup"><span data-stu-id="bc1fc-167">Encrypted PFX password.</span></span>|
|<span data-ttu-id="bc1fc-168">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bc1fc-168">createdDateTime</span></span>|<span data-ttu-id="bc1fc-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc1fc-169">DateTimeOffset</span></span>|<span data-ttu-id="bc1fc-170">导入此 PFX 证书的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="bc1fc-170">Date/time when this PFX certificate was imported.</span></span>|
|<span data-ttu-id="bc1fc-171">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bc1fc-171">lastModifiedDateTime</span></span>|<span data-ttu-id="bc1fc-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc1fc-172">DateTimeOffset</span></span>|<span data-ttu-id="bc1fc-173">上次修改此 PFX 证书的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="bc1fc-173">Date/time when this PFX certificate was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="bc1fc-174">响应</span><span class="sxs-lookup"><span data-stu-id="bc1fc-174">Response</span></span>
<span data-ttu-id="bc1fc-175">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bc1fc-175">If successful, this method returns a `201 Created` response code and a [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bc1fc-176">示例</span><span class="sxs-lookup"><span data-stu-id="bc1fc-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="bc1fc-177">请求</span><span class="sxs-lookup"><span data-stu-id="bc1fc-177">Request</span></span>
<span data-ttu-id="bc1fc-178">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bc1fc-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="bc1fc-179">响应</span><span class="sxs-lookup"><span data-stu-id="bc1fc-179">Response</span></span>
<span data-ttu-id="bc1fc-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bc1fc-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






