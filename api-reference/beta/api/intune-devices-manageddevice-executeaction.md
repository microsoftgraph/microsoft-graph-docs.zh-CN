---
title: executeAction 操作
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 933ab0a4171e45e67e900eb995667f722ed03c17
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37529906"
---
# <a name="executeaction-action"></a><span data-ttu-id="64396-103">executeAction 操作</span><span class="sxs-lookup"><span data-stu-id="64396-103">executeAction action</span></span>

> <span data-ttu-id="64396-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="64396-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="64396-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="64396-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64396-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="64396-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="64396-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="64396-107">Prerequisites</span></span>
<span data-ttu-id="64396-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="64396-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64396-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="64396-110">Permission type</span></span>|<span data-ttu-id="64396-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="64396-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="64396-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="64396-112">Delegated (work or school account)</span></span>|<span data-ttu-id="64396-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="64396-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="64396-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="64396-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="64396-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="64396-115">Not supported.</span></span>|
|<span data-ttu-id="64396-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="64396-116">Application</span></span>|<span data-ttu-id="64396-117">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="64396-117">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="64396-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="64396-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/executeAction
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/executeAction
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/executeAction
```

## <a name="request-headers"></a><span data-ttu-id="64396-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="64396-119">Request headers</span></span>
|<span data-ttu-id="64396-120">标头</span><span class="sxs-lookup"><span data-stu-id="64396-120">Header</span></span>|<span data-ttu-id="64396-121">值</span><span class="sxs-lookup"><span data-stu-id="64396-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="64396-122">授权</span><span class="sxs-lookup"><span data-stu-id="64396-122">Authorization</span></span>|<span data-ttu-id="64396-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="64396-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="64396-124">接受</span><span class="sxs-lookup"><span data-stu-id="64396-124">Accept</span></span>|<span data-ttu-id="64396-125">application/json</span><span class="sxs-lookup"><span data-stu-id="64396-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="64396-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="64396-126">Request body</span></span>
<span data-ttu-id="64396-127">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="64396-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="64396-128">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="64396-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="64396-129">属性</span><span class="sxs-lookup"><span data-stu-id="64396-129">Property</span></span>|<span data-ttu-id="64396-130">类型</span><span class="sxs-lookup"><span data-stu-id="64396-130">Type</span></span>|<span data-ttu-id="64396-131">说明</span><span class="sxs-lookup"><span data-stu-id="64396-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64396-132">actionName</span><span class="sxs-lookup"><span data-stu-id="64396-132">actionName</span></span>|[<span data-ttu-id="64396-133">managedDeviceRemoteAction</span><span class="sxs-lookup"><span data-stu-id="64396-133">managedDeviceRemoteAction</span></span>](../resources/intune-devices-manageddeviceremoteaction.md)|<span data-ttu-id="64396-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="64396-134">Not yet documented</span></span>|
|<span data-ttu-id="64396-135">keepEnrollmentData</span><span class="sxs-lookup"><span data-stu-id="64396-135">keepEnrollmentData</span></span>|<span data-ttu-id="64396-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="64396-136">Boolean</span></span>|<span data-ttu-id="64396-137">尚未记录</span><span class="sxs-lookup"><span data-stu-id="64396-137">Not yet documented</span></span>|
|<span data-ttu-id="64396-138">keepUserData</span><span class="sxs-lookup"><span data-stu-id="64396-138">keepUserData</span></span>|<span data-ttu-id="64396-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="64396-139">Boolean</span></span>|<span data-ttu-id="64396-140">尚未记录</span><span class="sxs-lookup"><span data-stu-id="64396-140">Not yet documented</span></span>|
|<span data-ttu-id="64396-141">deviceIds</span><span class="sxs-lookup"><span data-stu-id="64396-141">deviceIds</span></span>|<span data-ttu-id="64396-142">String collection</span><span class="sxs-lookup"><span data-stu-id="64396-142">String collection</span></span>|<span data-ttu-id="64396-143">尚未记录</span><span class="sxs-lookup"><span data-stu-id="64396-143">Not yet documented</span></span>|
|<span data-ttu-id="64396-144">notificationTitle</span><span class="sxs-lookup"><span data-stu-id="64396-144">notificationTitle</span></span>|<span data-ttu-id="64396-145">String</span><span class="sxs-lookup"><span data-stu-id="64396-145">String</span></span>|<span data-ttu-id="64396-146">尚未记录</span><span class="sxs-lookup"><span data-stu-id="64396-146">Not yet documented</span></span>|
|<span data-ttu-id="64396-147">notificationBody</span><span class="sxs-lookup"><span data-stu-id="64396-147">notificationBody</span></span>|<span data-ttu-id="64396-148">String</span><span class="sxs-lookup"><span data-stu-id="64396-148">String</span></span>|<span data-ttu-id="64396-149">尚未记录</span><span class="sxs-lookup"><span data-stu-id="64396-149">Not yet documented</span></span>|
|<span data-ttu-id="64396-150">deviceName</span><span class="sxs-lookup"><span data-stu-id="64396-150">deviceName</span></span>|<span data-ttu-id="64396-151">String</span><span class="sxs-lookup"><span data-stu-id="64396-151">String</span></span>|<span data-ttu-id="64396-152">尚未记录</span><span class="sxs-lookup"><span data-stu-id="64396-152">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="64396-153">响应</span><span class="sxs-lookup"><span data-stu-id="64396-153">Response</span></span>
<span data-ttu-id="64396-154">如果成功，此操作会在`200 OK`响应正文中返回响应代码和[bulkManagedDeviceActionResult](../resources/intune-devices-bulkmanageddeviceactionresult.md) 。</span><span class="sxs-lookup"><span data-stu-id="64396-154">If successful, this action returns a `200 OK` response code and a [bulkManagedDeviceActionResult](../resources/intune-devices-bulkmanageddeviceactionresult.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64396-155">示例</span><span class="sxs-lookup"><span data-stu-id="64396-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="64396-156">请求</span><span class="sxs-lookup"><span data-stu-id="64396-156">Request</span></span>
<span data-ttu-id="64396-157">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="64396-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="64396-158">响应</span><span class="sxs-lookup"><span data-stu-id="64396-158">Response</span></span>
<span data-ttu-id="64396-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="64396-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






