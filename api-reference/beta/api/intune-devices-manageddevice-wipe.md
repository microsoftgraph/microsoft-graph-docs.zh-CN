---
title: wipe 操作
description: 擦除设备
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2979333890626d197e596d6e768ac26205888276
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30139359"
---
# <a name="wipe-action"></a><span data-ttu-id="c09d9-103">擦除操作</span><span class="sxs-lookup"><span data-stu-id="c09d9-103">wipe action</span></span>

> <span data-ttu-id="c09d9-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c09d9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c09d9-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c09d9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c09d9-106">擦除设备</span><span class="sxs-lookup"><span data-stu-id="c09d9-106">Wipe a device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c09d9-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="c09d9-107">Prerequisites</span></span>
<span data-ttu-id="c09d9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="c09d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c09d9-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c09d9-110">Permission type</span></span>|<span data-ttu-id="c09d9-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c09d9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c09d9-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c09d9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c09d9-113">devicemanagementmanageddevices.readwrite.all、devicemanagementmanageddevices.readwrite.all 和所有 PriviligedOperation</span><span class="sxs-lookup"><span data-stu-id="c09d9-113">DeviceManagementManagedDevices.PriviligedOperation.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="c09d9-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c09d9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c09d9-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c09d9-115">Not supported.</span></span>|
|<span data-ttu-id="c09d9-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c09d9-116">Application</span></span>|<span data-ttu-id="c09d9-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="c09d9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c09d9-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c09d9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/wipe
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/wipe
```

## <a name="request-headers"></a><span data-ttu-id="c09d9-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c09d9-119">Request headers</span></span>
|<span data-ttu-id="c09d9-120">标头</span><span class="sxs-lookup"><span data-stu-id="c09d9-120">Header</span></span>|<span data-ttu-id="c09d9-121">值</span><span class="sxs-lookup"><span data-stu-id="c09d9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c09d9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c09d9-122">Authorization</span></span>|<span data-ttu-id="c09d9-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c09d9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c09d9-124">Accept</span><span class="sxs-lookup"><span data-stu-id="c09d9-124">Accept</span></span>|<span data-ttu-id="c09d9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c09d9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c09d9-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c09d9-126">Request body</span></span>
<span data-ttu-id="c09d9-127">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c09d9-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="c09d9-128">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="c09d9-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="c09d9-129">属性</span><span class="sxs-lookup"><span data-stu-id="c09d9-129">Property</span></span>|<span data-ttu-id="c09d9-130">类型</span><span class="sxs-lookup"><span data-stu-id="c09d9-130">Type</span></span>|<span data-ttu-id="c09d9-131">说明</span><span class="sxs-lookup"><span data-stu-id="c09d9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c09d9-132">keepEnrollmentData</span><span class="sxs-lookup"><span data-stu-id="c09d9-132">keepEnrollmentData</span></span>|<span data-ttu-id="c09d9-133">布尔</span><span class="sxs-lookup"><span data-stu-id="c09d9-133">Boolean</span></span>|<span data-ttu-id="c09d9-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c09d9-134">Not yet documented</span></span>|
|<span data-ttu-id="c09d9-135">keepUserData</span><span class="sxs-lookup"><span data-stu-id="c09d9-135">keepUserData</span></span>|<span data-ttu-id="c09d9-136">布尔</span><span class="sxs-lookup"><span data-stu-id="c09d9-136">Boolean</span></span>|<span data-ttu-id="c09d9-137">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c09d9-137">Not yet documented</span></span>|
|<span data-ttu-id="c09d9-138">macOsUnlockCode</span><span class="sxs-lookup"><span data-stu-id="c09d9-138">macOsUnlockCode</span></span>|<span data-ttu-id="c09d9-139">字符串</span><span class="sxs-lookup"><span data-stu-id="c09d9-139">String</span></span>|<span data-ttu-id="c09d9-140">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c09d9-140">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="c09d9-141">响应</span><span class="sxs-lookup"><span data-stu-id="c09d9-141">Response</span></span>
<span data-ttu-id="c09d9-142">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="c09d9-142">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c09d9-143">示例</span><span class="sxs-lookup"><span data-stu-id="c09d9-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="c09d9-144">请求</span><span class="sxs-lookup"><span data-stu-id="c09d9-144">Request</span></span>
<span data-ttu-id="c09d9-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c09d9-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/managedDevices/{managedDeviceId}/wipe

Content-type: application/json
Content-length: 109

{
  "keepEnrollmentData": true,
  "keepUserData": true,
  "macOsUnlockCode": "Mac Os Unlock Code value"
}
```

### <a name="response"></a><span data-ttu-id="c09d9-146">响应</span><span class="sxs-lookup"><span data-stu-id="c09d9-146">Response</span></span>
<span data-ttu-id="c09d9-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c09d9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




