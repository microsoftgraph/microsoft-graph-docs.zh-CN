---
title: managedDeviceEnrollmentAbandonmentDetails 函数
description: 注册放弃的元数据的详细信息报表
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8e2031657c3aff7d09d126b6eff01beaf34813a0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27939908"
---
# <a name="manageddeviceenrollmentabandonmentdetails-function"></a><span data-ttu-id="e7f9c-103">managedDeviceEnrollmentAbandonmentDetails 函数</span><span class="sxs-lookup"><span data-stu-id="e7f9c-103">managedDeviceEnrollmentAbandonmentDetails function</span></span>

> <span data-ttu-id="e7f9c-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e7f9c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e7f9c-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e7f9c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e7f9c-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e7f9c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e7f9c-107">注册放弃的元数据的详细信息报表</span><span class="sxs-lookup"><span data-stu-id="e7f9c-107">Metadata for Enrollment abandonment details report</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e7f9c-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="e7f9c-108">Prerequisites</span></span>
<span data-ttu-id="e7f9c-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="e7f9c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7f9c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e7f9c-111">Permission type</span></span>|<span data-ttu-id="e7f9c-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e7f9c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e7f9c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e7f9c-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="e7f9c-114">&nbsp;&nbsp; **故障诊断**</span><span class="sxs-lookup"><span data-stu-id="e7f9c-114">&nbsp; &nbsp; **Troublshooting**</span></span> | <span data-ttu-id="e7f9c-115">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="e7f9c-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="e7f9c-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e7f9c-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e7f9c-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="e7f9c-117">Not supported.</span></span>|
|<span data-ttu-id="e7f9c-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="e7f9c-118">Application</span></span>|<span data-ttu-id="e7f9c-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="e7f9c-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e7f9c-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e7f9c-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentAbandonmentDetails
```

## <a name="request-headers"></a><span data-ttu-id="e7f9c-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="e7f9c-121">Request headers</span></span>
|<span data-ttu-id="e7f9c-122">标头</span><span class="sxs-lookup"><span data-stu-id="e7f9c-122">Header</span></span>|<span data-ttu-id="e7f9c-123">值</span><span class="sxs-lookup"><span data-stu-id="e7f9c-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e7f9c-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e7f9c-124">Authorization</span></span>|<span data-ttu-id="e7f9c-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e7f9c-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e7f9c-126">Accept</span><span class="sxs-lookup"><span data-stu-id="e7f9c-126">Accept</span></span>|<span data-ttu-id="e7f9c-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e7f9c-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7f9c-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="e7f9c-128">Request body</span></span>
<span data-ttu-id="e7f9c-129">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="e7f9c-129">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="e7f9c-130">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="e7f9c-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="e7f9c-131">属性</span><span class="sxs-lookup"><span data-stu-id="e7f9c-131">Property</span></span>|<span data-ttu-id="e7f9c-132">类型</span><span class="sxs-lookup"><span data-stu-id="e7f9c-132">Type</span></span>|<span data-ttu-id="e7f9c-133">说明</span><span class="sxs-lookup"><span data-stu-id="e7f9c-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7f9c-134">skip</span><span class="sxs-lookup"><span data-stu-id="e7f9c-134">skip</span></span>|<span data-ttu-id="e7f9c-135">Int32</span><span class="sxs-lookup"><span data-stu-id="e7f9c-135">Int32</span></span>|<span data-ttu-id="e7f9c-136">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e7f9c-136">Not yet documented</span></span>|
|<span data-ttu-id="e7f9c-137">top</span><span class="sxs-lookup"><span data-stu-id="e7f9c-137">top</span></span>|<span data-ttu-id="e7f9c-138">Int32</span><span class="sxs-lookup"><span data-stu-id="e7f9c-138">Int32</span></span>|<span data-ttu-id="e7f9c-139">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e7f9c-139">Not yet documented</span></span>|
|<span data-ttu-id="e7f9c-140">filter</span><span class="sxs-lookup"><span data-stu-id="e7f9c-140">filter</span></span>|<span data-ttu-id="e7f9c-141">字符串</span><span class="sxs-lookup"><span data-stu-id="e7f9c-141">String</span></span>|<span data-ttu-id="e7f9c-142">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e7f9c-142">Not yet documented</span></span>|
|<span data-ttu-id="e7f9c-143">skipToken</span><span class="sxs-lookup"><span data-stu-id="e7f9c-143">skipToken</span></span>|<span data-ttu-id="e7f9c-144">字符串</span><span class="sxs-lookup"><span data-stu-id="e7f9c-144">String</span></span>|<span data-ttu-id="e7f9c-145">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e7f9c-145">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="e7f9c-146">响应</span><span class="sxs-lookup"><span data-stu-id="e7f9c-146">Response</span></span>
<span data-ttu-id="e7f9c-147">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 [report](../resources/intune-shared-report.md)。</span><span class="sxs-lookup"><span data-stu-id="e7f9c-147">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7f9c-148">示例</span><span class="sxs-lookup"><span data-stu-id="e7f9c-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="e7f9c-149">请求</span><span class="sxs-lookup"><span data-stu-id="e7f9c-149">Request</span></span>
<span data-ttu-id="e7f9c-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e7f9c-150">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentAbandonmentDetails(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="e7f9c-151">响应</span><span class="sxs-lookup"><span data-stu-id="e7f9c-151">Response</span></span>
<span data-ttu-id="e7f9c-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e7f9c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





