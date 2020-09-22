---
title: deviceConfigurationUserActivity 函数
description: 设备配置用户活动报告的元数据
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9ed6adadb0c40e51db1b4e83489555f85156ef4f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48087262"
---
# <a name="deviceconfigurationuseractivity-function"></a><span data-ttu-id="c9488-103">deviceConfigurationUserActivity 函数</span><span class="sxs-lookup"><span data-stu-id="c9488-103">deviceConfigurationUserActivity function</span></span>

<span data-ttu-id="c9488-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c9488-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c9488-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c9488-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c9488-106">设备配置用户活动报告的元数据</span><span class="sxs-lookup"><span data-stu-id="c9488-106">Metadata for the device configuration user activity report</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c9488-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="c9488-107">Prerequisites</span></span>
<span data-ttu-id="c9488-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c9488-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9488-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c9488-110">Permission type</span></span>|<span data-ttu-id="c9488-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c9488-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c9488-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c9488-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="c9488-113">&nbsp;&nbsp;设备配置</span><span class="sxs-lookup"><span data-stu-id="c9488-113">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="c9488-114">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c9488-114">DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c9488-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c9488-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c9488-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c9488-116">Not supported.</span></span>|
|<span data-ttu-id="c9488-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c9488-117">Application</span></span>|<span data-ttu-id="c9488-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="c9488-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c9488-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c9488-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/deviceConfigurationUserActivity
```

## <a name="request-headers"></a><span data-ttu-id="c9488-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c9488-120">Request headers</span></span>
|<span data-ttu-id="c9488-121">标头</span><span class="sxs-lookup"><span data-stu-id="c9488-121">Header</span></span>|<span data-ttu-id="c9488-122">值</span><span class="sxs-lookup"><span data-stu-id="c9488-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c9488-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c9488-123">Authorization</span></span>|<span data-ttu-id="c9488-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c9488-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c9488-125">接受</span><span class="sxs-lookup"><span data-stu-id="c9488-125">Accept</span></span>|<span data-ttu-id="c9488-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c9488-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c9488-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c9488-127">Request body</span></span>
<span data-ttu-id="c9488-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c9488-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c9488-129">响应</span><span class="sxs-lookup"><span data-stu-id="c9488-129">Response</span></span>
<span data-ttu-id="c9488-130">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 [report](../resources/intune-shared-report.md)。</span><span class="sxs-lookup"><span data-stu-id="c9488-130">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9488-131">示例</span><span class="sxs-lookup"><span data-stu-id="c9488-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="c9488-132">请求</span><span class="sxs-lookup"><span data-stu-id="c9488-132">Request</span></span>
<span data-ttu-id="c9488-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c9488-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/reports/deviceConfigurationUserActivity
```

### <a name="response"></a><span data-ttu-id="c9488-134">响应</span><span class="sxs-lookup"><span data-stu-id="c9488-134">Response</span></span>
<span data-ttu-id="c9488-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c9488-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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














