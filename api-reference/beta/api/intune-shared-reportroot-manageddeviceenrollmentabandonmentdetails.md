---
title: managedDeviceEnrollmentAbandonmentDetails 函数
description: 注册 abandonment 详细信息报告的元数据
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 30312706926293e24226801a7e0193b28d3d6f9c
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30956609"
---
# <a name="manageddeviceenrollmentabandonmentdetails-function"></a><span data-ttu-id="ea437-103">managedDeviceEnrollmentAbandonmentDetails 函数</span><span class="sxs-lookup"><span data-stu-id="ea437-103">managedDeviceEnrollmentAbandonmentDetails function</span></span>

> <span data-ttu-id="ea437-104">**重要说明:** Microsoft Graph 中的/beta 版本下的 api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ea437-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ea437-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ea437-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ea437-106">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ea437-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ea437-107">注册 abandonment 详细信息报告的元数据</span><span class="sxs-lookup"><span data-stu-id="ea437-107">Metadata for Enrollment abandonment details report</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ea437-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="ea437-108">Prerequisites</span></span>
<span data-ttu-id="ea437-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ea437-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea437-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ea437-111">Permission type</span></span>|<span data-ttu-id="ea437-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ea437-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ea437-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ea437-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="ea437-114">&nbsp;&nbsp; **Troublshooting**</span><span class="sxs-lookup"><span data-stu-id="ea437-114">&nbsp; &nbsp; **Troublshooting**</span></span> | <span data-ttu-id="ea437-115">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="ea437-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="ea437-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ea437-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ea437-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="ea437-117">Not supported.</span></span>|
|<span data-ttu-id="ea437-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="ea437-118">Application</span></span>|<span data-ttu-id="ea437-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="ea437-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ea437-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ea437-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentAbandonmentDetails
```

## <a name="request-headers"></a><span data-ttu-id="ea437-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="ea437-121">Request headers</span></span>
|<span data-ttu-id="ea437-122">标头</span><span class="sxs-lookup"><span data-stu-id="ea437-122">Header</span></span>|<span data-ttu-id="ea437-123">值</span><span class="sxs-lookup"><span data-stu-id="ea437-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ea437-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ea437-124">Authorization</span></span>|<span data-ttu-id="ea437-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ea437-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ea437-126">接受</span><span class="sxs-lookup"><span data-stu-id="ea437-126">Accept</span></span>|<span data-ttu-id="ea437-127">application/json</span><span class="sxs-lookup"><span data-stu-id="ea437-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ea437-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="ea437-128">Request body</span></span>
<span data-ttu-id="ea437-129">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="ea437-129">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="ea437-130">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="ea437-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="ea437-131">属性</span><span class="sxs-lookup"><span data-stu-id="ea437-131">Property</span></span>|<span data-ttu-id="ea437-132">类型</span><span class="sxs-lookup"><span data-stu-id="ea437-132">Type</span></span>|<span data-ttu-id="ea437-133">说明</span><span class="sxs-lookup"><span data-stu-id="ea437-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea437-134">skip</span><span class="sxs-lookup"><span data-stu-id="ea437-134">skip</span></span>|<span data-ttu-id="ea437-135">Int32</span><span class="sxs-lookup"><span data-stu-id="ea437-135">Int32</span></span>|<span data-ttu-id="ea437-136">尚未记录</span><span class="sxs-lookup"><span data-stu-id="ea437-136">Not yet documented</span></span>|
|<span data-ttu-id="ea437-137">top</span><span class="sxs-lookup"><span data-stu-id="ea437-137">top</span></span>|<span data-ttu-id="ea437-138">Int32</span><span class="sxs-lookup"><span data-stu-id="ea437-138">Int32</span></span>|<span data-ttu-id="ea437-139">尚未记录</span><span class="sxs-lookup"><span data-stu-id="ea437-139">Not yet documented</span></span>|
|<span data-ttu-id="ea437-140">筛选器</span><span class="sxs-lookup"><span data-stu-id="ea437-140">filter</span></span>|<span data-ttu-id="ea437-141">String</span><span class="sxs-lookup"><span data-stu-id="ea437-141">String</span></span>|<span data-ttu-id="ea437-142">尚未记录</span><span class="sxs-lookup"><span data-stu-id="ea437-142">Not yet documented</span></span>|
|<span data-ttu-id="ea437-143">skipToken</span><span class="sxs-lookup"><span data-stu-id="ea437-143">skipToken</span></span>|<span data-ttu-id="ea437-144">String</span><span class="sxs-lookup"><span data-stu-id="ea437-144">String</span></span>|<span data-ttu-id="ea437-145">尚未记录</span><span class="sxs-lookup"><span data-stu-id="ea437-145">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="ea437-146">响应</span><span class="sxs-lookup"><span data-stu-id="ea437-146">Response</span></span>
<span data-ttu-id="ea437-147">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 [report](../resources/intune-shared-report.md)。</span><span class="sxs-lookup"><span data-stu-id="ea437-147">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea437-148">示例</span><span class="sxs-lookup"><span data-stu-id="ea437-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="ea437-149">请求</span><span class="sxs-lookup"><span data-stu-id="ea437-149">Request</span></span>
<span data-ttu-id="ea437-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ea437-150">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentAbandonmentDetails(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="ea437-151">响应</span><span class="sxs-lookup"><span data-stu-id="ea437-151">Response</span></span>
<span data-ttu-id="ea437-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ea437-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





