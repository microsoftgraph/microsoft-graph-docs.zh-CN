---
title: remoteLock 操作
description: 远程锁定
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e611d90c0e453b6e82f436d386f7df79d889b510
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30157202"
---
# <a name="remotelock-action"></a><span data-ttu-id="7716b-103">remoteLock 操作</span><span class="sxs-lookup"><span data-stu-id="7716b-103">remoteLock action</span></span>

> <span data-ttu-id="7716b-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7716b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7716b-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7716b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7716b-106">远程锁定</span><span class="sxs-lookup"><span data-stu-id="7716b-106">Remote lock</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7716b-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="7716b-107">Prerequisites</span></span>
<span data-ttu-id="7716b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="7716b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="7716b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="7716b-110">Permission type</span></span>|<span data-ttu-id="7716b-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7716b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7716b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7716b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7716b-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="7716b-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="7716b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7716b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7716b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="7716b-115">Not supported.</span></span>|
|<span data-ttu-id="7716b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="7716b-116">Application</span></span>|<span data-ttu-id="7716b-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="7716b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7716b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7716b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/remoteLock
POST /deviceManagement/managedDevices/{managedDeviceId}/remoteLock
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/remoteLock
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/remoteLock
```

## <a name="request-headers"></a><span data-ttu-id="7716b-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="7716b-119">Request headers</span></span>
|<span data-ttu-id="7716b-120">标头</span><span class="sxs-lookup"><span data-stu-id="7716b-120">Header</span></span>|<span data-ttu-id="7716b-121">值</span><span class="sxs-lookup"><span data-stu-id="7716b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7716b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7716b-122">Authorization</span></span>|<span data-ttu-id="7716b-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7716b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7716b-124">Accept</span><span class="sxs-lookup"><span data-stu-id="7716b-124">Accept</span></span>|<span data-ttu-id="7716b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7716b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7716b-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="7716b-126">Request body</span></span>
<span data-ttu-id="7716b-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7716b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7716b-128">响应</span><span class="sxs-lookup"><span data-stu-id="7716b-128">Response</span></span>
<span data-ttu-id="7716b-129">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="7716b-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7716b-130">示例</span><span class="sxs-lookup"><span data-stu-id="7716b-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="7716b-131">请求</span><span class="sxs-lookup"><span data-stu-id="7716b-131">Request</span></span>
<span data-ttu-id="7716b-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7716b-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/managedDevices/{managedDeviceId}/remoteLock
```

### <a name="response"></a><span data-ttu-id="7716b-133">响应</span><span class="sxs-lookup"><span data-stu-id="7716b-133">Response</span></span>
<span data-ttu-id="7716b-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7716b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




