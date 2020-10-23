---
title: assign 操作
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b2f461e5933236f38f5fae55c6249de7e0b102e7
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48702815"
---
# <a name="assign-action"></a><span data-ttu-id="24de4-103">分配操作</span><span class="sxs-lookup"><span data-stu-id="24de4-103">assign action</span></span>

<span data-ttu-id="24de4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="24de4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="24de4-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="24de4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="24de4-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="24de4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24de4-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="24de4-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="24de4-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="24de4-108">Prerequisites</span></span>
<span data-ttu-id="24de4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="24de4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24de4-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="24de4-111">Permission type</span></span>|<span data-ttu-id="24de4-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="24de4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="24de4-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="24de4-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="24de4-114">&nbsp;&nbsp;**注册**</span><span class="sxs-lookup"><span data-stu-id="24de4-114">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="24de4-115">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24de4-115">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="24de4-116">&nbsp;&nbsp;**策略集**</span><span class="sxs-lookup"><span data-stu-id="24de4-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="24de4-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24de4-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="24de4-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="24de4-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="24de4-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="24de4-119">Not supported.</span></span>|
|<span data-ttu-id="24de4-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="24de4-120">Application</span></span>||
| <span data-ttu-id="24de4-121">&nbsp;&nbsp;**注册**</span><span class="sxs-lookup"><span data-stu-id="24de4-121">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="24de4-122">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24de4-122">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="24de4-123">&nbsp;&nbsp;**策略集**</span><span class="sxs-lookup"><span data-stu-id="24de4-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="24de4-124">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24de4-124">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="24de4-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="24de4-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}/assign
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assign
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/intendedDeploymentProfile/assign
```

## <a name="request-headers"></a><span data-ttu-id="24de4-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="24de4-126">Request headers</span></span>
|<span data-ttu-id="24de4-127">标头</span><span class="sxs-lookup"><span data-stu-id="24de4-127">Header</span></span>|<span data-ttu-id="24de4-128">值</span><span class="sxs-lookup"><span data-stu-id="24de4-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="24de4-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="24de4-129">Authorization</span></span>|<span data-ttu-id="24de4-130">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="24de4-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="24de4-131">接受</span><span class="sxs-lookup"><span data-stu-id="24de4-131">Accept</span></span>|<span data-ttu-id="24de4-132">application/json</span><span class="sxs-lookup"><span data-stu-id="24de4-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="24de4-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="24de4-133">Request body</span></span>
<span data-ttu-id="24de4-134">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="24de4-134">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="24de4-135">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="24de4-135">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="24de4-136">属性</span><span class="sxs-lookup"><span data-stu-id="24de4-136">Property</span></span>|<span data-ttu-id="24de4-137">类型</span><span class="sxs-lookup"><span data-stu-id="24de4-137">Type</span></span>|<span data-ttu-id="24de4-138">说明</span><span class="sxs-lookup"><span data-stu-id="24de4-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24de4-139">deviceIds</span><span class="sxs-lookup"><span data-stu-id="24de4-139">deviceIds</span></span>|<span data-ttu-id="24de4-140">String collection</span><span class="sxs-lookup"><span data-stu-id="24de4-140">String collection</span></span>|<span data-ttu-id="24de4-141">尚未记录</span><span class="sxs-lookup"><span data-stu-id="24de4-141">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="24de4-142">响应</span><span class="sxs-lookup"><span data-stu-id="24de4-142">Response</span></span>
<span data-ttu-id="24de4-143">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="24de4-143">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="24de4-144">示例</span><span class="sxs-lookup"><span data-stu-id="24de4-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="24de4-145">请求</span><span class="sxs-lookup"><span data-stu-id="24de4-145">Request</span></span>
<span data-ttu-id="24de4-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="24de4-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="24de4-147">响应</span><span class="sxs-lookup"><span data-stu-id="24de4-147">Response</span></span>
<span data-ttu-id="24de4-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="24de4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```








