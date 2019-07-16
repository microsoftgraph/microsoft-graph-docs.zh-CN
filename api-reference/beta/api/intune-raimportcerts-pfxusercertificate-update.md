---
title: 更新 pfxUserCertificate
description: 更新 pfxUserCertificate 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6756a6c35818426790e24d7f348ca760355ffec6
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35725897"
---
# <a name="update-pfxusercertificate"></a><span data-ttu-id="3dfd4-103">更新 pfxUserCertificate</span><span class="sxs-lookup"><span data-stu-id="3dfd4-103">Update pfxUserCertificate</span></span>

> <span data-ttu-id="3dfd4-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3dfd4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3dfd4-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3dfd4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3dfd4-106">更新[pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="3dfd4-106">Update the properties of a [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3dfd4-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="3dfd4-107">Prerequisites</span></span>
<span data-ttu-id="3dfd4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3dfd4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3dfd4-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="3dfd4-110">Permission type</span></span>|<span data-ttu-id="3dfd4-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3dfd4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3dfd4-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3dfd4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3dfd4-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3dfd4-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3dfd4-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3dfd4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3dfd4-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3dfd4-115">Not supported.</span></span>|
|<span data-ttu-id="3dfd4-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="3dfd4-116">Application</span></span>|<span data-ttu-id="3dfd4-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="3dfd4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3dfd4-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3dfd4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /pfxUserCertificates/{pfxUserCertificatesId}
```

## <a name="request-headers"></a><span data-ttu-id="3dfd4-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="3dfd4-119">Request headers</span></span>
|<span data-ttu-id="3dfd4-120">标头</span><span class="sxs-lookup"><span data-stu-id="3dfd4-120">Header</span></span>|<span data-ttu-id="3dfd4-121">值</span><span class="sxs-lookup"><span data-stu-id="3dfd4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3dfd4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3dfd4-122">Authorization</span></span>|<span data-ttu-id="3dfd4-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3dfd4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3dfd4-124">接受</span><span class="sxs-lookup"><span data-stu-id="3dfd4-124">Accept</span></span>|<span data-ttu-id="3dfd4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3dfd4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3dfd4-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="3dfd4-126">Request body</span></span>
<span data-ttu-id="3dfd4-127">在请求正文中, 提供[pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3dfd4-127">In the request body, supply a JSON representation for the [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) object.</span></span>

<span data-ttu-id="3dfd4-128">下表显示创建[pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3dfd4-128">The following table shows the properties that are required when you create the [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md).</span></span>

|<span data-ttu-id="3dfd4-129">属性</span><span class="sxs-lookup"><span data-stu-id="3dfd4-129">Property</span></span>|<span data-ttu-id="3dfd4-130">类型</span><span class="sxs-lookup"><span data-stu-id="3dfd4-130">Type</span></span>|<span data-ttu-id="3dfd4-131">说明</span><span class="sxs-lookup"><span data-stu-id="3dfd4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3dfd4-132">tenantId</span><span class="sxs-lookup"><span data-stu-id="3dfd4-132">tenantId</span></span>|<span data-ttu-id="3dfd4-133">Guid</span><span class="sxs-lookup"><span data-stu-id="3dfd4-133">Guid</span></span>|<span data-ttu-id="3dfd4-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="3dfd4-134">Not yet documented</span></span>|
|<span data-ttu-id="3dfd4-135">userId</span><span class="sxs-lookup"><span data-stu-id="3dfd4-135">userId</span></span>|<span data-ttu-id="3dfd4-136">Guid</span><span class="sxs-lookup"><span data-stu-id="3dfd4-136">Guid</span></span>|<span data-ttu-id="3dfd4-137">尚未记录</span><span class="sxs-lookup"><span data-stu-id="3dfd4-137">Not yet documented</span></span>|
|<span data-ttu-id="3dfd4-138">为</span><span class="sxs-lookup"><span data-stu-id="3dfd4-138">thumbprint</span></span>|<span data-ttu-id="3dfd4-139">String</span><span class="sxs-lookup"><span data-stu-id="3dfd4-139">String</span></span>|<span data-ttu-id="3dfd4-140">尚未记录</span><span class="sxs-lookup"><span data-stu-id="3dfd4-140">Not yet documented</span></span>|
|<span data-ttu-id="3dfd4-141">userUpn</span><span class="sxs-lookup"><span data-stu-id="3dfd4-141">userUpn</span></span>|<span data-ttu-id="3dfd4-142">String</span><span class="sxs-lookup"><span data-stu-id="3dfd4-142">String</span></span>|<span data-ttu-id="3dfd4-143">尚未记录</span><span class="sxs-lookup"><span data-stu-id="3dfd4-143">Not yet documented</span></span>|
|<span data-ttu-id="3dfd4-144">encryptedPfxBlob</span><span class="sxs-lookup"><span data-stu-id="3dfd4-144">encryptedPfxBlob</span></span>|<span data-ttu-id="3dfd4-145">String</span><span class="sxs-lookup"><span data-stu-id="3dfd4-145">String</span></span>|<span data-ttu-id="3dfd4-146">尚未记录</span><span class="sxs-lookup"><span data-stu-id="3dfd4-146">Not yet documented</span></span>|
|<span data-ttu-id="3dfd4-147">encryptedPfxPassword</span><span class="sxs-lookup"><span data-stu-id="3dfd4-147">encryptedPfxPassword</span></span>|<span data-ttu-id="3dfd4-148">String</span><span class="sxs-lookup"><span data-stu-id="3dfd4-148">String</span></span>|<span data-ttu-id="3dfd4-149">尚未记录</span><span class="sxs-lookup"><span data-stu-id="3dfd4-149">Not yet documented</span></span>|
|<span data-ttu-id="3dfd4-150">certStartDate</span><span class="sxs-lookup"><span data-stu-id="3dfd4-150">certStartDate</span></span>|<span data-ttu-id="3dfd4-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3dfd4-151">DateTimeOffset</span></span>|<span data-ttu-id="3dfd4-152">尚未记录</span><span class="sxs-lookup"><span data-stu-id="3dfd4-152">Not yet documented</span></span>|
|<span data-ttu-id="3dfd4-153">certExpirationDate</span><span class="sxs-lookup"><span data-stu-id="3dfd4-153">certExpirationDate</span></span>|<span data-ttu-id="3dfd4-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3dfd4-154">DateTimeOffset</span></span>|<span data-ttu-id="3dfd4-155">尚未记录</span><span class="sxs-lookup"><span data-stu-id="3dfd4-155">Not yet documented</span></span>|
|<span data-ttu-id="3dfd4-156">providerName</span><span class="sxs-lookup"><span data-stu-id="3dfd4-156">providerName</span></span>|<span data-ttu-id="3dfd4-157">String</span><span class="sxs-lookup"><span data-stu-id="3dfd4-157">String</span></span>|<span data-ttu-id="3dfd4-158">尚未记录</span><span class="sxs-lookup"><span data-stu-id="3dfd4-158">Not yet documented</span></span>|
|<span data-ttu-id="3dfd4-159">encryptionKeyName</span><span class="sxs-lookup"><span data-stu-id="3dfd4-159">encryptionKeyName</span></span>|<span data-ttu-id="3dfd4-160">String</span><span class="sxs-lookup"><span data-stu-id="3dfd4-160">String</span></span>|<span data-ttu-id="3dfd4-161">尚未记录</span><span class="sxs-lookup"><span data-stu-id="3dfd4-161">Not yet documented</span></span>|
|<span data-ttu-id="3dfd4-162">paddingScheme</span><span class="sxs-lookup"><span data-stu-id="3dfd4-162">paddingScheme</span></span>|<span data-ttu-id="3dfd4-163">Int32</span><span class="sxs-lookup"><span data-stu-id="3dfd4-163">Int32</span></span>|<span data-ttu-id="3dfd4-164">尚未记录</span><span class="sxs-lookup"><span data-stu-id="3dfd4-164">Not yet documented</span></span>|
|<span data-ttu-id="3dfd4-165">status</span><span class="sxs-lookup"><span data-stu-id="3dfd4-165">status</span></span>|<span data-ttu-id="3dfd4-166">Int32</span><span class="sxs-lookup"><span data-stu-id="3dfd4-166">Int32</span></span>|<span data-ttu-id="3dfd4-167">尚未记录</span><span class="sxs-lookup"><span data-stu-id="3dfd4-167">Not yet documented</span></span>|
|<span data-ttu-id="3dfd4-168">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="3dfd4-168">intendedPurpose</span></span>|<span data-ttu-id="3dfd4-169">Int32</span><span class="sxs-lookup"><span data-stu-id="3dfd4-169">Int32</span></span>|<span data-ttu-id="3dfd4-170">尚未记录</span><span class="sxs-lookup"><span data-stu-id="3dfd4-170">Not yet documented</span></span>|
|<span data-ttu-id="3dfd4-171">createdTime</span><span class="sxs-lookup"><span data-stu-id="3dfd4-171">createdTime</span></span>|<span data-ttu-id="3dfd4-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3dfd4-172">DateTimeOffset</span></span>|<span data-ttu-id="3dfd4-173">尚未记录</span><span class="sxs-lookup"><span data-stu-id="3dfd4-173">Not yet documented</span></span>|
|<span data-ttu-id="3dfd4-174">isDeleted</span><span class="sxs-lookup"><span data-stu-id="3dfd4-174">isDeleted</span></span>|<span data-ttu-id="3dfd4-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfd4-175">Boolean</span></span>|<span data-ttu-id="3dfd4-176">尚未记录</span><span class="sxs-lookup"><span data-stu-id="3dfd4-176">Not yet documented</span></span>|
|<span data-ttu-id="3dfd4-177">lastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="3dfd4-177">lastModifiedTime</span></span>|<span data-ttu-id="3dfd4-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3dfd4-178">DateTimeOffset</span></span>|<span data-ttu-id="3dfd4-179">尚未记录</span><span class="sxs-lookup"><span data-stu-id="3dfd4-179">Not yet documented</span></span>|
|<span data-ttu-id="3dfd4-180">eTag</span><span class="sxs-lookup"><span data-stu-id="3dfd4-180">eTag</span></span>|<span data-ttu-id="3dfd4-181">String</span><span class="sxs-lookup"><span data-stu-id="3dfd4-181">String</span></span>|<span data-ttu-id="3dfd4-182">尚未记录</span><span class="sxs-lookup"><span data-stu-id="3dfd4-182">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="3dfd4-183">响应</span><span class="sxs-lookup"><span data-stu-id="3dfd4-183">Response</span></span>
<span data-ttu-id="3dfd4-184">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="3dfd4-184">If successful, this method returns a `200 OK` response code and an updated [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3dfd4-185">示例</span><span class="sxs-lookup"><span data-stu-id="3dfd4-185">Example</span></span>

### <a name="request"></a><span data-ttu-id="3dfd4-186">请求</span><span class="sxs-lookup"><span data-stu-id="3dfd4-186">Request</span></span>
<span data-ttu-id="3dfd4-187">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3dfd4-187">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3dfd4-188">响应</span><span class="sxs-lookup"><span data-stu-id="3dfd4-188">Response</span></span>
<span data-ttu-id="3dfd4-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3dfd4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





