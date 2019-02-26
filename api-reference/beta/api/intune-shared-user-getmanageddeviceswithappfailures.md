---
title: getManagedDevicesWithAppFailures 函数
description: 检索具有失败的应用程序的设备的列表
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 44296ba60db476bd7c407ea4fbbc727ffca465ca
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172210"
---
# <a name="getmanageddeviceswithappfailures-function"></a><span data-ttu-id="a1ffe-103">getManagedDevicesWithAppFailures 函数</span><span class="sxs-lookup"><span data-stu-id="a1ffe-103">getManagedDevicesWithAppFailures function</span></span>

> <span data-ttu-id="a1ffe-104">**重要说明:** Microsoft Graph 中的/beta 版本下的 api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a1ffe-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a1ffe-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a1ffe-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a1ffe-106">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a1ffe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1ffe-107">检索具有失败的应用程序的设备的列表</span><span class="sxs-lookup"><span data-stu-id="a1ffe-107">Retrieves the list of devices with failed apps</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a1ffe-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="a1ffe-108">Prerequisites</span></span>
<span data-ttu-id="a1ffe-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a1ffe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference).</span></span>

|<span data-ttu-id="a1ffe-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a1ffe-111">Permission type</span></span>|<span data-ttu-id="a1ffe-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a1ffe-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1ffe-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a1ffe-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="a1ffe-114">&nbsp; &nbsp; **疑难解答**</span><span class="sxs-lookup"><span data-stu-id="a1ffe-114">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="a1ffe-115">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="a1ffe-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="a1ffe-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a1ffe-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1ffe-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="a1ffe-117">Not supported.</span></span>|
|<span data-ttu-id="a1ffe-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="a1ffe-118">Application</span></span>|<span data-ttu-id="a1ffe-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="a1ffe-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1ffe-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a1ffe-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedDevicesWithAppFailures
```

## <a name="request-headers"></a><span data-ttu-id="a1ffe-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="a1ffe-121">Request headers</span></span>
|<span data-ttu-id="a1ffe-122">标头</span><span class="sxs-lookup"><span data-stu-id="a1ffe-122">Header</span></span>|<span data-ttu-id="a1ffe-123">值</span><span class="sxs-lookup"><span data-stu-id="a1ffe-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a1ffe-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a1ffe-124">Authorization</span></span>|<span data-ttu-id="a1ffe-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a1ffe-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a1ffe-126">Accept</span><span class="sxs-lookup"><span data-stu-id="a1ffe-126">Accept</span></span>|<span data-ttu-id="a1ffe-127">application/json</span><span class="sxs-lookup"><span data-stu-id="a1ffe-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1ffe-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="a1ffe-128">Request body</span></span>
<span data-ttu-id="a1ffe-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a1ffe-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a1ffe-130">响应</span><span class="sxs-lookup"><span data-stu-id="a1ffe-130">Response</span></span>
<span data-ttu-id="a1ffe-131">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 String 集合。</span><span class="sxs-lookup"><span data-stu-id="a1ffe-131">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1ffe-132">示例</span><span class="sxs-lookup"><span data-stu-id="a1ffe-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="a1ffe-133">请求</span><span class="sxs-lookup"><span data-stu-id="a1ffe-133">Request</span></span>
<span data-ttu-id="a1ffe-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a1ffe-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getManagedDevicesWithAppFailures
```

### <a name="response"></a><span data-ttu-id="a1ffe-135">响应</span><span class="sxs-lookup"><span data-stu-id="a1ffe-135">Response</span></span>
<span data-ttu-id="a1ffe-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a1ffe-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





