---
title: updateWindowsDeviceAccount 操作
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ed7908abcfb8dec2a5903429e0269c350fbf8471
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759133"
---
# <a name="updatewindowsdeviceaccount-action"></a><span data-ttu-id="831e3-103">updateWindowsDeviceAccount 操作</span><span class="sxs-lookup"><span data-stu-id="831e3-103">updateWindowsDeviceAccount action</span></span>

<span data-ttu-id="831e3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="831e3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="831e3-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="831e3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="831e3-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="831e3-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="831e3-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="831e3-107">Prerequisites</span></span>
<span data-ttu-id="831e3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="831e3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="831e3-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="831e3-110">Permission type</span></span>|<span data-ttu-id="831e3-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="831e3-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="831e3-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="831e3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="831e3-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="831e3-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="831e3-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="831e3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="831e3-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="831e3-115">Not supported.</span></span>|
|<span data-ttu-id="831e3-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="831e3-116">Application</span></span>|<span data-ttu-id="831e3-117">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="831e3-117">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="831e3-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="831e3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/updateWindowsDeviceAccount
POST /deviceManagement/managedDevices/{managedDeviceId}/updateWindowsDeviceAccount
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/updateWindowsDeviceAccount
```

## <a name="request-headers"></a><span data-ttu-id="831e3-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="831e3-119">Request headers</span></span>
|<span data-ttu-id="831e3-120">标头</span><span class="sxs-lookup"><span data-stu-id="831e3-120">Header</span></span>|<span data-ttu-id="831e3-121">值</span><span class="sxs-lookup"><span data-stu-id="831e3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="831e3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="831e3-122">Authorization</span></span>|<span data-ttu-id="831e3-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="831e3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="831e3-124">接受</span><span class="sxs-lookup"><span data-stu-id="831e3-124">Accept</span></span>|<span data-ttu-id="831e3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="831e3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="831e3-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="831e3-126">Request body</span></span>
<span data-ttu-id="831e3-127">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="831e3-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="831e3-128">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="831e3-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="831e3-129">属性</span><span class="sxs-lookup"><span data-stu-id="831e3-129">Property</span></span>|<span data-ttu-id="831e3-130">类型</span><span class="sxs-lookup"><span data-stu-id="831e3-130">Type</span></span>|<span data-ttu-id="831e3-131">说明</span><span class="sxs-lookup"><span data-stu-id="831e3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="831e3-132">updateWindowsDeviceAccountActionParameter</span><span class="sxs-lookup"><span data-stu-id="831e3-132">updateWindowsDeviceAccountActionParameter</span></span>|[<span data-ttu-id="831e3-133">updateWindowsDeviceAccountActionParameter</span><span class="sxs-lookup"><span data-stu-id="831e3-133">updateWindowsDeviceAccountActionParameter</span></span>](../resources/intune-devices-updatewindowsdeviceaccountactionparameter.md)|<span data-ttu-id="831e3-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="831e3-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="831e3-135">响应</span><span class="sxs-lookup"><span data-stu-id="831e3-135">Response</span></span>
<span data-ttu-id="831e3-136">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="831e3-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="831e3-137">示例</span><span class="sxs-lookup"><span data-stu-id="831e3-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="831e3-138">请求</span><span class="sxs-lookup"><span data-stu-id="831e3-138">Request</span></span>
<span data-ttu-id="831e3-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="831e3-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/updateWindowsDeviceAccount

Content-type: application/json
Content-length: 532

{
  "updateWindowsDeviceAccountActionParameter": {
    "@odata.type": "microsoft.graph.updateWindowsDeviceAccountActionParameter",
    "deviceAccount": {
      "@odata.type": "microsoft.graph.windowsDeviceAccount",
      "password": "Password value"
    },
    "passwordRotationEnabled": true,
    "calendarSyncEnabled": true,
    "deviceAccountEmail": "Device Account Email value",
    "exchangeServer": "Exchange Server value",
    "sessionInitiationProtocalAddress": "Session Initiation Protocal Address value"
  }
}
```

### <a name="response"></a><span data-ttu-id="831e3-140">响应</span><span class="sxs-lookup"><span data-stu-id="831e3-140">Response</span></span>
<span data-ttu-id="831e3-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="831e3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




