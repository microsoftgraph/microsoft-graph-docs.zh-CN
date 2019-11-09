---
title: managedDeviceEnrollmentAbandonmentDetails 函数
description: 注册 abandonment 详细信息报告的元数据
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 212d55672ab9bcf9ce3bd54e344eb5e9fe612aff
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/09/2019
ms.locfileid: "38085694"
---
# <a name="manageddeviceenrollmentabandonmentdetails-function"></a><span data-ttu-id="b57e2-103">managedDeviceEnrollmentAbandonmentDetails 函数</span><span class="sxs-lookup"><span data-stu-id="b57e2-103">managedDeviceEnrollmentAbandonmentDetails function</span></span>

> <span data-ttu-id="b57e2-104">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b57e2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b57e2-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b57e2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b57e2-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b57e2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b57e2-107">注册 abandonment 详细信息报告的元数据</span><span class="sxs-lookup"><span data-stu-id="b57e2-107">Metadata for Enrollment abandonment details report</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b57e2-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b57e2-108">Prerequisites</span></span>
<span data-ttu-id="b57e2-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b57e2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b57e2-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b57e2-111">Permission type</span></span>|<span data-ttu-id="b57e2-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b57e2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b57e2-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b57e2-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="b57e2-114">&nbsp;&nbsp; **Troublshooting**</span><span class="sxs-lookup"><span data-stu-id="b57e2-114">&nbsp; &nbsp; **Troublshooting**</span></span> | <span data-ttu-id="b57e2-115">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="b57e2-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="b57e2-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b57e2-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b57e2-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="b57e2-117">Not supported.</span></span>|
|<span data-ttu-id="b57e2-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="b57e2-118">Application</span></span>||
| <span data-ttu-id="b57e2-119">&nbsp;&nbsp; **Troublshooting**</span><span class="sxs-lookup"><span data-stu-id="b57e2-119">&nbsp; &nbsp; **Troublshooting**</span></span> | <span data-ttu-id="b57e2-120">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="b57e2-120">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b57e2-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b57e2-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentAbandonmentDetails
```

## <a name="request-headers"></a><span data-ttu-id="b57e2-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="b57e2-122">Request headers</span></span>
|<span data-ttu-id="b57e2-123">标头</span><span class="sxs-lookup"><span data-stu-id="b57e2-123">Header</span></span>|<span data-ttu-id="b57e2-124">值</span><span class="sxs-lookup"><span data-stu-id="b57e2-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b57e2-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="b57e2-125">Authorization</span></span>|<span data-ttu-id="b57e2-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b57e2-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b57e2-127">接受</span><span class="sxs-lookup"><span data-stu-id="b57e2-127">Accept</span></span>|<span data-ttu-id="b57e2-128">application/json</span><span class="sxs-lookup"><span data-stu-id="b57e2-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b57e2-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="b57e2-129">Request body</span></span>
<span data-ttu-id="b57e2-130">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="b57e2-130">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="b57e2-131">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="b57e2-131">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="b57e2-132">属性</span><span class="sxs-lookup"><span data-stu-id="b57e2-132">Property</span></span>|<span data-ttu-id="b57e2-133">类型</span><span class="sxs-lookup"><span data-stu-id="b57e2-133">Type</span></span>|<span data-ttu-id="b57e2-134">描述</span><span class="sxs-lookup"><span data-stu-id="b57e2-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b57e2-135">skip</span><span class="sxs-lookup"><span data-stu-id="b57e2-135">skip</span></span>|<span data-ttu-id="b57e2-136">Int32</span><span class="sxs-lookup"><span data-stu-id="b57e2-136">Int32</span></span>|<span data-ttu-id="b57e2-137">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b57e2-137">Not yet documented</span></span>|
|<span data-ttu-id="b57e2-138">top</span><span class="sxs-lookup"><span data-stu-id="b57e2-138">top</span></span>|<span data-ttu-id="b57e2-139">Int32</span><span class="sxs-lookup"><span data-stu-id="b57e2-139">Int32</span></span>|<span data-ttu-id="b57e2-140">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b57e2-140">Not yet documented</span></span>|
|<span data-ttu-id="b57e2-141">filter</span><span class="sxs-lookup"><span data-stu-id="b57e2-141">filter</span></span>|<span data-ttu-id="b57e2-142">String</span><span class="sxs-lookup"><span data-stu-id="b57e2-142">String</span></span>|<span data-ttu-id="b57e2-143">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b57e2-143">Not yet documented</span></span>|
|<span data-ttu-id="b57e2-144">skipToken</span><span class="sxs-lookup"><span data-stu-id="b57e2-144">skipToken</span></span>|<span data-ttu-id="b57e2-145">String</span><span class="sxs-lookup"><span data-stu-id="b57e2-145">String</span></span>|<span data-ttu-id="b57e2-146">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b57e2-146">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="b57e2-147">响应</span><span class="sxs-lookup"><span data-stu-id="b57e2-147">Response</span></span>
<span data-ttu-id="b57e2-148">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 [report](../resources/intune-shared-report.md)。</span><span class="sxs-lookup"><span data-stu-id="b57e2-148">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b57e2-149">示例</span><span class="sxs-lookup"><span data-stu-id="b57e2-149">Example</span></span>
### <a name="request"></a><span data-ttu-id="b57e2-150">请求</span><span class="sxs-lookup"><span data-stu-id="b57e2-150">Request</span></span>
<span data-ttu-id="b57e2-151">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b57e2-151">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentAbandonmentDetails(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="b57e2-152">响应</span><span class="sxs-lookup"><span data-stu-id="b57e2-152">Response</span></span>
<span data-ttu-id="b57e2-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b57e2-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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














