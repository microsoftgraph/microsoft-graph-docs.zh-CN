---
title: 创建 pfxUserCertificate
description: 创建新的 pfxUserCertificate 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bc74f321c9247311a602fbf2fa7d51dc1d1bbf1c
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868403"
---
# <a name="create-pfxusercertificate"></a><span data-ttu-id="40abf-103">创建 pfxUserCertificate</span><span class="sxs-lookup"><span data-stu-id="40abf-103">Create pfxUserCertificate</span></span>

<span data-ttu-id="40abf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="40abf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="40abf-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="40abf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="40abf-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="40abf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="40abf-107">创建新的 [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="40abf-107">Create a new [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="40abf-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="40abf-108">Prerequisites</span></span>
<span data-ttu-id="40abf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="40abf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40abf-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="40abf-111">Permission type</span></span>|<span data-ttu-id="40abf-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="40abf-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="40abf-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="40abf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="40abf-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40abf-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="40abf-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="40abf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="40abf-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="40abf-116">Not supported.</span></span>|
|<span data-ttu-id="40abf-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="40abf-117">Application</span></span>|<span data-ttu-id="40abf-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40abf-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="40abf-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="40abf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /pfxUserCertificates
```

## <a name="request-headers"></a><span data-ttu-id="40abf-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="40abf-120">Request headers</span></span>
|<span data-ttu-id="40abf-121">标头</span><span class="sxs-lookup"><span data-stu-id="40abf-121">Header</span></span>|<span data-ttu-id="40abf-122">值</span><span class="sxs-lookup"><span data-stu-id="40abf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="40abf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="40abf-123">Authorization</span></span>|<span data-ttu-id="40abf-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="40abf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="40abf-125">接受</span><span class="sxs-lookup"><span data-stu-id="40abf-125">Accept</span></span>|<span data-ttu-id="40abf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="40abf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="40abf-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="40abf-127">Request body</span></span>
<span data-ttu-id="40abf-128">在请求正文中，提供 pfxUserCertificate 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="40abf-128">In the request body, supply a JSON representation for the pfxUserCertificate object.</span></span>

<span data-ttu-id="40abf-129">下表显示创建 pfxUserCertificate 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="40abf-129">The following table shows the properties that are required when you create the pfxUserCertificate.</span></span>

|<span data-ttu-id="40abf-130">属性</span><span class="sxs-lookup"><span data-stu-id="40abf-130">Property</span></span>|<span data-ttu-id="40abf-131">类型</span><span class="sxs-lookup"><span data-stu-id="40abf-131">Type</span></span>|<span data-ttu-id="40abf-132">说明</span><span class="sxs-lookup"><span data-stu-id="40abf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40abf-133">tenantId</span><span class="sxs-lookup"><span data-stu-id="40abf-133">tenantId</span></span>|<span data-ttu-id="40abf-134">Guid</span><span class="sxs-lookup"><span data-stu-id="40abf-134">Guid</span></span>|<span data-ttu-id="40abf-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="40abf-135">Not yet documented</span></span>|
|<span data-ttu-id="40abf-136">userId</span><span class="sxs-lookup"><span data-stu-id="40abf-136">userId</span></span>|<span data-ttu-id="40abf-137">Guid</span><span class="sxs-lookup"><span data-stu-id="40abf-137">Guid</span></span>|<span data-ttu-id="40abf-138">尚未记录</span><span class="sxs-lookup"><span data-stu-id="40abf-138">Not yet documented</span></span>|
|<span data-ttu-id="40abf-139">thumbprint</span><span class="sxs-lookup"><span data-stu-id="40abf-139">thumbprint</span></span>|<span data-ttu-id="40abf-140">String</span><span class="sxs-lookup"><span data-stu-id="40abf-140">String</span></span>|<span data-ttu-id="40abf-141">尚未记录</span><span class="sxs-lookup"><span data-stu-id="40abf-141">Not yet documented</span></span>|
|<span data-ttu-id="40abf-142">userUpn</span><span class="sxs-lookup"><span data-stu-id="40abf-142">userUpn</span></span>|<span data-ttu-id="40abf-143">String</span><span class="sxs-lookup"><span data-stu-id="40abf-143">String</span></span>|<span data-ttu-id="40abf-144">尚未记录</span><span class="sxs-lookup"><span data-stu-id="40abf-144">Not yet documented</span></span>|
|<span data-ttu-id="40abf-145">encryptedPfxBlob</span><span class="sxs-lookup"><span data-stu-id="40abf-145">encryptedPfxBlob</span></span>|<span data-ttu-id="40abf-146">String</span><span class="sxs-lookup"><span data-stu-id="40abf-146">String</span></span>|<span data-ttu-id="40abf-147">尚未记录</span><span class="sxs-lookup"><span data-stu-id="40abf-147">Not yet documented</span></span>|
|<span data-ttu-id="40abf-148">encryptedPfxPassword</span><span class="sxs-lookup"><span data-stu-id="40abf-148">encryptedPfxPassword</span></span>|<span data-ttu-id="40abf-149">String</span><span class="sxs-lookup"><span data-stu-id="40abf-149">String</span></span>|<span data-ttu-id="40abf-150">尚未记录</span><span class="sxs-lookup"><span data-stu-id="40abf-150">Not yet documented</span></span>|
|<span data-ttu-id="40abf-151">certStartDate</span><span class="sxs-lookup"><span data-stu-id="40abf-151">certStartDate</span></span>|<span data-ttu-id="40abf-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="40abf-152">DateTimeOffset</span></span>|<span data-ttu-id="40abf-153">尚未记录</span><span class="sxs-lookup"><span data-stu-id="40abf-153">Not yet documented</span></span>|
|<span data-ttu-id="40abf-154">certExpirationDate</span><span class="sxs-lookup"><span data-stu-id="40abf-154">certExpirationDate</span></span>|<span data-ttu-id="40abf-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="40abf-155">DateTimeOffset</span></span>|<span data-ttu-id="40abf-156">尚未记录</span><span class="sxs-lookup"><span data-stu-id="40abf-156">Not yet documented</span></span>|
|<span data-ttu-id="40abf-157">providerName</span><span class="sxs-lookup"><span data-stu-id="40abf-157">providerName</span></span>|<span data-ttu-id="40abf-158">String</span><span class="sxs-lookup"><span data-stu-id="40abf-158">String</span></span>|<span data-ttu-id="40abf-159">尚未记录</span><span class="sxs-lookup"><span data-stu-id="40abf-159">Not yet documented</span></span>|
|<span data-ttu-id="40abf-160">encryptionKeyName</span><span class="sxs-lookup"><span data-stu-id="40abf-160">encryptionKeyName</span></span>|<span data-ttu-id="40abf-161">String</span><span class="sxs-lookup"><span data-stu-id="40abf-161">String</span></span>|<span data-ttu-id="40abf-162">尚未记录</span><span class="sxs-lookup"><span data-stu-id="40abf-162">Not yet documented</span></span>|
|<span data-ttu-id="40abf-163">paddingScheme</span><span class="sxs-lookup"><span data-stu-id="40abf-163">paddingScheme</span></span>|<span data-ttu-id="40abf-164">Int32</span><span class="sxs-lookup"><span data-stu-id="40abf-164">Int32</span></span>|<span data-ttu-id="40abf-165">尚未记录</span><span class="sxs-lookup"><span data-stu-id="40abf-165">Not yet documented</span></span>|
|<span data-ttu-id="40abf-166">状态</span><span class="sxs-lookup"><span data-stu-id="40abf-166">status</span></span>|<span data-ttu-id="40abf-167">Int32</span><span class="sxs-lookup"><span data-stu-id="40abf-167">Int32</span></span>|<span data-ttu-id="40abf-168">尚未记录</span><span class="sxs-lookup"><span data-stu-id="40abf-168">Not yet documented</span></span>|
|<span data-ttu-id="40abf-169">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="40abf-169">intendedPurpose</span></span>|<span data-ttu-id="40abf-170">Int32</span><span class="sxs-lookup"><span data-stu-id="40abf-170">Int32</span></span>|<span data-ttu-id="40abf-171">尚未记录</span><span class="sxs-lookup"><span data-stu-id="40abf-171">Not yet documented</span></span>|
|<span data-ttu-id="40abf-172">createdTime</span><span class="sxs-lookup"><span data-stu-id="40abf-172">createdTime</span></span>|<span data-ttu-id="40abf-173">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="40abf-173">DateTimeOffset</span></span>|<span data-ttu-id="40abf-174">尚未记录</span><span class="sxs-lookup"><span data-stu-id="40abf-174">Not yet documented</span></span>|
|<span data-ttu-id="40abf-175">isDeleted</span><span class="sxs-lookup"><span data-stu-id="40abf-175">isDeleted</span></span>|<span data-ttu-id="40abf-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="40abf-176">Boolean</span></span>|<span data-ttu-id="40abf-177">尚未记录</span><span class="sxs-lookup"><span data-stu-id="40abf-177">Not yet documented</span></span>|
|<span data-ttu-id="40abf-178">lastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="40abf-178">lastModifiedTime</span></span>|<span data-ttu-id="40abf-179">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="40abf-179">DateTimeOffset</span></span>|<span data-ttu-id="40abf-180">尚未记录</span><span class="sxs-lookup"><span data-stu-id="40abf-180">Not yet documented</span></span>|
|<span data-ttu-id="40abf-181">eTag</span><span class="sxs-lookup"><span data-stu-id="40abf-181">eTag</span></span>|<span data-ttu-id="40abf-182">String</span><span class="sxs-lookup"><span data-stu-id="40abf-182">String</span></span>|<span data-ttu-id="40abf-183">尚未记录</span><span class="sxs-lookup"><span data-stu-id="40abf-183">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="40abf-184">响应</span><span class="sxs-lookup"><span data-stu-id="40abf-184">Response</span></span>
<span data-ttu-id="40abf-185">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="40abf-185">If successful, this method returns a `201 Created` response code and a [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40abf-186">示例</span><span class="sxs-lookup"><span data-stu-id="40abf-186">Example</span></span>

### <a name="request"></a><span data-ttu-id="40abf-187">请求</span><span class="sxs-lookup"><span data-stu-id="40abf-187">Request</span></span>
<span data-ttu-id="40abf-188">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="40abf-188">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="40abf-189">响应</span><span class="sxs-lookup"><span data-stu-id="40abf-189">Response</span></span>
<span data-ttu-id="40abf-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="40abf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




