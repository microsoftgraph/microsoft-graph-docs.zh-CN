---
title: getAuditActivityTypes 函数
description: 尚未记录
author: tfitzmac
ms.openlocfilehash: c493c688e4782b848b695fb8383dadb882b28ee2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27345981"
---
# <a name="getauditactivitytypes-function"></a><span data-ttu-id="78de8-103">getAuditActivityTypes 函数</span><span class="sxs-lookup"><span data-stu-id="78de8-103">getAuditActivityTypes function</span></span>

> <span data-ttu-id="78de8-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="78de8-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="78de8-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="78de8-105">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="78de8-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="78de8-106">Prerequisites</span></span>
<span data-ttu-id="78de8-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="78de8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78de8-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="78de8-109">Permission type</span></span>|<span data-ttu-id="78de8-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="78de8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="78de8-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="78de8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="78de8-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="78de8-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="78de8-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="78de8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="78de8-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="78de8-114">Not supported.</span></span>|
|<span data-ttu-id="78de8-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="78de8-115">Application</span></span>|<span data-ttu-id="78de8-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="78de8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="78de8-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="78de8-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents/getAuditActivityTypes
```

## <a name="request-headers"></a><span data-ttu-id="78de8-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="78de8-118">Request headers</span></span>
|<span data-ttu-id="78de8-119">标头</span><span class="sxs-lookup"><span data-stu-id="78de8-119">Header</span></span>|<span data-ttu-id="78de8-120">值</span><span class="sxs-lookup"><span data-stu-id="78de8-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="78de8-121">授权</span><span class="sxs-lookup"><span data-stu-id="78de8-121">Authorization</span></span>|<span data-ttu-id="78de8-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="78de8-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="78de8-123">Accept</span><span class="sxs-lookup"><span data-stu-id="78de8-123">Accept</span></span>|<span data-ttu-id="78de8-124">application/json</span><span class="sxs-lookup"><span data-stu-id="78de8-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="78de8-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="78de8-125">Request body</span></span>
<span data-ttu-id="78de8-126">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="78de8-126">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="78de8-127">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="78de8-127">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="78de8-128">属性</span><span class="sxs-lookup"><span data-stu-id="78de8-128">Property</span></span>|<span data-ttu-id="78de8-129">类型</span><span class="sxs-lookup"><span data-stu-id="78de8-129">Type</span></span>|<span data-ttu-id="78de8-130">说明</span><span class="sxs-lookup"><span data-stu-id="78de8-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78de8-131">category</span><span class="sxs-lookup"><span data-stu-id="78de8-131">category</span></span>|<span data-ttu-id="78de8-132">String</span><span class="sxs-lookup"><span data-stu-id="78de8-132">String</span></span>|<span data-ttu-id="78de8-133">尚未记录</span><span class="sxs-lookup"><span data-stu-id="78de8-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="78de8-134">响应</span><span class="sxs-lookup"><span data-stu-id="78de8-134">Response</span></span>
<span data-ttu-id="78de8-135">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 String 集合。</span><span class="sxs-lookup"><span data-stu-id="78de8-135">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="78de8-136">示例</span><span class="sxs-lookup"><span data-stu-id="78de8-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="78de8-137">请求</span><span class="sxs-lookup"><span data-stu-id="78de8-137">Request</span></span>
<span data-ttu-id="78de8-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="78de8-138">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/auditEvents/getAuditActivityTypes(category='parameterValue')
```

### <a name="response"></a><span data-ttu-id="78de8-139">响应</span><span class="sxs-lookup"><span data-stu-id="78de8-139">Response</span></span>
<span data-ttu-id="78de8-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="78de8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



