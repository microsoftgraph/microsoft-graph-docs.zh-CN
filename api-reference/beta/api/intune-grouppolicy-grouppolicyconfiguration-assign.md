---
title: assign 操作
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 00431a77432738eca351ccbe04d1a06c289db806
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791992"
---
# <a name="assign-action"></a><span data-ttu-id="5ca8f-103">分配操作</span><span class="sxs-lookup"><span data-stu-id="5ca8f-103">assign action</span></span>

<span data-ttu-id="5ca8f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ca8f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5ca8f-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5ca8f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5ca8f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5ca8f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5ca8f-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="5ca8f-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5ca8f-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="5ca8f-108">Prerequisites</span></span>
<span data-ttu-id="5ca8f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5ca8f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ca8f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="5ca8f-111">Permission type</span></span>|<span data-ttu-id="5ca8f-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5ca8f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5ca8f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5ca8f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5ca8f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ca8f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5ca8f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5ca8f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5ca8f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5ca8f-116">Not supported.</span></span>|
|<span data-ttu-id="5ca8f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="5ca8f-117">Application</span></span>|<span data-ttu-id="5ca8f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ca8f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5ca8f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5ca8f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="5ca8f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="5ca8f-120">Request headers</span></span>
|<span data-ttu-id="5ca8f-121">标头</span><span class="sxs-lookup"><span data-stu-id="5ca8f-121">Header</span></span>|<span data-ttu-id="5ca8f-122">值</span><span class="sxs-lookup"><span data-stu-id="5ca8f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5ca8f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5ca8f-123">Authorization</span></span>|<span data-ttu-id="5ca8f-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5ca8f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5ca8f-125">接受</span><span class="sxs-lookup"><span data-stu-id="5ca8f-125">Accept</span></span>|<span data-ttu-id="5ca8f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5ca8f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5ca8f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="5ca8f-127">Request body</span></span>
<span data-ttu-id="5ca8f-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5ca8f-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="5ca8f-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="5ca8f-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="5ca8f-130">属性</span><span class="sxs-lookup"><span data-stu-id="5ca8f-130">Property</span></span>|<span data-ttu-id="5ca8f-131">类型</span><span class="sxs-lookup"><span data-stu-id="5ca8f-131">Type</span></span>|<span data-ttu-id="5ca8f-132">说明</span><span class="sxs-lookup"><span data-stu-id="5ca8f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ca8f-133">assignments</span><span class="sxs-lookup"><span data-stu-id="5ca8f-133">assignments</span></span>|<span data-ttu-id="5ca8f-134">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="5ca8f-134">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="5ca8f-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="5ca8f-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="5ca8f-136">响应</span><span class="sxs-lookup"><span data-stu-id="5ca8f-136">Response</span></span>
<span data-ttu-id="5ca8f-137">如果成功，此操作会 `200 OK` 在响应正文中返回响应代码和[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)集合。</span><span class="sxs-lookup"><span data-stu-id="5ca8f-137">If successful, this action returns a `200 OK` response code and a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ca8f-138">示例</span><span class="sxs-lookup"><span data-stu-id="5ca8f-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="5ca8f-139">请求</span><span class="sxs-lookup"><span data-stu-id="5ca8f-139">Request</span></span>
<span data-ttu-id="5ca8f-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5ca8f-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assign

Content-type: application/json
Content-length: 513

{
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyConfigurationAssignment",
      "id": "2a4161e9-61e9-2a41-e961-412ae961412a",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="5ca8f-141">响应</span><span class="sxs-lookup"><span data-stu-id="5ca8f-141">Response</span></span>
<span data-ttu-id="5ca8f-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5ca8f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 507

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyConfigurationAssignment",
      "id": "2a4161e9-61e9-2a41-e961-412ae961412a",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      }
    }
  ]
}
```



