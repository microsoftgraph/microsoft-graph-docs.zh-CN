---
title: 创建 pfxUserCertificate
description: 创建新的 pfxUserCertificate 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bac316037c22a2a26d6331d32771895cbb6c7db1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42460092"
---
# <a name="create-pfxusercertificate"></a><span data-ttu-id="6e029-103">创建 pfxUserCertificate</span><span class="sxs-lookup"><span data-stu-id="6e029-103">Create pfxUserCertificate</span></span>

<span data-ttu-id="6e029-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="6e029-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6e029-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6e029-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6e029-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6e029-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6e029-107">创建新的[pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6e029-107">Create a new [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6e029-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="6e029-108">Prerequisites</span></span>
<span data-ttu-id="6e029-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6e029-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e029-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6e029-111">Permission type</span></span>|<span data-ttu-id="6e029-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6e029-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6e029-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6e029-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6e029-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e029-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6e029-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6e029-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6e029-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6e029-116">Not supported.</span></span>|
|<span data-ttu-id="6e029-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="6e029-117">Application</span></span>|<span data-ttu-id="6e029-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e029-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6e029-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6e029-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /pfxUserCertificates
```

## <a name="request-headers"></a><span data-ttu-id="6e029-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6e029-120">Request headers</span></span>
|<span data-ttu-id="6e029-121">标头</span><span class="sxs-lookup"><span data-stu-id="6e029-121">Header</span></span>|<span data-ttu-id="6e029-122">值</span><span class="sxs-lookup"><span data-stu-id="6e029-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6e029-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6e029-123">Authorization</span></span>|<span data-ttu-id="6e029-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6e029-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6e029-125">接受</span><span class="sxs-lookup"><span data-stu-id="6e029-125">Accept</span></span>|<span data-ttu-id="6e029-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6e029-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6e029-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6e029-127">Request body</span></span>
<span data-ttu-id="6e029-128">在请求正文中，提供 pfxUserCertificate 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6e029-128">In the request body, supply a JSON representation for the pfxUserCertificate object.</span></span>

<span data-ttu-id="6e029-129">下表显示创建 pfxUserCertificate 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6e029-129">The following table shows the properties that are required when you create the pfxUserCertificate.</span></span>

|<span data-ttu-id="6e029-130">属性</span><span class="sxs-lookup"><span data-stu-id="6e029-130">Property</span></span>|<span data-ttu-id="6e029-131">类型</span><span class="sxs-lookup"><span data-stu-id="6e029-131">Type</span></span>|<span data-ttu-id="6e029-132">说明</span><span class="sxs-lookup"><span data-stu-id="6e029-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e029-133">tenantId</span><span class="sxs-lookup"><span data-stu-id="6e029-133">tenantId</span></span>|<span data-ttu-id="6e029-134">Guid</span><span class="sxs-lookup"><span data-stu-id="6e029-134">Guid</span></span>|<span data-ttu-id="6e029-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6e029-135">Not yet documented</span></span>|
|<span data-ttu-id="6e029-136">userId</span><span class="sxs-lookup"><span data-stu-id="6e029-136">userId</span></span>|<span data-ttu-id="6e029-137">Guid</span><span class="sxs-lookup"><span data-stu-id="6e029-137">Guid</span></span>|<span data-ttu-id="6e029-138">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6e029-138">Not yet documented</span></span>|
|<span data-ttu-id="6e029-139">为</span><span class="sxs-lookup"><span data-stu-id="6e029-139">thumbprint</span></span>|<span data-ttu-id="6e029-140">String</span><span class="sxs-lookup"><span data-stu-id="6e029-140">String</span></span>|<span data-ttu-id="6e029-141">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6e029-141">Not yet documented</span></span>|
|<span data-ttu-id="6e029-142">userUpn</span><span class="sxs-lookup"><span data-stu-id="6e029-142">userUpn</span></span>|<span data-ttu-id="6e029-143">String</span><span class="sxs-lookup"><span data-stu-id="6e029-143">String</span></span>|<span data-ttu-id="6e029-144">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6e029-144">Not yet documented</span></span>|
|<span data-ttu-id="6e029-145">encryptedPfxBlob</span><span class="sxs-lookup"><span data-stu-id="6e029-145">encryptedPfxBlob</span></span>|<span data-ttu-id="6e029-146">String</span><span class="sxs-lookup"><span data-stu-id="6e029-146">String</span></span>|<span data-ttu-id="6e029-147">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6e029-147">Not yet documented</span></span>|
|<span data-ttu-id="6e029-148">encryptedPfxPassword</span><span class="sxs-lookup"><span data-stu-id="6e029-148">encryptedPfxPassword</span></span>|<span data-ttu-id="6e029-149">String</span><span class="sxs-lookup"><span data-stu-id="6e029-149">String</span></span>|<span data-ttu-id="6e029-150">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6e029-150">Not yet documented</span></span>|
|<span data-ttu-id="6e029-151">certStartDate</span><span class="sxs-lookup"><span data-stu-id="6e029-151">certStartDate</span></span>|<span data-ttu-id="6e029-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6e029-152">DateTimeOffset</span></span>|<span data-ttu-id="6e029-153">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6e029-153">Not yet documented</span></span>|
|<span data-ttu-id="6e029-154">certExpirationDate</span><span class="sxs-lookup"><span data-stu-id="6e029-154">certExpirationDate</span></span>|<span data-ttu-id="6e029-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6e029-155">DateTimeOffset</span></span>|<span data-ttu-id="6e029-156">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6e029-156">Not yet documented</span></span>|
|<span data-ttu-id="6e029-157">providerName</span><span class="sxs-lookup"><span data-stu-id="6e029-157">providerName</span></span>|<span data-ttu-id="6e029-158">String</span><span class="sxs-lookup"><span data-stu-id="6e029-158">String</span></span>|<span data-ttu-id="6e029-159">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6e029-159">Not yet documented</span></span>|
|<span data-ttu-id="6e029-160">encryptionKeyName</span><span class="sxs-lookup"><span data-stu-id="6e029-160">encryptionKeyName</span></span>|<span data-ttu-id="6e029-161">String</span><span class="sxs-lookup"><span data-stu-id="6e029-161">String</span></span>|<span data-ttu-id="6e029-162">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6e029-162">Not yet documented</span></span>|
|<span data-ttu-id="6e029-163">paddingScheme</span><span class="sxs-lookup"><span data-stu-id="6e029-163">paddingScheme</span></span>|<span data-ttu-id="6e029-164">Int32</span><span class="sxs-lookup"><span data-stu-id="6e029-164">Int32</span></span>|<span data-ttu-id="6e029-165">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6e029-165">Not yet documented</span></span>|
|<span data-ttu-id="6e029-166">status</span><span class="sxs-lookup"><span data-stu-id="6e029-166">status</span></span>|<span data-ttu-id="6e029-167">Int32</span><span class="sxs-lookup"><span data-stu-id="6e029-167">Int32</span></span>|<span data-ttu-id="6e029-168">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6e029-168">Not yet documented</span></span>|
|<span data-ttu-id="6e029-169">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="6e029-169">intendedPurpose</span></span>|<span data-ttu-id="6e029-170">Int32</span><span class="sxs-lookup"><span data-stu-id="6e029-170">Int32</span></span>|<span data-ttu-id="6e029-171">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6e029-171">Not yet documented</span></span>|
|<span data-ttu-id="6e029-172">createdTime</span><span class="sxs-lookup"><span data-stu-id="6e029-172">createdTime</span></span>|<span data-ttu-id="6e029-173">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6e029-173">DateTimeOffset</span></span>|<span data-ttu-id="6e029-174">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6e029-174">Not yet documented</span></span>|
|<span data-ttu-id="6e029-175">isDeleted</span><span class="sxs-lookup"><span data-stu-id="6e029-175">isDeleted</span></span>|<span data-ttu-id="6e029-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e029-176">Boolean</span></span>|<span data-ttu-id="6e029-177">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6e029-177">Not yet documented</span></span>|
|<span data-ttu-id="6e029-178">lastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="6e029-178">lastModifiedTime</span></span>|<span data-ttu-id="6e029-179">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6e029-179">DateTimeOffset</span></span>|<span data-ttu-id="6e029-180">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6e029-180">Not yet documented</span></span>|
|<span data-ttu-id="6e029-181">eTag</span><span class="sxs-lookup"><span data-stu-id="6e029-181">eTag</span></span>|<span data-ttu-id="6e029-182">String</span><span class="sxs-lookup"><span data-stu-id="6e029-182">String</span></span>|<span data-ttu-id="6e029-183">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6e029-183">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="6e029-184">响应</span><span class="sxs-lookup"><span data-stu-id="6e029-184">Response</span></span>
<span data-ttu-id="6e029-185">如果成功，此方法在响应`201 Created`正文中返回响应代码和[pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6e029-185">If successful, this method returns a `201 Created` response code and a [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e029-186">示例</span><span class="sxs-lookup"><span data-stu-id="6e029-186">Example</span></span>

### <a name="request"></a><span data-ttu-id="6e029-187">请求</span><span class="sxs-lookup"><span data-stu-id="6e029-187">Request</span></span>
<span data-ttu-id="6e029-188">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6e029-188">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6e029-189">响应</span><span class="sxs-lookup"><span data-stu-id="6e029-189">Response</span></span>
<span data-ttu-id="6e029-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6e029-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





