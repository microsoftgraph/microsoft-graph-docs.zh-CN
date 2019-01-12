---
title: managedDeviceEnrollmentFailureDetails 函数
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 48f7f2c36781be29842c1c614e8d2a14ec7e1d94
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27915114"
---
# <a name="manageddeviceenrollmentfailuredetails-function"></a><span data-ttu-id="89c19-103">managedDeviceEnrollmentFailureDetails 函数</span><span class="sxs-lookup"><span data-stu-id="89c19-103">managedDeviceEnrollmentFailureDetails function</span></span>

> <span data-ttu-id="89c19-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="89c19-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="89c19-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="89c19-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="89c19-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="89c19-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="89c19-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="89c19-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="89c19-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="89c19-108">Prerequisites</span></span>
<span data-ttu-id="89c19-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="89c19-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89c19-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="89c19-111">Permission type</span></span>|<span data-ttu-id="89c19-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="89c19-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="89c19-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="89c19-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="89c19-114">&nbsp; &nbsp; **故障排除**</span><span class="sxs-lookup"><span data-stu-id="89c19-114">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="89c19-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89c19-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="89c19-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="89c19-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="89c19-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="89c19-117">Not supported.</span></span>|
|<span data-ttu-id="89c19-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="89c19-118">Application</span></span>|<span data-ttu-id="89c19-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="89c19-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="89c19-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="89c19-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentFailureDetails
```

## <a name="request-headers"></a><span data-ttu-id="89c19-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="89c19-121">Request headers</span></span>
|<span data-ttu-id="89c19-122">标头</span><span class="sxs-lookup"><span data-stu-id="89c19-122">Header</span></span>|<span data-ttu-id="89c19-123">值</span><span class="sxs-lookup"><span data-stu-id="89c19-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="89c19-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="89c19-124">Authorization</span></span>|<span data-ttu-id="89c19-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="89c19-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="89c19-126">Accept</span><span class="sxs-lookup"><span data-stu-id="89c19-126">Accept</span></span>|<span data-ttu-id="89c19-127">application/json</span><span class="sxs-lookup"><span data-stu-id="89c19-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="89c19-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="89c19-128">Request body</span></span>
<span data-ttu-id="89c19-129">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="89c19-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="89c19-130">属性</span><span class="sxs-lookup"><span data-stu-id="89c19-130">Property</span></span>|<span data-ttu-id="89c19-131">类型</span><span class="sxs-lookup"><span data-stu-id="89c19-131">Type</span></span>|<span data-ttu-id="89c19-132">说明</span><span class="sxs-lookup"><span data-stu-id="89c19-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89c19-133">筛选器</span><span class="sxs-lookup"><span data-stu-id="89c19-133">filter</span></span>|<span data-ttu-id="89c19-134">字符串</span><span class="sxs-lookup"><span data-stu-id="89c19-134">String</span></span>|<span data-ttu-id="89c19-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="89c19-135">Not yet documented</span></span>|
|<span data-ttu-id="89c19-136">skipToken</span><span class="sxs-lookup"><span data-stu-id="89c19-136">skipToken</span></span>|<span data-ttu-id="89c19-137">字符串</span><span class="sxs-lookup"><span data-stu-id="89c19-137">String</span></span>|<span data-ttu-id="89c19-138">尚未记录</span><span class="sxs-lookup"><span data-stu-id="89c19-138">Not yet documented</span></span>|
|<span data-ttu-id="89c19-139">skip</span><span class="sxs-lookup"><span data-stu-id="89c19-139">skip</span></span>|<span data-ttu-id="89c19-140">Int32</span><span class="sxs-lookup"><span data-stu-id="89c19-140">Int32</span></span>|<span data-ttu-id="89c19-141">尚未记录</span><span class="sxs-lookup"><span data-stu-id="89c19-141">Not yet documented</span></span>|
|<span data-ttu-id="89c19-142">top</span><span class="sxs-lookup"><span data-stu-id="89c19-142">top</span></span>|<span data-ttu-id="89c19-143">Int32</span><span class="sxs-lookup"><span data-stu-id="89c19-143">Int32</span></span>|<span data-ttu-id="89c19-144">尚未记录</span><span class="sxs-lookup"><span data-stu-id="89c19-144">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="89c19-145">响应</span><span class="sxs-lookup"><span data-stu-id="89c19-145">Response</span></span>
<span data-ttu-id="89c19-146">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 [report](../resources/intune-shared-report.md)。</span><span class="sxs-lookup"><span data-stu-id="89c19-146">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89c19-147">示例</span><span class="sxs-lookup"><span data-stu-id="89c19-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="89c19-148">请求</span><span class="sxs-lookup"><span data-stu-id="89c19-148">Request</span></span>
<span data-ttu-id="89c19-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="89c19-149">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentFailureDetails(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="89c19-150">响应</span><span class="sxs-lookup"><span data-stu-id="89c19-150">Response</span></span>
<span data-ttu-id="89c19-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="89c19-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



