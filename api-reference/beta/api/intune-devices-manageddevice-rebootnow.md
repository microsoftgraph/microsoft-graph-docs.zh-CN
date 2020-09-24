---
title: rebootNow 操作
description: 重新启动设备
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 458ddfe2b7571075c194ef28309f4d57b929b2eb
ms.sourcegitcommit: b7e82d0d64f640a09f5da76b38d8ed9f13684f95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2020
ms.locfileid: "48258422"
---
# <a name="rebootnow-action"></a><span data-ttu-id="91709-103">rebootNow 操作</span><span class="sxs-lookup"><span data-stu-id="91709-103">rebootNow action</span></span>

<span data-ttu-id="91709-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="91709-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

> <span data-ttu-id="91709-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="91709-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="91709-106">重新启动设备。</span><span class="sxs-lookup"><span data-stu-id="91709-106">Reboot device.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="91709-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="91709-107">Prerequisites</span></span>
<span data-ttu-id="91709-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="91709-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91709-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="91709-110">Permission type</span></span>|<span data-ttu-id="91709-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="91709-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="91709-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="91709-112">Delegated (work or school account)</span></span>|<span data-ttu-id="91709-113">DeviceManagementManagedDevices.PrivilegedOperations.All</span><span class="sxs-lookup"><span data-stu-id="91709-113">DeviceManagementManagedDevices.PrivilegedOperations.All</span></span>|
|<span data-ttu-id="91709-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="91709-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="91709-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="91709-115">Not supported.</span></span>|
|<span data-ttu-id="91709-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="91709-116">Application</span></span>|<span data-ttu-id="91709-117">DeviceManagementManagedDevices.PrivilegedOperations.All</span><span class="sxs-lookup"><span data-stu-id="91709-117">DeviceManagementManagedDevices.PrivilegedOperations.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="91709-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="91709-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/rebootNow
POST /deviceManagement/comanagedDevices/{managedDeviceId}/rebootNow
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice/rebootNow
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/rebootNow
POST /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates/{deviceComplianceScriptDeviceStateId}/managedDevice/rebootNow
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/rebootNow
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/rebootNow
```

## <a name="request-headers"></a><span data-ttu-id="91709-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="91709-119">Request headers</span></span>
|<span data-ttu-id="91709-120">标头</span><span class="sxs-lookup"><span data-stu-id="91709-120">Header</span></span>|<span data-ttu-id="91709-121">值</span><span class="sxs-lookup"><span data-stu-id="91709-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="91709-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="91709-122">Authorization</span></span>|<span data-ttu-id="91709-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="91709-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="91709-124">接受</span><span class="sxs-lookup"><span data-stu-id="91709-124">Accept</span></span>|<span data-ttu-id="91709-125">application/json</span><span class="sxs-lookup"><span data-stu-id="91709-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="91709-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="91709-126">Request body</span></span>
<span data-ttu-id="91709-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="91709-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="91709-128">响应</span><span class="sxs-lookup"><span data-stu-id="91709-128">Response</span></span>
<span data-ttu-id="91709-129">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="91709-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="91709-130">示例</span><span class="sxs-lookup"><span data-stu-id="91709-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="91709-131">请求</span><span class="sxs-lookup"><span data-stu-id="91709-131">Request</span></span>
<span data-ttu-id="91709-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="91709-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/rebootNow
```

### <a name="response"></a><span data-ttu-id="91709-133">响应</span><span class="sxs-lookup"><span data-stu-id="91709-133">Response</span></span>
<span data-ttu-id="91709-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="91709-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






