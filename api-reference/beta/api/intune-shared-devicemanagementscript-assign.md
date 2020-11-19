---
title: assign 操作
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 385c2230dd6911388f3e357cae508ec5521cd481
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49223904"
---
# <a name="assign-action"></a><span data-ttu-id="85aa4-103">分配操作</span><span class="sxs-lookup"><span data-stu-id="85aa4-103">assign action</span></span>

<span data-ttu-id="85aa4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85aa4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="85aa4-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="85aa4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="85aa4-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="85aa4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="85aa4-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="85aa4-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="85aa4-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="85aa4-108">Prerequisites</span></span>
<span data-ttu-id="85aa4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="85aa4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85aa4-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="85aa4-111">Permission type</span></span>|<span data-ttu-id="85aa4-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="85aa4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="85aa4-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="85aa4-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="85aa4-114">&nbsp;&nbsp;**设备管理**</span><span class="sxs-lookup"><span data-stu-id="85aa4-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="85aa4-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85aa4-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="85aa4-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="85aa4-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="85aa4-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="85aa4-117">Not supported.</span></span>|
|<span data-ttu-id="85aa4-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="85aa4-118">Application</span></span>||
| <span data-ttu-id="85aa4-119">&nbsp;&nbsp;**设备管理**</span><span class="sxs-lookup"><span data-stu-id="85aa4-119">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="85aa4-120">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85aa4-120">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="85aa4-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="85aa4-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="85aa4-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="85aa4-122">Request headers</span></span>
|<span data-ttu-id="85aa4-123">标头</span><span class="sxs-lookup"><span data-stu-id="85aa4-123">Header</span></span>|<span data-ttu-id="85aa4-124">值</span><span class="sxs-lookup"><span data-stu-id="85aa4-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="85aa4-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="85aa4-125">Authorization</span></span>|<span data-ttu-id="85aa4-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="85aa4-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="85aa4-127">接受</span><span class="sxs-lookup"><span data-stu-id="85aa4-127">Accept</span></span>|<span data-ttu-id="85aa4-128">application/json</span><span class="sxs-lookup"><span data-stu-id="85aa4-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="85aa4-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="85aa4-129">Request body</span></span>
<span data-ttu-id="85aa4-130">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="85aa4-130">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="85aa4-131">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="85aa4-131">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="85aa4-132">属性</span><span class="sxs-lookup"><span data-stu-id="85aa4-132">Property</span></span>|<span data-ttu-id="85aa4-133">类型</span><span class="sxs-lookup"><span data-stu-id="85aa4-133">Type</span></span>|<span data-ttu-id="85aa4-134">说明</span><span class="sxs-lookup"><span data-stu-id="85aa4-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85aa4-135">deviceManagementScriptGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="85aa4-135">deviceManagementScriptGroupAssignments</span></span>|<span data-ttu-id="85aa4-136">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="85aa4-136">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) collection</span></span>|<span data-ttu-id="85aa4-137">尚未记录</span><span class="sxs-lookup"><span data-stu-id="85aa4-137">Not yet documented</span></span>|
|<span data-ttu-id="85aa4-138">deviceManagementScriptAssignments</span><span class="sxs-lookup"><span data-stu-id="85aa4-138">deviceManagementScriptAssignments</span></span>|<span data-ttu-id="85aa4-139">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="85aa4-139">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) collection</span></span>|<span data-ttu-id="85aa4-140">尚未记录</span><span class="sxs-lookup"><span data-stu-id="85aa4-140">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="85aa4-141">响应</span><span class="sxs-lookup"><span data-stu-id="85aa4-141">Response</span></span>
<span data-ttu-id="85aa4-142">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="85aa4-142">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="85aa4-143">示例</span><span class="sxs-lookup"><span data-stu-id="85aa4-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="85aa4-144">请求</span><span class="sxs-lookup"><span data-stu-id="85aa4-144">Request</span></span>
<span data-ttu-id="85aa4-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="85aa4-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="85aa4-146">响应</span><span class="sxs-lookup"><span data-stu-id="85aa4-146">Response</span></span>
<span data-ttu-id="85aa4-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="85aa4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```







