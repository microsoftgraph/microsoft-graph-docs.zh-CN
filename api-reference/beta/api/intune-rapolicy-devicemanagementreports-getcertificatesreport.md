---
title: getCertificatesReport 操作
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1930880aa60548858345c55346c793648b6f7934
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51152192"
---
# <a name="getcertificatesreport-action"></a><span data-ttu-id="c4cb3-103">getCertificatesReport 操作</span><span class="sxs-lookup"><span data-stu-id="c4cb3-103">getCertificatesReport action</span></span>

<span data-ttu-id="c4cb3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c4cb3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c4cb3-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c4cb3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c4cb3-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c4cb3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c4cb3-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c4cb3-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c4cb3-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="c4cb3-108">Prerequisites</span></span>
<span data-ttu-id="c4cb3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c4cb3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4cb3-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c4cb3-111">Permission type</span></span>|<span data-ttu-id="c4cb3-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c4cb3-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c4cb3-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c4cb3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c4cb3-114">DeviceManagementServiceConfig.Read.All、DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4cb3-114">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c4cb3-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c4cb3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c4cb3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c4cb3-116">Not supported.</span></span>|
|<span data-ttu-id="c4cb3-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c4cb3-117">Application</span></span>|<span data-ttu-id="c4cb3-118">DeviceManagementServiceConfig.Read.All、DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4cb3-118">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c4cb3-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c4cb3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/getCertificatesReport
```

## <a name="request-headers"></a><span data-ttu-id="c4cb3-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c4cb3-120">Request headers</span></span>
|<span data-ttu-id="c4cb3-121">标头</span><span class="sxs-lookup"><span data-stu-id="c4cb3-121">Header</span></span>|<span data-ttu-id="c4cb3-122">值</span><span class="sxs-lookup"><span data-stu-id="c4cb3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c4cb3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c4cb3-123">Authorization</span></span>|<span data-ttu-id="c4cb3-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c4cb3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c4cb3-125">接受</span><span class="sxs-lookup"><span data-stu-id="c4cb3-125">Accept</span></span>|<span data-ttu-id="c4cb3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c4cb3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4cb3-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c4cb3-127">Request body</span></span>
<span data-ttu-id="c4cb3-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c4cb3-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="c4cb3-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="c4cb3-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="c4cb3-130">属性</span><span class="sxs-lookup"><span data-stu-id="c4cb3-130">Property</span></span>|<span data-ttu-id="c4cb3-131">类型</span><span class="sxs-lookup"><span data-stu-id="c4cb3-131">Type</span></span>|<span data-ttu-id="c4cb3-132">说明</span><span class="sxs-lookup"><span data-stu-id="c4cb3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c4cb3-133">name</span><span class="sxs-lookup"><span data-stu-id="c4cb3-133">name</span></span>|<span data-ttu-id="c4cb3-134">String</span><span class="sxs-lookup"><span data-stu-id="c4cb3-134">String</span></span>|<span data-ttu-id="c4cb3-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c4cb3-135">Not yet documented</span></span>|
|<span data-ttu-id="c4cb3-136">select</span><span class="sxs-lookup"><span data-stu-id="c4cb3-136">select</span></span>|<span data-ttu-id="c4cb3-137">String collection</span><span class="sxs-lookup"><span data-stu-id="c4cb3-137">String collection</span></span>|<span data-ttu-id="c4cb3-138">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c4cb3-138">Not yet documented</span></span>|
|<span data-ttu-id="c4cb3-139">search</span><span class="sxs-lookup"><span data-stu-id="c4cb3-139">search</span></span>|<span data-ttu-id="c4cb3-140">String</span><span class="sxs-lookup"><span data-stu-id="c4cb3-140">String</span></span>|<span data-ttu-id="c4cb3-141">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c4cb3-141">Not yet documented</span></span>|
|<span data-ttu-id="c4cb3-142">groupBy</span><span class="sxs-lookup"><span data-stu-id="c4cb3-142">groupBy</span></span>|<span data-ttu-id="c4cb3-143">String collection</span><span class="sxs-lookup"><span data-stu-id="c4cb3-143">String collection</span></span>|<span data-ttu-id="c4cb3-144">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c4cb3-144">Not yet documented</span></span>|
|<span data-ttu-id="c4cb3-145">orderBy</span><span class="sxs-lookup"><span data-stu-id="c4cb3-145">orderBy</span></span>|<span data-ttu-id="c4cb3-146">String collection</span><span class="sxs-lookup"><span data-stu-id="c4cb3-146">String collection</span></span>|<span data-ttu-id="c4cb3-147">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c4cb3-147">Not yet documented</span></span>|
|<span data-ttu-id="c4cb3-148">skip</span><span class="sxs-lookup"><span data-stu-id="c4cb3-148">skip</span></span>|<span data-ttu-id="c4cb3-149">Int32</span><span class="sxs-lookup"><span data-stu-id="c4cb3-149">Int32</span></span>|<span data-ttu-id="c4cb3-150">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c4cb3-150">Not yet documented</span></span>|
|<span data-ttu-id="c4cb3-151">top</span><span class="sxs-lookup"><span data-stu-id="c4cb3-151">top</span></span>|<span data-ttu-id="c4cb3-152">Int32</span><span class="sxs-lookup"><span data-stu-id="c4cb3-152">Int32</span></span>|<span data-ttu-id="c4cb3-153">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c4cb3-153">Not yet documented</span></span>|
|<span data-ttu-id="c4cb3-154">sessionId</span><span class="sxs-lookup"><span data-stu-id="c4cb3-154">sessionId</span></span>|<span data-ttu-id="c4cb3-155">String</span><span class="sxs-lookup"><span data-stu-id="c4cb3-155">String</span></span>|<span data-ttu-id="c4cb3-156">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c4cb3-156">Not yet documented</span></span>|
|<span data-ttu-id="c4cb3-157">filter</span><span class="sxs-lookup"><span data-stu-id="c4cb3-157">filter</span></span>|<span data-ttu-id="c4cb3-158">String</span><span class="sxs-lookup"><span data-stu-id="c4cb3-158">String</span></span>|<span data-ttu-id="c4cb3-159">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c4cb3-159">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="c4cb3-160">响应</span><span class="sxs-lookup"><span data-stu-id="c4cb3-160">Response</span></span>
<span data-ttu-id="c4cb3-161">如果成功，此操作在响应 `200 OK` 正文中返回 响应代码和 Stream。</span><span class="sxs-lookup"><span data-stu-id="c4cb3-161">If successful, this action returns a `200 OK` response code and a Stream in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4cb3-162">示例</span><span class="sxs-lookup"><span data-stu-id="c4cb3-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="c4cb3-163">请求</span><span class="sxs-lookup"><span data-stu-id="c4cb3-163">Request</span></span>
<span data-ttu-id="c4cb3-164">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c4cb3-164">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/reports/getCertificatesReport

Content-type: application/json
Content-length: 278

{
  "name": "Name value",
  "select": [
    "Select value"
  ],
  "search": "Search value",
  "groupBy": [
    "Group By value"
  ],
  "orderBy": [
    "Order By value"
  ],
  "skip": 4,
  "top": 3,
  "sessionId": "Session Id value",
  "filter": "Filter value"
}
```

### <a name="response"></a><span data-ttu-id="c4cb3-165">响应</span><span class="sxs-lookup"><span data-stu-id="c4cb3-165">Response</span></span>
<span data-ttu-id="c4cb3-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c4cb3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 87

{
  "value": "Z2V0Q2VydGlmaWNhdGVzUmVwb3J0IEludHVuZSBEb2MgU2FtcGxlIDExMzUyMTc4MTI="
}
```




