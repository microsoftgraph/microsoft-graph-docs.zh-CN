---
title: executeAction 操作
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5efd0e372e876f5be30b87956cbb7c25a5da621d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43324876"
---
# <a name="executeaction-action"></a><span data-ttu-id="94f62-103">executeAction 操作</span><span class="sxs-lookup"><span data-stu-id="94f62-103">executeAction action</span></span>

<span data-ttu-id="94f62-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="94f62-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="94f62-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="94f62-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="94f62-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="94f62-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="94f62-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="94f62-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="94f62-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="94f62-108">Prerequisites</span></span>
<span data-ttu-id="94f62-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="94f62-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94f62-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="94f62-111">Permission type</span></span>|<span data-ttu-id="94f62-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="94f62-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="94f62-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="94f62-113">Delegated (work or school account)</span></span>|<span data-ttu-id="94f62-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="94f62-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="94f62-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="94f62-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="94f62-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="94f62-116">Not supported.</span></span>|
|<span data-ttu-id="94f62-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="94f62-117">Application</span></span>|<span data-ttu-id="94f62-118">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="94f62-118">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="94f62-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="94f62-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/executeAction
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/executeAction
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/executeAction
```

## <a name="request-headers"></a><span data-ttu-id="94f62-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="94f62-120">Request headers</span></span>
|<span data-ttu-id="94f62-121">标头</span><span class="sxs-lookup"><span data-stu-id="94f62-121">Header</span></span>|<span data-ttu-id="94f62-122">值</span><span class="sxs-lookup"><span data-stu-id="94f62-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="94f62-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="94f62-123">Authorization</span></span>|<span data-ttu-id="94f62-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="94f62-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="94f62-125">接受</span><span class="sxs-lookup"><span data-stu-id="94f62-125">Accept</span></span>|<span data-ttu-id="94f62-126">application/json</span><span class="sxs-lookup"><span data-stu-id="94f62-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="94f62-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="94f62-127">Request body</span></span>
<span data-ttu-id="94f62-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="94f62-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="94f62-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="94f62-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="94f62-130">属性</span><span class="sxs-lookup"><span data-stu-id="94f62-130">Property</span></span>|<span data-ttu-id="94f62-131">类型</span><span class="sxs-lookup"><span data-stu-id="94f62-131">Type</span></span>|<span data-ttu-id="94f62-132">说明</span><span class="sxs-lookup"><span data-stu-id="94f62-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94f62-133">actionName</span><span class="sxs-lookup"><span data-stu-id="94f62-133">actionName</span></span>|[<span data-ttu-id="94f62-134">managedDeviceRemoteAction</span><span class="sxs-lookup"><span data-stu-id="94f62-134">managedDeviceRemoteAction</span></span>](../resources/intune-devices-manageddeviceremoteaction.md)|<span data-ttu-id="94f62-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="94f62-135">Not yet documented</span></span>|
|<span data-ttu-id="94f62-136">keepEnrollmentData</span><span class="sxs-lookup"><span data-stu-id="94f62-136">keepEnrollmentData</span></span>|<span data-ttu-id="94f62-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="94f62-137">Boolean</span></span>|<span data-ttu-id="94f62-138">尚未记录</span><span class="sxs-lookup"><span data-stu-id="94f62-138">Not yet documented</span></span>|
|<span data-ttu-id="94f62-139">keepUserData</span><span class="sxs-lookup"><span data-stu-id="94f62-139">keepUserData</span></span>|<span data-ttu-id="94f62-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="94f62-140">Boolean</span></span>|<span data-ttu-id="94f62-141">尚未记录</span><span class="sxs-lookup"><span data-stu-id="94f62-141">Not yet documented</span></span>|
|<span data-ttu-id="94f62-142">deviceIds</span><span class="sxs-lookup"><span data-stu-id="94f62-142">deviceIds</span></span>|<span data-ttu-id="94f62-143">String collection</span><span class="sxs-lookup"><span data-stu-id="94f62-143">String collection</span></span>|<span data-ttu-id="94f62-144">尚未记录</span><span class="sxs-lookup"><span data-stu-id="94f62-144">Not yet documented</span></span>|
|<span data-ttu-id="94f62-145">notificationTitle</span><span class="sxs-lookup"><span data-stu-id="94f62-145">notificationTitle</span></span>|<span data-ttu-id="94f62-146">String</span><span class="sxs-lookup"><span data-stu-id="94f62-146">String</span></span>|<span data-ttu-id="94f62-147">尚未记录</span><span class="sxs-lookup"><span data-stu-id="94f62-147">Not yet documented</span></span>|
|<span data-ttu-id="94f62-148">notificationBody</span><span class="sxs-lookup"><span data-stu-id="94f62-148">notificationBody</span></span>|<span data-ttu-id="94f62-149">String</span><span class="sxs-lookup"><span data-stu-id="94f62-149">String</span></span>|<span data-ttu-id="94f62-150">尚未记录</span><span class="sxs-lookup"><span data-stu-id="94f62-150">Not yet documented</span></span>|
|<span data-ttu-id="94f62-151">deviceName</span><span class="sxs-lookup"><span data-stu-id="94f62-151">deviceName</span></span>|<span data-ttu-id="94f62-152">String</span><span class="sxs-lookup"><span data-stu-id="94f62-152">String</span></span>|<span data-ttu-id="94f62-153">尚未记录</span><span class="sxs-lookup"><span data-stu-id="94f62-153">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="94f62-154">响应</span><span class="sxs-lookup"><span data-stu-id="94f62-154">Response</span></span>
<span data-ttu-id="94f62-155">如果成功，此操作会在`200 OK`响应正文中返回响应代码和[bulkManagedDeviceActionResult](../resources/intune-devices-bulkmanageddeviceactionresult.md) 。</span><span class="sxs-lookup"><span data-stu-id="94f62-155">If successful, this action returns a `200 OK` response code and a [bulkManagedDeviceActionResult](../resources/intune-devices-bulkmanageddeviceactionresult.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="94f62-156">示例</span><span class="sxs-lookup"><span data-stu-id="94f62-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="94f62-157">请求</span><span class="sxs-lookup"><span data-stu-id="94f62-157">Request</span></span>
<span data-ttu-id="94f62-158">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="94f62-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="94f62-159">响应</span><span class="sxs-lookup"><span data-stu-id="94f62-159">Response</span></span>
<span data-ttu-id="94f62-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="94f62-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



