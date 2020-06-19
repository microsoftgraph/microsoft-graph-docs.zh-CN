---
title: 更新 windowsDefenderApplicationControlSupplementalPolicyAssignment
description: 更新 windowsDefenderApplicationControlSupplementalPolicyAssignment 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 89e958ee31dc09112f9279e7ad170f144c088d5f
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791249"
---
# <a name="update-windowsdefenderapplicationcontrolsupplementalpolicyassignment"></a><span data-ttu-id="6562b-103">更新 windowsDefenderApplicationControlSupplementalPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="6562b-103">Update windowsDefenderApplicationControlSupplementalPolicyAssignment</span></span>

<span data-ttu-id="6562b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6562b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6562b-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6562b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6562b-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6562b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6562b-107">更新[windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6562b-107">Update the properties of a [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6562b-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="6562b-108">Prerequisites</span></span>
<span data-ttu-id="6562b-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="6562b-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="6562b-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6562b-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6562b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6562b-111">Permission type</span></span>|<span data-ttu-id="6562b-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6562b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6562b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6562b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6562b-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6562b-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6562b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6562b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6562b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6562b-116">Not supported.</span></span>|
|<span data-ttu-id="6562b-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="6562b-117">Application</span></span>|<span data-ttu-id="6562b-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6562b-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6562b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6562b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/assignments/{windowsDefenderApplicationControlSupplementalPolicyAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="6562b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6562b-120">Request headers</span></span>
|<span data-ttu-id="6562b-121">标头</span><span class="sxs-lookup"><span data-stu-id="6562b-121">Header</span></span>|<span data-ttu-id="6562b-122">值</span><span class="sxs-lookup"><span data-stu-id="6562b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6562b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6562b-123">Authorization</span></span>|<span data-ttu-id="6562b-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6562b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6562b-125">接受</span><span class="sxs-lookup"><span data-stu-id="6562b-125">Accept</span></span>|<span data-ttu-id="6562b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6562b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6562b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6562b-127">Request body</span></span>
<span data-ttu-id="6562b-128">在请求正文中，提供[windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6562b-128">In the request body, supply a JSON representation for the [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) object.</span></span>

<span data-ttu-id="6562b-129">下表显示创建[windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6562b-129">The following table shows the properties that are required when you create the [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md).</span></span>

|<span data-ttu-id="6562b-130">属性</span><span class="sxs-lookup"><span data-stu-id="6562b-130">Property</span></span>|<span data-ttu-id="6562b-131">类型</span><span class="sxs-lookup"><span data-stu-id="6562b-131">Type</span></span>|<span data-ttu-id="6562b-132">说明</span><span class="sxs-lookup"><span data-stu-id="6562b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6562b-133">id</span><span class="sxs-lookup"><span data-stu-id="6562b-133">id</span></span>|<span data-ttu-id="6562b-134">String</span><span class="sxs-lookup"><span data-stu-id="6562b-134">String</span></span>|<span data-ttu-id="6562b-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="6562b-135">Key of the entity.</span></span>|
|<span data-ttu-id="6562b-136">target</span><span class="sxs-lookup"><span data-stu-id="6562b-136">target</span></span>|[<span data-ttu-id="6562b-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="6562b-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="6562b-138">由管理员定义的目标组分配。</span><span class="sxs-lookup"><span data-stu-id="6562b-138">The target group assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="6562b-139">响应</span><span class="sxs-lookup"><span data-stu-id="6562b-139">Response</span></span>
<span data-ttu-id="6562b-140">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的[windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6562b-140">If successful, this method returns a `200 OK` response code and an updated [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6562b-141">示例</span><span class="sxs-lookup"><span data-stu-id="6562b-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="6562b-142">请求</span><span class="sxs-lookup"><span data-stu-id="6562b-142">Request</span></span>
<span data-ttu-id="6562b-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6562b-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/assignments/{windowsDefenderApplicationControlSupplementalPolicyAssignmentId}
Content-type: application/json
Content-length: 368

{
  "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicyAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```

### <a name="response"></a><span data-ttu-id="6562b-144">响应</span><span class="sxs-lookup"><span data-stu-id="6562b-144">Response</span></span>
<span data-ttu-id="6562b-145">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="6562b-145">Here is an example of the response.</span></span> <span data-ttu-id="6562b-146">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="6562b-146">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="6562b-147">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="6562b-147">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 417

{
  "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicyAssignment",
  "id": "5e299ff3-9ff3-5e29-f39f-295ef39f295e",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```



