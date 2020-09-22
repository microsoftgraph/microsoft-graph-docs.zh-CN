---
title: getManagedDevicesWithAppFailures 函数
description: 检索具有失败的应用程序的设备的列表
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d98224fa7b2d6ac3b7c868b35e39af3a6e1ebbf3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48004751"
---
# <a name="getmanageddeviceswithappfailures-function"></a><span data-ttu-id="88f76-103">getManagedDevicesWithAppFailures 函数</span><span class="sxs-lookup"><span data-stu-id="88f76-103">getManagedDevicesWithAppFailures function</span></span>

<span data-ttu-id="88f76-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88f76-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="88f76-105">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="88f76-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="88f76-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="88f76-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="88f76-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="88f76-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88f76-108">检索具有失败的应用程序的设备的列表</span><span class="sxs-lookup"><span data-stu-id="88f76-108">Retrieves the list of devices with failed apps</span></span>
## <a name="prerequisites"></a><span data-ttu-id="88f76-109">先决条件</span><span class="sxs-lookup"><span data-stu-id="88f76-109">Prerequisites</span></span>
<span data-ttu-id="88f76-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="88f76-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88f76-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="88f76-112">Permission type</span></span>|<span data-ttu-id="88f76-113">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="88f76-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="88f76-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="88f76-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="88f76-115">&nbsp; &nbsp; **故障排除**</span><span class="sxs-lookup"><span data-stu-id="88f76-115">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="88f76-116">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="88f76-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="88f76-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="88f76-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="88f76-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="88f76-118">Not supported.</span></span>|
|<span data-ttu-id="88f76-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="88f76-119">Application</span></span>||
| <span data-ttu-id="88f76-120">&nbsp; &nbsp; **故障排除**</span><span class="sxs-lookup"><span data-stu-id="88f76-120">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="88f76-121">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="88f76-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="88f76-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="88f76-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedDevicesWithAppFailures
```

## <a name="request-headers"></a><span data-ttu-id="88f76-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="88f76-123">Request headers</span></span>
|<span data-ttu-id="88f76-124">标头</span><span class="sxs-lookup"><span data-stu-id="88f76-124">Header</span></span>|<span data-ttu-id="88f76-125">值</span><span class="sxs-lookup"><span data-stu-id="88f76-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="88f76-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="88f76-126">Authorization</span></span>|<span data-ttu-id="88f76-127">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="88f76-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="88f76-128">接受</span><span class="sxs-lookup"><span data-stu-id="88f76-128">Accept</span></span>|<span data-ttu-id="88f76-129">application/json</span><span class="sxs-lookup"><span data-stu-id="88f76-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="88f76-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="88f76-130">Request body</span></span>
<span data-ttu-id="88f76-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="88f76-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="88f76-132">响应</span><span class="sxs-lookup"><span data-stu-id="88f76-132">Response</span></span>
<span data-ttu-id="88f76-133">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 String 集合。</span><span class="sxs-lookup"><span data-stu-id="88f76-133">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88f76-134">示例</span><span class="sxs-lookup"><span data-stu-id="88f76-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="88f76-135">请求</span><span class="sxs-lookup"><span data-stu-id="88f76-135">Request</span></span>
<span data-ttu-id="88f76-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="88f76-136">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getManagedDevicesWithAppFailures
```

### <a name="response"></a><span data-ttu-id="88f76-137">响应</span><span class="sxs-lookup"><span data-stu-id="88f76-137">Response</span></span>
<span data-ttu-id="88f76-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="88f76-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 74

{
  "value": [
    "Get Managed Devices With App Failures value"
  ]
}
```














