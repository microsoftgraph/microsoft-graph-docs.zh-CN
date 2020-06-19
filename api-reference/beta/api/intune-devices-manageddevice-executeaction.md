---
title: executeAction 操作
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1b16beb4e8a40c674e3c1a95d937d21893df595e
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792294"
---
# <a name="executeaction-action"></a><span data-ttu-id="d70f0-103">executeAction 操作</span><span class="sxs-lookup"><span data-stu-id="d70f0-103">executeAction action</span></span>

<span data-ttu-id="d70f0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d70f0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d70f0-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d70f0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d70f0-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d70f0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d70f0-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d70f0-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d70f0-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="d70f0-108">Prerequisites</span></span>
<span data-ttu-id="d70f0-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="d70f0-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="d70f0-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d70f0-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d70f0-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d70f0-111">Permission type</span></span>|<span data-ttu-id="d70f0-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d70f0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d70f0-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d70f0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d70f0-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="d70f0-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="d70f0-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d70f0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d70f0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d70f0-116">Not supported.</span></span>|
|<span data-ttu-id="d70f0-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d70f0-117">Application</span></span>|<span data-ttu-id="d70f0-118">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="d70f0-118">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d70f0-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d70f0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/executeAction
POST /deviceManagement/comanagedDevices/executeAction
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/executeAction
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/executeAction
```

## <a name="request-headers"></a><span data-ttu-id="d70f0-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d70f0-120">Request headers</span></span>
|<span data-ttu-id="d70f0-121">标头</span><span class="sxs-lookup"><span data-stu-id="d70f0-121">Header</span></span>|<span data-ttu-id="d70f0-122">值</span><span class="sxs-lookup"><span data-stu-id="d70f0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d70f0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d70f0-123">Authorization</span></span>|<span data-ttu-id="d70f0-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d70f0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d70f0-125">接受</span><span class="sxs-lookup"><span data-stu-id="d70f0-125">Accept</span></span>|<span data-ttu-id="d70f0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d70f0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d70f0-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d70f0-127">Request body</span></span>
<span data-ttu-id="d70f0-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d70f0-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="d70f0-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="d70f0-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="d70f0-130">属性</span><span class="sxs-lookup"><span data-stu-id="d70f0-130">Property</span></span>|<span data-ttu-id="d70f0-131">类型</span><span class="sxs-lookup"><span data-stu-id="d70f0-131">Type</span></span>|<span data-ttu-id="d70f0-132">说明</span><span class="sxs-lookup"><span data-stu-id="d70f0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d70f0-133">actionName</span><span class="sxs-lookup"><span data-stu-id="d70f0-133">actionName</span></span>|[<span data-ttu-id="d70f0-134">managedDeviceRemoteAction</span><span class="sxs-lookup"><span data-stu-id="d70f0-134">managedDeviceRemoteAction</span></span>](../resources/intune-devices-manageddeviceremoteaction.md)|<span data-ttu-id="d70f0-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d70f0-135">Not yet documented</span></span>|
|<span data-ttu-id="d70f0-136">keepEnrollmentData</span><span class="sxs-lookup"><span data-stu-id="d70f0-136">keepEnrollmentData</span></span>|<span data-ttu-id="d70f0-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="d70f0-137">Boolean</span></span>|<span data-ttu-id="d70f0-138">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d70f0-138">Not yet documented</span></span>|
|<span data-ttu-id="d70f0-139">keepUserData</span><span class="sxs-lookup"><span data-stu-id="d70f0-139">keepUserData</span></span>|<span data-ttu-id="d70f0-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="d70f0-140">Boolean</span></span>|<span data-ttu-id="d70f0-141">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d70f0-141">Not yet documented</span></span>|
|<span data-ttu-id="d70f0-142">deviceIds</span><span class="sxs-lookup"><span data-stu-id="d70f0-142">deviceIds</span></span>|<span data-ttu-id="d70f0-143">String collection</span><span class="sxs-lookup"><span data-stu-id="d70f0-143">String collection</span></span>|<span data-ttu-id="d70f0-144">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d70f0-144">Not yet documented</span></span>|
|<span data-ttu-id="d70f0-145">notificationTitle</span><span class="sxs-lookup"><span data-stu-id="d70f0-145">notificationTitle</span></span>|<span data-ttu-id="d70f0-146">String</span><span class="sxs-lookup"><span data-stu-id="d70f0-146">String</span></span>|<span data-ttu-id="d70f0-147">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d70f0-147">Not yet documented</span></span>|
|<span data-ttu-id="d70f0-148">notificationBody</span><span class="sxs-lookup"><span data-stu-id="d70f0-148">notificationBody</span></span>|<span data-ttu-id="d70f0-149">String</span><span class="sxs-lookup"><span data-stu-id="d70f0-149">String</span></span>|<span data-ttu-id="d70f0-150">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d70f0-150">Not yet documented</span></span>|
|<span data-ttu-id="d70f0-151">deviceName</span><span class="sxs-lookup"><span data-stu-id="d70f0-151">deviceName</span></span>|<span data-ttu-id="d70f0-152">String</span><span class="sxs-lookup"><span data-stu-id="d70f0-152">String</span></span>|<span data-ttu-id="d70f0-153">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d70f0-153">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="d70f0-154">响应</span><span class="sxs-lookup"><span data-stu-id="d70f0-154">Response</span></span>
<span data-ttu-id="d70f0-155">如果成功，此操作会 `200 OK` 在响应正文中返回响应代码和[bulkManagedDeviceActionResult](../resources/intune-devices-bulkmanageddeviceactionresult.md) 。</span><span class="sxs-lookup"><span data-stu-id="d70f0-155">If successful, this action returns a `200 OK` response code and a [bulkManagedDeviceActionResult](../resources/intune-devices-bulkmanageddeviceactionresult.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d70f0-156">示例</span><span class="sxs-lookup"><span data-stu-id="d70f0-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="d70f0-157">请求</span><span class="sxs-lookup"><span data-stu-id="d70f0-157">Request</span></span>
<span data-ttu-id="d70f0-158">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d70f0-158">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/executeAction

Content-type: application/json
Content-length: 274

{
  "actionName": "delete",
  "keepEnrollmentData": true,
  "keepUserData": true,
  "deviceIds": [
    "Device Ids value"
  ],
  "notificationTitle": "Notification Title value",
  "notificationBody": "Notification Body value",
  "deviceName": "Device Name value"
}
```

### <a name="response"></a><span data-ttu-id="d70f0-159">响应</span><span class="sxs-lookup"><span data-stu-id="d70f0-159">Response</span></span>
<span data-ttu-id="d70f0-160">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="d70f0-160">Here is an example of the response.</span></span> <span data-ttu-id="d70f0-161">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="d70f0-161">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="d70f0-162">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="d70f0-162">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 385

{
  "value": {
    "@odata.type": "microsoft.graph.bulkManagedDeviceActionResult",
    "successfulDeviceIds": [
      "Successful Device Ids value"
    ],
    "failedDeviceIds": [
      "Failed Device Ids value"
    ],
    "notFoundDeviceIds": [
      "Not Found Device Ids value"
    ],
    "notSupportedDeviceIds": [
      "Not Supported Device Ids value"
    ]
  }
}
```



