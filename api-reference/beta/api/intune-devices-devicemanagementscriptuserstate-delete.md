---
title: 删除 deviceManagementScriptUserState
description: 删除 deviceManagementScriptUserState。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2397b08589ee392d89a5270b047eb3c66fc73b00
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42768357"
---
# <a name="delete-devicemanagementscriptuserstate"></a><span data-ttu-id="99905-103">删除 deviceManagementScriptUserState</span><span class="sxs-lookup"><span data-stu-id="99905-103">Delete deviceManagementScriptUserState</span></span>

> <span data-ttu-id="99905-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="99905-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="99905-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="99905-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="99905-106">删除[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)。</span><span class="sxs-lookup"><span data-stu-id="99905-106">Deletes a [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="99905-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="99905-107">Prerequisites</span></span>
<span data-ttu-id="99905-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="99905-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99905-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="99905-110">Permission type</span></span>|<span data-ttu-id="99905-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="99905-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="99905-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="99905-112">Delegated (work or school account)</span></span>|<span data-ttu-id="99905-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99905-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="99905-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="99905-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="99905-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="99905-115">Not supported.</span></span>|
|<span data-ttu-id="99905-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="99905-116">Application</span></span>|<span data-ttu-id="99905-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99905-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="99905-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="99905-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceShellScripts/{deviceShellScriptId}/userRunStates/{deviceManagementScriptUserStateId}
DELETE /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}
```

## <a name="request-headers"></a><span data-ttu-id="99905-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="99905-119">Request headers</span></span>
|<span data-ttu-id="99905-120">标头</span><span class="sxs-lookup"><span data-stu-id="99905-120">Header</span></span>|<span data-ttu-id="99905-121">值</span><span class="sxs-lookup"><span data-stu-id="99905-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="99905-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="99905-122">Authorization</span></span>|<span data-ttu-id="99905-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="99905-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="99905-124">接受</span><span class="sxs-lookup"><span data-stu-id="99905-124">Accept</span></span>|<span data-ttu-id="99905-125">application/json</span><span class="sxs-lookup"><span data-stu-id="99905-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="99905-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="99905-126">Request body</span></span>
<span data-ttu-id="99905-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="99905-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="99905-128">响应</span><span class="sxs-lookup"><span data-stu-id="99905-128">Response</span></span>
<span data-ttu-id="99905-129">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="99905-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="99905-130">示例</span><span class="sxs-lookup"><span data-stu-id="99905-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="99905-131">请求</span><span class="sxs-lookup"><span data-stu-id="99905-131">Request</span></span>
<span data-ttu-id="99905-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="99905-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}/userRunStates/{deviceManagementScriptUserStateId}
```

### <a name="response"></a><span data-ttu-id="99905-133">响应</span><span class="sxs-lookup"><span data-stu-id="99905-133">Response</span></span>
<span data-ttu-id="99905-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="99905-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




