---
title: managedDeviceEnrollmentTopFailures 函数
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 169c1f14b66b2e91f94c1cd23046c1d9c8c4a8b2
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39939576"
---
# <a name="manageddeviceenrollmenttopfailures-function"></a><span data-ttu-id="ff249-103">managedDeviceEnrollmentTopFailures 函数</span><span class="sxs-lookup"><span data-stu-id="ff249-103">managedDeviceEnrollmentTopFailures function</span></span>

> <span data-ttu-id="ff249-104">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ff249-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ff249-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ff249-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ff249-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ff249-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff249-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="ff249-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ff249-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="ff249-108">Prerequisites</span></span>
<span data-ttu-id="ff249-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ff249-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff249-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ff249-111">Permission type</span></span>|<span data-ttu-id="ff249-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ff249-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ff249-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ff249-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="ff249-114">&nbsp; &nbsp; **故障排除**</span><span class="sxs-lookup"><span data-stu-id="ff249-114">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="ff249-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff249-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="ff249-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ff249-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ff249-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="ff249-117">Not supported.</span></span>|
|<span data-ttu-id="ff249-118">Application</span><span class="sxs-lookup"><span data-stu-id="ff249-118">Application</span></span>||
| <span data-ttu-id="ff249-119">&nbsp; &nbsp; **故障排除**</span><span class="sxs-lookup"><span data-stu-id="ff249-119">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="ff249-120">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff249-120">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ff249-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ff249-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentTopFailures
```

## <a name="request-headers"></a><span data-ttu-id="ff249-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="ff249-122">Request headers</span></span>
|<span data-ttu-id="ff249-123">标头</span><span class="sxs-lookup"><span data-stu-id="ff249-123">Header</span></span>|<span data-ttu-id="ff249-124">值</span><span class="sxs-lookup"><span data-stu-id="ff249-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ff249-125">授权</span><span class="sxs-lookup"><span data-stu-id="ff249-125">Authorization</span></span>|<span data-ttu-id="ff249-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ff249-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ff249-127">接受</span><span class="sxs-lookup"><span data-stu-id="ff249-127">Accept</span></span>|<span data-ttu-id="ff249-128">application/json</span><span class="sxs-lookup"><span data-stu-id="ff249-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff249-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="ff249-129">Request body</span></span>
<span data-ttu-id="ff249-130">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="ff249-130">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="ff249-131">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="ff249-131">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="ff249-132">属性</span><span class="sxs-lookup"><span data-stu-id="ff249-132">Property</span></span>|<span data-ttu-id="ff249-133">类型</span><span class="sxs-lookup"><span data-stu-id="ff249-133">Type</span></span>|<span data-ttu-id="ff249-134">说明</span><span class="sxs-lookup"><span data-stu-id="ff249-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff249-135">period</span><span class="sxs-lookup"><span data-stu-id="ff249-135">period</span></span>|<span data-ttu-id="ff249-136">String</span><span class="sxs-lookup"><span data-stu-id="ff249-136">String</span></span>|<span data-ttu-id="ff249-137">尚未记录</span><span class="sxs-lookup"><span data-stu-id="ff249-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="ff249-138">响应</span><span class="sxs-lookup"><span data-stu-id="ff249-138">Response</span></span>
<span data-ttu-id="ff249-139">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 [report](../resources/intune-shared-report.md)。</span><span class="sxs-lookup"><span data-stu-id="ff249-139">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff249-140">示例</span><span class="sxs-lookup"><span data-stu-id="ff249-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="ff249-141">请求</span><span class="sxs-lookup"><span data-stu-id="ff249-141">Request</span></span>
<span data-ttu-id="ff249-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ff249-142">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentTopFailures(period='parameterValue')
```

### <a name="response"></a><span data-ttu-id="ff249-143">响应</span><span class="sxs-lookup"><span data-stu-id="ff249-143">Response</span></span>
<span data-ttu-id="ff249-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ff249-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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











