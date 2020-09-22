---
title: rotateFileVaultKey 操作
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6b0603afde84bc860d3dfaa78a27b570da6f32f7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48005178"
---
# <a name="rotatefilevaultkey-action"></a><span data-ttu-id="4e18c-103">rotateFileVaultKey 操作</span><span class="sxs-lookup"><span data-stu-id="4e18c-103">rotateFileVaultKey action</span></span>

<span data-ttu-id="4e18c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e18c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4e18c-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4e18c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4e18c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4e18c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4e18c-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="4e18c-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4e18c-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="4e18c-108">Prerequisites</span></span>
<span data-ttu-id="4e18c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4e18c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e18c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="4e18c-111">Permission type</span></span>|<span data-ttu-id="4e18c-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4e18c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4e18c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4e18c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4e18c-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="4e18c-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="4e18c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4e18c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4e18c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4e18c-116">Not supported.</span></span>|
|<span data-ttu-id="4e18c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="4e18c-117">Application</span></span>|<span data-ttu-id="4e18c-118">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="4e18c-118">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4e18c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4e18c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/rotateFileVaultKey
POST /deviceManagement/comanagedDevices/{managedDeviceId}/rotateFileVaultKey
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice/rotateFileVaultKey
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/rotateFileVaultKey
POST /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates/{deviceComplianceScriptDeviceStateId}/managedDevice/rotateFileVaultKey
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/rotateFileVaultKey
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/rotateFileVaultKey
```

## <a name="request-headers"></a><span data-ttu-id="4e18c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="4e18c-120">Request headers</span></span>
|<span data-ttu-id="4e18c-121">标头</span><span class="sxs-lookup"><span data-stu-id="4e18c-121">Header</span></span>|<span data-ttu-id="4e18c-122">值</span><span class="sxs-lookup"><span data-stu-id="4e18c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4e18c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4e18c-123">Authorization</span></span>|<span data-ttu-id="4e18c-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4e18c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4e18c-125">接受</span><span class="sxs-lookup"><span data-stu-id="4e18c-125">Accept</span></span>|<span data-ttu-id="4e18c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4e18c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e18c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="4e18c-127">Request body</span></span>
<span data-ttu-id="4e18c-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4e18c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4e18c-129">响应</span><span class="sxs-lookup"><span data-stu-id="4e18c-129">Response</span></span>
<span data-ttu-id="4e18c-130">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="4e18c-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4e18c-131">示例</span><span class="sxs-lookup"><span data-stu-id="4e18c-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="4e18c-132">请求</span><span class="sxs-lookup"><span data-stu-id="4e18c-132">Request</span></span>
<span data-ttu-id="4e18c-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4e18c-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/rotateFileVaultKey
```

### <a name="response"></a><span data-ttu-id="4e18c-134">响应</span><span class="sxs-lookup"><span data-stu-id="4e18c-134">Response</span></span>
<span data-ttu-id="4e18c-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4e18c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






