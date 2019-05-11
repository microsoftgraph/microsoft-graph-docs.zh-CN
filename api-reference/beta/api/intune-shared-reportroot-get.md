---
title: 获取 reportRoot
description: 读取 reportRoot 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 90d347aacefbe177174115433f1f03b6115101bf
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33899067"
---
# <a name="get-reportroot"></a><span data-ttu-id="527c3-103">获取 reportRoot</span><span class="sxs-lookup"><span data-stu-id="527c3-103">Get reportRoot</span></span>

> <span data-ttu-id="527c3-104">**重要说明:** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="527c3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="527c3-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="527c3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="527c3-106">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="527c3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="527c3-107">读取 [reportRoot](../resources/intune-shared-reportroot.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="527c3-107">Read properties and relationships of the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="527c3-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="527c3-108">Prerequisites</span></span>
<span data-ttu-id="527c3-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="527c3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="527c3-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="527c3-111">Permission type</span></span>|<span data-ttu-id="527c3-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="527c3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="527c3-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="527c3-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="527c3-114">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="527c3-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="527c3-115">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="527c3-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="527c3-116">&nbsp; &nbsp; **疑难解答**</span><span class="sxs-lookup"><span data-stu-id="527c3-116">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="527c3-117">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="527c3-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="527c3-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="527c3-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="527c3-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="527c3-119">Not supported.</span></span>|
|<span data-ttu-id="527c3-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="527c3-120">Application</span></span>|<span data-ttu-id="527c3-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="527c3-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="527c3-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="527c3-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports
```

## <a name="optional-query-parameters"></a><span data-ttu-id="527c3-123">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="527c3-123">Optional query parameters</span></span>
<span data-ttu-id="527c3-124">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="527c3-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="527c3-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="527c3-125">Request headers</span></span>
|<span data-ttu-id="527c3-126">标头</span><span class="sxs-lookup"><span data-stu-id="527c3-126">Header</span></span>|<span data-ttu-id="527c3-127">值</span><span class="sxs-lookup"><span data-stu-id="527c3-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="527c3-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="527c3-128">Authorization</span></span>|<span data-ttu-id="527c3-129">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="527c3-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="527c3-130">接受</span><span class="sxs-lookup"><span data-stu-id="527c3-130">Accept</span></span>|<span data-ttu-id="527c3-131">application/json</span><span class="sxs-lookup"><span data-stu-id="527c3-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="527c3-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="527c3-132">Request body</span></span>
<span data-ttu-id="527c3-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="527c3-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="527c3-134">响应</span><span class="sxs-lookup"><span data-stu-id="527c3-134">Response</span></span>
<span data-ttu-id="527c3-135">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [reportRoot](../resources/intune-shared-reportroot.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="527c3-135">If successful, this method returns a `200 OK` response code and [reportRoot](../resources/intune-shared-reportroot.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="527c3-136">示例</span><span class="sxs-lookup"><span data-stu-id="527c3-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="527c3-137">请求</span><span class="sxs-lookup"><span data-stu-id="527c3-137">Request</span></span>
<span data-ttu-id="527c3-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="527c3-138">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports
```

### <a name="response"></a><span data-ttu-id="527c3-139">响应</span><span class="sxs-lookup"><span data-stu-id="527c3-139">Response</span></span>
<span data-ttu-id="527c3-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="527c3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



