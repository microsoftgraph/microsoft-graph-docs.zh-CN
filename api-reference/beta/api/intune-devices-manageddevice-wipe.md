---
title: wipe 操作
description: 擦除设备
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5e8bd9d7f002a5b6446043b8b458609883326deb
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42773971"
---
# <a name="wipe-action"></a><span data-ttu-id="e8c2b-103">擦除操作</span><span class="sxs-lookup"><span data-stu-id="e8c2b-103">wipe action</span></span>

> <span data-ttu-id="e8c2b-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e8c2b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e8c2b-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e8c2b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8c2b-106">擦除设备</span><span class="sxs-lookup"><span data-stu-id="e8c2b-106">Wipe a device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e8c2b-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="e8c2b-107">Prerequisites</span></span>
<span data-ttu-id="e8c2b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e8c2b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8c2b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e8c2b-110">Permission type</span></span>|<span data-ttu-id="e8c2b-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e8c2b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e8c2b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e8c2b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e8c2b-113">Devicemanagementmanageddevices.readwrite.all、Devicemanagementmanageddevices.readwrite.all 和所有 PriviligedOperation</span><span class="sxs-lookup"><span data-stu-id="e8c2b-113">DeviceManagementManagedDevices.PriviligedOperation.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="e8c2b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e8c2b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e8c2b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e8c2b-115">Not supported.</span></span>|
|<span data-ttu-id="e8c2b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="e8c2b-116">Application</span></span>|<span data-ttu-id="e8c2b-117">Devicemanagementmanageddevices.readwrite.all、Devicemanagementmanageddevices.readwrite.all 和所有 PriviligedOperation</span><span class="sxs-lookup"><span data-stu-id="e8c2b-117">DeviceManagementManagedDevices.PriviligedOperation.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e8c2b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e8c2b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice/wipe
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/wipe
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/wipe
```

## <a name="request-headers"></a><span data-ttu-id="e8c2b-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="e8c2b-119">Request headers</span></span>
|<span data-ttu-id="e8c2b-120">标头</span><span class="sxs-lookup"><span data-stu-id="e8c2b-120">Header</span></span>|<span data-ttu-id="e8c2b-121">值</span><span class="sxs-lookup"><span data-stu-id="e8c2b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e8c2b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e8c2b-122">Authorization</span></span>|<span data-ttu-id="e8c2b-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e8c2b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e8c2b-124">接受</span><span class="sxs-lookup"><span data-stu-id="e8c2b-124">Accept</span></span>|<span data-ttu-id="e8c2b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e8c2b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8c2b-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="e8c2b-126">Request body</span></span>
<span data-ttu-id="e8c2b-127">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e8c2b-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="e8c2b-128">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="e8c2b-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="e8c2b-129">属性</span><span class="sxs-lookup"><span data-stu-id="e8c2b-129">Property</span></span>|<span data-ttu-id="e8c2b-130">类型</span><span class="sxs-lookup"><span data-stu-id="e8c2b-130">Type</span></span>|<span data-ttu-id="e8c2b-131">说明</span><span class="sxs-lookup"><span data-stu-id="e8c2b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8c2b-132">keepEnrollmentData</span><span class="sxs-lookup"><span data-stu-id="e8c2b-132">keepEnrollmentData</span></span>|<span data-ttu-id="e8c2b-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8c2b-133">Boolean</span></span>|<span data-ttu-id="e8c2b-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e8c2b-134">Not yet documented</span></span>|
|<span data-ttu-id="e8c2b-135">keepUserData</span><span class="sxs-lookup"><span data-stu-id="e8c2b-135">keepUserData</span></span>|<span data-ttu-id="e8c2b-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8c2b-136">Boolean</span></span>|<span data-ttu-id="e8c2b-137">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e8c2b-137">Not yet documented</span></span>|
|<span data-ttu-id="e8c2b-138">macOsUnlockCode</span><span class="sxs-lookup"><span data-stu-id="e8c2b-138">macOsUnlockCode</span></span>|<span data-ttu-id="e8c2b-139">字符串</span><span class="sxs-lookup"><span data-stu-id="e8c2b-139">String</span></span>|<span data-ttu-id="e8c2b-140">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e8c2b-140">Not yet documented</span></span>|
|<span data-ttu-id="e8c2b-141">useProtectedWipe</span><span class="sxs-lookup"><span data-stu-id="e8c2b-141">useProtectedWipe</span></span>|<span data-ttu-id="e8c2b-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8c2b-142">Boolean</span></span>|<span data-ttu-id="e8c2b-143">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e8c2b-143">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="e8c2b-144">响应</span><span class="sxs-lookup"><span data-stu-id="e8c2b-144">Response</span></span>
<span data-ttu-id="e8c2b-145">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="e8c2b-145">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e8c2b-146">示例</span><span class="sxs-lookup"><span data-stu-id="e8c2b-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="e8c2b-147">请求</span><span class="sxs-lookup"><span data-stu-id="e8c2b-147">Request</span></span>
<span data-ttu-id="e8c2b-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e8c2b-148">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/wipe

Content-type: application/json
Content-length: 138

{
  "keepEnrollmentData": true,
  "keepUserData": true,
  "macOsUnlockCode": "Mac Os Unlock Code value",
  "useProtectedWipe": true
}
```

### <a name="response"></a><span data-ttu-id="e8c2b-149">响应</span><span class="sxs-lookup"><span data-stu-id="e8c2b-149">Response</span></span>
<span data-ttu-id="e8c2b-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e8c2b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




