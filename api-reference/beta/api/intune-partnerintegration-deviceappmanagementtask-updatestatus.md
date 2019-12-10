---
title: updateStatus 操作
description: 设置任务的状态并附加注释。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 989263bd262b83dfda427a5505b8427d9b06c00f
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39941300"
---
# <a name="updatestatus-action"></a><span data-ttu-id="29ec2-103">updateStatus 操作</span><span class="sxs-lookup"><span data-stu-id="29ec2-103">updateStatus action</span></span>

> <span data-ttu-id="29ec2-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="29ec2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="29ec2-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="29ec2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="29ec2-106">设置任务的状态并附加注释。</span><span class="sxs-lookup"><span data-stu-id="29ec2-106">Set the task's status and attach a note.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="29ec2-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="29ec2-107">Prerequisites</span></span>
<span data-ttu-id="29ec2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="29ec2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29ec2-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="29ec2-110">Permission type</span></span>|<span data-ttu-id="29ec2-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="29ec2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="29ec2-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="29ec2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="29ec2-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29ec2-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="29ec2-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="29ec2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="29ec2-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="29ec2-115">Not supported.</span></span>|
|<span data-ttu-id="29ec2-116">Application</span><span class="sxs-lookup"><span data-stu-id="29ec2-116">Application</span></span>|<span data-ttu-id="29ec2-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29ec2-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="29ec2-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="29ec2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/deviceAppManagementTasks/{deviceAppManagementTaskId}/updateStatus
```

## <a name="request-headers"></a><span data-ttu-id="29ec2-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="29ec2-119">Request headers</span></span>
|<span data-ttu-id="29ec2-120">标头</span><span class="sxs-lookup"><span data-stu-id="29ec2-120">Header</span></span>|<span data-ttu-id="29ec2-121">值</span><span class="sxs-lookup"><span data-stu-id="29ec2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="29ec2-122">授权</span><span class="sxs-lookup"><span data-stu-id="29ec2-122">Authorization</span></span>|<span data-ttu-id="29ec2-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="29ec2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="29ec2-124">接受</span><span class="sxs-lookup"><span data-stu-id="29ec2-124">Accept</span></span>|<span data-ttu-id="29ec2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="29ec2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="29ec2-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="29ec2-126">Request body</span></span>
<span data-ttu-id="29ec2-127">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="29ec2-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="29ec2-128">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="29ec2-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="29ec2-129">属性</span><span class="sxs-lookup"><span data-stu-id="29ec2-129">Property</span></span>|<span data-ttu-id="29ec2-130">类型</span><span class="sxs-lookup"><span data-stu-id="29ec2-130">Type</span></span>|<span data-ttu-id="29ec2-131">说明</span><span class="sxs-lookup"><span data-stu-id="29ec2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29ec2-132">状态</span><span class="sxs-lookup"><span data-stu-id="29ec2-132">status</span></span>|[<span data-ttu-id="29ec2-133">deviceAppManagementTaskStatus</span><span class="sxs-lookup"><span data-stu-id="29ec2-133">deviceAppManagementTaskStatus</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskstatus.md)|<span data-ttu-id="29ec2-134">状态</span><span class="sxs-lookup"><span data-stu-id="29ec2-134">The status</span></span>|
|<span data-ttu-id="29ec2-135">便笺</span><span class="sxs-lookup"><span data-stu-id="29ec2-135">note</span></span>|<span data-ttu-id="29ec2-136">字符串</span><span class="sxs-lookup"><span data-stu-id="29ec2-136">String</span></span>|<span data-ttu-id="29ec2-137">注释</span><span class="sxs-lookup"><span data-stu-id="29ec2-137">The note</span></span>|



## <a name="response"></a><span data-ttu-id="29ec2-138">响应</span><span class="sxs-lookup"><span data-stu-id="29ec2-138">Response</span></span>
<span data-ttu-id="29ec2-139">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="29ec2-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="29ec2-140">示例</span><span class="sxs-lookup"><span data-stu-id="29ec2-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="29ec2-141">请求</span><span class="sxs-lookup"><span data-stu-id="29ec2-141">Request</span></span>
<span data-ttu-id="29ec2-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="29ec2-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/deviceAppManagementTasks/{deviceAppManagementTaskId}/updateStatus

Content-type: application/json
Content-length: 52

{
  "status": "pending",
  "note": "Note value"
}
```

### <a name="response"></a><span data-ttu-id="29ec2-143">响应</span><span class="sxs-lookup"><span data-stu-id="29ec2-143">Response</span></span>
<span data-ttu-id="29ec2-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="29ec2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





