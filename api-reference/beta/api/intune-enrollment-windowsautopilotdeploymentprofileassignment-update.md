---
title: 更新 windowsAutopilotDeploymentProfileAssignment
description: 更新 windowsAutopilotDeploymentProfileAssignment 对象的属性。
author: tfitzmac
ms.openlocfilehash: 74dda8d18468bf24030964a822b3d27a2a9d4451
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27346478"
---
# <a name="update-windowsautopilotdeploymentprofileassignment"></a><span data-ttu-id="4ecff-103">更新 windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="4ecff-103">Update windowsAutopilotDeploymentProfileAssignment</span></span>

> <span data-ttu-id="4ecff-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="4ecff-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4ecff-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="4ecff-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4ecff-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="4ecff-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4ecff-107">更新[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4ecff-107">Update the properties of a [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4ecff-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="4ecff-108">Prerequisites</span></span>
<span data-ttu-id="4ecff-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="4ecff-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ecff-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="4ecff-111">Permission type</span></span>|<span data-ttu-id="4ecff-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4ecff-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4ecff-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4ecff-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4ecff-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ecff-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="4ecff-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4ecff-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4ecff-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4ecff-116">Not supported.</span></span>|
|<span data-ttu-id="4ecff-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="4ecff-117">Application</span></span>|<span data-ttu-id="4ecff-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="4ecff-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4ecff-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4ecff-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments/{windowsAutopilotDeploymentProfileAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="4ecff-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="4ecff-120">Request headers</span></span>
|<span data-ttu-id="4ecff-121">标头</span><span class="sxs-lookup"><span data-stu-id="4ecff-121">Header</span></span>|<span data-ttu-id="4ecff-122">值</span><span class="sxs-lookup"><span data-stu-id="4ecff-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4ecff-123">授权</span><span class="sxs-lookup"><span data-stu-id="4ecff-123">Authorization</span></span>|<span data-ttu-id="4ecff-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4ecff-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4ecff-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4ecff-125">Accept</span></span>|<span data-ttu-id="4ecff-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4ecff-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4ecff-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="4ecff-127">Request body</span></span>
<span data-ttu-id="4ecff-128">在请求正文中，提供[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4ecff-128">In the request body, supply a JSON representation for the [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>

<span data-ttu-id="4ecff-129">下表显示时创建[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="4ecff-129">The following table shows the properties that are required when you create the [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md).</span></span>

|<span data-ttu-id="4ecff-130">属性</span><span class="sxs-lookup"><span data-stu-id="4ecff-130">Property</span></span>|<span data-ttu-id="4ecff-131">类型</span><span class="sxs-lookup"><span data-stu-id="4ecff-131">Type</span></span>|<span data-ttu-id="4ecff-132">说明</span><span class="sxs-lookup"><span data-stu-id="4ecff-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ecff-133">id</span><span class="sxs-lookup"><span data-stu-id="4ecff-133">id</span></span>|<span data-ttu-id="4ecff-134">String</span><span class="sxs-lookup"><span data-stu-id="4ecff-134">String</span></span>|<span data-ttu-id="4ecff-135">分配的键。</span><span class="sxs-lookup"><span data-stu-id="4ecff-135">The key of the assignment.</span></span>|
|<span data-ttu-id="4ecff-136">target</span><span class="sxs-lookup"><span data-stu-id="4ecff-136">target</span></span>|[<span data-ttu-id="4ecff-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="4ecff-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="4ecff-138">工作分配针对的 Windows 自动执行某些操作部署配置文件。</span><span class="sxs-lookup"><span data-stu-id="4ecff-138">The assignment target for the Windows Autopilot deployment profile.</span></span>|



## <a name="response"></a><span data-ttu-id="4ecff-139">响应</span><span class="sxs-lookup"><span data-stu-id="4ecff-139">Response</span></span>
<span data-ttu-id="4ecff-140">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4ecff-140">If successful, this method returns a `200 OK` response code and an updated [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ecff-141">示例</span><span class="sxs-lookup"><span data-stu-id="4ecff-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="4ecff-142">请求</span><span class="sxs-lookup"><span data-stu-id="4ecff-142">Request</span></span>
<span data-ttu-id="4ecff-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4ecff-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments/{windowsAutopilotDeploymentProfileAssignmentId}
Content-type: application/json
Content-length: 101

{
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="4ecff-144">响应</span><span class="sxs-lookup"><span data-stu-id="4ecff-144">Response</span></span>
<span data-ttu-id="4ecff-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4ecff-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 232

{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeploymentProfileAssignment",
  "id": "de7e1e1e-1e1e-de7e-1e1e-7ede1e1e7ede",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```





