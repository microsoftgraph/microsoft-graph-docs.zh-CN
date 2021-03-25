---
title: 更新 userPFXCertificate
description: 更新 userPFXCertificate 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 745faa38ded53e357cf78a56fcf0b4ab1b2298db
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51152185"
---
# <a name="update-userpfxcertificate"></a><span data-ttu-id="94126-103">更新 userPFXCertificate</span><span class="sxs-lookup"><span data-stu-id="94126-103">Update userPFXCertificate</span></span>

<span data-ttu-id="94126-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="94126-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="94126-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="94126-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="94126-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="94126-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="94126-107">更新 [userPFXCertificate 对象](../resources/intune-raimportcerts-userpfxcertificate.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="94126-107">Update the properties of a [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="94126-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="94126-108">Prerequisites</span></span>
<span data-ttu-id="94126-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="94126-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94126-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="94126-111">Permission type</span></span>|<span data-ttu-id="94126-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="94126-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="94126-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="94126-113">Delegated (work or school account)</span></span>|<span data-ttu-id="94126-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94126-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="94126-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="94126-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="94126-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="94126-116">Not supported.</span></span>|
|<span data-ttu-id="94126-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="94126-117">Application</span></span>|<span data-ttu-id="94126-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94126-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="94126-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="94126-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userPfxCertificates/{userPFXCertificateId}
```

## <a name="request-headers"></a><span data-ttu-id="94126-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="94126-120">Request headers</span></span>
|<span data-ttu-id="94126-121">标头</span><span class="sxs-lookup"><span data-stu-id="94126-121">Header</span></span>|<span data-ttu-id="94126-122">值</span><span class="sxs-lookup"><span data-stu-id="94126-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="94126-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="94126-123">Authorization</span></span>|<span data-ttu-id="94126-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="94126-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="94126-125">接受</span><span class="sxs-lookup"><span data-stu-id="94126-125">Accept</span></span>|<span data-ttu-id="94126-126">application/json</span><span class="sxs-lookup"><span data-stu-id="94126-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="94126-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="94126-127">Request body</span></span>
<span data-ttu-id="94126-128">在请求正文中，提供 [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="94126-128">In the request body, supply a JSON representation for the [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object.</span></span>

<span data-ttu-id="94126-129">下表显示创建 [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="94126-129">The following table shows the properties that are required when you create the [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md).</span></span>

|<span data-ttu-id="94126-130">属性</span><span class="sxs-lookup"><span data-stu-id="94126-130">Property</span></span>|<span data-ttu-id="94126-131">类型</span><span class="sxs-lookup"><span data-stu-id="94126-131">Type</span></span>|<span data-ttu-id="94126-132">说明</span><span class="sxs-lookup"><span data-stu-id="94126-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94126-133">id</span><span class="sxs-lookup"><span data-stu-id="94126-133">id</span></span>|<span data-ttu-id="94126-134">String</span><span class="sxs-lookup"><span data-stu-id="94126-134">String</span></span>|<span data-ttu-id="94126-135">PFX 证书的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="94126-135">Unique identifier for the PFX certificate.</span></span>|
|<span data-ttu-id="94126-136">thumbprint</span><span class="sxs-lookup"><span data-stu-id="94126-136">thumbprint</span></span>|<span data-ttu-id="94126-137">String</span><span class="sxs-lookup"><span data-stu-id="94126-137">String</span></span>|<span data-ttu-id="94126-138">PFX 证书的 SHA-1 指纹。</span><span class="sxs-lookup"><span data-stu-id="94126-138">SHA-1 thumbprint of the PFX certificate.</span></span>|
|<span data-ttu-id="94126-139">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="94126-139">intendedPurpose</span></span>|[<span data-ttu-id="94126-140">userPfxIntendedPurpose</span><span class="sxs-lookup"><span data-stu-id="94126-140">userPfxIntendedPurpose</span></span>](../resources/intune-raimportcerts-userpfxintendedpurpose.md)|<span data-ttu-id="94126-141">从部署的角度来看，证书的目的。</span><span class="sxs-lookup"><span data-stu-id="94126-141">Certificate's intended purpose from the point-of-view of deployment.</span></span> <span data-ttu-id="94126-142">可取值为：`unassigned`、`smimeEncryption`、`smimeSigning`、`vpn`、`wifi`。</span><span class="sxs-lookup"><span data-stu-id="94126-142">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|
|<span data-ttu-id="94126-143">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="94126-143">userPrincipalName</span></span>|<span data-ttu-id="94126-144">String</span><span class="sxs-lookup"><span data-stu-id="94126-144">String</span></span>|<span data-ttu-id="94126-145">用户主体 PFX 证书的名称。</span><span class="sxs-lookup"><span data-stu-id="94126-145">User Principal Name of the PFX certificate.</span></span>|
|<span data-ttu-id="94126-146">startDateTime</span><span class="sxs-lookup"><span data-stu-id="94126-146">startDateTime</span></span>|<span data-ttu-id="94126-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="94126-147">DateTimeOffset</span></span>|<span data-ttu-id="94126-148">证书的有效期开始日期/时间。</span><span class="sxs-lookup"><span data-stu-id="94126-148">Certificate's validity start date/time.</span></span>|
|<span data-ttu-id="94126-149">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="94126-149">expirationDateTime</span></span>|<span data-ttu-id="94126-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="94126-150">DateTimeOffset</span></span>|<span data-ttu-id="94126-151">证书的有效期过期日期/时间。</span><span class="sxs-lookup"><span data-stu-id="94126-151">Certificate's validity expiration date/time.</span></span>|
|<span data-ttu-id="94126-152">providerName</span><span class="sxs-lookup"><span data-stu-id="94126-152">providerName</span></span>|<span data-ttu-id="94126-153">String</span><span class="sxs-lookup"><span data-stu-id="94126-153">String</span></span>|<span data-ttu-id="94126-154">用于加密此 blob 的加密提供程序。</span><span class="sxs-lookup"><span data-stu-id="94126-154">Crypto provider used to encrypt this blob.</span></span>|
|<span data-ttu-id="94126-155">keyName</span><span class="sxs-lookup"><span data-stu-id="94126-155">keyName</span></span>|<span data-ttu-id="94126-156">String</span><span class="sxs-lookup"><span data-stu-id="94126-156">String</span></span>|<span data-ttu-id="94126-157">提供程序中用于 (blob 的) 的名称。</span><span class="sxs-lookup"><span data-stu-id="94126-157">Name of the key (within the provider) used to encrypt the blob.</span></span>|
|<span data-ttu-id="94126-158">paddingScheme</span><span class="sxs-lookup"><span data-stu-id="94126-158">paddingScheme</span></span>|[<span data-ttu-id="94126-159">userPfxPaddingScheme</span><span class="sxs-lookup"><span data-stu-id="94126-159">userPfxPaddingScheme</span></span>](../resources/intune-raimportcerts-userpfxpaddingscheme.md)|<span data-ttu-id="94126-160">提供程序在加密/解密期间使用的填充方案。</span><span class="sxs-lookup"><span data-stu-id="94126-160">Padding scheme used by the provider during encryption/decryption.</span></span> <span data-ttu-id="94126-161">可取值为：`none`、`pkcs1`、`oaepSha1`、`oaepSha256`、`oaepSha384`、`oaepSha512`。</span><span class="sxs-lookup"><span data-stu-id="94126-161">Possible values are: `none`, `pkcs1`, `oaepSha1`, `oaepSha256`, `oaepSha384`, `oaepSha512`.</span></span>|
|<span data-ttu-id="94126-162">encryptedPfxBlob</span><span class="sxs-lookup"><span data-stu-id="94126-162">encryptedPfxBlob</span></span>|<span data-ttu-id="94126-163">Binary</span><span class="sxs-lookup"><span data-stu-id="94126-163">Binary</span></span>|<span data-ttu-id="94126-164">加密的 PFX blob。</span><span class="sxs-lookup"><span data-stu-id="94126-164">Encrypted PFX blob.</span></span>|
|<span data-ttu-id="94126-165">encryptedPfxPassword</span><span class="sxs-lookup"><span data-stu-id="94126-165">encryptedPfxPassword</span></span>|<span data-ttu-id="94126-166">String</span><span class="sxs-lookup"><span data-stu-id="94126-166">String</span></span>|<span data-ttu-id="94126-167">加密的 PFX 密码。</span><span class="sxs-lookup"><span data-stu-id="94126-167">Encrypted PFX password.</span></span>|
|<span data-ttu-id="94126-168">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="94126-168">createdDateTime</span></span>|<span data-ttu-id="94126-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="94126-169">DateTimeOffset</span></span>|<span data-ttu-id="94126-170">导入此 PFX 证书的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="94126-170">Date/time when this PFX certificate was imported.</span></span>|
|<span data-ttu-id="94126-171">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="94126-171">lastModifiedDateTime</span></span>|<span data-ttu-id="94126-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="94126-172">DateTimeOffset</span></span>|<span data-ttu-id="94126-173">上次修改此 PFX 证书的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="94126-173">Date/time when this PFX certificate was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="94126-174">响应</span><span class="sxs-lookup"><span data-stu-id="94126-174">Response</span></span>
<span data-ttu-id="94126-175">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="94126-175">If successful, this method returns a `200 OK` response code and an updated [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="94126-176">示例</span><span class="sxs-lookup"><span data-stu-id="94126-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="94126-177">请求</span><span class="sxs-lookup"><span data-stu-id="94126-177">Request</span></span>
<span data-ttu-id="94126-178">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="94126-178">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userPfxCertificates/{userPFXCertificateId}
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

### <a name="response"></a><span data-ttu-id="94126-179">响应</span><span class="sxs-lookup"><span data-stu-id="94126-179">Response</span></span>
<span data-ttu-id="94126-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="94126-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




