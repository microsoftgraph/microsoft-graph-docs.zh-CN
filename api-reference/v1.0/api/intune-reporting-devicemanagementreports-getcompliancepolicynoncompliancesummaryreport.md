---
title: getCompliancePolicyNonComplianceSummaryReport 操作
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2aa7b2b4493947c29a2161218f1b3fd7f10ca8d8
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52748916"
---
# <a name="getcompliancepolicynoncompliancesummaryreport-action"></a><span data-ttu-id="f3250-103">getCompliancePolicyNonComplianceSummaryReport 操作</span><span class="sxs-lookup"><span data-stu-id="f3250-103">getCompliancePolicyNonComplianceSummaryReport action</span></span>

<span data-ttu-id="f3250-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f3250-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f3250-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f3250-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3250-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f3250-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f3250-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="f3250-107">Prerequisites</span></span>
<span data-ttu-id="f3250-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f3250-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3250-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f3250-110">Permission type</span></span>|<span data-ttu-id="f3250-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f3250-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f3250-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f3250-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f3250-113">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All、DeviceManagementApps.Read.All、DeviceManagementApps.ReadWrite.All、DeviceManagementManagedDevices.Read.All、DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3250-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f3250-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f3250-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f3250-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f3250-115">Not supported.</span></span>|
|<span data-ttu-id="f3250-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f3250-116">Application</span></span>|<span data-ttu-id="f3250-117">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All、DeviceManagementApps.Read.All、DeviceManagementApps.ReadWrite.All、DeviceManagementManagedDevices.Read.All、DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3250-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f3250-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f3250-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/getCompliancePolicyNonComplianceSummaryReport
```

## <a name="request-headers"></a><span data-ttu-id="f3250-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f3250-119">Request headers</span></span>
|<span data-ttu-id="f3250-120">标头</span><span class="sxs-lookup"><span data-stu-id="f3250-120">Header</span></span>|<span data-ttu-id="f3250-121">值</span><span class="sxs-lookup"><span data-stu-id="f3250-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f3250-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f3250-122">Authorization</span></span>|<span data-ttu-id="f3250-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f3250-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f3250-124">接受</span><span class="sxs-lookup"><span data-stu-id="f3250-124">Accept</span></span>|<span data-ttu-id="f3250-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f3250-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3250-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f3250-126">Request body</span></span>
<span data-ttu-id="f3250-127">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f3250-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="f3250-128">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="f3250-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="f3250-129">属性</span><span class="sxs-lookup"><span data-stu-id="f3250-129">Property</span></span>|<span data-ttu-id="f3250-130">类型</span><span class="sxs-lookup"><span data-stu-id="f3250-130">Type</span></span>|<span data-ttu-id="f3250-131">说明</span><span class="sxs-lookup"><span data-stu-id="f3250-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3250-132">name</span><span class="sxs-lookup"><span data-stu-id="f3250-132">name</span></span>|<span data-ttu-id="f3250-133">String</span><span class="sxs-lookup"><span data-stu-id="f3250-133">String</span></span>|<span data-ttu-id="f3250-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f3250-134">Not yet documented</span></span>|
|<span data-ttu-id="f3250-135">select</span><span class="sxs-lookup"><span data-stu-id="f3250-135">select</span></span>|<span data-ttu-id="f3250-136">String collection</span><span class="sxs-lookup"><span data-stu-id="f3250-136">String collection</span></span>|<span data-ttu-id="f3250-137">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f3250-137">Not yet documented</span></span>|
|<span data-ttu-id="f3250-138">search</span><span class="sxs-lookup"><span data-stu-id="f3250-138">search</span></span>|<span data-ttu-id="f3250-139">String</span><span class="sxs-lookup"><span data-stu-id="f3250-139">String</span></span>|<span data-ttu-id="f3250-140">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f3250-140">Not yet documented</span></span>|
|<span data-ttu-id="f3250-141">groupBy</span><span class="sxs-lookup"><span data-stu-id="f3250-141">groupBy</span></span>|<span data-ttu-id="f3250-142">String collection</span><span class="sxs-lookup"><span data-stu-id="f3250-142">String collection</span></span>|<span data-ttu-id="f3250-143">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f3250-143">Not yet documented</span></span>|
|<span data-ttu-id="f3250-144">orderBy</span><span class="sxs-lookup"><span data-stu-id="f3250-144">orderBy</span></span>|<span data-ttu-id="f3250-145">String collection</span><span class="sxs-lookup"><span data-stu-id="f3250-145">String collection</span></span>|<span data-ttu-id="f3250-146">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f3250-146">Not yet documented</span></span>|
|<span data-ttu-id="f3250-147">skip</span><span class="sxs-lookup"><span data-stu-id="f3250-147">skip</span></span>|<span data-ttu-id="f3250-148">Int32</span><span class="sxs-lookup"><span data-stu-id="f3250-148">Int32</span></span>|<span data-ttu-id="f3250-149">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f3250-149">Not yet documented</span></span>|
|<span data-ttu-id="f3250-150">top</span><span class="sxs-lookup"><span data-stu-id="f3250-150">top</span></span>|<span data-ttu-id="f3250-151">Int32</span><span class="sxs-lookup"><span data-stu-id="f3250-151">Int32</span></span>|<span data-ttu-id="f3250-152">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f3250-152">Not yet documented</span></span>|
|<span data-ttu-id="f3250-153">sessionId</span><span class="sxs-lookup"><span data-stu-id="f3250-153">sessionId</span></span>|<span data-ttu-id="f3250-154">String</span><span class="sxs-lookup"><span data-stu-id="f3250-154">String</span></span>|<span data-ttu-id="f3250-155">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f3250-155">Not yet documented</span></span>|
|<span data-ttu-id="f3250-156">filter</span><span class="sxs-lookup"><span data-stu-id="f3250-156">filter</span></span>|<span data-ttu-id="f3250-157">String</span><span class="sxs-lookup"><span data-stu-id="f3250-157">String</span></span>|<span data-ttu-id="f3250-158">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f3250-158">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="f3250-159">响应</span><span class="sxs-lookup"><span data-stu-id="f3250-159">Response</span></span>
<span data-ttu-id="f3250-160">如果成功，此操作在响应 `200 OK` 正文中返回 响应代码和 Stream。</span><span class="sxs-lookup"><span data-stu-id="f3250-160">If successful, this action returns a `200 OK` response code and a Stream in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3250-161">示例</span><span class="sxs-lookup"><span data-stu-id="f3250-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="f3250-162">请求</span><span class="sxs-lookup"><span data-stu-id="f3250-162">Request</span></span>
<span data-ttu-id="f3250-163">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f3250-163">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/reports/getCompliancePolicyNonComplianceSummaryReport

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

### <a name="response"></a><span data-ttu-id="f3250-164">响应</span><span class="sxs-lookup"><span data-stu-id="f3250-164">Response</span></span>
<span data-ttu-id="f3250-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f3250-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 119

{
  "value": "Z2V0Q29tcGxpYW5jZVBvbGljeU5vbkNvbXBsaWFuY2VTdW1tYXJ5UmVwb3J0IEludHVuZSBEb2MgU2FtcGxlIDg4MTYwMDMxNQ=="
}
```




