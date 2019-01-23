---
title: assign 操作
description: 尚未记录
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a58f087262200ac21bb521c899d5f5d6c3405ebb
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29420463"
---
# <a name="assign-action"></a><span data-ttu-id="c0879-103">assign 操作</span><span class="sxs-lookup"><span data-stu-id="c0879-103">assign action</span></span>

> <span data-ttu-id="c0879-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="c0879-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c0879-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c0879-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c0879-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c0879-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0879-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c0879-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c0879-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="c0879-108">Prerequisites</span></span>
<span data-ttu-id="c0879-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="c0879-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c0879-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c0879-111">Permission type</span></span>|<span data-ttu-id="c0879-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c0879-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c0879-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c0879-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c0879-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0879-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="c0879-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c0879-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c0879-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c0879-116">Not supported.</span></span>|
|<span data-ttu-id="c0879-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c0879-117">Application</span></span>|<span data-ttu-id="c0879-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="c0879-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c0879-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c0879-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="c0879-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c0879-120">Request headers</span></span>
|<span data-ttu-id="c0879-121">标头</span><span class="sxs-lookup"><span data-stu-id="c0879-121">Header</span></span>|<span data-ttu-id="c0879-122">值</span><span class="sxs-lookup"><span data-stu-id="c0879-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c0879-123">授权</span><span class="sxs-lookup"><span data-stu-id="c0879-123">Authorization</span></span>|<span data-ttu-id="c0879-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c0879-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c0879-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c0879-125">Accept</span></span>|<span data-ttu-id="c0879-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c0879-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0879-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c0879-127">Request body</span></span>
<span data-ttu-id="c0879-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c0879-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="c0879-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="c0879-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="c0879-130">属性</span><span class="sxs-lookup"><span data-stu-id="c0879-130">Property</span></span>|<span data-ttu-id="c0879-131">类型</span><span class="sxs-lookup"><span data-stu-id="c0879-131">Type</span></span>|<span data-ttu-id="c0879-132">说明</span><span class="sxs-lookup"><span data-stu-id="c0879-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0879-133">deviceManagementScriptGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="c0879-133">deviceManagementScriptGroupAssignments</span></span>|<span data-ttu-id="c0879-134">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="c0879-134">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) collection</span></span>|<span data-ttu-id="c0879-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c0879-135">Not yet documented</span></span>|
|<span data-ttu-id="c0879-136">deviceManagementScriptAssignments</span><span class="sxs-lookup"><span data-stu-id="c0879-136">deviceManagementScriptAssignments</span></span>|<span data-ttu-id="c0879-137">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="c0879-137">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) collection</span></span>|<span data-ttu-id="c0879-138">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c0879-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="c0879-139">响应</span><span class="sxs-lookup"><span data-stu-id="c0879-139">Response</span></span>
<span data-ttu-id="c0879-140">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="c0879-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c0879-141">示例</span><span class="sxs-lookup"><span data-stu-id="c0879-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="c0879-142">请求</span><span class="sxs-lookup"><span data-stu-id="c0879-142">Request</span></span>
<span data-ttu-id="c0879-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c0879-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c0879-144">响应</span><span class="sxs-lookup"><span data-stu-id="c0879-144">Response</span></span>
<span data-ttu-id="c0879-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c0879-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




