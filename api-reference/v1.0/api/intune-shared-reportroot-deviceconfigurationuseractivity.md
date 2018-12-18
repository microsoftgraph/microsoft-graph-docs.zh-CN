---
title: deviceConfigurationUserActivity 函数
description: 设备配置用户活动报告的元数据
author: tfitzmac
ms.openlocfilehash: f19f067212ee6162e2ede9afd325cd80e00af977
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27357041"
---
# <a name="deviceconfigurationuseractivity-function"></a><span data-ttu-id="9f793-103">deviceConfigurationUserActivity 函数</span><span class="sxs-lookup"><span data-stu-id="9f793-103">deviceConfigurationUserActivity function</span></span>

> <span data-ttu-id="9f793-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="9f793-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9f793-105">设备配置用户活动报告的元数据</span><span class="sxs-lookup"><span data-stu-id="9f793-105">Metadata for the device configuration user activity report</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9f793-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="9f793-106">Prerequisites</span></span>
<span data-ttu-id="9f793-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="9f793-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f793-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9f793-109">Permission type</span></span>|<span data-ttu-id="9f793-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9f793-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9f793-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9f793-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="9f793-112">&nbsp;&nbsp;设备配置</span><span class="sxs-lookup"><span data-stu-id="9f793-112">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="9f793-113">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9f793-113">DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="9f793-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9f793-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f793-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9f793-115">Not supported.</span></span>|
|<span data-ttu-id="9f793-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="9f793-116">Application</span></span>|<span data-ttu-id="9f793-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="9f793-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9f793-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9f793-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/deviceConfigurationUserActivity
```

## <a name="request-headers"></a><span data-ttu-id="9f793-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="9f793-119">Request headers</span></span>
|<span data-ttu-id="9f793-120">标头</span><span class="sxs-lookup"><span data-stu-id="9f793-120">Header</span></span>|<span data-ttu-id="9f793-121">值</span><span class="sxs-lookup"><span data-stu-id="9f793-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9f793-122">授权</span><span class="sxs-lookup"><span data-stu-id="9f793-122">Authorization</span></span>|<span data-ttu-id="9f793-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9f793-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9f793-124">Accept</span><span class="sxs-lookup"><span data-stu-id="9f793-124">Accept</span></span>|<span data-ttu-id="9f793-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9f793-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f793-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="9f793-126">Request body</span></span>
<span data-ttu-id="9f793-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9f793-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9f793-128">响应</span><span class="sxs-lookup"><span data-stu-id="9f793-128">Response</span></span>
<span data-ttu-id="9f793-129">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 [report](../resources/intune-shared-report.md)。</span><span class="sxs-lookup"><span data-stu-id="9f793-129">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f793-130">示例</span><span class="sxs-lookup"><span data-stu-id="9f793-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="9f793-131">请求</span><span class="sxs-lookup"><span data-stu-id="9f793-131">Request</span></span>
<span data-ttu-id="9f793-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9f793-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/reports/deviceConfigurationUserActivity
```

### <a name="response"></a><span data-ttu-id="9f793-133">响应</span><span class="sxs-lookup"><span data-stu-id="9f793-133">Response</span></span>
<span data-ttu-id="9f793-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9f793-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








