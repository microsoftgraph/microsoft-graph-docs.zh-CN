---
title: getPolicyNonComplianceMetadata 操作
description: 尚未记录
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1eb766fd73e1df52b2348f8183e5e5e038fd35a3
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42801374"
---
# <a name="getpolicynoncompliancemetadata-action"></a><span data-ttu-id="95a3f-103">getPolicyNonComplianceMetadata 操作</span><span class="sxs-lookup"><span data-stu-id="95a3f-103">getPolicyNonComplianceMetadata action</span></span>

> <span data-ttu-id="95a3f-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="95a3f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="95a3f-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="95a3f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95a3f-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="95a3f-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="95a3f-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="95a3f-107">Prerequisites</span></span>
<span data-ttu-id="95a3f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="95a3f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95a3f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="95a3f-110">Permission type</span></span>|<span data-ttu-id="95a3f-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="95a3f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="95a3f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="95a3f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="95a3f-113">Devicemanagementconfiguration.readwrite.all、Devicemanagementconfiguration.readwrite.all、Devicemanagementapps.readwrite.all、all、Devicemanagementapps.readwrite.all、all、Devicemanagementmanageddevices.readwrite.all、all、、all、Devicemanagementmanageddevices.readwrite.all</span><span class="sxs-lookup"><span data-stu-id="95a3f-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="95a3f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="95a3f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="95a3f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="95a3f-115">Not supported.</span></span>|
|<span data-ttu-id="95a3f-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="95a3f-116">Application</span></span>|<span data-ttu-id="95a3f-117">Devicemanagementconfiguration.readwrite.all、Devicemanagementconfiguration.readwrite.all、Devicemanagementapps.readwrite.all、all、Devicemanagementapps.readwrite.all、all、Devicemanagementmanageddevices.readwrite.all、all、、all、Devicemanagementmanageddevices.readwrite.all</span><span class="sxs-lookup"><span data-stu-id="95a3f-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="95a3f-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="95a3f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/getPolicyNonComplianceMetadata
```

## <a name="request-headers"></a><span data-ttu-id="95a3f-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="95a3f-119">Request headers</span></span>
|<span data-ttu-id="95a3f-120">标头</span><span class="sxs-lookup"><span data-stu-id="95a3f-120">Header</span></span>|<span data-ttu-id="95a3f-121">值</span><span class="sxs-lookup"><span data-stu-id="95a3f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="95a3f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="95a3f-122">Authorization</span></span>|<span data-ttu-id="95a3f-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="95a3f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="95a3f-124">接受</span><span class="sxs-lookup"><span data-stu-id="95a3f-124">Accept</span></span>|<span data-ttu-id="95a3f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="95a3f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="95a3f-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="95a3f-126">Request body</span></span>
<span data-ttu-id="95a3f-127">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="95a3f-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="95a3f-128">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="95a3f-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="95a3f-129">属性</span><span class="sxs-lookup"><span data-stu-id="95a3f-129">Property</span></span>|<span data-ttu-id="95a3f-130">类型</span><span class="sxs-lookup"><span data-stu-id="95a3f-130">Type</span></span>|<span data-ttu-id="95a3f-131">说明</span><span class="sxs-lookup"><span data-stu-id="95a3f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95a3f-132">name</span><span class="sxs-lookup"><span data-stu-id="95a3f-132">name</span></span>|<span data-ttu-id="95a3f-133">String</span><span class="sxs-lookup"><span data-stu-id="95a3f-133">String</span></span>|<span data-ttu-id="95a3f-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="95a3f-134">Not yet documented</span></span>|
|<span data-ttu-id="95a3f-135">select</span><span class="sxs-lookup"><span data-stu-id="95a3f-135">select</span></span>|<span data-ttu-id="95a3f-136">String collection</span><span class="sxs-lookup"><span data-stu-id="95a3f-136">String collection</span></span>|<span data-ttu-id="95a3f-137">尚未记录</span><span class="sxs-lookup"><span data-stu-id="95a3f-137">Not yet documented</span></span>|
|<span data-ttu-id="95a3f-138">search</span><span class="sxs-lookup"><span data-stu-id="95a3f-138">search</span></span>|<span data-ttu-id="95a3f-139">String</span><span class="sxs-lookup"><span data-stu-id="95a3f-139">String</span></span>|<span data-ttu-id="95a3f-140">尚未记录</span><span class="sxs-lookup"><span data-stu-id="95a3f-140">Not yet documented</span></span>|
|<span data-ttu-id="95a3f-141">groupBy</span><span class="sxs-lookup"><span data-stu-id="95a3f-141">groupBy</span></span>|<span data-ttu-id="95a3f-142">String collection</span><span class="sxs-lookup"><span data-stu-id="95a3f-142">String collection</span></span>|<span data-ttu-id="95a3f-143">尚未记录</span><span class="sxs-lookup"><span data-stu-id="95a3f-143">Not yet documented</span></span>|
|<span data-ttu-id="95a3f-144">By</span><span class="sxs-lookup"><span data-stu-id="95a3f-144">orderBy</span></span>|<span data-ttu-id="95a3f-145">String collection</span><span class="sxs-lookup"><span data-stu-id="95a3f-145">String collection</span></span>|<span data-ttu-id="95a3f-146">尚未记录</span><span class="sxs-lookup"><span data-stu-id="95a3f-146">Not yet documented</span></span>|
|<span data-ttu-id="95a3f-147">skip</span><span class="sxs-lookup"><span data-stu-id="95a3f-147">skip</span></span>|<span data-ttu-id="95a3f-148">Int32</span><span class="sxs-lookup"><span data-stu-id="95a3f-148">Int32</span></span>|<span data-ttu-id="95a3f-149">尚未记录</span><span class="sxs-lookup"><span data-stu-id="95a3f-149">Not yet documented</span></span>|
|<span data-ttu-id="95a3f-150">top</span><span class="sxs-lookup"><span data-stu-id="95a3f-150">top</span></span>|<span data-ttu-id="95a3f-151">Int32</span><span class="sxs-lookup"><span data-stu-id="95a3f-151">Int32</span></span>|<span data-ttu-id="95a3f-152">尚未记录</span><span class="sxs-lookup"><span data-stu-id="95a3f-152">Not yet documented</span></span>|
|<span data-ttu-id="95a3f-153">sessionId</span><span class="sxs-lookup"><span data-stu-id="95a3f-153">sessionId</span></span>|<span data-ttu-id="95a3f-154">String</span><span class="sxs-lookup"><span data-stu-id="95a3f-154">String</span></span>|<span data-ttu-id="95a3f-155">尚未记录</span><span class="sxs-lookup"><span data-stu-id="95a3f-155">Not yet documented</span></span>|
|<span data-ttu-id="95a3f-156">filter</span><span class="sxs-lookup"><span data-stu-id="95a3f-156">filter</span></span>|<span data-ttu-id="95a3f-157">String</span><span class="sxs-lookup"><span data-stu-id="95a3f-157">String</span></span>|<span data-ttu-id="95a3f-158">尚未记录</span><span class="sxs-lookup"><span data-stu-id="95a3f-158">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="95a3f-159">响应</span><span class="sxs-lookup"><span data-stu-id="95a3f-159">Response</span></span>
<span data-ttu-id="95a3f-160">如果成功，此操作会在`200 OK`响应正文中返回响应代码和 Stream。</span><span class="sxs-lookup"><span data-stu-id="95a3f-160">If successful, this action returns a `200 OK` response code and a Stream in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95a3f-161">示例</span><span class="sxs-lookup"><span data-stu-id="95a3f-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="95a3f-162">请求</span><span class="sxs-lookup"><span data-stu-id="95a3f-162">Request</span></span>
<span data-ttu-id="95a3f-163">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="95a3f-163">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/reports/getPolicyNonComplianceMetadata

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

### <a name="response"></a><span data-ttu-id="95a3f-164">响应</span><span class="sxs-lookup"><span data-stu-id="95a3f-164">Response</span></span>
<span data-ttu-id="95a3f-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="95a3f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 54

{
  "value": "<Unknown Primitive Type Edm.Stream>"
}
```




