---
title: 更新 onPremEncryptedPayload
description: 更新 onPremEncryptedPayload 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e1b17e73f773df8cf607789ea203efa1681382aa
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48093264"
---
# <a name="update-onpremencryptedpayload"></a><span data-ttu-id="6da8e-103">更新 onPremEncryptedPayload</span><span class="sxs-lookup"><span data-stu-id="6da8e-103">Update onPremEncryptedPayload</span></span>

<span data-ttu-id="6da8e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6da8e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6da8e-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6da8e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6da8e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6da8e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6da8e-107">更新 [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6da8e-107">Update the properties of a [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6da8e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="6da8e-108">Prerequisites</span></span>
<span data-ttu-id="6da8e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6da8e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6da8e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6da8e-111">Permission type</span></span>|<span data-ttu-id="6da8e-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6da8e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6da8e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6da8e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6da8e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6da8e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6da8e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6da8e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6da8e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6da8e-116">Not supported.</span></span>|
|<span data-ttu-id="6da8e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="6da8e-117">Application</span></span>|<span data-ttu-id="6da8e-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6da8e-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6da8e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6da8e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /onPremEncryptedPayloads/{onPremEncryptedPayloadsId}
```

## <a name="request-headers"></a><span data-ttu-id="6da8e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6da8e-120">Request headers</span></span>
|<span data-ttu-id="6da8e-121">标头</span><span class="sxs-lookup"><span data-stu-id="6da8e-121">Header</span></span>|<span data-ttu-id="6da8e-122">值</span><span class="sxs-lookup"><span data-stu-id="6da8e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6da8e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6da8e-123">Authorization</span></span>|<span data-ttu-id="6da8e-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6da8e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6da8e-125">接受</span><span class="sxs-lookup"><span data-stu-id="6da8e-125">Accept</span></span>|<span data-ttu-id="6da8e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6da8e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6da8e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6da8e-127">Request body</span></span>
<span data-ttu-id="6da8e-128">在请求正文中，提供 [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6da8e-128">In the request body, supply a JSON representation for the [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) object.</span></span>

<span data-ttu-id="6da8e-129">下表显示创建 [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6da8e-129">The following table shows the properties that are required when you create the [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md).</span></span>

|<span data-ttu-id="6da8e-130">属性</span><span class="sxs-lookup"><span data-stu-id="6da8e-130">Property</span></span>|<span data-ttu-id="6da8e-131">类型</span><span class="sxs-lookup"><span data-stu-id="6da8e-131">Type</span></span>|<span data-ttu-id="6da8e-132">说明</span><span class="sxs-lookup"><span data-stu-id="6da8e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6da8e-133">tenantId</span><span class="sxs-lookup"><span data-stu-id="6da8e-133">tenantId</span></span>|<span data-ttu-id="6da8e-134">Guid</span><span class="sxs-lookup"><span data-stu-id="6da8e-134">Guid</span></span>|<span data-ttu-id="6da8e-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6da8e-135">Not yet documented</span></span>|
|<span data-ttu-id="6da8e-136">userId</span><span class="sxs-lookup"><span data-stu-id="6da8e-136">userId</span></span>|<span data-ttu-id="6da8e-137">Guid</span><span class="sxs-lookup"><span data-stu-id="6da8e-137">Guid</span></span>|<span data-ttu-id="6da8e-138">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6da8e-138">Not yet documented</span></span>|
|<span data-ttu-id="6da8e-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="6da8e-139">deviceId</span></span>|<span data-ttu-id="6da8e-140">Guid</span><span class="sxs-lookup"><span data-stu-id="6da8e-140">Guid</span></span>|<span data-ttu-id="6da8e-141">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6da8e-141">Not yet documented</span></span>|
|<span data-ttu-id="6da8e-142">payloadId</span><span class="sxs-lookup"><span data-stu-id="6da8e-142">payloadId</span></span>|<span data-ttu-id="6da8e-143">Guid</span><span class="sxs-lookup"><span data-stu-id="6da8e-143">Guid</span></span>|<span data-ttu-id="6da8e-144">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6da8e-144">Not yet documented</span></span>|
|<span data-ttu-id="6da8e-145">deviceKeyThumbprint</span><span class="sxs-lookup"><span data-stu-id="6da8e-145">deviceKeyThumbprint</span></span>|<span data-ttu-id="6da8e-146">String</span><span class="sxs-lookup"><span data-stu-id="6da8e-146">String</span></span>|<span data-ttu-id="6da8e-147">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6da8e-147">Not yet documented</span></span>|
|<span data-ttu-id="6da8e-148">cert1PayloadUUID</span><span class="sxs-lookup"><span data-stu-id="6da8e-148">cert1PayloadUUID</span></span>|<span data-ttu-id="6da8e-149">String</span><span class="sxs-lookup"><span data-stu-id="6da8e-149">String</span></span>|<span data-ttu-id="6da8e-150">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6da8e-150">Not yet documented</span></span>|
|<span data-ttu-id="6da8e-151">cert2PayloadUUID</span><span class="sxs-lookup"><span data-stu-id="6da8e-151">cert2PayloadUUID</span></span>|<span data-ttu-id="6da8e-152">String</span><span class="sxs-lookup"><span data-stu-id="6da8e-152">String</span></span>|<span data-ttu-id="6da8e-153">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6da8e-153">Not yet documented</span></span>|
|<span data-ttu-id="6da8e-154">cert3PayloadUUID</span><span class="sxs-lookup"><span data-stu-id="6da8e-154">cert3PayloadUUID</span></span>|<span data-ttu-id="6da8e-155">String</span><span class="sxs-lookup"><span data-stu-id="6da8e-155">String</span></span>|<span data-ttu-id="6da8e-156">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6da8e-156">Not yet documented</span></span>|
|<span data-ttu-id="6da8e-157">plistTemplate</span><span class="sxs-lookup"><span data-stu-id="6da8e-157">plistTemplate</span></span>|<span data-ttu-id="6da8e-158">String</span><span class="sxs-lookup"><span data-stu-id="6da8e-158">String</span></span>|<span data-ttu-id="6da8e-159">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6da8e-159">Not yet documented</span></span>|
|<span data-ttu-id="6da8e-160">encryptedBlob</span><span class="sxs-lookup"><span data-stu-id="6da8e-160">encryptedBlob</span></span>|<span data-ttu-id="6da8e-161">Binary</span><span class="sxs-lookup"><span data-stu-id="6da8e-161">Binary</span></span>|<span data-ttu-id="6da8e-162">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6da8e-162">Not yet documented</span></span>|
|<span data-ttu-id="6da8e-163">payloadVersion</span><span class="sxs-lookup"><span data-stu-id="6da8e-163">payloadVersion</span></span>|<span data-ttu-id="6da8e-164">Int32</span><span class="sxs-lookup"><span data-stu-id="6da8e-164">Int32</span></span>|<span data-ttu-id="6da8e-165">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6da8e-165">Not yet documented</span></span>|
|<span data-ttu-id="6da8e-166">状态</span><span class="sxs-lookup"><span data-stu-id="6da8e-166">status</span></span>|<span data-ttu-id="6da8e-167">Int32</span><span class="sxs-lookup"><span data-stu-id="6da8e-167">Int32</span></span>|<span data-ttu-id="6da8e-168">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6da8e-168">Not yet documented</span></span>|
|<span data-ttu-id="6da8e-169">createdTime</span><span class="sxs-lookup"><span data-stu-id="6da8e-169">createdTime</span></span>|<span data-ttu-id="6da8e-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6da8e-170">DateTimeOffset</span></span>|<span data-ttu-id="6da8e-171">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6da8e-171">Not yet documented</span></span>|
|<span data-ttu-id="6da8e-172">lastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="6da8e-172">lastModifiedTime</span></span>|<span data-ttu-id="6da8e-173">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6da8e-173">DateTimeOffset</span></span>|<span data-ttu-id="6da8e-174">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6da8e-174">Not yet documented</span></span>|
|<span data-ttu-id="6da8e-175">eTag</span><span class="sxs-lookup"><span data-stu-id="6da8e-175">eTag</span></span>|<span data-ttu-id="6da8e-176">String</span><span class="sxs-lookup"><span data-stu-id="6da8e-176">String</span></span>|<span data-ttu-id="6da8e-177">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6da8e-177">Not yet documented</span></span>|
|<span data-ttu-id="6da8e-178">isDeleted</span><span class="sxs-lookup"><span data-stu-id="6da8e-178">isDeleted</span></span>|<span data-ttu-id="6da8e-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="6da8e-179">Boolean</span></span>|<span data-ttu-id="6da8e-180">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6da8e-180">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="6da8e-181">响应</span><span class="sxs-lookup"><span data-stu-id="6da8e-181">Response</span></span>
<span data-ttu-id="6da8e-182">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6da8e-182">If successful, this method returns a `200 OK` response code and an updated [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6da8e-183">示例</span><span class="sxs-lookup"><span data-stu-id="6da8e-183">Example</span></span>

### <a name="request"></a><span data-ttu-id="6da8e-184">请求</span><span class="sxs-lookup"><span data-stu-id="6da8e-184">Request</span></span>
<span data-ttu-id="6da8e-185">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6da8e-185">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/onPremEncryptedPayloads/{onPremEncryptedPayloadsId}
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

### <a name="response"></a><span data-ttu-id="6da8e-186">响应</span><span class="sxs-lookup"><span data-stu-id="6da8e-186">Response</span></span>
<span data-ttu-id="6da8e-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6da8e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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






