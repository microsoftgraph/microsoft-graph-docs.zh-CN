---
title: getAuditActivityTypes 函数
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 45ba5a7cf0280e5f54fbbfa00166521ff50e9354
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36015900"
---
# <a name="getauditactivitytypes-function"></a><span data-ttu-id="b9343-103">getAuditActivityTypes 函数</span><span class="sxs-lookup"><span data-stu-id="b9343-103">getAuditActivityTypes function</span></span>

> <span data-ttu-id="b9343-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b9343-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9343-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b9343-105">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b9343-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="b9343-106">Prerequisites</span></span>
<span data-ttu-id="b9343-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b9343-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9343-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b9343-109">Permission type</span></span>|<span data-ttu-id="b9343-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b9343-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b9343-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b9343-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b9343-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9343-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="b9343-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b9343-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b9343-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b9343-114">Not supported.</span></span>|
|<span data-ttu-id="b9343-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b9343-115">Application</span></span>|<span data-ttu-id="b9343-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b9343-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b9343-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b9343-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents/getAuditActivityTypes
```

## <a name="request-headers"></a><span data-ttu-id="b9343-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="b9343-118">Request headers</span></span>
|<span data-ttu-id="b9343-119">标头</span><span class="sxs-lookup"><span data-stu-id="b9343-119">Header</span></span>|<span data-ttu-id="b9343-120">值</span><span class="sxs-lookup"><span data-stu-id="b9343-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b9343-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9343-121">Authorization</span></span>|<span data-ttu-id="b9343-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b9343-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b9343-123">接受</span><span class="sxs-lookup"><span data-stu-id="b9343-123">Accept</span></span>|<span data-ttu-id="b9343-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b9343-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9343-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="b9343-125">Request body</span></span>
<span data-ttu-id="b9343-126">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="b9343-126">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="b9343-127">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="b9343-127">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="b9343-128">属性</span><span class="sxs-lookup"><span data-stu-id="b9343-128">Property</span></span>|<span data-ttu-id="b9343-129">类型</span><span class="sxs-lookup"><span data-stu-id="b9343-129">Type</span></span>|<span data-ttu-id="b9343-130">说明</span><span class="sxs-lookup"><span data-stu-id="b9343-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9343-131">“类别”</span><span class="sxs-lookup"><span data-stu-id="b9343-131">category</span></span>|<span data-ttu-id="b9343-132">String</span><span class="sxs-lookup"><span data-stu-id="b9343-132">String</span></span>|<span data-ttu-id="b9343-133">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b9343-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="b9343-134">响应</span><span class="sxs-lookup"><span data-stu-id="b9343-134">Response</span></span>
<span data-ttu-id="b9343-135">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 String 集合。</span><span class="sxs-lookup"><span data-stu-id="b9343-135">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9343-136">示例</span><span class="sxs-lookup"><span data-stu-id="b9343-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="b9343-137">请求</span><span class="sxs-lookup"><span data-stu-id="b9343-137">Request</span></span>
<span data-ttu-id="b9343-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b9343-138">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/auditEvents/getAuditActivityTypes(category='parameterValue')
```

### <a name="response"></a><span data-ttu-id="b9343-139">响应</span><span class="sxs-lookup"><span data-stu-id="b9343-139">Response</span></span>
<span data-ttu-id="b9343-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b9343-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



