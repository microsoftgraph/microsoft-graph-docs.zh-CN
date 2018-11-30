---
title: managedDeviceEnrollmentFailureDetails 函数
description: 尚未记录
ms.openlocfilehash: c5e68453cb1655e4018156ac207b60e4145e571a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27010672"
---
# <a name="manageddeviceenrollmentfailuredetails-function"></a><span data-ttu-id="cbfb4-103">managedDeviceEnrollmentFailureDetails 函数</span><span class="sxs-lookup"><span data-stu-id="cbfb4-103">managedDeviceEnrollmentFailureDetails function</span></span>

> <span data-ttu-id="cbfb4-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="cbfb4-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cbfb4-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="cbfb4-105">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cbfb4-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="cbfb4-106">Prerequisites</span></span>
<span data-ttu-id="cbfb4-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="cbfb4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cbfb4-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="cbfb4-109">Permission type</span></span>|<span data-ttu-id="cbfb4-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="cbfb4-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cbfb4-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cbfb4-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="cbfb4-112">&nbsp;&nbsp;疑难解答</span><span class="sxs-lookup"><span data-stu-id="cbfb4-112">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="cbfb4-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cbfb4-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="cbfb4-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cbfb4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cbfb4-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="cbfb4-115">Not supported.</span></span>|
|<span data-ttu-id="cbfb4-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="cbfb4-116">Application</span></span>|<span data-ttu-id="cbfb4-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="cbfb4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cbfb4-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cbfb4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentFailureDetails
```

## <a name="request-headers"></a><span data-ttu-id="cbfb4-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="cbfb4-119">Request headers</span></span>
|<span data-ttu-id="cbfb4-120">标头</span><span class="sxs-lookup"><span data-stu-id="cbfb4-120">Header</span></span>|<span data-ttu-id="cbfb4-121">值</span><span class="sxs-lookup"><span data-stu-id="cbfb4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cbfb4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cbfb4-122">Authorization</span></span>|<span data-ttu-id="cbfb4-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="cbfb4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cbfb4-124">Accept</span><span class="sxs-lookup"><span data-stu-id="cbfb4-124">Accept</span></span>|<span data-ttu-id="cbfb4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cbfb4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cbfb4-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="cbfb4-126">Request body</span></span>
<span data-ttu-id="cbfb4-127">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="cbfb4-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="cbfb4-128">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="cbfb4-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="cbfb4-129">属性</span><span class="sxs-lookup"><span data-stu-id="cbfb4-129">Property</span></span>|<span data-ttu-id="cbfb4-130">类型</span><span class="sxs-lookup"><span data-stu-id="cbfb4-130">Type</span></span>|<span data-ttu-id="cbfb4-131">说明</span><span class="sxs-lookup"><span data-stu-id="cbfb4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cbfb4-132">skip</span><span class="sxs-lookup"><span data-stu-id="cbfb4-132">skip</span></span>|<span data-ttu-id="cbfb4-133">Int32</span><span class="sxs-lookup"><span data-stu-id="cbfb4-133">Int32</span></span>|<span data-ttu-id="cbfb4-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="cbfb4-134">Not yet documented</span></span>|
|<span data-ttu-id="cbfb4-135">top</span><span class="sxs-lookup"><span data-stu-id="cbfb4-135">top</span></span>|<span data-ttu-id="cbfb4-136">Int32</span><span class="sxs-lookup"><span data-stu-id="cbfb4-136">Int32</span></span>|<span data-ttu-id="cbfb4-137">尚未记录</span><span class="sxs-lookup"><span data-stu-id="cbfb4-137">Not yet documented</span></span>|
|<span data-ttu-id="cbfb4-138">filter</span><span class="sxs-lookup"><span data-stu-id="cbfb4-138">filter</span></span>|<span data-ttu-id="cbfb4-139">字符串</span><span class="sxs-lookup"><span data-stu-id="cbfb4-139">String</span></span>|<span data-ttu-id="cbfb4-140">尚未记录</span><span class="sxs-lookup"><span data-stu-id="cbfb4-140">Not yet documented</span></span>|
|<span data-ttu-id="cbfb4-141">skipToken</span><span class="sxs-lookup"><span data-stu-id="cbfb4-141">skipToken</span></span>|<span data-ttu-id="cbfb4-142">字符串</span><span class="sxs-lookup"><span data-stu-id="cbfb4-142">String</span></span>|<span data-ttu-id="cbfb4-143">尚未记录</span><span class="sxs-lookup"><span data-stu-id="cbfb4-143">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="cbfb4-144">响应</span><span class="sxs-lookup"><span data-stu-id="cbfb4-144">Response</span></span>
<span data-ttu-id="cbfb4-145">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 [report](../resources/intune-shared-report.md)。</span><span class="sxs-lookup"><span data-stu-id="cbfb4-145">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cbfb4-146">示例</span><span class="sxs-lookup"><span data-stu-id="cbfb4-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="cbfb4-147">请求</span><span class="sxs-lookup"><span data-stu-id="cbfb4-147">Request</span></span>
<span data-ttu-id="cbfb4-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cbfb4-148">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1/reports/managedDeviceEnrollmentFailureDetails(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="cbfb4-149">响应</span><span class="sxs-lookup"><span data-stu-id="cbfb4-149">Response</span></span>
<span data-ttu-id="cbfb4-150">为简便起见，如下所示的响应对象可能会被截断。</span><span class="sxs-lookup"><span data-stu-id="cbfb4-150">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="cbfb4-151">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cbfb4-151">All of the properties will be returned from an actual call.</span></span>

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




