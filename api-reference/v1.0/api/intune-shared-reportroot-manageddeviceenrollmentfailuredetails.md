---
title: managedDeviceEnrollmentFailureDetails 函数
description: 尚未记录
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fd16afe8aafaefe84f385d13a9a56e823b689130
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37361369"
---
# <a name="manageddeviceenrollmentfailuredetails-function"></a><span data-ttu-id="61e3b-103">managedDeviceEnrollmentFailureDetails 函数</span><span class="sxs-lookup"><span data-stu-id="61e3b-103">managedDeviceEnrollmentFailureDetails function</span></span>

> <span data-ttu-id="61e3b-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="61e3b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="61e3b-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="61e3b-105">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="61e3b-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="61e3b-106">Prerequisites</span></span>
<span data-ttu-id="61e3b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="61e3b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="61e3b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="61e3b-109">Permission type</span></span>|<span data-ttu-id="61e3b-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="61e3b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="61e3b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="61e3b-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="61e3b-112">&nbsp;&nbsp;故障排除</span><span class="sxs-lookup"><span data-stu-id="61e3b-112">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="61e3b-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61e3b-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="61e3b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="61e3b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="61e3b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="61e3b-115">Not supported.</span></span>|
|<span data-ttu-id="61e3b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="61e3b-116">Application</span></span>|<span data-ttu-id="61e3b-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="61e3b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="61e3b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="61e3b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentFailureDetails
```

## <a name="request-headers"></a><span data-ttu-id="61e3b-119">请求头</span><span class="sxs-lookup"><span data-stu-id="61e3b-119">Request headers</span></span>
|<span data-ttu-id="61e3b-120">标头</span><span class="sxs-lookup"><span data-stu-id="61e3b-120">Header</span></span>|<span data-ttu-id="61e3b-121">值</span><span class="sxs-lookup"><span data-stu-id="61e3b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="61e3b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="61e3b-122">Authorization</span></span>|<span data-ttu-id="61e3b-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="61e3b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="61e3b-124">接受</span><span class="sxs-lookup"><span data-stu-id="61e3b-124">Accept</span></span>|<span data-ttu-id="61e3b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="61e3b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="61e3b-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="61e3b-126">Request body</span></span>
<span data-ttu-id="61e3b-127">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="61e3b-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="61e3b-128">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="61e3b-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="61e3b-129">属性</span><span class="sxs-lookup"><span data-stu-id="61e3b-129">Property</span></span>|<span data-ttu-id="61e3b-130">类型</span><span class="sxs-lookup"><span data-stu-id="61e3b-130">Type</span></span>|<span data-ttu-id="61e3b-131">说明</span><span class="sxs-lookup"><span data-stu-id="61e3b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61e3b-132">skip</span><span class="sxs-lookup"><span data-stu-id="61e3b-132">skip</span></span>|<span data-ttu-id="61e3b-133">Int32</span><span class="sxs-lookup"><span data-stu-id="61e3b-133">Int32</span></span>|<span data-ttu-id="61e3b-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="61e3b-134">Not yet documented</span></span>|
|<span data-ttu-id="61e3b-135">top</span><span class="sxs-lookup"><span data-stu-id="61e3b-135">top</span></span>|<span data-ttu-id="61e3b-136">Int32</span><span class="sxs-lookup"><span data-stu-id="61e3b-136">Int32</span></span>|<span data-ttu-id="61e3b-137">尚未记录</span><span class="sxs-lookup"><span data-stu-id="61e3b-137">Not yet documented</span></span>|
|<span data-ttu-id="61e3b-138">filter</span><span class="sxs-lookup"><span data-stu-id="61e3b-138">filter</span></span>|<span data-ttu-id="61e3b-139">String</span><span class="sxs-lookup"><span data-stu-id="61e3b-139">String</span></span>|<span data-ttu-id="61e3b-140">尚未记录</span><span class="sxs-lookup"><span data-stu-id="61e3b-140">Not yet documented</span></span>|
|<span data-ttu-id="61e3b-141">skipToken</span><span class="sxs-lookup"><span data-stu-id="61e3b-141">skipToken</span></span>|<span data-ttu-id="61e3b-142">String</span><span class="sxs-lookup"><span data-stu-id="61e3b-142">String</span></span>|<span data-ttu-id="61e3b-143">尚未记录</span><span class="sxs-lookup"><span data-stu-id="61e3b-143">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="61e3b-144">响应</span><span class="sxs-lookup"><span data-stu-id="61e3b-144">Response</span></span>
<span data-ttu-id="61e3b-145">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 [report](../resources/intune-shared-report.md)。</span><span class="sxs-lookup"><span data-stu-id="61e3b-145">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="61e3b-146">示例</span><span class="sxs-lookup"><span data-stu-id="61e3b-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="61e3b-147">请求</span><span class="sxs-lookup"><span data-stu-id="61e3b-147">Request</span></span>
<span data-ttu-id="61e3b-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="61e3b-148">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1/reports/managedDeviceEnrollmentFailureDetails(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="61e3b-149">响应</span><span class="sxs-lookup"><span data-stu-id="61e3b-149">Response</span></span>
<span data-ttu-id="61e3b-150">为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="61e3b-150">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="61e3b-151">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="61e3b-151">All of the properties will be returned from an actual call.</span></span>

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





