---
title: wipe 操作
description: 擦除设备
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 86676dd636decb822cab5549f1fcc619c033f179
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48704075"
---
# <a name="wipe-action"></a><span data-ttu-id="ea3a9-103">擦除操作</span><span class="sxs-lookup"><span data-stu-id="ea3a9-103">wipe action</span></span>

<span data-ttu-id="ea3a9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ea3a9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ea3a9-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ea3a9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ea3a9-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ea3a9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ea3a9-107">擦除设备</span><span class="sxs-lookup"><span data-stu-id="ea3a9-107">Wipe a device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ea3a9-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="ea3a9-108">Prerequisites</span></span>
<span data-ttu-id="ea3a9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ea3a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea3a9-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ea3a9-111">Permission type</span></span>|<span data-ttu-id="ea3a9-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ea3a9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ea3a9-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ea3a9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ea3a9-114">Devicemanagementmanageddevices.readwrite.all、Devicemanagementmanageddevices.readwrite.all 和所有 PriviligedOperation</span><span class="sxs-lookup"><span data-stu-id="ea3a9-114">DeviceManagementManagedDevices.PriviligedOperation.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="ea3a9-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ea3a9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ea3a9-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ea3a9-116">Not supported.</span></span>|
|<span data-ttu-id="ea3a9-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ea3a9-117">Application</span></span>|<span data-ttu-id="ea3a9-118">Devicemanagementmanageddevices.readwrite.all、Devicemanagementmanageddevices.readwrite.all 和所有 PriviligedOperation</span><span class="sxs-lookup"><span data-stu-id="ea3a9-118">DeviceManagementManagedDevices.PriviligedOperation.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ea3a9-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ea3a9-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="ea3a9-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ea3a9-120">Request headers</span></span>
|<span data-ttu-id="ea3a9-121">标头</span><span class="sxs-lookup"><span data-stu-id="ea3a9-121">Header</span></span>|<span data-ttu-id="ea3a9-122">值</span><span class="sxs-lookup"><span data-stu-id="ea3a9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ea3a9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ea3a9-123">Authorization</span></span>|<span data-ttu-id="ea3a9-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ea3a9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ea3a9-125">接受</span><span class="sxs-lookup"><span data-stu-id="ea3a9-125">Accept</span></span>|<span data-ttu-id="ea3a9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ea3a9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ea3a9-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ea3a9-127">Request body</span></span>
<span data-ttu-id="ea3a9-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ea3a9-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="ea3a9-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="ea3a9-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="ea3a9-130">属性</span><span class="sxs-lookup"><span data-stu-id="ea3a9-130">Property</span></span>|<span data-ttu-id="ea3a9-131">类型</span><span class="sxs-lookup"><span data-stu-id="ea3a9-131">Type</span></span>|<span data-ttu-id="ea3a9-132">说明</span><span class="sxs-lookup"><span data-stu-id="ea3a9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea3a9-133">keepEnrollmentData</span><span class="sxs-lookup"><span data-stu-id="ea3a9-133">keepEnrollmentData</span></span>|<span data-ttu-id="ea3a9-134">布尔</span><span class="sxs-lookup"><span data-stu-id="ea3a9-134">Boolean</span></span>|<span data-ttu-id="ea3a9-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="ea3a9-135">Not yet documented</span></span>|
|<span data-ttu-id="ea3a9-136">keepUserData</span><span class="sxs-lookup"><span data-stu-id="ea3a9-136">keepUserData</span></span>|<span data-ttu-id="ea3a9-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="ea3a9-137">Boolean</span></span>|<span data-ttu-id="ea3a9-138">尚未记录</span><span class="sxs-lookup"><span data-stu-id="ea3a9-138">Not yet documented</span></span>|
|<span data-ttu-id="ea3a9-139">macOsUnlockCode</span><span class="sxs-lookup"><span data-stu-id="ea3a9-139">macOsUnlockCode</span></span>|<span data-ttu-id="ea3a9-140">字符串</span><span class="sxs-lookup"><span data-stu-id="ea3a9-140">String</span></span>|<span data-ttu-id="ea3a9-141">尚未记录</span><span class="sxs-lookup"><span data-stu-id="ea3a9-141">Not yet documented</span></span>|
|<span data-ttu-id="ea3a9-142">useProtectedWipe</span><span class="sxs-lookup"><span data-stu-id="ea3a9-142">useProtectedWipe</span></span>|<span data-ttu-id="ea3a9-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="ea3a9-143">Boolean</span></span>|<span data-ttu-id="ea3a9-144">尚未记录</span><span class="sxs-lookup"><span data-stu-id="ea3a9-144">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="ea3a9-145">响应</span><span class="sxs-lookup"><span data-stu-id="ea3a9-145">Response</span></span>
<span data-ttu-id="ea3a9-146">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="ea3a9-146">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ea3a9-147">示例</span><span class="sxs-lookup"><span data-stu-id="ea3a9-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="ea3a9-148">请求</span><span class="sxs-lookup"><span data-stu-id="ea3a9-148">Request</span></span>
<span data-ttu-id="ea3a9-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ea3a9-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ea3a9-150">响应</span><span class="sxs-lookup"><span data-stu-id="ea3a9-150">Response</span></span>
<span data-ttu-id="ea3a9-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ea3a9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





