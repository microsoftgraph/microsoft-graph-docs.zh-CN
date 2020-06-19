---
title: assign 操作
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 29218ed644bb9718cefbf199b45ac416c0a98cec
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792027"
---
# <a name="assign-action"></a><span data-ttu-id="dd08f-103">分配操作</span><span class="sxs-lookup"><span data-stu-id="dd08f-103">assign action</span></span>

<span data-ttu-id="dd08f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd08f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dd08f-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="dd08f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dd08f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="dd08f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dd08f-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="dd08f-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dd08f-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="dd08f-108">Prerequisites</span></span>
<span data-ttu-id="dd08f-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="dd08f-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="dd08f-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd08f-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd08f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="dd08f-111">Permission type</span></span>|<span data-ttu-id="dd08f-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="dd08f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dd08f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dd08f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dd08f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd08f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dd08f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dd08f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dd08f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="dd08f-116">Not supported.</span></span>|
|<span data-ttu-id="dd08f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="dd08f-117">Application</span></span>|<span data-ttu-id="dd08f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd08f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dd08f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dd08f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="dd08f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="dd08f-120">Request headers</span></span>
|<span data-ttu-id="dd08f-121">标头</span><span class="sxs-lookup"><span data-stu-id="dd08f-121">Header</span></span>|<span data-ttu-id="dd08f-122">值</span><span class="sxs-lookup"><span data-stu-id="dd08f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dd08f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="dd08f-123">Authorization</span></span>|<span data-ttu-id="dd08f-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="dd08f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dd08f-125">接受</span><span class="sxs-lookup"><span data-stu-id="dd08f-125">Accept</span></span>|<span data-ttu-id="dd08f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dd08f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dd08f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="dd08f-127">Request body</span></span>
<span data-ttu-id="dd08f-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dd08f-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="dd08f-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="dd08f-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="dd08f-130">属性</span><span class="sxs-lookup"><span data-stu-id="dd08f-130">Property</span></span>|<span data-ttu-id="dd08f-131">类型</span><span class="sxs-lookup"><span data-stu-id="dd08f-131">Type</span></span>|<span data-ttu-id="dd08f-132">说明</span><span class="sxs-lookup"><span data-stu-id="dd08f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd08f-133">assignments</span><span class="sxs-lookup"><span data-stu-id="dd08f-133">assignments</span></span>|<span data-ttu-id="dd08f-134">[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="dd08f-134">[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) collection</span></span>|<span data-ttu-id="dd08f-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="dd08f-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="dd08f-136">响应</span><span class="sxs-lookup"><span data-stu-id="dd08f-136">Response</span></span>
<span data-ttu-id="dd08f-137">如果成功，此操作会 `200 OK` 在响应正文中返回响应代码和[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)集合。</span><span class="sxs-lookup"><span data-stu-id="dd08f-137">If successful, this action returns a `200 OK` response code and a [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd08f-138">示例</span><span class="sxs-lookup"><span data-stu-id="dd08f-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="dd08f-139">请求</span><span class="sxs-lookup"><span data-stu-id="dd08f-139">Request</span></span>
<span data-ttu-id="dd08f-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="dd08f-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assign

Content-type: application/json
Content-length: 456

{
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePoolAssignment",
      "id": "e7304dcc-4dcc-e730-cc4d-30e7cc4d30e7",
      "target": {
        "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="dd08f-141">响应</span><span class="sxs-lookup"><span data-stu-id="dd08f-141">Response</span></span>
<span data-ttu-id="dd08f-142">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="dd08f-142">Here is an example of the response.</span></span> <span data-ttu-id="dd08f-143">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="dd08f-143">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="dd08f-144">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="dd08f-144">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 450

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePoolAssignment",
      "id": "e7304dcc-4dcc-e730-cc4d-30e7cc4d30e7",
      "target": {
        "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      }
    }
  ]
}
```



