---
title: assign 操作
description: 尚未记录
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d568b92d737f7e4728742f4bf7e08654ebc59cb3
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42800499"
---
# <a name="assign-action"></a><span data-ttu-id="adf84-103">分配操作</span><span class="sxs-lookup"><span data-stu-id="adf84-103">assign action</span></span>

> <span data-ttu-id="adf84-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="adf84-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="adf84-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="adf84-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="adf84-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="adf84-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="adf84-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="adf84-107">Prerequisites</span></span>
<span data-ttu-id="adf84-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="adf84-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="adf84-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="adf84-110">Permission type</span></span>|<span data-ttu-id="adf84-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="adf84-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="adf84-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="adf84-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="adf84-113">&nbsp;&nbsp; **注册**</span><span class="sxs-lookup"><span data-stu-id="adf84-113">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="adf84-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="adf84-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="adf84-115">&nbsp;&nbsp; **策略集**</span><span class="sxs-lookup"><span data-stu-id="adf84-115">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="adf84-116">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="adf84-116">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="adf84-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="adf84-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="adf84-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="adf84-118">Not supported.</span></span>|
|<span data-ttu-id="adf84-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="adf84-119">Application</span></span>||
| <span data-ttu-id="adf84-120">&nbsp;&nbsp; **注册**</span><span class="sxs-lookup"><span data-stu-id="adf84-120">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="adf84-121">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="adf84-121">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="adf84-122">&nbsp;&nbsp; **策略集**</span><span class="sxs-lookup"><span data-stu-id="adf84-122">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="adf84-123">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="adf84-123">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="adf84-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="adf84-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}/assign
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assign
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/intendedDeploymentProfile/assign
```

## <a name="request-headers"></a><span data-ttu-id="adf84-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="adf84-125">Request headers</span></span>
|<span data-ttu-id="adf84-126">标头</span><span class="sxs-lookup"><span data-stu-id="adf84-126">Header</span></span>|<span data-ttu-id="adf84-127">值</span><span class="sxs-lookup"><span data-stu-id="adf84-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="adf84-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="adf84-128">Authorization</span></span>|<span data-ttu-id="adf84-129">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="adf84-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="adf84-130">接受</span><span class="sxs-lookup"><span data-stu-id="adf84-130">Accept</span></span>|<span data-ttu-id="adf84-131">application/json</span><span class="sxs-lookup"><span data-stu-id="adf84-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="adf84-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="adf84-132">Request body</span></span>
<span data-ttu-id="adf84-133">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="adf84-133">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="adf84-134">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="adf84-134">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="adf84-135">属性</span><span class="sxs-lookup"><span data-stu-id="adf84-135">Property</span></span>|<span data-ttu-id="adf84-136">类型</span><span class="sxs-lookup"><span data-stu-id="adf84-136">Type</span></span>|<span data-ttu-id="adf84-137">说明</span><span class="sxs-lookup"><span data-stu-id="adf84-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="adf84-138">deviceIds</span><span class="sxs-lookup"><span data-stu-id="adf84-138">deviceIds</span></span>|<span data-ttu-id="adf84-139">String collection</span><span class="sxs-lookup"><span data-stu-id="adf84-139">String collection</span></span>|<span data-ttu-id="adf84-140">尚未记录</span><span class="sxs-lookup"><span data-stu-id="adf84-140">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="adf84-141">响应</span><span class="sxs-lookup"><span data-stu-id="adf84-141">Response</span></span>
<span data-ttu-id="adf84-142">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="adf84-142">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="adf84-143">示例</span><span class="sxs-lookup"><span data-stu-id="adf84-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="adf84-144">请求</span><span class="sxs-lookup"><span data-stu-id="adf84-144">Request</span></span>
<span data-ttu-id="adf84-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="adf84-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}/assign

Content-type: application/json
Content-length: 51

{
  "deviceIds": [
    "Device Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="adf84-146">响应</span><span class="sxs-lookup"><span data-stu-id="adf84-146">Response</span></span>
<span data-ttu-id="adf84-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="adf84-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```







