---
title: executeAction 操作
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 95b6a2a27913d0b51935644609067d00b1304b9c
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51150057"
---
# <a name="executeaction-action"></a><span data-ttu-id="5cc1a-103">executeAction 操作</span><span class="sxs-lookup"><span data-stu-id="5cc1a-103">executeAction action</span></span>

<span data-ttu-id="5cc1a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5cc1a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5cc1a-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5cc1a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5cc1a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5cc1a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5cc1a-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="5cc1a-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5cc1a-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="5cc1a-108">Prerequisites</span></span>
<span data-ttu-id="5cc1a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5cc1a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5cc1a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="5cc1a-111">Permission type</span></span>|<span data-ttu-id="5cc1a-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5cc1a-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5cc1a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5cc1a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5cc1a-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="5cc1a-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="5cc1a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5cc1a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5cc1a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5cc1a-116">Not supported.</span></span>|
|<span data-ttu-id="5cc1a-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="5cc1a-117">Application</span></span>|<span data-ttu-id="5cc1a-118">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="5cc1a-118">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5cc1a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5cc1a-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="5cc1a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="5cc1a-120">Request headers</span></span>
|<span data-ttu-id="5cc1a-121">标头</span><span class="sxs-lookup"><span data-stu-id="5cc1a-121">Header</span></span>|<span data-ttu-id="5cc1a-122">值</span><span class="sxs-lookup"><span data-stu-id="5cc1a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5cc1a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5cc1a-123">Authorization</span></span>|<span data-ttu-id="5cc1a-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5cc1a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5cc1a-125">接受</span><span class="sxs-lookup"><span data-stu-id="5cc1a-125">Accept</span></span>|<span data-ttu-id="5cc1a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5cc1a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5cc1a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="5cc1a-127">Request body</span></span>
<span data-ttu-id="5cc1a-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5cc1a-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="5cc1a-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="5cc1a-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="5cc1a-130">属性</span><span class="sxs-lookup"><span data-stu-id="5cc1a-130">Property</span></span>|<span data-ttu-id="5cc1a-131">类型</span><span class="sxs-lookup"><span data-stu-id="5cc1a-131">Type</span></span>|<span data-ttu-id="5cc1a-132">说明</span><span class="sxs-lookup"><span data-stu-id="5cc1a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5cc1a-133">actionName</span><span class="sxs-lookup"><span data-stu-id="5cc1a-133">actionName</span></span>|[<span data-ttu-id="5cc1a-134">managedDeviceRemoteAction</span><span class="sxs-lookup"><span data-stu-id="5cc1a-134">managedDeviceRemoteAction</span></span>](../resources/intune-devices-manageddeviceremoteaction.md)|<span data-ttu-id="5cc1a-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="5cc1a-135">Not yet documented</span></span>|
|<span data-ttu-id="5cc1a-136">keepEnrollmentData</span><span class="sxs-lookup"><span data-stu-id="5cc1a-136">keepEnrollmentData</span></span>|<span data-ttu-id="5cc1a-137">布尔</span><span class="sxs-lookup"><span data-stu-id="5cc1a-137">Boolean</span></span>|<span data-ttu-id="5cc1a-138">尚未记录</span><span class="sxs-lookup"><span data-stu-id="5cc1a-138">Not yet documented</span></span>|
|<span data-ttu-id="5cc1a-139">keepUserData</span><span class="sxs-lookup"><span data-stu-id="5cc1a-139">keepUserData</span></span>|<span data-ttu-id="5cc1a-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="5cc1a-140">Boolean</span></span>|<span data-ttu-id="5cc1a-141">尚未记录</span><span class="sxs-lookup"><span data-stu-id="5cc1a-141">Not yet documented</span></span>|
|<span data-ttu-id="5cc1a-142">deviceIds</span><span class="sxs-lookup"><span data-stu-id="5cc1a-142">deviceIds</span></span>|<span data-ttu-id="5cc1a-143">String collection</span><span class="sxs-lookup"><span data-stu-id="5cc1a-143">String collection</span></span>|<span data-ttu-id="5cc1a-144">尚未记录</span><span class="sxs-lookup"><span data-stu-id="5cc1a-144">Not yet documented</span></span>|
|<span data-ttu-id="5cc1a-145">notificationTitle</span><span class="sxs-lookup"><span data-stu-id="5cc1a-145">notificationTitle</span></span>|<span data-ttu-id="5cc1a-146">String</span><span class="sxs-lookup"><span data-stu-id="5cc1a-146">String</span></span>|<span data-ttu-id="5cc1a-147">尚未记录</span><span class="sxs-lookup"><span data-stu-id="5cc1a-147">Not yet documented</span></span>|
|<span data-ttu-id="5cc1a-148">notificationBody</span><span class="sxs-lookup"><span data-stu-id="5cc1a-148">notificationBody</span></span>|<span data-ttu-id="5cc1a-149">String</span><span class="sxs-lookup"><span data-stu-id="5cc1a-149">String</span></span>|<span data-ttu-id="5cc1a-150">尚未记录</span><span class="sxs-lookup"><span data-stu-id="5cc1a-150">Not yet documented</span></span>|
|<span data-ttu-id="5cc1a-151">deviceName</span><span class="sxs-lookup"><span data-stu-id="5cc1a-151">deviceName</span></span>|<span data-ttu-id="5cc1a-152">String</span><span class="sxs-lookup"><span data-stu-id="5cc1a-152">String</span></span>|<span data-ttu-id="5cc1a-153">尚未记录</span><span class="sxs-lookup"><span data-stu-id="5cc1a-153">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="5cc1a-154">响应</span><span class="sxs-lookup"><span data-stu-id="5cc1a-154">Response</span></span>
<span data-ttu-id="5cc1a-155">如果成功，此操作在响应正文中返回 响应代码和 `200 OK` [bulkManagedDeviceActionResult。](../resources/intune-devices-bulkmanageddeviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="5cc1a-155">If successful, this action returns a `200 OK` response code and a [bulkManagedDeviceActionResult](../resources/intune-devices-bulkmanageddeviceactionresult.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5cc1a-156">示例</span><span class="sxs-lookup"><span data-stu-id="5cc1a-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="5cc1a-157">请求</span><span class="sxs-lookup"><span data-stu-id="5cc1a-157">Request</span></span>
<span data-ttu-id="5cc1a-158">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5cc1a-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5cc1a-159">响应</span><span class="sxs-lookup"><span data-stu-id="5cc1a-159">Response</span></span>
<span data-ttu-id="5cc1a-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5cc1a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




