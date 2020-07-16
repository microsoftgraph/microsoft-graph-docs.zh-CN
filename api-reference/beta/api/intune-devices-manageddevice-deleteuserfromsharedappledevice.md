---
title: deleteUserFromSharedAppleDevice 操作
description: 从共享 Apple 设备中删除用户
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1276351b8d0624bf8c54198f5e5d5b839a0e7406
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792315"
---
# <a name="deleteuserfromsharedappledevice-action"></a><span data-ttu-id="2a7b3-103">deleteUserFromSharedAppleDevice 操作</span><span class="sxs-lookup"><span data-stu-id="2a7b3-103">deleteUserFromSharedAppleDevice action</span></span>

<span data-ttu-id="2a7b3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2a7b3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2a7b3-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2a7b3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2a7b3-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2a7b3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2a7b3-107">从共享 Apple 设备中删除用户</span><span class="sxs-lookup"><span data-stu-id="2a7b3-107">Delete user from shared Apple device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2a7b3-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="2a7b3-108">Prerequisites</span></span>
<span data-ttu-id="2a7b3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2a7b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a7b3-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="2a7b3-111">Permission type</span></span>|<span data-ttu-id="2a7b3-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2a7b3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2a7b3-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2a7b3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2a7b3-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="2a7b3-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="2a7b3-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2a7b3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2a7b3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2a7b3-116">Not supported.</span></span>|
|<span data-ttu-id="2a7b3-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="2a7b3-117">Application</span></span>|<span data-ttu-id="2a7b3-118">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="2a7b3-118">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2a7b3-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2a7b3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/deleteUserFromSharedAppleDevice
POST /deviceManagement/comanagedDevices/{managedDeviceId}/deleteUserFromSharedAppleDevice
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice/deleteUserFromSharedAppleDevice
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deleteUserFromSharedAppleDevice
POST /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates/{deviceComplianceScriptDeviceStateId}/managedDevice/deleteUserFromSharedAppleDevice
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/deleteUserFromSharedAppleDevice
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deleteUserFromSharedAppleDevice
```

## <a name="request-headers"></a><span data-ttu-id="2a7b3-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="2a7b3-120">Request headers</span></span>
|<span data-ttu-id="2a7b3-121">标头</span><span class="sxs-lookup"><span data-stu-id="2a7b3-121">Header</span></span>|<span data-ttu-id="2a7b3-122">值</span><span class="sxs-lookup"><span data-stu-id="2a7b3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2a7b3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2a7b3-123">Authorization</span></span>|<span data-ttu-id="2a7b3-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2a7b3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2a7b3-125">接受</span><span class="sxs-lookup"><span data-stu-id="2a7b3-125">Accept</span></span>|<span data-ttu-id="2a7b3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2a7b3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a7b3-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2a7b3-127">Request body</span></span>
<span data-ttu-id="2a7b3-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2a7b3-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="2a7b3-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="2a7b3-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="2a7b3-130">属性</span><span class="sxs-lookup"><span data-stu-id="2a7b3-130">Property</span></span>|<span data-ttu-id="2a7b3-131">类型</span><span class="sxs-lookup"><span data-stu-id="2a7b3-131">Type</span></span>|<span data-ttu-id="2a7b3-132">说明</span><span class="sxs-lookup"><span data-stu-id="2a7b3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a7b3-133">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2a7b3-133">userPrincipalName</span></span>|<span data-ttu-id="2a7b3-134">String</span><span class="sxs-lookup"><span data-stu-id="2a7b3-134">String</span></span>|<span data-ttu-id="2a7b3-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="2a7b3-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="2a7b3-136">响应</span><span class="sxs-lookup"><span data-stu-id="2a7b3-136">Response</span></span>
<span data-ttu-id="2a7b3-137">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="2a7b3-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2a7b3-138">示例</span><span class="sxs-lookup"><span data-stu-id="2a7b3-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="2a7b3-139">请求</span><span class="sxs-lookup"><span data-stu-id="2a7b3-139">Request</span></span>
<span data-ttu-id="2a7b3-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2a7b3-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/deleteUserFromSharedAppleDevice

Content-type: application/json
Content-length: 56

{
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="2a7b3-141">响应</span><span class="sxs-lookup"><span data-stu-id="2a7b3-141">Response</span></span>
<span data-ttu-id="2a7b3-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2a7b3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



