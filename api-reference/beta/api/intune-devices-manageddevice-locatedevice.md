---
title: locateDevice 操作
description: 查找设备
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 359acf411ff80fc655d475ca1828b643f1f3a3a3
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51149987"
---
# <a name="locatedevice-action"></a><span data-ttu-id="a5a25-103">locateDevice 操作</span><span class="sxs-lookup"><span data-stu-id="a5a25-103">locateDevice action</span></span>

<span data-ttu-id="a5a25-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a5a25-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a5a25-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a5a25-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a5a25-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a5a25-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a5a25-107">查找设备</span><span class="sxs-lookup"><span data-stu-id="a5a25-107">Locate a device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a5a25-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="a5a25-108">Prerequisites</span></span>
<span data-ttu-id="a5a25-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a5a25-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5a25-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a5a25-111">Permission type</span></span>|<span data-ttu-id="a5a25-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a5a25-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a5a25-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a5a25-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a5a25-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="a5a25-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="a5a25-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a5a25-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a5a25-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a5a25-116">Not supported.</span></span>|
|<span data-ttu-id="a5a25-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a5a25-117">Application</span></span>|<span data-ttu-id="a5a25-118">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="a5a25-118">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a5a25-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a5a25-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/locateDevice
POST /deviceManagement/comanagedDevices/{managedDeviceId}/locateDevice
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice/locateDevice
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/locateDevice
POST /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates/{deviceComplianceScriptDeviceStateId}/managedDevice/locateDevice
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/locateDevice
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/locateDevice
```

## <a name="request-headers"></a><span data-ttu-id="a5a25-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a5a25-120">Request headers</span></span>
|<span data-ttu-id="a5a25-121">标头</span><span class="sxs-lookup"><span data-stu-id="a5a25-121">Header</span></span>|<span data-ttu-id="a5a25-122">值</span><span class="sxs-lookup"><span data-stu-id="a5a25-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a5a25-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a5a25-123">Authorization</span></span>|<span data-ttu-id="a5a25-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a5a25-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a5a25-125">接受</span><span class="sxs-lookup"><span data-stu-id="a5a25-125">Accept</span></span>|<span data-ttu-id="a5a25-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a5a25-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a5a25-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a5a25-127">Request body</span></span>
<span data-ttu-id="a5a25-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a5a25-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a5a25-129">响应</span><span class="sxs-lookup"><span data-stu-id="a5a25-129">Response</span></span>
<span data-ttu-id="a5a25-130">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="a5a25-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a5a25-131">示例</span><span class="sxs-lookup"><span data-stu-id="a5a25-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="a5a25-132">请求</span><span class="sxs-lookup"><span data-stu-id="a5a25-132">Request</span></span>
<span data-ttu-id="a5a25-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a5a25-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/locateDevice
```

### <a name="response"></a><span data-ttu-id="a5a25-134">响应</span><span class="sxs-lookup"><span data-stu-id="a5a25-134">Response</span></span>
<span data-ttu-id="a5a25-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a5a25-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




