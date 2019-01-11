---
title: 获取 reportRoot
description: 读取 reportRoot 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: dbf15ec9aab222c52c9fdcefaf3265bd1588dfd5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27850440"
---
# <a name="get-reportroot"></a><span data-ttu-id="73310-103">获取 reportRoot</span><span class="sxs-lookup"><span data-stu-id="73310-103">Get reportRoot</span></span>

> <span data-ttu-id="73310-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="73310-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="73310-105">读取 [reportRoot](../resources/intune-shared-reportroot.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="73310-105">Read properties and relationships of the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="73310-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="73310-106">Prerequisites</span></span>
<span data-ttu-id="73310-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="73310-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73310-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="73310-109">Permission type</span></span>|<span data-ttu-id="73310-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="73310-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="73310-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="73310-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="73310-112">&nbsp;&nbsp;设备配置</span><span class="sxs-lookup"><span data-stu-id="73310-112">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="73310-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="73310-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="73310-114">&nbsp;&nbsp;疑难解答</span><span class="sxs-lookup"><span data-stu-id="73310-114">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="73310-115">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="73310-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="73310-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="73310-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="73310-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="73310-117">Not supported.</span></span>|
|<span data-ttu-id="73310-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="73310-118">Application</span></span>|<span data-ttu-id="73310-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="73310-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="73310-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="73310-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports
```

## <a name="optional-query-parameters"></a><span data-ttu-id="73310-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="73310-121">Optional query parameters</span></span>
<span data-ttu-id="73310-122">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="73310-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="73310-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="73310-123">Request headers</span></span>
|<span data-ttu-id="73310-124">标头</span><span class="sxs-lookup"><span data-stu-id="73310-124">Header</span></span>|<span data-ttu-id="73310-125">值</span><span class="sxs-lookup"><span data-stu-id="73310-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="73310-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="73310-126">Authorization</span></span>|<span data-ttu-id="73310-127">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="73310-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="73310-128">Accept</span><span class="sxs-lookup"><span data-stu-id="73310-128">Accept</span></span>|<span data-ttu-id="73310-129">application/json</span><span class="sxs-lookup"><span data-stu-id="73310-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="73310-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="73310-130">Request body</span></span>
<span data-ttu-id="73310-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="73310-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="73310-132">响应</span><span class="sxs-lookup"><span data-stu-id="73310-132">Response</span></span>
<span data-ttu-id="73310-133">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [reportRoot](../resources/intune-shared-reportroot.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="73310-133">If successful, this method returns a `200 OK` response code and [reportRoot](../resources/intune-shared-reportroot.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73310-134">示例</span><span class="sxs-lookup"><span data-stu-id="73310-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="73310-135">请求</span><span class="sxs-lookup"><span data-stu-id="73310-135">Request</span></span>
<span data-ttu-id="73310-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="73310-136">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/reports
```

### <a name="response"></a><span data-ttu-id="73310-137">响应</span><span class="sxs-lookup"><span data-stu-id="73310-137">Response</span></span>
<span data-ttu-id="73310-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="73310-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 124

{
  "value": {
    "@odata.type": "#microsoft.graph.reportRoot",
    "id": "9ab6b3dd-b3dd-9ab6-ddb3-b69addb3b69a"
  }
}
```








