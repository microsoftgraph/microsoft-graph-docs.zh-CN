---
title: managedDeviceEnrollmentTopFailures 函数
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 4e9ff98c2ddc55110026153c854d91901ffd2335
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882969"
---
# <a name="manageddeviceenrollmenttopfailures-function"></a><span data-ttu-id="ca033-103">managedDeviceEnrollmentTopFailures 函数</span><span class="sxs-lookup"><span data-stu-id="ca033-103">managedDeviceEnrollmentTopFailures function</span></span>

> <span data-ttu-id="ca033-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ca033-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ca033-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="ca033-105">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ca033-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="ca033-106">Prerequisites</span></span>
<span data-ttu-id="ca033-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="ca033-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca033-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ca033-109">Permission type</span></span>|<span data-ttu-id="ca033-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ca033-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ca033-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ca033-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="ca033-112">&nbsp;&nbsp;疑难解答</span><span class="sxs-lookup"><span data-stu-id="ca033-112">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="ca033-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca033-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="ca033-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ca033-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ca033-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ca033-115">Not supported.</span></span>|
|<span data-ttu-id="ca033-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ca033-116">Application</span></span>|<span data-ttu-id="ca033-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="ca033-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ca033-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ca033-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentTopFailures
```

## <a name="request-headers"></a><span data-ttu-id="ca033-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ca033-119">Request headers</span></span>
|<span data-ttu-id="ca033-120">标头</span><span class="sxs-lookup"><span data-stu-id="ca033-120">Header</span></span>|<span data-ttu-id="ca033-121">值</span><span class="sxs-lookup"><span data-stu-id="ca033-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ca033-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ca033-122">Authorization</span></span>|<span data-ttu-id="ca033-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ca033-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ca033-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ca033-124">Accept</span></span>|<span data-ttu-id="ca033-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ca033-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ca033-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ca033-126">Request body</span></span>
<span data-ttu-id="ca033-127">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="ca033-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="ca033-128">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="ca033-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="ca033-129">属性</span><span class="sxs-lookup"><span data-stu-id="ca033-129">Property</span></span>|<span data-ttu-id="ca033-130">类型</span><span class="sxs-lookup"><span data-stu-id="ca033-130">Type</span></span>|<span data-ttu-id="ca033-131">说明</span><span class="sxs-lookup"><span data-stu-id="ca033-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca033-132">period</span><span class="sxs-lookup"><span data-stu-id="ca033-132">period</span></span>|<span data-ttu-id="ca033-133">字符串</span><span class="sxs-lookup"><span data-stu-id="ca033-133">String</span></span>|<span data-ttu-id="ca033-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="ca033-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="ca033-135">响应</span><span class="sxs-lookup"><span data-stu-id="ca033-135">Response</span></span>
<span data-ttu-id="ca033-136">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 [report](../resources/intune-shared-report.md)。</span><span class="sxs-lookup"><span data-stu-id="ca033-136">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca033-137">示例</span><span class="sxs-lookup"><span data-stu-id="ca033-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="ca033-138">请求</span><span class="sxs-lookup"><span data-stu-id="ca033-138">Request</span></span>
<span data-ttu-id="ca033-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ca033-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1/reports/managedDeviceEnrollmentTopFailures(period='parameterValue')
```

### <a name="response"></a><span data-ttu-id="ca033-140">响应</span><span class="sxs-lookup"><span data-stu-id="ca033-140">Response</span></span>
<span data-ttu-id="ca033-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ca033-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




