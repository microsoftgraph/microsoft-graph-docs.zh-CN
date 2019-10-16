---
title: 了 getmobileappcount 函数
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b65496109dcfcf9a259e4274e3bca636da12b218
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538005"
---
# <a name="getmobileappcount-function"></a><span data-ttu-id="b8b96-103">了 getmobileappcount 函数</span><span class="sxs-lookup"><span data-stu-id="b8b96-103">getMobileAppCount function</span></span>

> <span data-ttu-id="b8b96-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b8b96-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b8b96-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b8b96-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8b96-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b8b96-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b8b96-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="b8b96-107">Prerequisites</span></span>
<span data-ttu-id="b8b96-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b8b96-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8b96-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b8b96-110">Permission type</span></span>|<span data-ttu-id="b8b96-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b8b96-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b8b96-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b8b96-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="b8b96-113">&nbsp;&nbsp; **应用**</span><span class="sxs-lookup"><span data-stu-id="b8b96-113">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="b8b96-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b8b96-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="b8b96-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b8b96-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b8b96-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b8b96-116">Not supported.</span></span>|
|<span data-ttu-id="b8b96-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b8b96-117">Application</span></span>||
| <span data-ttu-id="b8b96-118">&nbsp;&nbsp; **应用**</span><span class="sxs-lookup"><span data-stu-id="b8b96-118">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="b8b96-119">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b8b96-119">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b8b96-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b8b96-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/getMobileAppCount
```

## <a name="request-headers"></a><span data-ttu-id="b8b96-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="b8b96-121">Request headers</span></span>
|<span data-ttu-id="b8b96-122">标头</span><span class="sxs-lookup"><span data-stu-id="b8b96-122">Header</span></span>|<span data-ttu-id="b8b96-123">值</span><span class="sxs-lookup"><span data-stu-id="b8b96-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b8b96-124">授权</span><span class="sxs-lookup"><span data-stu-id="b8b96-124">Authorization</span></span>|<span data-ttu-id="b8b96-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b8b96-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b8b96-126">接受</span><span class="sxs-lookup"><span data-stu-id="b8b96-126">Accept</span></span>|<span data-ttu-id="b8b96-127">application/json</span><span class="sxs-lookup"><span data-stu-id="b8b96-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b8b96-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="b8b96-128">Request body</span></span>
<span data-ttu-id="b8b96-129">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="b8b96-129">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="b8b96-130">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="b8b96-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="b8b96-131">属性</span><span class="sxs-lookup"><span data-stu-id="b8b96-131">Property</span></span>|<span data-ttu-id="b8b96-132">类型</span><span class="sxs-lookup"><span data-stu-id="b8b96-132">Type</span></span>|<span data-ttu-id="b8b96-133">说明</span><span class="sxs-lookup"><span data-stu-id="b8b96-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8b96-134">status</span><span class="sxs-lookup"><span data-stu-id="b8b96-134">status</span></span>|<span data-ttu-id="b8b96-135">字符串</span><span class="sxs-lookup"><span data-stu-id="b8b96-135">String</span></span>|<span data-ttu-id="b8b96-136">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b8b96-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="b8b96-137">响应</span><span class="sxs-lookup"><span data-stu-id="b8b96-137">Response</span></span>
<span data-ttu-id="b8b96-138">如果成功，此函数会在`200 OK`响应正文中返回响应代码和 Int64。</span><span class="sxs-lookup"><span data-stu-id="b8b96-138">If successful, this function returns a `200 OK` response code and a Int64 in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8b96-139">示例</span><span class="sxs-lookup"><span data-stu-id="b8b96-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="b8b96-140">请求</span><span class="sxs-lookup"><span data-stu-id="b8b96-140">Request</span></span>
<span data-ttu-id="b8b96-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b8b96-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/getMobileAppCount(status='parameterValue')
```

### <a name="response"></a><span data-ttu-id="b8b96-142">响应</span><span class="sxs-lookup"><span data-stu-id="b8b96-142">Response</span></span>
<span data-ttu-id="b8b96-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b8b96-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 18

{
  "value": 1
}
```






