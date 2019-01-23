---
title: 获取 reportRoot
description: 读取 reportRoot 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ecfdc13e5e4cdfea5a8c3c9cfb40fe9d6872bd92
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402928"
---
# <a name="get-reportroot"></a><span data-ttu-id="126c2-103">获取 reportRoot</span><span class="sxs-lookup"><span data-stu-id="126c2-103">Get reportRoot</span></span>

> <span data-ttu-id="126c2-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="126c2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="126c2-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="126c2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="126c2-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="126c2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="126c2-107">读取 [reportRoot](../resources/intune-shared-reportroot.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="126c2-107">Read properties and relationships of the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="126c2-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="126c2-108">Prerequisites</span></span>
<span data-ttu-id="126c2-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="126c2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="126c2-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="126c2-111">Permission type</span></span>|<span data-ttu-id="126c2-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="126c2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="126c2-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="126c2-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="126c2-114">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="126c2-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="126c2-115">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="126c2-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="126c2-116">&nbsp; &nbsp; **疑难解答**</span><span class="sxs-lookup"><span data-stu-id="126c2-116">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="126c2-117">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="126c2-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="126c2-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="126c2-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="126c2-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="126c2-119">Not supported.</span></span>|
|<span data-ttu-id="126c2-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="126c2-120">Application</span></span>|<span data-ttu-id="126c2-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="126c2-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="126c2-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="126c2-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports
```

## <a name="optional-query-parameters"></a><span data-ttu-id="126c2-123">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="126c2-123">Optional query parameters</span></span>
<span data-ttu-id="126c2-124">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="126c2-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="126c2-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="126c2-125">Request headers</span></span>
|<span data-ttu-id="126c2-126">标头</span><span class="sxs-lookup"><span data-stu-id="126c2-126">Header</span></span>|<span data-ttu-id="126c2-127">值</span><span class="sxs-lookup"><span data-stu-id="126c2-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="126c2-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="126c2-128">Authorization</span></span>|<span data-ttu-id="126c2-129">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="126c2-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="126c2-130">Accept</span><span class="sxs-lookup"><span data-stu-id="126c2-130">Accept</span></span>|<span data-ttu-id="126c2-131">application/json</span><span class="sxs-lookup"><span data-stu-id="126c2-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="126c2-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="126c2-132">Request body</span></span>
<span data-ttu-id="126c2-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="126c2-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="126c2-134">响应</span><span class="sxs-lookup"><span data-stu-id="126c2-134">Response</span></span>
<span data-ttu-id="126c2-135">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [reportRoot](../resources/intune-shared-reportroot.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="126c2-135">If successful, this method returns a `200 OK` response code and [reportRoot](../resources/intune-shared-reportroot.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="126c2-136">示例</span><span class="sxs-lookup"><span data-stu-id="126c2-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="126c2-137">请求</span><span class="sxs-lookup"><span data-stu-id="126c2-137">Request</span></span>
<span data-ttu-id="126c2-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="126c2-138">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports
```

### <a name="response"></a><span data-ttu-id="126c2-139">响应</span><span class="sxs-lookup"><span data-stu-id="126c2-139">Response</span></span>
<span data-ttu-id="126c2-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="126c2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



