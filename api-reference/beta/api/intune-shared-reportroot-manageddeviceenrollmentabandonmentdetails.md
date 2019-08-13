---
title: managedDeviceEnrollmentAbandonmentDetails 函数
description: 注册 abandonment 详细信息报告的元数据
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e8519f49ca93ee846dcb291d1a77ce44f81f2f86
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36347421"
---
# <a name="manageddeviceenrollmentabandonmentdetails-function"></a><span data-ttu-id="7adc3-103">managedDeviceEnrollmentAbandonmentDetails 函数</span><span class="sxs-lookup"><span data-stu-id="7adc3-103">managedDeviceEnrollmentAbandonmentDetails function</span></span>

> <span data-ttu-id="7adc3-104">**重要说明:** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="7adc3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7adc3-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7adc3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7adc3-106">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7adc3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7adc3-107">注册 abandonment 详细信息报告的元数据</span><span class="sxs-lookup"><span data-stu-id="7adc3-107">Metadata for Enrollment abandonment details report</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7adc3-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="7adc3-108">Prerequisites</span></span>
<span data-ttu-id="7adc3-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7adc3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7adc3-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7adc3-111">Permission type</span></span>|<span data-ttu-id="7adc3-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7adc3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7adc3-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7adc3-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="7adc3-114">&nbsp;&nbsp; **Troublshooting**</span><span class="sxs-lookup"><span data-stu-id="7adc3-114">&nbsp; &nbsp; **Troublshooting**</span></span> | <span data-ttu-id="7adc3-115">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="7adc3-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="7adc3-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7adc3-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7adc3-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="7adc3-117">Not supported.</span></span>|
|<span data-ttu-id="7adc3-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="7adc3-118">Application</span></span>|<span data-ttu-id="7adc3-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="7adc3-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7adc3-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7adc3-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentAbandonmentDetails
```

## <a name="request-headers"></a><span data-ttu-id="7adc3-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="7adc3-121">Request headers</span></span>
|<span data-ttu-id="7adc3-122">标头</span><span class="sxs-lookup"><span data-stu-id="7adc3-122">Header</span></span>|<span data-ttu-id="7adc3-123">值</span><span class="sxs-lookup"><span data-stu-id="7adc3-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7adc3-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="7adc3-124">Authorization</span></span>|<span data-ttu-id="7adc3-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7adc3-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7adc3-126">接受</span><span class="sxs-lookup"><span data-stu-id="7adc3-126">Accept</span></span>|<span data-ttu-id="7adc3-127">application/json</span><span class="sxs-lookup"><span data-stu-id="7adc3-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7adc3-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="7adc3-128">Request body</span></span>
<span data-ttu-id="7adc3-129">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="7adc3-129">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="7adc3-130">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="7adc3-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="7adc3-131">属性</span><span class="sxs-lookup"><span data-stu-id="7adc3-131">Property</span></span>|<span data-ttu-id="7adc3-132">类型</span><span class="sxs-lookup"><span data-stu-id="7adc3-132">Type</span></span>|<span data-ttu-id="7adc3-133">说明</span><span class="sxs-lookup"><span data-stu-id="7adc3-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7adc3-134">skip</span><span class="sxs-lookup"><span data-stu-id="7adc3-134">skip</span></span>|<span data-ttu-id="7adc3-135">Int32</span><span class="sxs-lookup"><span data-stu-id="7adc3-135">Int32</span></span>|<span data-ttu-id="7adc3-136">尚未记录</span><span class="sxs-lookup"><span data-stu-id="7adc3-136">Not yet documented</span></span>|
|<span data-ttu-id="7adc3-137">top</span><span class="sxs-lookup"><span data-stu-id="7adc3-137">top</span></span>|<span data-ttu-id="7adc3-138">Int32</span><span class="sxs-lookup"><span data-stu-id="7adc3-138">Int32</span></span>|<span data-ttu-id="7adc3-139">尚未记录</span><span class="sxs-lookup"><span data-stu-id="7adc3-139">Not yet documented</span></span>|
|<span data-ttu-id="7adc3-140">filter</span><span class="sxs-lookup"><span data-stu-id="7adc3-140">filter</span></span>|<span data-ttu-id="7adc3-141">String</span><span class="sxs-lookup"><span data-stu-id="7adc3-141">String</span></span>|<span data-ttu-id="7adc3-142">尚未记录</span><span class="sxs-lookup"><span data-stu-id="7adc3-142">Not yet documented</span></span>|
|<span data-ttu-id="7adc3-143">skipToken</span><span class="sxs-lookup"><span data-stu-id="7adc3-143">skipToken</span></span>|<span data-ttu-id="7adc3-144">String</span><span class="sxs-lookup"><span data-stu-id="7adc3-144">String</span></span>|<span data-ttu-id="7adc3-145">尚未记录</span><span class="sxs-lookup"><span data-stu-id="7adc3-145">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="7adc3-146">响应</span><span class="sxs-lookup"><span data-stu-id="7adc3-146">Response</span></span>
<span data-ttu-id="7adc3-147">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 [report](../resources/intune-shared-report.md)。</span><span class="sxs-lookup"><span data-stu-id="7adc3-147">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7adc3-148">示例</span><span class="sxs-lookup"><span data-stu-id="7adc3-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="7adc3-149">请求</span><span class="sxs-lookup"><span data-stu-id="7adc3-149">Request</span></span>
<span data-ttu-id="7adc3-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7adc3-150">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentAbandonmentDetails(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="7adc3-151">响应</span><span class="sxs-lookup"><span data-stu-id="7adc3-151">Response</span></span>
<span data-ttu-id="7adc3-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7adc3-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








