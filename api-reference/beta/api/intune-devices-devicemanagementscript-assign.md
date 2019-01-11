---
title: assign 操作
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: eede97b2c2cddf666e99f2f979520e3f9e9546fc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858224"
---
# <a name="assign-action"></a><span data-ttu-id="0e87c-103">assign 操作</span><span class="sxs-lookup"><span data-stu-id="0e87c-103">assign action</span></span>

> <span data-ttu-id="0e87c-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="0e87c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0e87c-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0e87c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0e87c-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="0e87c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0e87c-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="0e87c-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0e87c-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="0e87c-108">Prerequisites</span></span>
<span data-ttu-id="0e87c-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="0e87c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e87c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="0e87c-111">Permission type</span></span>|<span data-ttu-id="0e87c-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0e87c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0e87c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0e87c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0e87c-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e87c-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="0e87c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0e87c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0e87c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0e87c-116">Not supported.</span></span>|
|<span data-ttu-id="0e87c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="0e87c-117">Application</span></span>|<span data-ttu-id="0e87c-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="0e87c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0e87c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0e87c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="0e87c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="0e87c-120">Request headers</span></span>
|<span data-ttu-id="0e87c-121">标头</span><span class="sxs-lookup"><span data-stu-id="0e87c-121">Header</span></span>|<span data-ttu-id="0e87c-122">值</span><span class="sxs-lookup"><span data-stu-id="0e87c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0e87c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0e87c-123">Authorization</span></span>|<span data-ttu-id="0e87c-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0e87c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0e87c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0e87c-125">Accept</span></span>|<span data-ttu-id="0e87c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0e87c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0e87c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0e87c-127">Request body</span></span>
<span data-ttu-id="0e87c-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0e87c-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="0e87c-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="0e87c-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="0e87c-130">属性</span><span class="sxs-lookup"><span data-stu-id="0e87c-130">Property</span></span>|<span data-ttu-id="0e87c-131">类型</span><span class="sxs-lookup"><span data-stu-id="0e87c-131">Type</span></span>|<span data-ttu-id="0e87c-132">Description</span><span class="sxs-lookup"><span data-stu-id="0e87c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e87c-133">deviceManagementScriptGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="0e87c-133">deviceManagementScriptGroupAssignments</span></span>|<span data-ttu-id="0e87c-134">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="0e87c-134">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) collection</span></span>|<span data-ttu-id="0e87c-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="0e87c-135">Not yet documented</span></span>|
|<span data-ttu-id="0e87c-136">deviceManagementScriptAssignments</span><span class="sxs-lookup"><span data-stu-id="0e87c-136">deviceManagementScriptAssignments</span></span>|<span data-ttu-id="0e87c-137">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="0e87c-137">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) collection</span></span>|<span data-ttu-id="0e87c-138">尚未记录</span><span class="sxs-lookup"><span data-stu-id="0e87c-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="0e87c-139">响应</span><span class="sxs-lookup"><span data-stu-id="0e87c-139">Response</span></span>
<span data-ttu-id="0e87c-140">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="0e87c-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0e87c-141">示例</span><span class="sxs-lookup"><span data-stu-id="0e87c-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="0e87c-142">请求</span><span class="sxs-lookup"><span data-stu-id="0e87c-142">Request</span></span>
<span data-ttu-id="0e87c-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0e87c-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0e87c-144">响应</span><span class="sxs-lookup"><span data-stu-id="0e87c-144">Response</span></span>
<span data-ttu-id="0e87c-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0e87c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





