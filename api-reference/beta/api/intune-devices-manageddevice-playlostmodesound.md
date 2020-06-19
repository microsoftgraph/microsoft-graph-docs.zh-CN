---
title: playLostModeSound 操作
description: 远程锁定
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d1f1e6b13f4e778cf3cb6810b55a9019a64e46be
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792259"
---
# <a name="playlostmodesound-action"></a><span data-ttu-id="413e7-103">playLostModeSound 操作</span><span class="sxs-lookup"><span data-stu-id="413e7-103">playLostModeSound action</span></span>

<span data-ttu-id="413e7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="413e7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="413e7-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="413e7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="413e7-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="413e7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="413e7-107">远程锁定</span><span class="sxs-lookup"><span data-stu-id="413e7-107">Remote lock</span></span>

## <a name="prerequisites"></a><span data-ttu-id="413e7-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="413e7-108">Prerequisites</span></span>
<span data-ttu-id="413e7-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="413e7-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="413e7-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="413e7-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="413e7-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="413e7-111">Permission type</span></span>|<span data-ttu-id="413e7-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="413e7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="413e7-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="413e7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="413e7-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="413e7-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="413e7-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="413e7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="413e7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="413e7-116">Not supported.</span></span>|
|<span data-ttu-id="413e7-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="413e7-117">Application</span></span>|<span data-ttu-id="413e7-118">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="413e7-118">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="413e7-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="413e7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/playLostModeSound
POST /deviceManagement/comanagedDevices/{managedDeviceId}/playLostModeSound
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice/playLostModeSound
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/playLostModeSound
POST /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates/{deviceComplianceScriptDeviceStateId}/managedDevice/playLostModeSound
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/playLostModeSound
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/playLostModeSound
```

## <a name="request-headers"></a><span data-ttu-id="413e7-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="413e7-120">Request headers</span></span>
|<span data-ttu-id="413e7-121">标头</span><span class="sxs-lookup"><span data-stu-id="413e7-121">Header</span></span>|<span data-ttu-id="413e7-122">值</span><span class="sxs-lookup"><span data-stu-id="413e7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="413e7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="413e7-123">Authorization</span></span>|<span data-ttu-id="413e7-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="413e7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="413e7-125">接受</span><span class="sxs-lookup"><span data-stu-id="413e7-125">Accept</span></span>|<span data-ttu-id="413e7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="413e7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="413e7-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="413e7-127">Request body</span></span>
<span data-ttu-id="413e7-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="413e7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="413e7-129">响应</span><span class="sxs-lookup"><span data-stu-id="413e7-129">Response</span></span>
<span data-ttu-id="413e7-130">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="413e7-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="413e7-131">示例</span><span class="sxs-lookup"><span data-stu-id="413e7-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="413e7-132">请求</span><span class="sxs-lookup"><span data-stu-id="413e7-132">Request</span></span>
<span data-ttu-id="413e7-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="413e7-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/playLostModeSound
```

### <a name="response"></a><span data-ttu-id="413e7-134">响应</span><span class="sxs-lookup"><span data-stu-id="413e7-134">Response</span></span>
<span data-ttu-id="413e7-135">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="413e7-135">Here is an example of the response.</span></span> <span data-ttu-id="413e7-136">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="413e7-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="413e7-137">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="413e7-137">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



