---
title: managedDeviceEnrollmentFailureDetails 函数
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5cd1eed26f4bc9b29b0c8a7187869f0fded61e35
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37195823"
---
# <a name="manageddeviceenrollmentfailuredetails-function"></a><span data-ttu-id="5bb73-103">managedDeviceEnrollmentFailureDetails 函数</span><span class="sxs-lookup"><span data-stu-id="5bb73-103">managedDeviceEnrollmentFailureDetails function</span></span>

> <span data-ttu-id="5bb73-104">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5bb73-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5bb73-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5bb73-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5bb73-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5bb73-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5bb73-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="5bb73-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5bb73-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="5bb73-108">Prerequisites</span></span>
<span data-ttu-id="5bb73-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5bb73-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5bb73-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="5bb73-111">Permission type</span></span>|<span data-ttu-id="5bb73-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5bb73-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5bb73-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5bb73-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="5bb73-114">&nbsp; &nbsp; **疑难解答**</span><span class="sxs-lookup"><span data-stu-id="5bb73-114">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="5bb73-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5bb73-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="5bb73-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5bb73-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5bb73-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="5bb73-117">Not supported.</span></span>|
|<span data-ttu-id="5bb73-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="5bb73-118">Application</span></span>||
| <span data-ttu-id="5bb73-119">&nbsp; &nbsp; **疑难解答**</span><span class="sxs-lookup"><span data-stu-id="5bb73-119">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="5bb73-120">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5bb73-120">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5bb73-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5bb73-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentFailureDetails
```

## <a name="request-headers"></a><span data-ttu-id="5bb73-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="5bb73-122">Request headers</span></span>
|<span data-ttu-id="5bb73-123">标头</span><span class="sxs-lookup"><span data-stu-id="5bb73-123">Header</span></span>|<span data-ttu-id="5bb73-124">值</span><span class="sxs-lookup"><span data-stu-id="5bb73-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5bb73-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="5bb73-125">Authorization</span></span>|<span data-ttu-id="5bb73-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5bb73-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5bb73-127">接受</span><span class="sxs-lookup"><span data-stu-id="5bb73-127">Accept</span></span>|<span data-ttu-id="5bb73-128">application/json</span><span class="sxs-lookup"><span data-stu-id="5bb73-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5bb73-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="5bb73-129">Request body</span></span>
<span data-ttu-id="5bb73-130">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="5bb73-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="5bb73-131">属性</span><span class="sxs-lookup"><span data-stu-id="5bb73-131">Property</span></span>|<span data-ttu-id="5bb73-132">类型</span><span class="sxs-lookup"><span data-stu-id="5bb73-132">Type</span></span>|<span data-ttu-id="5bb73-133">说明</span><span class="sxs-lookup"><span data-stu-id="5bb73-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5bb73-134">筛选器</span><span class="sxs-lookup"><span data-stu-id="5bb73-134">filter</span></span>|<span data-ttu-id="5bb73-135">String</span><span class="sxs-lookup"><span data-stu-id="5bb73-135">String</span></span>|<span data-ttu-id="5bb73-136">尚未记录</span><span class="sxs-lookup"><span data-stu-id="5bb73-136">Not yet documented</span></span>|
|<span data-ttu-id="5bb73-137">skipToken</span><span class="sxs-lookup"><span data-stu-id="5bb73-137">skipToken</span></span>|<span data-ttu-id="5bb73-138">String</span><span class="sxs-lookup"><span data-stu-id="5bb73-138">String</span></span>|<span data-ttu-id="5bb73-139">尚未记录</span><span class="sxs-lookup"><span data-stu-id="5bb73-139">Not yet documented</span></span>|
|<span data-ttu-id="5bb73-140">skip</span><span class="sxs-lookup"><span data-stu-id="5bb73-140">skip</span></span>|<span data-ttu-id="5bb73-141">Int32</span><span class="sxs-lookup"><span data-stu-id="5bb73-141">Int32</span></span>|<span data-ttu-id="5bb73-142">尚未记录</span><span class="sxs-lookup"><span data-stu-id="5bb73-142">Not yet documented</span></span>|
|<span data-ttu-id="5bb73-143">top</span><span class="sxs-lookup"><span data-stu-id="5bb73-143">top</span></span>|<span data-ttu-id="5bb73-144">Int32</span><span class="sxs-lookup"><span data-stu-id="5bb73-144">Int32</span></span>|<span data-ttu-id="5bb73-145">尚未记录</span><span class="sxs-lookup"><span data-stu-id="5bb73-145">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="5bb73-146">响应</span><span class="sxs-lookup"><span data-stu-id="5bb73-146">Response</span></span>
<span data-ttu-id="5bb73-147">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 [report](../resources/intune-shared-report.md)。</span><span class="sxs-lookup"><span data-stu-id="5bb73-147">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5bb73-148">示例</span><span class="sxs-lookup"><span data-stu-id="5bb73-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="5bb73-149">请求</span><span class="sxs-lookup"><span data-stu-id="5bb73-149">Request</span></span>
<span data-ttu-id="5bb73-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5bb73-150">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentFailureDetails(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="5bb73-151">响应</span><span class="sxs-lookup"><span data-stu-id="5bb73-151">Response</span></span>
<span data-ttu-id="5bb73-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5bb73-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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







