---
title: managedDeviceEnrollmentAbandonmentDetails 函数
description: 注册 abandonment 详细信息报告的元数据
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ba02e4f87d62eb2519e24cce19e6ee0750d86125
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48053788"
---
# <a name="manageddeviceenrollmentabandonmentdetails-function"></a><span data-ttu-id="b1b29-103">managedDeviceEnrollmentAbandonmentDetails 函数</span><span class="sxs-lookup"><span data-stu-id="b1b29-103">managedDeviceEnrollmentAbandonmentDetails function</span></span>

<span data-ttu-id="b1b29-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1b29-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b1b29-105">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b1b29-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b1b29-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b1b29-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b1b29-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b1b29-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1b29-108">注册 abandonment 详细信息报告的元数据</span><span class="sxs-lookup"><span data-stu-id="b1b29-108">Metadata for Enrollment abandonment details report</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b1b29-109">先决条件</span><span class="sxs-lookup"><span data-stu-id="b1b29-109">Prerequisites</span></span>
<span data-ttu-id="b1b29-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b1b29-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1b29-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="b1b29-112">Permission type</span></span>|<span data-ttu-id="b1b29-113">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b1b29-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b1b29-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b1b29-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="b1b29-115">&nbsp;&nbsp; **Troublshooting**</span><span class="sxs-lookup"><span data-stu-id="b1b29-115">&nbsp; &nbsp; **Troublshooting**</span></span> | <span data-ttu-id="b1b29-116">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="b1b29-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="b1b29-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b1b29-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b1b29-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="b1b29-118">Not supported.</span></span>|
|<span data-ttu-id="b1b29-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="b1b29-119">Application</span></span>||
| <span data-ttu-id="b1b29-120">&nbsp;&nbsp; **Troublshooting**</span><span class="sxs-lookup"><span data-stu-id="b1b29-120">&nbsp; &nbsp; **Troublshooting**</span></span> | <span data-ttu-id="b1b29-121">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="b1b29-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b1b29-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b1b29-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentAbandonmentDetails
```

## <a name="request-headers"></a><span data-ttu-id="b1b29-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="b1b29-123">Request headers</span></span>
|<span data-ttu-id="b1b29-124">标头</span><span class="sxs-lookup"><span data-stu-id="b1b29-124">Header</span></span>|<span data-ttu-id="b1b29-125">值</span><span class="sxs-lookup"><span data-stu-id="b1b29-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b1b29-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="b1b29-126">Authorization</span></span>|<span data-ttu-id="b1b29-127">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b1b29-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b1b29-128">接受</span><span class="sxs-lookup"><span data-stu-id="b1b29-128">Accept</span></span>|<span data-ttu-id="b1b29-129">application/json</span><span class="sxs-lookup"><span data-stu-id="b1b29-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b1b29-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="b1b29-130">Request body</span></span>
<span data-ttu-id="b1b29-131">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="b1b29-131">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="b1b29-132">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="b1b29-132">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="b1b29-133">属性</span><span class="sxs-lookup"><span data-stu-id="b1b29-133">Property</span></span>|<span data-ttu-id="b1b29-134">类型</span><span class="sxs-lookup"><span data-stu-id="b1b29-134">Type</span></span>|<span data-ttu-id="b1b29-135">说明</span><span class="sxs-lookup"><span data-stu-id="b1b29-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1b29-136">skip</span><span class="sxs-lookup"><span data-stu-id="b1b29-136">skip</span></span>|<span data-ttu-id="b1b29-137">Int32</span><span class="sxs-lookup"><span data-stu-id="b1b29-137">Int32</span></span>|<span data-ttu-id="b1b29-138">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b1b29-138">Not yet documented</span></span>|
|<span data-ttu-id="b1b29-139">top</span><span class="sxs-lookup"><span data-stu-id="b1b29-139">top</span></span>|<span data-ttu-id="b1b29-140">Int32</span><span class="sxs-lookup"><span data-stu-id="b1b29-140">Int32</span></span>|<span data-ttu-id="b1b29-141">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b1b29-141">Not yet documented</span></span>|
|<span data-ttu-id="b1b29-142">filter</span><span class="sxs-lookup"><span data-stu-id="b1b29-142">filter</span></span>|<span data-ttu-id="b1b29-143">String</span><span class="sxs-lookup"><span data-stu-id="b1b29-143">String</span></span>|<span data-ttu-id="b1b29-144">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b1b29-144">Not yet documented</span></span>|
|<span data-ttu-id="b1b29-145">skipToken</span><span class="sxs-lookup"><span data-stu-id="b1b29-145">skipToken</span></span>|<span data-ttu-id="b1b29-146">String</span><span class="sxs-lookup"><span data-stu-id="b1b29-146">String</span></span>|<span data-ttu-id="b1b29-147">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b1b29-147">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="b1b29-148">响应</span><span class="sxs-lookup"><span data-stu-id="b1b29-148">Response</span></span>
<span data-ttu-id="b1b29-149">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 [report](../resources/intune-shared-report.md)。</span><span class="sxs-lookup"><span data-stu-id="b1b29-149">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1b29-150">示例</span><span class="sxs-lookup"><span data-stu-id="b1b29-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="b1b29-151">请求</span><span class="sxs-lookup"><span data-stu-id="b1b29-151">Request</span></span>
<span data-ttu-id="b1b29-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b1b29-152">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentAbandonmentDetails(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="b1b29-153">响应</span><span class="sxs-lookup"><span data-stu-id="b1b29-153">Response</span></span>
<span data-ttu-id="b1b29-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b1b29-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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














