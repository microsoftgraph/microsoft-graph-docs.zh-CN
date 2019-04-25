---
title: managedDeviceEnrollmentTopFailures 函数
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: edc44099ed325455b3bd94b01aa1cec9b9582c0e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32526844"
---
# <a name="manageddeviceenrollmenttopfailures-function"></a><span data-ttu-id="40468-103">managedDeviceEnrollmentTopFailures 函数</span><span class="sxs-lookup"><span data-stu-id="40468-103">managedDeviceEnrollmentTopFailures function</span></span>

> <span data-ttu-id="40468-104">**重要说明:** Microsoft Graph 中的/beta 版本下的 api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="40468-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="40468-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="40468-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="40468-106">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="40468-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="40468-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="40468-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="40468-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="40468-108">Prerequisites</span></span>
<span data-ttu-id="40468-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="40468-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40468-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="40468-111">Permission type</span></span>|<span data-ttu-id="40468-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="40468-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="40468-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="40468-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="40468-114">&nbsp; &nbsp; **疑难解答**</span><span class="sxs-lookup"><span data-stu-id="40468-114">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="40468-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40468-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="40468-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="40468-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="40468-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="40468-117">Not supported.</span></span>|
|<span data-ttu-id="40468-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="40468-118">Application</span></span>|<span data-ttu-id="40468-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="40468-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="40468-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="40468-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentTopFailures
```

## <a name="request-headers"></a><span data-ttu-id="40468-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="40468-121">Request headers</span></span>
|<span data-ttu-id="40468-122">标头</span><span class="sxs-lookup"><span data-stu-id="40468-122">Header</span></span>|<span data-ttu-id="40468-123">值</span><span class="sxs-lookup"><span data-stu-id="40468-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="40468-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="40468-124">Authorization</span></span>|<span data-ttu-id="40468-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="40468-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="40468-126">接受</span><span class="sxs-lookup"><span data-stu-id="40468-126">Accept</span></span>|<span data-ttu-id="40468-127">application/json</span><span class="sxs-lookup"><span data-stu-id="40468-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="40468-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="40468-128">Request body</span></span>
<span data-ttu-id="40468-129">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="40468-129">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="40468-130">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="40468-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="40468-131">属性</span><span class="sxs-lookup"><span data-stu-id="40468-131">Property</span></span>|<span data-ttu-id="40468-132">类型</span><span class="sxs-lookup"><span data-stu-id="40468-132">Type</span></span>|<span data-ttu-id="40468-133">说明</span><span class="sxs-lookup"><span data-stu-id="40468-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40468-134">period</span><span class="sxs-lookup"><span data-stu-id="40468-134">period</span></span>|<span data-ttu-id="40468-135">String</span><span class="sxs-lookup"><span data-stu-id="40468-135">String</span></span>|<span data-ttu-id="40468-136">尚未记录</span><span class="sxs-lookup"><span data-stu-id="40468-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="40468-137">响应</span><span class="sxs-lookup"><span data-stu-id="40468-137">Response</span></span>
<span data-ttu-id="40468-138">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 [report](../resources/intune-shared-report.md)。</span><span class="sxs-lookup"><span data-stu-id="40468-138">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40468-139">示例</span><span class="sxs-lookup"><span data-stu-id="40468-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="40468-140">请求</span><span class="sxs-lookup"><span data-stu-id="40468-140">Request</span></span>
<span data-ttu-id="40468-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="40468-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentTopFailures(period='parameterValue')
```

### <a name="response"></a><span data-ttu-id="40468-142">响应</span><span class="sxs-lookup"><span data-stu-id="40468-142">Response</span></span>
<span data-ttu-id="40468-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="40468-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



