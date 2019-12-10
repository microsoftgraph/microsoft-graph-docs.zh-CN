---
title: 创建 windowsAutopilotDeploymentProfileAssignment
description: 创建新的 windowsAutopilotDeploymentProfileAssignment 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4c4d467a4f3f601869903e702d50d7a08756246c
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39943752"
---
# <a name="create-windowsautopilotdeploymentprofileassignment"></a><span data-ttu-id="41d95-103">创建 windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="41d95-103">Create windowsAutopilotDeploymentProfileAssignment</span></span>

> <span data-ttu-id="41d95-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="41d95-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="41d95-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="41d95-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="41d95-106">创建新的[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="41d95-106">Create a new [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="41d95-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="41d95-107">Prerequisites</span></span>
<span data-ttu-id="41d95-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="41d95-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41d95-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="41d95-110">Permission type</span></span>|<span data-ttu-id="41d95-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="41d95-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="41d95-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="41d95-112">Delegated (work or school account)</span></span>|<span data-ttu-id="41d95-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41d95-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="41d95-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="41d95-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="41d95-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="41d95-115">Not supported.</span></span>|
|<span data-ttu-id="41d95-116">Application</span><span class="sxs-lookup"><span data-stu-id="41d95-116">Application</span></span>|<span data-ttu-id="41d95-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41d95-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="41d95-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="41d95-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments
```

## <a name="request-headers"></a><span data-ttu-id="41d95-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="41d95-119">Request headers</span></span>
|<span data-ttu-id="41d95-120">标头</span><span class="sxs-lookup"><span data-stu-id="41d95-120">Header</span></span>|<span data-ttu-id="41d95-121">值</span><span class="sxs-lookup"><span data-stu-id="41d95-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="41d95-122">授权</span><span class="sxs-lookup"><span data-stu-id="41d95-122">Authorization</span></span>|<span data-ttu-id="41d95-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="41d95-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="41d95-124">接受</span><span class="sxs-lookup"><span data-stu-id="41d95-124">Accept</span></span>|<span data-ttu-id="41d95-125">application/json</span><span class="sxs-lookup"><span data-stu-id="41d95-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="41d95-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="41d95-126">Request body</span></span>
<span data-ttu-id="41d95-127">在请求正文中，提供 windowsAutopilotDeploymentProfileAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="41d95-127">In the request body, supply a JSON representation for the windowsAutopilotDeploymentProfileAssignment object.</span></span>

<span data-ttu-id="41d95-128">下表显示创建 windowsAutopilotDeploymentProfileAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="41d95-128">The following table shows the properties that are required when you create the windowsAutopilotDeploymentProfileAssignment.</span></span>

|<span data-ttu-id="41d95-129">属性</span><span class="sxs-lookup"><span data-stu-id="41d95-129">Property</span></span>|<span data-ttu-id="41d95-130">类型</span><span class="sxs-lookup"><span data-stu-id="41d95-130">Type</span></span>|<span data-ttu-id="41d95-131">说明</span><span class="sxs-lookup"><span data-stu-id="41d95-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41d95-132">id</span><span class="sxs-lookup"><span data-stu-id="41d95-132">id</span></span>|<span data-ttu-id="41d95-133">字符串</span><span class="sxs-lookup"><span data-stu-id="41d95-133">String</span></span>|<span data-ttu-id="41d95-134">分配的键。</span><span class="sxs-lookup"><span data-stu-id="41d95-134">The key of the assignment.</span></span>|
|<span data-ttu-id="41d95-135">target</span><span class="sxs-lookup"><span data-stu-id="41d95-135">target</span></span>|[<span data-ttu-id="41d95-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="41d95-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="41d95-137">Windows Autopilot 部署配置文件的分配目标。</span><span class="sxs-lookup"><span data-stu-id="41d95-137">The assignment target for the Windows Autopilot deployment profile.</span></span>|
|<span data-ttu-id="41d95-138">source</span><span class="sxs-lookup"><span data-stu-id="41d95-138">source</span></span>|[<span data-ttu-id="41d95-139">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="41d95-139">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="41d95-140">用于部署到组、direct 或包裹/policySet 的资源类型。</span><span class="sxs-lookup"><span data-stu-id="41d95-140">Type of resource used for deployment to a group, direct or parcel/policySet.</span></span> <span data-ttu-id="41d95-141">可取值为：`direct`、`policySets`。</span><span class="sxs-lookup"><span data-stu-id="41d95-141">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="41d95-142">sourceId</span><span class="sxs-lookup"><span data-stu-id="41d95-142">sourceId</span></span>|<span data-ttu-id="41d95-143">字符串</span><span class="sxs-lookup"><span data-stu-id="41d95-143">String</span></span>|<span data-ttu-id="41d95-144">用于部署到组的资源的标识符</span><span class="sxs-lookup"><span data-stu-id="41d95-144">Identifier for resource used for deployment to a group</span></span>|



## <a name="response"></a><span data-ttu-id="41d95-145">响应</span><span class="sxs-lookup"><span data-stu-id="41d95-145">Response</span></span>
<span data-ttu-id="41d95-146">如果成功，此方法在响应`201 Created`正文中返回响应代码和[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="41d95-146">If successful, this method returns a `201 Created` response code and a [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41d95-147">示例</span><span class="sxs-lookup"><span data-stu-id="41d95-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="41d95-148">请求</span><span class="sxs-lookup"><span data-stu-id="41d95-148">Request</span></span>
<span data-ttu-id="41d95-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="41d95-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="41d95-150">响应</span><span class="sxs-lookup"><span data-stu-id="41d95-150">Response</span></span>
<span data-ttu-id="41d95-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="41d95-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





