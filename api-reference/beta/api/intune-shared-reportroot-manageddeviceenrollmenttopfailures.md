---
title: managedDeviceEnrollmentTopFailures 函数
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 163a75a2ffa675f939086fecf3e9c4a155352aa1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27934224"
---
# <a name="manageddeviceenrollmenttopfailures-function"></a><span data-ttu-id="fb4c7-103">managedDeviceEnrollmentTopFailures 函数</span><span class="sxs-lookup"><span data-stu-id="fb4c7-103">managedDeviceEnrollmentTopFailures function</span></span>

> <span data-ttu-id="fb4c7-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="fb4c7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fb4c7-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="fb4c7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fb4c7-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="fb4c7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fb4c7-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="fb4c7-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fb4c7-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="fb4c7-108">Prerequisites</span></span>
<span data-ttu-id="fb4c7-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="fb4c7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb4c7-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="fb4c7-111">Permission type</span></span>|<span data-ttu-id="fb4c7-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="fb4c7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fb4c7-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fb4c7-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="fb4c7-114">&nbsp; &nbsp; **疑难解答**</span><span class="sxs-lookup"><span data-stu-id="fb4c7-114">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="fb4c7-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb4c7-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="fb4c7-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fb4c7-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fb4c7-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="fb4c7-117">Not supported.</span></span>|
|<span data-ttu-id="fb4c7-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="fb4c7-118">Application</span></span>|<span data-ttu-id="fb4c7-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="fb4c7-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fb4c7-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fb4c7-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentTopFailures
```

## <a name="request-headers"></a><span data-ttu-id="fb4c7-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="fb4c7-121">Request headers</span></span>
|<span data-ttu-id="fb4c7-122">标头</span><span class="sxs-lookup"><span data-stu-id="fb4c7-122">Header</span></span>|<span data-ttu-id="fb4c7-123">值</span><span class="sxs-lookup"><span data-stu-id="fb4c7-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fb4c7-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="fb4c7-124">Authorization</span></span>|<span data-ttu-id="fb4c7-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="fb4c7-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fb4c7-126">Accept</span><span class="sxs-lookup"><span data-stu-id="fb4c7-126">Accept</span></span>|<span data-ttu-id="fb4c7-127">application/json</span><span class="sxs-lookup"><span data-stu-id="fb4c7-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb4c7-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="fb4c7-128">Request body</span></span>
<span data-ttu-id="fb4c7-129">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="fb4c7-129">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="fb4c7-130">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="fb4c7-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="fb4c7-131">属性</span><span class="sxs-lookup"><span data-stu-id="fb4c7-131">Property</span></span>|<span data-ttu-id="fb4c7-132">类型</span><span class="sxs-lookup"><span data-stu-id="fb4c7-132">Type</span></span>|<span data-ttu-id="fb4c7-133">说明</span><span class="sxs-lookup"><span data-stu-id="fb4c7-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb4c7-134">period</span><span class="sxs-lookup"><span data-stu-id="fb4c7-134">period</span></span>|<span data-ttu-id="fb4c7-135">字符串</span><span class="sxs-lookup"><span data-stu-id="fb4c7-135">String</span></span>|<span data-ttu-id="fb4c7-136">尚未记录</span><span class="sxs-lookup"><span data-stu-id="fb4c7-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="fb4c7-137">响应</span><span class="sxs-lookup"><span data-stu-id="fb4c7-137">Response</span></span>
<span data-ttu-id="fb4c7-138">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 [report](../resources/intune-shared-report.md)。</span><span class="sxs-lookup"><span data-stu-id="fb4c7-138">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb4c7-139">示例</span><span class="sxs-lookup"><span data-stu-id="fb4c7-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="fb4c7-140">请求</span><span class="sxs-lookup"><span data-stu-id="fb4c7-140">Request</span></span>
<span data-ttu-id="fb4c7-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fb4c7-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentTopFailures(period='parameterValue')
```

### <a name="response"></a><span data-ttu-id="fb4c7-142">响应</span><span class="sxs-lookup"><span data-stu-id="fb4c7-142">Response</span></span>
<span data-ttu-id="fb4c7-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fb4c7-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



