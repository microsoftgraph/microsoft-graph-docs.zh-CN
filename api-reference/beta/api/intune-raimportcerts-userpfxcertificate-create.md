---
title: 创建 userPFXCertificate
description: 创建新的 userPFXCertificate 对象。
author: tfitzmac
ms.openlocfilehash: 1f577189dc2e8a420bc4f62d0c7d59510c610ac9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27337735"
---
# <a name="create-userpfxcertificate"></a><span data-ttu-id="ae3c6-103">创建 userPFXCertificate</span><span class="sxs-lookup"><span data-stu-id="ae3c6-103">Create userPFXCertificate</span></span>

> <span data-ttu-id="ae3c6-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ae3c6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ae3c6-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ae3c6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ae3c6-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ae3c6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ae3c6-107">创建新的[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ae3c6-107">Create a new [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ae3c6-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="ae3c6-108">Prerequisites</span></span>
<span data-ttu-id="ae3c6-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="ae3c6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae3c6-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ae3c6-111">Permission type</span></span>|<span data-ttu-id="ae3c6-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ae3c6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ae3c6-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ae3c6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ae3c6-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae3c6-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ae3c6-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ae3c6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ae3c6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ae3c6-116">Not supported.</span></span>|
|<span data-ttu-id="ae3c6-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ae3c6-117">Application</span></span>|<span data-ttu-id="ae3c6-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="ae3c6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ae3c6-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ae3c6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userPfxCertificates
```

## <a name="request-headers"></a><span data-ttu-id="ae3c6-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ae3c6-120">Request headers</span></span>
|<span data-ttu-id="ae3c6-121">标头</span><span class="sxs-lookup"><span data-stu-id="ae3c6-121">Header</span></span>|<span data-ttu-id="ae3c6-122">值</span><span class="sxs-lookup"><span data-stu-id="ae3c6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ae3c6-123">授权</span><span class="sxs-lookup"><span data-stu-id="ae3c6-123">Authorization</span></span>|<span data-ttu-id="ae3c6-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ae3c6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ae3c6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ae3c6-125">Accept</span></span>|<span data-ttu-id="ae3c6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ae3c6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae3c6-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ae3c6-127">Request body</span></span>
<span data-ttu-id="ae3c6-128">在请求正文中，提供 userPFXCertificate 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ae3c6-128">In the request body, supply a JSON representation for the userPFXCertificate object.</span></span>

<span data-ttu-id="ae3c6-129">下表显示时创建 userPFXCertificate 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ae3c6-129">The following table shows the properties that are required when you create the userPFXCertificate.</span></span>

|<span data-ttu-id="ae3c6-130">属性</span><span class="sxs-lookup"><span data-stu-id="ae3c6-130">Property</span></span>|<span data-ttu-id="ae3c6-131">类型</span><span class="sxs-lookup"><span data-stu-id="ae3c6-131">Type</span></span>|<span data-ttu-id="ae3c6-132">说明</span><span class="sxs-lookup"><span data-stu-id="ae3c6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae3c6-133">id</span><span class="sxs-lookup"><span data-stu-id="ae3c6-133">id</span></span>|<span data-ttu-id="ae3c6-134">字符串</span><span class="sxs-lookup"><span data-stu-id="ae3c6-134">String</span></span>|<span data-ttu-id="ae3c6-135">PFX 证书的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="ae3c6-135">Unique identifier for the PFX certificate.</span></span>|
|<span data-ttu-id="ae3c6-136">指纹</span><span class="sxs-lookup"><span data-stu-id="ae3c6-136">thumbprint</span></span>|<span data-ttu-id="ae3c6-137">字符串</span><span class="sxs-lookup"><span data-stu-id="ae3c6-137">String</span></span>|<span data-ttu-id="ae3c6-138">Sha-1 PFX 证书的指纹。</span><span class="sxs-lookup"><span data-stu-id="ae3c6-138">SHA-1 thumbprint of the PFX certificate.</span></span>|
|<span data-ttu-id="ae3c6-139">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="ae3c6-139">intendedPurpose</span></span>|[<span data-ttu-id="ae3c6-140">userPfxIntendedPurpose</span><span class="sxs-lookup"><span data-stu-id="ae3c6-140">userPfxIntendedPurpose</span></span>](../resources/intune-raimportcerts-userpfxintendedpurpose.md)|<span data-ttu-id="ae3c6-141">证书的适用于从部署的视图点的用途。</span><span class="sxs-lookup"><span data-stu-id="ae3c6-141">Certificate's intended purpose from the point-of-view of deployment.</span></span> <span data-ttu-id="ae3c6-142">可取值为：`unassigned`、`smimeEncryption`、`smimeSigning`、`vpn`、`wifi`。</span><span class="sxs-lookup"><span data-stu-id="ae3c6-142">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|
|<span data-ttu-id="ae3c6-143">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ae3c6-143">userPrincipalName</span></span>|<span data-ttu-id="ae3c6-144">字符串</span><span class="sxs-lookup"><span data-stu-id="ae3c6-144">String</span></span>|<span data-ttu-id="ae3c6-145">PFX 证书的用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="ae3c6-145">User Principal Name of the PFX certificate.</span></span>|
|<span data-ttu-id="ae3c6-146">startDateTime</span><span class="sxs-lookup"><span data-stu-id="ae3c6-146">startDateTime</span></span>|<span data-ttu-id="ae3c6-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ae3c6-147">DateTimeOffset</span></span>|<span data-ttu-id="ae3c6-148">证书的有效性开始日期/时间。</span><span class="sxs-lookup"><span data-stu-id="ae3c6-148">Certificate's validity start date/time.</span></span>|
|<span data-ttu-id="ae3c6-149">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="ae3c6-149">expirationDateTime</span></span>|<span data-ttu-id="ae3c6-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ae3c6-150">DateTimeOffset</span></span>|<span data-ttu-id="ae3c6-151">证书的有效性过期日期/时间。</span><span class="sxs-lookup"><span data-stu-id="ae3c6-151">Certificate's validity expiration date/time.</span></span>|
|<span data-ttu-id="ae3c6-152">providerName</span><span class="sxs-lookup"><span data-stu-id="ae3c6-152">providerName</span></span>|<span data-ttu-id="ae3c6-153">字符串</span><span class="sxs-lookup"><span data-stu-id="ae3c6-153">String</span></span>|<span data-ttu-id="ae3c6-154">用于加密此 blob 的加密提供程序。</span><span class="sxs-lookup"><span data-stu-id="ae3c6-154">Crypto provider used to encrypt this blob.</span></span>|
|<span data-ttu-id="ae3c6-155">键名</span><span class="sxs-lookup"><span data-stu-id="ae3c6-155">keyName</span></span>|<span data-ttu-id="ae3c6-156">字符串</span><span class="sxs-lookup"><span data-stu-id="ae3c6-156">String</span></span>|<span data-ttu-id="ae3c6-157">用于加密 blob （在提供程序） 项的名称。</span><span class="sxs-lookup"><span data-stu-id="ae3c6-157">Name of the key (within the provider) used to encrypt the blob.</span></span>|
|<span data-ttu-id="ae3c6-158">paddingScheme</span><span class="sxs-lookup"><span data-stu-id="ae3c6-158">paddingScheme</span></span>|[<span data-ttu-id="ae3c6-159">userPfxPaddingScheme</span><span class="sxs-lookup"><span data-stu-id="ae3c6-159">userPfxPaddingScheme</span></span>](../resources/intune-raimportcerts-userpfxpaddingscheme.md)|<span data-ttu-id="ae3c6-160">填充在加密/解密过程中使用提供程序的方案。</span><span class="sxs-lookup"><span data-stu-id="ae3c6-160">Padding scheme used by the provider during encryption/decryption.</span></span> <span data-ttu-id="ae3c6-161">可取值为：`none`、`pkcs1`、`oaepSha1`、`oaepSha256`、`oaepSha384`、`oaepSha512`。</span><span class="sxs-lookup"><span data-stu-id="ae3c6-161">Possible values are: `none`, `pkcs1`, `oaepSha1`, `oaepSha256`, `oaepSha384`, `oaepSha512`.</span></span>|
|<span data-ttu-id="ae3c6-162">encryptedPfxBlob</span><span class="sxs-lookup"><span data-stu-id="ae3c6-162">encryptedPfxBlob</span></span>|<span data-ttu-id="ae3c6-163">Binary</span><span class="sxs-lookup"><span data-stu-id="ae3c6-163">Binary</span></span>|<span data-ttu-id="ae3c6-164">加密的 PFX blob。</span><span class="sxs-lookup"><span data-stu-id="ae3c6-164">Encrypted PFX blob.</span></span>|
|<span data-ttu-id="ae3c6-165">encryptedPfxPassword</span><span class="sxs-lookup"><span data-stu-id="ae3c6-165">encryptedPfxPassword</span></span>|<span data-ttu-id="ae3c6-166">字符串</span><span class="sxs-lookup"><span data-stu-id="ae3c6-166">String</span></span>|<span data-ttu-id="ae3c6-167">加密的 PFX 密码。</span><span class="sxs-lookup"><span data-stu-id="ae3c6-167">Encrypted PFX password.</span></span>|
|<span data-ttu-id="ae3c6-168">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ae3c6-168">createdDateTime</span></span>|<span data-ttu-id="ae3c6-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ae3c6-169">DateTimeOffset</span></span>|<span data-ttu-id="ae3c6-170">日期/时间时此 PFX 证书已导入。</span><span class="sxs-lookup"><span data-stu-id="ae3c6-170">Date/time when this PFX certificate was imported.</span></span>|
|<span data-ttu-id="ae3c6-171">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ae3c6-171">lastModifiedDateTime</span></span>|<span data-ttu-id="ae3c6-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ae3c6-172">DateTimeOffset</span></span>|<span data-ttu-id="ae3c6-173">上次修改此 PFX 证书时的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="ae3c6-173">Date/time when this PFX certificate was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="ae3c6-174">响应</span><span class="sxs-lookup"><span data-stu-id="ae3c6-174">Response</span></span>
<span data-ttu-id="ae3c6-175">如果成功，此方法返回`201 Created`响应代码和响应正文中的[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ae3c6-175">If successful, this method returns a `201 Created` response code and a [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae3c6-176">示例</span><span class="sxs-lookup"><span data-stu-id="ae3c6-176">Example</span></span>
### <a name="request"></a><span data-ttu-id="ae3c6-177">请求</span><span class="sxs-lookup"><span data-stu-id="ae3c6-177">Request</span></span>
<span data-ttu-id="ae3c6-178">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ae3c6-178">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userPfxCertificates
Content-type: application/json
Content-length: 587

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
  "encryptedPfxPassword": "Encrypted Pfx Password value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```

### <a name="response"></a><span data-ttu-id="ae3c6-179">响应</span><span class="sxs-lookup"><span data-stu-id="ae3c6-179">Response</span></span>
<span data-ttu-id="ae3c6-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ae3c6-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





