---
title: deviceConfigurationDeviceActivity 函数
description: 设备配置设备活动报告的元数据
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a92ca929c45e9da34e598df079197fd76a2761bd
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30262095"
---
# <a name="deviceconfigurationdeviceactivity-function"></a><span data-ttu-id="6a7ec-103">deviceConfigurationDeviceActivity 函数</span><span class="sxs-lookup"><span data-stu-id="6a7ec-103">deviceConfigurationDeviceActivity function</span></span>

> <span data-ttu-id="6a7ec-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6a7ec-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a7ec-105">设备配置设备活动报告的元数据</span><span class="sxs-lookup"><span data-stu-id="6a7ec-105">Metadata for the device configuration device activity report</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6a7ec-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="6a7ec-106">Prerequisites</span></span>
<span data-ttu-id="6a7ec-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6a7ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a7ec-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6a7ec-109">Permission type</span></span>|<span data-ttu-id="6a7ec-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6a7ec-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6a7ec-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6a7ec-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="6a7ec-112">&nbsp;&nbsp;设备配置</span><span class="sxs-lookup"><span data-stu-id="6a7ec-112">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="6a7ec-113">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6a7ec-113">DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="6a7ec-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6a7ec-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6a7ec-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6a7ec-115">Not supported.</span></span>|
|<span data-ttu-id="6a7ec-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="6a7ec-116">Application</span></span>|<span data-ttu-id="6a7ec-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="6a7ec-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6a7ec-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6a7ec-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/deviceConfigurationDeviceActivity
```

## <a name="request-headers"></a><span data-ttu-id="6a7ec-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="6a7ec-119">Request headers</span></span>
|<span data-ttu-id="6a7ec-120">标头</span><span class="sxs-lookup"><span data-stu-id="6a7ec-120">Header</span></span>|<span data-ttu-id="6a7ec-121">值</span><span class="sxs-lookup"><span data-stu-id="6a7ec-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6a7ec-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6a7ec-122">Authorization</span></span>|<span data-ttu-id="6a7ec-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6a7ec-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6a7ec-124">Accept</span><span class="sxs-lookup"><span data-stu-id="6a7ec-124">Accept</span></span>|<span data-ttu-id="6a7ec-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6a7ec-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a7ec-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="6a7ec-126">Request body</span></span>
<span data-ttu-id="6a7ec-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6a7ec-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6a7ec-128">响应</span><span class="sxs-lookup"><span data-stu-id="6a7ec-128">Response</span></span>
<span data-ttu-id="6a7ec-129">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 [report](../resources/intune-shared-report.md)。</span><span class="sxs-lookup"><span data-stu-id="6a7ec-129">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a7ec-130">示例</span><span class="sxs-lookup"><span data-stu-id="6a7ec-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="6a7ec-131">请求</span><span class="sxs-lookup"><span data-stu-id="6a7ec-131">Request</span></span>
<span data-ttu-id="6a7ec-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6a7ec-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/reports/deviceConfigurationDeviceActivity
```

### <a name="response"></a><span data-ttu-id="6a7ec-133">响应</span><span class="sxs-lookup"><span data-stu-id="6a7ec-133">Response</span></span>
<span data-ttu-id="6a7ec-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6a7ec-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








