---
title: managedDeviceEnrollmentAbandonmentDetails 函数
description: 注册放弃的元数据的详细信息报表
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 30312706926293e24226801a7e0193b28d3d6f9c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29393212"
---
# <a name="manageddeviceenrollmentabandonmentdetails-function"></a><span data-ttu-id="a512c-103">managedDeviceEnrollmentAbandonmentDetails 函数</span><span class="sxs-lookup"><span data-stu-id="a512c-103">managedDeviceEnrollmentAbandonmentDetails function</span></span>

> <span data-ttu-id="a512c-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="a512c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a512c-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a512c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a512c-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a512c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a512c-107">注册放弃的元数据的详细信息报表</span><span class="sxs-lookup"><span data-stu-id="a512c-107">Metadata for Enrollment abandonment details report</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a512c-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="a512c-108">Prerequisites</span></span>
<span data-ttu-id="a512c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a512c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a512c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a512c-111">Permission type</span></span>|<span data-ttu-id="a512c-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a512c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a512c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a512c-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="a512c-114">&nbsp;&nbsp; **故障诊断**</span><span class="sxs-lookup"><span data-stu-id="a512c-114">&nbsp; &nbsp; **Troublshooting**</span></span> | <span data-ttu-id="a512c-115">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="a512c-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="a512c-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a512c-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a512c-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="a512c-117">Not supported.</span></span>|
|<span data-ttu-id="a512c-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="a512c-118">Application</span></span>|<span data-ttu-id="a512c-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="a512c-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a512c-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a512c-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentAbandonmentDetails
```

## <a name="request-headers"></a><span data-ttu-id="a512c-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="a512c-121">Request headers</span></span>
|<span data-ttu-id="a512c-122">标头</span><span class="sxs-lookup"><span data-stu-id="a512c-122">Header</span></span>|<span data-ttu-id="a512c-123">值</span><span class="sxs-lookup"><span data-stu-id="a512c-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a512c-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a512c-124">Authorization</span></span>|<span data-ttu-id="a512c-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a512c-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a512c-126">Accept</span><span class="sxs-lookup"><span data-stu-id="a512c-126">Accept</span></span>|<span data-ttu-id="a512c-127">application/json</span><span class="sxs-lookup"><span data-stu-id="a512c-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a512c-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="a512c-128">Request body</span></span>
<span data-ttu-id="a512c-129">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="a512c-129">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="a512c-130">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="a512c-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="a512c-131">属性</span><span class="sxs-lookup"><span data-stu-id="a512c-131">Property</span></span>|<span data-ttu-id="a512c-132">类型</span><span class="sxs-lookup"><span data-stu-id="a512c-132">Type</span></span>|<span data-ttu-id="a512c-133">说明</span><span class="sxs-lookup"><span data-stu-id="a512c-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a512c-134">skip</span><span class="sxs-lookup"><span data-stu-id="a512c-134">skip</span></span>|<span data-ttu-id="a512c-135">Int32</span><span class="sxs-lookup"><span data-stu-id="a512c-135">Int32</span></span>|<span data-ttu-id="a512c-136">尚未记录</span><span class="sxs-lookup"><span data-stu-id="a512c-136">Not yet documented</span></span>|
|<span data-ttu-id="a512c-137">top</span><span class="sxs-lookup"><span data-stu-id="a512c-137">top</span></span>|<span data-ttu-id="a512c-138">Int32</span><span class="sxs-lookup"><span data-stu-id="a512c-138">Int32</span></span>|<span data-ttu-id="a512c-139">尚未记录</span><span class="sxs-lookup"><span data-stu-id="a512c-139">Not yet documented</span></span>|
|<span data-ttu-id="a512c-140">filter</span><span class="sxs-lookup"><span data-stu-id="a512c-140">filter</span></span>|<span data-ttu-id="a512c-141">String</span><span class="sxs-lookup"><span data-stu-id="a512c-141">String</span></span>|<span data-ttu-id="a512c-142">尚未记录</span><span class="sxs-lookup"><span data-stu-id="a512c-142">Not yet documented</span></span>|
|<span data-ttu-id="a512c-143">skipToken</span><span class="sxs-lookup"><span data-stu-id="a512c-143">skipToken</span></span>|<span data-ttu-id="a512c-144">String</span><span class="sxs-lookup"><span data-stu-id="a512c-144">String</span></span>|<span data-ttu-id="a512c-145">尚未记录</span><span class="sxs-lookup"><span data-stu-id="a512c-145">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="a512c-146">响应</span><span class="sxs-lookup"><span data-stu-id="a512c-146">Response</span></span>
<span data-ttu-id="a512c-147">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 [report](../resources/intune-shared-report.md)。</span><span class="sxs-lookup"><span data-stu-id="a512c-147">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a512c-148">示例</span><span class="sxs-lookup"><span data-stu-id="a512c-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="a512c-149">请求</span><span class="sxs-lookup"><span data-stu-id="a512c-149">Request</span></span>
<span data-ttu-id="a512c-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a512c-150">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentAbandonmentDetails(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="a512c-151">响应</span><span class="sxs-lookup"><span data-stu-id="a512c-151">Response</span></span>
<span data-ttu-id="a512c-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a512c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





