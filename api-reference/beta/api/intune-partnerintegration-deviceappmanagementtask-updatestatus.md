---
title: updateStatus 操作
description: 设置任务的状态并附加注释。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f6e8bc97b8c5ef9d54b7d1a753b1bd4602b2eeb4
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48726043"
---
# <a name="updatestatus-action"></a><span data-ttu-id="77fc8-103">updateStatus 操作</span><span class="sxs-lookup"><span data-stu-id="77fc8-103">updateStatus action</span></span>

<span data-ttu-id="77fc8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77fc8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="77fc8-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="77fc8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="77fc8-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="77fc8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77fc8-107">设置任务的状态并附加注释。</span><span class="sxs-lookup"><span data-stu-id="77fc8-107">Set the task's status and attach a note.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="77fc8-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="77fc8-108">Prerequisites</span></span>
<span data-ttu-id="77fc8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="77fc8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77fc8-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="77fc8-111">Permission type</span></span>|<span data-ttu-id="77fc8-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="77fc8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="77fc8-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="77fc8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="77fc8-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77fc8-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="77fc8-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="77fc8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="77fc8-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="77fc8-116">Not supported.</span></span>|
|<span data-ttu-id="77fc8-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="77fc8-117">Application</span></span>|<span data-ttu-id="77fc8-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77fc8-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="77fc8-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="77fc8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/deviceAppManagementTasks/{deviceAppManagementTaskId}/updateStatus
```

## <a name="request-headers"></a><span data-ttu-id="77fc8-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="77fc8-120">Request headers</span></span>
|<span data-ttu-id="77fc8-121">标头</span><span class="sxs-lookup"><span data-stu-id="77fc8-121">Header</span></span>|<span data-ttu-id="77fc8-122">值</span><span class="sxs-lookup"><span data-stu-id="77fc8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="77fc8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="77fc8-123">Authorization</span></span>|<span data-ttu-id="77fc8-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="77fc8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="77fc8-125">接受</span><span class="sxs-lookup"><span data-stu-id="77fc8-125">Accept</span></span>|<span data-ttu-id="77fc8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="77fc8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="77fc8-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="77fc8-127">Request body</span></span>
<span data-ttu-id="77fc8-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="77fc8-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="77fc8-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="77fc8-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="77fc8-130">属性</span><span class="sxs-lookup"><span data-stu-id="77fc8-130">Property</span></span>|<span data-ttu-id="77fc8-131">类型</span><span class="sxs-lookup"><span data-stu-id="77fc8-131">Type</span></span>|<span data-ttu-id="77fc8-132">说明</span><span class="sxs-lookup"><span data-stu-id="77fc8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77fc8-133">状态</span><span class="sxs-lookup"><span data-stu-id="77fc8-133">status</span></span>|[<span data-ttu-id="77fc8-134">deviceAppManagementTaskStatus</span><span class="sxs-lookup"><span data-stu-id="77fc8-134">deviceAppManagementTaskStatus</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskstatus.md)|<span data-ttu-id="77fc8-135">状态</span><span class="sxs-lookup"><span data-stu-id="77fc8-135">The status</span></span>|
|<span data-ttu-id="77fc8-136">便笺</span><span class="sxs-lookup"><span data-stu-id="77fc8-136">note</span></span>|<span data-ttu-id="77fc8-137">String</span><span class="sxs-lookup"><span data-stu-id="77fc8-137">String</span></span>|<span data-ttu-id="77fc8-138">注释</span><span class="sxs-lookup"><span data-stu-id="77fc8-138">The note</span></span>|



## <a name="response"></a><span data-ttu-id="77fc8-139">响应</span><span class="sxs-lookup"><span data-stu-id="77fc8-139">Response</span></span>
<span data-ttu-id="77fc8-140">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="77fc8-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="77fc8-141">示例</span><span class="sxs-lookup"><span data-stu-id="77fc8-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="77fc8-142">请求</span><span class="sxs-lookup"><span data-stu-id="77fc8-142">Request</span></span>
<span data-ttu-id="77fc8-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="77fc8-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/deviceAppManagementTasks/{deviceAppManagementTaskId}/updateStatus

Content-type: application/json
Content-length: 52

{
  "status": "pending",
  "note": "Note value"
}
```

### <a name="response"></a><span data-ttu-id="77fc8-144">响应</span><span class="sxs-lookup"><span data-stu-id="77fc8-144">Response</span></span>
<span data-ttu-id="77fc8-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="77fc8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





