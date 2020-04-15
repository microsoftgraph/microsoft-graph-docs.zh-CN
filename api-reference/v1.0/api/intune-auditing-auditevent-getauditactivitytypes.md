---
title: getAuditActivityTypes 函数
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 57f3af7dc556f05eeecd7dbb395152f923b41e11
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43464385"
---
# <a name="getauditactivitytypes-function"></a><span data-ttu-id="e28c5-103">getAuditActivityTypes 函数</span><span class="sxs-lookup"><span data-stu-id="e28c5-103">getAuditActivityTypes function</span></span>

<span data-ttu-id="e28c5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e28c5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e28c5-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e28c5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e28c5-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e28c5-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e28c5-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="e28c5-107">Prerequisites</span></span>
<span data-ttu-id="e28c5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e28c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e28c5-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e28c5-110">Permission type</span></span>|<span data-ttu-id="e28c5-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e28c5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e28c5-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e28c5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e28c5-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e28c5-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="e28c5-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e28c5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e28c5-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e28c5-115">Not supported.</span></span>|
|<span data-ttu-id="e28c5-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="e28c5-116">Application</span></span>|<span data-ttu-id="e28c5-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="e28c5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e28c5-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e28c5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents/getAuditActivityTypes
```

## <a name="request-headers"></a><span data-ttu-id="e28c5-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="e28c5-119">Request headers</span></span>
|<span data-ttu-id="e28c5-120">标头</span><span class="sxs-lookup"><span data-stu-id="e28c5-120">Header</span></span>|<span data-ttu-id="e28c5-121">值</span><span class="sxs-lookup"><span data-stu-id="e28c5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e28c5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e28c5-122">Authorization</span></span>|<span data-ttu-id="e28c5-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e28c5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e28c5-124">接受</span><span class="sxs-lookup"><span data-stu-id="e28c5-124">Accept</span></span>|<span data-ttu-id="e28c5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e28c5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e28c5-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="e28c5-126">Request body</span></span>
<span data-ttu-id="e28c5-127">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="e28c5-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="e28c5-128">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="e28c5-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="e28c5-129">属性</span><span class="sxs-lookup"><span data-stu-id="e28c5-129">Property</span></span>|<span data-ttu-id="e28c5-130">类型</span><span class="sxs-lookup"><span data-stu-id="e28c5-130">Type</span></span>|<span data-ttu-id="e28c5-131">说明</span><span class="sxs-lookup"><span data-stu-id="e28c5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e28c5-132">“类别”</span><span class="sxs-lookup"><span data-stu-id="e28c5-132">category</span></span>|<span data-ttu-id="e28c5-133">String</span><span class="sxs-lookup"><span data-stu-id="e28c5-133">String</span></span>|<span data-ttu-id="e28c5-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e28c5-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="e28c5-135">响应</span><span class="sxs-lookup"><span data-stu-id="e28c5-135">Response</span></span>
<span data-ttu-id="e28c5-136">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 String 集合。</span><span class="sxs-lookup"><span data-stu-id="e28c5-136">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e28c5-137">示例</span><span class="sxs-lookup"><span data-stu-id="e28c5-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="e28c5-138">请求</span><span class="sxs-lookup"><span data-stu-id="e28c5-138">Request</span></span>
<span data-ttu-id="e28c5-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e28c5-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/auditEvents/getAuditActivityTypes(category='parameterValue')
```

### <a name="response"></a><span data-ttu-id="e28c5-140">响应</span><span class="sxs-lookup"><span data-stu-id="e28c5-140">Response</span></span>
<span data-ttu-id="e28c5-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e28c5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






