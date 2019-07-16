---
title: 更新 onPremEncryptedPayload
description: 更新 onPremEncryptedPayload 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a50048080072c8bcc7feb08cac69d74a18460c19
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35741311"
---
# <a name="update-onpremencryptedpayload"></a><span data-ttu-id="1b19e-103">更新 onPremEncryptedPayload</span><span class="sxs-lookup"><span data-stu-id="1b19e-103">Update onPremEncryptedPayload</span></span>

> <span data-ttu-id="1b19e-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1b19e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1b19e-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1b19e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1b19e-106">更新[onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="1b19e-106">Update the properties of a [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1b19e-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="1b19e-107">Prerequisites</span></span>
<span data-ttu-id="1b19e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1b19e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b19e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="1b19e-110">Permission type</span></span>|<span data-ttu-id="1b19e-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1b19e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1b19e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1b19e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1b19e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b19e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1b19e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1b19e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1b19e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="1b19e-115">Not supported.</span></span>|
|<span data-ttu-id="1b19e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="1b19e-116">Application</span></span>|<span data-ttu-id="1b19e-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="1b19e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1b19e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1b19e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /onPremEncryptedPayloads/{onPremEncryptedPayloadsId}
```

## <a name="request-headers"></a><span data-ttu-id="1b19e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="1b19e-119">Request headers</span></span>
|<span data-ttu-id="1b19e-120">标头</span><span class="sxs-lookup"><span data-stu-id="1b19e-120">Header</span></span>|<span data-ttu-id="1b19e-121">值</span><span class="sxs-lookup"><span data-stu-id="1b19e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1b19e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1b19e-122">Authorization</span></span>|<span data-ttu-id="1b19e-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1b19e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1b19e-124">接受</span><span class="sxs-lookup"><span data-stu-id="1b19e-124">Accept</span></span>|<span data-ttu-id="1b19e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1b19e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1b19e-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="1b19e-126">Request body</span></span>
<span data-ttu-id="1b19e-127">在请求正文中, 提供[onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1b19e-127">In the request body, supply a JSON representation for the [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) object.</span></span>

<span data-ttu-id="1b19e-128">下表显示创建[onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="1b19e-128">The following table shows the properties that are required when you create the [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md).</span></span>

|<span data-ttu-id="1b19e-129">属性</span><span class="sxs-lookup"><span data-stu-id="1b19e-129">Property</span></span>|<span data-ttu-id="1b19e-130">类型</span><span class="sxs-lookup"><span data-stu-id="1b19e-130">Type</span></span>|<span data-ttu-id="1b19e-131">说明</span><span class="sxs-lookup"><span data-stu-id="1b19e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b19e-132">tenantId</span><span class="sxs-lookup"><span data-stu-id="1b19e-132">tenantId</span></span>|<span data-ttu-id="1b19e-133">Guid</span><span class="sxs-lookup"><span data-stu-id="1b19e-133">Guid</span></span>|<span data-ttu-id="1b19e-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="1b19e-134">Not yet documented</span></span>|
|<span data-ttu-id="1b19e-135">userId</span><span class="sxs-lookup"><span data-stu-id="1b19e-135">userId</span></span>|<span data-ttu-id="1b19e-136">Guid</span><span class="sxs-lookup"><span data-stu-id="1b19e-136">Guid</span></span>|<span data-ttu-id="1b19e-137">尚未记录</span><span class="sxs-lookup"><span data-stu-id="1b19e-137">Not yet documented</span></span>|
|<span data-ttu-id="1b19e-138">deviceId</span><span class="sxs-lookup"><span data-stu-id="1b19e-138">deviceId</span></span>|<span data-ttu-id="1b19e-139">Guid</span><span class="sxs-lookup"><span data-stu-id="1b19e-139">Guid</span></span>|<span data-ttu-id="1b19e-140">尚未记录</span><span class="sxs-lookup"><span data-stu-id="1b19e-140">Not yet documented</span></span>|
|<span data-ttu-id="1b19e-141">payloadId</span><span class="sxs-lookup"><span data-stu-id="1b19e-141">payloadId</span></span>|<span data-ttu-id="1b19e-142">Guid</span><span class="sxs-lookup"><span data-stu-id="1b19e-142">Guid</span></span>|<span data-ttu-id="1b19e-143">尚未记录</span><span class="sxs-lookup"><span data-stu-id="1b19e-143">Not yet documented</span></span>|
|<span data-ttu-id="1b19e-144">deviceKeyThumbprint</span><span class="sxs-lookup"><span data-stu-id="1b19e-144">deviceKeyThumbprint</span></span>|<span data-ttu-id="1b19e-145">String</span><span class="sxs-lookup"><span data-stu-id="1b19e-145">String</span></span>|<span data-ttu-id="1b19e-146">尚未记录</span><span class="sxs-lookup"><span data-stu-id="1b19e-146">Not yet documented</span></span>|
|<span data-ttu-id="1b19e-147">cert1PayloadUUID</span><span class="sxs-lookup"><span data-stu-id="1b19e-147">cert1PayloadUUID</span></span>|<span data-ttu-id="1b19e-148">String</span><span class="sxs-lookup"><span data-stu-id="1b19e-148">String</span></span>|<span data-ttu-id="1b19e-149">尚未记录</span><span class="sxs-lookup"><span data-stu-id="1b19e-149">Not yet documented</span></span>|
|<span data-ttu-id="1b19e-150">cert2PayloadUUID</span><span class="sxs-lookup"><span data-stu-id="1b19e-150">cert2PayloadUUID</span></span>|<span data-ttu-id="1b19e-151">String</span><span class="sxs-lookup"><span data-stu-id="1b19e-151">String</span></span>|<span data-ttu-id="1b19e-152">尚未记录</span><span class="sxs-lookup"><span data-stu-id="1b19e-152">Not yet documented</span></span>|
|<span data-ttu-id="1b19e-153">cert3PayloadUUID</span><span class="sxs-lookup"><span data-stu-id="1b19e-153">cert3PayloadUUID</span></span>|<span data-ttu-id="1b19e-154">String</span><span class="sxs-lookup"><span data-stu-id="1b19e-154">String</span></span>|<span data-ttu-id="1b19e-155">尚未记录</span><span class="sxs-lookup"><span data-stu-id="1b19e-155">Not yet documented</span></span>|
|<span data-ttu-id="1b19e-156">plistTemplate</span><span class="sxs-lookup"><span data-stu-id="1b19e-156">plistTemplate</span></span>|<span data-ttu-id="1b19e-157">String</span><span class="sxs-lookup"><span data-stu-id="1b19e-157">String</span></span>|<span data-ttu-id="1b19e-158">尚未记录</span><span class="sxs-lookup"><span data-stu-id="1b19e-158">Not yet documented</span></span>|
|<span data-ttu-id="1b19e-159">encryptedBlob</span><span class="sxs-lookup"><span data-stu-id="1b19e-159">encryptedBlob</span></span>|<span data-ttu-id="1b19e-160">Binary</span><span class="sxs-lookup"><span data-stu-id="1b19e-160">Binary</span></span>|<span data-ttu-id="1b19e-161">尚未记录</span><span class="sxs-lookup"><span data-stu-id="1b19e-161">Not yet documented</span></span>|
|<span data-ttu-id="1b19e-162">payloadVersion</span><span class="sxs-lookup"><span data-stu-id="1b19e-162">payloadVersion</span></span>|<span data-ttu-id="1b19e-163">Int32</span><span class="sxs-lookup"><span data-stu-id="1b19e-163">Int32</span></span>|<span data-ttu-id="1b19e-164">尚未记录</span><span class="sxs-lookup"><span data-stu-id="1b19e-164">Not yet documented</span></span>|
|<span data-ttu-id="1b19e-165">status</span><span class="sxs-lookup"><span data-stu-id="1b19e-165">status</span></span>|<span data-ttu-id="1b19e-166">Int32</span><span class="sxs-lookup"><span data-stu-id="1b19e-166">Int32</span></span>|<span data-ttu-id="1b19e-167">尚未记录</span><span class="sxs-lookup"><span data-stu-id="1b19e-167">Not yet documented</span></span>|
|<span data-ttu-id="1b19e-168">createdTime</span><span class="sxs-lookup"><span data-stu-id="1b19e-168">createdTime</span></span>|<span data-ttu-id="1b19e-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b19e-169">DateTimeOffset</span></span>|<span data-ttu-id="1b19e-170">尚未记录</span><span class="sxs-lookup"><span data-stu-id="1b19e-170">Not yet documented</span></span>|
|<span data-ttu-id="1b19e-171">lastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="1b19e-171">lastModifiedTime</span></span>|<span data-ttu-id="1b19e-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b19e-172">DateTimeOffset</span></span>|<span data-ttu-id="1b19e-173">尚未记录</span><span class="sxs-lookup"><span data-stu-id="1b19e-173">Not yet documented</span></span>|
|<span data-ttu-id="1b19e-174">eTag</span><span class="sxs-lookup"><span data-stu-id="1b19e-174">eTag</span></span>|<span data-ttu-id="1b19e-175">String</span><span class="sxs-lookup"><span data-stu-id="1b19e-175">String</span></span>|<span data-ttu-id="1b19e-176">尚未记录</span><span class="sxs-lookup"><span data-stu-id="1b19e-176">Not yet documented</span></span>|
|<span data-ttu-id="1b19e-177">isDeleted</span><span class="sxs-lookup"><span data-stu-id="1b19e-177">isDeleted</span></span>|<span data-ttu-id="1b19e-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b19e-178">Boolean</span></span>|<span data-ttu-id="1b19e-179">尚未记录</span><span class="sxs-lookup"><span data-stu-id="1b19e-179">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="1b19e-180">响应</span><span class="sxs-lookup"><span data-stu-id="1b19e-180">Response</span></span>
<span data-ttu-id="1b19e-181">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1b19e-181">If successful, this method returns a `200 OK` response code and an updated [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1b19e-182">示例</span><span class="sxs-lookup"><span data-stu-id="1b19e-182">Example</span></span>

### <a name="request"></a><span data-ttu-id="1b19e-183">请求</span><span class="sxs-lookup"><span data-stu-id="1b19e-183">Request</span></span>
<span data-ttu-id="1b19e-184">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1b19e-184">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1b19e-185">响应</span><span class="sxs-lookup"><span data-stu-id="1b19e-185">Response</span></span>
<span data-ttu-id="1b19e-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1b19e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





