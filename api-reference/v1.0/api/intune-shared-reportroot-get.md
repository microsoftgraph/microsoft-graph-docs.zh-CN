---
title: 获取 reportRoot
description: 读取 reportRoot 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e24a86c1ff4443b0d2867dc9f7da7e273a3012e0
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30251907"
---
# <a name="get-reportroot"></a><span data-ttu-id="5bd1a-103">获取 reportRoot</span><span class="sxs-lookup"><span data-stu-id="5bd1a-103">Get reportRoot</span></span>

> <span data-ttu-id="5bd1a-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5bd1a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5bd1a-105">读取 [reportRoot](../resources/intune-shared-reportroot.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5bd1a-105">Read properties and relationships of the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5bd1a-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="5bd1a-106">Prerequisites</span></span>
<span data-ttu-id="5bd1a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5bd1a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5bd1a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5bd1a-109">Permission type</span></span>|<span data-ttu-id="5bd1a-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5bd1a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5bd1a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5bd1a-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="5bd1a-112">&nbsp;&nbsp;设备配置</span><span class="sxs-lookup"><span data-stu-id="5bd1a-112">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="5bd1a-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5bd1a-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="5bd1a-114">&nbsp;&nbsp;故障排除</span><span class="sxs-lookup"><span data-stu-id="5bd1a-114">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="5bd1a-115">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="5bd1a-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="5bd1a-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5bd1a-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5bd1a-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="5bd1a-117">Not supported.</span></span>|
|<span data-ttu-id="5bd1a-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="5bd1a-118">Application</span></span>|<span data-ttu-id="5bd1a-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="5bd1a-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5bd1a-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5bd1a-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5bd1a-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5bd1a-121">Optional query parameters</span></span>
<span data-ttu-id="5bd1a-122">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="5bd1a-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="5bd1a-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="5bd1a-123">Request headers</span></span>
|<span data-ttu-id="5bd1a-124">标头</span><span class="sxs-lookup"><span data-stu-id="5bd1a-124">Header</span></span>|<span data-ttu-id="5bd1a-125">值</span><span class="sxs-lookup"><span data-stu-id="5bd1a-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5bd1a-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="5bd1a-126">Authorization</span></span>|<span data-ttu-id="5bd1a-127">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5bd1a-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5bd1a-128">Accept</span><span class="sxs-lookup"><span data-stu-id="5bd1a-128">Accept</span></span>|<span data-ttu-id="5bd1a-129">application/json</span><span class="sxs-lookup"><span data-stu-id="5bd1a-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5bd1a-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="5bd1a-130">Request body</span></span>
<span data-ttu-id="5bd1a-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5bd1a-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5bd1a-132">响应</span><span class="sxs-lookup"><span data-stu-id="5bd1a-132">Response</span></span>
<span data-ttu-id="5bd1a-133">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [reportRoot](../resources/intune-shared-reportroot.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5bd1a-133">If successful, this method returns a `200 OK` response code and [reportRoot](../resources/intune-shared-reportroot.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5bd1a-134">示例</span><span class="sxs-lookup"><span data-stu-id="5bd1a-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="5bd1a-135">请求</span><span class="sxs-lookup"><span data-stu-id="5bd1a-135">Request</span></span>
<span data-ttu-id="5bd1a-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5bd1a-136">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/reports
```

### <a name="response"></a><span data-ttu-id="5bd1a-137">响应</span><span class="sxs-lookup"><span data-stu-id="5bd1a-137">Response</span></span>
<span data-ttu-id="5bd1a-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5bd1a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








