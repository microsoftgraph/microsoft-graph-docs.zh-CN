---
title: 更新 userPFXCertificate
description: 更新 userPFXCertificate 对象的属性。
ms.openlocfilehash: 9fde1e8ff073df7acf76119ace0848616424951a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041259"
---
# <a name="update-userpfxcertificate"></a><span data-ttu-id="a16b5-103">更新 userPFXCertificate</span><span class="sxs-lookup"><span data-stu-id="a16b5-103">Update userPFXCertificate</span></span>

> <span data-ttu-id="a16b5-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a16b5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a16b5-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a16b5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a16b5-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="a16b5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a16b5-107">更新[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a16b5-107">Update the properties of a [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a16b5-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="a16b5-108">Prerequisites</span></span>
<span data-ttu-id="a16b5-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="a16b5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a16b5-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a16b5-111">Permission type</span></span>|<span data-ttu-id="a16b5-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a16b5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a16b5-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a16b5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a16b5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a16b5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a16b5-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a16b5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a16b5-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a16b5-116">Not supported.</span></span>|
|<span data-ttu-id="a16b5-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a16b5-117">Application</span></span>|<span data-ttu-id="a16b5-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="a16b5-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a16b5-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a16b5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userPfxCertificates/{userPFXCertificateId}
```

## <a name="request-headers"></a><span data-ttu-id="a16b5-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a16b5-120">Request headers</span></span>
|<span data-ttu-id="a16b5-121">标头</span><span class="sxs-lookup"><span data-stu-id="a16b5-121">Header</span></span>|<span data-ttu-id="a16b5-122">值</span><span class="sxs-lookup"><span data-stu-id="a16b5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a16b5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a16b5-123">Authorization</span></span>|<span data-ttu-id="a16b5-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a16b5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a16b5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a16b5-125">Accept</span></span>|<span data-ttu-id="a16b5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a16b5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a16b5-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a16b5-127">Request body</span></span>
<span data-ttu-id="a16b5-128">在请求正文中，提供[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a16b5-128">In the request body, supply a JSON representation for the [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object.</span></span>

<span data-ttu-id="a16b5-129">下表显示时创建[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a16b5-129">The following table shows the properties that are required when you create the [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md).</span></span>

|<span data-ttu-id="a16b5-130">属性</span><span class="sxs-lookup"><span data-stu-id="a16b5-130">Property</span></span>|<span data-ttu-id="a16b5-131">类型</span><span class="sxs-lookup"><span data-stu-id="a16b5-131">Type</span></span>|<span data-ttu-id="a16b5-132">说明</span><span class="sxs-lookup"><span data-stu-id="a16b5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a16b5-133">id</span><span class="sxs-lookup"><span data-stu-id="a16b5-133">id</span></span>|<span data-ttu-id="a16b5-134">字符串</span><span class="sxs-lookup"><span data-stu-id="a16b5-134">String</span></span>|<span data-ttu-id="a16b5-135">PFX 证书的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="a16b5-135">Unique identifier for the PFX certificate.</span></span>|
|<span data-ttu-id="a16b5-136">指纹</span><span class="sxs-lookup"><span data-stu-id="a16b5-136">thumbprint</span></span>|<span data-ttu-id="a16b5-137">字符串</span><span class="sxs-lookup"><span data-stu-id="a16b5-137">String</span></span>|<span data-ttu-id="a16b5-138">Sha-1 PFX 证书的指纹。</span><span class="sxs-lookup"><span data-stu-id="a16b5-138">SHA-1 thumbprint of the PFX certificate.</span></span>|
|<span data-ttu-id="a16b5-139">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="a16b5-139">intendedPurpose</span></span>|[<span data-ttu-id="a16b5-140">userPfxIntendedPurpose</span><span class="sxs-lookup"><span data-stu-id="a16b5-140">userPfxIntendedPurpose</span></span>](../resources/intune-raimportcerts-userpfxintendedpurpose.md)|<span data-ttu-id="a16b5-141">证书的适用于从部署的视图点的用途。</span><span class="sxs-lookup"><span data-stu-id="a16b5-141">Certificate's intended purpose from the point-of-view of deployment.</span></span> <span data-ttu-id="a16b5-142">可取值为：`unassigned`、`smimeEncryption`、`smimeSigning`、`vpn`、`wifi`。</span><span class="sxs-lookup"><span data-stu-id="a16b5-142">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|
|<span data-ttu-id="a16b5-143">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a16b5-143">userPrincipalName</span></span>|<span data-ttu-id="a16b5-144">字符串</span><span class="sxs-lookup"><span data-stu-id="a16b5-144">String</span></span>|<span data-ttu-id="a16b5-145">PFX 证书的用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="a16b5-145">User Principal Name of the PFX certificate.</span></span>|
|<span data-ttu-id="a16b5-146">startDateTime</span><span class="sxs-lookup"><span data-stu-id="a16b5-146">startDateTime</span></span>|<span data-ttu-id="a16b5-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a16b5-147">DateTimeOffset</span></span>|<span data-ttu-id="a16b5-148">证书的有效性开始日期/时间。</span><span class="sxs-lookup"><span data-stu-id="a16b5-148">Certificate's validity start date/time.</span></span>|
|<span data-ttu-id="a16b5-149">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="a16b5-149">expirationDateTime</span></span>|<span data-ttu-id="a16b5-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a16b5-150">DateTimeOffset</span></span>|<span data-ttu-id="a16b5-151">证书的有效性过期日期/时间。</span><span class="sxs-lookup"><span data-stu-id="a16b5-151">Certificate's validity expiration date/time.</span></span>|
|<span data-ttu-id="a16b5-152">providerName</span><span class="sxs-lookup"><span data-stu-id="a16b5-152">providerName</span></span>|<span data-ttu-id="a16b5-153">字符串</span><span class="sxs-lookup"><span data-stu-id="a16b5-153">String</span></span>|<span data-ttu-id="a16b5-154">用于加密此 blob 的加密提供程序。</span><span class="sxs-lookup"><span data-stu-id="a16b5-154">Crypto provider used to encrypt this blob.</span></span>|
|<span data-ttu-id="a16b5-155">键名</span><span class="sxs-lookup"><span data-stu-id="a16b5-155">keyName</span></span>|<span data-ttu-id="a16b5-156">字符串</span><span class="sxs-lookup"><span data-stu-id="a16b5-156">String</span></span>|<span data-ttu-id="a16b5-157">用于加密 blob （在提供程序） 项的名称。</span><span class="sxs-lookup"><span data-stu-id="a16b5-157">Name of the key (within the provider) used to encrypt the blob.</span></span>|
|<span data-ttu-id="a16b5-158">paddingScheme</span><span class="sxs-lookup"><span data-stu-id="a16b5-158">paddingScheme</span></span>|[<span data-ttu-id="a16b5-159">userPfxPaddingScheme</span><span class="sxs-lookup"><span data-stu-id="a16b5-159">userPfxPaddingScheme</span></span>](../resources/intune-raimportcerts-userpfxpaddingscheme.md)|<span data-ttu-id="a16b5-160">填充在加密/解密过程中使用提供程序的方案。</span><span class="sxs-lookup"><span data-stu-id="a16b5-160">Padding scheme used by the provider during encryption/decryption.</span></span> <span data-ttu-id="a16b5-161">可取值为：`none`、`pkcs1`、`oaepSha1`、`oaepSha256`、`oaepSha384`、`oaepSha512`。</span><span class="sxs-lookup"><span data-stu-id="a16b5-161">Possible values are: `none`, `pkcs1`, `oaepSha1`, `oaepSha256`, `oaepSha384`, `oaepSha512`.</span></span>|
|<span data-ttu-id="a16b5-162">encryptedPfxBlob</span><span class="sxs-lookup"><span data-stu-id="a16b5-162">encryptedPfxBlob</span></span>|<span data-ttu-id="a16b5-163">二进制数</span><span class="sxs-lookup"><span data-stu-id="a16b5-163">Binary</span></span>|<span data-ttu-id="a16b5-164">加密的 PFX blob。</span><span class="sxs-lookup"><span data-stu-id="a16b5-164">Encrypted PFX blob.</span></span>|
|<span data-ttu-id="a16b5-165">encryptedPfxPassword</span><span class="sxs-lookup"><span data-stu-id="a16b5-165">encryptedPfxPassword</span></span>|<span data-ttu-id="a16b5-166">字符串</span><span class="sxs-lookup"><span data-stu-id="a16b5-166">String</span></span>|<span data-ttu-id="a16b5-167">加密的 PFX 密码。</span><span class="sxs-lookup"><span data-stu-id="a16b5-167">Encrypted PFX password.</span></span>|
|<span data-ttu-id="a16b5-168">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a16b5-168">createdDateTime</span></span>|<span data-ttu-id="a16b5-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a16b5-169">DateTimeOffset</span></span>|<span data-ttu-id="a16b5-170">日期/时间时此 PFX 证书已导入。</span><span class="sxs-lookup"><span data-stu-id="a16b5-170">Date/time when this PFX certificate was imported.</span></span>|
|<span data-ttu-id="a16b5-171">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a16b5-171">lastModifiedDateTime</span></span>|<span data-ttu-id="a16b5-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a16b5-172">DateTimeOffset</span></span>|<span data-ttu-id="a16b5-173">上次修改此 PFX 证书时的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="a16b5-173">Date/time when this PFX certificate was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="a16b5-174">响应</span><span class="sxs-lookup"><span data-stu-id="a16b5-174">Response</span></span>
<span data-ttu-id="a16b5-175">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a16b5-175">If successful, this method returns a `200 OK` response code and an updated [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a16b5-176">示例</span><span class="sxs-lookup"><span data-stu-id="a16b5-176">Example</span></span>
### <a name="request"></a><span data-ttu-id="a16b5-177">请求</span><span class="sxs-lookup"><span data-stu-id="a16b5-177">Request</span></span>
<span data-ttu-id="a16b5-178">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a16b5-178">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userPfxCertificates/{userPFXCertificateId}
Content-type: application/json
Content-length: 530

{
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
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```

### <a name="response"></a><span data-ttu-id="a16b5-179">响应</span><span class="sxs-lookup"><span data-stu-id="a16b5-179">Response</span></span>
<span data-ttu-id="a16b5-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a16b5-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





