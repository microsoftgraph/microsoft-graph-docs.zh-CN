---
title: 获取 reportRoot
description: 读取 reportRoot 对象的属性和关系。
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9cbc8a52895f64d4a05a1204a15f058e8a87701d
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42800702"
---
# <a name="get-reportroot"></a><span data-ttu-id="699a4-103">获取 reportRoot</span><span class="sxs-lookup"><span data-stu-id="699a4-103">Get reportRoot</span></span>

> <span data-ttu-id="699a4-104">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="699a4-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="699a4-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="699a4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="699a4-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="699a4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="699a4-107">读取 [reportRoot](../resources/intune-shared-reportroot.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="699a4-107">Read properties and relationships of the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="699a4-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="699a4-108">Prerequisites</span></span>
<span data-ttu-id="699a4-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="699a4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="699a4-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="699a4-111">Permission type</span></span>|<span data-ttu-id="699a4-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="699a4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="699a4-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="699a4-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="699a4-114">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="699a4-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="699a4-115">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="699a4-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="699a4-116">&nbsp; &nbsp; **疑难解答**</span><span class="sxs-lookup"><span data-stu-id="699a4-116">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="699a4-117">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="699a4-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="699a4-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="699a4-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="699a4-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="699a4-119">Not supported.</span></span>|
|<span data-ttu-id="699a4-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="699a4-120">Application</span></span>||
| <span data-ttu-id="699a4-121">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="699a4-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="699a4-122">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="699a4-122">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="699a4-123">&nbsp; &nbsp; **疑难解答**</span><span class="sxs-lookup"><span data-stu-id="699a4-123">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="699a4-124">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="699a4-124">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="699a4-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="699a4-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports
```

## <a name="optional-query-parameters"></a><span data-ttu-id="699a4-126">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="699a4-126">Optional query parameters</span></span>
<span data-ttu-id="699a4-127">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="699a4-127">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="699a4-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="699a4-128">Request headers</span></span>
|<span data-ttu-id="699a4-129">标头</span><span class="sxs-lookup"><span data-stu-id="699a4-129">Header</span></span>|<span data-ttu-id="699a4-130">值</span><span class="sxs-lookup"><span data-stu-id="699a4-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="699a4-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="699a4-131">Authorization</span></span>|<span data-ttu-id="699a4-132">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="699a4-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="699a4-133">接受</span><span class="sxs-lookup"><span data-stu-id="699a4-133">Accept</span></span>|<span data-ttu-id="699a4-134">application/json</span><span class="sxs-lookup"><span data-stu-id="699a4-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="699a4-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="699a4-135">Request body</span></span>
<span data-ttu-id="699a4-136">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="699a4-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="699a4-137">响应</span><span class="sxs-lookup"><span data-stu-id="699a4-137">Response</span></span>
<span data-ttu-id="699a4-138">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [reportRoot](../resources/intune-shared-reportroot.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="699a4-138">If successful, this method returns a `200 OK` response code and [reportRoot](../resources/intune-shared-reportroot.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="699a4-139">示例</span><span class="sxs-lookup"><span data-stu-id="699a4-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="699a4-140">请求</span><span class="sxs-lookup"><span data-stu-id="699a4-140">Request</span></span>
<span data-ttu-id="699a4-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="699a4-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports
```

### <a name="response"></a><span data-ttu-id="699a4-142">响应</span><span class="sxs-lookup"><span data-stu-id="699a4-142">Response</span></span>
<span data-ttu-id="699a4-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="699a4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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










