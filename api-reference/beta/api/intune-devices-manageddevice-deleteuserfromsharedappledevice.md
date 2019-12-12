---
title: deleteUserFromSharedAppleDevice 操作
description: 从共享 Apple 设备中删除用户
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f314a59120d6cfce6ea0c3758d9fe4cd9255c58e
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39944818"
---
# <a name="deleteuserfromsharedappledevice-action"></a><span data-ttu-id="34e83-103">deleteUserFromSharedAppleDevice 操作</span><span class="sxs-lookup"><span data-stu-id="34e83-103">deleteUserFromSharedAppleDevice action</span></span>

> <span data-ttu-id="34e83-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="34e83-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="34e83-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="34e83-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34e83-106">从共享 Apple 设备中删除用户</span><span class="sxs-lookup"><span data-stu-id="34e83-106">Delete user from shared Apple device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="34e83-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="34e83-107">Prerequisites</span></span>
<span data-ttu-id="34e83-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="34e83-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34e83-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="34e83-110">Permission type</span></span>|<span data-ttu-id="34e83-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="34e83-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="34e83-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="34e83-112">Delegated (work or school account)</span></span>|<span data-ttu-id="34e83-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="34e83-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="34e83-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="34e83-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="34e83-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="34e83-115">Not supported.</span></span>|
|<span data-ttu-id="34e83-116">Application</span><span class="sxs-lookup"><span data-stu-id="34e83-116">Application</span></span>|<span data-ttu-id="34e83-117">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="34e83-117">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="34e83-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="34e83-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/deleteUserFromSharedAppleDevice
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice/deleteUserFromSharedAppleDevice
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deleteUserFromSharedAppleDevice
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/deleteUserFromSharedAppleDevice
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deleteUserFromSharedAppleDevice
```

## <a name="request-headers"></a><span data-ttu-id="34e83-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="34e83-119">Request headers</span></span>
|<span data-ttu-id="34e83-120">标头</span><span class="sxs-lookup"><span data-stu-id="34e83-120">Header</span></span>|<span data-ttu-id="34e83-121">值</span><span class="sxs-lookup"><span data-stu-id="34e83-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="34e83-122">授权</span><span class="sxs-lookup"><span data-stu-id="34e83-122">Authorization</span></span>|<span data-ttu-id="34e83-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="34e83-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="34e83-124">接受</span><span class="sxs-lookup"><span data-stu-id="34e83-124">Accept</span></span>|<span data-ttu-id="34e83-125">application/json</span><span class="sxs-lookup"><span data-stu-id="34e83-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="34e83-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="34e83-126">Request body</span></span>
<span data-ttu-id="34e83-127">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="34e83-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="34e83-128">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="34e83-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="34e83-129">属性</span><span class="sxs-lookup"><span data-stu-id="34e83-129">Property</span></span>|<span data-ttu-id="34e83-130">类型</span><span class="sxs-lookup"><span data-stu-id="34e83-130">Type</span></span>|<span data-ttu-id="34e83-131">说明</span><span class="sxs-lookup"><span data-stu-id="34e83-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34e83-132">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="34e83-132">userPrincipalName</span></span>|<span data-ttu-id="34e83-133">字符串</span><span class="sxs-lookup"><span data-stu-id="34e83-133">String</span></span>|<span data-ttu-id="34e83-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="34e83-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="34e83-135">响应</span><span class="sxs-lookup"><span data-stu-id="34e83-135">Response</span></span>
<span data-ttu-id="34e83-136">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="34e83-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="34e83-137">示例</span><span class="sxs-lookup"><span data-stu-id="34e83-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="34e83-138">请求</span><span class="sxs-lookup"><span data-stu-id="34e83-138">Request</span></span>
<span data-ttu-id="34e83-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="34e83-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/deleteUserFromSharedAppleDevice

Content-type: application/json
Content-length: 56

{
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="34e83-140">响应</span><span class="sxs-lookup"><span data-stu-id="34e83-140">Response</span></span>
<span data-ttu-id="34e83-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="34e83-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





