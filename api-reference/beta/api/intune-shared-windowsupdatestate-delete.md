---
title: 删除 windowsUpdateState
description: 删除 windowsUpdateState。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f86c4114ccd0cf06313c4a50bdb83d83ae033caf
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42457921"
---
# <a name="delete-windowsupdatestate"></a><span data-ttu-id="2eb0b-103">删除 windowsUpdateState</span><span class="sxs-lookup"><span data-stu-id="2eb0b-103">Delete windowsUpdateState</span></span>

<span data-ttu-id="2eb0b-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="2eb0b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2eb0b-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2eb0b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2eb0b-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2eb0b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2eb0b-107">删除[windowsUpdateState](../resources/intune-shared-windowsupdatestate.md)。</span><span class="sxs-lookup"><span data-stu-id="2eb0b-107">Deletes a [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2eb0b-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="2eb0b-108">Prerequisites</span></span>
<span data-ttu-id="2eb0b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2eb0b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2eb0b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="2eb0b-111">Permission type</span></span>|<span data-ttu-id="2eb0b-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2eb0b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2eb0b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2eb0b-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="2eb0b-114">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="2eb0b-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="2eb0b-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2eb0b-115">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="2eb0b-116">&nbsp;&nbsp; **软件更新**</span><span class="sxs-lookup"><span data-stu-id="2eb0b-116">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="2eb0b-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2eb0b-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2eb0b-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2eb0b-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2eb0b-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="2eb0b-119">Not supported.</span></span>|
|<span data-ttu-id="2eb0b-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="2eb0b-120">Application</span></span>||
| <span data-ttu-id="2eb0b-121">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="2eb0b-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="2eb0b-122">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2eb0b-122">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="2eb0b-123">&nbsp;&nbsp; **软件更新**</span><span class="sxs-lookup"><span data-stu-id="2eb0b-123">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="2eb0b-124">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2eb0b-124">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2eb0b-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2eb0b-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates/{windowsUpdateStateId}
```

## <a name="request-headers"></a><span data-ttu-id="2eb0b-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="2eb0b-126">Request headers</span></span>
|<span data-ttu-id="2eb0b-127">标头</span><span class="sxs-lookup"><span data-stu-id="2eb0b-127">Header</span></span>|<span data-ttu-id="2eb0b-128">值</span><span class="sxs-lookup"><span data-stu-id="2eb0b-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2eb0b-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="2eb0b-129">Authorization</span></span>|<span data-ttu-id="2eb0b-130">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2eb0b-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2eb0b-131">接受</span><span class="sxs-lookup"><span data-stu-id="2eb0b-131">Accept</span></span>|<span data-ttu-id="2eb0b-132">application/json</span><span class="sxs-lookup"><span data-stu-id="2eb0b-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2eb0b-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="2eb0b-133">Request body</span></span>
<span data-ttu-id="2eb0b-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2eb0b-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2eb0b-135">响应</span><span class="sxs-lookup"><span data-stu-id="2eb0b-135">Response</span></span>
<span data-ttu-id="2eb0b-136">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="2eb0b-136">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2eb0b-137">示例</span><span class="sxs-lookup"><span data-stu-id="2eb0b-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="2eb0b-138">请求</span><span class="sxs-lookup"><span data-stu-id="2eb0b-138">Request</span></span>
<span data-ttu-id="2eb0b-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2eb0b-139">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates/{windowsUpdateStateId}
```

### <a name="response"></a><span data-ttu-id="2eb0b-140">响应</span><span class="sxs-lookup"><span data-stu-id="2eb0b-140">Response</span></span>
<span data-ttu-id="2eb0b-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2eb0b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```








