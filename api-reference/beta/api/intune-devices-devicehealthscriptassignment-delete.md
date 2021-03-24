---
title: 删除 deviceHealthScriptAssignment
description: 删除 deviceHealthScriptAssignment。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 34be38d718d9345c1ac9a680284093d36d27a680
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51128570"
---
# <a name="delete-devicehealthscriptassignment"></a><span data-ttu-id="2f550-103">删除 deviceHealthScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="2f550-103">Delete deviceHealthScriptAssignment</span></span>

<span data-ttu-id="2f550-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f550-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2f550-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2f550-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2f550-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2f550-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f550-107">删除 [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="2f550-107">Deletes a [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2f550-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="2f550-108">Prerequisites</span></span>
<span data-ttu-id="2f550-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2f550-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f550-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="2f550-111">Permission type</span></span>|<span data-ttu-id="2f550-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2f550-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f550-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2f550-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2f550-114">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f550-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2f550-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2f550-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f550-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2f550-116">Not supported.</span></span>|
|<span data-ttu-id="2f550-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="2f550-117">Application</span></span>|<span data-ttu-id="2f550-118">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f550-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f550-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2f550-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/assignments/{deviceHealthScriptAssignmentId}
DELETE /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/assignments/{deviceHealthScriptAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="2f550-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="2f550-120">Request headers</span></span>
|<span data-ttu-id="2f550-121">标头</span><span class="sxs-lookup"><span data-stu-id="2f550-121">Header</span></span>|<span data-ttu-id="2f550-122">值</span><span class="sxs-lookup"><span data-stu-id="2f550-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f550-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2f550-123">Authorization</span></span>|<span data-ttu-id="2f550-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2f550-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f550-125">接受</span><span class="sxs-lookup"><span data-stu-id="2f550-125">Accept</span></span>|<span data-ttu-id="2f550-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2f550-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f550-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2f550-127">Request body</span></span>
<span data-ttu-id="2f550-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2f550-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2f550-129">响应</span><span class="sxs-lookup"><span data-stu-id="2f550-129">Response</span></span>
<span data-ttu-id="2f550-130">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="2f550-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2f550-131">示例</span><span class="sxs-lookup"><span data-stu-id="2f550-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="2f550-132">请求</span><span class="sxs-lookup"><span data-stu-id="2f550-132">Request</span></span>
<span data-ttu-id="2f550-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2f550-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/assignments/{deviceHealthScriptAssignmentId}
```

### <a name="response"></a><span data-ttu-id="2f550-134">响应</span><span class="sxs-lookup"><span data-stu-id="2f550-134">Response</span></span>
<span data-ttu-id="2f550-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2f550-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




