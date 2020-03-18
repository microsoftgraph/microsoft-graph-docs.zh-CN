---
title: 创建 pfxRecryptionRequest
description: 创建新的 pfxRecryptionRequest 对象。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d03cdd29fec84457ad736623b1feb2d389acf3c9
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42801913"
---
# <a name="create-pfxrecryptionrequest"></a><span data-ttu-id="d65fd-103">创建 pfxRecryptionRequest</span><span class="sxs-lookup"><span data-stu-id="d65fd-103">Create pfxRecryptionRequest</span></span>

> <span data-ttu-id="d65fd-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d65fd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d65fd-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d65fd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d65fd-106">创建新的[pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d65fd-106">Create a new [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d65fd-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="d65fd-107">Prerequisites</span></span>
<span data-ttu-id="d65fd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d65fd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d65fd-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d65fd-110">Permission type</span></span>|<span data-ttu-id="d65fd-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d65fd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d65fd-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d65fd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d65fd-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d65fd-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d65fd-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d65fd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d65fd-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d65fd-115">Not supported.</span></span>|
|<span data-ttu-id="d65fd-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d65fd-116">Application</span></span>|<span data-ttu-id="d65fd-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d65fd-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d65fd-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d65fd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /pfxRecryptionRequests
```

## <a name="request-headers"></a><span data-ttu-id="d65fd-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="d65fd-119">Request headers</span></span>
|<span data-ttu-id="d65fd-120">标头</span><span class="sxs-lookup"><span data-stu-id="d65fd-120">Header</span></span>|<span data-ttu-id="d65fd-121">值</span><span class="sxs-lookup"><span data-stu-id="d65fd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d65fd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d65fd-122">Authorization</span></span>|<span data-ttu-id="d65fd-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d65fd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d65fd-124">接受</span><span class="sxs-lookup"><span data-stu-id="d65fd-124">Accept</span></span>|<span data-ttu-id="d65fd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d65fd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d65fd-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d65fd-126">Request body</span></span>
<span data-ttu-id="d65fd-127">在请求正文中，提供 pfxRecryptionRequest 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d65fd-127">In the request body, supply a JSON representation for the pfxRecryptionRequest object.</span></span>

<span data-ttu-id="d65fd-128">下表显示创建 pfxRecryptionRequest 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d65fd-128">The following table shows the properties that are required when you create the pfxRecryptionRequest.</span></span>

|<span data-ttu-id="d65fd-129">属性</span><span class="sxs-lookup"><span data-stu-id="d65fd-129">Property</span></span>|<span data-ttu-id="d65fd-130">类型</span><span class="sxs-lookup"><span data-stu-id="d65fd-130">Type</span></span>|<span data-ttu-id="d65fd-131">说明</span><span class="sxs-lookup"><span data-stu-id="d65fd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d65fd-132">tenantId</span><span class="sxs-lookup"><span data-stu-id="d65fd-132">tenantId</span></span>|<span data-ttu-id="d65fd-133">Guid</span><span class="sxs-lookup"><span data-stu-id="d65fd-133">Guid</span></span>|<span data-ttu-id="d65fd-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d65fd-134">Not yet documented</span></span>|
|<span data-ttu-id="d65fd-135">userId</span><span class="sxs-lookup"><span data-stu-id="d65fd-135">userId</span></span>|<span data-ttu-id="d65fd-136">Guid</span><span class="sxs-lookup"><span data-stu-id="d65fd-136">Guid</span></span>|<span data-ttu-id="d65fd-137">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d65fd-137">Not yet documented</span></span>|
|<span data-ttu-id="d65fd-138">deviceId</span><span class="sxs-lookup"><span data-stu-id="d65fd-138">deviceId</span></span>|<span data-ttu-id="d65fd-139">Guid</span><span class="sxs-lookup"><span data-stu-id="d65fd-139">Guid</span></span>|<span data-ttu-id="d65fd-140">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d65fd-140">Not yet documented</span></span>|
|<span data-ttu-id="d65fd-141">profileId</span><span class="sxs-lookup"><span data-stu-id="d65fd-141">profileId</span></span>|<span data-ttu-id="d65fd-142">Guid</span><span class="sxs-lookup"><span data-stu-id="d65fd-142">Guid</span></span>|<span data-ttu-id="d65fd-143">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d65fd-143">Not yet documented</span></span>|
|<span data-ttu-id="d65fd-144">为</span><span class="sxs-lookup"><span data-stu-id="d65fd-144">thumbprint</span></span>|<span data-ttu-id="d65fd-145">String</span><span class="sxs-lookup"><span data-stu-id="d65fd-145">String</span></span>|<span data-ttu-id="d65fd-146">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d65fd-146">Not yet documented</span></span>|
|<span data-ttu-id="d65fd-147">deviceKeyThumbprint</span><span class="sxs-lookup"><span data-stu-id="d65fd-147">deviceKeyThumbprint</span></span>|<span data-ttu-id="d65fd-148">String</span><span class="sxs-lookup"><span data-stu-id="d65fd-148">String</span></span>|<span data-ttu-id="d65fd-149">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d65fd-149">Not yet documented</span></span>|
|<span data-ttu-id="d65fd-150">状态</span><span class="sxs-lookup"><span data-stu-id="d65fd-150">status</span></span>|<span data-ttu-id="d65fd-151">Int32</span><span class="sxs-lookup"><span data-stu-id="d65fd-151">Int32</span></span>|<span data-ttu-id="d65fd-152">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d65fd-152">Not yet documented</span></span>|
|<span data-ttu-id="d65fd-153">sourceType</span><span class="sxs-lookup"><span data-stu-id="d65fd-153">sourceType</span></span>|<span data-ttu-id="d65fd-154">Int32</span><span class="sxs-lookup"><span data-stu-id="d65fd-154">Int32</span></span>|<span data-ttu-id="d65fd-155">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d65fd-155">Not yet documented</span></span>|
|<span data-ttu-id="d65fd-156">createdTime</span><span class="sxs-lookup"><span data-stu-id="d65fd-156">createdTime</span></span>|<span data-ttu-id="d65fd-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d65fd-157">DateTimeOffset</span></span>|<span data-ttu-id="d65fd-158">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d65fd-158">Not yet documented</span></span>|
|<span data-ttu-id="d65fd-159">lastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="d65fd-159">lastModifiedTime</span></span>|<span data-ttu-id="d65fd-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d65fd-160">DateTimeOffset</span></span>|<span data-ttu-id="d65fd-161">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d65fd-161">Not yet documented</span></span>|
|<span data-ttu-id="d65fd-162">isDeleted</span><span class="sxs-lookup"><span data-stu-id="d65fd-162">isDeleted</span></span>|<span data-ttu-id="d65fd-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="d65fd-163">Boolean</span></span>|<span data-ttu-id="d65fd-164">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d65fd-164">Not yet documented</span></span>|
|<span data-ttu-id="d65fd-165">eTag</span><span class="sxs-lookup"><span data-stu-id="d65fd-165">eTag</span></span>|<span data-ttu-id="d65fd-166">String</span><span class="sxs-lookup"><span data-stu-id="d65fd-166">String</span></span>|<span data-ttu-id="d65fd-167">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d65fd-167">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="d65fd-168">响应</span><span class="sxs-lookup"><span data-stu-id="d65fd-168">Response</span></span>
<span data-ttu-id="d65fd-169">如果成功，此方法在响应`201 Created`正文中返回响应代码和[pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d65fd-169">If successful, this method returns a `201 Created` response code and a [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d65fd-170">示例</span><span class="sxs-lookup"><span data-stu-id="d65fd-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="d65fd-171">请求</span><span class="sxs-lookup"><span data-stu-id="d65fd-171">Request</span></span>
<span data-ttu-id="d65fd-172">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d65fd-172">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/pfxRecryptionRequests
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

### <a name="response"></a><span data-ttu-id="d65fd-173">响应</span><span class="sxs-lookup"><span data-stu-id="d65fd-173">Response</span></span>
<span data-ttu-id="d65fd-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d65fd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




