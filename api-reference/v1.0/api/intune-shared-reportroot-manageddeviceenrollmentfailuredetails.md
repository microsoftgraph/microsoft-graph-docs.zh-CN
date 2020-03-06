---
title: managedDeviceEnrollmentFailureDetails 函数
description: 尚未记录
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1fb6214cd36cdc61b7ca0843dd18103f62ee83dd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42512025"
---
# <a name="manageddeviceenrollmentfailuredetails-function"></a><span data-ttu-id="193a1-103">managedDeviceEnrollmentFailureDetails 函数</span><span class="sxs-lookup"><span data-stu-id="193a1-103">managedDeviceEnrollmentFailureDetails function</span></span>

<span data-ttu-id="193a1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="193a1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="193a1-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="193a1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="193a1-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="193a1-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="193a1-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="193a1-107">Prerequisites</span></span>
<span data-ttu-id="193a1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="193a1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="193a1-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="193a1-110">Permission type</span></span>|<span data-ttu-id="193a1-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="193a1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="193a1-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="193a1-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="193a1-113">&nbsp;&nbsp;故障排除</span><span class="sxs-lookup"><span data-stu-id="193a1-113">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="193a1-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="193a1-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="193a1-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="193a1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="193a1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="193a1-116">Not supported.</span></span>|
|<span data-ttu-id="193a1-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="193a1-117">Application</span></span>|<span data-ttu-id="193a1-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="193a1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="193a1-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="193a1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentFailureDetails
```

## <a name="request-headers"></a><span data-ttu-id="193a1-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="193a1-120">Request headers</span></span>
|<span data-ttu-id="193a1-121">标头</span><span class="sxs-lookup"><span data-stu-id="193a1-121">Header</span></span>|<span data-ttu-id="193a1-122">值</span><span class="sxs-lookup"><span data-stu-id="193a1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="193a1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="193a1-123">Authorization</span></span>|<span data-ttu-id="193a1-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="193a1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="193a1-125">接受</span><span class="sxs-lookup"><span data-stu-id="193a1-125">Accept</span></span>|<span data-ttu-id="193a1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="193a1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="193a1-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="193a1-127">Request body</span></span>
<span data-ttu-id="193a1-128">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="193a1-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="193a1-129">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="193a1-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="193a1-130">属性</span><span class="sxs-lookup"><span data-stu-id="193a1-130">Property</span></span>|<span data-ttu-id="193a1-131">类型</span><span class="sxs-lookup"><span data-stu-id="193a1-131">Type</span></span>|<span data-ttu-id="193a1-132">说明</span><span class="sxs-lookup"><span data-stu-id="193a1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="193a1-133">skip</span><span class="sxs-lookup"><span data-stu-id="193a1-133">skip</span></span>|<span data-ttu-id="193a1-134">Int32</span><span class="sxs-lookup"><span data-stu-id="193a1-134">Int32</span></span>|<span data-ttu-id="193a1-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="193a1-135">Not yet documented</span></span>|
|<span data-ttu-id="193a1-136">top</span><span class="sxs-lookup"><span data-stu-id="193a1-136">top</span></span>|<span data-ttu-id="193a1-137">Int32</span><span class="sxs-lookup"><span data-stu-id="193a1-137">Int32</span></span>|<span data-ttu-id="193a1-138">尚未记录</span><span class="sxs-lookup"><span data-stu-id="193a1-138">Not yet documented</span></span>|
|<span data-ttu-id="193a1-139">filter</span><span class="sxs-lookup"><span data-stu-id="193a1-139">filter</span></span>|<span data-ttu-id="193a1-140">String</span><span class="sxs-lookup"><span data-stu-id="193a1-140">String</span></span>|<span data-ttu-id="193a1-141">尚未记录</span><span class="sxs-lookup"><span data-stu-id="193a1-141">Not yet documented</span></span>|
|<span data-ttu-id="193a1-142">skipToken</span><span class="sxs-lookup"><span data-stu-id="193a1-142">skipToken</span></span>|<span data-ttu-id="193a1-143">String</span><span class="sxs-lookup"><span data-stu-id="193a1-143">String</span></span>|<span data-ttu-id="193a1-144">尚未记录</span><span class="sxs-lookup"><span data-stu-id="193a1-144">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="193a1-145">响应</span><span class="sxs-lookup"><span data-stu-id="193a1-145">Response</span></span>
<span data-ttu-id="193a1-146">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 [report](../resources/intune-shared-report.md)。</span><span class="sxs-lookup"><span data-stu-id="193a1-146">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="193a1-147">示例</span><span class="sxs-lookup"><span data-stu-id="193a1-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="193a1-148">请求</span><span class="sxs-lookup"><span data-stu-id="193a1-148">Request</span></span>
<span data-ttu-id="193a1-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="193a1-149">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1/reports/managedDeviceEnrollmentFailureDetails(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="193a1-150">响应</span><span class="sxs-lookup"><span data-stu-id="193a1-150">Response</span></span>
<span data-ttu-id="193a1-151">为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="193a1-151">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="193a1-152">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="193a1-152">All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 123

{
  "value": {
    "@odata.type": "microsoft.graph.report",
    "content": "<Unknown Primitive Type Edm.Stream>"
  }
}
```





