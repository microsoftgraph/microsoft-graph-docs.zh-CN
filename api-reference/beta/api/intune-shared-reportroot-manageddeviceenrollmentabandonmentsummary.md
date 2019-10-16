---
title: managedDeviceEnrollmentAbandonmentSummary 函数
description: 注册 abandonment 摘要报告的元数据
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e6e8502f609b2f9b1d23580d0b7d5e38f20226cc
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37537928"
---
# <a name="manageddeviceenrollmentabandonmentsummary-function"></a><span data-ttu-id="f9ef6-103">managedDeviceEnrollmentAbandonmentSummary 函数</span><span class="sxs-lookup"><span data-stu-id="f9ef6-103">managedDeviceEnrollmentAbandonmentSummary function</span></span>

> <span data-ttu-id="f9ef6-104">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f9ef6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f9ef6-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f9ef6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f9ef6-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f9ef6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f9ef6-107">注册 abandonment 摘要报告的元数据</span><span class="sxs-lookup"><span data-stu-id="f9ef6-107">Metadata for Enrollment abandonment summary report</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f9ef6-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="f9ef6-108">Prerequisites</span></span>
<span data-ttu-id="f9ef6-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f9ef6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9ef6-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f9ef6-111">Permission type</span></span>|<span data-ttu-id="f9ef6-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f9ef6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f9ef6-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f9ef6-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="f9ef6-114">&nbsp;&nbsp; **Troublshooting**</span><span class="sxs-lookup"><span data-stu-id="f9ef6-114">&nbsp; &nbsp; **Troublshooting**</span></span> | <span data-ttu-id="f9ef6-115">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="f9ef6-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="f9ef6-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f9ef6-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f9ef6-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="f9ef6-117">Not supported.</span></span>|
|<span data-ttu-id="f9ef6-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="f9ef6-118">Application</span></span>||
| <span data-ttu-id="f9ef6-119">&nbsp;&nbsp; **Troublshooting**</span><span class="sxs-lookup"><span data-stu-id="f9ef6-119">&nbsp; &nbsp; **Troublshooting**</span></span> | <span data-ttu-id="f9ef6-120">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="f9ef6-120">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f9ef6-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f9ef6-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentAbandonmentSummary
```

## <a name="request-headers"></a><span data-ttu-id="f9ef6-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="f9ef6-122">Request headers</span></span>
|<span data-ttu-id="f9ef6-123">标头</span><span class="sxs-lookup"><span data-stu-id="f9ef6-123">Header</span></span>|<span data-ttu-id="f9ef6-124">值</span><span class="sxs-lookup"><span data-stu-id="f9ef6-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f9ef6-125">授权</span><span class="sxs-lookup"><span data-stu-id="f9ef6-125">Authorization</span></span>|<span data-ttu-id="f9ef6-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f9ef6-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f9ef6-127">接受</span><span class="sxs-lookup"><span data-stu-id="f9ef6-127">Accept</span></span>|<span data-ttu-id="f9ef6-128">application/json</span><span class="sxs-lookup"><span data-stu-id="f9ef6-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9ef6-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="f9ef6-129">Request body</span></span>
<span data-ttu-id="f9ef6-130">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="f9ef6-130">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="f9ef6-131">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="f9ef6-131">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="f9ef6-132">属性</span><span class="sxs-lookup"><span data-stu-id="f9ef6-132">Property</span></span>|<span data-ttu-id="f9ef6-133">类型</span><span class="sxs-lookup"><span data-stu-id="f9ef6-133">Type</span></span>|<span data-ttu-id="f9ef6-134">说明</span><span class="sxs-lookup"><span data-stu-id="f9ef6-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9ef6-135">skip</span><span class="sxs-lookup"><span data-stu-id="f9ef6-135">skip</span></span>|<span data-ttu-id="f9ef6-136">Int32</span><span class="sxs-lookup"><span data-stu-id="f9ef6-136">Int32</span></span>|<span data-ttu-id="f9ef6-137">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f9ef6-137">Not yet documented</span></span>|
|<span data-ttu-id="f9ef6-138">top</span><span class="sxs-lookup"><span data-stu-id="f9ef6-138">top</span></span>|<span data-ttu-id="f9ef6-139">Int32</span><span class="sxs-lookup"><span data-stu-id="f9ef6-139">Int32</span></span>|<span data-ttu-id="f9ef6-140">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f9ef6-140">Not yet documented</span></span>|
|<span data-ttu-id="f9ef6-141">filter</span><span class="sxs-lookup"><span data-stu-id="f9ef6-141">filter</span></span>|<span data-ttu-id="f9ef6-142">String</span><span class="sxs-lookup"><span data-stu-id="f9ef6-142">String</span></span>|<span data-ttu-id="f9ef6-143">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f9ef6-143">Not yet documented</span></span>|
|<span data-ttu-id="f9ef6-144">skipToken</span><span class="sxs-lookup"><span data-stu-id="f9ef6-144">skipToken</span></span>|<span data-ttu-id="f9ef6-145">String</span><span class="sxs-lookup"><span data-stu-id="f9ef6-145">String</span></span>|<span data-ttu-id="f9ef6-146">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f9ef6-146">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="f9ef6-147">响应</span><span class="sxs-lookup"><span data-stu-id="f9ef6-147">Response</span></span>
<span data-ttu-id="f9ef6-148">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 [report](../resources/intune-shared-report.md)。</span><span class="sxs-lookup"><span data-stu-id="f9ef6-148">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9ef6-149">示例</span><span class="sxs-lookup"><span data-stu-id="f9ef6-149">Example</span></span>
### <a name="request"></a><span data-ttu-id="f9ef6-150">请求</span><span class="sxs-lookup"><span data-stu-id="f9ef6-150">Request</span></span>
<span data-ttu-id="f9ef6-151">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f9ef6-151">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentAbandonmentSummary(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="f9ef6-152">响应</span><span class="sxs-lookup"><span data-stu-id="f9ef6-152">Response</span></span>
<span data-ttu-id="f9ef6-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f9ef6-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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











