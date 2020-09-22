---
title: managedDeviceEnrollmentFailureDetails 函数
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2d1e81b68d895dfb4edbe80a6d46fa59907d4489
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48053777"
---
# <a name="manageddeviceenrollmentfailuredetails-function"></a><span data-ttu-id="d4118-103">managedDeviceEnrollmentFailureDetails 函数</span><span class="sxs-lookup"><span data-stu-id="d4118-103">managedDeviceEnrollmentFailureDetails function</span></span>

<span data-ttu-id="d4118-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4118-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d4118-105">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d4118-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d4118-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d4118-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d4118-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d4118-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d4118-108">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d4118-108">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d4118-109">先决条件</span><span class="sxs-lookup"><span data-stu-id="d4118-109">Prerequisites</span></span>
<span data-ttu-id="d4118-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d4118-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4118-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="d4118-112">Permission type</span></span>|<span data-ttu-id="d4118-113">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d4118-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d4118-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d4118-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="d4118-115">&nbsp; &nbsp; **故障排除**</span><span class="sxs-lookup"><span data-stu-id="d4118-115">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="d4118-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4118-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="d4118-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d4118-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d4118-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="d4118-118">Not supported.</span></span>|
|<span data-ttu-id="d4118-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="d4118-119">Application</span></span>||
| <span data-ttu-id="d4118-120">&nbsp; &nbsp; **故障排除**</span><span class="sxs-lookup"><span data-stu-id="d4118-120">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="d4118-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4118-121">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d4118-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d4118-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentFailureDetails
```

## <a name="request-headers"></a><span data-ttu-id="d4118-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="d4118-123">Request headers</span></span>
|<span data-ttu-id="d4118-124">标头</span><span class="sxs-lookup"><span data-stu-id="d4118-124">Header</span></span>|<span data-ttu-id="d4118-125">值</span><span class="sxs-lookup"><span data-stu-id="d4118-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d4118-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="d4118-126">Authorization</span></span>|<span data-ttu-id="d4118-127">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d4118-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d4118-128">接受</span><span class="sxs-lookup"><span data-stu-id="d4118-128">Accept</span></span>|<span data-ttu-id="d4118-129">application/json</span><span class="sxs-lookup"><span data-stu-id="d4118-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4118-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="d4118-130">Request body</span></span>
<span data-ttu-id="d4118-131">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="d4118-131">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="d4118-132">属性</span><span class="sxs-lookup"><span data-stu-id="d4118-132">Property</span></span>|<span data-ttu-id="d4118-133">类型</span><span class="sxs-lookup"><span data-stu-id="d4118-133">Type</span></span>|<span data-ttu-id="d4118-134">说明</span><span class="sxs-lookup"><span data-stu-id="d4118-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4118-135">筛选器</span><span class="sxs-lookup"><span data-stu-id="d4118-135">filter</span></span>|<span data-ttu-id="d4118-136">String</span><span class="sxs-lookup"><span data-stu-id="d4118-136">String</span></span>|<span data-ttu-id="d4118-137">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d4118-137">Not yet documented</span></span>|
|<span data-ttu-id="d4118-138">skipToken</span><span class="sxs-lookup"><span data-stu-id="d4118-138">skipToken</span></span>|<span data-ttu-id="d4118-139">String</span><span class="sxs-lookup"><span data-stu-id="d4118-139">String</span></span>|<span data-ttu-id="d4118-140">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d4118-140">Not yet documented</span></span>|
|<span data-ttu-id="d4118-141">skip</span><span class="sxs-lookup"><span data-stu-id="d4118-141">skip</span></span>|<span data-ttu-id="d4118-142">Int32</span><span class="sxs-lookup"><span data-stu-id="d4118-142">Int32</span></span>|<span data-ttu-id="d4118-143">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d4118-143">Not yet documented</span></span>|
|<span data-ttu-id="d4118-144">top</span><span class="sxs-lookup"><span data-stu-id="d4118-144">top</span></span>|<span data-ttu-id="d4118-145">Int32</span><span class="sxs-lookup"><span data-stu-id="d4118-145">Int32</span></span>|<span data-ttu-id="d4118-146">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d4118-146">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="d4118-147">响应</span><span class="sxs-lookup"><span data-stu-id="d4118-147">Response</span></span>
<span data-ttu-id="d4118-148">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 [report](../resources/intune-shared-report.md)。</span><span class="sxs-lookup"><span data-stu-id="d4118-148">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4118-149">示例</span><span class="sxs-lookup"><span data-stu-id="d4118-149">Example</span></span>
### <a name="request"></a><span data-ttu-id="d4118-150">请求</span><span class="sxs-lookup"><span data-stu-id="d4118-150">Request</span></span>
<span data-ttu-id="d4118-151">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d4118-151">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentFailureDetails(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="d4118-152">响应</span><span class="sxs-lookup"><span data-stu-id="d4118-152">Response</span></span>
<span data-ttu-id="d4118-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d4118-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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












