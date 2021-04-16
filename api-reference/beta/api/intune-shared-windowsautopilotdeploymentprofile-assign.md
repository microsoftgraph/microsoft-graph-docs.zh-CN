---
title: assign 操作
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b2c13bd6798c6a73b953b3f273c76a9dee1365ab
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868069"
---
# <a name="assign-action"></a><span data-ttu-id="7f4e8-103">分配操作</span><span class="sxs-lookup"><span data-stu-id="7f4e8-103">assign action</span></span>

<span data-ttu-id="7f4e8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f4e8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7f4e8-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7f4e8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7f4e8-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7f4e8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f4e8-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="7f4e8-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7f4e8-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="7f4e8-108">Prerequisites</span></span>
<span data-ttu-id="7f4e8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7f4e8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f4e8-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7f4e8-111">Permission type</span></span>|<span data-ttu-id="7f4e8-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7f4e8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7f4e8-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7f4e8-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="7f4e8-114">&nbsp;&nbsp;**注册**</span><span class="sxs-lookup"><span data-stu-id="7f4e8-114">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="7f4e8-115">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f4e8-115">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="7f4e8-116">&nbsp;&nbsp;**策略集**</span><span class="sxs-lookup"><span data-stu-id="7f4e8-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="7f4e8-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f4e8-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7f4e8-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7f4e8-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7f4e8-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="7f4e8-119">Not supported.</span></span>|
|<span data-ttu-id="7f4e8-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="7f4e8-120">Application</span></span>||
| <span data-ttu-id="7f4e8-121">&nbsp;&nbsp;**注册**</span><span class="sxs-lookup"><span data-stu-id="7f4e8-121">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="7f4e8-122">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f4e8-122">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="7f4e8-123">&nbsp;&nbsp;**策略集**</span><span class="sxs-lookup"><span data-stu-id="7f4e8-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="7f4e8-124">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f4e8-124">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7f4e8-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7f4e8-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}/assign
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assign
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/intendedDeploymentProfile/assign
```

## <a name="request-headers"></a><span data-ttu-id="7f4e8-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="7f4e8-126">Request headers</span></span>
|<span data-ttu-id="7f4e8-127">标头</span><span class="sxs-lookup"><span data-stu-id="7f4e8-127">Header</span></span>|<span data-ttu-id="7f4e8-128">值</span><span class="sxs-lookup"><span data-stu-id="7f4e8-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7f4e8-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f4e8-129">Authorization</span></span>|<span data-ttu-id="7f4e8-130">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7f4e8-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7f4e8-131">接受</span><span class="sxs-lookup"><span data-stu-id="7f4e8-131">Accept</span></span>|<span data-ttu-id="7f4e8-132">application/json</span><span class="sxs-lookup"><span data-stu-id="7f4e8-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f4e8-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="7f4e8-133">Request body</span></span>
<span data-ttu-id="7f4e8-134">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7f4e8-134">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="7f4e8-135">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="7f4e8-135">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="7f4e8-136">属性</span><span class="sxs-lookup"><span data-stu-id="7f4e8-136">Property</span></span>|<span data-ttu-id="7f4e8-137">类型</span><span class="sxs-lookup"><span data-stu-id="7f4e8-137">Type</span></span>|<span data-ttu-id="7f4e8-138">说明</span><span class="sxs-lookup"><span data-stu-id="7f4e8-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f4e8-139">deviceIds</span><span class="sxs-lookup"><span data-stu-id="7f4e8-139">deviceIds</span></span>|<span data-ttu-id="7f4e8-140">String collection</span><span class="sxs-lookup"><span data-stu-id="7f4e8-140">String collection</span></span>|<span data-ttu-id="7f4e8-141">尚未记录</span><span class="sxs-lookup"><span data-stu-id="7f4e8-141">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="7f4e8-142">响应</span><span class="sxs-lookup"><span data-stu-id="7f4e8-142">Response</span></span>
<span data-ttu-id="7f4e8-143">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="7f4e8-143">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7f4e8-144">示例</span><span class="sxs-lookup"><span data-stu-id="7f4e8-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="7f4e8-145">请求</span><span class="sxs-lookup"><span data-stu-id="7f4e8-145">Request</span></span>
<span data-ttu-id="7f4e8-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7f4e8-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7f4e8-147">响应</span><span class="sxs-lookup"><span data-stu-id="7f4e8-147">Response</span></span>
<span data-ttu-id="7f4e8-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7f4e8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```







