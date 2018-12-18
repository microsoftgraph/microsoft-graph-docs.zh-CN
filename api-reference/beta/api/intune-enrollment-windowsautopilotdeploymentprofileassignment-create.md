---
title: 创建 windowsAutopilotDeploymentProfileAssignment
description: 创建新的 windowsAutopilotDeploymentProfileAssignment 对象。
author: tfitzmac
ms.openlocfilehash: c73cd0c8f32ea5b5e84afb5873700a6523186059
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27338848"
---
# <a name="create-windowsautopilotdeploymentprofileassignment"></a><span data-ttu-id="6896c-103">创建 windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="6896c-103">Create windowsAutopilotDeploymentProfileAssignment</span></span>

> <span data-ttu-id="6896c-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="6896c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6896c-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6896c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6896c-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="6896c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6896c-107">创建新的[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6896c-107">Create a new [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6896c-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="6896c-108">Prerequisites</span></span>
<span data-ttu-id="6896c-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="6896c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6896c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6896c-111">Permission type</span></span>|<span data-ttu-id="6896c-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6896c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6896c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6896c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6896c-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6896c-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6896c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6896c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6896c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6896c-116">Not supported.</span></span>|
|<span data-ttu-id="6896c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="6896c-117">Application</span></span>|<span data-ttu-id="6896c-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="6896c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6896c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6896c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments
```

## <a name="request-headers"></a><span data-ttu-id="6896c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6896c-120">Request headers</span></span>
|<span data-ttu-id="6896c-121">标头</span><span class="sxs-lookup"><span data-stu-id="6896c-121">Header</span></span>|<span data-ttu-id="6896c-122">值</span><span class="sxs-lookup"><span data-stu-id="6896c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6896c-123">授权</span><span class="sxs-lookup"><span data-stu-id="6896c-123">Authorization</span></span>|<span data-ttu-id="6896c-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6896c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6896c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6896c-125">Accept</span></span>|<span data-ttu-id="6896c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6896c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6896c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6896c-127">Request body</span></span>
<span data-ttu-id="6896c-128">在请求正文中，提供 windowsAutopilotDeploymentProfileAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6896c-128">In the request body, supply a JSON representation for the windowsAutopilotDeploymentProfileAssignment object.</span></span>

<span data-ttu-id="6896c-129">下表显示时创建 windowsAutopilotDeploymentProfileAssignment 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6896c-129">The following table shows the properties that are required when you create the windowsAutopilotDeploymentProfileAssignment.</span></span>

|<span data-ttu-id="6896c-130">属性</span><span class="sxs-lookup"><span data-stu-id="6896c-130">Property</span></span>|<span data-ttu-id="6896c-131">类型</span><span class="sxs-lookup"><span data-stu-id="6896c-131">Type</span></span>|<span data-ttu-id="6896c-132">说明</span><span class="sxs-lookup"><span data-stu-id="6896c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6896c-133">id</span><span class="sxs-lookup"><span data-stu-id="6896c-133">id</span></span>|<span data-ttu-id="6896c-134">String</span><span class="sxs-lookup"><span data-stu-id="6896c-134">String</span></span>|<span data-ttu-id="6896c-135">分配的键。</span><span class="sxs-lookup"><span data-stu-id="6896c-135">The key of the assignment.</span></span>|
|<span data-ttu-id="6896c-136">target</span><span class="sxs-lookup"><span data-stu-id="6896c-136">target</span></span>|[<span data-ttu-id="6896c-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="6896c-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="6896c-138">工作分配针对的 Windows 自动执行某些操作部署配置文件。</span><span class="sxs-lookup"><span data-stu-id="6896c-138">The assignment target for the Windows Autopilot deployment profile.</span></span>|



## <a name="response"></a><span data-ttu-id="6896c-139">响应</span><span class="sxs-lookup"><span data-stu-id="6896c-139">Response</span></span>
<span data-ttu-id="6896c-140">如果成功，此方法返回`201 Created`响应代码和响应正文中的[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6896c-140">If successful, this method returns a `201 Created` response code and a [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6896c-141">示例</span><span class="sxs-lookup"><span data-stu-id="6896c-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="6896c-142">请求</span><span class="sxs-lookup"><span data-stu-id="6896c-142">Request</span></span>
<span data-ttu-id="6896c-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6896c-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments
Content-type: application/json
Content-length: 183

{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeploymentProfileAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="6896c-144">响应</span><span class="sxs-lookup"><span data-stu-id="6896c-144">Response</span></span>
<span data-ttu-id="6896c-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6896c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





