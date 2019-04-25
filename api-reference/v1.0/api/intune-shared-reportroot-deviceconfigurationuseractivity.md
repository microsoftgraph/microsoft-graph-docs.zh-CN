---
title: deviceConfigurationUserActivity 函数
description: 设备配置用户活动报告的元数据
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5c83c9a6216e678d16af212f6a31648f7dea8a2b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32576921"
---
# <a name="deviceconfigurationuseractivity-function"></a><span data-ttu-id="65d1c-103">deviceConfigurationUserActivity 函数</span><span class="sxs-lookup"><span data-stu-id="65d1c-103">deviceConfigurationUserActivity function</span></span>

> <span data-ttu-id="65d1c-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="65d1c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65d1c-105">设备配置用户活动报告的元数据</span><span class="sxs-lookup"><span data-stu-id="65d1c-105">Metadata for the device configuration user activity report</span></span>

## <a name="prerequisites"></a><span data-ttu-id="65d1c-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="65d1c-106">Prerequisites</span></span>
<span data-ttu-id="65d1c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="65d1c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65d1c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="65d1c-109">Permission type</span></span>|<span data-ttu-id="65d1c-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="65d1c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="65d1c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="65d1c-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="65d1c-112">&nbsp;&nbsp;设备配置</span><span class="sxs-lookup"><span data-stu-id="65d1c-112">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="65d1c-113">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="65d1c-113">DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="65d1c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="65d1c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="65d1c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="65d1c-115">Not supported.</span></span>|
|<span data-ttu-id="65d1c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="65d1c-116">Application</span></span>|<span data-ttu-id="65d1c-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="65d1c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="65d1c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="65d1c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/deviceConfigurationUserActivity
```

## <a name="request-headers"></a><span data-ttu-id="65d1c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="65d1c-119">Request headers</span></span>
|<span data-ttu-id="65d1c-120">标头</span><span class="sxs-lookup"><span data-stu-id="65d1c-120">Header</span></span>|<span data-ttu-id="65d1c-121">值</span><span class="sxs-lookup"><span data-stu-id="65d1c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="65d1c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="65d1c-122">Authorization</span></span>|<span data-ttu-id="65d1c-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="65d1c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="65d1c-124">接受</span><span class="sxs-lookup"><span data-stu-id="65d1c-124">Accept</span></span>|<span data-ttu-id="65d1c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="65d1c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="65d1c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="65d1c-126">Request body</span></span>
<span data-ttu-id="65d1c-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="65d1c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="65d1c-128">响应</span><span class="sxs-lookup"><span data-stu-id="65d1c-128">Response</span></span>
<span data-ttu-id="65d1c-129">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 [report](../resources/intune-shared-report.md)。</span><span class="sxs-lookup"><span data-stu-id="65d1c-129">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65d1c-130">示例</span><span class="sxs-lookup"><span data-stu-id="65d1c-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="65d1c-131">请求</span><span class="sxs-lookup"><span data-stu-id="65d1c-131">Request</span></span>
<span data-ttu-id="65d1c-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="65d1c-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/reports/deviceConfigurationUserActivity
```

### <a name="response"></a><span data-ttu-id="65d1c-133">响应</span><span class="sxs-lookup"><span data-stu-id="65d1c-133">Response</span></span>
<span data-ttu-id="65d1c-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="65d1c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








