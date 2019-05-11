---
title: assign 操作
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 88e7686d9d13084508cfed47927d4b44e7513cd5
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33910007"
---
# <a name="assign-action"></a><span data-ttu-id="42454-103">分配操作</span><span class="sxs-lookup"><span data-stu-id="42454-103">assign action</span></span>

> <span data-ttu-id="42454-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="42454-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="42454-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="42454-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42454-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="42454-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="42454-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="42454-107">Prerequisites</span></span>
<span data-ttu-id="42454-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="42454-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42454-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="42454-110">Permission type</span></span>|<span data-ttu-id="42454-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="42454-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="42454-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="42454-112">Delegated (work or school account)</span></span>|<span data-ttu-id="42454-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42454-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="42454-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="42454-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="42454-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="42454-115">Not supported.</span></span>|
|<span data-ttu-id="42454-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="42454-116">Application</span></span>|<span data-ttu-id="42454-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="42454-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="42454-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="42454-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="42454-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="42454-119">Request headers</span></span>
|<span data-ttu-id="42454-120">标头</span><span class="sxs-lookup"><span data-stu-id="42454-120">Header</span></span>|<span data-ttu-id="42454-121">值</span><span class="sxs-lookup"><span data-stu-id="42454-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="42454-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="42454-122">Authorization</span></span>|<span data-ttu-id="42454-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="42454-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="42454-124">接受</span><span class="sxs-lookup"><span data-stu-id="42454-124">Accept</span></span>|<span data-ttu-id="42454-125">application/json</span><span class="sxs-lookup"><span data-stu-id="42454-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="42454-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="42454-126">Request body</span></span>
<span data-ttu-id="42454-127">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="42454-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="42454-128">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="42454-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="42454-129">属性</span><span class="sxs-lookup"><span data-stu-id="42454-129">Property</span></span>|<span data-ttu-id="42454-130">类型</span><span class="sxs-lookup"><span data-stu-id="42454-130">Type</span></span>|<span data-ttu-id="42454-131">说明</span><span class="sxs-lookup"><span data-stu-id="42454-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42454-132">deviceManagementScriptGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="42454-132">deviceManagementScriptGroupAssignments</span></span>|<span data-ttu-id="42454-133">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="42454-133">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) collection</span></span>|<span data-ttu-id="42454-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="42454-134">Not yet documented</span></span>|
|<span data-ttu-id="42454-135">deviceManagementScriptAssignments</span><span class="sxs-lookup"><span data-stu-id="42454-135">deviceManagementScriptAssignments</span></span>|<span data-ttu-id="42454-136">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="42454-136">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) collection</span></span>|<span data-ttu-id="42454-137">尚未记录</span><span class="sxs-lookup"><span data-stu-id="42454-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="42454-138">响应</span><span class="sxs-lookup"><span data-stu-id="42454-138">Response</span></span>
<span data-ttu-id="42454-139">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="42454-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="42454-140">示例</span><span class="sxs-lookup"><span data-stu-id="42454-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="42454-141">请求</span><span class="sxs-lookup"><span data-stu-id="42454-141">Request</span></span>
<span data-ttu-id="42454-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="42454-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assign

Content-type: application/json
Content-length: 550

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
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="42454-143">响应</span><span class="sxs-lookup"><span data-stu-id="42454-143">Response</span></span>
<span data-ttu-id="42454-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="42454-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




