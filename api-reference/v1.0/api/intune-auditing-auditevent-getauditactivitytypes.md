---
title: getAuditActivityTypes 函数
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 845ae66814bbe02e52759e007bd58c749d5c3db3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47966119"
---
# <a name="getauditactivitytypes-function"></a><span data-ttu-id="69bc4-103">getAuditActivityTypes 函数</span><span class="sxs-lookup"><span data-stu-id="69bc4-103">getAuditActivityTypes function</span></span>

<span data-ttu-id="69bc4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69bc4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="69bc4-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="69bc4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="69bc4-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="69bc4-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="69bc4-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="69bc4-107">Prerequisites</span></span>
<span data-ttu-id="69bc4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="69bc4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69bc4-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="69bc4-110">Permission type</span></span>|<span data-ttu-id="69bc4-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="69bc4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="69bc4-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="69bc4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="69bc4-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="69bc4-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="69bc4-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="69bc4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="69bc4-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="69bc4-115">Not supported.</span></span>|
|<span data-ttu-id="69bc4-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="69bc4-116">Application</span></span>|<span data-ttu-id="69bc4-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="69bc4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="69bc4-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="69bc4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents/getAuditActivityTypes
```

## <a name="request-headers"></a><span data-ttu-id="69bc4-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="69bc4-119">Request headers</span></span>
|<span data-ttu-id="69bc4-120">标头</span><span class="sxs-lookup"><span data-stu-id="69bc4-120">Header</span></span>|<span data-ttu-id="69bc4-121">值</span><span class="sxs-lookup"><span data-stu-id="69bc4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="69bc4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="69bc4-122">Authorization</span></span>|<span data-ttu-id="69bc4-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="69bc4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="69bc4-124">接受</span><span class="sxs-lookup"><span data-stu-id="69bc4-124">Accept</span></span>|<span data-ttu-id="69bc4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="69bc4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="69bc4-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="69bc4-126">Request body</span></span>
<span data-ttu-id="69bc4-127">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="69bc4-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="69bc4-128">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="69bc4-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="69bc4-129">属性</span><span class="sxs-lookup"><span data-stu-id="69bc4-129">Property</span></span>|<span data-ttu-id="69bc4-130">类型</span><span class="sxs-lookup"><span data-stu-id="69bc4-130">Type</span></span>|<span data-ttu-id="69bc4-131">说明</span><span class="sxs-lookup"><span data-stu-id="69bc4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69bc4-132">“类别”</span><span class="sxs-lookup"><span data-stu-id="69bc4-132">category</span></span>|<span data-ttu-id="69bc4-133">String</span><span class="sxs-lookup"><span data-stu-id="69bc4-133">String</span></span>|<span data-ttu-id="69bc4-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="69bc4-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="69bc4-135">响应</span><span class="sxs-lookup"><span data-stu-id="69bc4-135">Response</span></span>
<span data-ttu-id="69bc4-136">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 String 集合。</span><span class="sxs-lookup"><span data-stu-id="69bc4-136">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69bc4-137">示例</span><span class="sxs-lookup"><span data-stu-id="69bc4-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="69bc4-138">请求</span><span class="sxs-lookup"><span data-stu-id="69bc4-138">Request</span></span>
<span data-ttu-id="69bc4-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="69bc4-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/auditEvents/getAuditActivityTypes(category='parameterValue')
```

### <a name="response"></a><span data-ttu-id="69bc4-140">响应</span><span class="sxs-lookup"><span data-stu-id="69bc4-140">Response</span></span>
<span data-ttu-id="69bc4-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="69bc4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 61

{
  "value": [
    "Get Audit Activity Types value"
  ]
}
```









