---
title: getAuditActivityTypes 函数
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3a8151169f1173594be3697e721e89556416e718
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952676"
---
# <a name="getauditactivitytypes-function"></a><span data-ttu-id="88bc6-103">getAuditActivityTypes 函数</span><span class="sxs-lookup"><span data-stu-id="88bc6-103">getAuditActivityTypes function</span></span>

> <span data-ttu-id="88bc6-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="88bc6-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="88bc6-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="88bc6-105">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="88bc6-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="88bc6-106">Prerequisites</span></span>
<span data-ttu-id="88bc6-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="88bc6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88bc6-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="88bc6-109">Permission type</span></span>|<span data-ttu-id="88bc6-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="88bc6-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="88bc6-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="88bc6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="88bc6-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="88bc6-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="88bc6-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="88bc6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="88bc6-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="88bc6-114">Not supported.</span></span>|
|<span data-ttu-id="88bc6-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="88bc6-115">Application</span></span>|<span data-ttu-id="88bc6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="88bc6-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="88bc6-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="88bc6-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents/getAuditActivityTypes
```

## <a name="request-headers"></a><span data-ttu-id="88bc6-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="88bc6-118">Request headers</span></span>
|<span data-ttu-id="88bc6-119">标头</span><span class="sxs-lookup"><span data-stu-id="88bc6-119">Header</span></span>|<span data-ttu-id="88bc6-120">值</span><span class="sxs-lookup"><span data-stu-id="88bc6-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="88bc6-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="88bc6-121">Authorization</span></span>|<span data-ttu-id="88bc6-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="88bc6-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="88bc6-123">Accept</span><span class="sxs-lookup"><span data-stu-id="88bc6-123">Accept</span></span>|<span data-ttu-id="88bc6-124">application/json</span><span class="sxs-lookup"><span data-stu-id="88bc6-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="88bc6-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="88bc6-125">Request body</span></span>
<span data-ttu-id="88bc6-126">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="88bc6-126">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="88bc6-127">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="88bc6-127">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="88bc6-128">属性</span><span class="sxs-lookup"><span data-stu-id="88bc6-128">Property</span></span>|<span data-ttu-id="88bc6-129">类型</span><span class="sxs-lookup"><span data-stu-id="88bc6-129">Type</span></span>|<span data-ttu-id="88bc6-130">说明</span><span class="sxs-lookup"><span data-stu-id="88bc6-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88bc6-131">category</span><span class="sxs-lookup"><span data-stu-id="88bc6-131">category</span></span>|<span data-ttu-id="88bc6-132">String</span><span class="sxs-lookup"><span data-stu-id="88bc6-132">String</span></span>|<span data-ttu-id="88bc6-133">尚未记录</span><span class="sxs-lookup"><span data-stu-id="88bc6-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="88bc6-134">响应</span><span class="sxs-lookup"><span data-stu-id="88bc6-134">Response</span></span>
<span data-ttu-id="88bc6-135">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 String 集合。</span><span class="sxs-lookup"><span data-stu-id="88bc6-135">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88bc6-136">示例</span><span class="sxs-lookup"><span data-stu-id="88bc6-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="88bc6-137">请求</span><span class="sxs-lookup"><span data-stu-id="88bc6-137">Request</span></span>
<span data-ttu-id="88bc6-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="88bc6-138">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/auditEvents/getAuditActivityTypes(category='parameterValue')
```

### <a name="response"></a><span data-ttu-id="88bc6-139">响应</span><span class="sxs-lookup"><span data-stu-id="88bc6-139">Response</span></span>
<span data-ttu-id="88bc6-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="88bc6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



