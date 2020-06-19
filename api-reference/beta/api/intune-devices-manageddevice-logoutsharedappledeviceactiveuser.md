---
title: logoutSharedAppleDeviceActiveUser 操作
description: 注销共享 Apple 设备活动用户
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6682e900761e4b5ff62815c88415fe3edc52cf48
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792266"
---
# <a name="logoutsharedappledeviceactiveuser-action"></a><span data-ttu-id="a3cfa-103">logoutSharedAppleDeviceActiveUser 操作</span><span class="sxs-lookup"><span data-stu-id="a3cfa-103">logoutSharedAppleDeviceActiveUser action</span></span>

<span data-ttu-id="a3cfa-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a3cfa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a3cfa-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a3cfa-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a3cfa-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a3cfa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3cfa-107">注销共享 Apple 设备活动用户</span><span class="sxs-lookup"><span data-stu-id="a3cfa-107">Logout shared Apple device active user</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a3cfa-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="a3cfa-108">Prerequisites</span></span>
<span data-ttu-id="a3cfa-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="a3cfa-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="a3cfa-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a3cfa-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3cfa-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a3cfa-111">Permission type</span></span>|<span data-ttu-id="a3cfa-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a3cfa-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a3cfa-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a3cfa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a3cfa-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="a3cfa-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="a3cfa-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a3cfa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a3cfa-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a3cfa-116">Not supported.</span></span>|
|<span data-ttu-id="a3cfa-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a3cfa-117">Application</span></span>|<span data-ttu-id="a3cfa-118">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="a3cfa-118">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a3cfa-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a3cfa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/logoutSharedAppleDeviceActiveUser
POST /deviceManagement/comanagedDevices/{managedDeviceId}/logoutSharedAppleDeviceActiveUser
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice/logoutSharedAppleDeviceActiveUser
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/logoutSharedAppleDeviceActiveUser
POST /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates/{deviceComplianceScriptDeviceStateId}/managedDevice/logoutSharedAppleDeviceActiveUser
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/logoutSharedAppleDeviceActiveUser
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/logoutSharedAppleDeviceActiveUser
```

## <a name="request-headers"></a><span data-ttu-id="a3cfa-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a3cfa-120">Request headers</span></span>
|<span data-ttu-id="a3cfa-121">标头</span><span class="sxs-lookup"><span data-stu-id="a3cfa-121">Header</span></span>|<span data-ttu-id="a3cfa-122">值</span><span class="sxs-lookup"><span data-stu-id="a3cfa-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a3cfa-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a3cfa-123">Authorization</span></span>|<span data-ttu-id="a3cfa-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a3cfa-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a3cfa-125">接受</span><span class="sxs-lookup"><span data-stu-id="a3cfa-125">Accept</span></span>|<span data-ttu-id="a3cfa-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a3cfa-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a3cfa-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a3cfa-127">Request body</span></span>
<span data-ttu-id="a3cfa-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a3cfa-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a3cfa-129">响应</span><span class="sxs-lookup"><span data-stu-id="a3cfa-129">Response</span></span>
<span data-ttu-id="a3cfa-130">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="a3cfa-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a3cfa-131">示例</span><span class="sxs-lookup"><span data-stu-id="a3cfa-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="a3cfa-132">请求</span><span class="sxs-lookup"><span data-stu-id="a3cfa-132">Request</span></span>
<span data-ttu-id="a3cfa-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a3cfa-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/logoutSharedAppleDeviceActiveUser
```

### <a name="response"></a><span data-ttu-id="a3cfa-134">响应</span><span class="sxs-lookup"><span data-stu-id="a3cfa-134">Response</span></span>
<span data-ttu-id="a3cfa-135">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="a3cfa-135">Here is an example of the response.</span></span> <span data-ttu-id="a3cfa-136">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="a3cfa-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="a3cfa-137">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="a3cfa-137">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



