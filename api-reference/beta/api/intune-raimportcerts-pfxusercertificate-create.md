---
title: 创建 pfxUserCertificate
description: 创建新的 pfxUserCertificate 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bda1a3e6b5f2296b3b7b1da62335cfdf7a8d10aa
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35725898"
---
# <a name="create-pfxusercertificate"></a><span data-ttu-id="8c822-103">创建 pfxUserCertificate</span><span class="sxs-lookup"><span data-stu-id="8c822-103">Create pfxUserCertificate</span></span>

> <span data-ttu-id="8c822-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8c822-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8c822-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8c822-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8c822-106">创建新的[pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8c822-106">Create a new [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8c822-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="8c822-107">Prerequisites</span></span>
<span data-ttu-id="8c822-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8c822-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c822-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="8c822-110">Permission type</span></span>|<span data-ttu-id="8c822-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8c822-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8c822-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8c822-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8c822-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c822-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8c822-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8c822-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8c822-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8c822-115">Not supported.</span></span>|
|<span data-ttu-id="8c822-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="8c822-116">Application</span></span>|<span data-ttu-id="8c822-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="8c822-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8c822-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8c822-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /pfxUserCertificates
```

## <a name="request-headers"></a><span data-ttu-id="8c822-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="8c822-119">Request headers</span></span>
|<span data-ttu-id="8c822-120">标头</span><span class="sxs-lookup"><span data-stu-id="8c822-120">Header</span></span>|<span data-ttu-id="8c822-121">值</span><span class="sxs-lookup"><span data-stu-id="8c822-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8c822-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8c822-122">Authorization</span></span>|<span data-ttu-id="8c822-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8c822-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8c822-124">接受</span><span class="sxs-lookup"><span data-stu-id="8c822-124">Accept</span></span>|<span data-ttu-id="8c822-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8c822-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c822-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="8c822-126">Request body</span></span>
<span data-ttu-id="8c822-127">在请求正文中, 提供 pfxUserCertificate 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8c822-127">In the request body, supply a JSON representation for the pfxUserCertificate object.</span></span>

<span data-ttu-id="8c822-128">下表显示创建 pfxUserCertificate 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="8c822-128">The following table shows the properties that are required when you create the pfxUserCertificate.</span></span>

|<span data-ttu-id="8c822-129">属性</span><span class="sxs-lookup"><span data-stu-id="8c822-129">Property</span></span>|<span data-ttu-id="8c822-130">类型</span><span class="sxs-lookup"><span data-stu-id="8c822-130">Type</span></span>|<span data-ttu-id="8c822-131">说明</span><span class="sxs-lookup"><span data-stu-id="8c822-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c822-132">tenantId</span><span class="sxs-lookup"><span data-stu-id="8c822-132">tenantId</span></span>|<span data-ttu-id="8c822-133">Guid</span><span class="sxs-lookup"><span data-stu-id="8c822-133">Guid</span></span>|<span data-ttu-id="8c822-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="8c822-134">Not yet documented</span></span>|
|<span data-ttu-id="8c822-135">userId</span><span class="sxs-lookup"><span data-stu-id="8c822-135">userId</span></span>|<span data-ttu-id="8c822-136">Guid</span><span class="sxs-lookup"><span data-stu-id="8c822-136">Guid</span></span>|<span data-ttu-id="8c822-137">尚未记录</span><span class="sxs-lookup"><span data-stu-id="8c822-137">Not yet documented</span></span>|
|<span data-ttu-id="8c822-138">为</span><span class="sxs-lookup"><span data-stu-id="8c822-138">thumbprint</span></span>|<span data-ttu-id="8c822-139">String</span><span class="sxs-lookup"><span data-stu-id="8c822-139">String</span></span>|<span data-ttu-id="8c822-140">尚未记录</span><span class="sxs-lookup"><span data-stu-id="8c822-140">Not yet documented</span></span>|
|<span data-ttu-id="8c822-141">userUpn</span><span class="sxs-lookup"><span data-stu-id="8c822-141">userUpn</span></span>|<span data-ttu-id="8c822-142">String</span><span class="sxs-lookup"><span data-stu-id="8c822-142">String</span></span>|<span data-ttu-id="8c822-143">尚未记录</span><span class="sxs-lookup"><span data-stu-id="8c822-143">Not yet documented</span></span>|
|<span data-ttu-id="8c822-144">encryptedPfxBlob</span><span class="sxs-lookup"><span data-stu-id="8c822-144">encryptedPfxBlob</span></span>|<span data-ttu-id="8c822-145">String</span><span class="sxs-lookup"><span data-stu-id="8c822-145">String</span></span>|<span data-ttu-id="8c822-146">尚未记录</span><span class="sxs-lookup"><span data-stu-id="8c822-146">Not yet documented</span></span>|
|<span data-ttu-id="8c822-147">encryptedPfxPassword</span><span class="sxs-lookup"><span data-stu-id="8c822-147">encryptedPfxPassword</span></span>|<span data-ttu-id="8c822-148">String</span><span class="sxs-lookup"><span data-stu-id="8c822-148">String</span></span>|<span data-ttu-id="8c822-149">尚未记录</span><span class="sxs-lookup"><span data-stu-id="8c822-149">Not yet documented</span></span>|
|<span data-ttu-id="8c822-150">certStartDate</span><span class="sxs-lookup"><span data-stu-id="8c822-150">certStartDate</span></span>|<span data-ttu-id="8c822-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8c822-151">DateTimeOffset</span></span>|<span data-ttu-id="8c822-152">尚未记录</span><span class="sxs-lookup"><span data-stu-id="8c822-152">Not yet documented</span></span>|
|<span data-ttu-id="8c822-153">certExpirationDate</span><span class="sxs-lookup"><span data-stu-id="8c822-153">certExpirationDate</span></span>|<span data-ttu-id="8c822-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8c822-154">DateTimeOffset</span></span>|<span data-ttu-id="8c822-155">尚未记录</span><span class="sxs-lookup"><span data-stu-id="8c822-155">Not yet documented</span></span>|
|<span data-ttu-id="8c822-156">providerName</span><span class="sxs-lookup"><span data-stu-id="8c822-156">providerName</span></span>|<span data-ttu-id="8c822-157">String</span><span class="sxs-lookup"><span data-stu-id="8c822-157">String</span></span>|<span data-ttu-id="8c822-158">尚未记录</span><span class="sxs-lookup"><span data-stu-id="8c822-158">Not yet documented</span></span>|
|<span data-ttu-id="8c822-159">encryptionKeyName</span><span class="sxs-lookup"><span data-stu-id="8c822-159">encryptionKeyName</span></span>|<span data-ttu-id="8c822-160">String</span><span class="sxs-lookup"><span data-stu-id="8c822-160">String</span></span>|<span data-ttu-id="8c822-161">尚未记录</span><span class="sxs-lookup"><span data-stu-id="8c822-161">Not yet documented</span></span>|
|<span data-ttu-id="8c822-162">paddingScheme</span><span class="sxs-lookup"><span data-stu-id="8c822-162">paddingScheme</span></span>|<span data-ttu-id="8c822-163">Int32</span><span class="sxs-lookup"><span data-stu-id="8c822-163">Int32</span></span>|<span data-ttu-id="8c822-164">尚未记录</span><span class="sxs-lookup"><span data-stu-id="8c822-164">Not yet documented</span></span>|
|<span data-ttu-id="8c822-165">status</span><span class="sxs-lookup"><span data-stu-id="8c822-165">status</span></span>|<span data-ttu-id="8c822-166">Int32</span><span class="sxs-lookup"><span data-stu-id="8c822-166">Int32</span></span>|<span data-ttu-id="8c822-167">尚未记录</span><span class="sxs-lookup"><span data-stu-id="8c822-167">Not yet documented</span></span>|
|<span data-ttu-id="8c822-168">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="8c822-168">intendedPurpose</span></span>|<span data-ttu-id="8c822-169">Int32</span><span class="sxs-lookup"><span data-stu-id="8c822-169">Int32</span></span>|<span data-ttu-id="8c822-170">尚未记录</span><span class="sxs-lookup"><span data-stu-id="8c822-170">Not yet documented</span></span>|
|<span data-ttu-id="8c822-171">createdTime</span><span class="sxs-lookup"><span data-stu-id="8c822-171">createdTime</span></span>|<span data-ttu-id="8c822-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8c822-172">DateTimeOffset</span></span>|<span data-ttu-id="8c822-173">尚未记录</span><span class="sxs-lookup"><span data-stu-id="8c822-173">Not yet documented</span></span>|
|<span data-ttu-id="8c822-174">isDeleted</span><span class="sxs-lookup"><span data-stu-id="8c822-174">isDeleted</span></span>|<span data-ttu-id="8c822-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="8c822-175">Boolean</span></span>|<span data-ttu-id="8c822-176">尚未记录</span><span class="sxs-lookup"><span data-stu-id="8c822-176">Not yet documented</span></span>|
|<span data-ttu-id="8c822-177">lastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="8c822-177">lastModifiedTime</span></span>|<span data-ttu-id="8c822-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8c822-178">DateTimeOffset</span></span>|<span data-ttu-id="8c822-179">尚未记录</span><span class="sxs-lookup"><span data-stu-id="8c822-179">Not yet documented</span></span>|
|<span data-ttu-id="8c822-180">eTag</span><span class="sxs-lookup"><span data-stu-id="8c822-180">eTag</span></span>|<span data-ttu-id="8c822-181">String</span><span class="sxs-lookup"><span data-stu-id="8c822-181">String</span></span>|<span data-ttu-id="8c822-182">尚未记录</span><span class="sxs-lookup"><span data-stu-id="8c822-182">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="8c822-183">响应</span><span class="sxs-lookup"><span data-stu-id="8c822-183">Response</span></span>
<span data-ttu-id="8c822-184">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8c822-184">If successful, this method returns a `201 Created` response code and a [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c822-185">示例</span><span class="sxs-lookup"><span data-stu-id="8c822-185">Example</span></span>

### <a name="request"></a><span data-ttu-id="8c822-186">请求</span><span class="sxs-lookup"><span data-stu-id="8c822-186">Request</span></span>
<span data-ttu-id="8c822-187">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8c822-187">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8c822-188">响应</span><span class="sxs-lookup"><span data-stu-id="8c822-188">Response</span></span>
<span data-ttu-id="8c822-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8c822-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





