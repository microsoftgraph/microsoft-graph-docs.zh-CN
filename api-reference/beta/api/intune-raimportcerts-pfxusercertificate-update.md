---
title: 更新 pfxUserCertificate
description: 更新 pfxUserCertificate 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cd11409a4e3a07b15d79104e7815f469d749522f
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48708002"
---
# <a name="update-pfxusercertificate"></a><span data-ttu-id="13bb9-103">更新 pfxUserCertificate</span><span class="sxs-lookup"><span data-stu-id="13bb9-103">Update pfxUserCertificate</span></span>

<span data-ttu-id="13bb9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="13bb9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="13bb9-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="13bb9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="13bb9-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="13bb9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13bb9-107">更新 [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="13bb9-107">Update the properties of a [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="13bb9-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="13bb9-108">Prerequisites</span></span>
<span data-ttu-id="13bb9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="13bb9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13bb9-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="13bb9-111">Permission type</span></span>|<span data-ttu-id="13bb9-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="13bb9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="13bb9-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="13bb9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="13bb9-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13bb9-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="13bb9-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="13bb9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="13bb9-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="13bb9-116">Not supported.</span></span>|
|<span data-ttu-id="13bb9-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="13bb9-117">Application</span></span>|<span data-ttu-id="13bb9-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13bb9-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="13bb9-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="13bb9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /pfxUserCertificates/{pfxUserCertificatesId}
```

## <a name="request-headers"></a><span data-ttu-id="13bb9-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="13bb9-120">Request headers</span></span>
|<span data-ttu-id="13bb9-121">标头</span><span class="sxs-lookup"><span data-stu-id="13bb9-121">Header</span></span>|<span data-ttu-id="13bb9-122">值</span><span class="sxs-lookup"><span data-stu-id="13bb9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="13bb9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="13bb9-123">Authorization</span></span>|<span data-ttu-id="13bb9-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="13bb9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="13bb9-125">接受</span><span class="sxs-lookup"><span data-stu-id="13bb9-125">Accept</span></span>|<span data-ttu-id="13bb9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="13bb9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="13bb9-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="13bb9-127">Request body</span></span>
<span data-ttu-id="13bb9-128">在请求正文中，提供 [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="13bb9-128">In the request body, supply a JSON representation for the [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) object.</span></span>

<span data-ttu-id="13bb9-129">下表显示创建 [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="13bb9-129">The following table shows the properties that are required when you create the [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md).</span></span>

|<span data-ttu-id="13bb9-130">属性</span><span class="sxs-lookup"><span data-stu-id="13bb9-130">Property</span></span>|<span data-ttu-id="13bb9-131">类型</span><span class="sxs-lookup"><span data-stu-id="13bb9-131">Type</span></span>|<span data-ttu-id="13bb9-132">说明</span><span class="sxs-lookup"><span data-stu-id="13bb9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13bb9-133">tenantId</span><span class="sxs-lookup"><span data-stu-id="13bb9-133">tenantId</span></span>|<span data-ttu-id="13bb9-134">Guid</span><span class="sxs-lookup"><span data-stu-id="13bb9-134">Guid</span></span>|<span data-ttu-id="13bb9-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="13bb9-135">Not yet documented</span></span>|
|<span data-ttu-id="13bb9-136">userId</span><span class="sxs-lookup"><span data-stu-id="13bb9-136">userId</span></span>|<span data-ttu-id="13bb9-137">Guid</span><span class="sxs-lookup"><span data-stu-id="13bb9-137">Guid</span></span>|<span data-ttu-id="13bb9-138">尚未记录</span><span class="sxs-lookup"><span data-stu-id="13bb9-138">Not yet documented</span></span>|
|<span data-ttu-id="13bb9-139">为</span><span class="sxs-lookup"><span data-stu-id="13bb9-139">thumbprint</span></span>|<span data-ttu-id="13bb9-140">String</span><span class="sxs-lookup"><span data-stu-id="13bb9-140">String</span></span>|<span data-ttu-id="13bb9-141">尚未记录</span><span class="sxs-lookup"><span data-stu-id="13bb9-141">Not yet documented</span></span>|
|<span data-ttu-id="13bb9-142">userUpn</span><span class="sxs-lookup"><span data-stu-id="13bb9-142">userUpn</span></span>|<span data-ttu-id="13bb9-143">String</span><span class="sxs-lookup"><span data-stu-id="13bb9-143">String</span></span>|<span data-ttu-id="13bb9-144">尚未记录</span><span class="sxs-lookup"><span data-stu-id="13bb9-144">Not yet documented</span></span>|
|<span data-ttu-id="13bb9-145">encryptedPfxBlob</span><span class="sxs-lookup"><span data-stu-id="13bb9-145">encryptedPfxBlob</span></span>|<span data-ttu-id="13bb9-146">String</span><span class="sxs-lookup"><span data-stu-id="13bb9-146">String</span></span>|<span data-ttu-id="13bb9-147">尚未记录</span><span class="sxs-lookup"><span data-stu-id="13bb9-147">Not yet documented</span></span>|
|<span data-ttu-id="13bb9-148">encryptedPfxPassword</span><span class="sxs-lookup"><span data-stu-id="13bb9-148">encryptedPfxPassword</span></span>|<span data-ttu-id="13bb9-149">String</span><span class="sxs-lookup"><span data-stu-id="13bb9-149">String</span></span>|<span data-ttu-id="13bb9-150">尚未记录</span><span class="sxs-lookup"><span data-stu-id="13bb9-150">Not yet documented</span></span>|
|<span data-ttu-id="13bb9-151">certStartDate</span><span class="sxs-lookup"><span data-stu-id="13bb9-151">certStartDate</span></span>|<span data-ttu-id="13bb9-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13bb9-152">DateTimeOffset</span></span>|<span data-ttu-id="13bb9-153">尚未记录</span><span class="sxs-lookup"><span data-stu-id="13bb9-153">Not yet documented</span></span>|
|<span data-ttu-id="13bb9-154">certExpirationDate</span><span class="sxs-lookup"><span data-stu-id="13bb9-154">certExpirationDate</span></span>|<span data-ttu-id="13bb9-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13bb9-155">DateTimeOffset</span></span>|<span data-ttu-id="13bb9-156">尚未记录</span><span class="sxs-lookup"><span data-stu-id="13bb9-156">Not yet documented</span></span>|
|<span data-ttu-id="13bb9-157">providerName</span><span class="sxs-lookup"><span data-stu-id="13bb9-157">providerName</span></span>|<span data-ttu-id="13bb9-158">String</span><span class="sxs-lookup"><span data-stu-id="13bb9-158">String</span></span>|<span data-ttu-id="13bb9-159">尚未记录</span><span class="sxs-lookup"><span data-stu-id="13bb9-159">Not yet documented</span></span>|
|<span data-ttu-id="13bb9-160">encryptionKeyName</span><span class="sxs-lookup"><span data-stu-id="13bb9-160">encryptionKeyName</span></span>|<span data-ttu-id="13bb9-161">String</span><span class="sxs-lookup"><span data-stu-id="13bb9-161">String</span></span>|<span data-ttu-id="13bb9-162">尚未记录</span><span class="sxs-lookup"><span data-stu-id="13bb9-162">Not yet documented</span></span>|
|<span data-ttu-id="13bb9-163">paddingScheme</span><span class="sxs-lookup"><span data-stu-id="13bb9-163">paddingScheme</span></span>|<span data-ttu-id="13bb9-164">Int32</span><span class="sxs-lookup"><span data-stu-id="13bb9-164">Int32</span></span>|<span data-ttu-id="13bb9-165">尚未记录</span><span class="sxs-lookup"><span data-stu-id="13bb9-165">Not yet documented</span></span>|
|<span data-ttu-id="13bb9-166">status</span><span class="sxs-lookup"><span data-stu-id="13bb9-166">status</span></span>|<span data-ttu-id="13bb9-167">Int32</span><span class="sxs-lookup"><span data-stu-id="13bb9-167">Int32</span></span>|<span data-ttu-id="13bb9-168">尚未记录</span><span class="sxs-lookup"><span data-stu-id="13bb9-168">Not yet documented</span></span>|
|<span data-ttu-id="13bb9-169">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="13bb9-169">intendedPurpose</span></span>|<span data-ttu-id="13bb9-170">Int32</span><span class="sxs-lookup"><span data-stu-id="13bb9-170">Int32</span></span>|<span data-ttu-id="13bb9-171">尚未记录</span><span class="sxs-lookup"><span data-stu-id="13bb9-171">Not yet documented</span></span>|
|<span data-ttu-id="13bb9-172">createdTime</span><span class="sxs-lookup"><span data-stu-id="13bb9-172">createdTime</span></span>|<span data-ttu-id="13bb9-173">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13bb9-173">DateTimeOffset</span></span>|<span data-ttu-id="13bb9-174">尚未记录</span><span class="sxs-lookup"><span data-stu-id="13bb9-174">Not yet documented</span></span>|
|<span data-ttu-id="13bb9-175">isDeleted</span><span class="sxs-lookup"><span data-stu-id="13bb9-175">isDeleted</span></span>|<span data-ttu-id="13bb9-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="13bb9-176">Boolean</span></span>|<span data-ttu-id="13bb9-177">尚未记录</span><span class="sxs-lookup"><span data-stu-id="13bb9-177">Not yet documented</span></span>|
|<span data-ttu-id="13bb9-178">lastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="13bb9-178">lastModifiedTime</span></span>|<span data-ttu-id="13bb9-179">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13bb9-179">DateTimeOffset</span></span>|<span data-ttu-id="13bb9-180">尚未记录</span><span class="sxs-lookup"><span data-stu-id="13bb9-180">Not yet documented</span></span>|
|<span data-ttu-id="13bb9-181">eTag</span><span class="sxs-lookup"><span data-stu-id="13bb9-181">eTag</span></span>|<span data-ttu-id="13bb9-182">String</span><span class="sxs-lookup"><span data-stu-id="13bb9-182">String</span></span>|<span data-ttu-id="13bb9-183">尚未记录</span><span class="sxs-lookup"><span data-stu-id="13bb9-183">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="13bb9-184">响应</span><span class="sxs-lookup"><span data-stu-id="13bb9-184">Response</span></span>
<span data-ttu-id="13bb9-185">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="13bb9-185">If successful, this method returns a `200 OK` response code and an updated [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13bb9-186">示例</span><span class="sxs-lookup"><span data-stu-id="13bb9-186">Example</span></span>

### <a name="request"></a><span data-ttu-id="13bb9-187">请求</span><span class="sxs-lookup"><span data-stu-id="13bb9-187">Request</span></span>
<span data-ttu-id="13bb9-188">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="13bb9-188">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/pfxUserCertificates/{pfxUserCertificatesId}
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

### <a name="response"></a><span data-ttu-id="13bb9-189">响应</span><span class="sxs-lookup"><span data-stu-id="13bb9-189">Response</span></span>
<span data-ttu-id="13bb9-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="13bb9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





