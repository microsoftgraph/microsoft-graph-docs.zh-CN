---
title: assign 操作
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e77be56361eb85568fb0c959c696bd6c2351b068
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51146445"
---
# <a name="assign-action"></a><span data-ttu-id="7381c-103">分配操作</span><span class="sxs-lookup"><span data-stu-id="7381c-103">assign action</span></span>

<span data-ttu-id="7381c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7381c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7381c-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7381c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7381c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7381c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7381c-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="7381c-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7381c-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="7381c-108">Prerequisites</span></span>
<span data-ttu-id="7381c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7381c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7381c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7381c-111">Permission type</span></span>|<span data-ttu-id="7381c-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7381c-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7381c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7381c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7381c-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7381c-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="7381c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7381c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7381c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7381c-116">Not supported.</span></span>|
|<span data-ttu-id="7381c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="7381c-117">Application</span></span>|<span data-ttu-id="7381c-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7381c-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7381c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7381c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="7381c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="7381c-120">Request headers</span></span>
|<span data-ttu-id="7381c-121">标头</span><span class="sxs-lookup"><span data-stu-id="7381c-121">Header</span></span>|<span data-ttu-id="7381c-122">值</span><span class="sxs-lookup"><span data-stu-id="7381c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7381c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7381c-123">Authorization</span></span>|<span data-ttu-id="7381c-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7381c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7381c-125">接受</span><span class="sxs-lookup"><span data-stu-id="7381c-125">Accept</span></span>|<span data-ttu-id="7381c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7381c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7381c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7381c-127">Request body</span></span>
<span data-ttu-id="7381c-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7381c-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="7381c-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="7381c-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="7381c-130">属性</span><span class="sxs-lookup"><span data-stu-id="7381c-130">Property</span></span>|<span data-ttu-id="7381c-131">类型</span><span class="sxs-lookup"><span data-stu-id="7381c-131">Type</span></span>|<span data-ttu-id="7381c-132">说明</span><span class="sxs-lookup"><span data-stu-id="7381c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7381c-133">deviceHealthScriptAssignments</span><span class="sxs-lookup"><span data-stu-id="7381c-133">deviceHealthScriptAssignments</span></span>|<span data-ttu-id="7381c-134">[deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7381c-134">[deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) collection</span></span>|<span data-ttu-id="7381c-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="7381c-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="7381c-136">响应</span><span class="sxs-lookup"><span data-stu-id="7381c-136">Response</span></span>
<span data-ttu-id="7381c-137">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="7381c-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7381c-138">示例</span><span class="sxs-lookup"><span data-stu-id="7381c-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="7381c-139">请求</span><span class="sxs-lookup"><span data-stu-id="7381c-139">Request</span></span>
<span data-ttu-id="7381c-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7381c-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/assign

Content-type: application/json
Content-length: 756

{
  "deviceHealthScriptAssignments": [
    {
      "@odata.type": "#microsoft.graph.deviceHealthScriptAssignment",
      "id": "c08c4eb1-4eb1-c08c-b14e-8cc0b14e8cc0",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include",
        "collectionId": "Collection Id value"
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

### <a name="response"></a><span data-ttu-id="7381c-141">响应</span><span class="sxs-lookup"><span data-stu-id="7381c-141">Response</span></span>
<span data-ttu-id="7381c-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7381c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




