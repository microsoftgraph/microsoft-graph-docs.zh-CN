---
title: 更新 userPFXCertificate
description: 更新 userPFXCertificate 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8f84d0579805fcb2fed5664a6046b380a9ce08cf
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32527943"
---
# <a name="update-userpfxcertificate"></a><span data-ttu-id="419c7-103">更新 userPFXCertificate</span><span class="sxs-lookup"><span data-stu-id="419c7-103">Update userPFXCertificate</span></span>

> <span data-ttu-id="419c7-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="419c7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="419c7-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="419c7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="419c7-106">更新[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="419c7-106">Update the properties of a [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="419c7-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="419c7-107">Prerequisites</span></span>
<span data-ttu-id="419c7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="419c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="419c7-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="419c7-110">Permission type</span></span>|<span data-ttu-id="419c7-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="419c7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="419c7-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="419c7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="419c7-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="419c7-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="419c7-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="419c7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="419c7-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="419c7-115">Not supported.</span></span>|
|<span data-ttu-id="419c7-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="419c7-116">Application</span></span>|<span data-ttu-id="419c7-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="419c7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="419c7-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="419c7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userPfxCertificates/{userPFXCertificateId}
```

## <a name="request-headers"></a><span data-ttu-id="419c7-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="419c7-119">Request headers</span></span>
|<span data-ttu-id="419c7-120">标头</span><span class="sxs-lookup"><span data-stu-id="419c7-120">Header</span></span>|<span data-ttu-id="419c7-121">值</span><span class="sxs-lookup"><span data-stu-id="419c7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="419c7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="419c7-122">Authorization</span></span>|<span data-ttu-id="419c7-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="419c7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="419c7-124">接受</span><span class="sxs-lookup"><span data-stu-id="419c7-124">Accept</span></span>|<span data-ttu-id="419c7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="419c7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="419c7-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="419c7-126">Request body</span></span>
<span data-ttu-id="419c7-127">在请求正文中, 提供[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="419c7-127">In the request body, supply a JSON representation for the [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object.</span></span>

<span data-ttu-id="419c7-128">下表显示创建[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="419c7-128">The following table shows the properties that are required when you create the [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md).</span></span>

|<span data-ttu-id="419c7-129">属性</span><span class="sxs-lookup"><span data-stu-id="419c7-129">Property</span></span>|<span data-ttu-id="419c7-130">类型</span><span class="sxs-lookup"><span data-stu-id="419c7-130">Type</span></span>|<span data-ttu-id="419c7-131">说明</span><span class="sxs-lookup"><span data-stu-id="419c7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="419c7-132">id</span><span class="sxs-lookup"><span data-stu-id="419c7-132">id</span></span>|<span data-ttu-id="419c7-133">字符串</span><span class="sxs-lookup"><span data-stu-id="419c7-133">String</span></span>|<span data-ttu-id="419c7-134">PFX 证书的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="419c7-134">Unique identifier for the PFX certificate.</span></span>|
|<span data-ttu-id="419c7-135">为</span><span class="sxs-lookup"><span data-stu-id="419c7-135">thumbprint</span></span>|<span data-ttu-id="419c7-136">String</span><span class="sxs-lookup"><span data-stu-id="419c7-136">String</span></span>|<span data-ttu-id="419c7-137">SHA-1 PFX 证书的指纹。</span><span class="sxs-lookup"><span data-stu-id="419c7-137">SHA-1 thumbprint of the PFX certificate.</span></span>|
|<span data-ttu-id="419c7-138">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="419c7-138">intendedPurpose</span></span>|[<span data-ttu-id="419c7-139">userPfxIntendedPurpose</span><span class="sxs-lookup"><span data-stu-id="419c7-139">userPfxIntendedPurpose</span></span>](../resources/intune-raimportcerts-userpfxintendedpurpose.md)|<span data-ttu-id="419c7-140">证书的预期目的是从部署的角度来看。</span><span class="sxs-lookup"><span data-stu-id="419c7-140">Certificate's intended purpose from the point-of-view of deployment.</span></span> <span data-ttu-id="419c7-141">可取值为：`unassigned`、`smimeEncryption`、`smimeSigning`、`vpn` 或 `wifi`。</span><span class="sxs-lookup"><span data-stu-id="419c7-141">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|
|<span data-ttu-id="419c7-142">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="419c7-142">userPrincipalName</span></span>|<span data-ttu-id="419c7-143">String</span><span class="sxs-lookup"><span data-stu-id="419c7-143">String</span></span>|<span data-ttu-id="419c7-144">PFX 证书的用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="419c7-144">User Principal Name of the PFX certificate.</span></span>|
|<span data-ttu-id="419c7-145">startDateTime</span><span class="sxs-lookup"><span data-stu-id="419c7-145">startDateTime</span></span>|<span data-ttu-id="419c7-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="419c7-146">DateTimeOffset</span></span>|<span data-ttu-id="419c7-147">证书的有效期开始日期/时间。</span><span class="sxs-lookup"><span data-stu-id="419c7-147">Certificate's validity start date/time.</span></span>|
|<span data-ttu-id="419c7-148">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="419c7-148">expirationDateTime</span></span>|<span data-ttu-id="419c7-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="419c7-149">DateTimeOffset</span></span>|<span data-ttu-id="419c7-150">证书的有效期到期日期/时间。</span><span class="sxs-lookup"><span data-stu-id="419c7-150">Certificate's validity expiration date/time.</span></span>|
|<span data-ttu-id="419c7-151">providerName</span><span class="sxs-lookup"><span data-stu-id="419c7-151">providerName</span></span>|<span data-ttu-id="419c7-152">String</span><span class="sxs-lookup"><span data-stu-id="419c7-152">String</span></span>|<span data-ttu-id="419c7-153">用于加密此 blob 的加密提供程序。</span><span class="sxs-lookup"><span data-stu-id="419c7-153">Crypto provider used to encrypt this blob.</span></span>|
|<span data-ttu-id="419c7-154">名</span><span class="sxs-lookup"><span data-stu-id="419c7-154">keyName</span></span>|<span data-ttu-id="419c7-155">String</span><span class="sxs-lookup"><span data-stu-id="419c7-155">String</span></span>|<span data-ttu-id="419c7-156">用于对 blob 进行加密的密钥 (在提供程序中) 的名称。</span><span class="sxs-lookup"><span data-stu-id="419c7-156">Name of the key (within the provider) used to encrypt the blob.</span></span>|
|<span data-ttu-id="419c7-157">paddingScheme</span><span class="sxs-lookup"><span data-stu-id="419c7-157">paddingScheme</span></span>|[<span data-ttu-id="419c7-158">userPfxPaddingScheme</span><span class="sxs-lookup"><span data-stu-id="419c7-158">userPfxPaddingScheme</span></span>](../resources/intune-raimportcerts-userpfxpaddingscheme.md)|<span data-ttu-id="419c7-159">加密/解密过程中提供程序使用的填充方案。</span><span class="sxs-lookup"><span data-stu-id="419c7-159">Padding scheme used by the provider during encryption/decryption.</span></span> <span data-ttu-id="419c7-160">可取值为：`none`、`pkcs1`、`oaepSha1`、`oaepSha256`、`oaepSha384`、`oaepSha512`。</span><span class="sxs-lookup"><span data-stu-id="419c7-160">Possible values are: `none`, `pkcs1`, `oaepSha1`, `oaepSha256`, `oaepSha384`, `oaepSha512`.</span></span>|
|<span data-ttu-id="419c7-161">encryptedPfxBlob</span><span class="sxs-lookup"><span data-stu-id="419c7-161">encryptedPfxBlob</span></span>|<span data-ttu-id="419c7-162">Binary</span><span class="sxs-lookup"><span data-stu-id="419c7-162">Binary</span></span>|<span data-ttu-id="419c7-163">加密的 PFX blob。</span><span class="sxs-lookup"><span data-stu-id="419c7-163">Encrypted PFX blob.</span></span>|
|<span data-ttu-id="419c7-164">encryptedPfxPassword</span><span class="sxs-lookup"><span data-stu-id="419c7-164">encryptedPfxPassword</span></span>|<span data-ttu-id="419c7-165">String</span><span class="sxs-lookup"><span data-stu-id="419c7-165">String</span></span>|<span data-ttu-id="419c7-166">加密的 PFX 密码。</span><span class="sxs-lookup"><span data-stu-id="419c7-166">Encrypted PFX password.</span></span>|
|<span data-ttu-id="419c7-167">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="419c7-167">createdDateTime</span></span>|<span data-ttu-id="419c7-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="419c7-168">DateTimeOffset</span></span>|<span data-ttu-id="419c7-169">导入此 PFX 证书的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="419c7-169">Date/time when this PFX certificate was imported.</span></span>|
|<span data-ttu-id="419c7-170">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="419c7-170">lastModifiedDateTime</span></span>|<span data-ttu-id="419c7-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="419c7-171">DateTimeOffset</span></span>|<span data-ttu-id="419c7-172">上次修改此 PFX 证书的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="419c7-172">Date/time when this PFX certificate was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="419c7-173">响应</span><span class="sxs-lookup"><span data-stu-id="419c7-173">Response</span></span>
<span data-ttu-id="419c7-174">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="419c7-174">If successful, this method returns a `200 OK` response code and an updated [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="419c7-175">示例</span><span class="sxs-lookup"><span data-stu-id="419c7-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="419c7-176">请求</span><span class="sxs-lookup"><span data-stu-id="419c7-176">Request</span></span>
<span data-ttu-id="419c7-177">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="419c7-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="419c7-178">响应</span><span class="sxs-lookup"><span data-stu-id="419c7-178">Response</span></span>
<span data-ttu-id="419c7-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="419c7-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



