---
title: managedDeviceEnrollmentFailureDetails 函数
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d7aebdedba18baa75f72b25256af53831552493e
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48731475"
---
# <a name="manageddeviceenrollmentfailuredetails-function"></a><span data-ttu-id="116f7-103">managedDeviceEnrollmentFailureDetails 函数</span><span class="sxs-lookup"><span data-stu-id="116f7-103">managedDeviceEnrollmentFailureDetails function</span></span>

<span data-ttu-id="116f7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="116f7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="116f7-105">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="116f7-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="116f7-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="116f7-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="116f7-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="116f7-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="116f7-108">尚未记录</span><span class="sxs-lookup"><span data-stu-id="116f7-108">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="116f7-109">先决条件</span><span class="sxs-lookup"><span data-stu-id="116f7-109">Prerequisites</span></span>
<span data-ttu-id="116f7-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="116f7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="116f7-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="116f7-112">Permission type</span></span>|<span data-ttu-id="116f7-113">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="116f7-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="116f7-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="116f7-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="116f7-115">&nbsp; &nbsp; **故障排除**</span><span class="sxs-lookup"><span data-stu-id="116f7-115">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="116f7-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="116f7-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="116f7-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="116f7-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="116f7-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="116f7-118">Not supported.</span></span>|
|<span data-ttu-id="116f7-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="116f7-119">Application</span></span>||
| <span data-ttu-id="116f7-120">&nbsp; &nbsp; **故障排除**</span><span class="sxs-lookup"><span data-stu-id="116f7-120">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="116f7-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="116f7-121">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="116f7-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="116f7-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentFailureDetails
```

## <a name="request-headers"></a><span data-ttu-id="116f7-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="116f7-123">Request headers</span></span>
|<span data-ttu-id="116f7-124">标头</span><span class="sxs-lookup"><span data-stu-id="116f7-124">Header</span></span>|<span data-ttu-id="116f7-125">值</span><span class="sxs-lookup"><span data-stu-id="116f7-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="116f7-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="116f7-126">Authorization</span></span>|<span data-ttu-id="116f7-127">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="116f7-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="116f7-128">接受</span><span class="sxs-lookup"><span data-stu-id="116f7-128">Accept</span></span>|<span data-ttu-id="116f7-129">application/json</span><span class="sxs-lookup"><span data-stu-id="116f7-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="116f7-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="116f7-130">Request body</span></span>
<span data-ttu-id="116f7-131">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="116f7-131">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="116f7-132">属性</span><span class="sxs-lookup"><span data-stu-id="116f7-132">Property</span></span>|<span data-ttu-id="116f7-133">类型</span><span class="sxs-lookup"><span data-stu-id="116f7-133">Type</span></span>|<span data-ttu-id="116f7-134">说明</span><span class="sxs-lookup"><span data-stu-id="116f7-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="116f7-135">筛选器</span><span class="sxs-lookup"><span data-stu-id="116f7-135">filter</span></span>|<span data-ttu-id="116f7-136">String</span><span class="sxs-lookup"><span data-stu-id="116f7-136">String</span></span>|<span data-ttu-id="116f7-137">尚未记录</span><span class="sxs-lookup"><span data-stu-id="116f7-137">Not yet documented</span></span>|
|<span data-ttu-id="116f7-138">skipToken</span><span class="sxs-lookup"><span data-stu-id="116f7-138">skipToken</span></span>|<span data-ttu-id="116f7-139">String</span><span class="sxs-lookup"><span data-stu-id="116f7-139">String</span></span>|<span data-ttu-id="116f7-140">尚未记录</span><span class="sxs-lookup"><span data-stu-id="116f7-140">Not yet documented</span></span>|
|<span data-ttu-id="116f7-141">skip</span><span class="sxs-lookup"><span data-stu-id="116f7-141">skip</span></span>|<span data-ttu-id="116f7-142">Int32</span><span class="sxs-lookup"><span data-stu-id="116f7-142">Int32</span></span>|<span data-ttu-id="116f7-143">尚未记录</span><span class="sxs-lookup"><span data-stu-id="116f7-143">Not yet documented</span></span>|
|<span data-ttu-id="116f7-144">top</span><span class="sxs-lookup"><span data-stu-id="116f7-144">top</span></span>|<span data-ttu-id="116f7-145">Int32</span><span class="sxs-lookup"><span data-stu-id="116f7-145">Int32</span></span>|<span data-ttu-id="116f7-146">尚未记录</span><span class="sxs-lookup"><span data-stu-id="116f7-146">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="116f7-147">响应</span><span class="sxs-lookup"><span data-stu-id="116f7-147">Response</span></span>
<span data-ttu-id="116f7-148">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 [report](../resources/intune-shared-report.md)。</span><span class="sxs-lookup"><span data-stu-id="116f7-148">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="116f7-149">示例</span><span class="sxs-lookup"><span data-stu-id="116f7-149">Example</span></span>
### <a name="request"></a><span data-ttu-id="116f7-150">请求</span><span class="sxs-lookup"><span data-stu-id="116f7-150">Request</span></span>
<span data-ttu-id="116f7-151">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="116f7-151">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentFailureDetails(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="116f7-152">响应</span><span class="sxs-lookup"><span data-stu-id="116f7-152">Response</span></span>
<span data-ttu-id="116f7-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="116f7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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











