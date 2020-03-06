---
title: getAuditActivityTypes 函数
description: 尚未记录
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f1749bd523acd02cc39596906be9627604182f87
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42515747"
---
# <a name="getauditactivitytypes-function"></a><span data-ttu-id="94660-103">getAuditActivityTypes 函数</span><span class="sxs-lookup"><span data-stu-id="94660-103">getAuditActivityTypes function</span></span>

<span data-ttu-id="94660-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="94660-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="94660-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="94660-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="94660-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="94660-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="94660-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="94660-107">Prerequisites</span></span>
<span data-ttu-id="94660-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="94660-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94660-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="94660-110">Permission type</span></span>|<span data-ttu-id="94660-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="94660-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="94660-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="94660-112">Delegated (work or school account)</span></span>|<span data-ttu-id="94660-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="94660-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="94660-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="94660-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="94660-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="94660-115">Not supported.</span></span>|
|<span data-ttu-id="94660-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="94660-116">Application</span></span>|<span data-ttu-id="94660-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="94660-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="94660-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="94660-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents/getAuditActivityTypes
```

## <a name="request-headers"></a><span data-ttu-id="94660-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="94660-119">Request headers</span></span>
|<span data-ttu-id="94660-120">标头</span><span class="sxs-lookup"><span data-stu-id="94660-120">Header</span></span>|<span data-ttu-id="94660-121">值</span><span class="sxs-lookup"><span data-stu-id="94660-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="94660-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="94660-122">Authorization</span></span>|<span data-ttu-id="94660-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="94660-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="94660-124">接受</span><span class="sxs-lookup"><span data-stu-id="94660-124">Accept</span></span>|<span data-ttu-id="94660-125">application/json</span><span class="sxs-lookup"><span data-stu-id="94660-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="94660-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="94660-126">Request body</span></span>
<span data-ttu-id="94660-127">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="94660-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="94660-128">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="94660-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="94660-129">属性</span><span class="sxs-lookup"><span data-stu-id="94660-129">Property</span></span>|<span data-ttu-id="94660-130">类型</span><span class="sxs-lookup"><span data-stu-id="94660-130">Type</span></span>|<span data-ttu-id="94660-131">说明</span><span class="sxs-lookup"><span data-stu-id="94660-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94660-132">“类别”</span><span class="sxs-lookup"><span data-stu-id="94660-132">category</span></span>|<span data-ttu-id="94660-133">字符串</span><span class="sxs-lookup"><span data-stu-id="94660-133">String</span></span>|<span data-ttu-id="94660-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="94660-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="94660-135">响应</span><span class="sxs-lookup"><span data-stu-id="94660-135">Response</span></span>
<span data-ttu-id="94660-136">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 String 集合。</span><span class="sxs-lookup"><span data-stu-id="94660-136">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="94660-137">示例</span><span class="sxs-lookup"><span data-stu-id="94660-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="94660-138">请求</span><span class="sxs-lookup"><span data-stu-id="94660-138">Request</span></span>
<span data-ttu-id="94660-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="94660-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/auditEvents/getAuditActivityTypes(category='parameterValue')
```

### <a name="response"></a><span data-ttu-id="94660-140">响应</span><span class="sxs-lookup"><span data-stu-id="94660-140">Response</span></span>
<span data-ttu-id="94660-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="94660-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




