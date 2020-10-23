---
title: 了 getmobileappcount 函数
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f8cb917403ecb942d385506b5a382f8f23fe3fc3
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48729873"
---
# <a name="getmobileappcount-function"></a><span data-ttu-id="77df6-103">了 getmobileappcount 函数</span><span class="sxs-lookup"><span data-stu-id="77df6-103">getMobileAppCount function</span></span>

<span data-ttu-id="77df6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77df6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="77df6-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="77df6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="77df6-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="77df6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77df6-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="77df6-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="77df6-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="77df6-108">Prerequisites</span></span>
<span data-ttu-id="77df6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="77df6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77df6-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="77df6-111">Permission type</span></span>|<span data-ttu-id="77df6-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="77df6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="77df6-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="77df6-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="77df6-114">&nbsp; &nbsp; **应用**</span><span class="sxs-lookup"><span data-stu-id="77df6-114">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="77df6-115">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="77df6-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="77df6-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="77df6-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="77df6-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="77df6-117">Not supported.</span></span>|
|<span data-ttu-id="77df6-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="77df6-118">Application</span></span>||
| <span data-ttu-id="77df6-119">&nbsp; &nbsp; **应用**</span><span class="sxs-lookup"><span data-stu-id="77df6-119">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="77df6-120">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="77df6-120">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="77df6-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="77df6-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/getMobileAppCount
```

## <a name="request-headers"></a><span data-ttu-id="77df6-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="77df6-122">Request headers</span></span>
|<span data-ttu-id="77df6-123">标头</span><span class="sxs-lookup"><span data-stu-id="77df6-123">Header</span></span>|<span data-ttu-id="77df6-124">值</span><span class="sxs-lookup"><span data-stu-id="77df6-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="77df6-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="77df6-125">Authorization</span></span>|<span data-ttu-id="77df6-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="77df6-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="77df6-127">接受</span><span class="sxs-lookup"><span data-stu-id="77df6-127">Accept</span></span>|<span data-ttu-id="77df6-128">application/json</span><span class="sxs-lookup"><span data-stu-id="77df6-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="77df6-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="77df6-129">Request body</span></span>
<span data-ttu-id="77df6-130">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="77df6-130">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="77df6-131">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="77df6-131">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="77df6-132">属性</span><span class="sxs-lookup"><span data-stu-id="77df6-132">Property</span></span>|<span data-ttu-id="77df6-133">类型</span><span class="sxs-lookup"><span data-stu-id="77df6-133">Type</span></span>|<span data-ttu-id="77df6-134">说明</span><span class="sxs-lookup"><span data-stu-id="77df6-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77df6-135">status</span><span class="sxs-lookup"><span data-stu-id="77df6-135">status</span></span>|<span data-ttu-id="77df6-136">String</span><span class="sxs-lookup"><span data-stu-id="77df6-136">String</span></span>|<span data-ttu-id="77df6-137">尚未记录</span><span class="sxs-lookup"><span data-stu-id="77df6-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="77df6-138">响应</span><span class="sxs-lookup"><span data-stu-id="77df6-138">Response</span></span>
<span data-ttu-id="77df6-139">如果成功，此函数会 `200 OK` 在响应正文中返回响应代码和 Int64。</span><span class="sxs-lookup"><span data-stu-id="77df6-139">If successful, this function returns a `200 OK` response code and a Int64 in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77df6-140">示例</span><span class="sxs-lookup"><span data-stu-id="77df6-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="77df6-141">请求</span><span class="sxs-lookup"><span data-stu-id="77df6-141">Request</span></span>
<span data-ttu-id="77df6-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="77df6-142">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/getMobileAppCount(status='parameterValue')
```

### <a name="response"></a><span data-ttu-id="77df6-143">响应</span><span class="sxs-lookup"><span data-stu-id="77df6-143">Response</span></span>
<span data-ttu-id="77df6-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="77df6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 18

{
  "value": 1
}
```








