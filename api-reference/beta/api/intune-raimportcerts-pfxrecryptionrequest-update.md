---
title: 更新 pfxRecryptionRequest
description: 更新 pfxRecryptionRequest 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b66443c43646fd592c995d322b88b6c69a6f51b9
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49304957"
---
# <a name="update-pfxrecryptionrequest"></a><span data-ttu-id="9716d-103">更新 pfxRecryptionRequest</span><span class="sxs-lookup"><span data-stu-id="9716d-103">Update pfxRecryptionRequest</span></span>

<span data-ttu-id="9716d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9716d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9716d-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9716d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9716d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9716d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9716d-107">更新 [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9716d-107">Update the properties of a [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9716d-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="9716d-108">Prerequisites</span></span>
<span data-ttu-id="9716d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9716d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9716d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9716d-111">Permission type</span></span>|<span data-ttu-id="9716d-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9716d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9716d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9716d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9716d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9716d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9716d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9716d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9716d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9716d-116">Not supported.</span></span>|
|<span data-ttu-id="9716d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9716d-117">Application</span></span>|<span data-ttu-id="9716d-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9716d-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9716d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9716d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /pfxRecryptionRequests/{pfxRecryptionRequestsId}
```

## <a name="request-headers"></a><span data-ttu-id="9716d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9716d-120">Request headers</span></span>
|<span data-ttu-id="9716d-121">标头</span><span class="sxs-lookup"><span data-stu-id="9716d-121">Header</span></span>|<span data-ttu-id="9716d-122">值</span><span class="sxs-lookup"><span data-stu-id="9716d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9716d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9716d-123">Authorization</span></span>|<span data-ttu-id="9716d-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9716d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9716d-125">接受</span><span class="sxs-lookup"><span data-stu-id="9716d-125">Accept</span></span>|<span data-ttu-id="9716d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9716d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9716d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9716d-127">Request body</span></span>
<span data-ttu-id="9716d-128">在请求正文中，提供 [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9716d-128">In the request body, supply a JSON representation for the [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) object.</span></span>

<span data-ttu-id="9716d-129">下表显示创建 [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="9716d-129">The following table shows the properties that are required when you create the [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md).</span></span>

|<span data-ttu-id="9716d-130">属性</span><span class="sxs-lookup"><span data-stu-id="9716d-130">Property</span></span>|<span data-ttu-id="9716d-131">类型</span><span class="sxs-lookup"><span data-stu-id="9716d-131">Type</span></span>|<span data-ttu-id="9716d-132">Description</span><span class="sxs-lookup"><span data-stu-id="9716d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9716d-133">tenantId</span><span class="sxs-lookup"><span data-stu-id="9716d-133">tenantId</span></span>|<span data-ttu-id="9716d-134">Guid</span><span class="sxs-lookup"><span data-stu-id="9716d-134">Guid</span></span>|<span data-ttu-id="9716d-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9716d-135">Not yet documented</span></span>|
|<span data-ttu-id="9716d-136">userId</span><span class="sxs-lookup"><span data-stu-id="9716d-136">userId</span></span>|<span data-ttu-id="9716d-137">Guid</span><span class="sxs-lookup"><span data-stu-id="9716d-137">Guid</span></span>|<span data-ttu-id="9716d-138">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9716d-138">Not yet documented</span></span>|
|<span data-ttu-id="9716d-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="9716d-139">deviceId</span></span>|<span data-ttu-id="9716d-140">Guid</span><span class="sxs-lookup"><span data-stu-id="9716d-140">Guid</span></span>|<span data-ttu-id="9716d-141">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9716d-141">Not yet documented</span></span>|
|<span data-ttu-id="9716d-142">profileId</span><span class="sxs-lookup"><span data-stu-id="9716d-142">profileId</span></span>|<span data-ttu-id="9716d-143">Guid</span><span class="sxs-lookup"><span data-stu-id="9716d-143">Guid</span></span>|<span data-ttu-id="9716d-144">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9716d-144">Not yet documented</span></span>|
|<span data-ttu-id="9716d-145">为</span><span class="sxs-lookup"><span data-stu-id="9716d-145">thumbprint</span></span>|<span data-ttu-id="9716d-146">String</span><span class="sxs-lookup"><span data-stu-id="9716d-146">String</span></span>|<span data-ttu-id="9716d-147">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9716d-147">Not yet documented</span></span>|
|<span data-ttu-id="9716d-148">deviceKeyThumbprint</span><span class="sxs-lookup"><span data-stu-id="9716d-148">deviceKeyThumbprint</span></span>|<span data-ttu-id="9716d-149">String</span><span class="sxs-lookup"><span data-stu-id="9716d-149">String</span></span>|<span data-ttu-id="9716d-150">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9716d-150">Not yet documented</span></span>|
|<span data-ttu-id="9716d-151">status</span><span class="sxs-lookup"><span data-stu-id="9716d-151">status</span></span>|<span data-ttu-id="9716d-152">Int32</span><span class="sxs-lookup"><span data-stu-id="9716d-152">Int32</span></span>|<span data-ttu-id="9716d-153">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9716d-153">Not yet documented</span></span>|
|<span data-ttu-id="9716d-154">sourceType</span><span class="sxs-lookup"><span data-stu-id="9716d-154">sourceType</span></span>|<span data-ttu-id="9716d-155">Int32</span><span class="sxs-lookup"><span data-stu-id="9716d-155">Int32</span></span>|<span data-ttu-id="9716d-156">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9716d-156">Not yet documented</span></span>|
|<span data-ttu-id="9716d-157">createdTime</span><span class="sxs-lookup"><span data-stu-id="9716d-157">createdTime</span></span>|<span data-ttu-id="9716d-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9716d-158">DateTimeOffset</span></span>|<span data-ttu-id="9716d-159">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9716d-159">Not yet documented</span></span>|
|<span data-ttu-id="9716d-160">lastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="9716d-160">lastModifiedTime</span></span>|<span data-ttu-id="9716d-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9716d-161">DateTimeOffset</span></span>|<span data-ttu-id="9716d-162">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9716d-162">Not yet documented</span></span>|
|<span data-ttu-id="9716d-163">isDeleted</span><span class="sxs-lookup"><span data-stu-id="9716d-163">isDeleted</span></span>|<span data-ttu-id="9716d-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="9716d-164">Boolean</span></span>|<span data-ttu-id="9716d-165">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9716d-165">Not yet documented</span></span>|
|<span data-ttu-id="9716d-166">eTag</span><span class="sxs-lookup"><span data-stu-id="9716d-166">eTag</span></span>|<span data-ttu-id="9716d-167">String</span><span class="sxs-lookup"><span data-stu-id="9716d-167">String</span></span>|<span data-ttu-id="9716d-168">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9716d-168">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="9716d-169">响应</span><span class="sxs-lookup"><span data-stu-id="9716d-169">Response</span></span>
<span data-ttu-id="9716d-170">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9716d-170">If successful, this method returns a `200 OK` response code and an updated [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9716d-171">示例</span><span class="sxs-lookup"><span data-stu-id="9716d-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="9716d-172">请求</span><span class="sxs-lookup"><span data-stu-id="9716d-172">Request</span></span>
<span data-ttu-id="9716d-173">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9716d-173">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/pfxRecryptionRequests/{pfxRecryptionRequestsId}
Content-type: application/json
Content-length: 574

{
  "@odata.type": "#microsoft.graph.pfxRecryptionRequest",
  "tenantId": "f9882bcd-2bcd-f988-cd2b-88f9cd2b88f9",
  "userId": "a991071c-071c-a991-1c07-91a91c0791a9",
  "deviceId": "6de0af45-af45-6de0-45af-e06d45afe06d",
  "profileId": "6389d896-d896-6389-96d8-896396d88963",
  "thumbprint": "Thumbprint value",
  "deviceKeyThumbprint": "Device Key Thumbprint value",
  "status": 6,
  "sourceType": 10,
  "createdTime": "2017-01-01T00:03:18.9597073-08:00",
  "lastModifiedTime": "2017-01-01T00:03:18.5958204-08:00",
  "isDeleted": true,
  "eTag": "ETag value"
}
```

### <a name="response"></a><span data-ttu-id="9716d-174">响应</span><span class="sxs-lookup"><span data-stu-id="9716d-174">Response</span></span>
<span data-ttu-id="9716d-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9716d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 574

{
  "@odata.type": "#microsoft.graph.pfxRecryptionRequest",
  "tenantId": "f9882bcd-2bcd-f988-cd2b-88f9cd2b88f9",
  "userId": "a991071c-071c-a991-1c07-91a91c0791a9",
  "deviceId": "6de0af45-af45-6de0-45af-e06d45afe06d",
  "profileId": "6389d896-d896-6389-96d8-896396d88963",
  "thumbprint": "Thumbprint value",
  "deviceKeyThumbprint": "Device Key Thumbprint value",
  "status": 6,
  "sourceType": 10,
  "createdTime": "2017-01-01T00:03:18.9597073-08:00",
  "lastModifiedTime": "2017-01-01T00:03:18.5958204-08:00",
  "isDeleted": true,
  "eTag": "ETag value"
}
```




