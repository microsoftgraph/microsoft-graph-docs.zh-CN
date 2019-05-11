---
title: getAuditActivityTypes 函数
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 685cf4982677d1cf572778c84badcb7184723e96
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33934402"
---
# <a name="getauditactivitytypes-function"></a><span data-ttu-id="42eb9-103">getAuditActivityTypes 函数</span><span class="sxs-lookup"><span data-stu-id="42eb9-103">getAuditActivityTypes function</span></span>

> <span data-ttu-id="42eb9-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="42eb9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="42eb9-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="42eb9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42eb9-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="42eb9-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="42eb9-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="42eb9-107">Prerequisites</span></span>
<span data-ttu-id="42eb9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="42eb9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42eb9-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="42eb9-110">Permission type</span></span>|<span data-ttu-id="42eb9-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="42eb9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="42eb9-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="42eb9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="42eb9-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="42eb9-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="42eb9-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="42eb9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="42eb9-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="42eb9-115">Not supported.</span></span>|
|<span data-ttu-id="42eb9-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="42eb9-116">Application</span></span>|<span data-ttu-id="42eb9-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="42eb9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="42eb9-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="42eb9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents/getAuditActivityTypes
```

## <a name="request-headers"></a><span data-ttu-id="42eb9-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="42eb9-119">Request headers</span></span>
|<span data-ttu-id="42eb9-120">标头</span><span class="sxs-lookup"><span data-stu-id="42eb9-120">Header</span></span>|<span data-ttu-id="42eb9-121">值</span><span class="sxs-lookup"><span data-stu-id="42eb9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="42eb9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="42eb9-122">Authorization</span></span>|<span data-ttu-id="42eb9-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="42eb9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="42eb9-124">接受</span><span class="sxs-lookup"><span data-stu-id="42eb9-124">Accept</span></span>|<span data-ttu-id="42eb9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="42eb9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="42eb9-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="42eb9-126">Request body</span></span>
<span data-ttu-id="42eb9-127">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="42eb9-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="42eb9-128">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="42eb9-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="42eb9-129">属性</span><span class="sxs-lookup"><span data-stu-id="42eb9-129">Property</span></span>|<span data-ttu-id="42eb9-130">类型</span><span class="sxs-lookup"><span data-stu-id="42eb9-130">Type</span></span>|<span data-ttu-id="42eb9-131">说明</span><span class="sxs-lookup"><span data-stu-id="42eb9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42eb9-132">“类别”</span><span class="sxs-lookup"><span data-stu-id="42eb9-132">category</span></span>|<span data-ttu-id="42eb9-133">String</span><span class="sxs-lookup"><span data-stu-id="42eb9-133">String</span></span>|<span data-ttu-id="42eb9-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="42eb9-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="42eb9-135">响应</span><span class="sxs-lookup"><span data-stu-id="42eb9-135">Response</span></span>
<span data-ttu-id="42eb9-136">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 String 集合。</span><span class="sxs-lookup"><span data-stu-id="42eb9-136">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42eb9-137">示例</span><span class="sxs-lookup"><span data-stu-id="42eb9-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="42eb9-138">请求</span><span class="sxs-lookup"><span data-stu-id="42eb9-138">Request</span></span>
<span data-ttu-id="42eb9-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="42eb9-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/auditEvents/getAuditActivityTypes(category='parameterValue')
```

### <a name="response"></a><span data-ttu-id="42eb9-140">响应</span><span class="sxs-lookup"><span data-stu-id="42eb9-140">Response</span></span>
<span data-ttu-id="42eb9-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="42eb9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




