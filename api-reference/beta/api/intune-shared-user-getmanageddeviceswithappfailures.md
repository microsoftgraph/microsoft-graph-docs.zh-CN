---
title: getManagedDevicesWithAppFailures 函数
description: 检索具有失败的应用程序的设备的列表
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5796100578a66899c69152d0bdb65ffe42675e34
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/09/2019
ms.locfileid: "38085540"
---
# <a name="getmanageddeviceswithappfailures-function"></a><span data-ttu-id="1616f-103">getManagedDevicesWithAppFailures 函数</span><span class="sxs-lookup"><span data-stu-id="1616f-103">getManagedDevicesWithAppFailures function</span></span>

> <span data-ttu-id="1616f-104">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="1616f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1616f-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1616f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1616f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1616f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1616f-107">检索具有失败的应用程序的设备的列表</span><span class="sxs-lookup"><span data-stu-id="1616f-107">Retrieves the list of devices with failed apps</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1616f-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="1616f-108">Prerequisites</span></span>
<span data-ttu-id="1616f-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1616f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1616f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="1616f-111">Permission type</span></span>|<span data-ttu-id="1616f-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1616f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1616f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1616f-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="1616f-114">&nbsp; &nbsp; **故障排除**</span><span class="sxs-lookup"><span data-stu-id="1616f-114">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="1616f-115">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="1616f-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="1616f-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1616f-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1616f-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="1616f-117">Not supported.</span></span>|
|<span data-ttu-id="1616f-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="1616f-118">Application</span></span>||
| <span data-ttu-id="1616f-119">&nbsp; &nbsp; **故障排除**</span><span class="sxs-lookup"><span data-stu-id="1616f-119">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="1616f-120">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="1616f-120">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1616f-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1616f-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedDevicesWithAppFailures
```

## <a name="request-headers"></a><span data-ttu-id="1616f-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="1616f-122">Request headers</span></span>
|<span data-ttu-id="1616f-123">标头</span><span class="sxs-lookup"><span data-stu-id="1616f-123">Header</span></span>|<span data-ttu-id="1616f-124">值</span><span class="sxs-lookup"><span data-stu-id="1616f-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1616f-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="1616f-125">Authorization</span></span>|<span data-ttu-id="1616f-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1616f-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1616f-127">接受</span><span class="sxs-lookup"><span data-stu-id="1616f-127">Accept</span></span>|<span data-ttu-id="1616f-128">application/json</span><span class="sxs-lookup"><span data-stu-id="1616f-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1616f-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="1616f-129">Request body</span></span>
<span data-ttu-id="1616f-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1616f-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1616f-131">响应</span><span class="sxs-lookup"><span data-stu-id="1616f-131">Response</span></span>
<span data-ttu-id="1616f-132">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 String 集合。</span><span class="sxs-lookup"><span data-stu-id="1616f-132">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1616f-133">示例</span><span class="sxs-lookup"><span data-stu-id="1616f-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="1616f-134">请求</span><span class="sxs-lookup"><span data-stu-id="1616f-134">Request</span></span>
<span data-ttu-id="1616f-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1616f-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getManagedDevicesWithAppFailures
```

### <a name="response"></a><span data-ttu-id="1616f-136">响应</span><span class="sxs-lookup"><span data-stu-id="1616f-136">Response</span></span>
<span data-ttu-id="1616f-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1616f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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














