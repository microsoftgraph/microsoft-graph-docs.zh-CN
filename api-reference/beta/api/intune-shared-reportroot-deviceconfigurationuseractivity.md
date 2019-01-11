---
title: deviceConfigurationUserActivity 函数
description: 设备配置用户活动报告的元数据
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 4b403fa45e228d1393127943dcbf9011b91ab18f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27806361"
---
# <a name="deviceconfigurationuseractivity-function"></a><span data-ttu-id="a8e91-103">deviceConfigurationUserActivity 函数</span><span class="sxs-lookup"><span data-stu-id="a8e91-103">deviceConfigurationUserActivity function</span></span>

> <span data-ttu-id="a8e91-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a8e91-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a8e91-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a8e91-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a8e91-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="a8e91-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a8e91-107">设备配置用户活动报告的元数据</span><span class="sxs-lookup"><span data-stu-id="a8e91-107">Metadata for the device configuration user activity report</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a8e91-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="a8e91-108">Prerequisites</span></span>
<span data-ttu-id="a8e91-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="a8e91-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8e91-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a8e91-111">Permission type</span></span>|<span data-ttu-id="a8e91-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a8e91-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a8e91-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a8e91-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="a8e91-114">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="a8e91-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="a8e91-115">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a8e91-115">DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a8e91-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a8e91-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a8e91-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="a8e91-117">Not supported.</span></span>|
|<span data-ttu-id="a8e91-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="a8e91-118">Application</span></span>|<span data-ttu-id="a8e91-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="a8e91-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a8e91-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a8e91-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/deviceConfigurationUserActivity
```

## <a name="request-headers"></a><span data-ttu-id="a8e91-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="a8e91-121">Request headers</span></span>
|<span data-ttu-id="a8e91-122">标头</span><span class="sxs-lookup"><span data-stu-id="a8e91-122">Header</span></span>|<span data-ttu-id="a8e91-123">值</span><span class="sxs-lookup"><span data-stu-id="a8e91-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a8e91-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a8e91-124">Authorization</span></span>|<span data-ttu-id="a8e91-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a8e91-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a8e91-126">Accept</span><span class="sxs-lookup"><span data-stu-id="a8e91-126">Accept</span></span>|<span data-ttu-id="a8e91-127">application/json</span><span class="sxs-lookup"><span data-stu-id="a8e91-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a8e91-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="a8e91-128">Request body</span></span>
<span data-ttu-id="a8e91-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a8e91-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a8e91-130">响应</span><span class="sxs-lookup"><span data-stu-id="a8e91-130">Response</span></span>
<span data-ttu-id="a8e91-131">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 [report](../resources/intune-shared-report.md)。</span><span class="sxs-lookup"><span data-stu-id="a8e91-131">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8e91-132">示例</span><span class="sxs-lookup"><span data-stu-id="a8e91-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="a8e91-133">请求</span><span class="sxs-lookup"><span data-stu-id="a8e91-133">Request</span></span>
<span data-ttu-id="a8e91-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a8e91-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/deviceConfigurationUserActivity
```

### <a name="response"></a><span data-ttu-id="a8e91-135">响应</span><span class="sxs-lookup"><span data-stu-id="a8e91-135">Response</span></span>
<span data-ttu-id="a8e91-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a8e91-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 123

{
  "value": {
    "@odata.type": "microsoft.graph.report",
    "content": "<Unknown Primitive Type Edm.Stream>"
  }
}
```



