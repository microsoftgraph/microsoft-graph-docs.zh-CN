---
title: 创建 pfxUserCertificate
description: 创建新的 pfxUserCertificate 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 44932e657452796a2e7363a8d8f33842e34de086
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/20/2020
ms.locfileid: "42161556"
---
# <a name="create-pfxusercertificate"></a><span data-ttu-id="9296a-103">创建 pfxUserCertificate</span><span class="sxs-lookup"><span data-stu-id="9296a-103">Create pfxUserCertificate</span></span>

> <span data-ttu-id="9296a-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9296a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9296a-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9296a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9296a-106">创建新的[pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9296a-106">Create a new [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9296a-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="9296a-107">Prerequisites</span></span>
<span data-ttu-id="9296a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9296a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9296a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="9296a-110">Permission type</span></span>|<span data-ttu-id="9296a-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9296a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9296a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9296a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9296a-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9296a-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9296a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9296a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9296a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9296a-115">Not supported.</span></span>|
|<span data-ttu-id="9296a-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="9296a-116">Application</span></span>|<span data-ttu-id="9296a-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9296a-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9296a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9296a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /pfxUserCertificates
```

## <a name="request-headers"></a><span data-ttu-id="9296a-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="9296a-119">Request headers</span></span>
|<span data-ttu-id="9296a-120">标头</span><span class="sxs-lookup"><span data-stu-id="9296a-120">Header</span></span>|<span data-ttu-id="9296a-121">值</span><span class="sxs-lookup"><span data-stu-id="9296a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9296a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9296a-122">Authorization</span></span>|<span data-ttu-id="9296a-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9296a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9296a-124">接受</span><span class="sxs-lookup"><span data-stu-id="9296a-124">Accept</span></span>|<span data-ttu-id="9296a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9296a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9296a-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="9296a-126">Request body</span></span>
<span data-ttu-id="9296a-127">在请求正文中，提供 pfxUserCertificate 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9296a-127">In the request body, supply a JSON representation for the pfxUserCertificate object.</span></span>

<span data-ttu-id="9296a-128">下表显示创建 pfxUserCertificate 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="9296a-128">The following table shows the properties that are required when you create the pfxUserCertificate.</span></span>

|<span data-ttu-id="9296a-129">属性</span><span class="sxs-lookup"><span data-stu-id="9296a-129">Property</span></span>|<span data-ttu-id="9296a-130">类型</span><span class="sxs-lookup"><span data-stu-id="9296a-130">Type</span></span>|<span data-ttu-id="9296a-131">说明</span><span class="sxs-lookup"><span data-stu-id="9296a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9296a-132">tenantId</span><span class="sxs-lookup"><span data-stu-id="9296a-132">tenantId</span></span>|<span data-ttu-id="9296a-133">Guid</span><span class="sxs-lookup"><span data-stu-id="9296a-133">Guid</span></span>|<span data-ttu-id="9296a-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9296a-134">Not yet documented</span></span>|
|<span data-ttu-id="9296a-135">userId</span><span class="sxs-lookup"><span data-stu-id="9296a-135">userId</span></span>|<span data-ttu-id="9296a-136">Guid</span><span class="sxs-lookup"><span data-stu-id="9296a-136">Guid</span></span>|<span data-ttu-id="9296a-137">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9296a-137">Not yet documented</span></span>|
|<span data-ttu-id="9296a-138">为</span><span class="sxs-lookup"><span data-stu-id="9296a-138">thumbprint</span></span>|<span data-ttu-id="9296a-139">String</span><span class="sxs-lookup"><span data-stu-id="9296a-139">String</span></span>|<span data-ttu-id="9296a-140">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9296a-140">Not yet documented</span></span>|
|<span data-ttu-id="9296a-141">userUpn</span><span class="sxs-lookup"><span data-stu-id="9296a-141">userUpn</span></span>|<span data-ttu-id="9296a-142">String</span><span class="sxs-lookup"><span data-stu-id="9296a-142">String</span></span>|<span data-ttu-id="9296a-143">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9296a-143">Not yet documented</span></span>|
|<span data-ttu-id="9296a-144">encryptedPfxBlob</span><span class="sxs-lookup"><span data-stu-id="9296a-144">encryptedPfxBlob</span></span>|<span data-ttu-id="9296a-145">String</span><span class="sxs-lookup"><span data-stu-id="9296a-145">String</span></span>|<span data-ttu-id="9296a-146">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9296a-146">Not yet documented</span></span>|
|<span data-ttu-id="9296a-147">encryptedPfxPassword</span><span class="sxs-lookup"><span data-stu-id="9296a-147">encryptedPfxPassword</span></span>|<span data-ttu-id="9296a-148">String</span><span class="sxs-lookup"><span data-stu-id="9296a-148">String</span></span>|<span data-ttu-id="9296a-149">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9296a-149">Not yet documented</span></span>|
|<span data-ttu-id="9296a-150">certStartDate</span><span class="sxs-lookup"><span data-stu-id="9296a-150">certStartDate</span></span>|<span data-ttu-id="9296a-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9296a-151">DateTimeOffset</span></span>|<span data-ttu-id="9296a-152">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9296a-152">Not yet documented</span></span>|
|<span data-ttu-id="9296a-153">certExpirationDate</span><span class="sxs-lookup"><span data-stu-id="9296a-153">certExpirationDate</span></span>|<span data-ttu-id="9296a-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9296a-154">DateTimeOffset</span></span>|<span data-ttu-id="9296a-155">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9296a-155">Not yet documented</span></span>|
|<span data-ttu-id="9296a-156">providerName</span><span class="sxs-lookup"><span data-stu-id="9296a-156">providerName</span></span>|<span data-ttu-id="9296a-157">String</span><span class="sxs-lookup"><span data-stu-id="9296a-157">String</span></span>|<span data-ttu-id="9296a-158">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9296a-158">Not yet documented</span></span>|
|<span data-ttu-id="9296a-159">encryptionKeyName</span><span class="sxs-lookup"><span data-stu-id="9296a-159">encryptionKeyName</span></span>|<span data-ttu-id="9296a-160">String</span><span class="sxs-lookup"><span data-stu-id="9296a-160">String</span></span>|<span data-ttu-id="9296a-161">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9296a-161">Not yet documented</span></span>|
|<span data-ttu-id="9296a-162">paddingScheme</span><span class="sxs-lookup"><span data-stu-id="9296a-162">paddingScheme</span></span>|<span data-ttu-id="9296a-163">Int32</span><span class="sxs-lookup"><span data-stu-id="9296a-163">Int32</span></span>|<span data-ttu-id="9296a-164">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9296a-164">Not yet documented</span></span>|
|<span data-ttu-id="9296a-165">status</span><span class="sxs-lookup"><span data-stu-id="9296a-165">status</span></span>|<span data-ttu-id="9296a-166">Int32</span><span class="sxs-lookup"><span data-stu-id="9296a-166">Int32</span></span>|<span data-ttu-id="9296a-167">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9296a-167">Not yet documented</span></span>|
|<span data-ttu-id="9296a-168">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="9296a-168">intendedPurpose</span></span>|<span data-ttu-id="9296a-169">Int32</span><span class="sxs-lookup"><span data-stu-id="9296a-169">Int32</span></span>|<span data-ttu-id="9296a-170">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9296a-170">Not yet documented</span></span>|
|<span data-ttu-id="9296a-171">createdTime</span><span class="sxs-lookup"><span data-stu-id="9296a-171">createdTime</span></span>|<span data-ttu-id="9296a-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9296a-172">DateTimeOffset</span></span>|<span data-ttu-id="9296a-173">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9296a-173">Not yet documented</span></span>|
|<span data-ttu-id="9296a-174">isDeleted</span><span class="sxs-lookup"><span data-stu-id="9296a-174">isDeleted</span></span>|<span data-ttu-id="9296a-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="9296a-175">Boolean</span></span>|<span data-ttu-id="9296a-176">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9296a-176">Not yet documented</span></span>|
|<span data-ttu-id="9296a-177">lastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="9296a-177">lastModifiedTime</span></span>|<span data-ttu-id="9296a-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9296a-178">DateTimeOffset</span></span>|<span data-ttu-id="9296a-179">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9296a-179">Not yet documented</span></span>|
|<span data-ttu-id="9296a-180">eTag</span><span class="sxs-lookup"><span data-stu-id="9296a-180">eTag</span></span>|<span data-ttu-id="9296a-181">String</span><span class="sxs-lookup"><span data-stu-id="9296a-181">String</span></span>|<span data-ttu-id="9296a-182">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9296a-182">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="9296a-183">响应</span><span class="sxs-lookup"><span data-stu-id="9296a-183">Response</span></span>
<span data-ttu-id="9296a-184">如果成功，此方法在响应`201 Created`正文中返回响应代码和[pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9296a-184">If successful, this method returns a `201 Created` response code and a [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9296a-185">示例</span><span class="sxs-lookup"><span data-stu-id="9296a-185">Example</span></span>

### <a name="request"></a><span data-ttu-id="9296a-186">请求</span><span class="sxs-lookup"><span data-stu-id="9296a-186">Request</span></span>
<span data-ttu-id="9296a-187">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9296a-187">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/pfxUserCertificates
Content-type: application/json
Content-length: 789

{
  "@odata.type": "#microsoft.graph.pfxUserCertificate",
  "tenantId": "f9882bcd-2bcd-f988-cd2b-88f9cd2b88f9",
  "userId": "a991071c-071c-a991-1c07-91a91c0791a9",
  "thumbprint": "Thumbprint value",
  "userUpn": "User Upn value",
  "encryptedPfxBlob": "Encrypted Pfx Blob value",
  "encryptedPfxPassword": "Encrypted Pfx Password value",
  "certStartDate": "2017-01-01T00:01:48.7697664-08:00",
  "certExpirationDate": "2016-12-31T23:56:39.3841403-08:00",
  "providerName": "Provider Name value",
  "encryptionKeyName": "Encryption Key Name value",
  "paddingScheme": 13,
  "status": 6,
  "intendedPurpose": 15,
  "createdTime": "2017-01-01T00:03:18.9597073-08:00",
  "isDeleted": true,
  "lastModifiedTime": "2017-01-01T00:03:18.5958204-08:00",
  "eTag": "ETag value"
}
```

### <a name="response"></a><span data-ttu-id="9296a-188">响应</span><span class="sxs-lookup"><span data-stu-id="9296a-188">Response</span></span>
<span data-ttu-id="9296a-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9296a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 789

{
  "@odata.type": "#microsoft.graph.pfxUserCertificate",
  "tenantId": "f9882bcd-2bcd-f988-cd2b-88f9cd2b88f9",
  "userId": "a991071c-071c-a991-1c07-91a91c0791a9",
  "thumbprint": "Thumbprint value",
  "userUpn": "User Upn value",
  "encryptedPfxBlob": "Encrypted Pfx Blob value",
  "encryptedPfxPassword": "Encrypted Pfx Password value",
  "certStartDate": "2017-01-01T00:01:48.7697664-08:00",
  "certExpirationDate": "2016-12-31T23:56:39.3841403-08:00",
  "providerName": "Provider Name value",
  "encryptionKeyName": "Encryption Key Name value",
  "paddingScheme": 13,
  "status": 6,
  "intendedPurpose": 15,
  "createdTime": "2017-01-01T00:03:18.9597073-08:00",
  "isDeleted": true,
  "lastModifiedTime": "2017-01-01T00:03:18.5958204-08:00",
  "eTag": "ETag value"
}
```





