---
title: windowsDefenderScan 操作
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c2f0f26cc0f0694358d01b746293c1c0660cc583
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48072443"
---
# <a name="windowsdefenderscan-action"></a><span data-ttu-id="e6945-103">windowsDefenderScan 操作</span><span class="sxs-lookup"><span data-stu-id="e6945-103">windowsDefenderScan action</span></span>

<span data-ttu-id="e6945-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e6945-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e6945-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e6945-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e6945-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e6945-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e6945-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e6945-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e6945-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="e6945-108">Prerequisites</span></span>
<span data-ttu-id="e6945-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e6945-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e6945-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e6945-111">Permission type</span></span>|<span data-ttu-id="e6945-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e6945-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e6945-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e6945-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e6945-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="e6945-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="e6945-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e6945-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e6945-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e6945-116">Not supported.</span></span>|
|<span data-ttu-id="e6945-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e6945-117">Application</span></span>|<span data-ttu-id="e6945-118">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="e6945-118">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e6945-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e6945-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/windowsDefenderScan
POST /deviceManagement/comanagedDevices/{managedDeviceId}/windowsDefenderScan
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice/windowsDefenderScan
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/windowsDefenderScan
POST /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates/{deviceComplianceScriptDeviceStateId}/managedDevice/windowsDefenderScan
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/windowsDefenderScan
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/windowsDefenderScan
```

## <a name="request-headers"></a><span data-ttu-id="e6945-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e6945-120">Request headers</span></span>
|<span data-ttu-id="e6945-121">标头</span><span class="sxs-lookup"><span data-stu-id="e6945-121">Header</span></span>|<span data-ttu-id="e6945-122">值</span><span class="sxs-lookup"><span data-stu-id="e6945-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e6945-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e6945-123">Authorization</span></span>|<span data-ttu-id="e6945-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e6945-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e6945-125">接受</span><span class="sxs-lookup"><span data-stu-id="e6945-125">Accept</span></span>|<span data-ttu-id="e6945-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e6945-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e6945-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e6945-127">Request body</span></span>
<span data-ttu-id="e6945-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e6945-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="e6945-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="e6945-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="e6945-130">属性</span><span class="sxs-lookup"><span data-stu-id="e6945-130">Property</span></span>|<span data-ttu-id="e6945-131">类型</span><span class="sxs-lookup"><span data-stu-id="e6945-131">Type</span></span>|<span data-ttu-id="e6945-132">说明</span><span class="sxs-lookup"><span data-stu-id="e6945-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6945-133">quickScan</span><span class="sxs-lookup"><span data-stu-id="e6945-133">quickScan</span></span>|<span data-ttu-id="e6945-134">布尔</span><span class="sxs-lookup"><span data-stu-id="e6945-134">Boolean</span></span>|<span data-ttu-id="e6945-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e6945-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="e6945-136">响应</span><span class="sxs-lookup"><span data-stu-id="e6945-136">Response</span></span>
<span data-ttu-id="e6945-137">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="e6945-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e6945-138">示例</span><span class="sxs-lookup"><span data-stu-id="e6945-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="e6945-139">请求</span><span class="sxs-lookup"><span data-stu-id="e6945-139">Request</span></span>
<span data-ttu-id="e6945-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e6945-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/windowsDefenderScan

Content-type: application/json
Content-length: 25

{
  "quickScan": true
}
```

### <a name="response"></a><span data-ttu-id="e6945-141">响应</span><span class="sxs-lookup"><span data-stu-id="e6945-141">Response</span></span>
<span data-ttu-id="e6945-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e6945-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






