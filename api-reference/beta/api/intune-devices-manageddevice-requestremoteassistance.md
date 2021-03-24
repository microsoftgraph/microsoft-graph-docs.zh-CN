---
title: requestRemoteAssistance 操作
description: 请求远程协助
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 04453110a7b324c9c07bf31298f6193a3b64904f
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51136382"
---
# <a name="requestremoteassistance-action"></a><span data-ttu-id="b35ad-103">requestRemoteAssistance 操作</span><span class="sxs-lookup"><span data-stu-id="b35ad-103">requestRemoteAssistance action</span></span>

<span data-ttu-id="b35ad-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b35ad-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b35ad-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b35ad-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b35ad-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b35ad-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b35ad-107">请求远程协助</span><span class="sxs-lookup"><span data-stu-id="b35ad-107">Request remote assistance</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b35ad-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b35ad-108">Prerequisites</span></span>
<span data-ttu-id="b35ad-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b35ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b35ad-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b35ad-111">Permission type</span></span>|<span data-ttu-id="b35ad-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b35ad-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b35ad-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b35ad-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b35ad-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b35ad-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b35ad-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b35ad-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b35ad-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b35ad-116">Not supported.</span></span>|
|<span data-ttu-id="b35ad-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b35ad-117">Application</span></span>|<span data-ttu-id="b35ad-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b35ad-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b35ad-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b35ad-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/requestRemoteAssistance
POST /deviceManagement/comanagedDevices/{managedDeviceId}/requestRemoteAssistance
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice/requestRemoteAssistance
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/requestRemoteAssistance
POST /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates/{deviceComplianceScriptDeviceStateId}/managedDevice/requestRemoteAssistance
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/requestRemoteAssistance
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/requestRemoteAssistance
```

## <a name="request-headers"></a><span data-ttu-id="b35ad-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b35ad-120">Request headers</span></span>
|<span data-ttu-id="b35ad-121">标头</span><span class="sxs-lookup"><span data-stu-id="b35ad-121">Header</span></span>|<span data-ttu-id="b35ad-122">值</span><span class="sxs-lookup"><span data-stu-id="b35ad-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b35ad-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b35ad-123">Authorization</span></span>|<span data-ttu-id="b35ad-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b35ad-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b35ad-125">接受</span><span class="sxs-lookup"><span data-stu-id="b35ad-125">Accept</span></span>|<span data-ttu-id="b35ad-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b35ad-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b35ad-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b35ad-127">Request body</span></span>
<span data-ttu-id="b35ad-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b35ad-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b35ad-129">响应</span><span class="sxs-lookup"><span data-stu-id="b35ad-129">Response</span></span>
<span data-ttu-id="b35ad-130">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="b35ad-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b35ad-131">示例</span><span class="sxs-lookup"><span data-stu-id="b35ad-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="b35ad-132">请求</span><span class="sxs-lookup"><span data-stu-id="b35ad-132">Request</span></span>
<span data-ttu-id="b35ad-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b35ad-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/requestRemoteAssistance
```

### <a name="response"></a><span data-ttu-id="b35ad-134">响应</span><span class="sxs-lookup"><span data-stu-id="b35ad-134">Response</span></span>
<span data-ttu-id="b35ad-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b35ad-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




