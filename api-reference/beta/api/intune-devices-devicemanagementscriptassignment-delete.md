---
title: 删除 deviceManagementScriptAssignment
description: 删除 deviceManagementScriptAssignment。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: eef81cec7c834c9ec7d7f999881c6c7c6f4f479d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51150540"
---
# <a name="delete-devicemanagementscriptassignment"></a><span data-ttu-id="a3d50-103">删除 deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="a3d50-103">Delete deviceManagementScriptAssignment</span></span>

<span data-ttu-id="a3d50-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a3d50-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a3d50-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a3d50-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a3d50-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a3d50-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3d50-107">删除 [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="a3d50-107">Deletes a [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a3d50-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="a3d50-108">Prerequisites</span></span>
<span data-ttu-id="a3d50-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a3d50-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3d50-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a3d50-111">Permission type</span></span>|<span data-ttu-id="a3d50-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a3d50-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a3d50-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a3d50-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a3d50-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3d50-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="a3d50-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a3d50-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a3d50-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a3d50-116">Not supported.</span></span>|
|<span data-ttu-id="a3d50-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a3d50-117">Application</span></span>|<span data-ttu-id="a3d50-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3d50-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a3d50-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a3d50-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceShellScripts/{deviceShellScriptId}/assignments/{deviceManagementScriptAssignmentId}
DELETE /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assignments/{deviceManagementScriptAssignmentId}
DELETE /deviceManagement/deviceCustomAttributeShellScripts/{deviceCustomAttributeShellScriptId}/assignments/{deviceManagementScriptAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="a3d50-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a3d50-120">Request headers</span></span>
|<span data-ttu-id="a3d50-121">标头</span><span class="sxs-lookup"><span data-stu-id="a3d50-121">Header</span></span>|<span data-ttu-id="a3d50-122">值</span><span class="sxs-lookup"><span data-stu-id="a3d50-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a3d50-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a3d50-123">Authorization</span></span>|<span data-ttu-id="a3d50-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a3d50-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a3d50-125">接受</span><span class="sxs-lookup"><span data-stu-id="a3d50-125">Accept</span></span>|<span data-ttu-id="a3d50-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a3d50-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a3d50-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a3d50-127">Request body</span></span>
<span data-ttu-id="a3d50-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a3d50-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a3d50-129">响应</span><span class="sxs-lookup"><span data-stu-id="a3d50-129">Response</span></span>
<span data-ttu-id="a3d50-130">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="a3d50-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a3d50-131">示例</span><span class="sxs-lookup"><span data-stu-id="a3d50-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="a3d50-132">请求</span><span class="sxs-lookup"><span data-stu-id="a3d50-132">Request</span></span>
<span data-ttu-id="a3d50-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a3d50-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}/assignments/{deviceManagementScriptAssignmentId}
```

### <a name="response"></a><span data-ttu-id="a3d50-134">响应</span><span class="sxs-lookup"><span data-stu-id="a3d50-134">Response</span></span>
<span data-ttu-id="a3d50-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a3d50-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




