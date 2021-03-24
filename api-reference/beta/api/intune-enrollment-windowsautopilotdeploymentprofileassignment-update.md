---
title: 更新 windowsAutopilotDeploymentProfileAssignment
description: 更新 windowsAutopilotDeploymentProfileAssignment 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2a29522f9d6141be5e2513e9a39f985c53de3306
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51142189"
---
# <a name="update-windowsautopilotdeploymentprofileassignment"></a><span data-ttu-id="bab55-103">更新 windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="bab55-103">Update windowsAutopilotDeploymentProfileAssignment</span></span>

<span data-ttu-id="bab55-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bab55-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bab55-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bab55-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bab55-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bab55-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bab55-107">更新 [windowsAutopilotDeploymentProfileAssignment 对象](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="bab55-107">Update the properties of a [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bab55-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="bab55-108">Prerequisites</span></span>
<span data-ttu-id="bab55-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bab55-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bab55-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="bab55-111">Permission type</span></span>|<span data-ttu-id="bab55-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bab55-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bab55-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bab55-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bab55-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bab55-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="bab55-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bab55-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bab55-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bab55-116">Not supported.</span></span>|
|<span data-ttu-id="bab55-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="bab55-117">Application</span></span>|<span data-ttu-id="bab55-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bab55-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bab55-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bab55-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments/{windowsAutopilotDeploymentProfileAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="bab55-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="bab55-120">Request headers</span></span>
|<span data-ttu-id="bab55-121">标头</span><span class="sxs-lookup"><span data-stu-id="bab55-121">Header</span></span>|<span data-ttu-id="bab55-122">值</span><span class="sxs-lookup"><span data-stu-id="bab55-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bab55-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bab55-123">Authorization</span></span>|<span data-ttu-id="bab55-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="bab55-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bab55-125">接受</span><span class="sxs-lookup"><span data-stu-id="bab55-125">Accept</span></span>|<span data-ttu-id="bab55-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bab55-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bab55-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="bab55-127">Request body</span></span>
<span data-ttu-id="bab55-128">在请求正文中，提供 [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bab55-128">In the request body, supply a JSON representation for the [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>

<span data-ttu-id="bab55-129">下表显示创建 [windowsAutopilotDeploymentProfileAssignment 时所需的属性](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="bab55-129">The following table shows the properties that are required when you create the [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md).</span></span>

|<span data-ttu-id="bab55-130">属性</span><span class="sxs-lookup"><span data-stu-id="bab55-130">Property</span></span>|<span data-ttu-id="bab55-131">类型</span><span class="sxs-lookup"><span data-stu-id="bab55-131">Type</span></span>|<span data-ttu-id="bab55-132">说明</span><span class="sxs-lookup"><span data-stu-id="bab55-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bab55-133">id</span><span class="sxs-lookup"><span data-stu-id="bab55-133">id</span></span>|<span data-ttu-id="bab55-134">String</span><span class="sxs-lookup"><span data-stu-id="bab55-134">String</span></span>|<span data-ttu-id="bab55-135">分配的键。</span><span class="sxs-lookup"><span data-stu-id="bab55-135">The key of the assignment.</span></span>|
|<span data-ttu-id="bab55-136">target</span><span class="sxs-lookup"><span data-stu-id="bab55-136">target</span></span>|[<span data-ttu-id="bab55-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="bab55-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="bab55-138">Windows Autopilot 部署配置文件的分配目标。</span><span class="sxs-lookup"><span data-stu-id="bab55-138">The assignment target for the Windows Autopilot deployment profile.</span></span>|
|<span data-ttu-id="bab55-139">source</span><span class="sxs-lookup"><span data-stu-id="bab55-139">source</span></span>|[<span data-ttu-id="bab55-140">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="bab55-140">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="bab55-141">用于部署到组、直接或直接/策略集的资源类型。</span><span class="sxs-lookup"><span data-stu-id="bab55-141">Type of resource used for deployment to a group, direct or parcel/policySet.</span></span> <span data-ttu-id="bab55-142">可取值为：`direct`、`policySets`。</span><span class="sxs-lookup"><span data-stu-id="bab55-142">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="bab55-143">sourceId</span><span class="sxs-lookup"><span data-stu-id="bab55-143">sourceId</span></span>|<span data-ttu-id="bab55-144">String</span><span class="sxs-lookup"><span data-stu-id="bab55-144">String</span></span>|<span data-ttu-id="bab55-145">用于部署到组的资源的标识符</span><span class="sxs-lookup"><span data-stu-id="bab55-145">Identifier for resource used for deployment to a group</span></span>|



## <a name="response"></a><span data-ttu-id="bab55-146">响应</span><span class="sxs-lookup"><span data-stu-id="bab55-146">Response</span></span>
<span data-ttu-id="bab55-147">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bab55-147">If successful, this method returns a `200 OK` response code and an updated [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bab55-148">示例</span><span class="sxs-lookup"><span data-stu-id="bab55-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="bab55-149">请求</span><span class="sxs-lookup"><span data-stu-id="bab55-149">Request</span></span>
<span data-ttu-id="bab55-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bab55-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="bab55-151">响应</span><span class="sxs-lookup"><span data-stu-id="bab55-151">Response</span></span>
<span data-ttu-id="bab55-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bab55-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




