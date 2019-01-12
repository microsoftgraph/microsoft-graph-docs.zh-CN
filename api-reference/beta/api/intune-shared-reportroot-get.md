---
title: 获取 reportRoot
description: 读取 reportRoot 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3ae57e5bd5638e41ab6c6acfda810fe64d04a461
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27954244"
---
# <a name="get-reportroot"></a><span data-ttu-id="d1708-103">获取 reportRoot</span><span class="sxs-lookup"><span data-stu-id="d1708-103">Get reportRoot</span></span>

> <span data-ttu-id="d1708-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d1708-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d1708-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d1708-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d1708-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d1708-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d1708-107">读取 [reportRoot](../resources/intune-shared-reportroot.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d1708-107">Read properties and relationships of the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d1708-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="d1708-108">Prerequisites</span></span>
<span data-ttu-id="d1708-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="d1708-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1708-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d1708-111">Permission type</span></span>|<span data-ttu-id="d1708-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d1708-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d1708-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d1708-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="d1708-114">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="d1708-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="d1708-115">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d1708-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="d1708-116">&nbsp; &nbsp; **疑难解答**</span><span class="sxs-lookup"><span data-stu-id="d1708-116">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="d1708-117">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="d1708-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="d1708-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d1708-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d1708-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="d1708-119">Not supported.</span></span>|
|<span data-ttu-id="d1708-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="d1708-120">Application</span></span>|<span data-ttu-id="d1708-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="d1708-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d1708-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d1708-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d1708-123">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d1708-123">Optional query parameters</span></span>
<span data-ttu-id="d1708-124">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d1708-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d1708-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="d1708-125">Request headers</span></span>
|<span data-ttu-id="d1708-126">标头</span><span class="sxs-lookup"><span data-stu-id="d1708-126">Header</span></span>|<span data-ttu-id="d1708-127">值</span><span class="sxs-lookup"><span data-stu-id="d1708-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d1708-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="d1708-128">Authorization</span></span>|<span data-ttu-id="d1708-129">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d1708-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d1708-130">Accept</span><span class="sxs-lookup"><span data-stu-id="d1708-130">Accept</span></span>|<span data-ttu-id="d1708-131">application/json</span><span class="sxs-lookup"><span data-stu-id="d1708-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d1708-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="d1708-132">Request body</span></span>
<span data-ttu-id="d1708-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d1708-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d1708-134">响应</span><span class="sxs-lookup"><span data-stu-id="d1708-134">Response</span></span>
<span data-ttu-id="d1708-135">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [reportRoot](../resources/intune-shared-reportroot.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d1708-135">If successful, this method returns a `200 OK` response code and [reportRoot](../resources/intune-shared-reportroot.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1708-136">示例</span><span class="sxs-lookup"><span data-stu-id="d1708-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="d1708-137">请求</span><span class="sxs-lookup"><span data-stu-id="d1708-137">Request</span></span>
<span data-ttu-id="d1708-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d1708-138">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports
```

### <a name="response"></a><span data-ttu-id="d1708-139">响应</span><span class="sxs-lookup"><span data-stu-id="d1708-139">Response</span></span>
<span data-ttu-id="d1708-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d1708-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



