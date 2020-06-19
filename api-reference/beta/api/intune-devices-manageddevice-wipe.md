---
title: wipe 操作
description: 擦除设备
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8ea07fd650a00e91896639d0312b48bb787b2b54
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792125"
---
# <a name="wipe-action"></a><span data-ttu-id="12772-103">擦除操作</span><span class="sxs-lookup"><span data-stu-id="12772-103">wipe action</span></span>

<span data-ttu-id="12772-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="12772-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="12772-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="12772-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="12772-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="12772-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12772-107">擦除设备</span><span class="sxs-lookup"><span data-stu-id="12772-107">Wipe a device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="12772-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="12772-108">Prerequisites</span></span>
<span data-ttu-id="12772-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="12772-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="12772-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12772-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12772-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="12772-111">Permission type</span></span>|<span data-ttu-id="12772-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="12772-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="12772-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="12772-113">Delegated (work or school account)</span></span>|<span data-ttu-id="12772-114">Devicemanagementmanageddevices.readwrite.all、Devicemanagementmanageddevices.readwrite.all 和所有 PriviligedOperation</span><span class="sxs-lookup"><span data-stu-id="12772-114">DeviceManagementManagedDevices.PriviligedOperation.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="12772-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="12772-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12772-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="12772-116">Not supported.</span></span>|
|<span data-ttu-id="12772-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="12772-117">Application</span></span>|<span data-ttu-id="12772-118">Devicemanagementmanageddevices.readwrite.all、Devicemanagementmanageddevices.readwrite.all 和所有 PriviligedOperation</span><span class="sxs-lookup"><span data-stu-id="12772-118">DeviceManagementManagedDevices.PriviligedOperation.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="12772-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="12772-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/comanagedDevices/{managedDeviceId}/wipe
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice/wipe
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/wipe
POST /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates/{deviceComplianceScriptDeviceStateId}/managedDevice/wipe
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/wipe
```

## <a name="request-headers"></a><span data-ttu-id="12772-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="12772-120">Request headers</span></span>
|<span data-ttu-id="12772-121">标头</span><span class="sxs-lookup"><span data-stu-id="12772-121">Header</span></span>|<span data-ttu-id="12772-122">值</span><span class="sxs-lookup"><span data-stu-id="12772-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="12772-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="12772-123">Authorization</span></span>|<span data-ttu-id="12772-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="12772-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="12772-125">接受</span><span class="sxs-lookup"><span data-stu-id="12772-125">Accept</span></span>|<span data-ttu-id="12772-126">application/json</span><span class="sxs-lookup"><span data-stu-id="12772-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="12772-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="12772-127">Request body</span></span>
<span data-ttu-id="12772-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="12772-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="12772-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="12772-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="12772-130">属性</span><span class="sxs-lookup"><span data-stu-id="12772-130">Property</span></span>|<span data-ttu-id="12772-131">类型</span><span class="sxs-lookup"><span data-stu-id="12772-131">Type</span></span>|<span data-ttu-id="12772-132">说明</span><span class="sxs-lookup"><span data-stu-id="12772-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12772-133">keepEnrollmentData</span><span class="sxs-lookup"><span data-stu-id="12772-133">keepEnrollmentData</span></span>|<span data-ttu-id="12772-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="12772-134">Boolean</span></span>|<span data-ttu-id="12772-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="12772-135">Not yet documented</span></span>|
|<span data-ttu-id="12772-136">keepUserData</span><span class="sxs-lookup"><span data-stu-id="12772-136">keepUserData</span></span>|<span data-ttu-id="12772-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="12772-137">Boolean</span></span>|<span data-ttu-id="12772-138">尚未记录</span><span class="sxs-lookup"><span data-stu-id="12772-138">Not yet documented</span></span>|
|<span data-ttu-id="12772-139">macOsUnlockCode</span><span class="sxs-lookup"><span data-stu-id="12772-139">macOsUnlockCode</span></span>|<span data-ttu-id="12772-140">字符串</span><span class="sxs-lookup"><span data-stu-id="12772-140">String</span></span>|<span data-ttu-id="12772-141">尚未记录</span><span class="sxs-lookup"><span data-stu-id="12772-141">Not yet documented</span></span>|
|<span data-ttu-id="12772-142">useProtectedWipe</span><span class="sxs-lookup"><span data-stu-id="12772-142">useProtectedWipe</span></span>|<span data-ttu-id="12772-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="12772-143">Boolean</span></span>|<span data-ttu-id="12772-144">尚未记录</span><span class="sxs-lookup"><span data-stu-id="12772-144">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="12772-145">响应</span><span class="sxs-lookup"><span data-stu-id="12772-145">Response</span></span>
<span data-ttu-id="12772-146">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="12772-146">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="12772-147">示例</span><span class="sxs-lookup"><span data-stu-id="12772-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="12772-148">请求</span><span class="sxs-lookup"><span data-stu-id="12772-148">Request</span></span>
<span data-ttu-id="12772-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="12772-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="12772-150">响应</span><span class="sxs-lookup"><span data-stu-id="12772-150">Response</span></span>
<span data-ttu-id="12772-151">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="12772-151">Here is an example of the response.</span></span> <span data-ttu-id="12772-152">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="12772-152">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="12772-153">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="12772-153">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



