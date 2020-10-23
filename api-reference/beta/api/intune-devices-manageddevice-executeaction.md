---
title: executeAction 操作
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3e64ed7ab003ae340cbcab24bc093843b01e23c0
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48708233"
---
# <a name="executeaction-action"></a><span data-ttu-id="e9fec-103">executeAction 操作</span><span class="sxs-lookup"><span data-stu-id="e9fec-103">executeAction action</span></span>

<span data-ttu-id="e9fec-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e9fec-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e9fec-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e9fec-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e9fec-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e9fec-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e9fec-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e9fec-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e9fec-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="e9fec-108">Prerequisites</span></span>
<span data-ttu-id="e9fec-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e9fec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e9fec-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e9fec-111">Permission type</span></span>|<span data-ttu-id="e9fec-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e9fec-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e9fec-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e9fec-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e9fec-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="e9fec-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="e9fec-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e9fec-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e9fec-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e9fec-116">Not supported.</span></span>|
|<span data-ttu-id="e9fec-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e9fec-117">Application</span></span>|<span data-ttu-id="e9fec-118">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="e9fec-118">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e9fec-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e9fec-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="e9fec-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e9fec-120">Request headers</span></span>
|<span data-ttu-id="e9fec-121">标头</span><span class="sxs-lookup"><span data-stu-id="e9fec-121">Header</span></span>|<span data-ttu-id="e9fec-122">值</span><span class="sxs-lookup"><span data-stu-id="e9fec-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e9fec-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e9fec-123">Authorization</span></span>|<span data-ttu-id="e9fec-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e9fec-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e9fec-125">接受</span><span class="sxs-lookup"><span data-stu-id="e9fec-125">Accept</span></span>|<span data-ttu-id="e9fec-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e9fec-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e9fec-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e9fec-127">Request body</span></span>
<span data-ttu-id="e9fec-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e9fec-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="e9fec-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="e9fec-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="e9fec-130">属性</span><span class="sxs-lookup"><span data-stu-id="e9fec-130">Property</span></span>|<span data-ttu-id="e9fec-131">类型</span><span class="sxs-lookup"><span data-stu-id="e9fec-131">Type</span></span>|<span data-ttu-id="e9fec-132">说明</span><span class="sxs-lookup"><span data-stu-id="e9fec-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e9fec-133">actionName</span><span class="sxs-lookup"><span data-stu-id="e9fec-133">actionName</span></span>|[<span data-ttu-id="e9fec-134">managedDeviceRemoteAction</span><span class="sxs-lookup"><span data-stu-id="e9fec-134">managedDeviceRemoteAction</span></span>](../resources/intune-devices-manageddeviceremoteaction.md)|<span data-ttu-id="e9fec-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e9fec-135">Not yet documented</span></span>|
|<span data-ttu-id="e9fec-136">keepEnrollmentData</span><span class="sxs-lookup"><span data-stu-id="e9fec-136">keepEnrollmentData</span></span>|<span data-ttu-id="e9fec-137">布尔</span><span class="sxs-lookup"><span data-stu-id="e9fec-137">Boolean</span></span>|<span data-ttu-id="e9fec-138">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e9fec-138">Not yet documented</span></span>|
|<span data-ttu-id="e9fec-139">keepUserData</span><span class="sxs-lookup"><span data-stu-id="e9fec-139">keepUserData</span></span>|<span data-ttu-id="e9fec-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="e9fec-140">Boolean</span></span>|<span data-ttu-id="e9fec-141">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e9fec-141">Not yet documented</span></span>|
|<span data-ttu-id="e9fec-142">deviceIds</span><span class="sxs-lookup"><span data-stu-id="e9fec-142">deviceIds</span></span>|<span data-ttu-id="e9fec-143">String collection</span><span class="sxs-lookup"><span data-stu-id="e9fec-143">String collection</span></span>|<span data-ttu-id="e9fec-144">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e9fec-144">Not yet documented</span></span>|
|<span data-ttu-id="e9fec-145">notificationTitle</span><span class="sxs-lookup"><span data-stu-id="e9fec-145">notificationTitle</span></span>|<span data-ttu-id="e9fec-146">String</span><span class="sxs-lookup"><span data-stu-id="e9fec-146">String</span></span>|<span data-ttu-id="e9fec-147">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e9fec-147">Not yet documented</span></span>|
|<span data-ttu-id="e9fec-148">notificationBody</span><span class="sxs-lookup"><span data-stu-id="e9fec-148">notificationBody</span></span>|<span data-ttu-id="e9fec-149">String</span><span class="sxs-lookup"><span data-stu-id="e9fec-149">String</span></span>|<span data-ttu-id="e9fec-150">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e9fec-150">Not yet documented</span></span>|
|<span data-ttu-id="e9fec-151">deviceName</span><span class="sxs-lookup"><span data-stu-id="e9fec-151">deviceName</span></span>|<span data-ttu-id="e9fec-152">String</span><span class="sxs-lookup"><span data-stu-id="e9fec-152">String</span></span>|<span data-ttu-id="e9fec-153">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e9fec-153">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="e9fec-154">响应</span><span class="sxs-lookup"><span data-stu-id="e9fec-154">Response</span></span>
<span data-ttu-id="e9fec-155">如果成功，此操作会 `200 OK` 在响应正文中返回响应代码和 [bulkManagedDeviceActionResult](../resources/intune-devices-bulkmanageddeviceactionresult.md) 。</span><span class="sxs-lookup"><span data-stu-id="e9fec-155">If successful, this action returns a `200 OK` response code and a [bulkManagedDeviceActionResult](../resources/intune-devices-bulkmanageddeviceactionresult.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e9fec-156">示例</span><span class="sxs-lookup"><span data-stu-id="e9fec-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="e9fec-157">请求</span><span class="sxs-lookup"><span data-stu-id="e9fec-157">Request</span></span>
<span data-ttu-id="e9fec-158">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e9fec-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e9fec-159">响应</span><span class="sxs-lookup"><span data-stu-id="e9fec-159">Response</span></span>
<span data-ttu-id="e9fec-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e9fec-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





