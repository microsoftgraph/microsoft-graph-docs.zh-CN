---
title: cleanWindowsDevice 操作
description: 清理 Windows 设备
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 68775825b67e6e6410f5159f1a43b1dc3f248bb6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32520205"
---
# <a name="cleanwindowsdevice-action"></a><span data-ttu-id="54adf-103">cleanWindowsDevice 操作</span><span class="sxs-lookup"><span data-stu-id="54adf-103">cleanWindowsDevice action</span></span>

> <span data-ttu-id="54adf-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="54adf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="54adf-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="54adf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="54adf-106">清理 Windows 设备</span><span class="sxs-lookup"><span data-stu-id="54adf-106">Clean Windows device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="54adf-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="54adf-107">Prerequisites</span></span>
<span data-ttu-id="54adf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="54adf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="54adf-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="54adf-110">Permission type</span></span>|<span data-ttu-id="54adf-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="54adf-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="54adf-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="54adf-112">Delegated (work or school account)</span></span>|<span data-ttu-id="54adf-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="54adf-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="54adf-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="54adf-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="54adf-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="54adf-115">Not supported.</span></span>|
|<span data-ttu-id="54adf-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="54adf-116">Application</span></span>|<span data-ttu-id="54adf-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="54adf-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="54adf-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="54adf-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/cleanWindowsDevice
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/cleanWindowsDevice
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/cleanWindowsDevice
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/cleanWindowsDevice
```

## <a name="request-headers"></a><span data-ttu-id="54adf-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="54adf-119">Request headers</span></span>
|<span data-ttu-id="54adf-120">标头</span><span class="sxs-lookup"><span data-stu-id="54adf-120">Header</span></span>|<span data-ttu-id="54adf-121">值</span><span class="sxs-lookup"><span data-stu-id="54adf-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="54adf-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="54adf-122">Authorization</span></span>|<span data-ttu-id="54adf-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="54adf-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="54adf-124">接受</span><span class="sxs-lookup"><span data-stu-id="54adf-124">Accept</span></span>|<span data-ttu-id="54adf-125">application/json</span><span class="sxs-lookup"><span data-stu-id="54adf-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="54adf-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="54adf-126">Request body</span></span>
<span data-ttu-id="54adf-127">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="54adf-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="54adf-128">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="54adf-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="54adf-129">属性</span><span class="sxs-lookup"><span data-stu-id="54adf-129">Property</span></span>|<span data-ttu-id="54adf-130">类型</span><span class="sxs-lookup"><span data-stu-id="54adf-130">Type</span></span>|<span data-ttu-id="54adf-131">说明</span><span class="sxs-lookup"><span data-stu-id="54adf-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54adf-132">keepUserData</span><span class="sxs-lookup"><span data-stu-id="54adf-132">keepUserData</span></span>|<span data-ttu-id="54adf-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="54adf-133">Boolean</span></span>|<span data-ttu-id="54adf-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="54adf-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="54adf-135">响应</span><span class="sxs-lookup"><span data-stu-id="54adf-135">Response</span></span>
<span data-ttu-id="54adf-136">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="54adf-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="54adf-137">示例</span><span class="sxs-lookup"><span data-stu-id="54adf-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="54adf-138">请求</span><span class="sxs-lookup"><span data-stu-id="54adf-138">Request</span></span>
<span data-ttu-id="54adf-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="54adf-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/cleanWindowsDevice

Content-type: application/json
Content-length: 28

{
  "keepUserData": true
}
```

### <a name="response"></a><span data-ttu-id="54adf-140">响应</span><span class="sxs-lookup"><span data-stu-id="54adf-140">Response</span></span>
<span data-ttu-id="54adf-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="54adf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





