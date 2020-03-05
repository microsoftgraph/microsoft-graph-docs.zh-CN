---
title: 更新 windowsDefenderApplicationControlSupplementalPolicyAssignment
description: 更新 windowsDefenderApplicationControlSupplementalPolicyAssignment 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 801fe68368d3ee45772b5225af7216b558acd586
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42457508"
---
# <a name="update-windowsdefenderapplicationcontrolsupplementalpolicyassignment"></a><span data-ttu-id="e5284-103">更新 windowsDefenderApplicationControlSupplementalPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="e5284-103">Update windowsDefenderApplicationControlSupplementalPolicyAssignment</span></span>

<span data-ttu-id="e5284-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="e5284-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e5284-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e5284-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e5284-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e5284-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5284-107">更新[windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e5284-107">Update the properties of a [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e5284-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="e5284-108">Prerequisites</span></span>
<span data-ttu-id="e5284-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e5284-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5284-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e5284-111">Permission type</span></span>|<span data-ttu-id="e5284-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e5284-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e5284-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e5284-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e5284-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5284-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e5284-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e5284-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e5284-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e5284-116">Not supported.</span></span>|
|<span data-ttu-id="e5284-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e5284-117">Application</span></span>|<span data-ttu-id="e5284-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5284-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e5284-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e5284-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/assignments/{windowsDefenderApplicationControlSupplementalPolicyAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="e5284-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e5284-120">Request headers</span></span>
|<span data-ttu-id="e5284-121">标头</span><span class="sxs-lookup"><span data-stu-id="e5284-121">Header</span></span>|<span data-ttu-id="e5284-122">值</span><span class="sxs-lookup"><span data-stu-id="e5284-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e5284-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e5284-123">Authorization</span></span>|<span data-ttu-id="e5284-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e5284-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e5284-125">接受</span><span class="sxs-lookup"><span data-stu-id="e5284-125">Accept</span></span>|<span data-ttu-id="e5284-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e5284-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e5284-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e5284-127">Request body</span></span>
<span data-ttu-id="e5284-128">在请求正文中，提供[windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e5284-128">In the request body, supply a JSON representation for the [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) object.</span></span>

<span data-ttu-id="e5284-129">下表显示创建[windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e5284-129">The following table shows the properties that are required when you create the [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md).</span></span>

|<span data-ttu-id="e5284-130">属性</span><span class="sxs-lookup"><span data-stu-id="e5284-130">Property</span></span>|<span data-ttu-id="e5284-131">类型</span><span class="sxs-lookup"><span data-stu-id="e5284-131">Type</span></span>|<span data-ttu-id="e5284-132">说明</span><span class="sxs-lookup"><span data-stu-id="e5284-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5284-133">id</span><span class="sxs-lookup"><span data-stu-id="e5284-133">id</span></span>|<span data-ttu-id="e5284-134">String</span><span class="sxs-lookup"><span data-stu-id="e5284-134">String</span></span>|<span data-ttu-id="e5284-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e5284-135">Key of the entity.</span></span>|
|<span data-ttu-id="e5284-136">target</span><span class="sxs-lookup"><span data-stu-id="e5284-136">target</span></span>|[<span data-ttu-id="e5284-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="e5284-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="e5284-138">由管理员定义的目标组分配。</span><span class="sxs-lookup"><span data-stu-id="e5284-138">The target group assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="e5284-139">响应</span><span class="sxs-lookup"><span data-stu-id="e5284-139">Response</span></span>
<span data-ttu-id="e5284-140">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e5284-140">If successful, this method returns a `200 OK` response code and an updated [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5284-141">示例</span><span class="sxs-lookup"><span data-stu-id="e5284-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="e5284-142">请求</span><span class="sxs-lookup"><span data-stu-id="e5284-142">Request</span></span>
<span data-ttu-id="e5284-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e5284-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/assignments/{windowsDefenderApplicationControlSupplementalPolicyAssignmentId}
Content-type: application/json
Content-length: 201

{
  "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicyAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="e5284-144">响应</span><span class="sxs-lookup"><span data-stu-id="e5284-144">Response</span></span>
<span data-ttu-id="e5284-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e5284-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 250

{
  "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicyAssignment",
  "id": "5e299ff3-9ff3-5e29-f39f-295ef39f295e",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```





