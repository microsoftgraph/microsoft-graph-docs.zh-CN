---
title: 创建 windowsAutopilotDeploymentProfileAssignment
description: 创建新的 windowsAutopilotDeploymentProfileAssignment 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 545066786e2c896229bdf5f7327ba465c1b5f9f5
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43452495"
---
# <a name="create-windowsautopilotdeploymentprofileassignment"></a><span data-ttu-id="8b545-103">创建 windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="8b545-103">Create windowsAutopilotDeploymentProfileAssignment</span></span>

<span data-ttu-id="8b545-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8b545-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8b545-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8b545-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8b545-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8b545-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8b545-107">创建新的[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8b545-107">Create a new [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8b545-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="8b545-108">Prerequisites</span></span>
<span data-ttu-id="8b545-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8b545-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8b545-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="8b545-111">Permission type</span></span>|<span data-ttu-id="8b545-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8b545-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8b545-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8b545-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8b545-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b545-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="8b545-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8b545-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8b545-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8b545-116">Not supported.</span></span>|
|<span data-ttu-id="8b545-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="8b545-117">Application</span></span>|<span data-ttu-id="8b545-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b545-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8b545-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8b545-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments
```

## <a name="request-headers"></a><span data-ttu-id="8b545-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="8b545-120">Request headers</span></span>
|<span data-ttu-id="8b545-121">标头</span><span class="sxs-lookup"><span data-stu-id="8b545-121">Header</span></span>|<span data-ttu-id="8b545-122">值</span><span class="sxs-lookup"><span data-stu-id="8b545-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8b545-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8b545-123">Authorization</span></span>|<span data-ttu-id="8b545-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8b545-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8b545-125">接受</span><span class="sxs-lookup"><span data-stu-id="8b545-125">Accept</span></span>|<span data-ttu-id="8b545-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8b545-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8b545-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="8b545-127">Request body</span></span>
<span data-ttu-id="8b545-128">在请求正文中，提供 windowsAutopilotDeploymentProfileAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8b545-128">In the request body, supply a JSON representation for the windowsAutopilotDeploymentProfileAssignment object.</span></span>

<span data-ttu-id="8b545-129">下表显示创建 windowsAutopilotDeploymentProfileAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="8b545-129">The following table shows the properties that are required when you create the windowsAutopilotDeploymentProfileAssignment.</span></span>

|<span data-ttu-id="8b545-130">属性</span><span class="sxs-lookup"><span data-stu-id="8b545-130">Property</span></span>|<span data-ttu-id="8b545-131">类型</span><span class="sxs-lookup"><span data-stu-id="8b545-131">Type</span></span>|<span data-ttu-id="8b545-132">说明</span><span class="sxs-lookup"><span data-stu-id="8b545-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b545-133">id</span><span class="sxs-lookup"><span data-stu-id="8b545-133">id</span></span>|<span data-ttu-id="8b545-134">String</span><span class="sxs-lookup"><span data-stu-id="8b545-134">String</span></span>|<span data-ttu-id="8b545-135">分配的键。</span><span class="sxs-lookup"><span data-stu-id="8b545-135">The key of the assignment.</span></span>|
|<span data-ttu-id="8b545-136">target</span><span class="sxs-lookup"><span data-stu-id="8b545-136">target</span></span>|[<span data-ttu-id="8b545-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="8b545-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="8b545-138">Windows Autopilot 部署配置文件的分配目标。</span><span class="sxs-lookup"><span data-stu-id="8b545-138">The assignment target for the Windows Autopilot deployment profile.</span></span>|
|<span data-ttu-id="8b545-139">source</span><span class="sxs-lookup"><span data-stu-id="8b545-139">source</span></span>|[<span data-ttu-id="8b545-140">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="8b545-140">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="8b545-141">用于部署到组、direct 或包裹/policySet 的资源类型。</span><span class="sxs-lookup"><span data-stu-id="8b545-141">Type of resource used for deployment to a group, direct or parcel/policySet.</span></span> <span data-ttu-id="8b545-142">可取值为：`direct`、`policySets`。</span><span class="sxs-lookup"><span data-stu-id="8b545-142">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="8b545-143">sourceId</span><span class="sxs-lookup"><span data-stu-id="8b545-143">sourceId</span></span>|<span data-ttu-id="8b545-144">String</span><span class="sxs-lookup"><span data-stu-id="8b545-144">String</span></span>|<span data-ttu-id="8b545-145">用于部署到组的资源的标识符</span><span class="sxs-lookup"><span data-stu-id="8b545-145">Identifier for resource used for deployment to a group</span></span>|



## <a name="response"></a><span data-ttu-id="8b545-146">响应</span><span class="sxs-lookup"><span data-stu-id="8b545-146">Response</span></span>
<span data-ttu-id="8b545-147">如果成功，此方法在响应`201 Created`正文中返回响应代码和[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8b545-147">If successful, this method returns a `201 Created` response code and a [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8b545-148">示例</span><span class="sxs-lookup"><span data-stu-id="8b545-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="8b545-149">请求</span><span class="sxs-lookup"><span data-stu-id="8b545-149">Request</span></span>
<span data-ttu-id="8b545-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8b545-150">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments
Content-type: application/json
Content-length: 244

{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeploymentProfileAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```

### <a name="response"></a><span data-ttu-id="8b545-151">响应</span><span class="sxs-lookup"><span data-stu-id="8b545-151">Response</span></span>
<span data-ttu-id="8b545-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8b545-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 293

{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeploymentProfileAssignment",
  "id": "de7e1e1e-1e1e-de7e-1e1e-7ede1e1e7ede",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```



