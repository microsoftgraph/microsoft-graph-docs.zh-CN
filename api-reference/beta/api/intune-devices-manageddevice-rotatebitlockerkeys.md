---
title: rotateBitLockerKeys 操作
description: 旋转 BitLockerKeys
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b4bb754e922d9c52129d1d4fdb7992c80654c03b
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49234858"
---
# <a name="rotatebitlockerkeys-action"></a><span data-ttu-id="da807-103">rotateBitLockerKeys 操作</span><span class="sxs-lookup"><span data-stu-id="da807-103">rotateBitLockerKeys action</span></span>

<span data-ttu-id="da807-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="da807-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="da807-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="da807-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="da807-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="da807-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="da807-107">旋转 BitLockerKeys</span><span class="sxs-lookup"><span data-stu-id="da807-107">Rotate BitLockerKeys</span></span>

## <a name="prerequisites"></a><span data-ttu-id="da807-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="da807-108">Prerequisites</span></span>
<span data-ttu-id="da807-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="da807-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da807-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="da807-111">Permission type</span></span>|<span data-ttu-id="da807-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="da807-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="da807-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="da807-113">Delegated (work or school account)</span></span>|<span data-ttu-id="da807-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da807-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="da807-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="da807-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="da807-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="da807-116">Not supported.</span></span>|
|<span data-ttu-id="da807-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="da807-117">Application</span></span>|<span data-ttu-id="da807-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da807-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="da807-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="da807-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/rotateBitLockerKeys
POST /deviceManagement/comanagedDevices/{managedDeviceId}/rotateBitLockerKeys
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice/rotateBitLockerKeys
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/rotateBitLockerKeys
POST /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates/{deviceComplianceScriptDeviceStateId}/managedDevice/rotateBitLockerKeys
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/rotateBitLockerKeys
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/rotateBitLockerKeys
```

## <a name="request-headers"></a><span data-ttu-id="da807-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="da807-120">Request headers</span></span>
|<span data-ttu-id="da807-121">标头</span><span class="sxs-lookup"><span data-stu-id="da807-121">Header</span></span>|<span data-ttu-id="da807-122">值</span><span class="sxs-lookup"><span data-stu-id="da807-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="da807-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="da807-123">Authorization</span></span>|<span data-ttu-id="da807-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="da807-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="da807-125">接受</span><span class="sxs-lookup"><span data-stu-id="da807-125">Accept</span></span>|<span data-ttu-id="da807-126">application/json</span><span class="sxs-lookup"><span data-stu-id="da807-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="da807-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="da807-127">Request body</span></span>
<span data-ttu-id="da807-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="da807-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="da807-129">响应</span><span class="sxs-lookup"><span data-stu-id="da807-129">Response</span></span>
<span data-ttu-id="da807-130">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="da807-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="da807-131">示例</span><span class="sxs-lookup"><span data-stu-id="da807-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="da807-132">请求</span><span class="sxs-lookup"><span data-stu-id="da807-132">Request</span></span>
<span data-ttu-id="da807-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="da807-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/rotateBitLockerKeys
```

### <a name="response"></a><span data-ttu-id="da807-134">响应</span><span class="sxs-lookup"><span data-stu-id="da807-134">Response</span></span>
<span data-ttu-id="da807-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="da807-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




