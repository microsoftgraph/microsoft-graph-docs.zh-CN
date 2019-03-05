---
title: 了 getmobileappcount 函数
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6b01006e6b1976e02836fe0d532647014c632a02
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30164594"
---
# <a name="getmobileappcount-function"></a><span data-ttu-id="01a12-103">了 getmobileappcount 函数</span><span class="sxs-lookup"><span data-stu-id="01a12-103">getMobileAppCount function</span></span>

> <span data-ttu-id="01a12-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="01a12-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="01a12-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="01a12-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="01a12-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="01a12-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="01a12-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="01a12-107">Prerequisites</span></span>
<span data-ttu-id="01a12-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="01a12-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="01a12-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="01a12-110">Permission type</span></span>|<span data-ttu-id="01a12-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="01a12-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="01a12-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="01a12-112">Delegated (work or school account)</span></span>|<span data-ttu-id="01a12-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="01a12-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="01a12-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="01a12-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="01a12-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="01a12-115">Not supported.</span></span>|
|<span data-ttu-id="01a12-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="01a12-116">Application</span></span>|<span data-ttu-id="01a12-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="01a12-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="01a12-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="01a12-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/getMobileAppCount
```

## <a name="request-headers"></a><span data-ttu-id="01a12-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="01a12-119">Request headers</span></span>
|<span data-ttu-id="01a12-120">标头</span><span class="sxs-lookup"><span data-stu-id="01a12-120">Header</span></span>|<span data-ttu-id="01a12-121">值</span><span class="sxs-lookup"><span data-stu-id="01a12-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="01a12-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="01a12-122">Authorization</span></span>|<span data-ttu-id="01a12-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="01a12-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="01a12-124">Accept</span><span class="sxs-lookup"><span data-stu-id="01a12-124">Accept</span></span>|<span data-ttu-id="01a12-125">application/json</span><span class="sxs-lookup"><span data-stu-id="01a12-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="01a12-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="01a12-126">Request body</span></span>
<span data-ttu-id="01a12-127">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="01a12-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="01a12-128">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="01a12-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="01a12-129">属性</span><span class="sxs-lookup"><span data-stu-id="01a12-129">Property</span></span>|<span data-ttu-id="01a12-130">类型</span><span class="sxs-lookup"><span data-stu-id="01a12-130">Type</span></span>|<span data-ttu-id="01a12-131">说明</span><span class="sxs-lookup"><span data-stu-id="01a12-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01a12-132">状态</span><span class="sxs-lookup"><span data-stu-id="01a12-132">status</span></span>|<span data-ttu-id="01a12-133">String</span><span class="sxs-lookup"><span data-stu-id="01a12-133">String</span></span>|<span data-ttu-id="01a12-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="01a12-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="01a12-135">响应</span><span class="sxs-lookup"><span data-stu-id="01a12-135">Response</span></span>
<span data-ttu-id="01a12-136">如果成功, 此函数会在`200 OK`响应正文中返回响应代码和 Int64。</span><span class="sxs-lookup"><span data-stu-id="01a12-136">If successful, this function returns a `200 OK` response code and a Int64 in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01a12-137">示例</span><span class="sxs-lookup"><span data-stu-id="01a12-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="01a12-138">请求</span><span class="sxs-lookup"><span data-stu-id="01a12-138">Request</span></span>
<span data-ttu-id="01a12-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="01a12-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/getMobileAppCount(status='parameterValue')
```

### <a name="response"></a><span data-ttu-id="01a12-140">响应</span><span class="sxs-lookup"><span data-stu-id="01a12-140">Response</span></span>
<span data-ttu-id="01a12-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="01a12-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 18

{
  "value": 1
}
```




