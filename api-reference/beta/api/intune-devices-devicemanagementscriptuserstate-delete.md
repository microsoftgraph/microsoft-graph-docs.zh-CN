---
title: 删除 deviceManagementScriptUserState
description: 删除 deviceManagementScriptUserState。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d837f98d3daa4450b196f414a7a90ff4d505484f
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51150344"
---
# <a name="delete-devicemanagementscriptuserstate"></a><span data-ttu-id="7f0e8-103">删除 deviceManagementScriptUserState</span><span class="sxs-lookup"><span data-stu-id="7f0e8-103">Delete deviceManagementScriptUserState</span></span>

<span data-ttu-id="7f0e8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f0e8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7f0e8-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7f0e8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7f0e8-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7f0e8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f0e8-107">删除 [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)。</span><span class="sxs-lookup"><span data-stu-id="7f0e8-107">Deletes a [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7f0e8-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="7f0e8-108">Prerequisites</span></span>
<span data-ttu-id="7f0e8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7f0e8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f0e8-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7f0e8-111">Permission type</span></span>|<span data-ttu-id="7f0e8-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7f0e8-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7f0e8-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7f0e8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7f0e8-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f0e8-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="7f0e8-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7f0e8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7f0e8-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7f0e8-116">Not supported.</span></span>|
|<span data-ttu-id="7f0e8-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="7f0e8-117">Application</span></span>|<span data-ttu-id="7f0e8-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f0e8-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7f0e8-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7f0e8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceShellScripts/{deviceShellScriptId}/userRunStates/{deviceManagementScriptUserStateId}
DELETE /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}
DELETE /deviceManagement/deviceCustomAttributeShellScripts/{deviceCustomAttributeShellScriptId}/userRunStates/{deviceManagementScriptUserStateId}
```

## <a name="request-headers"></a><span data-ttu-id="7f0e8-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="7f0e8-120">Request headers</span></span>
|<span data-ttu-id="7f0e8-121">标头</span><span class="sxs-lookup"><span data-stu-id="7f0e8-121">Header</span></span>|<span data-ttu-id="7f0e8-122">值</span><span class="sxs-lookup"><span data-stu-id="7f0e8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7f0e8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f0e8-123">Authorization</span></span>|<span data-ttu-id="7f0e8-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7f0e8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7f0e8-125">接受</span><span class="sxs-lookup"><span data-stu-id="7f0e8-125">Accept</span></span>|<span data-ttu-id="7f0e8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7f0e8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f0e8-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7f0e8-127">Request body</span></span>
<span data-ttu-id="7f0e8-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7f0e8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7f0e8-129">响应</span><span class="sxs-lookup"><span data-stu-id="7f0e8-129">Response</span></span>
<span data-ttu-id="7f0e8-130">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="7f0e8-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7f0e8-131">示例</span><span class="sxs-lookup"><span data-stu-id="7f0e8-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="7f0e8-132">请求</span><span class="sxs-lookup"><span data-stu-id="7f0e8-132">Request</span></span>
<span data-ttu-id="7f0e8-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7f0e8-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}/userRunStates/{deviceManagementScriptUserStateId}
```

### <a name="response"></a><span data-ttu-id="7f0e8-134">响应</span><span class="sxs-lookup"><span data-stu-id="7f0e8-134">Response</span></span>
<span data-ttu-id="7f0e8-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7f0e8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




