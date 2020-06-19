---
title: 更新 windowsAutopilotDeploymentProfileAssignment
description: 更新 windowsAutopilotDeploymentProfileAssignment 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 168616aa23934d5aa5e01d995cda533ed7d786e4
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792034"
---
# <a name="update-windowsautopilotdeploymentprofileassignment"></a><span data-ttu-id="de986-103">更新 windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="de986-103">Update windowsAutopilotDeploymentProfileAssignment</span></span>

<span data-ttu-id="de986-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="de986-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="de986-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="de986-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="de986-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="de986-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="de986-107">更新[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="de986-107">Update the properties of a [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="de986-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="de986-108">Prerequisites</span></span>
<span data-ttu-id="de986-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="de986-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="de986-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de986-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de986-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="de986-111">Permission type</span></span>|<span data-ttu-id="de986-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="de986-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="de986-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="de986-113">Delegated (work or school account)</span></span>|<span data-ttu-id="de986-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de986-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="de986-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="de986-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="de986-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="de986-116">Not supported.</span></span>|
|<span data-ttu-id="de986-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="de986-117">Application</span></span>|<span data-ttu-id="de986-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de986-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="de986-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="de986-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments/{windowsAutopilotDeploymentProfileAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="de986-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="de986-120">Request headers</span></span>
|<span data-ttu-id="de986-121">标头</span><span class="sxs-lookup"><span data-stu-id="de986-121">Header</span></span>|<span data-ttu-id="de986-122">值</span><span class="sxs-lookup"><span data-stu-id="de986-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="de986-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="de986-123">Authorization</span></span>|<span data-ttu-id="de986-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="de986-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="de986-125">接受</span><span class="sxs-lookup"><span data-stu-id="de986-125">Accept</span></span>|<span data-ttu-id="de986-126">application/json</span><span class="sxs-lookup"><span data-stu-id="de986-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="de986-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="de986-127">Request body</span></span>
<span data-ttu-id="de986-128">在请求正文中，提供[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="de986-128">In the request body, supply a JSON representation for the [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>

<span data-ttu-id="de986-129">下表显示创建[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="de986-129">The following table shows the properties that are required when you create the [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md).</span></span>

|<span data-ttu-id="de986-130">属性</span><span class="sxs-lookup"><span data-stu-id="de986-130">Property</span></span>|<span data-ttu-id="de986-131">类型</span><span class="sxs-lookup"><span data-stu-id="de986-131">Type</span></span>|<span data-ttu-id="de986-132">说明</span><span class="sxs-lookup"><span data-stu-id="de986-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de986-133">id</span><span class="sxs-lookup"><span data-stu-id="de986-133">id</span></span>|<span data-ttu-id="de986-134">String</span><span class="sxs-lookup"><span data-stu-id="de986-134">String</span></span>|<span data-ttu-id="de986-135">分配的键。</span><span class="sxs-lookup"><span data-stu-id="de986-135">The key of the assignment.</span></span>|
|<span data-ttu-id="de986-136">target</span><span class="sxs-lookup"><span data-stu-id="de986-136">target</span></span>|[<span data-ttu-id="de986-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="de986-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="de986-138">Windows Autopilot 部署配置文件的分配目标。</span><span class="sxs-lookup"><span data-stu-id="de986-138">The assignment target for the Windows Autopilot deployment profile.</span></span>|
|<span data-ttu-id="de986-139">source</span><span class="sxs-lookup"><span data-stu-id="de986-139">source</span></span>|[<span data-ttu-id="de986-140">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="de986-140">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="de986-141">用于部署到组、direct 或包裹/policySet 的资源类型。</span><span class="sxs-lookup"><span data-stu-id="de986-141">Type of resource used for deployment to a group, direct or parcel/policySet.</span></span> <span data-ttu-id="de986-142">可取值为：`direct`、`policySets`。</span><span class="sxs-lookup"><span data-stu-id="de986-142">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="de986-143">sourceId</span><span class="sxs-lookup"><span data-stu-id="de986-143">sourceId</span></span>|<span data-ttu-id="de986-144">String</span><span class="sxs-lookup"><span data-stu-id="de986-144">String</span></span>|<span data-ttu-id="de986-145">用于部署到组的资源的标识符</span><span class="sxs-lookup"><span data-stu-id="de986-145">Identifier for resource used for deployment to a group</span></span>|



## <a name="response"></a><span data-ttu-id="de986-146">响应</span><span class="sxs-lookup"><span data-stu-id="de986-146">Response</span></span>
<span data-ttu-id="de986-147">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="de986-147">If successful, this method returns a `200 OK` response code and an updated [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de986-148">示例</span><span class="sxs-lookup"><span data-stu-id="de986-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="de986-149">请求</span><span class="sxs-lookup"><span data-stu-id="de986-149">Request</span></span>
<span data-ttu-id="de986-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="de986-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments/{windowsAutopilotDeploymentProfileAssignmentId}
Content-type: application/json
Content-length: 411

{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeploymentProfileAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```

### <a name="response"></a><span data-ttu-id="de986-151">响应</span><span class="sxs-lookup"><span data-stu-id="de986-151">Response</span></span>
<span data-ttu-id="de986-152">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="de986-152">Here is an example of the response.</span></span> <span data-ttu-id="de986-153">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="de986-153">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="de986-154">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="de986-154">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 460

{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeploymentProfileAssignment",
  "id": "de7e1e1e-1e1e-de7e-1e1e-7ede1e1e7ede",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```



