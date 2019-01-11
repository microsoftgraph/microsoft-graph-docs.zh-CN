---
title: deviceConfigurationDeviceActivity 函数
description: 设备配置设备活动报告的元数据
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 7bbe0531df6f4a975fd9192838339ca424650c04
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27867702"
---
# <a name="deviceconfigurationdeviceactivity-function"></a><span data-ttu-id="8a200-103">deviceConfigurationDeviceActivity 函数</span><span class="sxs-lookup"><span data-stu-id="8a200-103">deviceConfigurationDeviceActivity function</span></span>

> <span data-ttu-id="8a200-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="8a200-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8a200-105">设备配置设备活动报告的元数据</span><span class="sxs-lookup"><span data-stu-id="8a200-105">Metadata for the device configuration device activity report</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8a200-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="8a200-106">Prerequisites</span></span>
<span data-ttu-id="8a200-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="8a200-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a200-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8a200-109">Permission type</span></span>|<span data-ttu-id="8a200-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8a200-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8a200-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8a200-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="8a200-112">&nbsp;&nbsp;设备配置</span><span class="sxs-lookup"><span data-stu-id="8a200-112">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="8a200-113">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8a200-113">DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="8a200-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8a200-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8a200-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8a200-115">Not supported.</span></span>|
|<span data-ttu-id="8a200-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="8a200-116">Application</span></span>|<span data-ttu-id="8a200-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="8a200-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8a200-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8a200-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/deviceConfigurationDeviceActivity
```

## <a name="request-headers"></a><span data-ttu-id="8a200-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="8a200-119">Request headers</span></span>
|<span data-ttu-id="8a200-120">标头</span><span class="sxs-lookup"><span data-stu-id="8a200-120">Header</span></span>|<span data-ttu-id="8a200-121">值</span><span class="sxs-lookup"><span data-stu-id="8a200-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8a200-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8a200-122">Authorization</span></span>|<span data-ttu-id="8a200-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8a200-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8a200-124">Accept</span><span class="sxs-lookup"><span data-stu-id="8a200-124">Accept</span></span>|<span data-ttu-id="8a200-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8a200-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8a200-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="8a200-126">Request body</span></span>
<span data-ttu-id="8a200-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8a200-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8a200-128">响应</span><span class="sxs-lookup"><span data-stu-id="8a200-128">Response</span></span>
<span data-ttu-id="8a200-129">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 [report](../resources/intune-shared-report.md)。</span><span class="sxs-lookup"><span data-stu-id="8a200-129">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8a200-130">示例</span><span class="sxs-lookup"><span data-stu-id="8a200-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="8a200-131">请求</span><span class="sxs-lookup"><span data-stu-id="8a200-131">Request</span></span>
<span data-ttu-id="8a200-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8a200-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/reports/deviceConfigurationDeviceActivity
```

### <a name="response"></a><span data-ttu-id="8a200-133">响应</span><span class="sxs-lookup"><span data-stu-id="8a200-133">Response</span></span>
<span data-ttu-id="8a200-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8a200-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








