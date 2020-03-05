---
title: 了 getmobileappcount 函数
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6b00e12a0810ba89ca868e6a1f4d9146ca351997
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42458299"
---
# <a name="getmobileappcount-function"></a><span data-ttu-id="faad1-103">了 getmobileappcount 函数</span><span class="sxs-lookup"><span data-stu-id="faad1-103">getMobileAppCount function</span></span>

<span data-ttu-id="faad1-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="faad1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="faad1-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="faad1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="faad1-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="faad1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="faad1-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="faad1-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="faad1-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="faad1-108">Prerequisites</span></span>
<span data-ttu-id="faad1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="faad1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="faad1-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="faad1-111">Permission type</span></span>|<span data-ttu-id="faad1-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="faad1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="faad1-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="faad1-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="faad1-114">&nbsp; &nbsp; **应用**</span><span class="sxs-lookup"><span data-stu-id="faad1-114">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="faad1-115">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="faad1-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="faad1-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="faad1-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="faad1-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="faad1-117">Not supported.</span></span>|
|<span data-ttu-id="faad1-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="faad1-118">Application</span></span>||
| <span data-ttu-id="faad1-119">&nbsp; &nbsp; **应用**</span><span class="sxs-lookup"><span data-stu-id="faad1-119">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="faad1-120">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="faad1-120">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="faad1-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="faad1-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/getMobileAppCount
```

## <a name="request-headers"></a><span data-ttu-id="faad1-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="faad1-122">Request headers</span></span>
|<span data-ttu-id="faad1-123">标头</span><span class="sxs-lookup"><span data-stu-id="faad1-123">Header</span></span>|<span data-ttu-id="faad1-124">值</span><span class="sxs-lookup"><span data-stu-id="faad1-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="faad1-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="faad1-125">Authorization</span></span>|<span data-ttu-id="faad1-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="faad1-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="faad1-127">接受</span><span class="sxs-lookup"><span data-stu-id="faad1-127">Accept</span></span>|<span data-ttu-id="faad1-128">application/json</span><span class="sxs-lookup"><span data-stu-id="faad1-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="faad1-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="faad1-129">Request body</span></span>
<span data-ttu-id="faad1-130">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="faad1-130">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="faad1-131">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="faad1-131">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="faad1-132">属性</span><span class="sxs-lookup"><span data-stu-id="faad1-132">Property</span></span>|<span data-ttu-id="faad1-133">类型</span><span class="sxs-lookup"><span data-stu-id="faad1-133">Type</span></span>|<span data-ttu-id="faad1-134">说明</span><span class="sxs-lookup"><span data-stu-id="faad1-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="faad1-135">status</span><span class="sxs-lookup"><span data-stu-id="faad1-135">status</span></span>|<span data-ttu-id="faad1-136">String</span><span class="sxs-lookup"><span data-stu-id="faad1-136">String</span></span>|<span data-ttu-id="faad1-137">尚未记录</span><span class="sxs-lookup"><span data-stu-id="faad1-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="faad1-138">响应</span><span class="sxs-lookup"><span data-stu-id="faad1-138">Response</span></span>
<span data-ttu-id="faad1-139">如果成功，此函数会在`200 OK`响应正文中返回响应代码和 Int64。</span><span class="sxs-lookup"><span data-stu-id="faad1-139">If successful, this function returns a `200 OK` response code and a Int64 in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="faad1-140">示例</span><span class="sxs-lookup"><span data-stu-id="faad1-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="faad1-141">请求</span><span class="sxs-lookup"><span data-stu-id="faad1-141">Request</span></span>
<span data-ttu-id="faad1-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="faad1-142">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/getMobileAppCount(status='parameterValue')
```

### <a name="response"></a><span data-ttu-id="faad1-143">响应</span><span class="sxs-lookup"><span data-stu-id="faad1-143">Response</span></span>
<span data-ttu-id="faad1-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="faad1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 18

{
  "value": 1
}
```








