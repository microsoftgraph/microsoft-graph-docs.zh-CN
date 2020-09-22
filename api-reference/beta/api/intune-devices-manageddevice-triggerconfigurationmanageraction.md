---
title: triggerConfigurationManagerAction 操作
description: ConfigurationManager 客户端上的触发操作
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d16e3b278755b53f42f5b4203032306fd332855b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48050701"
---
# <a name="triggerconfigurationmanageraction-action"></a><span data-ttu-id="42477-103">triggerConfigurationManagerAction 操作</span><span class="sxs-lookup"><span data-stu-id="42477-103">triggerConfigurationManagerAction action</span></span>

<span data-ttu-id="42477-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42477-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="42477-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="42477-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="42477-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="42477-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42477-107">ConfigurationManager 客户端上的触发操作</span><span class="sxs-lookup"><span data-stu-id="42477-107">Trigger action on ConfigurationManager client</span></span>

## <a name="prerequisites"></a><span data-ttu-id="42477-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="42477-108">Prerequisites</span></span>
<span data-ttu-id="42477-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="42477-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42477-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="42477-111">Permission type</span></span>|<span data-ttu-id="42477-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="42477-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="42477-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="42477-113">Delegated (work or school account)</span></span>|<span data-ttu-id="42477-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="42477-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="42477-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="42477-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="42477-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="42477-116">Not supported.</span></span>|
|<span data-ttu-id="42477-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="42477-117">Application</span></span>|<span data-ttu-id="42477-118">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="42477-118">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="42477-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="42477-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/triggerConfigurationManagerAction
POST /deviceManagement/comanagedDevices/{managedDeviceId}/triggerConfigurationManagerAction
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice/triggerConfigurationManagerAction
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/triggerConfigurationManagerAction
POST /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates/{deviceComplianceScriptDeviceStateId}/managedDevice/triggerConfigurationManagerAction
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/triggerConfigurationManagerAction
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/triggerConfigurationManagerAction
```

## <a name="request-headers"></a><span data-ttu-id="42477-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="42477-120">Request headers</span></span>
|<span data-ttu-id="42477-121">标头</span><span class="sxs-lookup"><span data-stu-id="42477-121">Header</span></span>|<span data-ttu-id="42477-122">值</span><span class="sxs-lookup"><span data-stu-id="42477-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="42477-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="42477-123">Authorization</span></span>|<span data-ttu-id="42477-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="42477-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="42477-125">接受</span><span class="sxs-lookup"><span data-stu-id="42477-125">Accept</span></span>|<span data-ttu-id="42477-126">application/json</span><span class="sxs-lookup"><span data-stu-id="42477-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="42477-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="42477-127">Request body</span></span>
<span data-ttu-id="42477-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="42477-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="42477-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="42477-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="42477-130">属性</span><span class="sxs-lookup"><span data-stu-id="42477-130">Property</span></span>|<span data-ttu-id="42477-131">类型</span><span class="sxs-lookup"><span data-stu-id="42477-131">Type</span></span>|<span data-ttu-id="42477-132">说明</span><span class="sxs-lookup"><span data-stu-id="42477-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42477-133">configurationManagerAction</span><span class="sxs-lookup"><span data-stu-id="42477-133">configurationManagerAction</span></span>|[<span data-ttu-id="42477-134">configurationManagerAction</span><span class="sxs-lookup"><span data-stu-id="42477-134">configurationManagerAction</span></span>](../resources/intune-devices-configurationmanageraction.md)|<span data-ttu-id="42477-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="42477-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="42477-136">响应</span><span class="sxs-lookup"><span data-stu-id="42477-136">Response</span></span>
<span data-ttu-id="42477-137">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="42477-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="42477-138">示例</span><span class="sxs-lookup"><span data-stu-id="42477-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="42477-139">请求</span><span class="sxs-lookup"><span data-stu-id="42477-139">Request</span></span>
<span data-ttu-id="42477-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="42477-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/triggerConfigurationManagerAction

Content-type: application/json
Content-length: 145

{
  "configurationManagerAction": {
    "@odata.type": "microsoft.graph.configurationManagerAction",
    "action": "refreshUserPolicy"
  }
}
```

### <a name="response"></a><span data-ttu-id="42477-141">响应</span><span class="sxs-lookup"><span data-stu-id="42477-141">Response</span></span>
<span data-ttu-id="42477-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="42477-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






