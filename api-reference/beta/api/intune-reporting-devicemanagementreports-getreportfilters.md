---
title: getReportFilters 操作
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 57b0f0095ae5b85fce3fad3c72957df51175d313
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791333"
---
# <a name="getreportfilters-action"></a><span data-ttu-id="c82e0-103">getReportFilters 操作</span><span class="sxs-lookup"><span data-stu-id="c82e0-103">getReportFilters action</span></span>

<span data-ttu-id="c82e0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c82e0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c82e0-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c82e0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c82e0-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c82e0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c82e0-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c82e0-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c82e0-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="c82e0-108">Prerequisites</span></span>
<span data-ttu-id="c82e0-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="c82e0-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="c82e0-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c82e0-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c82e0-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c82e0-111">Permission type</span></span>|<span data-ttu-id="c82e0-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c82e0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c82e0-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c82e0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c82e0-114">Devicemanagementconfiguration.readwrite.all、Devicemanagementconfiguration.readwrite.all、Devicemanagementapps.readwrite.all、all、Devicemanagementapps.readwrite.all、all、devicemanagementmanageddevices.readwrite.all、all、devicemanagementmanageddevices.readwrite.all、all 和 Read. all。 All</span><span class="sxs-lookup"><span data-stu-id="c82e0-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="c82e0-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c82e0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c82e0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c82e0-116">Not supported.</span></span>|
|<span data-ttu-id="c82e0-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c82e0-117">Application</span></span>|<span data-ttu-id="c82e0-118">Devicemanagementconfiguration.readwrite.all、Devicemanagementconfiguration.readwrite.all、Devicemanagementapps.readwrite.all、all、Devicemanagementapps.readwrite.all、all、devicemanagementmanageddevices.readwrite.all、all、devicemanagementmanageddevices.readwrite.all、all 和 Read. all。 All</span><span class="sxs-lookup"><span data-stu-id="c82e0-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c82e0-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c82e0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/getReportFilters
```

## <a name="request-headers"></a><span data-ttu-id="c82e0-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c82e0-120">Request headers</span></span>
|<span data-ttu-id="c82e0-121">标头</span><span class="sxs-lookup"><span data-stu-id="c82e0-121">Header</span></span>|<span data-ttu-id="c82e0-122">值</span><span class="sxs-lookup"><span data-stu-id="c82e0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c82e0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c82e0-123">Authorization</span></span>|<span data-ttu-id="c82e0-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c82e0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c82e0-125">接受</span><span class="sxs-lookup"><span data-stu-id="c82e0-125">Accept</span></span>|<span data-ttu-id="c82e0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c82e0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c82e0-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c82e0-127">Request body</span></span>
<span data-ttu-id="c82e0-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c82e0-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="c82e0-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="c82e0-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="c82e0-130">属性</span><span class="sxs-lookup"><span data-stu-id="c82e0-130">Property</span></span>|<span data-ttu-id="c82e0-131">类型</span><span class="sxs-lookup"><span data-stu-id="c82e0-131">Type</span></span>|<span data-ttu-id="c82e0-132">说明</span><span class="sxs-lookup"><span data-stu-id="c82e0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c82e0-133">name</span><span class="sxs-lookup"><span data-stu-id="c82e0-133">name</span></span>|<span data-ttu-id="c82e0-134">String</span><span class="sxs-lookup"><span data-stu-id="c82e0-134">String</span></span>|<span data-ttu-id="c82e0-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c82e0-135">Not yet documented</span></span>|
|<span data-ttu-id="c82e0-136">select</span><span class="sxs-lookup"><span data-stu-id="c82e0-136">select</span></span>|<span data-ttu-id="c82e0-137">String collection</span><span class="sxs-lookup"><span data-stu-id="c82e0-137">String collection</span></span>|<span data-ttu-id="c82e0-138">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c82e0-138">Not yet documented</span></span>|
|<span data-ttu-id="c82e0-139">search</span><span class="sxs-lookup"><span data-stu-id="c82e0-139">search</span></span>|<span data-ttu-id="c82e0-140">String</span><span class="sxs-lookup"><span data-stu-id="c82e0-140">String</span></span>|<span data-ttu-id="c82e0-141">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c82e0-141">Not yet documented</span></span>|
|<span data-ttu-id="c82e0-142">groupBy</span><span class="sxs-lookup"><span data-stu-id="c82e0-142">groupBy</span></span>|<span data-ttu-id="c82e0-143">String collection</span><span class="sxs-lookup"><span data-stu-id="c82e0-143">String collection</span></span>|<span data-ttu-id="c82e0-144">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c82e0-144">Not yet documented</span></span>|
|<span data-ttu-id="c82e0-145">By</span><span class="sxs-lookup"><span data-stu-id="c82e0-145">orderBy</span></span>|<span data-ttu-id="c82e0-146">String collection</span><span class="sxs-lookup"><span data-stu-id="c82e0-146">String collection</span></span>|<span data-ttu-id="c82e0-147">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c82e0-147">Not yet documented</span></span>|
|<span data-ttu-id="c82e0-148">skip</span><span class="sxs-lookup"><span data-stu-id="c82e0-148">skip</span></span>|<span data-ttu-id="c82e0-149">Int32</span><span class="sxs-lookup"><span data-stu-id="c82e0-149">Int32</span></span>|<span data-ttu-id="c82e0-150">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c82e0-150">Not yet documented</span></span>|
|<span data-ttu-id="c82e0-151">top</span><span class="sxs-lookup"><span data-stu-id="c82e0-151">top</span></span>|<span data-ttu-id="c82e0-152">Int32</span><span class="sxs-lookup"><span data-stu-id="c82e0-152">Int32</span></span>|<span data-ttu-id="c82e0-153">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c82e0-153">Not yet documented</span></span>|
|<span data-ttu-id="c82e0-154">sessionId</span><span class="sxs-lookup"><span data-stu-id="c82e0-154">sessionId</span></span>|<span data-ttu-id="c82e0-155">String</span><span class="sxs-lookup"><span data-stu-id="c82e0-155">String</span></span>|<span data-ttu-id="c82e0-156">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c82e0-156">Not yet documented</span></span>|
|<span data-ttu-id="c82e0-157">filter</span><span class="sxs-lookup"><span data-stu-id="c82e0-157">filter</span></span>|<span data-ttu-id="c82e0-158">String</span><span class="sxs-lookup"><span data-stu-id="c82e0-158">String</span></span>|<span data-ttu-id="c82e0-159">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c82e0-159">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="c82e0-160">响应</span><span class="sxs-lookup"><span data-stu-id="c82e0-160">Response</span></span>
<span data-ttu-id="c82e0-161">如果成功，此操作会 `200 OK` 在响应正文中返回响应代码和 Stream。</span><span class="sxs-lookup"><span data-stu-id="c82e0-161">If successful, this action returns a `200 OK` response code and a Stream in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c82e0-162">示例</span><span class="sxs-lookup"><span data-stu-id="c82e0-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="c82e0-163">请求</span><span class="sxs-lookup"><span data-stu-id="c82e0-163">Request</span></span>
<span data-ttu-id="c82e0-164">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c82e0-164">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/reports/getReportFilters

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

### <a name="response"></a><span data-ttu-id="c82e0-165">响应</span><span class="sxs-lookup"><span data-stu-id="c82e0-165">Response</span></span>
<span data-ttu-id="c82e0-166">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="c82e0-166">Here is an example of the response.</span></span> <span data-ttu-id="c82e0-167">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="c82e0-167">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="c82e0-168">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="c82e0-168">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 79

{
  "value": "Z2V0UmVwb3J0RmlsdGVycyBJbnR1bmUgRG9jIFNhbXBsZSAxMzYxOTI0Mjkx"
}
```



