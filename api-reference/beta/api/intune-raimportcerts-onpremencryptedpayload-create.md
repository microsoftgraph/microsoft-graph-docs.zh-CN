---
title: 创建 onPremEncryptedPayload
description: 创建新的 onPremEncryptedPayload 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6d59d96b814505f4c19cf3a0257b2744ac907182
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868385"
---
# <a name="create-onpremencryptedpayload"></a><span data-ttu-id="564b0-103">创建 onPremEncryptedPayload</span><span class="sxs-lookup"><span data-stu-id="564b0-103">Create onPremEncryptedPayload</span></span>

<span data-ttu-id="564b0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="564b0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="564b0-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="564b0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="564b0-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="564b0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="564b0-107">创建新的 [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="564b0-107">Create a new [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="564b0-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="564b0-108">Prerequisites</span></span>
<span data-ttu-id="564b0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="564b0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="564b0-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="564b0-111">Permission type</span></span>|<span data-ttu-id="564b0-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="564b0-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="564b0-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="564b0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="564b0-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="564b0-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="564b0-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="564b0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="564b0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="564b0-116">Not supported.</span></span>|
|<span data-ttu-id="564b0-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="564b0-117">Application</span></span>|<span data-ttu-id="564b0-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="564b0-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="564b0-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="564b0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /onPremEncryptedPayloads
```

## <a name="request-headers"></a><span data-ttu-id="564b0-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="564b0-120">Request headers</span></span>
|<span data-ttu-id="564b0-121">标头</span><span class="sxs-lookup"><span data-stu-id="564b0-121">Header</span></span>|<span data-ttu-id="564b0-122">值</span><span class="sxs-lookup"><span data-stu-id="564b0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="564b0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="564b0-123">Authorization</span></span>|<span data-ttu-id="564b0-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="564b0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="564b0-125">接受</span><span class="sxs-lookup"><span data-stu-id="564b0-125">Accept</span></span>|<span data-ttu-id="564b0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="564b0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="564b0-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="564b0-127">Request body</span></span>
<span data-ttu-id="564b0-128">在请求正文中，提供 onPremEncryptedPayload 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="564b0-128">In the request body, supply a JSON representation for the onPremEncryptedPayload object.</span></span>

<span data-ttu-id="564b0-129">下表显示创建 onPremEncryptedPayload 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="564b0-129">The following table shows the properties that are required when you create the onPremEncryptedPayload.</span></span>

|<span data-ttu-id="564b0-130">属性</span><span class="sxs-lookup"><span data-stu-id="564b0-130">Property</span></span>|<span data-ttu-id="564b0-131">类型</span><span class="sxs-lookup"><span data-stu-id="564b0-131">Type</span></span>|<span data-ttu-id="564b0-132">说明</span><span class="sxs-lookup"><span data-stu-id="564b0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="564b0-133">tenantId</span><span class="sxs-lookup"><span data-stu-id="564b0-133">tenantId</span></span>|<span data-ttu-id="564b0-134">Guid</span><span class="sxs-lookup"><span data-stu-id="564b0-134">Guid</span></span>|<span data-ttu-id="564b0-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="564b0-135">Not yet documented</span></span>|
|<span data-ttu-id="564b0-136">userId</span><span class="sxs-lookup"><span data-stu-id="564b0-136">userId</span></span>|<span data-ttu-id="564b0-137">Guid</span><span class="sxs-lookup"><span data-stu-id="564b0-137">Guid</span></span>|<span data-ttu-id="564b0-138">尚未记录</span><span class="sxs-lookup"><span data-stu-id="564b0-138">Not yet documented</span></span>|
|<span data-ttu-id="564b0-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="564b0-139">deviceId</span></span>|<span data-ttu-id="564b0-140">Guid</span><span class="sxs-lookup"><span data-stu-id="564b0-140">Guid</span></span>|<span data-ttu-id="564b0-141">尚未记录</span><span class="sxs-lookup"><span data-stu-id="564b0-141">Not yet documented</span></span>|
|<span data-ttu-id="564b0-142">payloadId</span><span class="sxs-lookup"><span data-stu-id="564b0-142">payloadId</span></span>|<span data-ttu-id="564b0-143">Guid</span><span class="sxs-lookup"><span data-stu-id="564b0-143">Guid</span></span>|<span data-ttu-id="564b0-144">尚未记录</span><span class="sxs-lookup"><span data-stu-id="564b0-144">Not yet documented</span></span>|
|<span data-ttu-id="564b0-145">deviceKeyThumbprint</span><span class="sxs-lookup"><span data-stu-id="564b0-145">deviceKeyThumbprint</span></span>|<span data-ttu-id="564b0-146">String</span><span class="sxs-lookup"><span data-stu-id="564b0-146">String</span></span>|<span data-ttu-id="564b0-147">尚未记录</span><span class="sxs-lookup"><span data-stu-id="564b0-147">Not yet documented</span></span>|
|<span data-ttu-id="564b0-148">cert1PayloadUUID</span><span class="sxs-lookup"><span data-stu-id="564b0-148">cert1PayloadUUID</span></span>|<span data-ttu-id="564b0-149">String</span><span class="sxs-lookup"><span data-stu-id="564b0-149">String</span></span>|<span data-ttu-id="564b0-150">尚未记录</span><span class="sxs-lookup"><span data-stu-id="564b0-150">Not yet documented</span></span>|
|<span data-ttu-id="564b0-151">cert2PayloadUUID</span><span class="sxs-lookup"><span data-stu-id="564b0-151">cert2PayloadUUID</span></span>|<span data-ttu-id="564b0-152">String</span><span class="sxs-lookup"><span data-stu-id="564b0-152">String</span></span>|<span data-ttu-id="564b0-153">尚未记录</span><span class="sxs-lookup"><span data-stu-id="564b0-153">Not yet documented</span></span>|
|<span data-ttu-id="564b0-154">cert3PayloadUUID</span><span class="sxs-lookup"><span data-stu-id="564b0-154">cert3PayloadUUID</span></span>|<span data-ttu-id="564b0-155">String</span><span class="sxs-lookup"><span data-stu-id="564b0-155">String</span></span>|<span data-ttu-id="564b0-156">尚未记录</span><span class="sxs-lookup"><span data-stu-id="564b0-156">Not yet documented</span></span>|
|<span data-ttu-id="564b0-157">plistTemplate</span><span class="sxs-lookup"><span data-stu-id="564b0-157">plistTemplate</span></span>|<span data-ttu-id="564b0-158">String</span><span class="sxs-lookup"><span data-stu-id="564b0-158">String</span></span>|<span data-ttu-id="564b0-159">尚未记录</span><span class="sxs-lookup"><span data-stu-id="564b0-159">Not yet documented</span></span>|
|<span data-ttu-id="564b0-160">encryptedBlob</span><span class="sxs-lookup"><span data-stu-id="564b0-160">encryptedBlob</span></span>|<span data-ttu-id="564b0-161">二进制</span><span class="sxs-lookup"><span data-stu-id="564b0-161">Binary</span></span>|<span data-ttu-id="564b0-162">尚未记录</span><span class="sxs-lookup"><span data-stu-id="564b0-162">Not yet documented</span></span>|
|<span data-ttu-id="564b0-163">payloadVersion</span><span class="sxs-lookup"><span data-stu-id="564b0-163">payloadVersion</span></span>|<span data-ttu-id="564b0-164">Int32</span><span class="sxs-lookup"><span data-stu-id="564b0-164">Int32</span></span>|<span data-ttu-id="564b0-165">尚未记录</span><span class="sxs-lookup"><span data-stu-id="564b0-165">Not yet documented</span></span>|
|<span data-ttu-id="564b0-166">状态</span><span class="sxs-lookup"><span data-stu-id="564b0-166">status</span></span>|<span data-ttu-id="564b0-167">Int32</span><span class="sxs-lookup"><span data-stu-id="564b0-167">Int32</span></span>|<span data-ttu-id="564b0-168">尚未记录</span><span class="sxs-lookup"><span data-stu-id="564b0-168">Not yet documented</span></span>|
|<span data-ttu-id="564b0-169">createdTime</span><span class="sxs-lookup"><span data-stu-id="564b0-169">createdTime</span></span>|<span data-ttu-id="564b0-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="564b0-170">DateTimeOffset</span></span>|<span data-ttu-id="564b0-171">尚未记录</span><span class="sxs-lookup"><span data-stu-id="564b0-171">Not yet documented</span></span>|
|<span data-ttu-id="564b0-172">lastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="564b0-172">lastModifiedTime</span></span>|<span data-ttu-id="564b0-173">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="564b0-173">DateTimeOffset</span></span>|<span data-ttu-id="564b0-174">尚未记录</span><span class="sxs-lookup"><span data-stu-id="564b0-174">Not yet documented</span></span>|
|<span data-ttu-id="564b0-175">eTag</span><span class="sxs-lookup"><span data-stu-id="564b0-175">eTag</span></span>|<span data-ttu-id="564b0-176">String</span><span class="sxs-lookup"><span data-stu-id="564b0-176">String</span></span>|<span data-ttu-id="564b0-177">尚未记录</span><span class="sxs-lookup"><span data-stu-id="564b0-177">Not yet documented</span></span>|
|<span data-ttu-id="564b0-178">isDeleted</span><span class="sxs-lookup"><span data-stu-id="564b0-178">isDeleted</span></span>|<span data-ttu-id="564b0-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="564b0-179">Boolean</span></span>|<span data-ttu-id="564b0-180">尚未记录</span><span class="sxs-lookup"><span data-stu-id="564b0-180">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="564b0-181">响应</span><span class="sxs-lookup"><span data-stu-id="564b0-181">Response</span></span>
<span data-ttu-id="564b0-182">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="564b0-182">If successful, this method returns a `201 Created` response code and a [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="564b0-183">示例</span><span class="sxs-lookup"><span data-stu-id="564b0-183">Example</span></span>

### <a name="request"></a><span data-ttu-id="564b0-184">请求</span><span class="sxs-lookup"><span data-stu-id="564b0-184">Request</span></span>
<span data-ttu-id="564b0-185">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="564b0-185">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/onPremEncryptedPayloads
Content-type: application/json
Content-length: 781

{
  "@odata.type": "#microsoft.graph.onPremEncryptedPayload",
  "tenantId": "f9882bcd-2bcd-f988-cd2b-88f9cd2b88f9",
  "userId": "a991071c-071c-a991-1c07-91a91c0791a9",
  "deviceId": "6de0af45-af45-6de0-45af-e06d45afe06d",
  "payloadId": "f12f6c03-6c03-f12f-036c-2ff1036c2ff1",
  "deviceKeyThumbprint": "Device Key Thumbprint value",
  "cert1PayloadUUID": "Cert1Payload UUID value",
  "cert2PayloadUUID": "Cert2Payload UUID value",
  "cert3PayloadUUID": "Cert3Payload UUID value",
  "plistTemplate": "Plist Template value",
  "encryptedBlob": "ZW5jcnlwdGVkQmxvYg==",
  "payloadVersion": 14,
  "status": 6,
  "createdTime": "2017-01-01T00:03:18.9597073-08:00",
  "lastModifiedTime": "2017-01-01T00:03:18.5958204-08:00",
  "eTag": "ETag value",
  "isDeleted": true
}
```

### <a name="response"></a><span data-ttu-id="564b0-186">响应</span><span class="sxs-lookup"><span data-stu-id="564b0-186">Response</span></span>
<span data-ttu-id="564b0-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="564b0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 781

{
  "@odata.type": "#microsoft.graph.onPremEncryptedPayload",
  "tenantId": "f9882bcd-2bcd-f988-cd2b-88f9cd2b88f9",
  "userId": "a991071c-071c-a991-1c07-91a91c0791a9",
  "deviceId": "6de0af45-af45-6de0-45af-e06d45afe06d",
  "payloadId": "f12f6c03-6c03-f12f-036c-2ff1036c2ff1",
  "deviceKeyThumbprint": "Device Key Thumbprint value",
  "cert1PayloadUUID": "Cert1Payload UUID value",
  "cert2PayloadUUID": "Cert2Payload UUID value",
  "cert3PayloadUUID": "Cert3Payload UUID value",
  "plistTemplate": "Plist Template value",
  "encryptedBlob": "ZW5jcnlwdGVkQmxvYg==",
  "payloadVersion": 14,
  "status": 6,
  "createdTime": "2017-01-01T00:03:18.9597073-08:00",
  "lastModifiedTime": "2017-01-01T00:03:18.5958204-08:00",
  "eTag": "ETag value",
  "isDeleted": true
}
```




