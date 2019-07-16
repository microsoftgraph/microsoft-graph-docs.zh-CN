---
title: 更新 pfxRecryptionRequest
description: 更新 pfxRecryptionRequest 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ca4addaae01a6fea69d1742338e0452ed7227380
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35741292"
---
# <a name="update-pfxrecryptionrequest"></a><span data-ttu-id="c7f02-103">更新 pfxRecryptionRequest</span><span class="sxs-lookup"><span data-stu-id="c7f02-103">Update pfxRecryptionRequest</span></span>

> <span data-ttu-id="c7f02-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c7f02-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c7f02-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c7f02-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7f02-106">更新[pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c7f02-106">Update the properties of a [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c7f02-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="c7f02-107">Prerequisites</span></span>
<span data-ttu-id="c7f02-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c7f02-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7f02-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c7f02-110">Permission type</span></span>|<span data-ttu-id="c7f02-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c7f02-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c7f02-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c7f02-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c7f02-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7f02-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c7f02-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c7f02-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c7f02-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c7f02-115">Not supported.</span></span>|
|<span data-ttu-id="c7f02-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c7f02-116">Application</span></span>|<span data-ttu-id="c7f02-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="c7f02-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c7f02-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c7f02-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /pfxRecryptionRequests/{pfxRecryptionRequestsId}
```

## <a name="request-headers"></a><span data-ttu-id="c7f02-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c7f02-119">Request headers</span></span>
|<span data-ttu-id="c7f02-120">标头</span><span class="sxs-lookup"><span data-stu-id="c7f02-120">Header</span></span>|<span data-ttu-id="c7f02-121">值</span><span class="sxs-lookup"><span data-stu-id="c7f02-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c7f02-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c7f02-122">Authorization</span></span>|<span data-ttu-id="c7f02-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c7f02-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c7f02-124">接受</span><span class="sxs-lookup"><span data-stu-id="c7f02-124">Accept</span></span>|<span data-ttu-id="c7f02-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c7f02-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7f02-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c7f02-126">Request body</span></span>
<span data-ttu-id="c7f02-127">在请求正文中, 提供[pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c7f02-127">In the request body, supply a JSON representation for the [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) object.</span></span>

<span data-ttu-id="c7f02-128">下表显示创建[pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c7f02-128">The following table shows the properties that are required when you create the [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md).</span></span>

|<span data-ttu-id="c7f02-129">属性</span><span class="sxs-lookup"><span data-stu-id="c7f02-129">Property</span></span>|<span data-ttu-id="c7f02-130">类型</span><span class="sxs-lookup"><span data-stu-id="c7f02-130">Type</span></span>|<span data-ttu-id="c7f02-131">说明</span><span class="sxs-lookup"><span data-stu-id="c7f02-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7f02-132">tenantId</span><span class="sxs-lookup"><span data-stu-id="c7f02-132">tenantId</span></span>|<span data-ttu-id="c7f02-133">Guid</span><span class="sxs-lookup"><span data-stu-id="c7f02-133">Guid</span></span>|<span data-ttu-id="c7f02-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c7f02-134">Not yet documented</span></span>|
|<span data-ttu-id="c7f02-135">userId</span><span class="sxs-lookup"><span data-stu-id="c7f02-135">userId</span></span>|<span data-ttu-id="c7f02-136">Guid</span><span class="sxs-lookup"><span data-stu-id="c7f02-136">Guid</span></span>|<span data-ttu-id="c7f02-137">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c7f02-137">Not yet documented</span></span>|
|<span data-ttu-id="c7f02-138">deviceId</span><span class="sxs-lookup"><span data-stu-id="c7f02-138">deviceId</span></span>|<span data-ttu-id="c7f02-139">Guid</span><span class="sxs-lookup"><span data-stu-id="c7f02-139">Guid</span></span>|<span data-ttu-id="c7f02-140">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c7f02-140">Not yet documented</span></span>|
|<span data-ttu-id="c7f02-141">profileId</span><span class="sxs-lookup"><span data-stu-id="c7f02-141">profileId</span></span>|<span data-ttu-id="c7f02-142">Guid</span><span class="sxs-lookup"><span data-stu-id="c7f02-142">Guid</span></span>|<span data-ttu-id="c7f02-143">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c7f02-143">Not yet documented</span></span>|
|<span data-ttu-id="c7f02-144">为</span><span class="sxs-lookup"><span data-stu-id="c7f02-144">thumbprint</span></span>|<span data-ttu-id="c7f02-145">String</span><span class="sxs-lookup"><span data-stu-id="c7f02-145">String</span></span>|<span data-ttu-id="c7f02-146">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c7f02-146">Not yet documented</span></span>|
|<span data-ttu-id="c7f02-147">deviceKeyThumbprint</span><span class="sxs-lookup"><span data-stu-id="c7f02-147">deviceKeyThumbprint</span></span>|<span data-ttu-id="c7f02-148">String</span><span class="sxs-lookup"><span data-stu-id="c7f02-148">String</span></span>|<span data-ttu-id="c7f02-149">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c7f02-149">Not yet documented</span></span>|
|<span data-ttu-id="c7f02-150">status</span><span class="sxs-lookup"><span data-stu-id="c7f02-150">status</span></span>|<span data-ttu-id="c7f02-151">Int32</span><span class="sxs-lookup"><span data-stu-id="c7f02-151">Int32</span></span>|<span data-ttu-id="c7f02-152">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c7f02-152">Not yet documented</span></span>|
|<span data-ttu-id="c7f02-153">sourceType</span><span class="sxs-lookup"><span data-stu-id="c7f02-153">sourceType</span></span>|<span data-ttu-id="c7f02-154">Int32</span><span class="sxs-lookup"><span data-stu-id="c7f02-154">Int32</span></span>|<span data-ttu-id="c7f02-155">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c7f02-155">Not yet documented</span></span>|
|<span data-ttu-id="c7f02-156">createdTime</span><span class="sxs-lookup"><span data-stu-id="c7f02-156">createdTime</span></span>|<span data-ttu-id="c7f02-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7f02-157">DateTimeOffset</span></span>|<span data-ttu-id="c7f02-158">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c7f02-158">Not yet documented</span></span>|
|<span data-ttu-id="c7f02-159">lastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="c7f02-159">lastModifiedTime</span></span>|<span data-ttu-id="c7f02-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7f02-160">DateTimeOffset</span></span>|<span data-ttu-id="c7f02-161">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c7f02-161">Not yet documented</span></span>|
|<span data-ttu-id="c7f02-162">isDeleted</span><span class="sxs-lookup"><span data-stu-id="c7f02-162">isDeleted</span></span>|<span data-ttu-id="c7f02-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="c7f02-163">Boolean</span></span>|<span data-ttu-id="c7f02-164">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c7f02-164">Not yet documented</span></span>|
|<span data-ttu-id="c7f02-165">eTag</span><span class="sxs-lookup"><span data-stu-id="c7f02-165">eTag</span></span>|<span data-ttu-id="c7f02-166">String</span><span class="sxs-lookup"><span data-stu-id="c7f02-166">String</span></span>|<span data-ttu-id="c7f02-167">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c7f02-167">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="c7f02-168">响应</span><span class="sxs-lookup"><span data-stu-id="c7f02-168">Response</span></span>
<span data-ttu-id="c7f02-169">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c7f02-169">If successful, this method returns a `200 OK` response code and an updated [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7f02-170">示例</span><span class="sxs-lookup"><span data-stu-id="c7f02-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="c7f02-171">请求</span><span class="sxs-lookup"><span data-stu-id="c7f02-171">Request</span></span>
<span data-ttu-id="c7f02-172">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c7f02-172">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c7f02-173">响应</span><span class="sxs-lookup"><span data-stu-id="c7f02-173">Response</span></span>
<span data-ttu-id="c7f02-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c7f02-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





