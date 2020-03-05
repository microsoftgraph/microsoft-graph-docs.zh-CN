---
title: managedDeviceEnrollmentAbandonmentSummary 函数
description: 注册 abandonment 摘要报告的元数据
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e0ac224ec30110abd39675c1fcb8c64e3087185a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42458166"
---
# <a name="manageddeviceenrollmentabandonmentsummary-function"></a><span data-ttu-id="bf74f-103">managedDeviceEnrollmentAbandonmentSummary 函数</span><span class="sxs-lookup"><span data-stu-id="bf74f-103">managedDeviceEnrollmentAbandonmentSummary function</span></span>

<span data-ttu-id="bf74f-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="bf74f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bf74f-105">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="bf74f-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bf74f-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="bf74f-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bf74f-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bf74f-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bf74f-108">注册 abandonment 摘要报告的元数据</span><span class="sxs-lookup"><span data-stu-id="bf74f-108">Metadata for Enrollment abandonment summary report</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bf74f-109">先决条件</span><span class="sxs-lookup"><span data-stu-id="bf74f-109">Prerequisites</span></span>
<span data-ttu-id="bf74f-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bf74f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bf74f-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="bf74f-112">Permission type</span></span>|<span data-ttu-id="bf74f-113">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="bf74f-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bf74f-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bf74f-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="bf74f-115">&nbsp;&nbsp; **Troublshooting**</span><span class="sxs-lookup"><span data-stu-id="bf74f-115">&nbsp; &nbsp; **Troublshooting**</span></span> | <span data-ttu-id="bf74f-116">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="bf74f-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="bf74f-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bf74f-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bf74f-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="bf74f-118">Not supported.</span></span>|
|<span data-ttu-id="bf74f-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="bf74f-119">Application</span></span>||
| <span data-ttu-id="bf74f-120">&nbsp;&nbsp; **Troublshooting**</span><span class="sxs-lookup"><span data-stu-id="bf74f-120">&nbsp; &nbsp; **Troublshooting**</span></span> | <span data-ttu-id="bf74f-121">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="bf74f-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bf74f-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bf74f-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentAbandonmentSummary
```

## <a name="request-headers"></a><span data-ttu-id="bf74f-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="bf74f-123">Request headers</span></span>
|<span data-ttu-id="bf74f-124">标头</span><span class="sxs-lookup"><span data-stu-id="bf74f-124">Header</span></span>|<span data-ttu-id="bf74f-125">值</span><span class="sxs-lookup"><span data-stu-id="bf74f-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bf74f-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="bf74f-126">Authorization</span></span>|<span data-ttu-id="bf74f-127">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="bf74f-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bf74f-128">接受</span><span class="sxs-lookup"><span data-stu-id="bf74f-128">Accept</span></span>|<span data-ttu-id="bf74f-129">application/json</span><span class="sxs-lookup"><span data-stu-id="bf74f-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bf74f-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="bf74f-130">Request body</span></span>
<span data-ttu-id="bf74f-131">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="bf74f-131">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="bf74f-132">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="bf74f-132">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="bf74f-133">属性</span><span class="sxs-lookup"><span data-stu-id="bf74f-133">Property</span></span>|<span data-ttu-id="bf74f-134">类型</span><span class="sxs-lookup"><span data-stu-id="bf74f-134">Type</span></span>|<span data-ttu-id="bf74f-135">说明</span><span class="sxs-lookup"><span data-stu-id="bf74f-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf74f-136">skip</span><span class="sxs-lookup"><span data-stu-id="bf74f-136">skip</span></span>|<span data-ttu-id="bf74f-137">Int32</span><span class="sxs-lookup"><span data-stu-id="bf74f-137">Int32</span></span>|<span data-ttu-id="bf74f-138">尚未记录</span><span class="sxs-lookup"><span data-stu-id="bf74f-138">Not yet documented</span></span>|
|<span data-ttu-id="bf74f-139">top</span><span class="sxs-lookup"><span data-stu-id="bf74f-139">top</span></span>|<span data-ttu-id="bf74f-140">Int32</span><span class="sxs-lookup"><span data-stu-id="bf74f-140">Int32</span></span>|<span data-ttu-id="bf74f-141">尚未记录</span><span class="sxs-lookup"><span data-stu-id="bf74f-141">Not yet documented</span></span>|
|<span data-ttu-id="bf74f-142">filter</span><span class="sxs-lookup"><span data-stu-id="bf74f-142">filter</span></span>|<span data-ttu-id="bf74f-143">String</span><span class="sxs-lookup"><span data-stu-id="bf74f-143">String</span></span>|<span data-ttu-id="bf74f-144">尚未记录</span><span class="sxs-lookup"><span data-stu-id="bf74f-144">Not yet documented</span></span>|
|<span data-ttu-id="bf74f-145">skipToken</span><span class="sxs-lookup"><span data-stu-id="bf74f-145">skipToken</span></span>|<span data-ttu-id="bf74f-146">String</span><span class="sxs-lookup"><span data-stu-id="bf74f-146">String</span></span>|<span data-ttu-id="bf74f-147">尚未记录</span><span class="sxs-lookup"><span data-stu-id="bf74f-147">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="bf74f-148">响应</span><span class="sxs-lookup"><span data-stu-id="bf74f-148">Response</span></span>
<span data-ttu-id="bf74f-149">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 [report](../resources/intune-shared-report.md)。</span><span class="sxs-lookup"><span data-stu-id="bf74f-149">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bf74f-150">示例</span><span class="sxs-lookup"><span data-stu-id="bf74f-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="bf74f-151">请求</span><span class="sxs-lookup"><span data-stu-id="bf74f-151">Request</span></span>
<span data-ttu-id="bf74f-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bf74f-152">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentAbandonmentSummary(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="bf74f-153">响应</span><span class="sxs-lookup"><span data-stu-id="bf74f-153">Response</span></span>
<span data-ttu-id="bf74f-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bf74f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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













