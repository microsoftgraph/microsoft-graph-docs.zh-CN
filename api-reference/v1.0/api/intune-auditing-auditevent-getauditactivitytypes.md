---
title: getAuditActivityTypes 函数
description: 尚未记录
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 40326b1f08bf5ac243770b98c00d580cc66aa665
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37358044"
---
# <a name="getauditactivitytypes-function"></a><span data-ttu-id="0a1e2-103">getAuditActivityTypes 函数</span><span class="sxs-lookup"><span data-stu-id="0a1e2-103">getAuditActivityTypes function</span></span>

> <span data-ttu-id="0a1e2-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0a1e2-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0a1e2-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="0a1e2-105">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0a1e2-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="0a1e2-106">Prerequisites</span></span>
<span data-ttu-id="0a1e2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0a1e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a1e2-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0a1e2-109">Permission type</span></span>|<span data-ttu-id="0a1e2-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0a1e2-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0a1e2-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0a1e2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0a1e2-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="0a1e2-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="0a1e2-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0a1e2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0a1e2-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0a1e2-114">Not supported.</span></span>|
|<span data-ttu-id="0a1e2-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="0a1e2-115">Application</span></span>|<span data-ttu-id="0a1e2-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0a1e2-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0a1e2-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0a1e2-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents/getAuditActivityTypes
```

## <a name="request-headers"></a><span data-ttu-id="0a1e2-118">请求头</span><span class="sxs-lookup"><span data-stu-id="0a1e2-118">Request headers</span></span>
|<span data-ttu-id="0a1e2-119">标头</span><span class="sxs-lookup"><span data-stu-id="0a1e2-119">Header</span></span>|<span data-ttu-id="0a1e2-120">值</span><span class="sxs-lookup"><span data-stu-id="0a1e2-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0a1e2-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0a1e2-121">Authorization</span></span>|<span data-ttu-id="0a1e2-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0a1e2-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0a1e2-123">接受</span><span class="sxs-lookup"><span data-stu-id="0a1e2-123">Accept</span></span>|<span data-ttu-id="0a1e2-124">application/json</span><span class="sxs-lookup"><span data-stu-id="0a1e2-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0a1e2-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="0a1e2-125">Request body</span></span>
<span data-ttu-id="0a1e2-126">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="0a1e2-126">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="0a1e2-127">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="0a1e2-127">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="0a1e2-128">属性</span><span class="sxs-lookup"><span data-stu-id="0a1e2-128">Property</span></span>|<span data-ttu-id="0a1e2-129">类型</span><span class="sxs-lookup"><span data-stu-id="0a1e2-129">Type</span></span>|<span data-ttu-id="0a1e2-130">说明</span><span class="sxs-lookup"><span data-stu-id="0a1e2-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a1e2-131">“类别”</span><span class="sxs-lookup"><span data-stu-id="0a1e2-131">category</span></span>|<span data-ttu-id="0a1e2-132">String</span><span class="sxs-lookup"><span data-stu-id="0a1e2-132">String</span></span>|<span data-ttu-id="0a1e2-133">尚未记录</span><span class="sxs-lookup"><span data-stu-id="0a1e2-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="0a1e2-134">响应</span><span class="sxs-lookup"><span data-stu-id="0a1e2-134">Response</span></span>
<span data-ttu-id="0a1e2-135">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 String 集合。</span><span class="sxs-lookup"><span data-stu-id="0a1e2-135">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0a1e2-136">示例</span><span class="sxs-lookup"><span data-stu-id="0a1e2-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="0a1e2-137">请求</span><span class="sxs-lookup"><span data-stu-id="0a1e2-137">Request</span></span>
<span data-ttu-id="0a1e2-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0a1e2-138">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/auditEvents/getAuditActivityTypes(category='parameterValue')
```

### <a name="response"></a><span data-ttu-id="0a1e2-139">响应</span><span class="sxs-lookup"><span data-stu-id="0a1e2-139">Response</span></span>
<span data-ttu-id="0a1e2-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0a1e2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




