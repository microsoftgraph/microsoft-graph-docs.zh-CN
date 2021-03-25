---
title: updateWindowsDeviceAccount 操作
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d3645b1aa22c01bfc8f9d317e0d1c21e771570c9
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51158323"
---
# <a name="updatewindowsdeviceaccount-action"></a><span data-ttu-id="420ee-103">updateWindowsDeviceAccount 操作</span><span class="sxs-lookup"><span data-stu-id="420ee-103">updateWindowsDeviceAccount action</span></span>

<span data-ttu-id="420ee-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="420ee-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="420ee-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="420ee-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="420ee-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="420ee-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="420ee-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="420ee-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="420ee-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="420ee-108">Prerequisites</span></span>
<span data-ttu-id="420ee-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="420ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="420ee-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="420ee-111">Permission type</span></span>|<span data-ttu-id="420ee-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="420ee-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="420ee-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="420ee-113">Delegated (work or school account)</span></span>|<span data-ttu-id="420ee-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="420ee-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="420ee-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="420ee-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="420ee-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="420ee-116">Not supported.</span></span>|
|<span data-ttu-id="420ee-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="420ee-117">Application</span></span>|<span data-ttu-id="420ee-118">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="420ee-118">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="420ee-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="420ee-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/updateWindowsDeviceAccount
POST /deviceManagement/comanagedDevices/{managedDeviceId}/updateWindowsDeviceAccount
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice/updateWindowsDeviceAccount
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/updateWindowsDeviceAccount
POST /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates/{deviceComplianceScriptDeviceStateId}/managedDevice/updateWindowsDeviceAccount
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/updateWindowsDeviceAccount
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/updateWindowsDeviceAccount
```

## <a name="request-headers"></a><span data-ttu-id="420ee-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="420ee-120">Request headers</span></span>
|<span data-ttu-id="420ee-121">标头</span><span class="sxs-lookup"><span data-stu-id="420ee-121">Header</span></span>|<span data-ttu-id="420ee-122">值</span><span class="sxs-lookup"><span data-stu-id="420ee-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="420ee-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="420ee-123">Authorization</span></span>|<span data-ttu-id="420ee-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="420ee-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="420ee-125">接受</span><span class="sxs-lookup"><span data-stu-id="420ee-125">Accept</span></span>|<span data-ttu-id="420ee-126">application/json</span><span class="sxs-lookup"><span data-stu-id="420ee-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="420ee-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="420ee-127">Request body</span></span>
<span data-ttu-id="420ee-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="420ee-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="420ee-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="420ee-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="420ee-130">属性</span><span class="sxs-lookup"><span data-stu-id="420ee-130">Property</span></span>|<span data-ttu-id="420ee-131">类型</span><span class="sxs-lookup"><span data-stu-id="420ee-131">Type</span></span>|<span data-ttu-id="420ee-132">说明</span><span class="sxs-lookup"><span data-stu-id="420ee-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="420ee-133">updateWindowsDeviceAccountActionParameter</span><span class="sxs-lookup"><span data-stu-id="420ee-133">updateWindowsDeviceAccountActionParameter</span></span>|[<span data-ttu-id="420ee-134">updateWindowsDeviceAccountActionParameter</span><span class="sxs-lookup"><span data-stu-id="420ee-134">updateWindowsDeviceAccountActionParameter</span></span>](../resources/intune-devices-updatewindowsdeviceaccountactionparameter.md)|<span data-ttu-id="420ee-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="420ee-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="420ee-136">响应</span><span class="sxs-lookup"><span data-stu-id="420ee-136">Response</span></span>
<span data-ttu-id="420ee-137">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="420ee-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="420ee-138">示例</span><span class="sxs-lookup"><span data-stu-id="420ee-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="420ee-139">请求</span><span class="sxs-lookup"><span data-stu-id="420ee-139">Request</span></span>
<span data-ttu-id="420ee-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="420ee-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/updateWindowsDeviceAccount

Content-type: application/json
Content-length: 532

{
  "updateWindowsDeviceAccountActionParameter": {
    "@odata.type": "microsoft.graph.updateWindowsDeviceAccountActionParameter",
    "deviceAccount": {
      "@odata.type": "microsoft.graph.windowsDeviceAccount",
      "password": "Password value"
    },
    "passwordRotationEnabled": true,
    "calendarSyncEnabled": true,
    "deviceAccountEmail": "Device Account Email value",
    "exchangeServer": "Exchange Server value",
    "sessionInitiationProtocalAddress": "Session Initiation Protocal Address value"
  }
}
```

### <a name="response"></a><span data-ttu-id="420ee-141">响应</span><span class="sxs-lookup"><span data-stu-id="420ee-141">Response</span></span>
<span data-ttu-id="420ee-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="420ee-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




