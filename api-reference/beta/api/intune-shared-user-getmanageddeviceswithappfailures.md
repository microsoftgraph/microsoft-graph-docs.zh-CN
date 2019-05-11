---
title: getManagedDevicesWithAppFailures 函数
description: 检索具有失败的应用程序的设备的列表
author: rolyon
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 96d58ab7be68c7ba63f84bf686337230c9c5c11e
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33897798"
---
# <a name="getmanageddeviceswithappfailures-function"></a><span data-ttu-id="ab35d-103">getManagedDevicesWithAppFailures 函数</span><span class="sxs-lookup"><span data-stu-id="ab35d-103">getManagedDevicesWithAppFailures function</span></span>

> <span data-ttu-id="ab35d-104">**重要说明:** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ab35d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ab35d-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ab35d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ab35d-106">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ab35d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ab35d-107">检索具有失败的应用程序的设备的列表</span><span class="sxs-lookup"><span data-stu-id="ab35d-107">Retrieves the list of devices with failed apps</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ab35d-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="ab35d-108">Prerequisites</span></span>
<span data-ttu-id="ab35d-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ab35d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab35d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ab35d-111">Permission type</span></span>|<span data-ttu-id="ab35d-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ab35d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ab35d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ab35d-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="ab35d-114">&nbsp; &nbsp; **疑难解答**</span><span class="sxs-lookup"><span data-stu-id="ab35d-114">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="ab35d-115">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="ab35d-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="ab35d-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ab35d-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ab35d-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="ab35d-117">Not supported.</span></span>|
|<span data-ttu-id="ab35d-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="ab35d-118">Application</span></span>|<span data-ttu-id="ab35d-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="ab35d-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ab35d-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ab35d-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedDevicesWithAppFailures
```

## <a name="request-headers"></a><span data-ttu-id="ab35d-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="ab35d-121">Request headers</span></span>
|<span data-ttu-id="ab35d-122">标头</span><span class="sxs-lookup"><span data-stu-id="ab35d-122">Header</span></span>|<span data-ttu-id="ab35d-123">值</span><span class="sxs-lookup"><span data-stu-id="ab35d-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ab35d-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ab35d-124">Authorization</span></span>|<span data-ttu-id="ab35d-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ab35d-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ab35d-126">接受</span><span class="sxs-lookup"><span data-stu-id="ab35d-126">Accept</span></span>|<span data-ttu-id="ab35d-127">application/json</span><span class="sxs-lookup"><span data-stu-id="ab35d-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ab35d-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="ab35d-128">Request body</span></span>
<span data-ttu-id="ab35d-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ab35d-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ab35d-130">响应</span><span class="sxs-lookup"><span data-stu-id="ab35d-130">Response</span></span>
<span data-ttu-id="ab35d-131">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 String 集合。</span><span class="sxs-lookup"><span data-stu-id="ab35d-131">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab35d-132">示例</span><span class="sxs-lookup"><span data-stu-id="ab35d-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="ab35d-133">请求</span><span class="sxs-lookup"><span data-stu-id="ab35d-133">Request</span></span>
<span data-ttu-id="ab35d-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ab35d-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getManagedDevicesWithAppFailures
```

### <a name="response"></a><span data-ttu-id="ab35d-135">响应</span><span class="sxs-lookup"><span data-stu-id="ab35d-135">Response</span></span>
<span data-ttu-id="ab35d-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ab35d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





