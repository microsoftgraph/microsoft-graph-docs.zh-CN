---
title: 获取 managedAppStatusRaw
description: 读取 managedAppStatusRaw 对象的属性和关系。
ms.openlocfilehash: acaa8b7dd98a58c934731b871e4b8b078034f3ec
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27011645"
---
# <a name="get-managedappstatusraw"></a><span data-ttu-id="949b7-103">获取 managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="949b7-103">Get managedAppStatusRaw</span></span>

> <span data-ttu-id="949b7-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="949b7-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="949b7-105">读取 [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="949b7-105">Read properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="949b7-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="949b7-106">Prerequisites</span></span>
<span data-ttu-id="949b7-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="949b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="949b7-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="949b7-109">Permission type</span></span>|<span data-ttu-id="949b7-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="949b7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="949b7-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="949b7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="949b7-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="949b7-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="949b7-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="949b7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="949b7-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="949b7-114">Not supported.</span></span>|
|<span data-ttu-id="949b7-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="949b7-115">Application</span></span>|<span data-ttu-id="949b7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="949b7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="949b7-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="949b7-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppStatuses/{managedAppStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="949b7-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="949b7-118">Optional query parameters</span></span>
<span data-ttu-id="949b7-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="949b7-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="949b7-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="949b7-120">Request headers</span></span>
|<span data-ttu-id="949b7-121">标头</span><span class="sxs-lookup"><span data-stu-id="949b7-121">Header</span></span>|<span data-ttu-id="949b7-122">值</span><span class="sxs-lookup"><span data-stu-id="949b7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="949b7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="949b7-123">Authorization</span></span>|<span data-ttu-id="949b7-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="949b7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="949b7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="949b7-125">Accept</span></span>|<span data-ttu-id="949b7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="949b7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="949b7-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="949b7-127">Request body</span></span>
<span data-ttu-id="949b7-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="949b7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="949b7-129">响应</span><span class="sxs-lookup"><span data-stu-id="949b7-129">Response</span></span>
<span data-ttu-id="949b7-130">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="949b7-130">If successful, this method returns a `200 OK` response code and [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="949b7-131">示例</span><span class="sxs-lookup"><span data-stu-id="949b7-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="949b7-132">请求</span><span class="sxs-lookup"><span data-stu-id="949b7-132">Request</span></span>
<span data-ttu-id="949b7-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="949b7-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppStatuses/{managedAppStatusId}
```

### <a name="response"></a><span data-ttu-id="949b7-134">响应</span><span class="sxs-lookup"><span data-stu-id="949b7-134">Response</span></span>
<span data-ttu-id="949b7-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="949b7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 279

{
  "value": {
    "@odata.type": "#microsoft.graph.managedAppStatusRaw",
    "displayName": "Display Name value",
    "id": "80847581-7581-8084-8175-848081758480",
    "version": "Version value",
    "content": {
      "@odata.type": "microsoft.graph.Json"
    }
  }
}
```



