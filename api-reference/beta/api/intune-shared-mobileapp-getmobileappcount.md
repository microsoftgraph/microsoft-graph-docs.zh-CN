---
title: 了 getmobileappcount 函数
description: 尚未记录
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6c0c0e78046ad9c9ff2833adf6b68c97ca8508d9
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42800793"
---
# <a name="getmobileappcount-function"></a><span data-ttu-id="2a736-103">了 getmobileappcount 函数</span><span class="sxs-lookup"><span data-stu-id="2a736-103">getMobileAppCount function</span></span>

> <span data-ttu-id="2a736-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2a736-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2a736-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2a736-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2a736-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="2a736-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2a736-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="2a736-107">Prerequisites</span></span>
<span data-ttu-id="2a736-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2a736-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a736-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="2a736-110">Permission type</span></span>|<span data-ttu-id="2a736-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2a736-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2a736-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2a736-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="2a736-113">&nbsp; &nbsp; **应用**</span><span class="sxs-lookup"><span data-stu-id="2a736-113">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="2a736-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="2a736-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="2a736-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2a736-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2a736-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2a736-116">Not supported.</span></span>|
|<span data-ttu-id="2a736-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="2a736-117">Application</span></span>||
| <span data-ttu-id="2a736-118">&nbsp; &nbsp; **应用**</span><span class="sxs-lookup"><span data-stu-id="2a736-118">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="2a736-119">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="2a736-119">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2a736-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2a736-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/getMobileAppCount
```

## <a name="request-headers"></a><span data-ttu-id="2a736-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="2a736-121">Request headers</span></span>
|<span data-ttu-id="2a736-122">标头</span><span class="sxs-lookup"><span data-stu-id="2a736-122">Header</span></span>|<span data-ttu-id="2a736-123">值</span><span class="sxs-lookup"><span data-stu-id="2a736-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2a736-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="2a736-124">Authorization</span></span>|<span data-ttu-id="2a736-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2a736-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2a736-126">接受</span><span class="sxs-lookup"><span data-stu-id="2a736-126">Accept</span></span>|<span data-ttu-id="2a736-127">application/json</span><span class="sxs-lookup"><span data-stu-id="2a736-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a736-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="2a736-128">Request body</span></span>
<span data-ttu-id="2a736-129">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="2a736-129">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="2a736-130">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="2a736-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="2a736-131">属性</span><span class="sxs-lookup"><span data-stu-id="2a736-131">Property</span></span>|<span data-ttu-id="2a736-132">类型</span><span class="sxs-lookup"><span data-stu-id="2a736-132">Type</span></span>|<span data-ttu-id="2a736-133">说明</span><span class="sxs-lookup"><span data-stu-id="2a736-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a736-134">状态</span><span class="sxs-lookup"><span data-stu-id="2a736-134">status</span></span>|<span data-ttu-id="2a736-135">String</span><span class="sxs-lookup"><span data-stu-id="2a736-135">String</span></span>|<span data-ttu-id="2a736-136">尚未记录</span><span class="sxs-lookup"><span data-stu-id="2a736-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="2a736-137">响应</span><span class="sxs-lookup"><span data-stu-id="2a736-137">Response</span></span>
<span data-ttu-id="2a736-138">如果成功，此函数会在`200 OK`响应正文中返回响应代码和 Int64。</span><span class="sxs-lookup"><span data-stu-id="2a736-138">If successful, this function returns a `200 OK` response code and a Int64 in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2a736-139">示例</span><span class="sxs-lookup"><span data-stu-id="2a736-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="2a736-140">请求</span><span class="sxs-lookup"><span data-stu-id="2a736-140">Request</span></span>
<span data-ttu-id="2a736-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2a736-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/getMobileAppCount(status='parameterValue')
```

### <a name="response"></a><span data-ttu-id="2a736-142">响应</span><span class="sxs-lookup"><span data-stu-id="2a736-142">Response</span></span>
<span data-ttu-id="2a736-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2a736-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 18

{
  "value": 1
}
```







