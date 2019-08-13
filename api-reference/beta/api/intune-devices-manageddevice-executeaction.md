---
title: executeAction 操作
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6fc154f7b0f8b6fafded763c8fbc1276284e53f0
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36348779"
---
# <a name="executeaction-action"></a><span data-ttu-id="242cf-103">executeAction 操作</span><span class="sxs-lookup"><span data-stu-id="242cf-103">executeAction action</span></span>

> <span data-ttu-id="242cf-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="242cf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="242cf-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="242cf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="242cf-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="242cf-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="242cf-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="242cf-107">Prerequisites</span></span>
<span data-ttu-id="242cf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="242cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="242cf-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="242cf-110">Permission type</span></span>|<span data-ttu-id="242cf-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="242cf-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="242cf-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="242cf-112">Delegated (work or school account)</span></span>|<span data-ttu-id="242cf-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="242cf-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="242cf-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="242cf-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="242cf-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="242cf-115">Not supported.</span></span>|
|<span data-ttu-id="242cf-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="242cf-116">Application</span></span>|<span data-ttu-id="242cf-117">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="242cf-117">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="242cf-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="242cf-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/executeAction
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/executeAction
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/executeAction
```

## <a name="request-headers"></a><span data-ttu-id="242cf-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="242cf-119">Request headers</span></span>
|<span data-ttu-id="242cf-120">标头</span><span class="sxs-lookup"><span data-stu-id="242cf-120">Header</span></span>|<span data-ttu-id="242cf-121">值</span><span class="sxs-lookup"><span data-stu-id="242cf-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="242cf-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="242cf-122">Authorization</span></span>|<span data-ttu-id="242cf-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="242cf-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="242cf-124">接受</span><span class="sxs-lookup"><span data-stu-id="242cf-124">Accept</span></span>|<span data-ttu-id="242cf-125">application/json</span><span class="sxs-lookup"><span data-stu-id="242cf-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="242cf-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="242cf-126">Request body</span></span>
<span data-ttu-id="242cf-127">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="242cf-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="242cf-128">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="242cf-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="242cf-129">属性</span><span class="sxs-lookup"><span data-stu-id="242cf-129">Property</span></span>|<span data-ttu-id="242cf-130">类型</span><span class="sxs-lookup"><span data-stu-id="242cf-130">Type</span></span>|<span data-ttu-id="242cf-131">说明</span><span class="sxs-lookup"><span data-stu-id="242cf-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="242cf-132">actionName</span><span class="sxs-lookup"><span data-stu-id="242cf-132">actionName</span></span>|[<span data-ttu-id="242cf-133">managedDeviceRemoteAction</span><span class="sxs-lookup"><span data-stu-id="242cf-133">managedDeviceRemoteAction</span></span>](../resources/intune-devices-manageddeviceremoteaction.md)|<span data-ttu-id="242cf-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="242cf-134">Not yet documented</span></span>|
|<span data-ttu-id="242cf-135">keepEnrollmentData</span><span class="sxs-lookup"><span data-stu-id="242cf-135">keepEnrollmentData</span></span>|<span data-ttu-id="242cf-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="242cf-136">Boolean</span></span>|<span data-ttu-id="242cf-137">尚未记录</span><span class="sxs-lookup"><span data-stu-id="242cf-137">Not yet documented</span></span>|
|<span data-ttu-id="242cf-138">keepUserData</span><span class="sxs-lookup"><span data-stu-id="242cf-138">keepUserData</span></span>|<span data-ttu-id="242cf-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="242cf-139">Boolean</span></span>|<span data-ttu-id="242cf-140">尚未记录</span><span class="sxs-lookup"><span data-stu-id="242cf-140">Not yet documented</span></span>|
|<span data-ttu-id="242cf-141">deviceIds</span><span class="sxs-lookup"><span data-stu-id="242cf-141">deviceIds</span></span>|<span data-ttu-id="242cf-142">String collection</span><span class="sxs-lookup"><span data-stu-id="242cf-142">String collection</span></span>|<span data-ttu-id="242cf-143">尚未记录</span><span class="sxs-lookup"><span data-stu-id="242cf-143">Not yet documented</span></span>|
|<span data-ttu-id="242cf-144">notificationTitle</span><span class="sxs-lookup"><span data-stu-id="242cf-144">notificationTitle</span></span>|<span data-ttu-id="242cf-145">String</span><span class="sxs-lookup"><span data-stu-id="242cf-145">String</span></span>|<span data-ttu-id="242cf-146">尚未记录</span><span class="sxs-lookup"><span data-stu-id="242cf-146">Not yet documented</span></span>|
|<span data-ttu-id="242cf-147">notificationBody</span><span class="sxs-lookup"><span data-stu-id="242cf-147">notificationBody</span></span>|<span data-ttu-id="242cf-148">String</span><span class="sxs-lookup"><span data-stu-id="242cf-148">String</span></span>|<span data-ttu-id="242cf-149">尚未记录</span><span class="sxs-lookup"><span data-stu-id="242cf-149">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="242cf-150">响应</span><span class="sxs-lookup"><span data-stu-id="242cf-150">Response</span></span>
<span data-ttu-id="242cf-151">如果成功, 此操作会在`200 OK`响应正文中返回响应代码和[bulkManagedDeviceActionResult](../resources/intune-devices-bulkmanageddeviceactionresult.md) 。</span><span class="sxs-lookup"><span data-stu-id="242cf-151">If successful, this action returns a `200 OK` response code and a [bulkManagedDeviceActionResult](../resources/intune-devices-bulkmanageddeviceactionresult.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="242cf-152">示例</span><span class="sxs-lookup"><span data-stu-id="242cf-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="242cf-153">请求</span><span class="sxs-lookup"><span data-stu-id="242cf-153">Request</span></span>
<span data-ttu-id="242cf-154">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="242cf-154">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/executeAction

Content-type: application/json
Content-length: 236

{
  "actionName": "delete",
  "keepEnrollmentData": true,
  "keepUserData": true,
  "deviceIds": [
    "Device Ids value"
  ],
  "notificationTitle": "Notification Title value",
  "notificationBody": "Notification Body value"
}
```

### <a name="response"></a><span data-ttu-id="242cf-155">响应</span><span class="sxs-lookup"><span data-stu-id="242cf-155">Response</span></span>
<span data-ttu-id="242cf-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="242cf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






