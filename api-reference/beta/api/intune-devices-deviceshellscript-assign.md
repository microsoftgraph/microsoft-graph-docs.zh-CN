---
title: assign 操作
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1fcfc73de0958193d15187712debeddb12ddad21
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49228645"
---
# <a name="assign-action"></a><span data-ttu-id="d2558-103">分配操作</span><span class="sxs-lookup"><span data-stu-id="d2558-103">assign action</span></span>

<span data-ttu-id="d2558-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d2558-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d2558-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d2558-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d2558-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d2558-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d2558-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d2558-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d2558-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="d2558-108">Prerequisites</span></span>
<span data-ttu-id="d2558-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d2558-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2558-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d2558-111">Permission type</span></span>|<span data-ttu-id="d2558-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d2558-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d2558-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d2558-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d2558-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2558-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="d2558-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d2558-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d2558-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d2558-116">Not supported.</span></span>|
|<span data-ttu-id="d2558-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d2558-117">Application</span></span>|<span data-ttu-id="d2558-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2558-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d2558-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d2558-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceShellScripts/{deviceShellScriptId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="d2558-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d2558-120">Request headers</span></span>
|<span data-ttu-id="d2558-121">标头</span><span class="sxs-lookup"><span data-stu-id="d2558-121">Header</span></span>|<span data-ttu-id="d2558-122">值</span><span class="sxs-lookup"><span data-stu-id="d2558-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d2558-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d2558-123">Authorization</span></span>|<span data-ttu-id="d2558-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d2558-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d2558-125">接受</span><span class="sxs-lookup"><span data-stu-id="d2558-125">Accept</span></span>|<span data-ttu-id="d2558-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d2558-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2558-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d2558-127">Request body</span></span>
<span data-ttu-id="d2558-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d2558-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="d2558-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="d2558-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="d2558-130">属性</span><span class="sxs-lookup"><span data-stu-id="d2558-130">Property</span></span>|<span data-ttu-id="d2558-131">类型</span><span class="sxs-lookup"><span data-stu-id="d2558-131">Type</span></span>|<span data-ttu-id="d2558-132">说明</span><span class="sxs-lookup"><span data-stu-id="d2558-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2558-133">deviceManagementScriptGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="d2558-133">deviceManagementScriptGroupAssignments</span></span>|<span data-ttu-id="d2558-134">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d2558-134">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) collection</span></span>|<span data-ttu-id="d2558-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d2558-135">Not yet documented</span></span>|
|<span data-ttu-id="d2558-136">deviceManagementScriptAssignments</span><span class="sxs-lookup"><span data-stu-id="d2558-136">deviceManagementScriptAssignments</span></span>|<span data-ttu-id="d2558-137">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d2558-137">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) collection</span></span>|<span data-ttu-id="d2558-138">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d2558-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="d2558-139">响应</span><span class="sxs-lookup"><span data-stu-id="d2558-139">Response</span></span>
<span data-ttu-id="d2558-140">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="d2558-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d2558-141">示例</span><span class="sxs-lookup"><span data-stu-id="d2558-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="d2558-142">请求</span><span class="sxs-lookup"><span data-stu-id="d2558-142">Request</span></span>
<span data-ttu-id="d2558-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d2558-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}/assign

Content-type: application/json
Content-length: 713

{
  "deviceManagementScriptGroupAssignments": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementScriptGroupAssignment",
      "id": "ecd2357d-357d-ecd2-7d35-d2ec7d35d2ec",
      "targetGroupId": "Target Group Id value"
    }
  ],
  "deviceManagementScriptAssignments": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementScriptAssignment",
      "id": "a87a601e-601e-a87a-1e60-7aa81e607aa8",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="d2558-144">响应</span><span class="sxs-lookup"><span data-stu-id="d2558-144">Response</span></span>
<span data-ttu-id="d2558-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d2558-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




