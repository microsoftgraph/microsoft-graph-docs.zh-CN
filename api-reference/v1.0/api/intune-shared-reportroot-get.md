---
title: 获取 reportRoot
description: 读取 reportRoot 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b74c970e31c809367b4dc1a1403675e32304d24d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47971095"
---
# <a name="get-reportroot"></a><span data-ttu-id="e3114-103">获取 reportRoot</span><span class="sxs-lookup"><span data-stu-id="e3114-103">Get reportRoot</span></span>

<span data-ttu-id="e3114-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3114-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e3114-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e3114-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e3114-106">读取 [reportRoot](../resources/intune-shared-reportroot.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e3114-106">Read properties and relationships of the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e3114-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="e3114-107">Prerequisites</span></span>
<span data-ttu-id="e3114-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e3114-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3114-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e3114-110">Permission type</span></span>|<span data-ttu-id="e3114-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e3114-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e3114-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e3114-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="e3114-113">&nbsp;&nbsp;设备配置</span><span class="sxs-lookup"><span data-stu-id="e3114-113">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="e3114-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e3114-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="e3114-115">&nbsp;&nbsp;故障排除</span><span class="sxs-lookup"><span data-stu-id="e3114-115">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="e3114-116">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="e3114-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="e3114-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e3114-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e3114-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="e3114-118">Not supported.</span></span>|
|<span data-ttu-id="e3114-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="e3114-119">Application</span></span>|<span data-ttu-id="e3114-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="e3114-120">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e3114-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e3114-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e3114-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e3114-122">Optional query parameters</span></span>
<span data-ttu-id="e3114-123">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e3114-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e3114-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="e3114-124">Request headers</span></span>
|<span data-ttu-id="e3114-125">标头</span><span class="sxs-lookup"><span data-stu-id="e3114-125">Header</span></span>|<span data-ttu-id="e3114-126">值</span><span class="sxs-lookup"><span data-stu-id="e3114-126">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e3114-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3114-127">Authorization</span></span>|<span data-ttu-id="e3114-128">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e3114-128">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e3114-129">接受</span><span class="sxs-lookup"><span data-stu-id="e3114-129">Accept</span></span>|<span data-ttu-id="e3114-130">application/json</span><span class="sxs-lookup"><span data-stu-id="e3114-130">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3114-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="e3114-131">Request body</span></span>
<span data-ttu-id="e3114-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e3114-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e3114-133">响应</span><span class="sxs-lookup"><span data-stu-id="e3114-133">Response</span></span>
<span data-ttu-id="e3114-134">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [reportRoot](../resources/intune-shared-reportroot.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e3114-134">If successful, this method returns a `200 OK` response code and [reportRoot](../resources/intune-shared-reportroot.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3114-135">示例</span><span class="sxs-lookup"><span data-stu-id="e3114-135">Example</span></span>
### <a name="request"></a><span data-ttu-id="e3114-136">请求</span><span class="sxs-lookup"><span data-stu-id="e3114-136">Request</span></span>
<span data-ttu-id="e3114-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e3114-137">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/reports
```

### <a name="response"></a><span data-ttu-id="e3114-138">响应</span><span class="sxs-lookup"><span data-stu-id="e3114-138">Response</span></span>
<span data-ttu-id="e3114-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e3114-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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














