---
title: managedDeviceEnrollmentAbandonmentSummary 函数
description: 注册 abandonment 摘要报告的元数据
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4ebb529e5c56ee62a6836be5e27914e1ed530155
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43470340"
---
# <a name="manageddeviceenrollmentabandonmentsummary-function"></a><span data-ttu-id="6aefe-103">managedDeviceEnrollmentAbandonmentSummary 函数</span><span class="sxs-lookup"><span data-stu-id="6aefe-103">managedDeviceEnrollmentAbandonmentSummary function</span></span>

<span data-ttu-id="6aefe-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6aefe-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6aefe-105">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="6aefe-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6aefe-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6aefe-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6aefe-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6aefe-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6aefe-108">注册 abandonment 摘要报告的元数据</span><span class="sxs-lookup"><span data-stu-id="6aefe-108">Metadata for Enrollment abandonment summary report</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6aefe-109">先决条件</span><span class="sxs-lookup"><span data-stu-id="6aefe-109">Prerequisites</span></span>
<span data-ttu-id="6aefe-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6aefe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6aefe-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="6aefe-112">Permission type</span></span>|<span data-ttu-id="6aefe-113">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6aefe-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6aefe-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6aefe-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="6aefe-115">&nbsp;&nbsp; **Troublshooting**</span><span class="sxs-lookup"><span data-stu-id="6aefe-115">&nbsp; &nbsp; **Troublshooting**</span></span> | <span data-ttu-id="6aefe-116">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="6aefe-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="6aefe-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6aefe-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6aefe-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="6aefe-118">Not supported.</span></span>|
|<span data-ttu-id="6aefe-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="6aefe-119">Application</span></span>||
| <span data-ttu-id="6aefe-120">&nbsp;&nbsp; **Troublshooting**</span><span class="sxs-lookup"><span data-stu-id="6aefe-120">&nbsp; &nbsp; **Troublshooting**</span></span> | <span data-ttu-id="6aefe-121">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="6aefe-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6aefe-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6aefe-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentAbandonmentSummary
```

## <a name="request-headers"></a><span data-ttu-id="6aefe-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="6aefe-123">Request headers</span></span>
|<span data-ttu-id="6aefe-124">标头</span><span class="sxs-lookup"><span data-stu-id="6aefe-124">Header</span></span>|<span data-ttu-id="6aefe-125">值</span><span class="sxs-lookup"><span data-stu-id="6aefe-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6aefe-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="6aefe-126">Authorization</span></span>|<span data-ttu-id="6aefe-127">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6aefe-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6aefe-128">接受</span><span class="sxs-lookup"><span data-stu-id="6aefe-128">Accept</span></span>|<span data-ttu-id="6aefe-129">application/json</span><span class="sxs-lookup"><span data-stu-id="6aefe-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6aefe-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="6aefe-130">Request body</span></span>
<span data-ttu-id="6aefe-131">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="6aefe-131">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="6aefe-132">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="6aefe-132">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="6aefe-133">属性</span><span class="sxs-lookup"><span data-stu-id="6aefe-133">Property</span></span>|<span data-ttu-id="6aefe-134">类型</span><span class="sxs-lookup"><span data-stu-id="6aefe-134">Type</span></span>|<span data-ttu-id="6aefe-135">说明</span><span class="sxs-lookup"><span data-stu-id="6aefe-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6aefe-136">skip</span><span class="sxs-lookup"><span data-stu-id="6aefe-136">skip</span></span>|<span data-ttu-id="6aefe-137">Int32</span><span class="sxs-lookup"><span data-stu-id="6aefe-137">Int32</span></span>|<span data-ttu-id="6aefe-138">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6aefe-138">Not yet documented</span></span>|
|<span data-ttu-id="6aefe-139">top</span><span class="sxs-lookup"><span data-stu-id="6aefe-139">top</span></span>|<span data-ttu-id="6aefe-140">Int32</span><span class="sxs-lookup"><span data-stu-id="6aefe-140">Int32</span></span>|<span data-ttu-id="6aefe-141">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6aefe-141">Not yet documented</span></span>|
|<span data-ttu-id="6aefe-142">filter</span><span class="sxs-lookup"><span data-stu-id="6aefe-142">filter</span></span>|<span data-ttu-id="6aefe-143">String</span><span class="sxs-lookup"><span data-stu-id="6aefe-143">String</span></span>|<span data-ttu-id="6aefe-144">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6aefe-144">Not yet documented</span></span>|
|<span data-ttu-id="6aefe-145">skipToken</span><span class="sxs-lookup"><span data-stu-id="6aefe-145">skipToken</span></span>|<span data-ttu-id="6aefe-146">String</span><span class="sxs-lookup"><span data-stu-id="6aefe-146">String</span></span>|<span data-ttu-id="6aefe-147">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6aefe-147">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="6aefe-148">响应</span><span class="sxs-lookup"><span data-stu-id="6aefe-148">Response</span></span>
<span data-ttu-id="6aefe-149">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 [report](../resources/intune-shared-report.md)。</span><span class="sxs-lookup"><span data-stu-id="6aefe-149">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6aefe-150">示例</span><span class="sxs-lookup"><span data-stu-id="6aefe-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="6aefe-151">请求</span><span class="sxs-lookup"><span data-stu-id="6aefe-151">Request</span></span>
<span data-ttu-id="6aefe-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6aefe-152">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentAbandonmentSummary(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="6aefe-153">响应</span><span class="sxs-lookup"><span data-stu-id="6aefe-153">Response</span></span>
<span data-ttu-id="6aefe-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6aefe-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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











