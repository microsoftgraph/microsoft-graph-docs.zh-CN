---
title: managedDeviceEnrollmentAbandonmentDetails 函数
description: 注册 abandonment 详细信息报告的元数据
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ff7d7e09d385773f98ef9c759c0f092e3abb00f5
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37195837"
---
# <a name="manageddeviceenrollmentabandonmentdetails-function"></a><span data-ttu-id="4eede-103">managedDeviceEnrollmentAbandonmentDetails 函数</span><span class="sxs-lookup"><span data-stu-id="4eede-103">managedDeviceEnrollmentAbandonmentDetails function</span></span>

> <span data-ttu-id="4eede-104">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="4eede-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4eede-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="4eede-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4eede-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4eede-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4eede-107">注册 abandonment 详细信息报告的元数据</span><span class="sxs-lookup"><span data-stu-id="4eede-107">Metadata for Enrollment abandonment details report</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4eede-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="4eede-108">Prerequisites</span></span>
<span data-ttu-id="4eede-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4eede-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4eede-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="4eede-111">Permission type</span></span>|<span data-ttu-id="4eede-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4eede-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4eede-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4eede-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="4eede-114">&nbsp;&nbsp; **Troublshooting**</span><span class="sxs-lookup"><span data-stu-id="4eede-114">&nbsp; &nbsp; **Troublshooting**</span></span> | <span data-ttu-id="4eede-115">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="4eede-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="4eede-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4eede-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4eede-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="4eede-117">Not supported.</span></span>|
|<span data-ttu-id="4eede-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="4eede-118">Application</span></span>||
| <span data-ttu-id="4eede-119">&nbsp;&nbsp; **Troublshooting**</span><span class="sxs-lookup"><span data-stu-id="4eede-119">&nbsp; &nbsp; **Troublshooting**</span></span> | <span data-ttu-id="4eede-120">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="4eede-120">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4eede-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4eede-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentAbandonmentDetails
```

## <a name="request-headers"></a><span data-ttu-id="4eede-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="4eede-122">Request headers</span></span>
|<span data-ttu-id="4eede-123">标头</span><span class="sxs-lookup"><span data-stu-id="4eede-123">Header</span></span>|<span data-ttu-id="4eede-124">值</span><span class="sxs-lookup"><span data-stu-id="4eede-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4eede-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="4eede-125">Authorization</span></span>|<span data-ttu-id="4eede-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4eede-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4eede-127">接受</span><span class="sxs-lookup"><span data-stu-id="4eede-127">Accept</span></span>|<span data-ttu-id="4eede-128">application/json</span><span class="sxs-lookup"><span data-stu-id="4eede-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4eede-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="4eede-129">Request body</span></span>
<span data-ttu-id="4eede-130">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="4eede-130">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="4eede-131">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="4eede-131">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="4eede-132">属性</span><span class="sxs-lookup"><span data-stu-id="4eede-132">Property</span></span>|<span data-ttu-id="4eede-133">类型</span><span class="sxs-lookup"><span data-stu-id="4eede-133">Type</span></span>|<span data-ttu-id="4eede-134">说明</span><span class="sxs-lookup"><span data-stu-id="4eede-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4eede-135">skip</span><span class="sxs-lookup"><span data-stu-id="4eede-135">skip</span></span>|<span data-ttu-id="4eede-136">Int32</span><span class="sxs-lookup"><span data-stu-id="4eede-136">Int32</span></span>|<span data-ttu-id="4eede-137">尚未记录</span><span class="sxs-lookup"><span data-stu-id="4eede-137">Not yet documented</span></span>|
|<span data-ttu-id="4eede-138">top</span><span class="sxs-lookup"><span data-stu-id="4eede-138">top</span></span>|<span data-ttu-id="4eede-139">Int32</span><span class="sxs-lookup"><span data-stu-id="4eede-139">Int32</span></span>|<span data-ttu-id="4eede-140">尚未记录</span><span class="sxs-lookup"><span data-stu-id="4eede-140">Not yet documented</span></span>|
|<span data-ttu-id="4eede-141">filter</span><span class="sxs-lookup"><span data-stu-id="4eede-141">filter</span></span>|<span data-ttu-id="4eede-142">String</span><span class="sxs-lookup"><span data-stu-id="4eede-142">String</span></span>|<span data-ttu-id="4eede-143">尚未记录</span><span class="sxs-lookup"><span data-stu-id="4eede-143">Not yet documented</span></span>|
|<span data-ttu-id="4eede-144">skipToken</span><span class="sxs-lookup"><span data-stu-id="4eede-144">skipToken</span></span>|<span data-ttu-id="4eede-145">String</span><span class="sxs-lookup"><span data-stu-id="4eede-145">String</span></span>|<span data-ttu-id="4eede-146">尚未记录</span><span class="sxs-lookup"><span data-stu-id="4eede-146">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="4eede-147">响应</span><span class="sxs-lookup"><span data-stu-id="4eede-147">Response</span></span>
<span data-ttu-id="4eede-148">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 [report](../resources/intune-shared-report.md)。</span><span class="sxs-lookup"><span data-stu-id="4eede-148">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4eede-149">示例</span><span class="sxs-lookup"><span data-stu-id="4eede-149">Example</span></span>
### <a name="request"></a><span data-ttu-id="4eede-150">请求</span><span class="sxs-lookup"><span data-stu-id="4eede-150">Request</span></span>
<span data-ttu-id="4eede-151">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4eede-151">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentAbandonmentDetails(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="4eede-152">响应</span><span class="sxs-lookup"><span data-stu-id="4eede-152">Response</span></span>
<span data-ttu-id="4eede-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4eede-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









