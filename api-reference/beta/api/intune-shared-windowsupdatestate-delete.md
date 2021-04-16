---
title: 删除 windowsUpdateState
description: 删除 windowsUpdateState。
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 75212db281d3d14b27f69ff3e342f7af33ffb513
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51863028"
---
# <a name="delete-windowsupdatestate"></a><span data-ttu-id="2736d-103">删除 windowsUpdateState</span><span class="sxs-lookup"><span data-stu-id="2736d-103">Delete windowsUpdateState</span></span>

<span data-ttu-id="2736d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2736d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2736d-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2736d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2736d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2736d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2736d-107">删除 [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md)。</span><span class="sxs-lookup"><span data-stu-id="2736d-107">Deletes a [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2736d-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="2736d-108">Prerequisites</span></span>
<span data-ttu-id="2736d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2736d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2736d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="2736d-111">Permission type</span></span>|<span data-ttu-id="2736d-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2736d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2736d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2736d-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="2736d-114">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="2736d-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="2736d-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2736d-115">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="2736d-116">&nbsp;&nbsp;**软件更新**</span><span class="sxs-lookup"><span data-stu-id="2736d-116">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="2736d-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2736d-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2736d-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2736d-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2736d-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="2736d-119">Not supported.</span></span>|
|<span data-ttu-id="2736d-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="2736d-120">Application</span></span>||
| <span data-ttu-id="2736d-121">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="2736d-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="2736d-122">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2736d-122">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="2736d-123">&nbsp;&nbsp;**软件更新**</span><span class="sxs-lookup"><span data-stu-id="2736d-123">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="2736d-124">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2736d-124">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2736d-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2736d-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates/{windowsUpdateStateId}
```

## <a name="request-headers"></a><span data-ttu-id="2736d-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="2736d-126">Request headers</span></span>
|<span data-ttu-id="2736d-127">标头</span><span class="sxs-lookup"><span data-stu-id="2736d-127">Header</span></span>|<span data-ttu-id="2736d-128">值</span><span class="sxs-lookup"><span data-stu-id="2736d-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2736d-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="2736d-129">Authorization</span></span>|<span data-ttu-id="2736d-130">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2736d-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2736d-131">接受</span><span class="sxs-lookup"><span data-stu-id="2736d-131">Accept</span></span>|<span data-ttu-id="2736d-132">application/json</span><span class="sxs-lookup"><span data-stu-id="2736d-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2736d-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="2736d-133">Request body</span></span>
<span data-ttu-id="2736d-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2736d-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2736d-135">响应</span><span class="sxs-lookup"><span data-stu-id="2736d-135">Response</span></span>
<span data-ttu-id="2736d-136">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="2736d-136">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2736d-137">示例</span><span class="sxs-lookup"><span data-stu-id="2736d-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="2736d-138">请求</span><span class="sxs-lookup"><span data-stu-id="2736d-138">Request</span></span>
<span data-ttu-id="2736d-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2736d-139">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates/{windowsUpdateStateId}
```

### <a name="response"></a><span data-ttu-id="2736d-140">响应</span><span class="sxs-lookup"><span data-stu-id="2736d-140">Response</span></span>
<span data-ttu-id="2736d-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2736d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```







