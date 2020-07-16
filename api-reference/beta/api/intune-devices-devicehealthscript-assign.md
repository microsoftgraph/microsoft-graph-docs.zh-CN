---
title: assign 操作
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bd35d0edabdd0f20e5a3c567858159fdf5dd8de6
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792420"
---
# <a name="assign-action"></a><span data-ttu-id="f82ca-103">分配操作</span><span class="sxs-lookup"><span data-stu-id="f82ca-103">assign action</span></span>

<span data-ttu-id="f82ca-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f82ca-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f82ca-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f82ca-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f82ca-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f82ca-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f82ca-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f82ca-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f82ca-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="f82ca-108">Prerequisites</span></span>
<span data-ttu-id="f82ca-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f82ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f82ca-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f82ca-111">Permission type</span></span>|<span data-ttu-id="f82ca-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f82ca-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f82ca-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f82ca-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f82ca-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f82ca-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f82ca-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f82ca-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f82ca-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f82ca-116">Not supported.</span></span>|
|<span data-ttu-id="f82ca-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f82ca-117">Application</span></span>|<span data-ttu-id="f82ca-118">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f82ca-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f82ca-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f82ca-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="f82ca-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f82ca-120">Request headers</span></span>
|<span data-ttu-id="f82ca-121">标头</span><span class="sxs-lookup"><span data-stu-id="f82ca-121">Header</span></span>|<span data-ttu-id="f82ca-122">值</span><span class="sxs-lookup"><span data-stu-id="f82ca-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f82ca-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f82ca-123">Authorization</span></span>|<span data-ttu-id="f82ca-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f82ca-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f82ca-125">接受</span><span class="sxs-lookup"><span data-stu-id="f82ca-125">Accept</span></span>|<span data-ttu-id="f82ca-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f82ca-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f82ca-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f82ca-127">Request body</span></span>
<span data-ttu-id="f82ca-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f82ca-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="f82ca-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="f82ca-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="f82ca-130">属性</span><span class="sxs-lookup"><span data-stu-id="f82ca-130">Property</span></span>|<span data-ttu-id="f82ca-131">类型</span><span class="sxs-lookup"><span data-stu-id="f82ca-131">Type</span></span>|<span data-ttu-id="f82ca-132">说明</span><span class="sxs-lookup"><span data-stu-id="f82ca-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f82ca-133">deviceHealthScriptAssignments</span><span class="sxs-lookup"><span data-stu-id="f82ca-133">deviceHealthScriptAssignments</span></span>|<span data-ttu-id="f82ca-134">[deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="f82ca-134">[deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) collection</span></span>|<span data-ttu-id="f82ca-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f82ca-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="f82ca-136">响应</span><span class="sxs-lookup"><span data-stu-id="f82ca-136">Response</span></span>
<span data-ttu-id="f82ca-137">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="f82ca-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f82ca-138">示例</span><span class="sxs-lookup"><span data-stu-id="f82ca-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="f82ca-139">请求</span><span class="sxs-lookup"><span data-stu-id="f82ca-139">Request</span></span>
<span data-ttu-id="f82ca-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f82ca-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/assign

Content-type: application/json
Content-length: 688

{
  "deviceHealthScriptAssignments": [
    {
      "@odata.type": "#microsoft.graph.deviceHealthScriptAssignment",
      "id": "c08c4eb1-4eb1-c08c-b14e-8cc0b14e8cc0",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      },
      "runRemediationScript": true,
      "runSchedule": {
        "@odata.type": "microsoft.graph.deviceHealthScriptDailySchedule",
        "interval": 8,
        "useUtc": true,
        "time": "11:58:36.2550000"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="f82ca-141">响应</span><span class="sxs-lookup"><span data-stu-id="f82ca-141">Response</span></span>
<span data-ttu-id="f82ca-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f82ca-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



