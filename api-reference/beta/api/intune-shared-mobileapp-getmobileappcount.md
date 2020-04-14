---
title: 了 getmobileappcount 函数
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b86a60fe9a9ac80152677e97682bd29f8a57ad13
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43441316"
---
# <a name="getmobileappcount-function"></a><span data-ttu-id="a6de2-103">了 getmobileappcount 函数</span><span class="sxs-lookup"><span data-stu-id="a6de2-103">getMobileAppCount function</span></span>

<span data-ttu-id="a6de2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a6de2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a6de2-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a6de2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a6de2-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a6de2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6de2-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="a6de2-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a6de2-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="a6de2-108">Prerequisites</span></span>
<span data-ttu-id="a6de2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a6de2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6de2-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a6de2-111">Permission type</span></span>|<span data-ttu-id="a6de2-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a6de2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a6de2-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a6de2-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="a6de2-114">&nbsp; &nbsp; **应用**</span><span class="sxs-lookup"><span data-stu-id="a6de2-114">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="a6de2-115">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a6de2-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="a6de2-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a6de2-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a6de2-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="a6de2-117">Not supported.</span></span>|
|<span data-ttu-id="a6de2-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="a6de2-118">Application</span></span>||
| <span data-ttu-id="a6de2-119">&nbsp; &nbsp; **应用**</span><span class="sxs-lookup"><span data-stu-id="a6de2-119">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="a6de2-120">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a6de2-120">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a6de2-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a6de2-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/getMobileAppCount
```

## <a name="request-headers"></a><span data-ttu-id="a6de2-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="a6de2-122">Request headers</span></span>
|<span data-ttu-id="a6de2-123">标头</span><span class="sxs-lookup"><span data-stu-id="a6de2-123">Header</span></span>|<span data-ttu-id="a6de2-124">值</span><span class="sxs-lookup"><span data-stu-id="a6de2-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a6de2-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="a6de2-125">Authorization</span></span>|<span data-ttu-id="a6de2-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a6de2-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a6de2-127">接受</span><span class="sxs-lookup"><span data-stu-id="a6de2-127">Accept</span></span>|<span data-ttu-id="a6de2-128">application/json</span><span class="sxs-lookup"><span data-stu-id="a6de2-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6de2-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="a6de2-129">Request body</span></span>
<span data-ttu-id="a6de2-130">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="a6de2-130">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="a6de2-131">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="a6de2-131">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="a6de2-132">属性</span><span class="sxs-lookup"><span data-stu-id="a6de2-132">Property</span></span>|<span data-ttu-id="a6de2-133">类型</span><span class="sxs-lookup"><span data-stu-id="a6de2-133">Type</span></span>|<span data-ttu-id="a6de2-134">说明</span><span class="sxs-lookup"><span data-stu-id="a6de2-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6de2-135">状态</span><span class="sxs-lookup"><span data-stu-id="a6de2-135">status</span></span>|<span data-ttu-id="a6de2-136">String</span><span class="sxs-lookup"><span data-stu-id="a6de2-136">String</span></span>|<span data-ttu-id="a6de2-137">尚未记录</span><span class="sxs-lookup"><span data-stu-id="a6de2-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="a6de2-138">响应</span><span class="sxs-lookup"><span data-stu-id="a6de2-138">Response</span></span>
<span data-ttu-id="a6de2-139">如果成功，此函数会在`200 OK`响应正文中返回响应代码和 Int64。</span><span class="sxs-lookup"><span data-stu-id="a6de2-139">If successful, this function returns a `200 OK` response code and a Int64 in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6de2-140">示例</span><span class="sxs-lookup"><span data-stu-id="a6de2-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="a6de2-141">请求</span><span class="sxs-lookup"><span data-stu-id="a6de2-141">Request</span></span>
<span data-ttu-id="a6de2-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a6de2-142">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/getMobileAppCount(status='parameterValue')
```

### <a name="response"></a><span data-ttu-id="a6de2-143">响应</span><span class="sxs-lookup"><span data-stu-id="a6de2-143">Response</span></span>
<span data-ttu-id="a6de2-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a6de2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 18

{
  "value": 1
}
```






