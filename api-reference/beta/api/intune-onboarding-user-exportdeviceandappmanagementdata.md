---
title: exportDeviceAndAppManagementData 函数
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9fd7b9ddcf82ce8ec65e2e58d97ea1a8b08f2ea7
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35741318"
---
# <a name="exportdeviceandappmanagementdata-function"></a><span data-ttu-id="f3654-103">exportDeviceAndAppManagementData 函数</span><span class="sxs-lookup"><span data-stu-id="f3654-103">exportDeviceAndAppManagementData function</span></span>

> <span data-ttu-id="f3654-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f3654-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f3654-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f3654-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3654-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f3654-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f3654-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="f3654-107">Prerequisites</span></span>
<span data-ttu-id="f3654-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f3654-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3654-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f3654-110">Permission type</span></span>|<span data-ttu-id="f3654-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f3654-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f3654-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f3654-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f3654-113">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="f3654-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="f3654-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f3654-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f3654-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f3654-115">Not supported.</span></span>|
|<span data-ttu-id="f3654-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f3654-116">Application</span></span>|<span data-ttu-id="f3654-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="f3654-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f3654-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f3654-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/exportDeviceAndAppManagementData
```

## <a name="request-headers"></a><span data-ttu-id="f3654-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f3654-119">Request headers</span></span>
|<span data-ttu-id="f3654-120">标头</span><span class="sxs-lookup"><span data-stu-id="f3654-120">Header</span></span>|<span data-ttu-id="f3654-121">值</span><span class="sxs-lookup"><span data-stu-id="f3654-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f3654-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f3654-122">Authorization</span></span>|<span data-ttu-id="f3654-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f3654-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f3654-124">接受</span><span class="sxs-lookup"><span data-stu-id="f3654-124">Accept</span></span>|<span data-ttu-id="f3654-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f3654-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3654-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f3654-126">Request body</span></span>
<span data-ttu-id="f3654-127">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="f3654-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="f3654-128">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="f3654-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="f3654-129">属性</span><span class="sxs-lookup"><span data-stu-id="f3654-129">Property</span></span>|<span data-ttu-id="f3654-130">类型</span><span class="sxs-lookup"><span data-stu-id="f3654-130">Type</span></span>|<span data-ttu-id="f3654-131">说明</span><span class="sxs-lookup"><span data-stu-id="f3654-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3654-132">skip</span><span class="sxs-lookup"><span data-stu-id="f3654-132">skip</span></span>|<span data-ttu-id="f3654-133">Int32</span><span class="sxs-lookup"><span data-stu-id="f3654-133">Int32</span></span>|<span data-ttu-id="f3654-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f3654-134">Not yet documented</span></span>|
|<span data-ttu-id="f3654-135">top</span><span class="sxs-lookup"><span data-stu-id="f3654-135">top</span></span>|<span data-ttu-id="f3654-136">Int32</span><span class="sxs-lookup"><span data-stu-id="f3654-136">Int32</span></span>|<span data-ttu-id="f3654-137">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f3654-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="f3654-138">响应</span><span class="sxs-lookup"><span data-stu-id="f3654-138">Response</span></span>
<span data-ttu-id="f3654-139">如果成功, 此函数会在`200 OK`响应正文中返回响应代码和[deviceAndAppManagementData](../resources/intune-onboarding-deviceandappmanagementdata.md) 。</span><span class="sxs-lookup"><span data-stu-id="f3654-139">If successful, this function returns a `200 OK` response code and a [deviceAndAppManagementData](../resources/intune-onboarding-deviceandappmanagementdata.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3654-140">示例</span><span class="sxs-lookup"><span data-stu-id="f3654-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="f3654-141">请求</span><span class="sxs-lookup"><span data-stu-id="f3654-141">Request</span></span>
<span data-ttu-id="f3654-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f3654-142">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/exportDeviceAndAppManagementData(skip=4,top=3)
```

### <a name="response"></a><span data-ttu-id="f3654-143">响应</span><span class="sxs-lookup"><span data-stu-id="f3654-143">Response</span></span>
<span data-ttu-id="f3654-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f3654-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 143

{
  "value": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementData",
    "content": "<Unknown Primitive Type Edm.Stream>"
  }
}
```





