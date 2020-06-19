---
title: updateWindowsDeviceAccount 操作
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 52ddeb86f69ddc781633ffa87a02f261575c6791
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792140"
---
# <a name="updatewindowsdeviceaccount-action"></a><span data-ttu-id="c0edb-103">updateWindowsDeviceAccount 操作</span><span class="sxs-lookup"><span data-stu-id="c0edb-103">updateWindowsDeviceAccount action</span></span>

<span data-ttu-id="c0edb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0edb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c0edb-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c0edb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c0edb-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c0edb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0edb-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c0edb-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c0edb-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="c0edb-108">Prerequisites</span></span>
<span data-ttu-id="c0edb-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="c0edb-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="c0edb-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0edb-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0edb-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c0edb-111">Permission type</span></span>|<span data-ttu-id="c0edb-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c0edb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c0edb-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c0edb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c0edb-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="c0edb-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="c0edb-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c0edb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c0edb-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c0edb-116">Not supported.</span></span>|
|<span data-ttu-id="c0edb-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c0edb-117">Application</span></span>|<span data-ttu-id="c0edb-118">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="c0edb-118">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c0edb-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c0edb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/updateWindowsDeviceAccount
POST /deviceManagement/comanagedDevices/{managedDeviceId}/updateWindowsDeviceAccount
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice/updateWindowsDeviceAccount
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/updateWindowsDeviceAccount
POST /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates/{deviceComplianceScriptDeviceStateId}/managedDevice/updateWindowsDeviceAccount
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/updateWindowsDeviceAccount
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/updateWindowsDeviceAccount
```

## <a name="request-headers"></a><span data-ttu-id="c0edb-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c0edb-120">Request headers</span></span>
|<span data-ttu-id="c0edb-121">标头</span><span class="sxs-lookup"><span data-stu-id="c0edb-121">Header</span></span>|<span data-ttu-id="c0edb-122">值</span><span class="sxs-lookup"><span data-stu-id="c0edb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c0edb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0edb-123">Authorization</span></span>|<span data-ttu-id="c0edb-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c0edb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c0edb-125">接受</span><span class="sxs-lookup"><span data-stu-id="c0edb-125">Accept</span></span>|<span data-ttu-id="c0edb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c0edb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0edb-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c0edb-127">Request body</span></span>
<span data-ttu-id="c0edb-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c0edb-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="c0edb-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="c0edb-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="c0edb-130">属性</span><span class="sxs-lookup"><span data-stu-id="c0edb-130">Property</span></span>|<span data-ttu-id="c0edb-131">类型</span><span class="sxs-lookup"><span data-stu-id="c0edb-131">Type</span></span>|<span data-ttu-id="c0edb-132">说明</span><span class="sxs-lookup"><span data-stu-id="c0edb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0edb-133">updateWindowsDeviceAccountActionParameter</span><span class="sxs-lookup"><span data-stu-id="c0edb-133">updateWindowsDeviceAccountActionParameter</span></span>|[<span data-ttu-id="c0edb-134">updateWindowsDeviceAccountActionParameter</span><span class="sxs-lookup"><span data-stu-id="c0edb-134">updateWindowsDeviceAccountActionParameter</span></span>](../resources/intune-devices-updatewindowsdeviceaccountactionparameter.md)|<span data-ttu-id="c0edb-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c0edb-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="c0edb-136">响应</span><span class="sxs-lookup"><span data-stu-id="c0edb-136">Response</span></span>
<span data-ttu-id="c0edb-137">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="c0edb-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c0edb-138">示例</span><span class="sxs-lookup"><span data-stu-id="c0edb-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="c0edb-139">请求</span><span class="sxs-lookup"><span data-stu-id="c0edb-139">Request</span></span>
<span data-ttu-id="c0edb-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c0edb-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/updateWindowsDeviceAccount

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

### <a name="response"></a><span data-ttu-id="c0edb-141">响应</span><span class="sxs-lookup"><span data-stu-id="c0edb-141">Response</span></span>
<span data-ttu-id="c0edb-142">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="c0edb-142">Here is an example of the response.</span></span> <span data-ttu-id="c0edb-143">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="c0edb-143">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="c0edb-144">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="c0edb-144">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



