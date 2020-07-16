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
# <a name="executeaction-action"></a><span data-ttu-id="44bcf-103">executeAction 操作</span><span class="sxs-lookup"><span data-stu-id="44bcf-103">executeAction action</span></span>

<span data-ttu-id="44bcf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="44bcf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="44bcf-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="44bcf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="44bcf-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="44bcf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="44bcf-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="44bcf-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="44bcf-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="44bcf-108">Prerequisites</span></span>
<span data-ttu-id="44bcf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="44bcf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44bcf-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="44bcf-111">Permission type</span></span>|<span data-ttu-id="44bcf-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="44bcf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="44bcf-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="44bcf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="44bcf-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="44bcf-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="44bcf-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="44bcf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="44bcf-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="44bcf-116">Not supported.</span></span>|
|<span data-ttu-id="44bcf-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="44bcf-117">Application</span></span>|<span data-ttu-id="44bcf-118">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="44bcf-118">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="44bcf-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="44bcf-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="44bcf-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="44bcf-120">Request headers</span></span>
|<span data-ttu-id="44bcf-121">标头</span><span class="sxs-lookup"><span data-stu-id="44bcf-121">Header</span></span>|<span data-ttu-id="44bcf-122">值</span><span class="sxs-lookup"><span data-stu-id="44bcf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="44bcf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="44bcf-123">Authorization</span></span>|<span data-ttu-id="44bcf-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="44bcf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="44bcf-125">接受</span><span class="sxs-lookup"><span data-stu-id="44bcf-125">Accept</span></span>|<span data-ttu-id="44bcf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="44bcf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="44bcf-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="44bcf-127">Request body</span></span>
<span data-ttu-id="44bcf-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="44bcf-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="44bcf-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="44bcf-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="44bcf-130">属性</span><span class="sxs-lookup"><span data-stu-id="44bcf-130">Property</span></span>|<span data-ttu-id="44bcf-131">类型</span><span class="sxs-lookup"><span data-stu-id="44bcf-131">Type</span></span>|<span data-ttu-id="44bcf-132">说明</span><span class="sxs-lookup"><span data-stu-id="44bcf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44bcf-133">actionName</span><span class="sxs-lookup"><span data-stu-id="44bcf-133">actionName</span></span>|[<span data-ttu-id="44bcf-134">managedDeviceRemoteAction</span><span class="sxs-lookup"><span data-stu-id="44bcf-134">managedDeviceRemoteAction</span></span>](../resources/intune-devices-manageddeviceremoteaction.md)|<span data-ttu-id="44bcf-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="44bcf-135">Not yet documented</span></span>|
|<span data-ttu-id="44bcf-136">keepEnrollmentData</span><span class="sxs-lookup"><span data-stu-id="44bcf-136">keepEnrollmentData</span></span>|<span data-ttu-id="44bcf-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="44bcf-137">Boolean</span></span>|<span data-ttu-id="44bcf-138">尚未记录</span><span class="sxs-lookup"><span data-stu-id="44bcf-138">Not yet documented</span></span>|
|<span data-ttu-id="44bcf-139">keepUserData</span><span class="sxs-lookup"><span data-stu-id="44bcf-139">keepUserData</span></span>|<span data-ttu-id="44bcf-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="44bcf-140">Boolean</span></span>|<span data-ttu-id="44bcf-141">尚未记录</span><span class="sxs-lookup"><span data-stu-id="44bcf-141">Not yet documented</span></span>|
|<span data-ttu-id="44bcf-142">deviceIds</span><span class="sxs-lookup"><span data-stu-id="44bcf-142">deviceIds</span></span>|<span data-ttu-id="44bcf-143">String collection</span><span class="sxs-lookup"><span data-stu-id="44bcf-143">String collection</span></span>|<span data-ttu-id="44bcf-144">尚未记录</span><span class="sxs-lookup"><span data-stu-id="44bcf-144">Not yet documented</span></span>|
|<span data-ttu-id="44bcf-145">notificationTitle</span><span class="sxs-lookup"><span data-stu-id="44bcf-145">notificationTitle</span></span>|<span data-ttu-id="44bcf-146">String</span><span class="sxs-lookup"><span data-stu-id="44bcf-146">String</span></span>|<span data-ttu-id="44bcf-147">尚未记录</span><span class="sxs-lookup"><span data-stu-id="44bcf-147">Not yet documented</span></span>|
|<span data-ttu-id="44bcf-148">notificationBody</span><span class="sxs-lookup"><span data-stu-id="44bcf-148">notificationBody</span></span>|<span data-ttu-id="44bcf-149">String</span><span class="sxs-lookup"><span data-stu-id="44bcf-149">String</span></span>|<span data-ttu-id="44bcf-150">尚未记录</span><span class="sxs-lookup"><span data-stu-id="44bcf-150">Not yet documented</span></span>|
|<span data-ttu-id="44bcf-151">deviceName</span><span class="sxs-lookup"><span data-stu-id="44bcf-151">deviceName</span></span>|<span data-ttu-id="44bcf-152">String</span><span class="sxs-lookup"><span data-stu-id="44bcf-152">String</span></span>|<span data-ttu-id="44bcf-153">尚未记录</span><span class="sxs-lookup"><span data-stu-id="44bcf-153">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="44bcf-154">响应</span><span class="sxs-lookup"><span data-stu-id="44bcf-154">Response</span></span>
<span data-ttu-id="44bcf-155">如果成功，此操作会 `200 OK` 在响应正文中返回响应代码和[bulkManagedDeviceActionResult](../resources/intune-devices-bulkmanageddeviceactionresult.md) 。</span><span class="sxs-lookup"><span data-stu-id="44bcf-155">If successful, this action returns a `200 OK` response code and a [bulkManagedDeviceActionResult](../resources/intune-devices-bulkmanageddeviceactionresult.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44bcf-156">示例</span><span class="sxs-lookup"><span data-stu-id="44bcf-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="44bcf-157">请求</span><span class="sxs-lookup"><span data-stu-id="44bcf-157">Request</span></span>
<span data-ttu-id="44bcf-158">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="44bcf-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="44bcf-159">响应</span><span class="sxs-lookup"><span data-stu-id="44bcf-159">Response</span></span>
<span data-ttu-id="44bcf-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="44bcf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



